# Comparing `tmp/pssapi-0.4.1.tar.gz` & `tmp/pssapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssapi-0.4.1.tar", max compression
+gzip compressed data, was "pssapi-0.5.0.tar", max compression
```

## Comparing `pssapi-0.4.1.tar` & `pssapi-0.5.0.tar`

### file list

```diff
@@ -1,361 +1,364 @@
--rw-r--r--   0        0        0     1062 2023-05-21 15:50:02.286723 pssapi-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     1108 2023-05-24 15:27:45.611976 pssapi-0.4.1/README.md
--rw-r--r--   0        0        0     1669 2024-03-26 13:52:25.340885 pssapi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      273 2024-03-26 13:52:41.980881 pssapi-0.4.1/src/pssapi/__init__.py
--rw-r--r--   0        0        0      403 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/client.py
--rw-r--r--   0        0        0     9320 2024-03-28 14:31:47.439241 pssapi-0.4.1/src/pssapi/client_base.py
--rw-r--r--   0        0        0      441 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/constants.py
--rw-r--r--   0        0        0     5159 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/core.py
--rw-r--r--   0        0        0     4315 2024-01-03 14:50:36.584459 pssapi-0.4.1/src/pssapi/entities/__init__.py
--rw-r--r--   0        0        0     1203 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/achievement_design.py
--rw-r--r--   0        0        0     2153 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/action_type.py
--rw-r--r--   0        0        0      301 2023-05-27 01:32:07.517526 pssapi-0.4.1/src/pssapi/entities/add_starbux.py
--rw-r--r--   0        0        0      377 2024-03-26 13:49:56.280912 pssapi-0.4.1/src/pssapi/entities/alliance.py
--rw-r--r--   0        0        0      735 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/animation.py
--rw-r--r--   0        0        0      864 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/asset.py
--rw-r--r--   0        0        0     1999 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/background.py
--rw-r--r--   0        0        0     1884 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/battle.py
--rw-r--r--   0        0        0     1486 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/challenge_design.py
--rw-r--r--   0        0        0      656 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/character.py
--rw-r--r--   0        0        0      429 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/character_action.py
--rw-r--r--   0        0        0     2112 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/character_design.py
--rw-r--r--   0        0        0      474 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/character_design_action.py
--rw-r--r--   0        0        0      752 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/character_part.py
--rw-r--r--   0        0        0     1223 2024-03-26 13:49:56.280912 pssapi-0.4.1/src/pssapi/entities/collection_design.py
--rw-r--r--   0        0        0     2189 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/condition_type.py
--rw-r--r--   0        0        0      980 2023-09-01 14:23:05.614118 pssapi-0.4.1/src/pssapi/entities/craft_design.py
--rw-r--r--   0        0        0      720 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/division_design.py
--rw-r--r--   0        0        0     1130 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/draw_design.py
--rw-r--r--   0        0        0      404 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/entity_base.py
--rw-r--r--   0        0        0      703 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/file.py
--rw-r--r--   0        0        0      641 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/friend.py
--rw-r--r--   0        0        0      351 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/get_catalog_quantity.py
--rw-r--r--   0        0        0      357 2023-05-30 14:52:49.598254 pssapi-0.4.1/src/pssapi/entities/get_current_resources.py
--rw-r--r--   0        0        0      661 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/history.py
--rw-r--r--   0        0        0      692 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/item.py
--rw-r--r--   0        0        0     2034 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/item_design.py
--rw-r--r--   0        0        0      439 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/item_design_action.py
--rw-r--r--   0        0        0      363 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/league.py
--rw-r--r--   0        0        0      307 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/list_friends.py
--rw-r--r--   0        0        0     1676 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/live_ops.py
--rw-r--r--   0        0        0      892 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/message.py
--rw-r--r--   0        0        0     1094 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/__init__.py
--rw-r--r--   0        0        0      304 2024-01-03 13:50:53.964701 pssapi-0.4.1/src/pssapi/entities/metadata/entity_metadata_base.py
--rw-r--r--   0        0        0     3000 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/item_design_metadata.py
--rw-r--r--   0        0        0     1501 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/metadata_color.py
--rw-r--r--   0        0        0     1079 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/missile_design_metadata.py
--rw-r--r--   0        0        0      466 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/mission_design_metadata.py
--rw-r--r--   0        0        0      192 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/promotion_design_metadata.py
--rw-r--r--   0        0        0      657 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/reward_design_metadata.py
--rw-r--r--   0        0        0     1105 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/room_design_metadata.py
--rw-r--r--   0        0        0     2006 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/room_design_sprite_metadata.py
--rw-r--r--   0        0        0     1314 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/season_design_metadata.py
--rw-r--r--   0        0        0     1994 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/skin_metadata.py
--rw-r--r--   0        0        0      184 2023-09-01 14:23:05.624118 pssapi-0.4.1/src/pssapi/entities/metadata/skin_set_metadata.py
--rw-r--r--   0        0        0      826 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/metadata/star_system_marker_generator_metadata.py
--rw-r--r--   0        0        0     1458 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/missile_design.py
--rw-r--r--   0        0        0     1547 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/mission_design.py
--rw-r--r--   0        0        0      949 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/mission_event.py
--rw-r--r--   0        0        0      394 2023-06-01 13:54:35.955134 pssapi-0.4.1/src/pssapi/entities/news_design.py
--rw-r--r--   0        0        0      275 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/planet.py
--rw-r--r--   0        0        0      287 2023-05-24 16:24:47.020759 pssapi-0.4.1/src/pssapi/entities/prestige.py
--rw-r--r--   0        0        0     1498 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/promotion_design.py
--rw-r--r--   0        0        0     4880 2024-03-28 14:31:47.329241 pssapi-0.4.1/src/pssapi/entities/raw/__init__.py
--rw-r--r--   0        0        0     5952 2024-03-28 14:31:47.369241 pssapi-0.4.1/src/pssapi/entities/raw/achievement_design_raw.py
--rw-r--r--   0        0        0     5277 2024-03-28 14:31:47.349241 pssapi-0.4.1/src/pssapi/entities/raw/action_type_raw.py
--rw-r--r--   0        0        0      952 2024-03-26 13:49:56.280912 pssapi-0.4.1/src/pssapi/entities/raw/add_starbux_raw.py
--rw-r--r--   0        0        0     6254 2024-03-28 14:31:47.419241 pssapi-0.4.1/src/pssapi/entities/raw/alliance_raw.py
--rw-r--r--   0        0        0     1988 2024-03-28 14:31:47.299241 pssapi-0.4.1/src/pssapi/entities/raw/animation_raw.py
--rw-r--r--   0        0        0     2150 2024-03-28 14:31:47.299241 pssapi-0.4.1/src/pssapi/entities/raw/asset_raw.py
--rw-r--r--   0        0        0     7250 2024-03-28 14:31:47.439241 pssapi-0.4.1/src/pssapi/entities/raw/background_raw.py
--rw-r--r--   0        0        0    17291 2024-03-28 14:31:47.709241 pssapi-0.4.1/src/pssapi/entities/raw/battle_raw.py
--rw-r--r--   0        0        0     8144 2024-03-28 14:31:47.449241 pssapi-0.4.1/src/pssapi/entities/raw/challenge_design_raw.py
--rw-r--r--   0        0        0     2200 2024-03-28 14:31:47.299241 pssapi-0.4.1/src/pssapi/entities/raw/character_action_raw.py
--rw-r--r--   0        0        0     2402 2024-03-28 14:31:47.309241 pssapi-0.4.1/src/pssapi/entities/raw/character_design_action_raw.py
--rw-r--r--   0        0        0    15048 2024-03-28 14:31:47.679241 pssapi-0.4.1/src/pssapi/entities/raw/character_design_raw.py
--rw-r--r--   0        0        0     3425 2024-03-28 14:31:47.369241 pssapi-0.4.1/src/pssapi/entities/raw/character_part_raw.py
--rw-r--r--   0        0        0    12329 2024-03-28 14:31:47.689241 pssapi-0.4.1/src/pssapi/entities/raw/character_raw.py
--rw-r--r--   0        0        0     6513 2024-03-28 14:31:47.439241 pssapi-0.4.1/src/pssapi/entities/raw/collection_design_raw.py
--rw-r--r--   0        0        0     5441 2024-03-28 14:31:47.389241 pssapi-0.4.1/src/pssapi/entities/raw/condition_type_raw.py
--rw-r--r--   0        0        0     4024 2024-03-28 14:31:47.389241 pssapi-0.4.1/src/pssapi/entities/raw/craft_design_raw.py
--rw-r--r--   0        0        0     4302 2024-03-28 14:31:47.389241 pssapi-0.4.1/src/pssapi/entities/raw/division_design_raw.py
--rw-r--r--   0        0        0     5989 2024-03-28 14:31:47.469241 pssapi-0.4.1/src/pssapi/entities/raw/draw_design_raw.py
--rw-r--r--   0        0        0     1188 2024-03-28 14:31:47.359241 pssapi-0.4.1/src/pssapi/entities/raw/entity_base_raw.py
--rw-r--r--   0        0        0     2476 2024-03-28 14:31:47.409241 pssapi-0.4.1/src/pssapi/entities/raw/file_raw.py
--rw-r--r--   0        0        0     3566 2024-03-28 14:31:47.449241 pssapi-0.4.1/src/pssapi/entities/raw/friend_raw.py
--rw-r--r--   0        0        0     1070 2024-03-28 14:31:47.409241 pssapi-0.4.1/src/pssapi/entities/raw/get_catalog_quantity_raw.py
--rw-r--r--   0        0        0     1656 2024-03-26 13:49:56.280912 pssapi-0.4.1/src/pssapi/entities/raw/get_current_resources_raw.py
--rw-r--r--   0        0        0     1880 2024-03-28 14:31:47.439241 pssapi-0.4.1/src/pssapi/entities/raw/history_raw.py
--rw-r--r--   0        0        0     2252 2024-03-28 14:31:47.449241 pssapi-0.4.1/src/pssapi/entities/raw/item_design_action_raw.py
--rw-r--r--   0        0        0    15885 2024-03-28 14:31:47.799241 pssapi-0.4.1/src/pssapi/entities/raw/item_design_raw.py
--rw-r--r--   0        0        0     3155 2024-03-28 14:31:47.469241 pssapi-0.4.1/src/pssapi/entities/raw/item_raw.py
--rw-r--r--   0        0        0     3022 2024-03-28 14:31:47.509241 pssapi-0.4.1/src/pssapi/entities/raw/league_raw.py
--rw-r--r--   0        0        0     1426 2024-03-28 14:31:47.449241 pssapi-0.4.1/src/pssapi/entities/raw/list_friends_raw.py
--rw-r--r--   0        0        0     9494 2024-03-28 14:31:47.699241 pssapi-0.4.1/src/pssapi/entities/raw/live_ops_raw.py
--rw-r--r--   0        0        0     5461 2024-03-28 14:31:47.669241 pssapi-0.4.1/src/pssapi/entities/raw/message_raw.py
--rw-r--r--   0        0        0     9595 2024-03-28 14:31:47.789240 pssapi-0.4.1/src/pssapi/entities/raw/missile_design_raw.py
--rw-r--r--   0        0        0     8292 2024-03-28 14:31:47.689241 pssapi-0.4.1/src/pssapi/entities/raw/mission_design_raw.py
--rw-r--r--   0        0        0     6239 2024-03-28 14:31:47.679241 pssapi-0.4.1/src/pssapi/entities/raw/mission_event_raw.py
--rw-r--r--   0        0        0     2932 2024-03-28 14:31:47.609241 pssapi-0.4.1/src/pssapi/entities/raw/news_design_raw.py
--rw-r--r--   0        0        0      638 2024-03-28 14:31:47.489241 pssapi-0.4.1/src/pssapi/entities/raw/planet_raw.py
--rw-r--r--   0        0        0     1646 2024-03-28 14:31:47.509241 pssapi-0.4.1/src/pssapi/entities/raw/prestige_raw.py
--rw-r--r--   0        0        0    10877 2024-03-28 14:31:47.759240 pssapi-0.4.1/src/pssapi/entities/raw/promotion_design_raw.py
--rw-r--r--   0        0        0     5393 2024-03-28 14:31:47.639241 pssapi-0.4.1/src/pssapi/entities/raw/research_design_raw.py
--rw-r--r--   0        0        0     2089 2024-03-28 14:31:47.539241 pssapi-0.4.1/src/pssapi/entities/raw/research_raw.py
--rw-r--r--   0        0        0     6210 2024-03-28 14:31:47.769240 pssapi-0.4.1/src/pssapi/entities/raw/reward_design_raw.py
--rw-r--r--   0        0        0     2050 2024-03-28 14:31:47.639241 pssapi-0.4.1/src/pssapi/entities/raw/room_action_raw.py
--rw-r--r--   0        0        0     2429 2024-03-28 14:31:47.629241 pssapi-0.4.1/src/pssapi/entities/raw/room_design_purchase_raw.py
--rw-r--r--   0        0        0    13889 2024-03-28 14:31:47.869241 pssapi-0.4.1/src/pssapi/entities/raw/room_design_raw.py
--rw-r--r--   0        0        0     4508 2024-03-28 14:31:47.719241 pssapi-0.4.1/src/pssapi/entities/raw/room_design_sprite_raw.py
--rw-r--r--   0        0        0    11731 2024-03-28 14:31:47.909241 pssapi-0.4.1/src/pssapi/entities/raw/room_raw.py
--rw-r--r--   0        0        0     4533 2024-03-28 14:31:47.759240 pssapi-0.4.1/src/pssapi/entities/raw/sale_raw.py
--rw-r--r--   0        0        0     6719 2024-03-28 14:31:47.769240 pssapi-0.4.1/src/pssapi/entities/raw/season_design_raw.py
--rw-r--r--   0        0        0    42626 2024-03-28 14:31:48.299240 pssapi-0.4.1/src/pssapi/entities/raw/setting_raw.py
--rw-r--r--   0        0        0    14882 2024-03-28 14:31:48.019240 pssapi-0.4.1/src/pssapi/entities/raw/ship_design_raw.py
--rw-r--r--   0        0        0    12182 2024-03-28 14:31:47.949241 pssapi-0.4.1/src/pssapi/entities/raw/ship_raw.py
--rw-r--r--   0        0        0     4936 2024-03-28 14:31:47.809241 pssapi-0.4.1/src/pssapi/entities/raw/situation_design_raw.py
--rw-r--r--   0        0        0     5387 2024-03-28 14:31:47.829241 pssapi-0.4.1/src/pssapi/entities/raw/skin_raw.py
--rw-r--r--   0        0        0     3303 2024-03-28 14:31:47.789240 pssapi-0.4.1/src/pssapi/entities/raw/skin_set_raw.py
--rw-r--r--   0        0        0     2189 2024-03-28 14:31:47.769240 pssapi-0.4.1/src/pssapi/entities/raw/sprite_raw.py
--rw-r--r--   0        0        0     2139 2024-03-28 14:31:47.779240 pssapi-0.4.1/src/pssapi/entities/raw/star_system_link_raw.py
--rw-r--r--   0        0        0    12260 2024-03-28 14:31:48.049240 pssapi-0.4.1/src/pssapi/entities/raw/star_system_marker_generator_raw.py
--rw-r--r--   0        0        0    11533 2024-03-28 14:31:47.999240 pssapi-0.4.1/src/pssapi/entities/raw/star_system_marker_raw.py
--rw-r--r--   0        0        0     3362 2024-03-28 14:31:47.839241 pssapi-0.4.1/src/pssapi/entities/raw/star_system_raw.py
--rw-r--r--   0        0        0     5114 2024-03-28 14:31:47.899241 pssapi-0.4.1/src/pssapi/entities/raw/task_design_raw.py
--rw-r--r--   0        0        0     7386 2024-03-28 14:31:48.009240 pssapi-0.4.1/src/pssapi/entities/raw/training_design_raw.py
--rw-r--r--   0        0        0     2273 2024-03-28 14:31:47.829241 pssapi-0.4.1/src/pssapi/entities/raw/user_email_password_authorize_raw.py
--rw-r--r--   0        0        0     1943 2024-03-28 14:31:47.829241 pssapi-0.4.1/src/pssapi/entities/raw/user_login_raw.py
--rw-r--r--   0        0        0     2709 2024-03-28 14:31:47.879241 pssapi-0.4.1/src/pssapi/entities/raw/user_marker_raw.py
--rw-r--r--   0        0        0    32144 2024-03-28 14:31:48.349240 pssapi-0.4.1/src/pssapi/entities/raw/user_raw.py
--rw-r--r--   0        0        0     2706 2024-03-28 14:31:47.859241 pssapi-0.4.1/src/pssapi/entities/raw/user_season_raw.py
--rw-r--r--   0        0        0     1868 2024-03-28 14:31:47.869241 pssapi-0.4.1/src/pssapi/entities/raw/user_star_system_raw.py
--rw-r--r--   0        0        0      677 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/research.py
--rw-r--r--   0        0        0     1277 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/research_design.py
--rw-r--r--   0        0        0     1275 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/reward_design.py
--rw-r--r--   0        0        0      633 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/room.py
--rw-r--r--   0        0        0      394 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/room_action.py
--rw-r--r--   0        0        0     2338 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/room_design.py
--rw-r--r--   0        0        0      779 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/room_design_purchase.py
--rw-r--r--   0        0        0     1551 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/room_design_sprite.py
--rw-r--r--   0        0        0      864 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/sale.py
--rw-r--r--   0        0        0      981 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/season_design.py
--rw-r--r--   0        0        0     2995 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/setting.py
--rw-r--r--   0        0        0      628 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/ship.py
--rw-r--r--   0        0        0      916 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/ship_design.py
--rw-r--r--   0        0        0     1395 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/situation_design.py
--rw-r--r--   0        0        0     1060 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/entities/skin.py
--rw-r--r--   0        0        0      622 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/skin_set.py
--rw-r--r--   0        0        0      363 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/sprite.py
--rw-r--r--   0        0        0      394 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/star_system.py
--rw-r--r--   0        0        0      425 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/star_system_link.py
--rw-r--r--   0        0        0     2309 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/star_system_marker.py
--rw-r--r--   0        0        0     2617 2023-09-01 14:23:05.634118 pssapi-0.4.1/src/pssapi/entities/star_system_marker_generator.py
--rw-r--r--   0        0        0     1150 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/entities/task_design.py
--rw-r--r--   0        0        0      794 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/entities/training_design.py
--rw-r--r--   0        0        0     3875 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/entities/user.py
--rw-r--r--   0        0        0      401 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/user_email_password_authorize.py
--rw-r--r--   0        0        0      295 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/user_login.py
--rw-r--r--   0        0        0      685 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/entities/user_marker.py
--rw-r--r--   0        0        0      731 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/entities/user_season.py
--rw-r--r--   0        0        0      425 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/entities/user_star_system.py
--rw-r--r--   0        0        0     8925 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/achievement_type.py
--rw-r--r--   0        0        0      357 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/action_type_category.py
--rw-r--r--   0        0        0      398 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/action_type_parameter_relativity.py
--rw-r--r--   0        0        0     1196 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/activity_type.py
--rw-r--r--   0        0        0      481 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/alliance_membership.py
--rw-r--r--   0        0        0      341 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/ammo_category.py
--rw-r--r--   0        0        0      348 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/animation_effect_type.py
--rw-r--r--   0        0        0      307 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/argument.py
--rw-r--r--   0        0        0      384 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/asset_type.py
--rw-r--r--   0        0        0      311 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/authentication_type.py
--rw-r--r--   0        0        0      188 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/availability_mask.py
--rw-r--r--   0        0        0      383 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/background_effect_type.py
--rw-r--r--   0        0        0      319 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/background_type.py
--rw-r--r--   0        0        0      419 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/battle_type.py
--rw-r--r--   0        0        0      227 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/behavior_flags.py
--rw-r--r--   0        0        0      383 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/category_type.py
--rw-r--r--   0        0        0      328 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/challenge_flags.py
--rw-r--r--   0        0        0      269 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/challenge_scoring_type.py
--rw-r--r--   0        0        0      316 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/challenge_type.py
--rw-r--r--   0        0        0      565 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/change_type.py
--rw-r--r--   0        0        0      352 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/character_design_flag_type.py
--rw-r--r--   0        0        0      233 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/character_flags.py
--rw-r--r--   0        0        0      292 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/character_part_type.py
--rw-r--r--   0        0        0      267 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/enums/checksum_type.py
--rw-r--r--   0        0        0      249 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/enums/collection_design_flag.py
--rw-r--r--   0        0        0      301 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/collection_type.py
--rw-r--r--   0        0        0      292 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/completion_value_type.py
--rw-r--r--   0        0        0      144 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/condition_type_availability_mask.py
--rw-r--r--   0        0        0      629 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/condition_type_category.py
--rw-r--r--   0        0        0      576 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/condition_type_comparison.py
--rw-r--r--   0        0        0      914 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/condition_type_parameter.py
--rw-r--r--   0        0        0      332 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/cost_type.py
--rw-r--r--   0        0        0      288 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/craft_attack_type.py
--rw-r--r--   0        0        0      282 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/craft_target_type.py
--rw-r--r--   0        0        0      171 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/crew_rarity.py
--rw-r--r--   0        0        0      938 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/currency_type.py
--rw-r--r--   0        0        0      494 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/daily_reward_status.py
--rw-r--r--   0        0        0      338 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/daily_reward_type.py
--rw-r--r--   0        0        0      570 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/device_type.py
--rw-r--r--   0        0        0      303 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/division_type.py
--rw-r--r--   0        0        0      283 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/download_type.py
--rw-r--r--   0        0        0      277 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/draw_type.py
--rw-r--r--   0        0        0      327 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/duration_type.py
--rw-r--r--   0        0        0      382 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/email_verification_status.py
--rw-r--r--   0        0        0      770 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/enhancement_type.py
--rw-r--r--   0        0        0      302 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/environment_type.py
--rw-r--r--   0        0        0      172 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/equipment_mask_flag.py
--rw-r--r--   0        0        0      371 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/explosion_type.py
--rw-r--r--   0        0        0      169 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/feature_flag.py
--rw-r--r--   0        0        0      482 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/file_download_category.py
--rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/flight_type.py
--rw-r--r--   0        0        0      416 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/friend_type.py
--rw-r--r--   0        0        0      297 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/gender_type.py
--rw-r--r--   0        0        0      229 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/generation_flags.py
--rw-r--r--   0        0        0       89 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/grid_type_flag.py
--rw-r--r--   0        0        0      458 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/guide_type.py
--rw-r--r--   0        0        0      305 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/hazard_category.py
--rw-r--r--   0        0        0      307 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/hazard_type.py
--rw-r--r--   0        0        0      468 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/history_type.py
--rw-r--r--   0        0        0      669 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/item_design_flag_type.py
--rw-r--r--   0        0        0     1702 2024-01-03 13:50:53.964701 pssapi-0.4.1/src/pssapi/enums/item_sub_type.py
--rw-r--r--   0        0        0      411 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/item_type.py
--rw-r--r--   0        0        0      700 2024-01-03 13:50:53.964701 pssapi-0.4.1/src/pssapi/enums/language_key.py
--rw-r--r--   0        0        0      143 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/league_type.py
--rw-r--r--   0        0        0      274 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/manufacture_type.py
--rw-r--r--   0        0        0      315 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/marker_flag.py
--rw-r--r--   0        0        0      439 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/marker_type.py
--rw-r--r--   0        0        0      311 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/matching_status.py
--rw-r--r--   0        0        0      514 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/message_type.py
--rw-r--r--   0        0        0      326 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/missile_type.py
--rw-r--r--   0        0        0      398 2023-06-10 07:56:08.789595 pssapi-0.4.1/src/pssapi/enums/mission_design_flag.py
--rw-r--r--   0        0        0      432 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/mission_design_status.py
--rw-r--r--   0        0        0      384 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/mission_design_type.py
--rw-r--r--   0        0        0      273 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/mission_event_flag.py
--rw-r--r--   0        0        0      329 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/mission_event_type.py
--rw-r--r--   0        0        0      406 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/module_type.py
--rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/movement_type.py
--rw-r--r--   0        0        0     1452 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/objective_type.py
--rw-r--r--   0        0        0      475 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/orbit_anchor_alignment.py
--rw-r--r--   0        0        0      533 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/outcome_type.py
--rw-r--r--   0        0        0      474 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/platform_type.py
--rw-r--r--   0        0        0      460 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/production_server.py
--rw-r--r--   0        0        0      308 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/progression_type.py
--rw-r--r--   0        0        0      344 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/promotion_design_flag.py
--rw-r--r--   0        0        0      476 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/promotion_type.py
--rw-r--r--   0        0        0      274 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/purchase_vip_status.py
--rw-r--r--   0        0        0      767 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/enums/pusher_channel_type.py
--rw-r--r--   0        0        0      377 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/race_type.py
--rw-r--r--   0        0        0      399 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/rarity.py
--rw-r--r--   0        0        0      753 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/research_design_type.py
--rw-r--r--   0        0        0      314 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/research_state.py
--rw-r--r--   0        0        0      412 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/reward_type.py
--rw-r--r--   0        0        0      270 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/room_design_sprite_flag.py
--rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/room_effect_type.py
--rw-r--r--   0        0        0      265 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/enums/room_flags.py
--rw-r--r--   0        0        0      489 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/room_sprite_type.py
--rw-r--r--   0        0        0      337 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/room_status.py
--rw-r--r--   0        0        0     1008 2023-09-01 14:23:05.644118 pssapi-0.4.1/src/pssapi/enums/room_type.py
--rw-r--r--   0        0        0      642 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/sale_item_mask.py
--rw-r--r--   0        0        0      375 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/sale_status.py
--rw-r--r--   0        0        0      380 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/sale_type.py
--rw-r--r--   0        0        0      224 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/enums/season_type.py
--rw-r--r--   0        0        0     1179 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/setting_flags.py
--rw-r--r--   0        0        0      363 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/ship_status.py
--rw-r--r--   0        0        0      341 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/ship_type.py
--rw-r--r--   0        0        0      375 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/situation_design_flag.py
--rw-r--r--   0        0        0      308 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/situation_type.py
--rw-r--r--   0        0        0      374 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/skin_type.py
--rw-r--r--   0        0        0     1186 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/special_ability_type.py
--rw-r--r--   0        0        0      379 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/special_rule_type.py
--rw-r--r--   0        0        0      359 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/enums/sprite_type.py
--rw-r--r--   0        0        0      277 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/status.py
--rw-r--r--   0        0        0      810 2024-03-24 17:02:42.172939 pssapi-0.4.1/src/pssapi/enums/str_enum_base.py
--rw-r--r--   0        0        0      333 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/target_type.py
--rw-r--r--   0        0        0      594 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/task_category.py
--rw-r--r--   0        0        0      233 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/task_design_flags_type.py
--rw-r--r--   0        0        0      431 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/training_animation_style.py
--rw-r--r--   0        0        0      339 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/trigger_type.py
--rw-r--r--   0        0        0      250 2023-06-10 07:56:08.799595 pssapi-0.4.1/src/pssapi/enums/user_flags.py
--rw-r--r--   0        0        0      262 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/enums/user_source_ads_platform_type.py
--rw-r--r--   0        0        0      852 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/user_status.py
--rw-r--r--   0        0        0      797 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/user_type.py
--rw-r--r--   0        0        0      424 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/enums/visibility_flags.py
--rw-r--r--   0        0        0      378 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/exc.py
--rw-r--r--   0        0        0      114 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/pusher/__init__.py
--rw-r--r--   0        0        0     1505 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/pusher/channel.py
--rw-r--r--   0        0        0     5577 2024-01-29 10:13:39.676498 pssapi-0.4.1/src/pssapi/pusher/pusher.py
--rw-r--r--   0        0        0      125 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/raw/__init__.py
--rw-r--r--   0        0        0     2305 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/services/__init__.py
--rw-r--r--   0        0        0      657 2023-05-24 16:24:47.030759 pssapi-0.4.1/src/pssapi/services/achievement_service.py
--rw-r--r--   0        0        0     2835 2024-01-03 13:50:22.304705 pssapi-0.4.1/src/pssapi/services/alliance_service.py
--rw-r--r--   0        0        0      743 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/animation_service.py
--rw-r--r--   0        0        0      753 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/background_service.py
--rw-r--r--   0        0        0      810 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/challenge_service.py
--rw-r--r--   0        0        0     2885 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/character_service.py
--rw-r--r--   0        0        0      818 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/collection_service.py
--rw-r--r--   0        0        0     6435 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/design_service.py
--rw-r--r--   0        0        0      800 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/division_service.py
--rw-r--r--   0        0        0      915 2023-05-24 16:24:47.040759 pssapi-0.4.1/src/pssapi/services/file_service.py
--rw-r--r--   0        0        0     3351 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/galaxy_service.py
--rw-r--r--   0        0        0      449 2023-05-24 16:24:47.040759 pssapi-0.4.1/src/pssapi/services/history_service.py
--rw-r--r--   0        0        0     1611 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/item_service.py
--rw-r--r--   0        0        0      851 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/services/ladder_service.py
--rw-r--r--   0        0        0      767 2024-03-24 18:51:52.601372 pssapi-0.4.1/src/pssapi/services/league_service.py
--rw-r--r--   0        0        0      772 2023-05-24 16:24:47.040759 pssapi-0.4.1/src/pssapi/services/live_ops_service.py
--rw-r--r--   0        0        0      570 2023-05-24 16:24:47.040759 pssapi-0.4.1/src/pssapi/services/market_service.py
--rw-r--r--   0        0        0     1911 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/services/message_service.py
--rw-r--r--   0        0        0     1814 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/mission_service.py
--rw-r--r--   0        0        0      810 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/promotion_service.py
--rw-r--r--   0        0        0     2739 2024-03-28 14:31:47.869241 pssapi-0.4.1/src/pssapi/services/raw/__init__.py
--rw-r--r--   0        0        0      844 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/achievement_service_raw.py
--rw-r--r--   0        0        0     4290 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/alliance_service_raw.py
--rw-r--r--   0        0        0      763 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/animation_service_raw.py
--rw-r--r--   0        0        0      774 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/background_service_raw.py
--rw-r--r--   0        0        0      896 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/challenge_service_raw.py
--rw-r--r--   0        0        0     3097 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/character_service_raw.py
--rw-r--r--   0        0        0      900 2024-03-28 15:03:22.338781 pssapi-0.4.1/src/pssapi/services/raw/collection_service_raw.py
--rw-r--r--   0        0        0    22010 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/design_service_raw.py
--rw-r--r--   0        0        0      885 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/division_service_raw.py
--rw-r--r--   0        0        0     1181 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/file_service_raw.py
--rw-r--r--   0        0        0     4390 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/galaxy_service_raw.py
--rw-r--r--   0        0        0      642 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/history_service_raw.py
--rw-r--r--   0        0        0     1413 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/item_service_raw.py
--rw-r--r--   0        0        0     1255 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/ladder_service_raw.py
--rw-r--r--   0        0        0      833 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/league_service_raw.py
--rw-r--r--   0        0        0     1623 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/live_ops_service_raw.py
--rw-r--r--   0        0        0      809 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/market_service_raw.py
--rw-r--r--   0        0        0     3464 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/message_service_raw.py
--rw-r--r--   0        0        0     3098 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/mission_service_raw.py
--rw-r--r--   0        0        0      896 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/promotion_service_raw.py
--rw-r--r--   0        0        0      885 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/research_service_raw.py
--rw-r--r--   0        0        0      863 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/reward_service_raw.py
--rw-r--r--   0        0        0     1379 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/room_design_sprite_service_raw.py
--rw-r--r--   0        0        0     4518 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/room_service_raw.py
--rw-r--r--   0        0        0      856 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/season_service_raw.py
--rw-r--r--   0        0        0     1795 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/setting_service_raw.py
--rw-r--r--   0        0        0     1881 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/ship_service_raw.py
--rw-r--r--   0        0        0      874 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/situation_service_raw.py
--rw-r--r--   0        0        0      841 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/task_service_raw.py
--rw-r--r--   0        0        0      885 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/training_service_raw.py
--rw-r--r--   0        0        0    13573 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/raw/user_service_raw.py
--rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/research_service.py
--rw-r--r--   0        0        0      780 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/reward_service.py
--rw-r--r--   0        0        0      777 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/room_design_sprite_service.py
--rw-r--r--   0        0        0     3605 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/room_service.py
--rw-r--r--   0        0        0      778 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/season_service.py
--rw-r--r--   0        0        0     2599 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/services/service_base.py
--rw-r--r--   0        0        0     1083 2024-03-28 15:03:22.348781 pssapi-0.4.1/src/pssapi/services/setting_service.py
--rw-r--r--   0        0        0     1859 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/ship_service.py
--rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/situation_service.py
--rw-r--r--   0        0        0      758 2024-03-24 11:23:40.047808 pssapi-0.4.1/src/pssapi/services/task_service.py
--rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/training_service.py
--rw-r--r--   0        0        0    10174 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/services/user_service.py
--rw-r--r--   0        0        0      252 2023-05-24 16:24:47.040759 pssapi-0.4.1/src/pssapi/types.py
--rw-r--r--   0        0        0      181 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/utils/__init__.py
--rw-r--r--   0        0        0       82 2023-09-01 14:23:05.654118 pssapi-0.4.1/src/pssapi/utils/convert.py
--rw-r--r--   0        0        0      487 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/utils/datetime.py
--rw-r--r--   0        0        0      776 2023-09-11 22:35:29.156892 pssapi-0.4.1/src/pssapi/utils/exceptions.py
--rw-r--r--   0        0        0     2259 2024-03-24 18:51:52.611372 pssapi-0.4.1/src/pssapi/utils/parse.py
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 pssapi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-21 15:50:02.286723 pssapi-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1108 2023-05-24 15:27:45.611976 pssapi-0.5.0/README.md
+-rw-r--r--   0        0        0     1669 2024-05-05 14:47:41.467328 pssapi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      273 2024-05-05 14:47:57.257327 pssapi-0.5.0/src/pssapi/__init__.py
+-rw-r--r--   0        0        0      403 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/client.py
+-rw-r--r--   0        0        0     9518 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/client_base.py
+-rw-r--r--   0        0        0      441 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/constants.py
+-rw-r--r--   0        0        0     5823 2024-05-05 14:56:50.227326 pssapi-0.5.0/src/pssapi/core.py
+-rw-r--r--   0        0        0     4315 2024-01-03 14:50:36.584459 pssapi-0.5.0/src/pssapi/entities/__init__.py
+-rw-r--r--   0        0        0     1203 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/achievement_design.py
+-rw-r--r--   0        0        0     2153 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/action_type.py
+-rw-r--r--   0        0        0      301 2023-05-27 01:32:07.517526 pssapi-0.5.0/src/pssapi/entities/add_starbux.py
+-rw-r--r--   0        0        0      377 2024-03-29 11:50:57.087248 pssapi-0.5.0/src/pssapi/entities/alliance.py
+-rw-r--r--   0        0        0      735 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/animation.py
+-rw-r--r--   0        0        0      864 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/asset.py
+-rw-r--r--   0        0        0     1999 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/background.py
+-rw-r--r--   0        0        0     1884 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/battle.py
+-rw-r--r--   0        0        0     1486 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/challenge_design.py
+-rw-r--r--   0        0        0      656 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/character.py
+-rw-r--r--   0        0        0      429 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/character_action.py
+-rw-r--r--   0        0        0     2112 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/character_design.py
+-rw-r--r--   0        0        0      474 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/character_design_action.py
+-rw-r--r--   0        0        0      752 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/character_part.py
+-rw-r--r--   0        0        0     1223 2024-03-29 11:50:57.087248 pssapi-0.5.0/src/pssapi/entities/collection_design.py
+-rw-r--r--   0        0        0     2189 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/condition_type.py
+-rw-r--r--   0        0        0      980 2023-09-01 14:23:05.614118 pssapi-0.5.0/src/pssapi/entities/craft_design.py
+-rw-r--r--   0        0        0      720 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/division_design.py
+-rw-r--r--   0        0        0     1130 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/draw_design.py
+-rw-r--r--   0        0        0      404 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/entity_base.py
+-rw-r--r--   0        0        0      703 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/file.py
+-rw-r--r--   0        0        0      641 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/friend.py
+-rw-r--r--   0        0        0      351 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/get_catalog_quantity.py
+-rw-r--r--   0        0        0      357 2023-05-30 14:52:49.598254 pssapi-0.5.0/src/pssapi/entities/get_current_resources.py
+-rw-r--r--   0        0        0      661 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/history.py
+-rw-r--r--   0        0        0      692 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/item.py
+-rw-r--r--   0        0        0     2034 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/item_design.py
+-rw-r--r--   0        0        0      439 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/item_design_action.py
+-rw-r--r--   0        0        0      363 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/league.py
+-rw-r--r--   0        0        0      307 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/list_friends.py
+-rw-r--r--   0        0        0     1676 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/live_ops.py
+-rw-r--r--   0        0        0      892 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/message.py
+-rw-r--r--   0        0        0     1094 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/__init__.py
+-rw-r--r--   0        0        0      304 2024-01-03 13:50:53.964701 pssapi-0.5.0/src/pssapi/entities/metadata/entity_metadata_base.py
+-rw-r--r--   0        0        0     3000 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/item_design_metadata.py
+-rw-r--r--   0        0        0     1501 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/metadata_color.py
+-rw-r--r--   0        0        0     1079 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/missile_design_metadata.py
+-rw-r--r--   0        0        0      466 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/mission_design_metadata.py
+-rw-r--r--   0        0        0      192 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/promotion_design_metadata.py
+-rw-r--r--   0        0        0      657 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/reward_design_metadata.py
+-rw-r--r--   0        0        0     1105 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/room_design_metadata.py
+-rw-r--r--   0        0        0     2006 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/room_design_sprite_metadata.py
+-rw-r--r--   0        0        0     1314 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/season_design_metadata.py
+-rw-r--r--   0        0        0     1994 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/skin_metadata.py
+-rw-r--r--   0        0        0      184 2023-09-01 14:23:05.624118 pssapi-0.5.0/src/pssapi/entities/metadata/skin_set_metadata.py
+-rw-r--r--   0        0        0      826 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/metadata/star_system_marker_generator_metadata.py
+-rw-r--r--   0        0        0     1458 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/missile_design.py
+-rw-r--r--   0        0        0     1547 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/mission_design.py
+-rw-r--r--   0        0        0      949 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/mission_event.py
+-rw-r--r--   0        0        0      394 2023-06-01 13:54:35.955134 pssapi-0.5.0/src/pssapi/entities/news_design.py
+-rw-r--r--   0        0        0      275 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/planet.py
+-rw-r--r--   0        0        0      287 2023-05-24 16:24:47.020759 pssapi-0.5.0/src/pssapi/entities/prestige.py
+-rw-r--r--   0        0        0     1498 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/promotion_design.py
+-rw-r--r--   0        0        0     4880 2024-05-05 10:50:43.964795 pssapi-0.5.0/src/pssapi/entities/raw/__init__.py
+-rw-r--r--   0        0        0     5952 2024-05-05 10:50:43.994795 pssapi-0.5.0/src/pssapi/entities/raw/achievement_design_raw.py
+-rw-r--r--   0        0        0     5644 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/action_type_raw.py
+-rw-r--r--   0        0        0      952 2024-03-29 11:50:57.087248 pssapi-0.5.0/src/pssapi/entities/raw/add_starbux_raw.py
+-rw-r--r--   0        0        0     6254 2024-05-05 10:50:44.484795 pssapi-0.5.0/src/pssapi/entities/raw/alliance_raw.py
+-rw-r--r--   0        0        0     1988 2024-05-05 10:50:43.814795 pssapi-0.5.0/src/pssapi/entities/raw/animation_raw.py
+-rw-r--r--   0        0        0     2150 2024-05-05 10:50:44.094795 pssapi-0.5.0/src/pssapi/entities/raw/asset_raw.py
+-rw-r--r--   0        0        0     7250 2024-05-05 10:50:44.284795 pssapi-0.5.0/src/pssapi/entities/raw/background_raw.py
+-rw-r--r--   0        0        0    17291 2024-05-05 10:50:44.534795 pssapi-0.5.0/src/pssapi/entities/raw/battle_raw.py
+-rw-r--r--   0        0        0     8144 2024-05-05 10:50:44.074795 pssapi-0.5.0/src/pssapi/entities/raw/challenge_design_raw.py
+-rw-r--r--   0        0        0     2200 2024-05-05 10:50:43.864795 pssapi-0.5.0/src/pssapi/entities/raw/character_action_raw.py
+-rw-r--r--   0        0        0     2402 2024-05-05 10:50:44.124795 pssapi-0.5.0/src/pssapi/entities/raw/character_design_action_raw.py
+-rw-r--r--   0        0        0    15357 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/character_design_raw.py
+-rw-r--r--   0        0        0     3425 2024-05-05 10:50:44.164795 pssapi-0.5.0/src/pssapi/entities/raw/character_part_raw.py
+-rw-r--r--   0        0        0    12907 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/character_raw.py
+-rw-r--r--   0        0        0     7343 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/collection_design_raw.py
+-rw-r--r--   0        0        0     5811 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/condition_type_raw.py
+-rw-r--r--   0        0        0     4580 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/craft_design_raw.py
+-rw-r--r--   0        0        0     4302 2024-05-05 10:50:44.344795 pssapi-0.5.0/src/pssapi/entities/raw/division_design_raw.py
+-rw-r--r--   0        0        0     5989 2024-05-05 10:50:44.484795 pssapi-0.5.0/src/pssapi/entities/raw/draw_design_raw.py
+-rw-r--r--   0        0        0     1188 2024-05-05 10:50:44.144795 pssapi-0.5.0/src/pssapi/entities/raw/entity_base_raw.py
+-rw-r--r--   0        0        0     2476 2024-05-05 10:50:44.234795 pssapi-0.5.0/src/pssapi/entities/raw/file_raw.py
+-rw-r--r--   0        0        0     3566 2024-05-05 10:50:44.424795 pssapi-0.5.0/src/pssapi/entities/raw/friend_raw.py
+-rw-r--r--   0        0        0     1070 2024-05-05 10:50:44.234795 pssapi-0.5.0/src/pssapi/entities/raw/get_catalog_quantity_raw.py
+-rw-r--r--   0        0        0     1656 2024-03-29 11:50:57.087248 pssapi-0.5.0/src/pssapi/entities/raw/get_current_resources_raw.py
+-rw-r--r--   0        0        0     1880 2024-05-05 10:50:44.324795 pssapi-0.5.0/src/pssapi/entities/raw/history_raw.py
+-rw-r--r--   0        0        0     2252 2024-05-05 10:50:44.404795 pssapi-0.5.0/src/pssapi/entities/raw/item_design_action_raw.py
+-rw-r--r--   0        0        0    15885 2024-05-05 10:50:45.414795 pssapi-0.5.0/src/pssapi/entities/raw/item_design_raw.py
+-rw-r--r--   0        0        0     3155 2024-05-05 10:50:44.404795 pssapi-0.5.0/src/pssapi/entities/raw/item_raw.py
+-rw-r--r--   0        0        0     3022 2024-05-05 10:50:44.594795 pssapi-0.5.0/src/pssapi/entities/raw/league_raw.py
+-rw-r--r--   0        0        0     1426 2024-05-05 10:50:44.394795 pssapi-0.5.0/src/pssapi/entities/raw/list_friends_raw.py
+-rw-r--r--   0        0        0     9494 2024-05-05 10:50:45.004795 pssapi-0.5.0/src/pssapi/entities/raw/live_ops_raw.py
+-rw-r--r--   0        0        0     5461 2024-05-05 10:50:44.854795 pssapi-0.5.0/src/pssapi/entities/raw/message_raw.py
+-rw-r--r--   0        0        0     9595 2024-05-05 10:50:45.094795 pssapi-0.5.0/src/pssapi/entities/raw/missile_design_raw.py
+-rw-r--r--   0        0        0     8292 2024-05-05 10:50:44.814795 pssapi-0.5.0/src/pssapi/entities/raw/mission_design_raw.py
+-rw-r--r--   0        0        0     6239 2024-05-05 10:50:44.864795 pssapi-0.5.0/src/pssapi/entities/raw/mission_event_raw.py
+-rw-r--r--   0        0        0     2932 2024-05-05 10:50:44.684795 pssapi-0.5.0/src/pssapi/entities/raw/news_design_raw.py
+-rw-r--r--   0        0        0      638 2024-05-05 10:50:44.454795 pssapi-0.5.0/src/pssapi/entities/raw/planet_raw.py
+-rw-r--r--   0        0        0     1646 2024-05-05 10:50:44.574795 pssapi-0.5.0/src/pssapi/entities/raw/prestige_raw.py
+-rw-r--r--   0        0        0    10877 2024-05-05 10:50:45.114795 pssapi-0.5.0/src/pssapi/entities/raw/promotion_design_raw.py
+-rw-r--r--   0        0        0     5393 2024-05-05 10:50:44.664795 pssapi-0.5.0/src/pssapi/entities/raw/research_design_raw.py
+-rw-r--r--   0        0        0     2089 2024-05-05 10:50:44.624795 pssapi-0.5.0/src/pssapi/entities/raw/research_raw.py
+-rw-r--r--   0        0        0     6210 2024-05-05 10:50:45.114795 pssapi-0.5.0/src/pssapi/entities/raw/reward_design_raw.py
+-rw-r--r--   0        0        0     2050 2024-05-05 10:50:44.644795 pssapi-0.5.0/src/pssapi/entities/raw/room_action_raw.py
+-rw-r--r--   0        0        0     2429 2024-05-05 10:50:44.734795 pssapi-0.5.0/src/pssapi/entities/raw/room_design_purchase_raw.py
+-rw-r--r--   0        0        0    14179 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/room_design_raw.py
+-rw-r--r--   0        0        0     4508 2024-05-05 10:50:44.834795 pssapi-0.5.0/src/pssapi/entities/raw/room_design_sprite_raw.py
+-rw-r--r--   0        0        0    11731 2024-05-05 10:50:45.144795 pssapi-0.5.0/src/pssapi/entities/raw/room_raw.py
+-rw-r--r--   0        0        0     4533 2024-05-05 10:50:44.864795 pssapi-0.5.0/src/pssapi/entities/raw/sale_raw.py
+-rw-r--r--   0        0        0     7352 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/season_design_raw.py
+-rw-r--r--   0        0        0    42858 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/entities/raw/setting_raw.py
+-rw-r--r--   0        0        0    14882 2024-05-05 10:50:45.324795 pssapi-0.5.0/src/pssapi/entities/raw/ship_design_raw.py
+-rw-r--r--   0        0        0    12182 2024-05-05 10:50:45.364795 pssapi-0.5.0/src/pssapi/entities/raw/ship_raw.py
+-rw-r--r--   0        0        0     4936 2024-05-05 10:50:45.034795 pssapi-0.5.0/src/pssapi/entities/raw/situation_design_raw.py
+-rw-r--r--   0        0        0     5387 2024-05-05 10:50:45.104795 pssapi-0.5.0/src/pssapi/entities/raw/skin_raw.py
+-rw-r--r--   0        0        0     3303 2024-05-05 10:50:45.144795 pssapi-0.5.0/src/pssapi/entities/raw/skin_set_raw.py
+-rw-r--r--   0        0        0     2189 2024-05-05 10:50:44.974795 pssapi-0.5.0/src/pssapi/entities/raw/sprite_raw.py
+-rw-r--r--   0        0        0     2139 2024-05-05 10:50:45.074795 pssapi-0.5.0/src/pssapi/entities/raw/star_system_link_raw.py
+-rw-r--r--   0        0        0    12260 2024-05-05 10:50:45.714795 pssapi-0.5.0/src/pssapi/entities/raw/star_system_marker_generator_raw.py
+-rw-r--r--   0        0        0    11533 2024-05-05 10:50:45.634795 pssapi-0.5.0/src/pssapi/entities/raw/star_system_marker_raw.py
+-rw-r--r--   0        0        0     3362 2024-05-05 10:50:45.174795 pssapi-0.5.0/src/pssapi/entities/raw/star_system_raw.py
+-rw-r--r--   0        0        0     5114 2024-05-05 10:50:45.294795 pssapi-0.5.0/src/pssapi/entities/raw/task_design_raw.py
+-rw-r--r--   0        0        0     7386 2024-05-05 10:50:45.494795 pssapi-0.5.0/src/pssapi/entities/raw/training_design_raw.py
+-rw-r--r--   0        0        0     2273 2024-05-05 10:50:45.204795 pssapi-0.5.0/src/pssapi/entities/raw/user_email_password_authorize_raw.py
+-rw-r--r--   0        0        0     1943 2024-05-05 10:50:45.274795 pssapi-0.5.0/src/pssapi/entities/raw/user_login_raw.py
+-rw-r--r--   0        0        0     2709 2024-05-05 10:50:45.284795 pssapi-0.5.0/src/pssapi/entities/raw/user_marker_raw.py
+-rw-r--r--   0        0        0    32144 2024-05-05 10:50:46.114795 pssapi-0.5.0/src/pssapi/entities/raw/user_raw.py
+-rw-r--r--   0        0        0     2706 2024-05-05 10:50:45.304795 pssapi-0.5.0/src/pssapi/entities/raw/user_season_raw.py
+-rw-r--r--   0        0        0     1868 2024-05-05 10:50:45.224795 pssapi-0.5.0/src/pssapi/entities/raw/user_star_system_raw.py
+-rw-r--r--   0        0        0      677 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/research.py
+-rw-r--r--   0        0        0     1277 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/research_design.py
+-rw-r--r--   0        0        0     1275 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/reward_design.py
+-rw-r--r--   0        0        0      633 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/room.py
+-rw-r--r--   0        0        0      394 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/room_action.py
+-rw-r--r--   0        0        0     2338 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/room_design.py
+-rw-r--r--   0        0        0      779 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/room_design_purchase.py
+-rw-r--r--   0        0        0     1551 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/room_design_sprite.py
+-rw-r--r--   0        0        0      864 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/sale.py
+-rw-r--r--   0        0        0      981 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/season_design.py
+-rw-r--r--   0        0        0     2995 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/setting.py
+-rw-r--r--   0        0        0      628 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/ship.py
+-rw-r--r--   0        0        0      916 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/ship_design.py
+-rw-r--r--   0        0        0     1395 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/situation_design.py
+-rw-r--r--   0        0        0     1060 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/entities/skin.py
+-rw-r--r--   0        0        0      622 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/skin_set.py
+-rw-r--r--   0        0        0      363 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/sprite.py
+-rw-r--r--   0        0        0      394 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/star_system.py
+-rw-r--r--   0        0        0      425 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/star_system_link.py
+-rw-r--r--   0        0        0     2309 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/star_system_marker.py
+-rw-r--r--   0        0        0     2617 2023-09-01 14:23:05.634118 pssapi-0.5.0/src/pssapi/entities/star_system_marker_generator.py
+-rw-r--r--   0        0        0     1150 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/entities/task_design.py
+-rw-r--r--   0        0        0      794 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/entities/training_design.py
+-rw-r--r--   0        0        0     3875 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/entities/user.py
+-rw-r--r--   0        0        0      401 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/user_email_password_authorize.py
+-rw-r--r--   0        0        0      295 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/user_login.py
+-rw-r--r--   0        0        0      685 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/entities/user_marker.py
+-rw-r--r--   0        0        0      731 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/entities/user_season.py
+-rw-r--r--   0        0        0      425 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/entities/user_star_system.py
+-rw-r--r--   0        0        0     8925 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/achievement_type.py
+-rw-r--r--   0        0        0      357 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/action_type_category.py
+-rw-r--r--   0        0        0      398 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/action_type_parameter_relativity.py
+-rw-r--r--   0        0        0     1196 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/activity_type.py
+-rw-r--r--   0        0        0      481 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/alliance_membership.py
+-rw-r--r--   0        0        0      341 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/ammo_category.py
+-rw-r--r--   0        0        0      348 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/animation_effect_type.py
+-rw-r--r--   0        0        0      307 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/argument.py
+-rw-r--r--   0        0        0      384 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/asset_type.py
+-rw-r--r--   0        0        0      311 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/authentication_type.py
+-rw-r--r--   0        0        0      188 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/availability_mask.py
+-rw-r--r--   0        0        0      383 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/background_effect_type.py
+-rw-r--r--   0        0        0      319 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/background_type.py
+-rw-r--r--   0        0        0      419 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/battle_type.py
+-rw-r--r--   0        0        0      227 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/behavior_flags.py
+-rw-r--r--   0        0        0      383 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/category_type.py
+-rw-r--r--   0        0        0      328 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/challenge_flags.py
+-rw-r--r--   0        0        0      269 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/challenge_scoring_type.py
+-rw-r--r--   0        0        0      316 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/challenge_type.py
+-rw-r--r--   0        0        0      565 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/change_type.py
+-rw-r--r--   0        0        0      352 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/character_design_flag_type.py
+-rw-r--r--   0        0        0      233 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/character_flags.py
+-rw-r--r--   0        0        0      292 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/character_part_type.py
+-rw-r--r--   0        0        0      267 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/enums/checksum_type.py
+-rw-r--r--   0        0        0      249 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/enums/collection_design_flag.py
+-rw-r--r--   0        0        0      301 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/collection_type.py
+-rw-r--r--   0        0        0      292 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/completion_value_type.py
+-rw-r--r--   0        0        0      144 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/condition_type_availability_mask.py
+-rw-r--r--   0        0        0      629 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/condition_type_category.py
+-rw-r--r--   0        0        0      576 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/condition_type_comparison.py
+-rw-r--r--   0        0        0      914 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/condition_type_parameter.py
+-rw-r--r--   0        0        0      332 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/cost_type.py
+-rw-r--r--   0        0        0      288 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/craft_attack_type.py
+-rw-r--r--   0        0        0      282 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/craft_target_type.py
+-rw-r--r--   0        0        0      171 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/crew_rarity.py
+-rw-r--r--   0        0        0      938 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/currency_type.py
+-rw-r--r--   0        0        0      494 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/daily_reward_status.py
+-rw-r--r--   0        0        0      338 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/daily_reward_type.py
+-rw-r--r--   0        0        0      570 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/device_type.py
+-rw-r--r--   0        0        0      303 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/division_type.py
+-rw-r--r--   0        0        0      283 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/download_type.py
+-rw-r--r--   0        0        0      277 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/draw_type.py
+-rw-r--r--   0        0        0      327 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/duration_type.py
+-rw-r--r--   0        0        0      382 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/email_verification_status.py
+-rw-r--r--   0        0        0      770 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/enhancement_type.py
+-rw-r--r--   0        0        0      302 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/environment_type.py
+-rw-r--r--   0        0        0      172 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/equipment_mask_flag.py
+-rw-r--r--   0        0        0      371 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/explosion_type.py
+-rw-r--r--   0        0        0      169 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/feature_flag.py
+-rw-r--r--   0        0        0      482 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/file_download_category.py
+-rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/flight_type.py
+-rw-r--r--   0        0        0      416 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/friend_type.py
+-rw-r--r--   0        0        0      297 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/gender_type.py
+-rw-r--r--   0        0        0      229 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/generation_flags.py
+-rw-r--r--   0        0        0       89 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/grid_type_flag.py
+-rw-r--r--   0        0        0      458 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/guide_type.py
+-rw-r--r--   0        0        0      305 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/hazard_category.py
+-rw-r--r--   0        0        0      307 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/hazard_type.py
+-rw-r--r--   0        0        0      468 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/history_type.py
+-rw-r--r--   0        0        0      669 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/item_design_flag_type.py
+-rw-r--r--   0        0        0     1702 2024-01-03 13:50:53.964701 pssapi-0.5.0/src/pssapi/enums/item_sub_type.py
+-rw-r--r--   0        0        0      411 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/item_type.py
+-rw-r--r--   0        0        0      700 2024-01-03 13:50:53.964701 pssapi-0.5.0/src/pssapi/enums/language_key.py
+-rw-r--r--   0        0        0      143 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/league_type.py
+-rw-r--r--   0        0        0      274 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/manufacture_type.py
+-rw-r--r--   0        0        0      315 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/marker_flag.py
+-rw-r--r--   0        0        0      439 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/marker_type.py
+-rw-r--r--   0        0        0      311 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/matching_status.py
+-rw-r--r--   0        0        0      514 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/message_type.py
+-rw-r--r--   0        0        0      326 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/missile_type.py
+-rw-r--r--   0        0        0      398 2023-06-10 07:56:08.789595 pssapi-0.5.0/src/pssapi/enums/mission_design_flag.py
+-rw-r--r--   0        0        0      432 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/mission_design_status.py
+-rw-r--r--   0        0        0      384 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/mission_design_type.py
+-rw-r--r--   0        0        0      273 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/mission_event_flag.py
+-rw-r--r--   0        0        0      329 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/mission_event_type.py
+-rw-r--r--   0        0        0      406 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/module_type.py
+-rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/movement_type.py
+-rw-r--r--   0        0        0     1452 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/objective_type.py
+-rw-r--r--   0        0        0      475 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/orbit_anchor_alignment.py
+-rw-r--r--   0        0        0      533 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/outcome_type.py
+-rw-r--r--   0        0        0      474 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/platform_type.py
+-rw-r--r--   0        0        0      460 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/production_server.py
+-rw-r--r--   0        0        0      308 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/progression_type.py
+-rw-r--r--   0        0        0      344 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/promotion_design_flag.py
+-rw-r--r--   0        0        0      476 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/promotion_type.py
+-rw-r--r--   0        0        0      274 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/purchase_vip_status.py
+-rw-r--r--   0        0        0      767 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/enums/pusher_channel_type.py
+-rw-r--r--   0        0        0      377 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/race_type.py
+-rw-r--r--   0        0        0      399 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/rarity.py
+-rw-r--r--   0        0        0      753 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/research_design_type.py
+-rw-r--r--   0        0        0      314 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/research_state.py
+-rw-r--r--   0        0        0      412 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/reward_type.py
+-rw-r--r--   0        0        0      270 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/room_design_sprite_flag.py
+-rw-r--r--   0        0        0      321 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/room_effect_type.py
+-rw-r--r--   0        0        0      265 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/enums/room_flags.py
+-rw-r--r--   0        0        0      489 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/room_sprite_type.py
+-rw-r--r--   0        0        0      337 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/room_status.py
+-rw-r--r--   0        0        0     1008 2023-09-01 14:23:05.644118 pssapi-0.5.0/src/pssapi/enums/room_type.py
+-rw-r--r--   0        0        0      642 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/sale_item_mask.py
+-rw-r--r--   0        0        0      375 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/sale_status.py
+-rw-r--r--   0        0        0      380 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/sale_type.py
+-rw-r--r--   0        0        0      224 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/enums/season_type.py
+-rw-r--r--   0        0        0     1179 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/setting_flags.py
+-rw-r--r--   0        0        0      363 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/ship_status.py
+-rw-r--r--   0        0        0      341 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/ship_type.py
+-rw-r--r--   0        0        0      375 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/situation_design_flag.py
+-rw-r--r--   0        0        0      308 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/situation_type.py
+-rw-r--r--   0        0        0      374 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/skin_type.py
+-rw-r--r--   0        0        0     1186 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/special_ability_type.py
+-rw-r--r--   0        0        0      379 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/special_rule_type.py
+-rw-r--r--   0        0        0      359 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/enums/sprite_type.py
+-rw-r--r--   0        0        0      277 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/status.py
+-rw-r--r--   0        0        0      810 2024-03-24 17:02:42.172939 pssapi-0.5.0/src/pssapi/enums/str_enum_base.py
+-rw-r--r--   0        0        0      333 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/target_type.py
+-rw-r--r--   0        0        0      594 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/task_category.py
+-rw-r--r--   0        0        0      233 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/task_design_flags_type.py
+-rw-r--r--   0        0        0      431 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/training_animation_style.py
+-rw-r--r--   0        0        0      339 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/trigger_type.py
+-rw-r--r--   0        0        0      250 2023-06-10 07:56:08.799595 pssapi-0.5.0/src/pssapi/enums/user_flags.py
+-rw-r--r--   0        0        0      262 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/enums/user_source_ads_platform_type.py
+-rw-r--r--   0        0        0      852 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/user_status.py
+-rw-r--r--   0        0        0      797 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/user_type.py
+-rw-r--r--   0        0        0      424 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/enums/visibility_flags.py
+-rw-r--r--   0        0        0      378 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/exc.py
+-rw-r--r--   0        0        0      114 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/pusher/__init__.py
+-rw-r--r--   0        0        0     1505 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/pusher/channel.py
+-rw-r--r--   0        0        0     5577 2024-01-29 10:13:39.676498 pssapi-0.5.0/src/pssapi/pusher/pusher.py
+-rw-r--r--   0        0        0      125 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/raw/__init__.py
+-rw-r--r--   0        0        0     2375 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/__init__.py
+-rw-r--r--   0        0        0      657 2023-05-24 16:24:47.030759 pssapi-0.5.0/src/pssapi/services/achievement_service.py
+-rw-r--r--   0        0        0     2835 2024-01-03 13:50:22.304705 pssapi-0.5.0/src/pssapi/services/alliance_service.py
+-rw-r--r--   0        0        0      743 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/animation_service.py
+-rw-r--r--   0        0        0      753 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/background_service.py
+-rw-r--r--   0        0        0      810 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/challenge_service.py
+-rw-r--r--   0        0        0     2885 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/character_service.py
+-rw-r--r--   0        0        0      818 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/collection_service.py
+-rw-r--r--   0        0        0    11250 2024-05-05 14:55:30.387328 pssapi-0.5.0/src/pssapi/services/design_service.py
+-rw-r--r--   0        0        0      800 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/division_service.py
+-rw-r--r--   0        0        0      915 2023-05-24 16:24:47.040759 pssapi-0.5.0/src/pssapi/services/file_service.py
+-rw-r--r--   0        0        0     3351 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/galaxy_service.py
+-rw-r--r--   0        0        0      449 2023-05-24 16:24:47.040759 pssapi-0.5.0/src/pssapi/services/history_service.py
+-rw-r--r--   0        0        0     1611 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/item_service.py
+-rw-r--r--   0        0        0      851 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/services/ladder_service.py
+-rw-r--r--   0        0        0      767 2024-03-24 18:51:52.601372 pssapi-0.5.0/src/pssapi/services/league_service.py
+-rw-r--r--   0        0        0      772 2023-05-24 16:24:47.040759 pssapi-0.5.0/src/pssapi/services/live_ops_service.py
+-rw-r--r--   0        0        0      570 2023-05-24 16:24:47.040759 pssapi-0.5.0/src/pssapi/services/market_service.py
+-rw-r--r--   0        0        0     1911 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/services/message_service.py
+-rw-r--r--   0        0        0     1814 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/mission_service.py
+-rw-r--r--   0        0        0      810 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/promotion_service.py
+-rw-r--r--   0        0        0      977 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/public_service.py
+-rw-r--r--   0        0        0     2823 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/raw/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-05 10:50:45.264795 pssapi-0.5.0/src/pssapi/services/raw/achievement_service_raw.py
+-rw-r--r--   0        0        0     4510 2024-05-05 10:50:45.464795 pssapi-0.5.0/src/pssapi/services/raw/alliance_service_raw.py
+-rw-r--r--   0        0        0      787 2024-05-05 10:50:45.294795 pssapi-0.5.0/src/pssapi/services/raw/animation_service_raw.py
+-rw-r--r--   0        0        0      798 2024-05-05 10:50:45.324795 pssapi-0.5.0/src/pssapi/services/raw/background_service_raw.py
+-rw-r--r--   0        0        0      934 2024-05-05 10:50:45.334795 pssapi-0.5.0/src/pssapi/services/raw/challenge_service_raw.py
+-rw-r--r--   0        0        0     3231 2024-05-05 10:50:45.444795 pssapi-0.5.0/src/pssapi/services/raw/character_service_raw.py
+-rw-r--r--   0        0        0      938 2024-05-05 10:50:45.324795 pssapi-0.5.0/src/pssapi/services/raw/collection_service_raw.py
+-rw-r--r--   0        0        0    29705 2024-05-05 10:50:46.004795 pssapi-0.5.0/src/pssapi/services/raw/design_service_raw.py
+-rw-r--r--   0        0        0      923 2024-05-05 10:50:45.334795 pssapi-0.5.0/src/pssapi/services/raw/division_service_raw.py
+-rw-r--r--   0        0        0     1229 2024-05-05 10:50:45.404795 pssapi-0.5.0/src/pssapi/services/raw/file_service_raw.py
+-rw-r--r--   0        0        0     4643 2024-05-05 10:50:45.594795 pssapi-0.5.0/src/pssapi/services/raw/galaxy_service_raw.py
+-rw-r--r--   0        0        0      666 2024-05-05 10:50:45.364795 pssapi-0.5.0/src/pssapi/services/raw/history_service_raw.py
+-rw-r--r--   0        0        0     1475 2024-05-05 10:50:45.394795 pssapi-0.5.0/src/pssapi/services/raw/item_service_raw.py
+-rw-r--r--   0        0        0     1303 2024-05-05 10:50:45.444795 pssapi-0.5.0/src/pssapi/services/raw/ladder_service_raw.py
+-rw-r--r--   0        0        0      857 2024-05-05 10:50:45.414795 pssapi-0.5.0/src/pssapi/services/raw/league_service_raw.py
+-rw-r--r--   0        0        0     1709 2024-05-05 10:50:45.494795 pssapi-0.5.0/src/pssapi/services/raw/live_ops_service_raw.py
+-rw-r--r--   0        0        0      833 2024-05-05 10:50:45.434795 pssapi-0.5.0/src/pssapi/services/raw/market_service_raw.py
+-rw-r--r--   0        0        0     3612 2024-05-05 10:50:45.644795 pssapi-0.5.0/src/pssapi/services/raw/message_service_raw.py
+-rw-r--r--   0        0        0     3230 2024-05-05 10:50:45.604795 pssapi-0.5.0/src/pssapi/services/raw/mission_service_raw.py
+-rw-r--r--   0        0        0      934 2024-05-05 10:50:45.484795 pssapi-0.5.0/src/pssapi/services/raw/promotion_service_raw.py
+-rw-r--r--   0        0        0     1159 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/raw/public_service_raw.py
+-rw-r--r--   0        0        0      923 2024-05-05 10:50:45.494795 pssapi-0.5.0/src/pssapi/services/raw/research_service_raw.py
+-rw-r--r--   0        0        0      901 2024-05-05 10:50:45.504795 pssapi-0.5.0/src/pssapi/services/raw/reward_service_raw.py
+-rw-r--r--   0        0        0     1455 2024-05-05 10:50:45.584795 pssapi-0.5.0/src/pssapi/services/raw/room_design_sprite_service_raw.py
+-rw-r--r--   0        0        0     4766 2024-05-05 10:50:45.724795 pssapi-0.5.0/src/pssapi/services/raw/room_service_raw.py
+-rw-r--r--   0        0        0      894 2024-05-05 10:50:45.524795 pssapi-0.5.0/src/pssapi/services/raw/season_service_raw.py
+-rw-r--r--   0        0        0     1867 2024-05-05 10:50:45.614795 pssapi-0.5.0/src/pssapi/services/raw/setting_service_raw.py
+-rw-r--r--   0        0        0     1953 2024-05-05 10:50:45.594795 pssapi-0.5.0/src/pssapi/services/raw/ship_service_raw.py
+-rw-r--r--   0        0        0      912 2024-05-05 10:50:45.564795 pssapi-0.5.0/src/pssapi/services/raw/situation_service_raw.py
+-rw-r--r--   0        0        0      865 2024-05-05 10:50:45.534795 pssapi-0.5.0/src/pssapi/services/raw/task_service_raw.py
+-rw-r--r--   0        0        0      923 2024-05-05 10:50:45.554795 pssapi-0.5.0/src/pssapi/services/raw/training_service_raw.py
+-rw-r--r--   0        0        0    14996 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/raw/user_service_raw.py
+-rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/research_service.py
+-rw-r--r--   0        0        0      780 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/reward_service.py
+-rw-r--r--   0        0        0      777 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/room_design_sprite_service.py
+-rw-r--r--   0        0        0     3605 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/room_service.py
+-rw-r--r--   0        0        0      778 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/season_service.py
+-rw-r--r--   0        0        0     2599 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/services/service_base.py
+-rw-r--r--   0        0        0     1083 2024-05-05 14:55:30.387328 pssapi-0.5.0/src/pssapi/services/setting_service.py
+-rw-r--r--   0        0        0     1859 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/ship_service.py
+-rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/situation_service.py
+-rw-r--r--   0        0        0      758 2024-03-24 11:23:40.047808 pssapi-0.5.0/src/pssapi/services/task_service.py
+-rw-r--r--   0        0        0      800 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/services/training_service.py
+-rw-r--r--   0        0        0    10514 2024-05-05 14:17:03.097357 pssapi-0.5.0/src/pssapi/services/user_service.py
+-rw-r--r--   0        0        0      252 2023-05-24 16:24:47.040759 pssapi-0.5.0/src/pssapi/types.py
+-rw-r--r--   0        0        0      308 2024-05-05 14:39:33.677339 pssapi-0.5.0/src/pssapi/utils/__init__.py
+-rw-r--r--   0        0        0       82 2023-09-01 14:23:05.654118 pssapi-0.5.0/src/pssapi/utils/convert.py
+-rw-r--r--   0        0        0      831 2024-05-05 15:40:50.593700 pssapi-0.5.0/src/pssapi/utils/datetime.py
+-rw-r--r--   0        0        0      776 2023-09-11 22:35:29.156892 pssapi-0.5.0/src/pssapi/utils/exceptions.py
+-rw-r--r--   0        0        0     2259 2024-03-24 18:51:52.611372 pssapi-0.5.0/src/pssapi/utils/parse.py
+-rw-r--r--   0        0        0      564 2024-05-05 15:26:58.633702 pssapi-0.5.0/src/pssapi/utils/pss.py
+-rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 pssapi-0.5.0/PKG-INFO
```

### Comparing `pssapi-0.4.1/LICENSE.md` & `pssapi-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/README.md` & `pssapi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/pyproject.toml` & `pssapi-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pssapi"
 description = "Wrapper for the Pixel Starships API"
