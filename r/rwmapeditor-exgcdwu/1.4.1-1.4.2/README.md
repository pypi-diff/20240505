# Comparing `tmp/rwmapeditor_exgcdwu-1.4.1.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.4.1.tar", last modified: Tue Apr 30 14:09:26 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.4.2.tar", last modified: Sun May  5 06:28:23 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.4.1.tar` & `rwmapeditor_exgcdwu-1.4.2.tar`

### file list

```diff
@@ -1,320 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.018130 rwmapeditor_exgcdwu-1.4.1/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/otgroup_grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/otgroup_grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapText.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitAdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitRemove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_normal_unit_add.py
--rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_refresh_building.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/_troop_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_one_and_acti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_add_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.066130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.078131 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.078131 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-30 14:09:26.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitRemove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14198 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_normal_unit_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_refresh_building.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/_flash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/_troop_add.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/_victory_co.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_coo_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_matrix_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.591302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.603302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.603302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14028 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/LICENSE` & `rwmapeditor_exgcdwu-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.1
+Version: 1.4.2
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -688,14 +688,16 @@
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 [简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/Tutorial.md)
 
+【教程已过时】
+
 [简单城夺地图代码例子](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/examples/example1/example1.py)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
@@ -704,14 +706,16 @@
 
 基本框架已完成。
 
 地块组框架已完成。
 
 宾语组框架已完成。
 
+该版本为临时版本，尽量不要直接使用。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
@@ -731,7 +735,10 @@
 #### 4.即可使用python库改变地块和宾语
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
+
+文件中存在一些地块集模版，存放在rwmap/examples/template/，包括
+notTiled的v3模板，城夺地块集模板（来自Xs）
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/README.md` & `rwmapeditor_exgcdwu-1.4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 [简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/Tutorial.md)
 
+【教程已过时】
+
 [简单城夺地图代码例子](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/examples/example1/example1.py)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
@@ -18,14 +20,16 @@
 
 基本框架已完成。
 
 地块组框架已完成。
 
 宾语组框架已完成。
 
+该版本为临时版本，尽量不要直接使用。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
@@ -45,7 +49,10 @@
 #### 4.即可使用python库改变地块和宾语
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
+
+文件中存在一些地块集模版，存放在rwmap/examples/template/，包括
+notTiled的v3模板，城夺地块集模板（来自Xs）
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_layer.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,14 +21,19 @@
         self._compression = deepcopy(compression)
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
         properties = ElementProperties.init_etElement(root)
         data = utility.get_etElement_callable_from_tag_s(root, "data")
         _tilematrix = utility.get_etElement_ndarray_from_text_packed(data, frame.Coordinate(root.attrib['width'], root.attrib['height']))
         return cls(properties, _tilematrix, data.attrib["encoding"], data.attrib.get("compression"))
+    
+    @classmethod
+    def init_Layer(cls, property:frame.TagCoordinate, compression:str = "zlib")->None:
+        properties = ElementProperties("layer", {"name": property.tag(), "width": str(property.x()), "height": str(property.y())})
+        return cls(properties, np.zeros((property.y(), property.x()), dtype = np.uint32), "base64", compression)
 
     def output_str(self, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)))->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([" ".join([str(self._tilematrix[i][j]) for j in range(max(output_rectangle.i().y(), 0), min(output_rectangle.e().y(), self._tilematrix.shape[1]))]) + "\n"
                                  for i in range(max(output_rectangle.i().x(), 0), min(output_rectangle.e().x(), self._tilematrix.shape[0]))]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
@@ -47,21 +52,44 @@
         return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
                                 int(self._properties.returnDefaultProperty("height")))
 
     def __repr__(self)->str:
         return self.output_str()
 
     def id(self)->int:
-        return int(self._properties.default_properties["id"])
+        return int(self._properties.returnDefaultProperty("id"))
     
+    def changeid(self, id:int)->None:
+        self._properties.assignDefaultProperty("id", id)
+
+    def opacity(self)->float:
+        return float(self._properties.returnDefaultProperty("opacity"))
+    
+    def change_opacity(self, num:float)->None:
+        self._properties.assignDefaultProperty("opacity", f"{num:.2f}")
+
     def tileid(self, place_grid:frame.Coordinate)->int:
         return int(self._tilematrix[place_grid.x()][place_grid.y()])
     
     def assigntileid(self, place_grid:frame.Coordinate, tileid:int):
-        self._tilematrix[place_grid.y()][place_grid.x()] = tileid
+        size = self.size()
+        if place_grid.x() < 0 or place_grid.y() < 0 or place_grid.x() >= size.x() or place_grid.y() >= size.y():
+            return
+        self._tilematrix[place_grid.x()][place_grid.y()] = tileid
 
     def assigntileid_square(self, square_grid:frame.Rectangle, tileid:int):
-        self._tilematrix[square_grid.i().y():square_grid.e().y()][square_grid.i().x():square_grid.e().x()] = tileid
+        size = self.size()
+        self._tilematrix[max(0, square_grid.i().x()):min(size.x(), square_grid.e().x()), 
+        max(0, square_grid.i().y()):min(size.y(), square_grid.e().y())]\
+        = tileid
+
+    def assigntileid_squarematrix_exclude0(self, pos:frame.Coordinate, tileid_matrix:np.ndarray, tilerec:frame.Rectangle = None):
+        utility.save_matrix_exclude0(self._tilematrix, pos, tileid_matrix, tilerec)
+
+    def assigntileid_squarematrix(self, pos:frame.Coordinate, tileid_matrix:np.ndarray, tilerec:frame.Coordinate = None):
+        utility.save_matrix(self._tilematrix, pos, tileid_matrix, tilerec)
+        
+
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_objectgroup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,25 @@
 
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
         properties = ElementProperties.init_etElement(root)
         object_list = [TObject.init_etElement(tobject) for tobject in root if tobject.tag == "object"]
         return cls(properties, object_list)
     
+    @classmethod
+    def init_ObjectGroup(cls, name:str)->None:
+        properties = ElementProperties("objectgroup", {"name": "Triggers"})
+        return cls(properties, [])
+    
+    def id(self)->int:
+        return int(self._properties.returnDefaultProperty("id"))
+    
+    def changeid(self, id:int)->None:
+        self._properties.assignDefaultProperty("id", id)
+    
     def output_str(self, objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, min(len(self._object_list), objectnum))]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_tileset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 import xml.etree.ElementTree as et
 from copy import deepcopy
+import numpy as np
+import os
+import base64
 
 import rwmap._util as utility
 import rwmap._frame as frame
+import rwmap._data.const as const
 import rwmap._exceptions as exception
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
 
 class TileSet(ElementOri):
     def __init__(self, properties:ElementProperties, size:frame.Coordinate, image_properties:ElementProperties = None,
-                  png_text:str = None, tilelist_properties:list[ElementProperties] = None)->None:
+                  png_text:str = None, tilelist_properties:list[ElementProperties] = None, coo_to_tileid_matrix:np.ndarray = None, 
+                  tileid_to_coo_list:list[frame.Coordinate] = None)->None:
         super().__init__(properties)
         self._size = deepcopy(size)
         self._image_properties = deepcopy(image_properties)
         self._png_text = deepcopy(png_text)
         self._tilelist_properties = deepcopy(tilelist_properties)
+        self._coo_to_tileid_matrix = deepcopy(coo_to_tileid_matrix)
+        self._tileid_to_coo_list = deepcopy(tileid_to_coo_list)
     @classmethod
-    def init_etElement(cls, root:et.Element, rwmaps_dir:str)->None:
+    def init_etElement(cls, root:et.Element, rwmaps_dir:str, istilesort:bool = True)->None:
         png_text_pro = utility.get_etElement_callable_from_tag_s(root, "properties")
         png_text = utility.get_etElement_name_to_text_s(png_text_pro, "embedded_png")
         properties = ElementProperties.init_etElement(root)
         if png_text != None:
             properties.deleteOptionalProperty("embedded_png")
         image_properties = ElementProperties.init_etElement(utility.get_etElement_callable_from_tag_s(root, "image"))
         tilelist_properties = [ElementProperties.init_etElement(tile) for tile in root if tile.tag == "tile"]
         tilelist_properties = None if tilelist_properties == [] else tilelist_properties
         
+        if tilelist_properties != None and istilesort:
+            tilelist_properties.sort()
+
         if properties.returnDefaultProperty("columns") == None:
 
             source_file = properties.returnDefaultProperty("source")
             source_list = source_file.split("/")
             source_list = source_list[utility.search_list_to_index(source_list, "maps") + 1:]
             source_list = source_list[utility.search_list_to_index(source_list, "tilesets") + 1:]
             source_file = "/".join(source_list)
@@ -54,16 +64,53 @@
             else:
                 column = int(root.attrib["columns"])
                 row = int(int(root.attrib["tilecount"]) / column)
 
         else:
             column = int(properties.returnDefaultProperty("columns"))
             row = int(int(properties.returnDefaultProperty("tilecount")) / column)
+
         size = frame.Coordinate(row, column)
-        return cls(properties, size, image_properties, png_text, tilelist_properties)
+
+        coo_to_tileid_matrix = None
+        tileid_to_coo_list = None
+        
+        if tilelist_properties != None and (not istilesort):
+            has_pro_tileid = np.zeros([size.x(), size.y()], dtype = np.bool_)
+            pre = -1
+            isneed_matrix = False
+            
+            for tilenow in tilelist_properties:
+                tileid = int(tilenow.returnDefaultProperty("id"))
+                if tileid > pre:
+                    pre = tileid
+                else:
+                    isneed_matrix = True
+                coo = frame.Coordinate.init_id(tileid, size.y())
+                has_pro_tileid[coo.x(), coo.y()] = True
+            
+            if isneed_matrix:
+                coo_to_tileid_matrix = np.ndarray([size.x(), size.y()], dtype = np.uint32)
+                for coo in size:
+                    coo_to_tileid_matrix[coo.x(), coo.y()] = coo.id(size.y())
+
+                tileid_to_coo_list = list(range(size.x() * size.y()))
+                tilelist_index = 0
+                for coo in size:
+                    if has_pro_tileid[coo.x(), coo.y()]:
+                        coo_to_tileid_matrix[coo.x(), coo.y()] = \
+                            int(tilelist_properties[tilelist_index].returnDefaultProperty("id"))
+                        tilelist_index = tilelist_index + 1
+                
+                for coo in size:
+                    tileid_to_coo_list[coo_to_tileid_matrix[coo.x()][coo.y()]] = coo
+            
+        
+
+        return cls(properties, size, image_properties, png_text, tilelist_properties, coo_to_tileid_matrix, tileid_to_coo_list)
     
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         if self._image_properties != None:
             str_ans = str_ans + self._image_properties.output_str() + "\n"
         if self._png_text != None:
@@ -76,35 +123,47 @@
     
     def __repr__(self)->str:
         return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("tileset")
         root = self._properties.output_etElement(root)
-        if self._image_properties != None:
-            image_element = et.Element("image")
-            image_element = self._image_properties.output_etElement(image_element)
-            root.append(image_element)
         if self._png_text != None:
             png_element = et.Element("property", {"name": "embedded_png"})
             png_element.text = self._png_text
             properties = utility.get_etElement_callable_from_tag_s(root, "properties")
+            if properties == None:
+                properties = et.Element("properties")
+                root.append(properties)
             properties.insert(0, png_element)
+        if self._image_properties != None:
+            image_element = et.Element("image")
+            image_element = self._image_properties.output_etElement(image_element)
+            root.append(image_element)
         if self._tilelist_properties != None:
             for tile in self._tilelist_properties:
                 tile_element = et.Element("tile")
                 tile_element = tile.output_etElement(tile_element)
                 root.append(tile_element)
         return root
     
+    def write_png(self, dir:str)->None:
+        if self._image_properties != None:
+            pngbyte = base64.b64decode(self._png_text.encode('utf-8'))
+            file_path = dir + '/' + self._image_properties.returnDefaultProperty("source")
+            os.makedirs(os.path.dirname(file_path), exist_ok=True)
+            with open(file_path, 'wb') as file_now:
+                file_now.write(pngbyte)
+
+    
     def name(self)->str:
         tileset_name = self._properties.returnDefaultProperty("name")
         if tileset_name == None:
             tileset_name = self._properties.returnDefaultProperty("source")
-        tileset_name = utility.str_slash_to_dot(tileset_name)
+            tileset_name = utility.str_slash_to_dot(tileset_name)
         return tileset_name
     
     def totalgid(self)->int:
         return self._size.x() * self._size.y()
 
     def firstgid(self)->int:
         return int(self._properties.returnDefaultProperty("firstgid"))
@@ -120,33 +179,51 @@
         if tileid < 0:
             raise IndexError("The gid cannot be loaded into the current tileset.")
         return (self.name(), gid - self.firstgid())
     
     def tileid_to_gid(self, tileid:int)->int:
         return self.firstgid() + tileid
     
-    def tileid_to_coo(self, tileid:int)->frame.TagCoordinate:
+    def tileid_to_coo(self, tileid:int, isre:bool = True)->frame.TagCoordinate:
         if tileid < self.totalgid:
-            tagcoo = frame.TagCoordinate.init_id(self.name(), tileid, self._size.y())
+            if self._tileid_to_coo_list != None:
+                if isre:
+                    tagcoo = frame.TagCoordinate(self.name(), self._tileid_to_coo_list[tileid])
+                else:
+                    tagcoo = frame.TagCoordinate(self.name() + const.KEY.tag_for_tile_notre, self._tileid_to_coo_list[tileid])
+            else:
+                if isre:
+                    tagcoo = frame.TagCoordinate(self.name(), self._tileid_to_coo_list[tileid])
+                else:
+                    raise TypeError(f"tileid_to_coo:error transfromation")                    
         else:
             raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.name()}")
         return tagcoo
 
-    def coo_to_tileid(self, tile_grid:frame.Coordinate)->int:
+    def coo_to_tileid(self, tile_grid:frame.Coordinate, isre:bool = True)->int:
         if tile_grid < self._size:
-            id_ans = tile_grid.id(self._size.y())
+            if self._tileid_to_coo_list != None:
+                if isre:
+                    id_ans = int(self._coo_to_tileid_matrix[tile_grid.x(), tile_grid.y()])
+                else:
+                    id_ans = tile_grid.id(self._size.y())
+            else:
+                if isre:
+                    id_ans = tile_grid.id(self._size.y())
+                else:
+                    raise TypeError(f"coo_to_tileid:error transfromation")   
         else:
             raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.name()}")
         return id_ans
     
-    def coo_to_gid(self, tile_grid:frame.Coordinate)->int:
-        return self.coo_to_tileid(tile_grid) + self.firstgid()
+    def coo_to_gid(self, tile_grid:frame.Coordinate, isre:bool = True)->int:
+        return self.coo_to_tileid(tile_grid, isre = isre) + self.firstgid()
     
-    def gid_to_coo(self, gid:int)->frame.TagCoordinate:
-        return self.tileid_to_coo(self.gid_to_tileid(gid))
+    def gid_to_coo(self, gid:int, isre:bool = True)->frame.TagCoordinate:
+        return self.tileid_to_coo(self.gid_to_tileid(gid), isre = isre)
 
     def isexist(self)->bool:
-        return self._properties.returnDefaultProperty("firstgid") != "0"
+        return self._properties.returnDefaultProperty("firstgid") != const.KEY.empty_tile
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import xml.etree.ElementTree as et
 import re
 import os
 from copy import deepcopy
 from typing import Generator, Union
 from numbers import Integral
+import numpy as np
 
 import rwmap._exceptions as rwexceptions
 import rwmap._util as utility
 import rwmap._case as case
 import rwmap._frame as frame
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
@@ -21,43 +22,79 @@
 import rwmap._data.const as const
 
 
 RWMAP_DIR = os.path.dirname(__file__)
 RWMAP_MAPS = RWMAP_DIR + "/other_data/maps/"
 
 class RWmap(ElementOri):
+    pass
+
+class RWmap(ElementOri):
     def __init__(self, properties:ElementProperties, tileset_list:list[case.TileSet],
                   layer_list:list[case.Layer], objectGroup_list:list[case.ObjectGroup])->None:
         super().__init__(properties)
         self._tileset_list = deepcopy(tileset_list)
         self._layer_list = deepcopy(layer_list)
         self._objectGroup_list = deepcopy(objectGroup_list)
     @classmethod
     def init_mapfile(cls, map_file:str, rwmaps_dir = RWMAP_MAPS):
         xmlTree:et.ElementTree = et.ElementTree(file=map_file)
         root:et.Element = xmlTree.getroot()
         properties = ElementProperties.init_etElement(root)
 
-        tileset_list = [case.TileSet(ElementProperties("tileset", {"firstgid": "0", "name": "empty"}), frame.Coordinate(1, 1))]
+        tileset_list = [case.TileSet(ElementProperties("tileset", {"firstgid": const.KEY.empty_tile, "name": "empty"}), frame.Coordinate(1, 1))]
         tileset_list = tileset_list + [case.TileSet.init_etElement(tileset, rwmaps_dir) for tileset in root if tileset.tag == "tileset"]
         layer_list = [case.Layer.init_etElement(layer) for layer in root if layer.tag == "layer"]
         objectGroup_list = [case.ObjectGroup.init_etElement(objectGroup) for objectGroup in root if objectGroup.tag == "objectgroup"]  
         
         return cls(properties, tileset_list, layer_list, objectGroup_list)
 
+    @classmethod
+    def init_map(cls, size:frame.Coordinate, tile_size:frame.Coordinate = const.COO.SIZE_STANDARD):
+        properties = ElementProperties("map", \
+                                       {
+                                           "version": "1.10", 
+                                           "tiledversion": "1.10.2", 
+                                           "orientation": "orthogonal", 
+                                           "renderorder": "right-down", 
+                                           "width": str(size.x()), 
+                                           "height": str(size.y()), 
+                                           "tilewidth": str(tile_size.x()), 
+                                           "tileheight": str(tile_size.y()), 
+                                           "infinite": "0"
+                                       })
+        properties.assignDefaultProperty("nextlayerid", "1")
+        properties.assignDefaultProperty("nextobjectid", "1")
+        tileset_list = [case.TileSet(ElementProperties("tileset", {"firstgid": const.KEY.empty_tile, "name": "empty"}), frame.Coordinate(1, 1))]
+        layer_list = []
+        objectGroup_list = []
+        return cls(properties, tileset_list, layer_list, objectGroup_list)
+
     def size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
                                 int(self._properties.returnDefaultProperty("height")))
     
     def tile_size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._properties.returnDefaultProperty("tilewidth")), 
                                 int(self._properties.returnDefaultProperty("tileheight")))
     
+    def nextlayerid(self)->int:
+        return int(self._properties.returnDefaultProperty("nextlayerid"))
+    
+    def changenextlayerid(self, layerid:int)->None:
+        self._properties.assignDefaultProperty("nextlayerid", str(layerid))
+
+    def nextobjectid(self)->int:
+        return int(self._properties.returnDefaultProperty("nextobjectid"))
+    
+    def changenextobjectid(self, layerid:int)->None:
+        self._properties.assignDefaultProperty("nextobjectid", str(layerid))
+
     def tileset_name_list(self)->list[str]:
-        return [tileset.name() for tileset in self._tileset_list]
+        return [tileset.name() for tileset in self._tileset_list if tileset.isexist()]
     
     def layer_name_list(self)->list[str]:
         return [layer.name() for layer in self._layer_list]
     
     def objectgroup_name_list(self)->list[str]:
         return [objectgroup.name() for objectgroup in self._objectGroup_list]
     
@@ -75,20 +112,60 @@
         
     def get_objectgroup_s(self, name:str)->case.ObjectGroup:
         objectgroup = utility.get_ElementOri_from_list_by_name_s(self._objectGroup_list, name)
         if objectgroup == None:
             raise KeyError("objectgroup name:" + name + " not found")
         return objectgroup
     
-    def add_tileset(self, tileset:case.TileSet)->None:
+    def add_tileset_fromTileSet(self, tileset:case.TileSet)->None:
         tileset_n = deepcopy(tileset)
         firstgid = self._tileset_list[-1].endgid()
         tileset_n.changefirstgid(firstgid)
         self._tileset_list.append(tileset_n)
 
+    def add_tileset_fromMap(self, rwmap:RWmap)->None:
+        for tileset in rwmap._tileset_list:
+            if tileset.isexist():
+                self.add_tileset_fromTileSet(tileset)
+
+    def add_tileset_fromMapFile(self, map_file:str)->None:
+        rwmap = RWmap.init_mapfile(map_file)
+        self.add_tileset_fromMap(rwmap)
+
+    def add_layer(self, layername:str, compression:str = "default")->None:
+        if compression == "default":
+            if self._layer_list == []:
+                compression = "zlib"
+            else:
+                compression = self._layer_list[0]._compression
+        layer = case.Layer.init_Layer(frame.TagCoordinate(layername, self.size()), compression = compression)
+        self._layer_list.append(layer)
+
+    def add_Layer_fromLayer(self, layer:case.Layer)->None:
+        layer_n = deepcopy(layer)
+        layerid = self.nextlayerid()
+        self.changenextlayerid(layerid)
+        layer_n.changeid(layerid)
+        self._layer_list.append(layer_n)
+
+    def add_objectgroup(self, objectgroupname:str)->None:
+        objectgroup = case.ObjectGroup.init_ObjectGroup(objectgroupname)
+        self._objectGroup_list.append(objectgroup)
+
+    def add_objectgroup_fromObjectGroup(self, objectgroup:case.ObjectGroup)->None:
+        objectgroup_n = deepcopy(objectgroup)
+        layerid = int(self._properties.returnDefaultProperty("nextlayerid"))
+        self._properties.assignDefaultProperty("nextlayerid", str(layerid + 1))
+        objectgroup_n.changeid(layerid)
+        self._objectGroup_list.append(objectgroup_n)
+
+    def write_png(self, dir:str)->None:
+        for tileset in self._tileset_list:
+            tileset.write_png(dir)
+
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)), objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "\n".join([tileset.output_str(pngtextnum, tilenum) for tileset in self._tileset_list if tileset.isexist()]) + "\n"
         str_ans = str_ans + "\n".join([layer.output_str(output_rectangle) for layer in self._layer_list]) + "\n"
         str_ans = str_ans + "\n".join([tobject.output_str(objectnum) for tobject in self._objectGroup_list]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
@@ -168,15 +245,21 @@
     
     def _tileplace_to_gid(self, tileplace:Union[int, tuple[str, int], frame.TagCoordinate])->int:
         if isinstance(tileplace, int):
             tileplace_now = tileplace
         elif isinstance(tileplace, tuple) and isinstance(tileplace[0], str) and isinstance(tileplace[1], int):
             tileplace_now = self.get_tileset_s(tileplace[0]).tileid_to_gid(tileplace[1])
         elif isinstance(tileplace, frame.TagCoordinate):
-            tileplace_now = self.get_tileset_s(tileplace.tag()).coo_to_gid(tileplace.place())
+            if tileplace.tag()[-1] == const.KEY.tag_for_tile_notre:
+                tileset = self.get_tileset_s(tileplace.tag()[:-1])
+                isre = False
+            else:
+                tileset = self.get_tileset_s(tileplace.tag())
+                isre = True
+            tileplace_now = tileset.coo_to_gid(tileplace.place(), isre = isre)
         else:
             raise TypeError("The type of RWmap.addTile(..., tileplace) is wrong.")
         return tileplace_now
 
     def addTile_gid(self, layerplace:frame.TagCoordinate, gid:int):
         if gid >= 0 and isinstance(gid, Integral):
             layer:case.Layer = self.get_layer_s(layerplace.tag())
@@ -189,24 +272,38 @@
         self.addTile_gid(layerplace, tileplace_now)
 
     def addTile_square(self, layerRectangle:frame.TagRectangle, tileplace:Union[int, tuple[str, int], frame.TagCoordinate])->None:
         tileplace_now = self._tileplace_to_gid(tileplace)
         layer:case.Layer = self.get_layer_s(layerRectangle.tag())
         layer.assigntileid_square(layerRectangle.rectangle(), tileplace_now)
 
-    def addTile_group(self, tilegroup:tile.TileGroup_One, original_grid:frame.Coordinate):
-        for place_grid in tilegroup.size():
-            layerplace = frame.TagCoordinate(tilegroup.layername(), original_grid + place_grid)
-            tileplace = tilegroup[place_grid]
-            if tileplace.tag() != "empty":
-                self.addTile(layerplace, tileplace)
+    def addTile_group(self, tilegroup:tile.TileGroup_One, original_grid:frame.Coordinate, rect_execute:frame.Rectangle = None, isacce = False):
+        if rect_execute == None:
+            range_excute = frame.Rectangle(frame.Coordinate(0, 0), tilegroup.size())
+        else:
+            range_excute = rect_execute
+        
+        selfid = str(id(self))
+
+        gidmatrix = tilegroup.get_acce_s(selfid)
+        if type(gidmatrix) != np.ndarray:
+            gidmatrix = np.ndarray([tilegroup.size().x(), tilegroup.size().y()], dtype = np.uint32)
+            for place_grid in tilegroup.size():
+                gidmatrix[place_grid.x(), place_grid.y()] = self._tileplace_to_gid(tilegroup[place_grid])
+        
+        layer_s = self.get_layer_s(tilegroup.layername())
+        
+        layer_s.assigntileid_squarematrix_exclude0(original_grid, gidmatrix, range_excute)
+        if isacce:
+            if type(tilegroup.get_acce_s(selfid)) != np.ndarray:
+                tilegroup.save_acce_s(selfid, gidmatrix)
 
-    def addTile_group_list(self, tilegroup_list:tile.TileGroup_List, original_grid:frame.Coordinate):
+    def addTile_group_list(self, tilegroup_list:tile.TileGroup_List, original_grid:frame.Coordinate, rect_execute:frame.Rectangle = None):
         for tilegroup in tilegroup_list:
-            self.addTile_group(tilegroup, original_grid)
+            self.addTile_group(tilegroup, original_grid, rect_execute)
 
     def addOTGroup(self, otgroup:otgroup.OTGroup, offset_grid:frame.Coordinate = frame.Coordinate()):
         self.addTile_group_list(otgroup._tilegroup_list, offset_grid)
         self.addObject_group(otgroup._tobject_group, offset_grid * self.tile_size())
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_credit.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapText.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
-class Credit(object.TObject_One):
-    def __init__(self, pos:frame.Coordinate, team:int, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
-                 setCredits:int = None, addCredits:int = None, name:str = None, warmup:int = -1, 
-                 reset:int = -1, actiBy_s:list[object.TObject_One] = [], 
-                 deactiBy_s:list[object.TObject_One] = [], isalltoacti:bool = False):
-        upos = frame.Rectangle(pos - size / 2, size)
-        object.TObject_One.__init__(self, object.TObject_Type.init_changeCredits(team, setCredits = setCredits, addCredits = addCredits), 
+class MapText(object.TObject_One):
+    def __init__(self, pos:frame.Coordinate, text:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
+                 textColor:str = None, textSize:int = -1, name:str = None,
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
+                 isalltoacti:bool = False, reset:int = 1):
+        upos = frame.Rectangle(pos, size)
+        object.TObject_One.__init__(self, object.TObject_Type.init_mapText(text, textColor = textColor, textSize = textSize), 
                                     object.TObject_Pos.init_rectangle(upos), name, 
                                     object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
-                                    object.TObject_Time.init_time(warmup = warmup, reset = reset))
+                                    object.TObject_Time.init_time(reset = reset))
+
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapText.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
-class MapText(object.TObject_One):
-    def __init__(self, pos:frame.Coordinate, text:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
-                 textColor:str = None, textSize:int = -1, name:str = None,
-                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
-                 isalltoacti:bool = False, reset:int = 1):
-        upos = frame.Rectangle(pos - size / 2, size)
-        object.TObject_One.__init__(self, object.TObject_Type.init_mapText(text, textColor = textColor, textSize = textSize), 
-                                    object.TObject_Pos.init_rectangle(upos), name, 
-                                    object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
-                                    object.TObject_Time.init_time(reset = reset))
+from rwmap._object._object_time import _make_tobject_time
 
+class Node(object.TObject_One):
+    def __init__(self, pos:frame.Coordinate, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
+                 name:str = None, warmup:int = -1, reset:int = -1, 
+                 isdelay:bool = False, isrepeat:bool = False, 
+                 id:str = None, alsoacti_s:list[object.TObject_One] = [], 
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
+                 isalltoacti:bool = False):
+        upos = frame.Rectangle(pos, size)
+        object.TObject_One.__init__(self, object.TObject_Type.init_node(), 
+                                    object.TObject_Pos.init_rectangle(upos), 
+                                    name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s, 
+                                                                        actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, 
+                                                                        isalltoacti = isalltoacti), 
+                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapinfo.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapinfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class Mapinfo(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, mapType:str, mapFog:str, 
                  winCondition:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  text:str = None):
-        upos = frame.Rectangle(pos - size / 2, size)
+        upos = frame.Rectangle(pos, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_mapinfo(mapType = mapType, mapFog = mapFog, 
                                                                            winCondition = winCondition, text = text), 
                                     object.TObject_Pos.init_rectangle(upos))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_message.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
+from rwmap._object._object_time import _make_tobject_time
+
 class Message(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, message:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  delayPerChar:int = -1, textColor:str = None, 
                  name:str = None, warmup:int = -1, reset:int = -1, 
+                 isdelay:bool = False, isrepeat:bool = False, 
                  actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
                  isalltoacti:bool = False):
-        upos = frame.Rectangle(pos - size / 2, size)
+        upos = frame.Rectangle(pos, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_mapText(None), 
                                     object.TObject_Pos.init_rectangle(upos), 
                                     name, object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
-                                    object.TObject_Time.init_time(warmup = warmup, reset = reset), 
+                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat), 
                                     object.TObject_Global.init_global(message = message, 
                                                                       delayPerChar = delayPerChar, textColor = textColor))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_node.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitRemove.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import rwmap._object as object
 import rwmap._frame as frame
-import rwmap._data.const as const
 
-class Node(object.TObject_One):
-    def __init__(self, pos:frame.Coordinate, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
-                 name:str = None, warmup:int = -1, reset:int = -1, 
-                 id:str = None, alsoacti_s:list[object.TObject_One] = [], 
-                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
-                 isalltoacti:bool = False):
-        upos = frame.Rectangle(pos - size / 2, size)
-        object.TObject_One.__init__(self, object.TObject_Type.init_node(), 
+from rwmap._object._object_time import _make_tobject_time
+
+class UnitRemove(object.TObject_One):
+    def __init__(self, pos:frame.Coordinate, size:frame.Coordinate, name:str = None, team:int = None, 
+               warmup:int = -1, reset:int = -1, 
+               isdelay:bool = False, isrepeat:bool = False, actiBy_s:list[object.TObject_One] = [], 
+               deactiBy_s:list[object.TObject_One] = [], isalltoacti:bool = False):
+        upos = frame.Rectangle(pos, size)
+        object.TObject_One.__init__(self, object.TObject_Type.init_unitRemove(team), 
                                     object.TObject_Pos.init_rectangle(upos), 
-                                    name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s, 
-                                                                        actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, 
-                                                                        isalltoacti = isalltoacti), 
-                                    object.TObject_Time.init_time(warmup = warmup, reset = reset))
+                                    name, object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
+                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitDetect.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitDetect.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
+from rwmap._object._object_time import _make_tobject_time
+
 class UnitDetect(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, size:frame.Coordinate, name:str = None,
                  team:int = None, minUnits:int = None, maxUnits:int = None, 
                  unitType:str = None, onlyList:list[str] = [], warmup:int = -1, reset:int = -1, 
+                 isdelay:bool = False, isrepeat:bool = False, 
                  id:str = None, alsoacti_s:list[object.TObject_One] = []):
-        upos = frame.Rectangle(pos - size / 2, size)
+        upos = frame.Rectangle(pos, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_unitDetect(team = team, minUnits = minUnits, maxUnits = maxUnits, 
                                                                               unitType = unitType, onlyList = onlyList), 
                                     object.TObject_Pos.init_rectangle(upos), 
                                     name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s), 
-                                    object.TObject_Time.init_time(warmup = warmup, reset = reset))
+                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/__init__.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 from rwmap._data.tobject_group._city._city import City, CityNoTeam, CityAllTeam, CityAllTeamGroup
 from rwmap._data.tobject_group._city._refresh_building import RefreshBuilding, RefreshBuildingNoTeam, RefreshBuildingAllTeam, RefreshBuildingAllTeamGroup
 from rwmap._data.tobject_group._city._city_detect import BuildingDetect, BuildingDetectNoTeam, BuildingDetectAllTeam, BuildingDetectAllTeamGroup
 from rwmap._data.tobject_group._city._city_text import CityText, CityTextNoTeam, CityTextAllTeam
 from rwmap._data.tobject_group._city._normal_unit_add import NormalUnitAdd, NormalUnitAddInstant
+from rwmap._data.tobject_group._city._city_remove import unitRemoveAllTeam
 from rwmap._data.tobject_group._troop._troop_add import RefreshTroop
+from rwmap._data.tobject_group._count._flash import Flash
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
                     raise IndexError("The number of city text is less.")
                 if building_s._is_detect_acti_add:
                     citytext.maptext(textindex).add_deactiBy_s(building_s.idTObject_s_index(index))
                 else:
                     citytext.maptext(textindex).add_actiBy_s(building_s.idTObject_s_index(index))
         self._TObject_Group_list.append(citytext)
     
+    def cityText_s(self)->city_text.CityText:
+        return self._TObject_Group_list[2]
+
     @classmethod
     def init_adt(cls, uadd_s:city_add.NormalUnitAdd, udetect_s:city_detect.BuildingDetect, 
                  citytext:city_text.CityText, is_detect_acti_add:bool = True, 
                  detect_to_text:list[int] = None):
         building_s = refresh_building.RefreshBuilding(uadd_s, udetect_s, 
                                                       is_detect_acti_add = is_detect_acti_add)
         return cls(building_s, citytext, detect_to_text)
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_detect.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_detect.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     
     def idTObject_s_team(self, team:Union[int, None])->Union[object.TObject_One, None]:
         team = str(team) if isinstance(team, int) else team
         for tobject in self._TObject_One_list:
             if tobject._otype.output_optional_properties().get("team") == team:
                 return tobject.idTObject_s()
         return None
+    
+    def idTObject_s_team_list(self, team_list:list[Union[int, None]])->list[Union[object.TObject_One, None]]:
+        return [self.idTObject_s_team(team) for team in team_list]
 
     def pos(self)->frame.Coordinate:
         return self.idTObject_s_index(0)._pos.pos()
 
     def size(self)->frame.Coordinate:
         return self.idTObject_s_index(0)._pos.size()
     
@@ -78,20 +81,17 @@
         teamlist = list(range(teamnum)) + [None]
         name_list = name_list + [f'{name}'] if name != None else []
         
         BuildingDetect.__init__(self, pos, id_list, warmup, reset, size = size, 
                               unitType_andob = unitType_andob, name = name_list, 
                               team = teamlist, minUnits = minUnits, 
                               maxUnits = maxUnits)
-
-    def idTObject_s_list(self, teamlist:list[int])->list[object.TObject_One]:
-        return [self.idTObject_s_index(team) for team in teamlist]
     
     def idTObject_s_team_list(self, teamnow:int, teamgroupnum:int = 2)->list[object.TObject_One]:
-        return self.idTObject_s_list([team for team in range(len(self._TObject_One_list))
+        return self.idTObject_s_team_list([team for team in range(len(self._TObject_One_list))
                                              if team % teamgroupnum == teamnow])
     
     def idTObject_s_id(self, id:str)->list[object.TObject_One]:
         return [self.idTObject_s_index(index) for index in range(len(self._TObject_One_list))
                 if self.idTObject_s_index(index)._name == id]
 
 class BuildingDetectAllTeamGroup(BuildingDetectAllTeam):
@@ -103,8 +103,11 @@
         self._teamgroup = teamgroup
         id_group = [team % teamgroup for team in range(teamnum)]  if isacti_accu else []
         BuildingDetectAllTeam.__init__(self, pos, id, teamnum, warmup, reset, size = size, 
                                        unitType_andob = unitType_andob, name = name, 
                                        id_group = id_group, minUnits = minUnits, maxUnits = maxUnits)
         
     def group(self)->int:
-        return self._teamgroup
+        return self._teamgroup
+    
+    def team_list(self, teamgroupnow:int)->list[int]:
+        return [team for team in range(self.length()) if team % self._teamgroup == teamgroupnow]
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_text.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_text.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_normal_unit_add.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_normal_unit_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_refresh_building.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_refresh_building.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,14 @@
 class RefreshBuilding(object.TObject_Group):
     pass
 
 class RefreshBuilding(object.TObject_Group):
     def __init__(self, uadd_s:city_add.NormalUnitAdd, udetect_s:city_detect.BuildingDetect, 
                  is_detect_acti_add:bool = True):
         self._is_detect_acti_add = is_detect_acti_add
-        udetect_s._TObject_Group_list
-        udetect_s._TObject_One_list
         toba = udetect_s.idTObject_s_team(None)
         if is_detect_acti_add:
             uadd_s.add_actiBy_s(toba)
         else:
             uadd_s.add_deactiBy_s(toba)
         object.TObject_Group.__init__(self, [], [uadd_s, udetect_s])
     
@@ -172,14 +170,17 @@
 
     def idTObject_s_index(self, index:int)->object.TObject_One:
         return self.unitDetect_s().idTObject_s_index(index)
     
     def idTObject_s_team(self, team:Union[int, None])->Union[object.TObject_One, None]:
         return self.unitDetect_s().idTObject_s_team(team)
     
+    def idTObject_s_team_list(self, team_list:list[Union[int, None]])->list[Union[object.TObject_One, None]]:
+        return [self.unitDetect_s().idTObject_s_team(team) for team in team_list]
+    
 class RefreshBuildingNoTeam(RefreshBuilding):
     def __init__(self, uadd_s:city_add.NormalUnitAdd, udetect_s:city_detect.BuildingDetectNoTeam, 
                  is_detect_acti_add:bool = True):
         RefreshBuilding.__init__(self, uadd_s, udetect_s, is_detect_acti_add)
     
     @classmethod
     def init_base(cls, pos:frame.Coordinate, id:str, units:str,
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/_troop_add.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/_troop_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_coordinate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from copy import deepcopy
 import math
 
 import rwmap._exceptions as rwexceptions
 
 class Coordinate:
+    pass
+
+class Coordinate:
     
     def __init__(self, x:int = 0, y:int = 0, dtype:str = np.int32):
         self._content = np.array([[0], [0]], dtype=dtype)
         self._content[0][0] = x
         self._content[1][0] = y
 
     @classmethod
@@ -26,20 +29,23 @@
         return deepcopy(self._content[0][0])
 
     def y(self):
         return deepcopy(self._content[1][0])
     
     def id(self, width:int)->int:
         return int(self.x() * width + self.y())
+    
+    def transpose(self)->Coordinate:
+        return Coordinate(self.y(), self.x(), self._content.dtype)
 
     def __add__(self, other):
         if isinstance(other, Coordinate):
-            return Coordinate(self.x() + other.x(), self.y() + other.y())
+            return Coordinate(self.x() + other.x(), self.y() + other.y(), self._content.dtype)
         else:
-            return Coordinate(other + self.x(), other + self.y())
+            return Coordinate(other + self.x(), other + self.y(), self._content.dtype)
 
     def __mul__(self, other):
         ans = Coordinate(0, 0)
         if isinstance(other, Coordinate):
             new_content = other._content * self._content
         elif isinstance(other, np.matrix) or (isinstance(other, np.ndarray) and other.ndim == 2):
             new_content = other @ self._content
@@ -58,60 +64,89 @@
         return ans
     
     def __floordiv__(self, other):
         return self.__truediv__(other)
     
     def __sub__(self, other):
         if isinstance(other, Coordinate):
-            return Coordinate(self.x() - other.x(), self.y() - other.y())
+            return Coordinate(self.x() - other.x(), self.y() - other.y(), self._content.dtype)
         else:
-            return Coordinate(self.x() - other, self.y() - other)
+            return Coordinate(self.x() - other, self.y() - other, self._content.dtype)
 
     def __neg__(self):
-        return Coordinate(-self.x(), -self.y())
+        return Coordinate(-self.x(), -self.y(), self._content.dtype)
     
     def _iterator(self):
         for i in range(0, self.x()):
             for j in range(0, self.y()):
-                yield Coordinate(i, j)
+                yield Coordinate(i, j, self._content.dtype)
 
     def __iter__(self):
         return self._iterator()
     
     def __lt__(self, other)->int:
         if self.x() < other.x() and self.y() < other.y():
             return 1
         elif self.x() > other.x() and self.y() > other.y():
             return -1
         else:
             return 0
     
 class Rectangle:
+    pass
+
+class Rectangle:
     def __init__(self, initialCoordinate:Coordinate, addCoordinate:Coordinate):
-        self._initialCoordinate = initialCoordinate
-        self._addCoordinate = addCoordinate
+        self._initialCoordinate = deepcopy(initialCoordinate)
+        self._addCoordinate = deepcopy(addCoordinate)
     
     def i(self):
         return deepcopy(self._initialCoordinate)
 
     def a(self):
         return deepcopy(self._addCoordinate)
     
     def e(self):
         return deepcopy(self._initialCoordinate + self._addCoordinate)
     
+    def transpose(self)->Rectangle:
+        return Rectangle(self._initialCoordinate.transpose(), self._addCoordinate.transpose())
+    
+    @classmethod
+    def init_ae(cls, initialCoordinate:Coordinate, endCoordinate:Coordinate):
+        addCoordinate = endCoordinate - initialCoordinate
+        return cls(initialCoordinate, addCoordinate)
+
     def _iterator(self):
         for i in range(0, self._addCoordinate.x()):
             for j in range(0, self._addCoordinate.y()):
                 coordinate_now = self._initialCoordinate + Coordinate(i, j)
                 yield Coordinate(coordinate_now.x(), coordinate_now.y())
 
     def __iter__(self):
         return self._iterator()
     
+    def __add__(self, other):
+        if isinstance(other, Rectangle):
+            return Rectangle(self._addCoordinate + other._addCoordinate, self._initialCoordinate + other._initialCoordinate)
+        elif isinstance(other, Coordinate):
+            return Rectangle(self._initialCoordinate, self._addCoordinate + other)
+    
+    def __sub__(self, other):
+        if isinstance(other, Rectangle):
+            return Rectangle(self._initialCoordinate - other._initialCoordinate, self._addCoordinate - other._addCoordinate)
+        elif isinstance(other, Coordinate):
+            return Rectangle(self._initialCoordinate, self._addCoordinate - other)
+
+    def __neg__(self):
+        return Rectangle(-self._initialCoordinate, -self._addCoordinate)
+    
+class TagCoordinate(Coordinate):
+    pass
+
 class TagCoordinate(Coordinate):
     def __init__(self, tag:str, place:Coordinate):
         self.__dict__ = deepcopy(place.__dict__)
         self._tag = tag
 
     @classmethod
     def init_xy(cls, tag:str, x = 0, y = 0, dtype:str = np.int32):
@@ -127,25 +162,56 @@
 
     def tag(self):
         return self._tag
     
     def place(self):
         return Coordinate.init_np(self._content)
     
+    def transpose(self)->TagCoordinate:
+        return TagCoordinate(self._tag, Coordinate.transpose(self))
+    
+    def __add__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__add__(self, other))
+
+    def __mul__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__mul__(self, other))
+    
+    def __truediv__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__truediv__(self, other))
+    
+    def __floordiv__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__floordiv__(self, other))
+    
+    def __sub__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__sub__(self, other))
+
+    def __neg__(self, other):
+        return TagCoordinate(deepcopy(self._tag), Coordinate.__neg__(self, other))
+    
+    def _iterator(self):
+        for coo in Coordinate._iterator(self):
+            yield TagCoordinate(deepcopy(self._tag), coo)
+    
+class TagRectangle(Rectangle):
+    pass
+
 class TagRectangle(Rectangle):
     def __init__(self, tag:str, place:Rectangle):
         self._initialCoordinate = deepcopy(place._initialCoordinate)
         self._addCoordinate = deepcopy(place._addCoordinate)
         self._tag = tag
 
     def tag(self)->str:
         return self._tag
     
     def rectangle(self)->Rectangle:
         return Rectangle(deepcopy(self._initialCoordinate), deepcopy(self._addCoordinate))
+    
+    def transpose(self)->TagRectangle:
+        return TagRectangle(self._tag, Rectangle.transpose(self))
 
     def i(self):
         return TagCoordinate(self._tag, deepcopy(self._initialCoordinate))
 
     def a(self):
         return TagCoordinate(self._tag, deepcopy(self._addCoordinate))
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import xml.etree.ElementTree as et
 from copy import deepcopy
 from typing import Union
 
 import rwmap._util as utility
 
 class ElementProperties:
+    pass
+
+class ElementProperties:
     def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, Union[str, dict[str, str]]] = {})->None:
         self._tag = tag
         self._default_properties = deepcopy(default_properties)
         self._optional_properties = deepcopy(optional_properties)
         
     @classmethod
     def init_etElement(cls, root:et.Element):
@@ -30,24 +33,28 @@
         str_ans = ""
         str_ans = str_ans + self._tag + ":\n"
         str_ans = str_ans + "default_properties:" + str(self._default_properties) + "\n"
         str_ans = str_ans + "optional_properties:" + str(self._optional_properties) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
     
+    def __lt__(self, other:ElementProperties)->bool:
+        return int(self.returnDefaultProperty("id")) < int(other.returnDefaultProperty("id"))
+
     def assignDefaultProperty(self, name:str, value:Union[str, dict[str, str]]):
         self._default_properties[name] = value
     
     def assignOptionalProperty(self, name:str, value:Union[str, dict[str, str]]):
         self._optional_properties[name] = value
 
     def returnDefaultProperty(self, name:str)->Union[str, dict[str, str]]:
-        return self._default_properties.get(name)
+        return deepcopy(self._default_properties.get(name))
     
     def returnOptionalProperty(self, name:str)->Union[str, dict[str, str]]:
-        return self._optional_properties.get(name)
+        return deepcopy(self._optional_properties.get(name))
     
     def deleteDefaultProperty(self, name:str)->None:
         self._default_properties.pop(name)
     
     def deleteOptionalProperty(self, name:str)->None:
-        self._optional_properties.pop(name)
+        self._optional_properties.pop(name)
+
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_global.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_global.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_group.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_one_and_acti.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_one_and_acti.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_pos.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import xml.etree.ElementTree as et
 from copy import deepcopy
 
 import rwmap._frame as frame
+import rwmap._util as utility
 
 class TObject_Pos:
     pass
 
 class TObject_Pos:
     def __init__(self, default_properties:dict[str, str], other_properties:list[et.Element] = {}):
         self._default_properties = deepcopy(default_properties)
@@ -13,21 +14,28 @@
 
     @classmethod
     def init_rectangle(cls, rect:frame.Rectangle):
         default_properties = {"x": f"{rect.i().x():.0f}", "y": f"{rect.i().y():.0f}", 
                               "width": f"{rect.a().x():.0f}", "height": f"{rect.a().y():.0f}"}
         return cls(default_properties)
     
+    @classmethod
+    def init_polygon(cls, point_list:list[frame.Coordinate], midpos:frame.Coordinate):
+        default_properties = {"x": f"{midpos.x():.0f}", "y": f"{midpos.y():.0f}"}
+        point_list_str = utility.point_list_to_str(point_list)
+        other_properties = [et.Element("polygon", {"points": point_list_str})]
+        return cls(default_properties, other_properties)
+
     def size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._default_properties["width"]),
                                 int(self._default_properties["height"]))
     
     def pos(self)->frame.Coordinate:
-        return frame.Coordinate(int(self._default_properties["x"]) + int(self._default_properties["width"]) / 2,
-                                int(self._default_properties["y"]) + int(self._default_properties["height"]) / 2)
+        return frame.Coordinate(int(self._default_properties["x"]),
+                                int(self._default_properties["y"]))
     
     def rectangle(self)->frame.Rectangle:
         return frame.Rectangle(self.pos(), self.size())
 
     def output_default_properties(self):
         return deepcopy(self._default_properties)
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_type.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_type.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/_tile_group.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,76 @@
 import numpy as np
 from copy import deepcopy
 from typing import Union
 
 import rwmap._frame as frame
+import rwmap._data.const as const
 import rwmap._util as utility
 from rwmap._exceptions import KeyConflictError
 from rwmap._data.const import TYPE
 
 tilestate_type = "S20"
 
 class TileGroup_Matrix:
-    def __init__(self, tilename_matrix):
+    pass
+
+class TileGroup_Matrix:
+    def __init__(self, tilename_matrix:list[list]):
         self._tilematrix = deepcopy(np.array(tilename_matrix, tilestate_type))
         self._size = frame.Coordinate(self._tilematrix.shape[0], self._tilematrix.shape[1])
+        self._acce_dict = {}
 
     def tilematrix(self):
         return self._tilematrix
 
     def size(self)->frame.Coordinate:
         return self._size
     
     def __getitem__(self, place:frame.Coordinate)->str:
-        return deepcopy(self._tilematrix[place.x()][place.y()])
+        return bytes(self._tilematrix[place.x(), place.y()]).decode("utf-8")
+    
+    def save_acce_s(self, map:str, gidmatrix:np.ndarray):
+        self._acce_dict[map] = gidmatrix
+    
+    def get_acce_s(self, map:str):
+        return self._acce_dict.get(map)
+
+    def map(self, dic:dict)->TileGroup_Matrix:
+        tilegroup_map = deepcopy(self)
+        for place in self._size:
+            value = self.__getitem__(place)
+            if dic.get(value) != None:
+                tilegroup_map._tilematrix[place.x()][place.y()] = deepcopy(dic[value])
+        return tilegroup_map
+    
+    def part(self, rect:frame.Rectangle)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._size = deepcopy(rect._addCoordinate)
+        tilegroup_part._tilematrix = deepcopy(self._tilematrix[int(rect.i().x()):int(rect.e().x()), int(rect.i().y()):int(rect.e().y())])
+        return tilegroup_part
+    
+    def flip_h(self)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._tilematrix = np.flipud(tilegroup_part._tilematrix)
+
+    def flip_v(self)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._tilematrix = np.fliplr(tilegroup_part._tilematrix)
+
+    def rotate_CW(self)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._tilematrix = np.flipud(tilegroup_part._tilematrix.transpose())
+
+    def rotate_RW(self)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._tilematrix = np.fliplr(tilegroup_part._tilematrix.transpose())
+    
+    def rotate_O(self)->TileGroup_Matrix:
+        tilegroup_part = deepcopy(self)
+        tilegroup_part._tilematrix = np.fliplr(np.flipud(tilegroup_part._tilematrix))
     
 class TileGroup_AddLayer(TileGroup_Matrix):
     def __init__(self, layername:str, tilename_matrix):
         TileGroup_Matrix.__init__(self, tilename_matrix)
         TileGroup_AddLayer._add_layername(self, layername)
 
     def _add_layername(self, layername:str)->None:
@@ -47,28 +92,31 @@
 class TileGroup_AddFile(TileGroup_Matrix):
     def __init__(self, tilename_to_tileset:dict[str, TYPE.tileid], tilename_matrix):
         TileGroup_Matrix.__init__(self, tilename_matrix)
         TileGroup_AddFile._add_tilename(self, tilename_to_tileset)
 
     def _add_tilename(self, tilename_to_tileset:dict[str, TYPE.tileid])->None:
         tilename_to_tileset_n = deepcopy(tilename_to_tileset)
-        zeroadd = {"0": frame.TagCoordinate.init_xy("empty", 0, 0)}
+        zeroadd = {const.KEY.empty_tile_for_tilegroup: frame.TagCoordinate.init_xy("empty", 0, 0)}
         if utility.dict_isconflict(tilename_to_tileset, zeroadd):
             raise KeyConflictError("Key-value of the tile group conflicts at instantiation. \
                                    0 is the default empty tile.")
         tilename_to_tileset_n.update(zeroadd)
         self._tilename_to_tileset = tilename_to_tileset_n
 
     @classmethod
     def init_tilegroup_matrix(cls, tilename_to_tileset:str, tilegroup_matrix:TileGroup_Matrix):
         return cls(tilename_to_tileset, tilegroup_matrix._tilematrix)
 
     def __getitem__(self, place: frame.Coordinate) -> TYPE.tileid:
-        stritems = bytes(TileGroup_Matrix.__getitem__(self, place)).decode("utf-8")
-        return deepcopy(self._tilename_to_tileset[stritems])
+        stritems = TileGroup_Matrix.__getitem__(self, place)
+        if self._tilename_to_tileset.get(stritems) == None:
+            return 0
+        else:
+            return deepcopy(self._tilename_to_tileset[stritems])
     
     def tilename_to_tileset(self)->dict[str, TYPE.tileid]:
         return deepcopy(self._tilename_to_tileset)
     
 class TileGroup_One(TileGroup_AddFile, TileGroup_AddLayer):
     def __init__(self, layername:str, tilename_to_tileset:dict[str, TYPE.tileid], tilename_matrix)->None:
         TileGroup_Matrix.__init__(self, tilename_matrix)
@@ -92,32 +140,34 @@
         self._tilegrouplist_addlayer = deepcopy(tilegrouplist_addlayer)
 
     def tilegrouplist(self):
         return deepcopy(self._tilegrouplist_addlayer)
 
 class TileGroup_List(TileGroup_List_SubTileName):
     def __init__(self, tilename_to_tileset:dict[str, TYPE.tileid], tilegrouplist_addlayer:list[TileGroup_AddLayer]):
-        super().__init__(self, tilegrouplist_addlayer)
+        TileGroup_List_SubTileName.__init__(self, tilegrouplist_addlayer)
         self._add_tilename(tilename_to_tileset)
 
     def _add_tilename(self, tilename_to_tileset:dict[str, TYPE.tileid])->None:
         self._tilename_to_tileset = deepcopy(tilename_to_tileset)
 
     @classmethod
     def init_tilegroup_list_subtilename(cls, tilename_to_tileset:dict[str, TYPE.tileid], tilegrouplist_subtilename:TileGroup_List_SubTileName):
         return cls(tilename_to_tileset, tilegrouplist_subtilename.tilegrouplist())
 
     @classmethod
     def init_tilegroup_list(cls, tilegrouplist:list[TileGroup_One]):
         tilegrouplist_addlayer = []
         tilename_to_tileset = {}
         for tilegroup in tilegrouplist:
-            if utility.dict_isconflict(tilename_to_tileset, tilegroup.tilename_to_tileset()):
+            dict_new = tilegroup.tilename_to_tileset()
+            del dict_new[const.KEY.empty_tile_for_tilegroup]
+            if utility.dict_isconflict(tilename_to_tileset, dict_new):
                 raise KeyConflictError("Key-value of the tile group conflicts at instantiation.")
-            tilename_to_tileset.update(tilegroup.tilename_to_tileset())
+            tilename_to_tileset.update(dict_new)
             tilegrouplist_addlayer.append(TileGroup_AddLayer.init_tilegroup(tilegroup))
         return cls(tilename_to_tileset, tilegrouplist_addlayer)
 
     def _iterator(self):
         for tilegroup in self._tilegrouplist_addlayer:
             yield TileGroup_One.init_tilegroup_addlayer(self._tilename_to_tileset, tilegroup)
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,10 +12,14 @@
 
 from rwmap._util._dict_util import dict_isconflict, udictstr_to_dict
 
 from rwmap._util._class_rel import get_ElementOri_from_list_by_name_s
 
 from rwmap._util._png_rel import image_width, image_height
 
-from rwmap._util._list_util import fill_list_of_list, list_variable_s, list_get_s, team_list_inv, search_list_to_index
+from rwmap._util._list_util import *
 
-from rwmap._util._add_dict import add_str_pro, add_time_pro, add_acti_pro
+from rwmap._util._add_dict import add_str_pro, add_time_pro, add_acti_pro
+
+from rwmap._util._coo_util import point_list_to_str
+
+from rwmap._util._matrix_util import *
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_add_dict.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_add_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from rwmap._object import TObject_One
 import rwmap._exceptions as rwexception
 
 def add_time_pro(name:str, aint:float, issecond:bool = True)->dict[str, str]:
     if aint != -1:
         if issecond:
-            return {name: str(aint) + "s"}
+            if isinstance(aint, int):
+                return {name: f"{str(aint)}s"}
+            else:
+                return {name: f"{aint:.2f}s"}
         else:
             return {name: str(int(aint))}
     else:
         return {}
     
 def add_str_pro(name:str, value:str)->dict[str, str]:
     if value != None:
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_list_util.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_list_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import deepcopy
 
 import rwmap._frame as frame
 
 def fill_list_of_list(element, size:frame.Coordinate):
-    return [[deepcopy(element)] * size.y() for i in range(size.x())]
+    return [[deepcopy(element)] * size.x() for i in range(size.y())]
 
 def list_variable_s(element_s):
     if isinstance(element_s, list):
         return element_s
     elif element_s == None:
         return element_s
     else:
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.1
+Version: 1.4.2
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -688,14 +688,16 @@
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 [简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/Tutorial.md)
 
+【教程已过时】
+
 [简单城夺地图代码例子](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/examples/example1/example1.py)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
@@ -704,14 +706,16 @@
 
 基本框架已完成。
 
 地块组框架已完成。
 
 宾语组框架已完成。
 
+该版本为临时版本，尽量不要直接使用。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
@@ -731,7 +735,10 @@
 #### 4.即可使用python库改变地块和宾语
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
+
+文件中存在一些地块集模版，存放在rwmap/examples/template/，包括
+notTiled的v3模板，城夺地块集模板（来自Xs）
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 rwmap/_case/__init__.py
 rwmap/_case/_layer.py
 rwmap/_case/_object.py
 rwmap/_case/_objectgroup.py
 rwmap/_case/_tileset.py
 rwmap/_data/__init__.py
 rwmap/_data/const.py
-rwmap/_data/otgroup_grid/__init__.py
-rwmap/_data/tile_group_grid/__init__.py
-rwmap/_data/tile_group_grid/_tile_group_addlayer.py
-rwmap/_data/tile_group_grid/_tile_group_matrix.py
-rwmap/_data/tile_group_grid/_tile_group_one.py
 rwmap/_data/tobject/__init__.py
 rwmap/_data/tobject/_camera.py
 rwmap/_data/tobject/_credit.py
 rwmap/_data/tobject/_mapText.py
 rwmap/_data/tobject/_mapinfo.py
 rwmap/_data/tobject/_message.py
 rwmap/_data/tobject/_node.py
@@ -31,16 +26,20 @@
 rwmap/_data/tobject_group/_city/__init__.py
 rwmap/_data/tobject_group/_city/_city.py
 rwmap/_data/tobject_group/_city/_city_detect.py
 rwmap/_data/tobject_group/_city/_city_remove.py
 rwmap/_data/tobject_group/_city/_city_text.py
 rwmap/_data/tobject_group/_city/_normal_unit_add.py
 rwmap/_data/tobject_group/_city/_refresh_building.py
+rwmap/_data/tobject_group/_count/__init__.py
+rwmap/_data/tobject_group/_count/_flash.py
 rwmap/_data/tobject_group/_troop/__init__.py
 rwmap/_data/tobject_group/_troop/_troop_add.py
+rwmap/_data/tobject_group/_victory/__init__.py
+rwmap/_data/tobject_group/_victory/_victory_co.py
 rwmap/_frame/__init__.py
 rwmap/_frame/_coordinate.py
 rwmap/_frame/_element_ori.py
 rwmap/_frame/_element_property.py
 rwmap/_object/__init__.py
 rwmap/_object/_object_global.py
 rwmap/_object/_object_group.py
@@ -51,17 +50,19 @@
 rwmap/_otgroup/__init__.py
 rwmap/_otgroup/_object_tile_group.py
 rwmap/_tile/__init__.py
 rwmap/_tile/_tile_group.py
 rwmap/_util/__init__.py
 rwmap/_util/_add_dict.py
 rwmap/_util/_class_rel.py
+rwmap/_util/_coo_util.py
 rwmap/_util/_dict_util.py
 rwmap/_util/_etElement_process.py
 rwmap/_util/_list_util.py
+rwmap/_util/_matrix_util.py
 rwmap/_util/_png_rel.py
 rwmap/_util/_str_util.py
 rwmap/other_data/requirements.txt
 rwmap/other_data/maps/decoration.tsx
 rwmap/other_data/maps/misc.tsx
 rwmap/other_data/maps/units.tsx
 rwmap/other_data/maps/bitmaps/bridge.png
```

### Comparing `rwmapeditor_exgcdwu-1.4.1/setup.py` & `rwmapeditor_exgcdwu-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
```