-version = "0.4.1"
+version = "0.5.0"
 license = "MIT"
 authors = [
     "The worst. <theworstpss@gmail.com>",
     "Solevis",
 ]
 readme = "README.md"
 homepage = "https://github.com/PSS-Tools-Development/pssapi.py"
```

### Comparing `pssapi-0.4.1/src/pssapi/client_base.py` & `pssapi-0.5.0/src/pssapi/client_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,18 @@
         return self.__mission_service
 
     @property
     def promotion_service(self) -> "_services.PromotionService":
         return self.__promotion_service
 
     @property
+    def public_service(self) -> "_services.PublicService":
+        return self.__public_service
+
+    @property
     def research_service(self) -> "_services.ResearchService":
         return self.__research_service
 
     @property
     def reward_service(self) -> "_services.RewardService":
         return self.__reward_service
 
@@ -204,14 +208,15 @@
         self.__ladder_service: _services.LadderService = _services.LadderService(self)
         self.__league_service: _services.LeagueService = _services.LeagueService(self)
         self.__live_ops_service: _services.LiveOpsService = _services.LiveOpsService(self)
         self.__market_service: _services.MarketService = _services.MarketService(self)
         self.__message_service: _services.MessageService = _services.MessageService(self)
         self.__mission_service: _services.MissionService = _services.MissionService(self)
         self.__promotion_service: _services.PromotionService = _services.PromotionService(self)
+        self.__public_service: _services.PublicService = _services.PublicService(self)
         self.__research_service: _services.ResearchService = _services.ResearchService(self)
         self.__reward_service: _services.RewardService = _services.RewardService(self)
         self.__room_design_sprite_service: _services.RoomDesignSpriteService = _services.RoomDesignSpriteService(self)
         self.__room_service: _services.RoomService = _services.RoomService(self)
         self.__season_service: _services.SeasonService = _services.SeasonService(self)
         self.__setting_service: _services.SettingService = _services.SettingService(self)
         self.__ship_service: _services.ShipService = _services.ShipService(self)
```

### Comparing `pssapi-0.4.1/src/pssapi/core.py` & `pssapi-0.5.0/src/pssapi/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import base64 as _base64
 import json as _json
+import zlib as _zlib
 from datetime import datetime as _datetime
 from typing import Any as _Any
 from typing import Dict as _Dict
 from typing import Iterable as _Iterable
 from typing import Tuple as _Tuple
 from typing import Type as _Type
 from xml.etree import ElementTree as _ElementTree
@@ -24,17 +26,24 @@
     if content_type == "json":
         return create_json_request_content(structure, params)
     elif content_type == "xml":
         pass
 
 
 async def get_entities_from_path(
-    entity_tags: _Iterable[_Tuple[_Type["_entities.EntityBase"], str, bool]], xml_parent_tag_name: str, production_server: str, path: str, method: str, request_content: str = None, **params
+    entity_tags: _Iterable[_Tuple[_Type["_entities.EntityBase"], str, bool]],
+    xml_parent_tag_name: str,
+    production_server: str,
+    path: str,
+    method: str,
+    request_content: str = None,
+    response_gzipped: bool = False,
+    **params,
 ):
-    raw_xml = await __get_data_from_path(production_server, path, method, content=request_content, **params)
+    raw_xml = await __get_data_from_path(production_server, path, method, content=request_content, response_gzipped=response_gzipped, **params)
 
     root = _ElementTree.fromstring(raw_xml)
     if root is None or root.tag is None or root.tag.startswith("{http://www.w3.org/1999/xhtml}html"):
         raise _utils.exceptions.PssApiError(f"A server error occured: {raw_xml}")
     if "errorMessage" in root.attrib:
         raise _utils.exceptions.PssApiError(root.attrib["errorMessage"])
 
@@ -74,42 +83,51 @@
 
 def create_json_request_content(structure: str, params: _Dict[str, _Any]) -> str:
     d = _json.loads(structure)
     __update_nested_dict_values(d, params)
     return _json.dumps(d)
 
 
-async def __get_data_from_path(production_server: str, path: str, method: str, content: str = None, **params) -> str:
+async def __get_data_from_path(production_server: str, path: str, method: str, content: str = None, response_gzipped: bool = False, **params) -> str:
     if path:
         path = path.strip("/")
     url = f"https://{production_server}/{path}"
-    return await __get_data_from_url(url, method, content, **params)
+    return await __get_data_from_url(url, method, content=content, response_gzipped=response_gzipped, **params)
 
 
-async def __get_data_from_url(url: str, method: str, content: str = None, **params) -> str:
+async def __get_data_from_url(url: str, method: str, content: str = None, response_gzipped: bool = False, **params) -> str:
     # filter parameters with a None value and format datetime
     filtered_params = {}
     for key, value in params.items():
         if value is None:
             continue
 
         if isinstance(value, _datetime):
             filtered_params[key] = value.strftime(_constants.DATETIME_FORMAT_ISO)
         else:
             filtered_params[key] = value
 
     async with _aiohttp.ClientSession() as session:
         if method == "GET":
             async with session.get(url, params=filtered_params) as response:
-                data = await response.text(encoding="utf-8")
+                response_data = await response.read()
         elif method == "POST":
-            data = content.encode("utf-8") if content else None
-            async with session.post(url, data=data, params=filtered_params) as response:
-                data = await response.text(encoding="utf-8")
-    return data
+            request_data = content.encode("utf-8") if content else None
+            async with session.post(url, data=request_data, params=filtered_params) as response:
+                response_data = await response.read()
+
+    if response_gzipped:
+        try:
+            base64_decoded_data = _base64.b64decode(response_data)
+            response_data = _zlib.decompress(base64_decoded_data, _zlib.MAX_WBITS | 32)
+        except Exception:
+            pass  # If the data can't be base64-decoded or unzipped, then the endpoint returned an error message in plain xml instead.
+
+    decoded_data = response_data.decode("utf-8")
+    return decoded_data
 
 
 def __get_raw_entity_xml(node: _ElementTree.Element) -> dict[str, str]:
     result = node.attrib
     for child in node:
         result.setdefault(child.tag, []).append(__get_raw_entity_xml(child))
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/__init__.py` & `pssapi-0.5.0/src/pssapi/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/achievement_design.py` & `pssapi-0.5.0/src/pssapi/entities/achievement_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/action_type.py` & `pssapi-0.5.0/src/pssapi/entities/action_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/animation.py` & `pssapi-0.5.0/src/pssapi/entities/animation.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/asset.py` & `pssapi-0.5.0/src/pssapi/entities/asset.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/background.py` & `pssapi-0.5.0/src/pssapi/entities/background.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/battle.py` & `pssapi-0.5.0/src/pssapi/entities/battle.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/challenge_design.py` & `pssapi-0.5.0/src/pssapi/entities/challenge_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/character.py` & `pssapi-0.5.0/src/pssapi/entities/character.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/character_design.py` & `pssapi-0.5.0/src/pssapi/entities/character_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/character_part.py` & `pssapi-0.5.0/src/pssapi/entities/character_part.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/collection_design.py` & `pssapi-0.5.0/src/pssapi/entities/collection_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/condition_type.py` & `pssapi-0.5.0/src/pssapi/entities/condition_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/craft_design.py` & `pssapi-0.5.0/src/pssapi/entities/craft_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/division_design.py` & `pssapi-0.5.0/src/pssapi/entities/division_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/draw_design.py` & `pssapi-0.5.0/src/pssapi/entities/draw_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/file.py` & `pssapi-0.5.0/src/pssapi/entities/file.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/friend.py` & `pssapi-0.5.0/src/pssapi/entities/friend.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/history.py` & `pssapi-0.5.0/src/pssapi/entities/history.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/item.py` & `pssapi-0.5.0/src/pssapi/entities/item.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/item_design.py` & `pssapi-0.5.0/src/pssapi/entities/item_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/live_ops.py` & `pssapi-0.5.0/src/pssapi/entities/live_ops.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/message.py` & `pssapi-0.5.0/src/pssapi/entities/message.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/__init__.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/item_design_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/item_design_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/metadata_color.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/metadata_color.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/missile_design_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/missile_design_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/reward_design_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/reward_design_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/room_design_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/room_design_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/room_design_sprite_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/room_design_sprite_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/season_design_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/season_design_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/skin_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/skin_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/metadata/star_system_marker_generator_metadata.py` & `pssapi-0.5.0/src/pssapi/entities/metadata/star_system_marker_generator_metadata.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/missile_design.py` & `pssapi-0.5.0/src/pssapi/entities/missile_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/mission_design.py` & `pssapi-0.5.0/src/pssapi/entities/mission_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/mission_event.py` & `pssapi-0.5.0/src/pssapi/entities/mission_event.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/promotion_design.py` & `pssapi-0.5.0/src/pssapi/entities/promotion_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/__init__.py` & `pssapi-0.5.0/src/pssapi/entities/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/achievement_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/achievement_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/action_type_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/action_type_raw.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self._action_type_description: str = _parse.pss_str(action_type_info.pop("ActionTypeDescription", None))
         self._action_type_id: int = _parse.pss_int(action_type_info.pop("ActionTypeId", None))
         self._action_type_key: str = _parse.pss_str(action_type_info.pop("ActionTypeKey", None))
         self._action_type_name: str = _parse.pss_str(action_type_info.pop("ActionTypeName", None))
         self._action_type_parameter_relativity: str = _parse.pss_str(action_type_info.pop("ActionTypeParameterRelativity", None))
         self._action_type_parameter_value: int = _parse.pss_int(action_type_info.pop("ActionTypeParameterValue", None))
         self._color_string: str = _parse.pss_str(action_type_info.pop("ColorString", None))
+        self._condition_parameter_argument: int = _parse.pss_int(action_type_info.pop("ConditionParameterArgument", None))
         self._condition_type_category: str = _parse.pss_str(action_type_info.pop("ConditionTypeCategory", None))
         self._condition_type_parameter: str = _parse.pss_str(action_type_info.pop("ConditionTypeParameter", None))
         self._image_sprite_id: int = _parse.pss_int(action_type_info.pop("ImageSpriteId", None))
         self._order_index: int = _parse.pss_int(action_type_info.pop("OrderIndex", None))
         self._required_research_design_id: int = _parse.pss_int(action_type_info.pop("RequiredResearchDesignId", None))
         self._room_category_type: str = _parse.pss_str(action_type_info.pop("RoomCategoryType", None))
         self._room_type: str = _parse.pss_str(action_type_info.pop("RoomType", None))
@@ -61,14 +62,18 @@
         return self._action_type_parameter_value
 
     @property
     def color_string(self) -> str:
         return self._color_string
 
     @property
+    def condition_parameter_argument(self) -> int:
+        return self._condition_parameter_argument
+
+    @property
     def condition_type_category(self) -> str:
         return self._condition_type_category
 
     @property
     def condition_type_parameter(self) -> str:
         return self._condition_type_parameter
 
@@ -98,14 +103,15 @@
             self.action_type_description,
             self.action_type_id,
             self.action_type_key,
             self.action_type_name,
             self.action_type_parameter_relativity,
             self.action_type_parameter_value,
             self.color_string,
+            self.condition_parameter_argument,
             self.condition_type_category,
             self.condition_type_parameter,
             self.image_sprite_id,
             self.order_index,
             self.required_research_design_id,
             self.room_category_type,
             self.room_type,
@@ -118,14 +124,15 @@
                 "ActionTypeDescription": self.action_type_description,
                 "ActionTypeId": self.action_type_id,
                 "ActionTypeKey": self.action_type_key,
                 "ActionTypeName": self.action_type_name,
                 "ActionTypeParameterRelativity": self.action_type_parameter_relativity,
                 "ActionTypeParameterValue": self.action_type_parameter_value,
                 "ColorString": self.color_string,
+                "ConditionParameterArgument": self.condition_parameter_argument,
                 "ConditionTypeCategory": self.condition_type_category,
                 "ConditionTypeParameter": self.condition_type_parameter,
                 "ImageSpriteId": self.image_sprite_id,
                 "OrderIndex": self.order_index,
                 "RequiredResearchDesignId": self.required_research_design_id,
                 "RoomCategoryType": self.room_category_type,
                 "RoomType": self.room_type,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/add_starbux_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/add_starbux_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/alliance_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/alliance_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/animation_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/animation_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/asset_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/asset_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/background_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/background_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/battle_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/battle_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/challenge_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/challenge_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/character_action_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/character_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/character_design_action_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/character_design_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/character_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/character_design_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class CharacterDesignRaw(_EntityBaseRaw):
     XML_NODE_NAME: str = "CharacterDesign"
 
     def __init__(self, character_design_info: _EntityInfo) -> None:
         self._dict: _Dict[str, _Any] = {}
         self._action_sound_file_id: int = _parse.pss_int(character_design_info.pop("ActionSoundFileId", None))
         self._attack: float = _parse.pss_float(character_design_info.pop("Attack", None))
+        self._boost_values_string: str = _parse.pss_str(character_design_info.pop("BoostValuesString", None))
         self._character_body_part_id: int = _parse.pss_int(character_design_info.pop("CharacterBodyPartId", None))
         self._character_design_description: str = _parse.pss_str(character_design_info.pop("CharacterDesignDescription", None))
         self._character_design_id: int = _parse.pss_int(character_design_info.pop("CharacterDesignId", None))
         self._character_design_name: str = _parse.pss_str(character_design_info.pop("CharacterDesignName", None))
         self._character_head_part_id: int = _parse.pss_int(character_design_info.pop("CharacterHeadPartId", None))
         self._character_leg_part_id: int = _parse.pss_int(character_design_info.pop("CharacterLegPartId", None))
         self._character_parts: _List[_entities.CharacterPart] = (
@@ -78,14 +79,18 @@
         return self._action_sound_file_id
 
     @property
     def attack(self) -> float:
         return self._attack
 
     @property
+    def boost_values_string(self) -> str:
+        return self._boost_values_string
+
+    @property
     def character_body_part_id(self) -> int:
         return self._character_body_part_id
 
     @property
     def character_design_description(self) -> str:
         return self._character_design_description
 
@@ -277,14 +282,15 @@
     def xp_requirement_scale(self) -> int:
         return self._xp_requirement_scale
 
     def _key(self):
         return (
             self.action_sound_file_id,
             self.attack,
+            self.boost_values_string,
             self.character_body_part_id,
             self.character_design_description,
             self.character_design_id,
             self.character_design_name,
             self.character_head_part_id,
             self.character_leg_part_id,
             tuple(child._key() for child in self.character_parts),
@@ -333,14 +339,15 @@
         )
 
     def __dict__(self):
         if not self._dict:
             self._dict = {
                 "ActionSoundFileId": self.action_sound_file_id,
                 "Attack": self.attack,
+                "BoostValuesString": self.boost_values_string,
                 "CharacterBodyPartId": self.character_body_part_id,
                 "CharacterDesignDescription": self.character_design_description,
                 "CharacterDesignId": self.character_design_id,
                 "CharacterDesignName": self.character_design_name,
                 "CharacterHeadPartId": self.character_head_part_id,
                 "CharacterLegPartId": self.character_leg_part_id,
                 "CharacterParts": [dict(child) for child in self.character_parts],
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/character_part_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/character_part_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/character_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/character_raw.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     def __init__(self, character_info: _EntityInfo) -> None:
         self._dict: _Dict[str, _Any] = {}
         self._ability_improvement: int = _parse.pss_int(character_info.pop("AbilityImprovement", None))
         self._attack_improvement: int = _parse.pss_int(character_info.pop("AttackImprovement", None))
         self._available_date: _datetime = _parse.pss_datetime(character_info.pop("AvailableDate", None))
         self._battle_character_hp: int = _parse.pss_int(character_info.pop("BattleCharacterHp", None))
         self._bloodlust_frame: int = _parse.pss_int(character_info.pop("BloodlustFrame", None))
+        self._bonus_training_capacity: int = _parse.pss_int(character_info.pop("BonusTrainingCapacity", None))
+        self._boost_level: int = _parse.pss_int(character_info.pop("BoostLevel", None))
         self._character_actions: _List[_entities.CharacterAction] = (
             [_entities.CharacterAction(child_info) for child_info in character_info.pop("CharacterActions")[0].get("CharacterAction", [])] if character_info.get("CharacterActions") else []
         )
         self._character_design_id: int = _parse.pss_int(character_info.pop("CharacterDesignId", None))
         self._character_id: int = _parse.pss_int(character_info.pop("CharacterId", None))
         self._character_name: str = _parse.pss_str(character_info.pop("CharacterName", None))
         self._deployment_date: _datetime = _parse.pss_datetime(character_info.pop("DeploymentDate", None))
@@ -81,14 +83,22 @@
         return self._battle_character_hp
 
     @property
     def bloodlust_frame(self) -> int:
         return self._bloodlust_frame
 
     @property
+    def bonus_training_capacity(self) -> int:
+        return self._bonus_training_capacity
+
+    @property
+    def boost_level(self) -> int:
+        return self._boost_level
+
+    @property
     def character_actions(self) -> _List["_entities.CharacterAction"]:
         return self._character_actions
 
     @property
     def character_design_id(self) -> int:
         return self._character_design_id
 
@@ -231,14 +241,16 @@
     def _key(self):
         return (
             self.ability_improvement,
             self.attack_improvement,
             self.available_date,
             self.battle_character_hp,
             self.bloodlust_frame,
+            self.bonus_training_capacity,
+            self.boost_level,
             tuple(child._key() for child in self.character_actions),
             self.character_design_id,
             self.character_id,
             self.character_name,
             self.deployment_date,
             self.designated_room_id,
             self.engine_improvement,
@@ -277,14 +289,16 @@
         if not self._dict:
             self._dict = {
                 "AbilityImprovement": self.ability_improvement,
                 "AttackImprovement": self.attack_improvement,
                 "AvailableDate": self.available_date,
                 "BattleCharacterHp": self.battle_character_hp,
                 "BloodlustFrame": self.bloodlust_frame,
+                "BonusTrainingCapacity": self.bonus_training_capacity,
+                "BoostLevel": self.boost_level,
                 "CharacterActions": [dict(child) for child in self.character_actions],
                 "CharacterDesignId": self.character_design_id,
                 "CharacterId": self.character_id,
                 "CharacterName": self.character_name,
                 "DeploymentDate": self.deployment_date,
                 "DesignatedRoomId": self.designated_room_id,
                 "EngineImprovement": self.engine_improvement,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/collection_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/collection_design_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,27 @@
         self._base_chance: int = _parse.pss_int(collection_design_info.pop("BaseChance", None))
         self._base_enhancement_value: int = _parse.pss_int(collection_design_info.pop("BaseEnhancementValue", None))
         self._collection_description: str = _parse.pss_str(collection_design_info.pop("CollectionDescription", None))
         self._collection_design_id: int = _parse.pss_int(collection_design_info.pop("CollectionDesignId", None))
         self._collection_name: str = _parse.pss_str(collection_design_info.pop("CollectionName", None))
         self._collection_type: str = _parse.pss_str(collection_design_info.pop("CollectionType", None))
         self._color_string: str = _parse.pss_str(collection_design_info.pop("ColorString", None))
+        self._cooldown_time: int = _parse.pss_int(collection_design_info.pop("CooldownTime", None))
         self._enhancement_type: str = _parse.pss_str(collection_design_info.pop("EnhancementType", None))
         self._flags: int = _parse.pss_int(collection_design_info.pop("Flags", None))
         self._halo_animation_id: int = _parse.pss_int(collection_design_info.pop("HaloAnimationId", None))
         self._icon_sprite_id: int = _parse.pss_int(collection_design_info.pop("IconSpriteId", None))
         self._max_combo: int = _parse.pss_int(collection_design_info.pop("MaxCombo", None))
         self._max_use: int = _parse.pss_int(collection_design_info.pop("MaxUse", None))
+        self._metadata: str = _parse.pss_str(collection_design_info.pop("Metadata", None))
         self._min_combo: int = _parse.pss_int(collection_design_info.pop("MinCombo", None))
         self._sprite_id: int = _parse.pss_int(collection_design_info.pop("SpriteId", None))
         self._step_chance: int = _parse.pss_int(collection_design_info.pop("StepChance", None))
-        self._step_enhancement_value: int = _parse.pss_int(collection_design_info.pop("StepEnhancementValue", None))
+        self._step_enhancement_value: float = _parse.pss_float(collection_design_info.pop("StepEnhancementValue", None))
+        self._trigger_animation_id: int = _parse.pss_int(collection_design_info.pop("TriggerAnimationId", None))
         self._trigger_type: str = _parse.pss_str(collection_design_info.pop("TriggerType", None))
         super().__init__(collection_design_info)
 
     @property
     def ability_icon_sprite_id(self) -> int:
         return self._ability_icon_sprite_id
 
@@ -75,14 +78,18 @@
         return self._collection_type
 
     @property
     def color_string(self) -> str:
         return self._color_string
 
     @property
+    def cooldown_time(self) -> int:
+        return self._cooldown_time
+
+    @property
     def enhancement_type(self) -> str:
         return self._enhancement_type
 
     @property
     def flags(self) -> int:
         return self._flags
 
@@ -99,30 +106,38 @@
         return self._max_combo
 
     @property
     def max_use(self) -> int:
         return self._max_use
 
     @property
+    def metadata(self) -> str:
+        return self._metadata
+
+    @property
     def min_combo(self) -> int:
         return self._min_combo
 
     @property
     def sprite_id(self) -> int:
         return self._sprite_id
 
     @property
     def step_chance(self) -> int:
         return self._step_chance
 
     @property
-    def step_enhancement_value(self) -> int:
+    def step_enhancement_value(self) -> float:
         return self._step_enhancement_value
 
     @property
+    def trigger_animation_id(self) -> int:
+        return self._trigger_animation_id
+
+    @property
     def trigger_type(self) -> str:
         return self._trigger_type
 
     def _key(self):
         return (
             self.ability_icon_sprite_id,
             self.ability_name,
@@ -130,24 +145,27 @@
             self.base_chance,
             self.base_enhancement_value,
             self.collection_description,
             self.collection_design_id,
             self.collection_name,
             self.collection_type,
             self.color_string,
+            self.cooldown_time,
             self.enhancement_type,
             self.flags,
             self.halo_animation_id,
             self.icon_sprite_id,
             self.max_combo,
             self.max_use,
+            self.metadata,
             self.min_combo,
             self.sprite_id,
             self.step_chance,
             self.step_enhancement_value,
+            self.trigger_animation_id,
             self.trigger_type,
         )
 
     def __dict__(self):
         if not self._dict:
             self._dict = {
                 "AbilityIconSpriteId": self.ability_icon_sprite_id,
@@ -156,22 +174,25 @@
                 "BaseChance": self.base_chance,
                 "BaseEnhancementValue": self.base_enhancement_value,
                 "CollectionDescription": self.collection_description,
                 "CollectionDesignId": self.collection_design_id,
                 "CollectionName": self.collection_name,
                 "CollectionType": self.collection_type,
                 "ColorString": self.color_string,
+                "CooldownTime": self.cooldown_time,
                 "EnhancementType": self.enhancement_type,
                 "Flags": self.flags,
                 "HaloAnimationId": self.halo_animation_id,
                 "IconSpriteId": self.icon_sprite_id,
                 "MaxCombo": self.max_combo,
                 "MaxUse": self.max_use,
+                "Metadata": self.metadata,
                 "MinCombo": self.min_combo,
                 "SpriteId": self.sprite_id,
                 "StepChance": self.step_chance,
                 "StepEnhancementValue": self.step_enhancement_value,
+                "TriggerAnimationId": self.trigger_animation_id,
                 "TriggerType": self.trigger_type,
             }
             self._dict.update(super().__dict__())
 
         return self._dict
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/condition_type_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/condition_type_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class ConditionTypeRaw(_EntityBaseRaw):
     XML_NODE_NAME: str = "ConditionType"
 
     def __init__(self, condition_type_info: _EntityInfo) -> None:
         self._dict: _Dict[str, _Any] = {}
         self._color_string: str = _parse.pss_str(condition_type_info.pop("ColorString", None))
+        self._condition_parameter_argument: int = _parse.pss_int(condition_type_info.pop("ConditionParameterArgument", None))
         self._condition_type_availability: int = _parse.pss_int(condition_type_info.pop("ConditionTypeAvailability", None))
         self._condition_type_category: str = _parse.pss_str(condition_type_info.pop("ConditionTypeCategory", None))
         self._condition_type_comparison: str = _parse.pss_str(condition_type_info.pop("ConditionTypeComparison", None))
         self._condition_type_description: str = _parse.pss_str(condition_type_info.pop("ConditionTypeDescription", None))
         self._condition_type_id: int = _parse.pss_int(condition_type_info.pop("ConditionTypeId", None))
         self._condition_type_key: str = _parse.pss_str(condition_type_info.pop("ConditionTypeKey", None))
         self._condition_type_name: str = _parse.pss_str(condition_type_info.pop("ConditionTypeName", None))
@@ -33,14 +34,18 @@
         super().__init__(condition_type_info)
 
     @property
     def color_string(self) -> str:
         return self._color_string
 
     @property
+    def condition_parameter_argument(self) -> int:
+        return self._condition_parameter_argument
+
+    @property
     def condition_type_availability(self) -> int:
         return self._condition_type_availability
 
     @property
     def condition_type_category(self) -> str:
         return self._condition_type_category
 
@@ -91,14 +96,15 @@
     @property
     def room_type(self) -> str:
         return self._room_type
 
     def _key(self):
         return (
             self.color_string,
+            self.condition_parameter_argument,
             self.condition_type_availability,
             self.condition_type_category,
             self.condition_type_comparison,
             self.condition_type_description,
             self.condition_type_id,
             self.condition_type_key,
             self.condition_type_name,
@@ -111,14 +117,15 @@
             self.room_type,
         )
 
     def __dict__(self):
         if not self._dict:
             self._dict = {
                 "ColorString": self.color_string,
+                "ConditionParameterArgument": self.condition_parameter_argument,
                 "ConditionTypeAvailability": self.condition_type_availability,
                 "ConditionTypeCategory": self.condition_type_category,
                 "ConditionTypeComparison": self.condition_type_comparison,
                 "ConditionTypeDescription": self.condition_type_description,
                 "ConditionTypeId": self.condition_type_id,
                 "ConditionTypeKey": self.condition_type_key,
                 "ConditionTypeName": self.condition_type_name,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/craft_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/craft_design_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     def __init__(self, craft_design_info: _EntityInfo) -> None:
         self._dict: _Dict[str, _Any] = {}
         self._attack_distance: int = _parse.pss_int(craft_design_info.pop("AttackDistance", None))
         self._attack_range: int = _parse.pss_int(craft_design_info.pop("AttackRange", None))
         self._craft_attack_type: str = _parse.pss_str(craft_design_info.pop("CraftAttackType", None))
         self._craft_design_id: int = _parse.pss_int(craft_design_info.pop("CraftDesignId", None))
         self._craft_name: str = _parse.pss_str(craft_design_info.pop("CraftName", None))
+        self._craft_pathing_type: str = _parse.pss_str(craft_design_info.pop("CraftPathingType", None))
         self._craft_target_type: str = _parse.pss_str(craft_design_info.pop("CraftTargetType", None))
+        self._entity_count: int = _parse.pss_int(craft_design_info.pop("EntityCount", None))
         self._flight_speed: int = _parse.pss_int(craft_design_info.pop("FlightSpeed", None))
         self._hp: int = _parse.pss_int(craft_design_info.pop("Hp", None))
         self._missile_design_id: int = _parse.pss_int(craft_design_info.pop("MissileDesignId", None))
         self._reload: int = _parse.pss_int(craft_design_info.pop("Reload", None))
         self._sprite_id: int = _parse.pss_int(craft_design_info.pop("SpriteId", None))
         self._volley: int = _parse.pss_int(craft_design_info.pop("Volley", None))
         self._volley_delay: int = _parse.pss_int(craft_design_info.pop("VolleyDelay", None))
@@ -47,18 +49,26 @@
         return self._craft_design_id
 
     @property
     def craft_name(self) -> str:
         return self._craft_name
 
     @property
+    def craft_pathing_type(self) -> str:
+        return self._craft_pathing_type
+
+    @property
     def craft_target_type(self) -> str:
         return self._craft_target_type
 
     @property
+    def entity_count(self) -> int:
+        return self._entity_count
+
+    @property
     def flight_speed(self) -> int:
         return self._flight_speed
 
     @property
     def hp(self) -> int:
         return self._hp
 
@@ -85,15 +95,17 @@
     def _key(self):
         return (
             self.attack_distance,
             self.attack_range,
             self.craft_attack_type,
             self.craft_design_id,
             self.craft_name,
+            self.craft_pathing_type,
             self.craft_target_type,
+            self.entity_count,
             self.flight_speed,
             self.hp,
             self.missile_design_id,
             self.reload,
             self.sprite_id,
             self.volley,
             self.volley_delay,
@@ -103,15 +115,17 @@
         if not self._dict:
             self._dict = {
                 "AttackDistance": self.attack_distance,
                 "AttackRange": self.attack_range,
                 "CraftAttackType": self.craft_attack_type,
                 "CraftDesignId": self.craft_design_id,
                 "CraftName": self.craft_name,
+                "CraftPathingType": self.craft_pathing_type,
                 "CraftTargetType": self.craft_target_type,
+                "EntityCount": self.entity_count,
                 "FlightSpeed": self.flight_speed,
                 "Hp": self.hp,
                 "MissileDesignId": self.missile_design_id,
                 "Reload": self.reload,
                 "SpriteId": self.sprite_id,
                 "Volley": self.volley,
                 "VolleyDelay": self.volley_delay,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/division_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/division_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/draw_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/draw_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/entity_base_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/entity_base_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/file_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/file_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/friend_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/friend_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/get_catalog_quantity_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/get_catalog_quantity_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/get_current_resources_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/get_current_resources_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/history_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/history_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/item_design_action_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/item_design_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/item_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/item_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/item_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/item_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/league_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/league_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/list_friends_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/list_friends_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/live_ops_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/live_ops_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/message_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/message_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/missile_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/missile_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/mission_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/mission_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/mission_event_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/mission_event_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/news_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/news_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/planet_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/planet_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/prestige_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/prestige_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/promotion_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/promotion_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/research_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/research_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/research_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/research_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/reward_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/reward_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/room_action_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/room_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/room_design_purchase_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/room_design_purchase_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/room_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/room_design_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         self._reload_time: int = _parse.pss_int(room_design_info.pop("ReloadTime", None))
         self._requirement_string: str = _parse.pss_str(room_design_info.pop("RequirementString", None))
         self._room_description: str = _parse.pss_str(room_design_info.pop("RoomDescription", None))
         self._room_design_id: int = _parse.pss_int(room_design_info.pop("RoomDesignId", None))
         self._room_name: str = _parse.pss_str(room_design_info.pop("RoomName", None))
         self._room_short_name: str = _parse.pss_str(room_design_info.pop("RoomShortName", None))
         self._room_type: str = _parse.pss_str(room_design_info.pop("RoomType", None))
+        self._room_variant_type: int = _parse.pss_int(room_design_info.pop("RoomVariantType", None))
         self._root_room_design_id: int = _parse.pss_int(room_design_info.pop("RootRoomDesignId", None))
         self._rotate: bool = _parse.pss_bool(room_design_info.pop("Rotate", None))
         self._rows: int = _parse.pss_int(room_design_info.pop("Rows", None))
         self._sort_index: int = _parse.pss_int(room_design_info.pop("SortIndex", None))
         self._supported_grid_types: int = _parse.pss_int(room_design_info.pop("SupportedGridTypes", None))
         self._tags: str = _parse.pss_str(room_design_info.pop("Tags", None))
         self._target_type: str = _parse.pss_str(room_design_info.pop("TargetType", None))
@@ -227,14 +228,18 @@
         return self._room_short_name
 
     @property
     def room_type(self) -> str:
         return self._room_type
 
     @property
+    def room_variant_type(self) -> int:
+        return self._room_variant_type
+
+    @property
     def root_room_design_id(self) -> int:
         return self._root_room_design_id
 
     @property
     def rotate(self) -> bool:
         return self._rotate
 
@@ -301,14 +306,15 @@
             self.reload_time,
             self.requirement_string,
             self.room_description,
             self.room_design_id,
             self.room_name,
             self.room_short_name,
             self.room_type,
+            self.room_variant_type,
             self.root_room_design_id,
             self.rotate,
             self.rows,
             self.sort_index,
             self.supported_grid_types,
             self.tags,
             self.target_type,
@@ -355,14 +361,15 @@
                 "ReloadTime": self.reload_time,
                 "RequirementString": self.requirement_string,
                 "RoomDescription": self.room_description,
                 "RoomDesignId": self.room_design_id,
                 "RoomName": self.room_name,
                 "RoomShortName": self.room_short_name,
                 "RoomType": self.room_type,
+                "RoomVariantType": self.room_variant_type,
                 "RootRoomDesignId": self.root_room_design_id,
                 "Rotate": self.rotate,
                 "Rows": self.rows,
                 "SortIndex": self.sort_index,
                 "SupportedGridTypes": self.supported_grid_types,
                 "Tags": self.tags,
                 "TargetType": self.target_type,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/room_design_sprite_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/room_design_sprite_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/room_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/room_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/sale_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/sale_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/season_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/season_design_raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         self._banner_sprite_id: int = _parse.pss_int(season_design_info.pop("BannerSpriteId", None))
         self._button_sprite_id: int = _parse.pss_int(season_design_info.pop("ButtonSpriteId", None))
         self._close_button_sprite_id: int = _parse.pss_int(season_design_info.pop("CloseButtonSpriteId", None))
         self._end_date: _datetime = _parse.pss_datetime(season_design_info.pop("EndDate", None))
         self._from_date: _datetime = _parse.pss_datetime(season_design_info.pop("FromDate", None))
         self._icon_sprite_id: int = _parse.pss_int(season_design_info.pop("IconSpriteId", None))
         self._metadata: str = _parse.pss_str(season_design_info.pop("Metadata", None))
+        self._premium_reward_string: str = _parse.pss_str(season_design_info.pop("PremiumRewardString", None))
         self._prologue_description: str = _parse.pss_str(season_design_info.pop("PrologueDescription", None))
+        self._repeat_reward_string: str = _parse.pss_str(season_design_info.pop("RepeatRewardString", None))
         self._requirement_string: str = _parse.pss_str(season_design_info.pop("RequirementString", None))
         self._reward_string: str = _parse.pss_str(season_design_info.pop("RewardString", None))
         self._season_description: str = _parse.pss_str(season_design_info.pop("SeasonDescription", None))
         self._season_design_id: int = _parse.pss_int(season_design_info.pop("SeasonDesignId", None))
         self._season_name: str = _parse.pss_str(season_design_info.pop("SeasonName", None))
         self._season_sprite_id: int = _parse.pss_int(season_design_info.pop("SeasonSpriteId", None))
         self._season_type: str = _parse.pss_str(season_design_info.pop("SeasonType", None))
@@ -72,18 +74,26 @@
         return self._icon_sprite_id
 
     @property
     def metadata(self) -> str:
         return self._metadata
 
     @property
+    def premium_reward_string(self) -> str:
+        return self._premium_reward_string
+
+    @property
     def prologue_description(self) -> str:
         return self._prologue_description
 
     @property
+    def repeat_reward_string(self) -> str:
+        return self._repeat_reward_string
+
+    @property
     def requirement_string(self) -> str:
         return self._requirement_string
 
     @property
     def reward_string(self) -> str:
         return self._reward_string
 
@@ -130,15 +140,17 @@
             self.banner_sprite_id,
             self.button_sprite_id,
             self.close_button_sprite_id,
             self.end_date,
             self.from_date,
             self.icon_sprite_id,
             self.metadata,
+            self.premium_reward_string,
             self.prologue_description,
+            self.repeat_reward_string,
             self.requirement_string,
             self.reward_string,
             self.season_description,
             self.season_design_id,
             self.season_name,
             self.season_sprite_id,
             self.season_type,
@@ -156,15 +168,17 @@
                 "BannerSpriteId": self.banner_sprite_id,
                 "ButtonSpriteId": self.button_sprite_id,
                 "CloseButtonSpriteId": self.close_button_sprite_id,
                 "EndDate": self.end_date,
                 "FromDate": self.from_date,
                 "IconSpriteId": self.icon_sprite_id,
                 "Metadata": self.metadata,
+                "PremiumRewardString": self.premium_reward_string,
                 "PrologueDescription": self.prologue_description,
+                "RepeatRewardString": self.repeat_reward_string,
                 "RequirementString": self.requirement_string,
                 "RewardString": self.reward_string,
                 "SeasonDescription": self.season_description,
                 "SeasonDesignId": self.season_design_id,
                 "SeasonName": self.season_name,
                 "SeasonSpriteId": self.season_sprite_id,
                 "SeasonType": self.season_type,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/setting_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/setting_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         self._loading_title_sprite_id: int = _parse.pss_int(setting_info.pop("LoadingTitleSpriteId", None))
         self._loot_modifiers: str = _parse.pss_str(setting_info.pop("LootModifiers", None))
         self._maintenance_date: _datetime = _parse.pss_datetime(setting_info.pop("MaintenanceDate", None))
         self._maintenance_message: str = _parse.pss_str(setting_info.pop("MaintenanceMessage", None))
         self._maintenance_title: str = _parse.pss_str(setting_info.pop("MaintenanceTitle", None))
         self._marker_generator_design_version: int = _parse.pss_int(setting_info.pop("MarkerGeneratorDesignVersion", None))
         self._max_boost_duration: int = _parse.pss_int(setting_info.pop("MaxBoostDuration", None))
+        self._max_crews: int = _parse.pss_int(setting_info.pop("MaxCrews", None))
         self._max_daily_draws: int = _parse.pss_int(setting_info.pop("MaxDailyDraws", None))
         self._max_redemption_count: int = _parse.pss_int(setting_info.pop("MaxRedemptionCount", None))
         self._max_redemption_count_per_month: int = _parse.pss_int(setting_info.pop("MaxRedemptionCountPerMonth", None))
         self._merchant_ship_exterior_sprite_id: int = _parse.pss_int(setting_info.pop("MerchantShipExteriorSpriteId", None))
         self._merchant_ship_sprite_id: int = _parse.pss_int(setting_info.pop("MerchantShipSpriteId", None))
         self._min_purchase_reward_points_for_starbux_trading: int = _parse.pss_int(setting_info.pop("MinPurchaseRewardPointsForStarbuxTrading", None))
         self._min_trophies_for_starbux_trading: int = _parse.pss_int(setting_info.pop("MinTrophiesForStarbuxTrading", None))
@@ -440,14 +441,18 @@
         return self._marker_generator_design_version
 
     @property
     def max_boost_duration(self) -> int:
         return self._max_boost_duration
 
     @property
+    def max_crews(self) -> int:
+        return self._max_crews
+
+    @property
     def max_daily_draws(self) -> int:
         return self._max_daily_draws
 
     @property
     def max_redemption_count(self) -> int:
         return self._max_redemption_count
 
@@ -773,14 +778,15 @@
             self.loading_title_sprite_id,
             self.loot_modifiers,
             self.maintenance_date,
             self.maintenance_message,
             self.maintenance_title,
             self.marker_generator_design_version,
             self.max_boost_duration,
+            self.max_crews,
             self.max_daily_draws,
             self.max_redemption_count,
             self.max_redemption_count_per_month,
             self.merchant_ship_exterior_sprite_id,
             self.merchant_ship_sprite_id,
             self.min_purchase_reward_points_for_starbux_trading,
             self.min_trophies_for_starbux_trading,
@@ -915,14 +921,15 @@
                 "LoadingTitleSpriteId": self.loading_title_sprite_id,
                 "LootModifiers": self.loot_modifiers,
                 "MaintenanceDate": self.maintenance_date,
                 "MaintenanceMessage": self.maintenance_message,
                 "MaintenanceTitle": self.maintenance_title,
                 "MarkerGeneratorDesignVersion": self.marker_generator_design_version,
                 "MaxBoostDuration": self.max_boost_duration,
+                "MaxCrews": self.max_crews,
                 "MaxDailyDraws": self.max_daily_draws,
                 "MaxRedemptionCount": self.max_redemption_count,
                 "MaxRedemptionCountPerMonth": self.max_redemption_count_per_month,
                 "MerchantShipExteriorSpriteId": self.merchant_ship_exterior_sprite_id,
                 "MerchantShipSpriteId": self.merchant_ship_sprite_id,
                 "MinPurchaseRewardPointsForStarbuxTrading": self.min_purchase_reward_points_for_starbux_trading,
                 "MinTrophiesForStarbuxTrading": self.min_trophies_for_starbux_trading,
```

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/ship_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/ship_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/ship_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/ship_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/situation_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/situation_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/skin_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/skin_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/skin_set_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/skin_set_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/sprite_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/sprite_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/star_system_link_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/star_system_link_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/star_system_marker_generator_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/star_system_marker_generator_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/star_system_marker_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/star_system_marker_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/star_system_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/star_system_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/task_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/task_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/training_design_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/training_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_email_password_authorize_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_email_password_authorize_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_login_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_login_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_marker_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_marker_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_season_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_season_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/raw/user_star_system_raw.py` & `pssapi-0.5.0/src/pssapi/entities/raw/user_star_system_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/research.py` & `pssapi-0.5.0/src/pssapi/entities/research.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/research_design.py` & `pssapi-0.5.0/src/pssapi/entities/research_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/reward_design.py` & `pssapi-0.5.0/src/pssapi/entities/reward_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/room.py` & `pssapi-0.5.0/src/pssapi/entities/room.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/room_design.py` & `pssapi-0.5.0/src/pssapi/entities/room_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/room_design_purchase.py` & `pssapi-0.5.0/src/pssapi/entities/room_design_purchase.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/room_design_sprite.py` & `pssapi-0.5.0/src/pssapi/entities/room_design_sprite.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/sale.py` & `pssapi-0.5.0/src/pssapi/entities/sale.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/season_design.py` & `pssapi-0.5.0/src/pssapi/entities/season_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/setting.py` & `pssapi-0.5.0/src/pssapi/entities/setting.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/ship.py` & `pssapi-0.5.0/src/pssapi/entities/ship.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/ship_design.py` & `pssapi-0.5.0/src/pssapi/entities/ship_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/situation_design.py` & `pssapi-0.5.0/src/pssapi/entities/situation_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/skin.py` & `pssapi-0.5.0/src/pssapi/entities/skin.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/skin_set.py` & `pssapi-0.5.0/src/pssapi/entities/skin_set.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/star_system_marker.py` & `pssapi-0.5.0/src/pssapi/entities/star_system_marker.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/star_system_marker_generator.py` & `pssapi-0.5.0/src/pssapi/entities/star_system_marker_generator.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/task_design.py` & `pssapi-0.5.0/src/pssapi/entities/task_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/training_design.py` & `pssapi-0.5.0/src/pssapi/entities/training_design.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/user.py` & `pssapi-0.5.0/src/pssapi/entities/user.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/user_marker.py` & `pssapi-0.5.0/src/pssapi/entities/user_marker.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/entities/user_season.py` & `pssapi-0.5.0/src/pssapi/entities/user_season.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/__init__.py` & `pssapi-0.5.0/src/pssapi/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/achievement_type.py` & `pssapi-0.5.0/src/pssapi/enums/achievement_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/activity_type.py` & `pssapi-0.5.0/src/pssapi/enums/activity_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/change_type.py` & `pssapi-0.5.0/src/pssapi/enums/change_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/condition_type_category.py` & `pssapi-0.5.0/src/pssapi/enums/condition_type_category.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/condition_type_comparison.py` & `pssapi-0.5.0/src/pssapi/enums/condition_type_comparison.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/condition_type_parameter.py` & `pssapi-0.5.0/src/pssapi/enums/condition_type_parameter.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/currency_type.py` & `pssapi-0.5.0/src/pssapi/enums/currency_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/device_type.py` & `pssapi-0.5.0/src/pssapi/enums/device_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/enhancement_type.py` & `pssapi-0.5.0/src/pssapi/enums/enhancement_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/item_design_flag_type.py` & `pssapi-0.5.0/src/pssapi/enums/item_design_flag_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/item_sub_type.py` & `pssapi-0.5.0/src/pssapi/enums/item_sub_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/language_key.py` & `pssapi-0.5.0/src/pssapi/enums/language_key.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/message_type.py` & `pssapi-0.5.0/src/pssapi/enums/message_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/objective_type.py` & `pssapi-0.5.0/src/pssapi/enums/objective_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/outcome_type.py` & `pssapi-0.5.0/src/pssapi/enums/outcome_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/pusher_channel_type.py` & `pssapi-0.5.0/src/pssapi/enums/pusher_channel_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/research_design_type.py` & `pssapi-0.5.0/src/pssapi/enums/research_design_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/room_type.py` & `pssapi-0.5.0/src/pssapi/enums/room_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/sale_item_mask.py` & `pssapi-0.5.0/src/pssapi/enums/sale_item_mask.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/setting_flags.py` & `pssapi-0.5.0/src/pssapi/enums/setting_flags.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/special_ability_type.py` & `pssapi-0.5.0/src/pssapi/enums/special_ability_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/str_enum_base.py` & `pssapi-0.5.0/src/pssapi/enums/str_enum_base.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/task_category.py` & `pssapi-0.5.0/src/pssapi/enums/task_category.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/user_status.py` & `pssapi-0.5.0/src/pssapi/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/enums/user_type.py` & `pssapi-0.5.0/src/pssapi/enums/user_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/pusher/channel.py` & `pssapi-0.5.0/src/pssapi/pusher/channel.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/pusher/pusher.py` & `pssapi-0.5.0/src/pssapi/pusher/pusher.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/__init__.py` & `pssapi-0.5.0/src/pssapi/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .ladder_service import LadderService
 from .league_service import LeagueService
 from .live_ops_service import LiveOpsService
 from .market_service import MarketService
 from .message_service import MessageService
 from .mission_service import MissionService
 from .promotion_service import PromotionService
+from .public_service import PublicService
 from .research_service import ResearchService
 from .reward_service import RewardService
 from .room_design_sprite_service import RoomDesignSpriteService
 from .room_service import RoomService
 from .season_service import SeasonService
 from .setting_service import SettingService
 from .ship_service import ShipService
@@ -47,14 +48,15 @@
     LadderService.__name__,
     LeagueService.__name__,
     LiveOpsService.__name__,
     MarketService.__name__,
     MessageService.__name__,
     MissionService.__name__,
     PromotionService.__name__,
+    PublicService.__name__,
     ResearchService.__name__,
     RewardService.__name__,
     RoomDesignSpriteService.__name__,
     RoomService.__name__,
     SeasonService.__name__,
     SettingService.__name__,
     ShipService.__name__,
```

### Comparing `pssapi-0.4.1/src/pssapi/services/achievement_service.py` & `pssapi-0.5.0/src/pssapi/services/achievement_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/alliance_service.py` & `pssapi-0.5.0/src/pssapi/services/alliance_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/animation_service.py` & `pssapi-0.5.0/src/pssapi/services/animation_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/background_service.py` & `pssapi-0.5.0/src/pssapi/services/background_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/challenge_service.py` & `pssapi-0.5.0/src/pssapi/services/challenge_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/character_service.py` & `pssapi-0.5.0/src/pssapi/services/character_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/collection_service.py` & `pssapi-0.5.0/src/pssapi/services/collection_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/division_service.py` & `pssapi-0.5.0/src/pssapi/services/division_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/file_service.py` & `pssapi-0.5.0/src/pssapi/services/file_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/galaxy_service.py` & `pssapi-0.5.0/src/pssapi/services/galaxy_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/item_service.py` & `pssapi-0.5.0/src/pssapi/services/item_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/ladder_service.py` & `pssapi-0.5.0/src/pssapi/services/ladder_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/league_service.py` & `pssapi-0.5.0/src/pssapi/services/league_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/live_ops_service.py` & `pssapi-0.5.0/src/pssapi/services/live_ops_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/market_service.py` & `pssapi-0.5.0/src/pssapi/services/market_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/message_service.py` & `pssapi-0.5.0/src/pssapi/services/message_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/mission_service.py` & `pssapi-0.5.0/src/pssapi/services/mission_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/promotion_service.py` & `pssapi-0.5.0/src/pssapi/services/promotion_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/__init__.py` & `pssapi-0.5.0/src/pssapi/services/raw/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from . import ladder_service_raw as LadderServiceRaw
 from . import league_service_raw as LeagueServiceRaw
 from . import live_ops_service_raw as LiveOpsServiceRaw
 from . import market_service_raw as MarketServiceRaw
 from . import message_service_raw as MessageServiceRaw
 from . import mission_service_raw as MissionServiceRaw
 from . import promotion_service_raw as PromotionServiceRaw
+from . import public_service_raw as PublicServiceRaw
 from . import research_service_raw as ResearchServiceRaw
 from . import reward_service_raw as RewardServiceRaw
 from . import room_design_sprite_service_raw as RoomDesignSpriteServiceRaw
 from . import room_service_raw as RoomServiceRaw
 from . import season_service_raw as SeasonServiceRaw
 from . import setting_service_raw as SettingServiceRaw
 from . import ship_service_raw as ShipServiceRaw
@@ -47,14 +48,15 @@
     LadderServiceRaw.__name__,
     LeagueServiceRaw.__name__,
     LiveOpsServiceRaw.__name__,
     MarketServiceRaw.__name__,
     MessageServiceRaw.__name__,
     MissionServiceRaw.__name__,
     PromotionServiceRaw.__name__,
+    PublicServiceRaw.__name__,
     ResearchServiceRaw.__name__,
     RewardServiceRaw.__name__,
     RoomDesignSpriteServiceRaw.__name__,
     RoomServiceRaw.__name__,
     SeasonServiceRaw.__name__,
     SettingServiceRaw.__name__,
     ShipServiceRaw.__name__,
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/achievement_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/achievement_service_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_achievement_designs_2(production_server: str, design_version: int, language_key: str, **params) -> _List[_AchievementDesign]:
     params = {"designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_AchievementDesign, "AchievementDesigns", True),), "AchievementDesigns", production_server, LIST_ACHIEVEMENT_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_AchievementDesign, "AchievementDesigns", True),), "AchievementDesigns", production_server, LIST_ACHIEVEMENT_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/alliance_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/alliance_service_raw.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,51 +25,55 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def get_alliance(production_server: str, access_token: str, alliance_id: int, **params) -> _Alliance:
     params = {"accessToken": access_token, "allianceId": alliance_id, **params}
-    result = await _core.get_entities_from_path(((_Alliance, "Alliance", False),), "GetAlliance", production_server, GET_ALLIANCE_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Alliance, "Alliance", False),), "GetAlliance", production_server, GET_ALLIANCE_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def get_user(production_server: str, access_token: str, user_id: int, **params) -> _User:
     params = {"accessToken": access_token, "userId": user_id, **params}
-    result = await _core.get_entities_from_path(((_User, "User", False),), "GetUser", production_server, GET_USER_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_User, "User", False),), "GetUser", production_server, GET_USER_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_alliances_by_championship_score_ranking(production_server: str, access_token: str, from_: int, to: int, **params) -> _List[_Alliance]:
     params = {"accessToken": access_token, "from": from_, "to": to, **params}
-    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_BY_CHAMPIONSHIP_SCORE_RANKING_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_BY_CHAMPIONSHIP_SCORE_RANKING_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_alliances_by_ranking(production_server: str, skip: int, take: int, **params) -> _List[_Alliance]:
     params = {"skip": skip, "take": take, **params}
-    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_BY_RANKING_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_BY_RANKING_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_alliances_with_division(production_server: str, division_design_id: int, **params) -> _List[_Alliance]:
     params = {"divisionDesignId": division_design_id, **params}
-    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_WITH_DIVISION_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, LIST_ALLIANCES_WITH_DIVISION_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_characters_given_in_alliance(production_server: str, access_token: str, alliance_id: int, skip: int, take: int, **params) -> _List[_Character]:
     params = {"accessToken": access_token, "allianceId": alliance_id, "skip": skip, "take": take, **params}
-    result = await _core.get_entities_from_path(((_Character, "Characters", True),), "Characters", production_server, LIST_CHARACTERS_GIVEN_IN_ALLIANCE_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_Character, "Characters", True),), "Characters", production_server, LIST_CHARACTERS_GIVEN_IN_ALLIANCE_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_users_2(production_server: str, access_token: str, alliance_id: int, skip: int, take: int, **params) -> _Tuple[_List[_Message], _List[_User]]:
     params = {"accessToken": access_token, "allianceId": alliance_id, "skip": skip, "take": take, **params}
-    result = await _core.get_entities_from_path(((_Message, "Messages", True), (_User, "Users", True)), "ListUsers", production_server, LIST_USERS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Message, "Messages", True), (_User, "Users", True)), "ListUsers", production_server, LIST_USERS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def search_alliances(production_server: str, access_token: str, name: str, skip: int, take: int, **params) -> _List[_Alliance]:
     params = {"accessToken": access_token, "name": name, "skip": skip, "take": take, **params}
-    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, SEARCH_ALLIANCES_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Alliance, "Alliances", True),), "Alliances", production_server, SEARCH_ALLIANCES_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/animation_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/animation_service_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_animations(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_Animation]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_Animation, "Animations", True),), "Animations", production_server, LIST_ANIMATIONS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Animation, "Animations", True),), "Animations", production_server, LIST_ANIMATIONS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/background_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/background_service_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_backgrounds(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_Background]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_Background, "Backgrounds", True),), "Backgrounds", production_server, LIST_BACKGROUNDS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Background, "Backgrounds", True),), "Backgrounds", production_server, LIST_BACKGROUNDS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/challenge_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/training_service_raw.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,23 @@
     This file has been generated automatically.
     Any changes to this file will be lost eventually.
 """
 
 from typing import List as _List
 
 from ... import core as _core
-from ...entities import ChallengeDesign as _ChallengeDesign
+from ...entities import TrainingDesign as _TrainingDesign
 
 # ---------- Constants ----------
 
-LIST_ALL_CHALLENGE_DESIGNS_2_BASE_PATH: str = "ChallengeService/ListAllChallengeDesigns2"
+LIST_ALL_TRAINING_DESIGNS_2_BASE_PATH: str = "TrainingService/ListAllTrainingDesigns2"
 
 
 # ---------- Endpoints ----------
 
 
-async def list_all_challenge_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_ChallengeDesign]:
+async def list_all_training_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_TrainingDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ChallengeDesign, "ChallengeDesigns", True),), "ChallengeDesigns", production_server, LIST_ALL_CHALLENGE_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_TrainingDesign, "TrainingDesigns", True),), "TrainingDesigns", production_server, LIST_ALL_TRAINING_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/character_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/character_service_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,34 +22,36 @@
 
 # ---------- Endpoints ----------
 
 
 async def list_all_character_design_actions(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_CharacterDesignAction]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
     result = await _core.get_entities_from_path(
-        ((_CharacterDesignAction, "CharacterDesignActions", True),), "CharacterDesignActions", production_server, LIST_ALL_CHARACTER_DESIGN_ACTIONS_BASE_PATH, "GET", **params
+        ((_CharacterDesignAction, "CharacterDesignActions", True),), "CharacterDesignActions", production_server, LIST_ALL_CHARACTER_DESIGN_ACTIONS_BASE_PATH, "GET", response_gzipped=False, **params
     )
     return result
 
 
 async def list_all_character_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_CharacterDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_CharacterDesign, "CharacterDesigns", True),), "CharacterDesigns", production_server, LIST_ALL_CHARACTER_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_CharacterDesign, "CharacterDesigns", True),), "CharacterDesigns", production_server, LIST_ALL_CHARACTER_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_all_draw_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_DrawDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_DrawDesign, "DrawDesigns", True),), "DrawDesigns", production_server, LIST_ALL_DRAW_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_DrawDesign, "DrawDesigns", True),), "DrawDesigns", production_server, LIST_ALL_DRAW_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def prestige_character_from(production_server: str, character_design_id: int, **params) -> _List[_Prestige]:
     params = {"characterDesignId": character_design_id, **params}
-    result = await _core.get_entities_from_path(((_Prestige, "Prestiges", True),), "Prestiges", production_server, PRESTIGE_CHARACTER_FROM_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Prestige, "Prestiges", True),), "Prestiges", production_server, PRESTIGE_CHARACTER_FROM_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def prestige_character_to(production_server: str, character_design_id: int, **params) -> _List[_Prestige]:
     params = {"characterDesignId": character_design_id, **params}
-    result = await _core.get_entities_from_path(((_Prestige, "Prestiges", True),), "Prestiges", production_server, PRESTIGE_CHARACTER_TO_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Prestige, "Prestiges", True),), "Prestiges", production_server, PRESTIGE_CHARACTER_TO_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/collection_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/situation_service_raw.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,23 @@
     This file has been generated automatically.
     Any changes to this file will be lost eventually.
 """
 
 from typing import List as _List
 
 from ... import core as _core
-from ...entities import CollectionDesign as _CollectionDesign
+from ...entities import SituationDesign as _SituationDesign
 
 # ---------- Constants ----------
 
-LIST_ALL_COLLECTION_DESIGNS_BASE_PATH: str = "CollectionService/ListAllCollectionDesigns"
+LIST_SITUATION_DESIGNS_BASE_PATH: str = "SituationService/ListSituationDesigns"
 
 
 # ---------- Endpoints ----------
 
 
-async def list_all_collection_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_CollectionDesign]:
+async def list_situation_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_SituationDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_CollectionDesign, "CollectionDesigns", True),), "CollectionDesigns", production_server, LIST_ALL_COLLECTION_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_SituationDesign, "SituationDesigns", True),), "SituationDesigns", production_server, LIST_SITUATION_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/design_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/design_service_raw.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,21 +36,24 @@
 from ...entities import SituationDesign as _SituationDesign
 from ...entities import Skin as _Skin
 from ...entities import SkinSet as _SkinSet
 from ...entities import Sprite as _Sprite
 from ...entities import StarSystem as _StarSystem
 from ...entities import StarSystemLink as _StarSystemLink
 from ...entities import StarSystemMarkerGenerator as _StarSystemMarkerGenerator
+from ...entities import TaskDesign as _TaskDesign
 from ...entities import TrainingDesign as _TrainingDesign
 
 # ---------- Constants ----------
 
 LIST_ALL_DESIGNS_2_BASE_PATH: str = "DesignService/ListAllDesigns2"
 LIST_ALL_DESIGNS_4_BASE_PATH: str = "DesignService/ListAllDesigns4"
 LIST_ALL_DESIGNS_5_BASE_PATH: str = "DesignService/ListAllDesigns5"
+LIST_ALL_DYNAMIC_DESIGNS_BASE_PATH: str = "DesignService/ListAllDynamicDesigns"
+LIST_ALL_STATIC_DESIGNS_BASE_PATH: str = "DesignService/ListAllStaticDesigns"
 
 
 # ---------- Endpoints ----------
 
 
 async def list_all_designs_2(
     production_server: str,
@@ -187,14 +190,15 @@
             (_StarSystem, "StarSystems", True),
             (_TrainingDesign, "TrainingDesigns", True),
         ),
         "ListAllDesigns",
         production_server,
         LIST_ALL_DESIGNS_2_BASE_PATH,
         "GET",
+        response_gzipped=False,
         **params,
     )
     return result
 
 
 async def list_all_designs_4(
     production_server: str,
@@ -343,14 +347,15 @@
             (_StarSystem, "StarSystems", True),
             (_TrainingDesign, "TrainingDesigns", True),
         ),
         "ListAllDesigns",
         production_server,
         LIST_ALL_DESIGNS_4_BASE_PATH,
         "GET",
+        response_gzipped=False,
         **params,
     )
     return result
 
 
 async def list_all_designs_5(
     production_server: str,
@@ -505,10 +510,186 @@
             (_StarSystem, "StarSystems", True),
             (_TrainingDesign, "TrainingDesigns", True),
         ),
         "ListAllDesigns",
         production_server,
         LIST_ALL_DESIGNS_5_BASE_PATH,
         "GET",
+        response_gzipped=False,
+        **params,
+    )
+    return result
+
+
+async def list_all_dynamic_designs(
+    production_server: str, language_key: str, list_all_promotion_design_version: int, list_all_task_design_version: int, list_item_design_version: int, **params
+) -> _Tuple[_List[_ItemDesign], _List[_PromotionDesign], _List[_TaskDesign]]:
+    params = {
+        "LanguageKey": language_key,
+        "ListAllPromotionDesignVersion": list_all_promotion_design_version,
+        "ListAllTaskDesignVersion": list_all_task_design_version,
+        "ListItemDesignVersion": list_item_design_version,
+        **params,
+    }
+    result = await _core.get_entities_from_path(
+        ((_ItemDesign, "ItemDesigns", True), (_PromotionDesign, "PromotionDesigns", True), (_TaskDesign, "TaskDesigns", True)),
+        "ListAllDynamicDesigns",
+        production_server,
+        LIST_ALL_DYNAMIC_DESIGNS_BASE_PATH,
+        "GET",
+        response_gzipped=True,
+        **params,
+    )
+    return result
+
+
+async def list_all_static_designs(
+    production_server: str,
+    language_key: str,
+    list_achievement_design_version: int,
+    list_action_type_version: int,
+    list_all_challenge_design_version: int,
+    list_all_character_design_action_version: int,
+    list_all_character_design_version: int,
+    list_all_collection_design_version: int,
+    list_all_division_design_version: int,
+    list_all_draw_design_version: int,
+    list_all_mission_design_version: int,
+    list_all_news_design_version: int,
+    list_all_research_design_version: int,
+    list_all_reward_design_version: int,
+    list_all_ship_design_version: int,
+    list_all_situation_design_version: int,
+    list_all_training_design_version: int,
+    list_animation_version: int,
+    list_asset_version: int,
+    list_background_version: int,
+    list_condition_type_version: int,
+    list_craft_design_version: int,
+    list_file_version: int,
+    list_item_design_action_version: int,
+    list_league_version: int,
+    list_marker_generator_design_version: int,
+    list_missile_design_version: int,
+    list_room_design_purchase_version: int,
+    list_room_design_sprite_version: int,
+    list_room_design_version: int,
+    list_season_design_version: int,
+    list_skin_set_version: int,
+    list_skin_version: int,
+    list_sprite_version: int,
+    list_star_system_link_version: int,
+    list_star_system_version: int,
+    **params,
+) -> _Tuple[
+    _List[_AchievementDesign],
+    _List[_Animation],
+    _List[_Background],
+    _List[_ChallengeDesign],
+    _List[_CharacterDesignAction],
+    _List[_CharacterDesign],
+    _List[_CollectionDesign],
+    _List[_CraftDesign],
+    _List[_DivisionDesign],
+    _List[_DrawDesign],
+    _List[_File],
+    _List[_ItemDesignAction],
+    _List[_League],
+    _List[_MissileDesign],
+    _List[_MissionDesign],
+    _List[_NewsDesign],
+    _List[_ResearchDesign],
+    _List[_RewardDesign],
+    _List[_RoomDesignPurchase],
+    _List[_RoomDesignSprite],
+    _List[_RoomDesign],
+    _List[_SeasonDesign],
+    _List[_ShipDesign],
+    _List[_SituationDesign],
+    _List[_SkinSet],
+    _List[_Skin],
+    _List[_Sprite],
+    _List[_StarSystemLink],
+    _List[_StarSystemMarkerGenerator],
+    _List[_StarSystem],
+    _List[_TrainingDesign],
+]:
+    params = {
+        "LanguageKey": language_key,
+        "ListAchievementDesignVersion": list_achievement_design_version,
+        "ListActionTypeVersion": list_action_type_version,
+        "ListAllChallengeDesignVersion": list_all_challenge_design_version,
+        "ListAllCharacterDesignActionVersion": list_all_character_design_action_version,
+        "ListAllCharacterDesignVersion": list_all_character_design_version,
+        "ListAllCollectionDesignVersion": list_all_collection_design_version,
+        "ListAllDivisionDesignVersion": list_all_division_design_version,
+        "ListAllDrawDesignVersion": list_all_draw_design_version,
+        "ListAllMissionDesignVersion": list_all_mission_design_version,
+        "ListAllNewsDesignVersion": list_all_news_design_version,
+        "ListAllResearchDesignVersion": list_all_research_design_version,
+        "ListAllRewardDesignVersion": list_all_reward_design_version,
+        "ListAllShipDesignVersion": list_all_ship_design_version,
+        "ListAllSituationDesignVersion": list_all_situation_design_version,
+        "ListAllTrainingDesignVersion": list_all_training_design_version,
+        "ListAnimationVersion": list_animation_version,
+        "ListAssetVersion": list_asset_version,
+        "ListBackgroundVersion": list_background_version,
+        "ListConditionTypeVersion": list_condition_type_version,
+        "ListCraftDesignVersion": list_craft_design_version,
+        "ListFileVersion": list_file_version,
+        "ListItemDesignActionVersion": list_item_design_action_version,
+        "ListLeagueVersion": list_league_version,
+        "ListMarkerGeneratorDesignVersion": list_marker_generator_design_version,
+        "ListMissileDesignVersion": list_missile_design_version,
+        "ListRoomDesignPurchaseVersion": list_room_design_purchase_version,
+        "ListRoomDesignSpriteVersion": list_room_design_sprite_version,
+        "ListRoomDesignVersion": list_room_design_version,
+        "ListSeasonDesignVersion": list_season_design_version,
+        "ListSkinSetVersion": list_skin_set_version,
+        "ListSkinVersion": list_skin_version,
+        "ListSpriteVersion": list_sprite_version,
+        "ListStarSystemLinkVersion": list_star_system_link_version,
+        "ListStarSystemVersion": list_star_system_version,
+        **params,
+    }
+    result = await _core.get_entities_from_path(
+        (
+            (_AchievementDesign, "AchievementDesigns", True),
+            (_Animation, "Animations", True),
+            (_Background, "Backgrounds", True),
+            (_ChallengeDesign, "ChallengeDesigns", True),
+            (_CharacterDesignAction, "CharacterDesignActions", True),
+            (_CharacterDesign, "CharacterDesigns", True),
+            (_CollectionDesign, "CollectionDesigns", True),
+            (_CraftDesign, "CraftDesigns", True),
+            (_DivisionDesign, "DivisionDesigns", True),
+            (_DrawDesign, "DrawDesigns", True),
+            (_File, "Files", True),
+            (_ItemDesignAction, "ItemDesignActions", True),
+            (_League, "Leagues", True),
+            (_MissileDesign, "MissileDesigns", True),
+            (_MissionDesign, "MissionDesigns", True),
+            (_NewsDesign, "NewsDesigns", True),
+            (_ResearchDesign, "ResearchDesigns", True),
+            (_RewardDesign, "RewardDesigns", True),
+            (_RoomDesignPurchase, "RoomDesignPurchases", True),
+            (_RoomDesignSprite, "RoomDesignSprites", True),
+            (_RoomDesign, "RoomDesigns", True),
+            (_SeasonDesign, "SeasonDesigns", True),
+            (_ShipDesign, "ShipDesigns", True),
+            (_SituationDesign, "SituationDesigns", True),
+            (_SkinSet, "SkinSets", True),
+            (_Skin, "Skins", True),
+            (_Sprite, "Sprites", True),
+            (_StarSystemLink, "StarSystemLinks", True),
+            (_StarSystemMarkerGenerator, "StarSystemMarkerGenerators", True),
+            (_StarSystem, "StarSystems", True),
+            (_TrainingDesign, "TrainingDesigns", True),
+        ),
+        "ListAllStaticDesigns",
+        production_server,
+        LIST_ALL_STATIC_DESIGNS_BASE_PATH,
+        "GET",
+        response_gzipped=True,
         **params,
     )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/division_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/promotion_service_raw.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,23 @@
     This file has been generated automatically.
     Any changes to this file will be lost eventually.
 """
 
 from typing import List as _List
 
 from ... import core as _core
-from ...entities import DivisionDesign as _DivisionDesign
+from ...entities import PromotionDesign as _PromotionDesign
 
 # ---------- Constants ----------
 
-LIST_ALL_DIVISION_DESIGNS_2_BASE_PATH: str = "DivisionService/ListAllDivisionDesigns2"
+LIST_ALL_PROMOTION_DESIGNS_2_BASE_PATH: str = "PromotionService/ListAllPromotionDesigns2"
 
 
 # ---------- Endpoints ----------
 
 
-async def list_all_division_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_DivisionDesign]:
+async def list_all_promotion_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_PromotionDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_DivisionDesign, "DivisionDesigns", True),), "DivisionDesigns", production_server, LIST_ALL_DIVISION_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_PromotionDesign, "PromotionDesigns", True),), "PromotionDesigns", production_server, LIST_ALL_PROMOTION_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/file_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/file_service_raw.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_files_4(production_server: str, design_version: int, language_key: str, **params) -> _List[_File]:
     params = {"designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_File, "Files", True),), "Files", production_server, LIST_FILES_4_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_File, "Files", True),), "Files", production_server, LIST_FILES_4_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_sprites_2(production_server: str, design_version: int, language_key: str, **params) -> _List[_Sprite]:
     params = {"designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_Sprite, "Sprites", True),), "Sprites", production_server, LIST_SPRITES_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Sprite, "Sprites", True),), "Sprites", production_server, LIST_SPRITES_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/galaxy_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/galaxy_service_raw.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,54 +27,65 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def go_to(production_server: str, access_token: str, checksum: str, client_date_time: str, star_system_id: int, **params) -> _Ship:
     params = {"accessToken": access_token, "checksum": checksum, "clientDateTime": client_date_time, "starSystemId": star_system_id, **params}
-    result = await _core.get_entities_from_path(((_Ship, "Ship", False),), "GoTo", production_server, GO_TO_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_Ship, "Ship", False),), "GoTo", production_server, GO_TO_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def list_marker_generator_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_StarSystemMarkerGenerator]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
     result = await _core.get_entities_from_path(
-        ((_StarSystemMarkerGenerator, "StarSystemMarkerGenerators", True),), "StarSystemMarkerGenerators", production_server, LIST_MARKER_GENERATOR_DESIGNS_BASE_PATH, "GET", **params
+        ((_StarSystemMarkerGenerator, "StarSystemMarkerGenerators", True),),
+        "StarSystemMarkerGenerators",
+        production_server,
+        LIST_MARKER_GENERATOR_DESIGNS_BASE_PATH,
+        "GET",
+        response_gzipped=False,
+        **params,
     )
     return result
 
 
 async def list_planets(production_server: str, design_version: int, **params) -> _List[_Planet]:
     params = {"designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_Planet, "Planets", True),), "Planets", production_server, LIST_PLANETS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Planet, "Planets", True),), "Planets", production_server, LIST_PLANETS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_star_system_links(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_StarSystemLink]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_StarSystemLink, "StarSystemLinks", True),), "StarSystemLinks", production_server, LIST_STAR_SYSTEM_LINKS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_StarSystemLink, "StarSystemLinks", True),), "StarSystemLinks", production_server, LIST_STAR_SYSTEM_LINKS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_star_system_markers(production_server: str, access_token: str, client_date_time: str, **params) -> _List[_StarSystemMarker]:
     params = {"accessToken": access_token, "clientDateTime": client_date_time, **params}
-    result = await _core.get_entities_from_path(((_StarSystemMarker, "StarSystemMarkers", True),), "StarSystemMarkers", production_server, LIST_STAR_SYSTEM_MARKERS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_StarSystemMarker, "StarSystemMarkers", True),), "StarSystemMarkers", production_server, LIST_STAR_SYSTEM_MARKERS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_star_system_markers_and_user_markers(production_server: str, access_token: str, **params) -> _Tuple[_List[_StarSystemMarker], _List[_UserMarker]]:
     params = {"accessToken": access_token, **params}
     result = await _core.get_entities_from_path(
         ((_StarSystemMarker, "StarSystemMarkers", True), (_UserMarker, "UserMarkers", True)),
         "ListStarSystemMarkersAndUserMarkers",
         production_server,
         LIST_STAR_SYSTEM_MARKERS_AND_USER_MARKERS_BASE_PATH,
         "GET",
+        response_gzipped=False,
         **params,
     )
     return result
 
 
 async def list_star_systems(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_StarSystem]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_StarSystem, "StarSystems", True),), "StarSystems", production_server, LIST_STAR_SYSTEMS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_StarSystem, "StarSystems", True),), "StarSystems", production_server, LIST_STAR_SYSTEMS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/history_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/history_service_raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def price_history(production_server: str, item_design_id: int, **params) -> _History:
     params = {"itemDesignId": item_design_id, **params}
-    result = await _core.get_entities_from_path(((_History, "History", False),), "Histories", production_server, PRICE_HISTORY_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_History, "History", False),), "Histories", production_server, PRICE_HISTORY_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/item_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/item_service_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_item_design_actions(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_ItemDesignAction]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_ItemDesignAction, "ItemDesignActions", True),), "ItemDesignActions", production_server, LIST_ITEM_DESIGN_ACTIONS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_ItemDesignAction, "ItemDesignActions", True),), "ItemDesignActions", production_server, LIST_ITEM_DESIGN_ACTIONS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_item_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_ItemDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ItemDesign, "ItemDesigns", True),), "ItemDesigns", production_server, LIST_ITEM_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_ItemDesign, "ItemDesigns", True),), "ItemDesigns", production_server, LIST_ITEM_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/ladder_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/ladder_service_raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_users_by_championship_score_ranking(production_server: str, access_token: str, from_: int, to: int, **params) -> _List[_User]:
     params = {"accessToken": access_token, "from": from_, "to": to, **params}
-    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, LIST_USERS_BY_CHAMPIONSHIP_SCORE_RANKING_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, LIST_USERS_BY_CHAMPIONSHIP_SCORE_RANKING_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_users_by_ranking(production_server: str, access_token: str, from_: int, to: int, **params) -> _List[_User]:
     params = {"accessToken": access_token, "from": from_, "to": to, **params}
-    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, LIST_USERS_BY_RANKING_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, LIST_USERS_BY_RANKING_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/league_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/league_service_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_leagues_2(production_server: str, access_token: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_League]:
     params = {"accessToken": access_token, "clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_League, "Leagues", True),), "Leagues", production_server, LIST_LEAGUES_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_League, "Leagues", True),), "Leagues", production_server, LIST_LEAGUES_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/market_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/market_service_raw.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_sales_by_item_design_id(production_server: str, from_: int, item_design_id: int, sale_status: str, to: int, **params) -> _List[_Sale]:
     params = {"from": from_, "itemDesignId": item_design_id, "saleStatus": sale_status, "to": to, **params}
-    result = await _core.get_entities_from_path(((_Sale, "Sales", True),), "Sales", production_server, LIST_SALES_BY_ITEM_DESIGN_ID_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Sale, "Sales", True),), "Sales", production_server, LIST_SALES_BY_ITEM_DESIGN_ID_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/message_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/message_service_raw.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,41 +30,45 @@
         "itemSubType": item_sub_type,
         "rarity": rarity,
         "skip": skip,
         "take": take,
         "userId": user_id,
         **params,
     }
-    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_ACTIVE_MARKETPLACE_MESSAGES_5_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_ACTIVE_MARKETPLACE_MESSAGES_5_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_messages_for_channel_key(production_server: str, access_token: str, channel_key: str, **params) -> _List[_Message]:
     params = {"accessToken": access_token, "channelKey": channel_key, **params}
-    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_MESSAGES_FOR_CHANNEL_KEY_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_MESSAGES_FOR_CHANNEL_KEY_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_private_messages(production_server: str, access_token: str, **params) -> _List[_Message]:
     params = {"accessToken": access_token, **params}
-    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_PRIVATE_MESSAGES_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Message, "Messages", True),), "Messages", production_server, LIST_PRIVATE_MESSAGES_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def send_message_3(production_server: str, access_token: str, channel_key: str, message: str, **params) -> _Message:
     params = {"AccessToken": access_token, "ChannelKey": channel_key, "Message": message, **params}
     content = _core.create_request_content(__SEND_MESSAGE_3_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_Message, "Message", False),), "SendMessage", production_server, SEND_MESSAGE_3_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_Message, "Message", False),), "SendMessage", production_server, SEND_MESSAGE_3_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __SEND_MESSAGE_3_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","ChannelKey":"str","Message":"str"}'
 
 
 async def send_private_message_3(production_server: str, access_token: str, message: str, to_user_id: int, **params) -> _Message:
     params = {"AccessToken": access_token, "Message": message, "ToUserId": to_user_id, **params}
     content = _core.create_request_content(__SEND_PRIVATE_MESSAGE_3_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_Message, "Message", False),), "SendMessage", production_server, SEND_PRIVATE_MESSAGE_3_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_Message, "Message", False),), "SendMessage", production_server, SEND_PRIVATE_MESSAGE_3_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __SEND_PRIVATE_MESSAGE_3_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","Message":"str","ToUserId":"int"}'
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/mission_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/mission_service_raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,30 +29,35 @@
     params = {"accessToken": access_token, "checksum": checksum, "clientDateTime": client_date_time, "messageId": message_id, "missionDesignId": mission_design_id, **params}
     result = await _core.get_entities_from_path(
         ((_Battle, "Battle", False), (_MissionEvent, "MissionEvent", False), (_User, "User", False), (_MissionEvent, "MissionEvents", True)),
         "CreateMission",
         production_server,
         CREATE_MISSION_2_BASE_PATH,
         "POST",
+        response_gzipped=False,
         **params,
     )
     return result
 
 
 async def list_all_mission_designs_4(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_MissionDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_MissionDesign, "MissionDesigns", True),), "MissionDesigns", production_server, LIST_ALL_MISSION_DESIGNS_4_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_MissionDesign, "MissionDesigns", True),), "MissionDesigns", production_server, LIST_ALL_MISSION_DESIGNS_4_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def select_event_2(production_server: str, access_token: str, battle_id: int, checksum: str, client_date_time: str, mission_event_id: int, **params) -> _Battle:
     params = {"accessToken": access_token, "battleId": battle_id, "checksum": checksum, "clientDateTime": client_date_time, "missionEventId": mission_event_id, **params}
-    result = await _core.get_entities_from_path(((_Battle, "Battle", False),), "SelectEvent", production_server, SELECT_EVENT_2_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_Battle, "Battle", False),), "SelectEvent", production_server, SELECT_EVENT_2_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def select_event_3(
     production_server: str, access_token: str, battle_id: int, checksum: str, client_date_time: str, client_number: int, mission_event_id: int, **params
 ) -> _Tuple[_Battle, _User]:
     params = {"accessToken": access_token, "battleId": battle_id, "checksum": checksum, "clientDateTime": client_date_time, "clientNumber": client_number, "missionEventId": mission_event_id, **params}
-    result = await _core.get_entities_from_path(((_Battle, "Battle", False), (_User, "User", False)), "SelectEvent", production_server, SELECT_EVENT_3_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(
+        ((_Battle, "Battle", False), (_User, "User", False)), "SelectEvent", production_server, SELECT_EVENT_3_BASE_PATH, "POST", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/promotion_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/reward_service_raw.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,23 @@
     This file has been generated automatically.
     Any changes to this file will be lost eventually.
 """
 
 from typing import List as _List
 
 from ... import core as _core
-from ...entities import PromotionDesign as _PromotionDesign
+from ...entities import RewardDesign as _RewardDesign
 
 # ---------- Constants ----------
 
-LIST_ALL_PROMOTION_DESIGNS_2_BASE_PATH: str = "PromotionService/ListAllPromotionDesigns2"
+LIST_ALL_REWARD_DESIGNS_2_BASE_PATH: str = "RewardService/ListAllRewardDesigns2"
 
 
 # ---------- Endpoints ----------
 
 
-async def list_all_promotion_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_PromotionDesign]:
+async def list_all_reward_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_RewardDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_PromotionDesign, "PromotionDesigns", True),), "PromotionDesigns", production_server, LIST_ALL_PROMOTION_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_RewardDesign, "RewardDesigns", True),), "RewardDesigns", production_server, LIST_ALL_REWARD_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/research_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/research_service_raw.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_all_research_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_ResearchDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ResearchDesign, "ResearchDesigns", True),), "ResearchDesigns", production_server, LIST_ALL_RESEARCH_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_ResearchDesign, "ResearchDesigns", True),), "ResearchDesigns", production_server, LIST_ALL_RESEARCH_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/reward_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/division_service_raw.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,23 @@
     This file has been generated automatically.
     Any changes to this file will be lost eventually.
 """
 
 from typing import List as _List
 
 from ... import core as _core
-from ...entities import RewardDesign as _RewardDesign
+from ...entities import DivisionDesign as _DivisionDesign
 
 # ---------- Constants ----------
 
-LIST_ALL_REWARD_DESIGNS_2_BASE_PATH: str = "RewardService/ListAllRewardDesigns2"
+LIST_ALL_DIVISION_DESIGNS_2_BASE_PATH: str = "DivisionService/ListAllDivisionDesigns2"
 
 
 # ---------- Endpoints ----------
 
 
-async def list_all_reward_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_RewardDesign]:
+async def list_all_division_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_DivisionDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_RewardDesign, "RewardDesigns", True),), "RewardDesigns", production_server, LIST_ALL_REWARD_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_DivisionDesign, "DivisionDesigns", True),), "DivisionDesigns", production_server, LIST_ALL_DIVISION_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/room_design_sprite_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/room_design_sprite_service_raw.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_room_design_sprites(production_server: str, design_version: int, **params) -> _List[_RoomDesignSprite]:
     params = {"designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_RoomDesignSprite, "RoomDesignSprites", True),), "RoomDesignSprites", production_server, LIST_ROOM_DESIGN_SPRITES_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_RoomDesignSprite, "RoomDesignSprites", True),), "RoomDesignSprites", production_server, LIST_ROOM_DESIGN_SPRITES_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_room_design_sprites_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_RoomDesignSprite]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_RoomDesignSprite, "RoomDesignSprites", True),), "RoomDesignSprites", production_server, LIST_ROOM_DESIGN_SPRITES_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_RoomDesignSprite, "RoomDesignSprites", True),), "RoomDesignSprites", production_server, LIST_ROOM_DESIGN_SPRITES_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/room_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/room_service_raw.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,51 +26,59 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def get_missile_design(production_server: str, language_key: str, missile_design_id: int, **params) -> _MissileDesign:
     params = {"languageKey": language_key, "missileDesignId": missile_design_id, **params}
-    result = await _core.get_entities_from_path(((_MissileDesign, "MissileDesign", False),), "GetMissileDesign", production_server, GET_MISSILE_DESIGN_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_MissileDesign, "MissileDesign", False),), "GetMissileDesign", production_server, GET_MISSILE_DESIGN_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def get_room_design(production_server: str, language_key: str, room_design_id: int, **params) -> _RoomDesign:
     params = {"languageKey": language_key, "roomDesignId": room_design_id, **params}
-    result = await _core.get_entities_from_path(((_RoomDesign, "RoomDesign", False),), "GetRoomDesign", production_server, GET_ROOM_DESIGN_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_RoomDesign, "RoomDesign", False),), "GetRoomDesign", production_server, GET_ROOM_DESIGN_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_action_types_2(production_server: str, design_version: int, language_key: str, **params) -> _List[_ActionType]:
     params = {"designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ActionType, "ActionTypes", True),), "ActionTypes", production_server, LIST_ACTION_TYPES_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_ActionType, "ActionTypes", True),), "ActionTypes", production_server, LIST_ACTION_TYPES_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_condition_types_2(production_server: str, design_version: int, language_key: str, **params) -> _List[_ConditionType]:
     params = {"designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ConditionType, "ConditionTypes", True),), "ConditionTypes", production_server, LIST_CONDITION_TYPES_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_ConditionType, "ConditionTypes", True),), "ConditionTypes", production_server, LIST_CONDITION_TYPES_2_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_craft_designs(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_CraftDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_CraftDesign, "CraftDesigns", True),), "CraftDesigns", production_server, LIST_CRAFT_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_CraftDesign, "CraftDesigns", True),), "CraftDesigns", production_server, LIST_CRAFT_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_missile_designs(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_MissileDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_MissileDesign, "MissileDesigns", True),), "MissileDesigns", production_server, LIST_MISSILE_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_MissileDesign, "MissileDesigns", True),), "MissileDesigns", production_server, LIST_MISSILE_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_room_design_purchase(production_server: str, client_date_time: str, design_version: int, **params) -> _List[_RoomDesignPurchase]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, **params}
-    result = await _core.get_entities_from_path(((_RoomDesignPurchase, "RoomDesignPurchases", True),), "RoomDesignPurchases", production_server, LIST_ROOM_DESIGN_PURCHASE_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_RoomDesignPurchase, "RoomDesignPurchases", True),), "RoomDesignPurchases", production_server, LIST_ROOM_DESIGN_PURCHASE_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
 
 
 async def list_room_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_RoomDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_RoomDesign, "RoomDesigns", True),), "RoomDesigns", production_server, LIST_ROOM_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_RoomDesign, "RoomDesigns", True),), "RoomDesigns", production_server, LIST_ROOM_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/season_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/season_service_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_all_season_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_SeasonDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_SeasonDesign, "SeasonDesigns", True),), "SeasonDesigns", production_server, LIST_ALL_SEASON_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(
+        ((_SeasonDesign, "SeasonDesigns", True),), "SeasonDesigns", production_server, LIST_ALL_SEASON_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params
+    )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/setting_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/setting_service_raw.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def get_latest_version_3(production_server: str, device_type: str, language_key: str, **params) -> _Setting:
     params = {"deviceType": device_type, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_Setting, "Setting", False),), "GetLatestSetting", production_server, GET_LATEST_VERSION_3_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Setting, "Setting", False),), "GetLatestSetting", production_server, GET_LATEST_VERSION_3_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def get_latest_version_4(production_server: str, device_type: str, language_key: str, **params) -> _Setting:
     params = {"deviceType": device_type, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_Setting, "Setting", False),), "GetLatestSetting", production_server, GET_LATEST_VERSION_4_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Setting, "Setting", False),), "GetLatestSetting", production_server, GET_LATEST_VERSION_4_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_all_news_designs(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_NewsDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_NewsDesign, "NewsDesigns", True),), "NewsDesigns", production_server, LIST_ALL_NEWS_DESIGNS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_NewsDesign, "NewsDesigns", True),), "NewsDesigns", production_server, LIST_ALL_NEWS_DESIGNS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/ship_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/ship_service_raw.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def get_ship_by_user_id(production_server: str, access_token: str, client_date_time: str, user_id: int, **params) -> _Ship:
     params = {"accessToken": access_token, "clientDateTime": client_date_time, "userId": user_id, **params}
-    result = await _core.get_entities_from_path(((_Ship, "Ship", False),), "GetShipByUserId", production_server, GET_SHIP_BY_USER_ID_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Ship, "Ship", False),), "GetShipByUserId", production_server, GET_SHIP_BY_USER_ID_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def inspect_ship_2(production_server: str, access_token: str, user_id: int, **params) -> _Tuple[_Ship, _User]:
     params = {"accessToken": access_token, "userId": user_id, **params}
-    result = await _core.get_entities_from_path(((_Ship, "Ship", False), (_User, "User", False)), "InspectShip", production_server, INSPECT_SHIP_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_Ship, "Ship", False), (_User, "User", False)), "InspectShip", production_server, INSPECT_SHIP_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_all_ship_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_ShipDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_ShipDesign, "ShipDesigns", True),), "ShipDesigns", production_server, LIST_ALL_SHIP_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_ShipDesign, "ShipDesigns", True),), "ShipDesigns", production_server, LIST_ALL_SHIP_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/task_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/task_service_raw.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 
 # ---------- Endpoints ----------
 
 
 async def list_all_task_designs_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_TaskDesign]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_TaskDesign, "TaskDesigns", True),), "TaskDesigns", production_server, LIST_ALL_TASK_DESIGNS_2_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_TaskDesign, "TaskDesigns", True),), "TaskDesigns", production_server, LIST_ALL_TASK_DESIGNS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/raw/user_service_raw.py` & `pssapi-0.5.0/src/pssapi/services/raw/user_service_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,41 +21,43 @@
 ACCEPT_FRIEND_REQUEST_BASE_PATH: str = "UserService/AcceptFriendRequest"
 ADD_FRIEND_2_BASE_PATH: str = "UserService/AddFriend2"
 DECLINE_FRIEND_REQUEST_BASE_PATH: str = "UserService/DeclineFriendRequest"
 DEVICE_LOGIN_11_BASE_PATH: str = "UserService/DeviceLogin11"
 DEVICE_LOGIN_12_BASE_PATH: str = "UserService/DeviceLogin12"
 DEVICE_LOGIN_15_BASE_PATH: str = "UserService/DeviceLogin15"
 LIST_FRIENDS_BASE_PATH: str = "UserService/ListFriends"
+LIST_SKIN_SETS_2_BASE_PATH: str = "UserService/ListSkinSets2"
 LIST_SKINS_BASE_PATH: str = "UserService/ListSkins"
+LIST_SKINS_2_BASE_PATH: str = "UserService/ListSkins2"
 REMOVE_FRIEND_BASE_PATH: str = "UserService/RemoveFriend"
 SEARCH_USERS_BASE_PATH: str = "UserService/SearchUsers"
 STEAM_LOGIN_3_BASE_PATH: str = "UserService/SteamLogin3"
 STEAM_LOGIN_6_BASE_PATH: str = "UserService/SteamLogin6"
 USER_EMAIL_PASSWORD_AUTHORIZE_2_BASE_PATH: str = "UserService/UserEmailPasswordAuthorize2"
 USER_EMAIL_PASSWORD_AUTHORIZE_4_BASE_PATH: str = "UserService/UserEmailPasswordAuthorize4"
 
 
 # ---------- Endpoints ----------
 
 
 async def accept_friend_request(production_server: str, access_token: str, friend_user_id: int, **params) -> _Friend:
     params = {"accessToken": access_token, "friendUserId": friend_user_id, **params}
-    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "AcceptFriendRequest", production_server, ACCEPT_FRIEND_REQUEST_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "AcceptFriendRequest", production_server, ACCEPT_FRIEND_REQUEST_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def add_friend_2(production_server: str, access_token: str, friend_user_id: int, **params) -> _Friend:
     params = {"accessToken": access_token, "friendUserId": friend_user_id, **params}
-    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "AddFriend", production_server, ADD_FRIEND_2_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "AddFriend", production_server, ADD_FRIEND_2_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def decline_friend_request(production_server: str, access_token: str, friend_user_id: int, **params) -> _Friend:
     params = {"accessToken": access_token, "friendUserId": friend_user_id, **params}
-    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "DeclineFriendRequest", production_server, DECLINE_FRIEND_REQUEST_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_Friend, "Friend", False),), "DeclineFriendRequest", production_server, DECLINE_FRIEND_REQUEST_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def device_login_11(
     production_server: str,
     advertising_key: str,
     checksum: str,
@@ -76,15 +78,15 @@
         "device_type": device_type,
         "is_jail_broken": is_jail_broken,
         "language_key": language_key,
         "refresh_token": refresh_token,
         "signal": signal,
         **params,
     }
-    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_11_BASE_PATH, "POST", **params)
+    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_11_BASE_PATH, "POST", response_gzipped=False, **params)
     return result
 
 
 async def device_login_12(
     production_server: str,
     access_token: str,
     advertising_key: str,
@@ -120,15 +122,17 @@
         "OSBuild": os_build,
         "OsVersion": os_version,
         "RefreshToken": refresh_token,
         "Signal": signal,
         **params,
     }
     content = _core.create_request_content(__DEVICE_LOGIN_12_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_12_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_12_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __DEVICE_LOGIN_12_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","AdvertisingKey":"str","Checksum":"str","ClientDateTime":"datetime","DeviceKey":"str","DeviceType":"str","IsJailBroken":"bool","LanguageKey":"str","RefreshToken":"str","Signal":"bool","UserDeviceInfo":{"ClientBuild":"int","ClientVersion":"str","DeviceName":"str","Locale":"str","OSBuild":"int","OsVersion":"str"}}'
 
 
 async def device_login_15(
@@ -167,41 +171,55 @@
         "OSBuild": os_build,
         "OsVersion": os_version,
         "RefreshToken": refresh_token,
         "Signal": signal,
         **params,
     }
     content = _core.create_request_content(__DEVICE_LOGIN_15_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_15_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_UserLogin, "UserLogin", False),), "UserService", production_server, DEVICE_LOGIN_15_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __DEVICE_LOGIN_15_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","AdvertisingKey":"str","Checksum":"str","ClientDateTime":"datetime","DeviceKey":"str","DeviceType":"str","IsJailBroken":"bool","LanguageKey":"str","RefreshToken":"str","Signal":"bool","UserDeviceInfo":{"ClientBuild":"int","ClientVersion":"str","DeviceName":"str","Locale":"str","OSBuild":"int","OsVersion":"str"}}'
 
 
 async def list_friends(production_server: str, user_id: int, access_token: str, **params) -> _ListFriends:
     params = {"UserId": user_id, "accessToken": access_token, **params}
-    result = await _core.get_entities_from_path(((_ListFriends, "ListFriends", False),), "UserService", production_server, LIST_FRIENDS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_ListFriends, "ListFriends", False),), "UserService", production_server, LIST_FRIENDS_BASE_PATH, "GET", response_gzipped=False, **params)
+    return result
+
+
+async def list_skin_sets_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_SkinSet]:
+    params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
+    result = await _core.get_entities_from_path(((_SkinSet, "SkinSets", True),), "SkinSets", production_server, LIST_SKIN_SETS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def list_skins(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _Tuple[_List[_SkinSet], _List[_Skin]]:
     params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
-    result = await _core.get_entities_from_path(((_SkinSet, "SkinSets", True), (_Skin, "Skins", True)), "ListSkins", production_server, LIST_SKINS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_SkinSet, "SkinSets", True), (_Skin, "Skins", True)), "ListSkins", production_server, LIST_SKINS_BASE_PATH, "GET", response_gzipped=False, **params)
+    return result
+
+
+async def list_skins_2(production_server: str, client_date_time: str, design_version: int, language_key: str, **params) -> _List[_Skin]:
+    params = {"clientDateTime": client_date_time, "designVersion": design_version, "languageKey": language_key, **params}
+    result = await _core.get_entities_from_path(((_Skin, "Skins", True),), "Skins", production_server, LIST_SKINS_2_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def remove_friend(production_server: str, access_token: str, friend_user_id: int, **params) -> None:
     params = {"accessToken": access_token, "friendUserId": friend_user_id, **params}
-    await _core.get_entities_from_path((), None, production_server, REMOVE_FRIEND_BASE_PATH, "POST", **params)
+    await _core.get_entities_from_path((), None, production_server, REMOVE_FRIEND_BASE_PATH, "POST", response_gzipped=False, **params)
 
 
 async def search_users(production_server: str, search_string: str, **params) -> _List[_User]:
     params = {"searchString": search_string, **params}
-    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, SEARCH_USERS_BASE_PATH, "GET", **params)
+    result = await _core.get_entities_from_path(((_User, "Users", True),), "Users", production_server, SEARCH_USERS_BASE_PATH, "GET", response_gzipped=False, **params)
     return result
 
 
 async def steam_login_3(
     production_server: str,
     access_token: str,
     advertising_key: str,
@@ -239,15 +257,17 @@
         "OsVersion": os_version,
         "RefreshToken": refresh_token,
         "Signal": signal,
         "Ticket": ticket,
         **params,
     }
     content = _core.create_request_content(__STEAM_LOGIN_3_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, STEAM_LOGIN_3_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_UserLogin, "UserLogin", False),), "UserService", production_server, STEAM_LOGIN_3_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __STEAM_LOGIN_3_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","AdvertisingKey":null,"Checksum":"str","ClientDateTime":"str","DeviceKey":"str","DeviceType":"str","IsJailBroken":"bool","LanguageKey":"str","RefreshToken":"str","Signal":"bool","Ticket":"str","UserDeviceInfo":{"ClientBuild":"int","ClientVersion":"str","DeviceName":"str","Locale":"str","OSBuild":"int","OsVersion":"str"}}'
 
 
 async def steam_login_6(
@@ -288,27 +308,29 @@
         "OsVersion": os_version,
         "RefreshToken": refresh_token,
         "Signal": signal,
         "Ticket": ticket,
         **params,
     }
     content = _core.create_request_content(__STEAM_LOGIN_6_REQUEST_CONTENT_STRUCTURE, params, "json")
-    result = await _core.get_entities_from_path(((_UserLogin, "UserLogin", False),), "UserService", production_server, STEAM_LOGIN_6_BASE_PATH, "POST", request_content=content, **params)
+    result = await _core.get_entities_from_path(
+        ((_UserLogin, "UserLogin", False),), "UserService", production_server, STEAM_LOGIN_6_BASE_PATH, "POST", request_content=content, response_gzipped=False, **params
+    )
     return result
 
 
 __STEAM_LOGIN_6_REQUEST_CONTENT_STRUCTURE: str = '{"AccessToken":"str","AdvertisingKey":null,"Checksum":"str","ClientDateTime":"str","DeviceKey":"str","DeviceType":"str","IsJailBroken":"bool","LanguageKey":"str","RefreshToken":"str","Signal":"bool","Ticket":"str","UserDeviceInfo":{"ClientBuild":"int","ClientVersion":"str","DeviceName":"str","Locale":"str","OSBuild":"int","OsVersion":"str"}}'
 
 
 async def user_email_password_authorize_2(
     production_server: str, access_token: str, checksum: str, client_date_time: str, device_key: str, email: str, password: str, **params
 ) -> _UserEmailPasswordAuthorize:
     params = {"accessToken": access_token, "checksum": checksum, "clientDateTime": client_date_time, "deviceKey": device_key, "email": email, "password": password, **params}
     result = await _core.get_entities_from_path(
-        ((_UserEmailPasswordAuthorize, "UserEmailPasswordAuthorize", False),), "UserService", production_server, USER_EMAIL_PASSWORD_AUTHORIZE_2_BASE_PATH, "POST", **params
+        ((_UserEmailPasswordAuthorize, "UserEmailPasswordAuthorize", False),), "UserService", production_server, USER_EMAIL_PASSWORD_AUTHORIZE_2_BASE_PATH, "POST", response_gzipped=False, **params
     )
     return result
 
 
 async def user_email_password_authorize_4(
     production_server: str, access_token: str, checksum: str, client_date_time: str, device_key: str, email: str, is_web: bool, language_key: str, password: str, **params
 ) -> _UserEmailPasswordAuthorize:
@@ -320,10 +342,10 @@
         "email": email,
         "isWeb": is_web,
         "languageKey": language_key,
         "password": password,
         **params,
     }
     result = await _core.get_entities_from_path(
-        ((_UserEmailPasswordAuthorize, "UserEmailPasswordAuthorize", False),), "UserService", production_server, USER_EMAIL_PASSWORD_AUTHORIZE_4_BASE_PATH, "POST", **params
+        ((_UserEmailPasswordAuthorize, "UserEmailPasswordAuthorize", False),), "UserService", production_server, USER_EMAIL_PASSWORD_AUTHORIZE_4_BASE_PATH, "POST", response_gzipped=False, **params
     )
     return result
```

### Comparing `pssapi-0.4.1/src/pssapi/services/research_service.py` & `pssapi-0.5.0/src/pssapi/services/research_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/reward_service.py` & `pssapi-0.5.0/src/pssapi/services/reward_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/room_design_sprite_service.py` & `pssapi-0.5.0/src/pssapi/services/room_design_sprite_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/room_service.py` & `pssapi-0.5.0/src/pssapi/services/room_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/season_service.py` & `pssapi-0.5.0/src/pssapi/services/season_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/service_base.py` & `pssapi-0.5.0/src/pssapi/services/service_base.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/setting_service.py` & `pssapi-0.5.0/src/pssapi/services/setting_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/ship_service.py` & `pssapi-0.5.0/src/pssapi/services/ship_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/situation_service.py` & `pssapi-0.5.0/src/pssapi/services/situation_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/task_service.py` & `pssapi-0.5.0/src/pssapi/services/task_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/training_service.py` & `pssapi-0.5.0/src/pssapi/services/training_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/services/user_service.py` & `pssapi-0.5.0/src/pssapi/services/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime as _datetime
 import hashlib as _hashlib
 import random as _random
 import string as _string
 from typing import List as _List
-from typing import Tuple as _Tuple
 
 import pssapi.services.service_base as _service_base
 
 from .. import entities as _entities
 from .. import enums as _enums
 from .. import utils as _utils
 from .raw import UserServiceRaw as _UserServiceRaw
@@ -194,17 +193,22 @@
         return result
 
     async def list_friends(self, user_id: int, access_token: str) -> _entities.ListFriends:
         production_server = await self.get_production_server()
         result = await _UserServiceRaw.list_friends(production_server, user_id, access_token)
         return result
 
-    async def list_skins(self, client_date_time: _datetime.datetime = None, design_version: int = None) -> _Tuple[_entities.SkinSet, _entities.Skin]:
+    async def list_skin_sets(self, client_date_time: _datetime.datetime = None, design_version: int = None) -> _List[_entities.SkinSet]:
         production_server = await self.get_production_server()
-        result = await _UserServiceRaw.list_skins(production_server, _utils.datetime.convert_to_pss_timestamp(client_date_time), design_version, self.language_key)
+        result = await _UserServiceRaw.list_skin_sets_2(production_server, _utils.datetime.convert_to_pss_timestamp(client_date_time), design_version, self.language_key)
+        return result
+
+    async def list_skins(self, client_date_time: _datetime.datetime = None, design_version: int = None) -> _List[_entities.Skin]:
+        production_server = await self.get_production_server()
+        result = await _UserServiceRaw.list_skins_2(production_server, _utils.datetime.convert_to_pss_timestamp(client_date_time), design_version, self.language_key)
         return result
 
     async def remove_friend(self, access_token: str, friend_user_id: int) -> None:
         production_server = await self.get_production_server()
         await _UserServiceRaw.remove_friend(production_server, access_token, friend_user_id)
 
     async def search_users(self, search_string: str) -> _List[_entities.User]:
```

### Comparing `pssapi-0.4.1/src/pssapi/utils/exceptions.py` & `pssapi-0.5.0/src/pssapi/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/src/pssapi/utils/parse.py` & `pssapi-0.5.0/src/pssapi/utils/parse.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.4.1/PKG-INFO` & `pssapi-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssapi
-Version: 0.4.1
+Version: 0.5.0
 Summary: Wrapper for the Pixel Starships API
 Home-page: https://github.com/PSS-Tools-Development/pssapi.py
 License: MIT
 Author: The worst.
 Author-email: theworstpss@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

