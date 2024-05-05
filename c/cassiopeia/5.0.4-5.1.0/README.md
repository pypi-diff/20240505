# Comparing `tmp/cassiopeia-5.0.4.tar.gz` & `tmp/cassiopeia-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassiopeia-5.0.4.tar", last modified: Wed Apr 10 05:29:30 2024, max compression
+gzip compressed data, was "cassiopeia-5.1.0.tar", last modified: Sun May  5 03:44:34 2024, max compression
```

## Comparing `cassiopeia-5.0.4.tar` & `cassiopeia-5.1.0.tar`

### file list

```diff
@@ -1,133 +1,138 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.428426 cassiopeia-5.0.4/
--rw-rw-rw-   0        0        0     1113 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2024-04-10 05:29:30.428426 cassiopeia-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5743 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.288804 cassiopeia-5.0.4/cassiopeia/
--rw-rw-rw-   0        0        0     1853 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.328195 cassiopeia-5.0.4/cassiopeia/_configuration/
--rw-rw-rw-   0        0        0     1260 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/_configuration/__init__.py
--rw-rw-rw-   0        0        0      499 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/_configuration/all_plugins.json
--rw-rw-rw-   0        0        0      679 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/_configuration/load.py
--rw-rw-rw-   0        0        0     7504 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/_configuration/settings.py
--rw-rw-rw-   0        0        0     6546 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/cassiopeia.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.338881 cassiopeia-5.0.4/cassiopeia/core/
--rw-rw-rw-   0        0        0      761 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/__init__.py
--rw-rw-rw-   0        0        0     1819 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/champion.py
--rw-rw-rw-   0        0        0     9734 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/core/championmastery.py
--rw-rw-rw-   0        0        0    13675 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/common.py
--rw-rw-rw-   0        0        0    20748 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/league.py
--rw-rw-rw-   0        0        0    72368 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/core/match.py
--rw-rw-rw-   0        0        0     4865 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/patch.py
--rw-rw-rw-   0        0        0    11987 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/spectator.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.348285 cassiopeia-5.0.4/cassiopeia/core/staticdata/
--rw-rw-rw-   0        0        0      392 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/__init__.py
--rw-rw-rw-   0        0        0    30430 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/champion.py
--rw-rw-rw-   0        0        0     2497 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/common.py
--rw-rw-rw-   0        0        0    17615 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/item.py
--rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/language.py
--rw-rw-rw-   0        0        0     2343 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/languagestrings.py
--rw-rw-rw-   0        0        0     5877 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/map.py
--rw-rw-rw-   0        0        0     6330 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/profileicon.py
--rw-rw-rw-   0        0        0     3040 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/realm.py
--rw-rw-rw-   0        0        0    10615 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/rune.py
--rw-rw-rw-   0        0        0    12152 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/summonerspell.py
--rw-rw-rw-   0        0        0      776 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/staticdata/version.py
--rw-rw-rw-   0        0        0     5634 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/status.py
--rw-rw-rw-   0        0        0     7774 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/summoner.py
--rw-rw-rw-   0        0        0     1412 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/core/thirdpartycode.py
--rw-rw-rw-   0        0        0    28713 2024-04-10 05:25:33.000000 cassiopeia-5.0.4/cassiopeia/data.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.360740 cassiopeia-5.0.4/cassiopeia/datastores/
--rw-rw-rw-   0        0        0      237 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/__init__.py
--rw-rw-rw-   0        0        0    54667 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/cache.py
--rw-rw-rw-   0        0        0     9819 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/common.py
--rw-rw-rw-   0        0        0    32605 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/ddragon.py
--rw-rw-rw-   0        0        0    31226 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/ghost.py
--rw-rw-rw-   0        0        0     2145 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/image.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.366259 cassiopeia-5.0.4/cassiopeia/datastores/kernel/
--rw-rw-rw-   0        0        0     1933 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/champion.py
--rw-rw-rw-   0        0        0     8555 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/championmastery.py
--rw-rw-rw-   0        0        0     4637 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/common.py
--rw-rw-rw-   0        0        0    11466 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/leagues.py
--rw-rw-rw-   0        0        0    12070 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/match.py
--rw-rw-rw-   0        0        0     3204 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/spectator.py
--rw-rw-rw-   0        0        0     3038 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/status.py
--rw-rw-rw-   0        0        0     2407 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/summoner.py
--rw-rw-rw-   0        0        0     3474 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/kernel/thirdpartycode.py
--rw-rw-rw-   0        0        0     4033 2024-04-10 05:26:46.000000 cassiopeia-5.0.4/cassiopeia/datastores/lolwikia.py
--rw-rw-rw-   0        0        0     2897 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/merakianalyticscdn.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.380881 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/
--rw-rw-rw-   0        0        0     3586 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/__init__.py
--rw-rw-rw-   0        0        0     2643 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/champion.py
--rw-rw-rw-   0        0        0    10255 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/championmastery.py
--rw-rw-rw-   0        0        0    17773 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/common.py
--rw-rw-rw-   0        0        0    15725 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/leagues.py
--rw-rw-rw-   0        0        0     8276 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/match.py
--rw-rw-rw-   0        0        0     3667 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/spectator.py
--rw-rw-rw-   0        0        0     3530 2024-04-10 05:17:47.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/status.py
--rw-rw-rw-   0        0        0     3100 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/summoner.py
--rw-rw-rw-   0        0        0     3871 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/riotapi/thirdpartycode.py
--rw-rw-rw-   0        0        0    89187 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/datastores/uniquekeys.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.393570 cassiopeia-5.0.4/cassiopeia/dto/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/__init__.py
--rw-rw-rw-   0        0        0       84 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/champion.py
--rw-rw-rw-   0        0        0      196 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/championmastery.py
--rw-rw-rw-   0        0        0      407 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/common.py
--rw-rw-rw-   0        0        0      445 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/league.py
--rw-rw-rw-   0        0        0      215 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/match.py
--rw-rw-rw-   0        0        0       77 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/patch.py
--rw-rw-rw-   0        0        0      133 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/spectator.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.403695 cassiopeia-5.0.4/cassiopeia/dto/staticdata/
--rw-rw-rw-   0        0        0      516 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/__init__.py
--rw-rw-rw-   0        0        0      334 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/champion.py
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/common.py
--rw-rw-rw-   0        0        0      118 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/item.py
--rw-rw-rw-   0        0        0      130 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/language.py
--rw-rw-rw-   0        0        0      116 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/map.py
--rw-rw-rw-   0        0        0      139 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/profileicon.py
--rw-rw-rw-   0        0        0       74 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/realm.py
--rw-rw-rw-   0        0        0      209 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/rune.py
--rw-rw-rw-   0        0        0      136 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/summonerspell.py
--rw-rw-rw-   0        0        0       80 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/staticdata/version.py
--rw-rw-rw-   0        0        0       79 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/status.py
--rw-rw-rw-   0        0        0       76 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/summoner.py
--rw-rw-rw-   0        0        0       86 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/dto/thirdpartycode.py
--rw-rw-rw-   0        0        0    26420 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/profile_icon_names.json
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.403695 cassiopeia-5.0.4/cassiopeia/resources/
--rw-rw-rw-   0        0        0    15654 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/resources/summonersRiftAreas.png
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.413613 cassiopeia-5.0.4/cassiopeia/transformers/
--rw-rw-rw-   0        0        0      871 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/champion.py
--rw-rw-rw-   0        0        0     2203 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/championmastery.py
--rw-rw-rw-   0        0        0     5348 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/leagues.py
--rw-rw-rw-   0        0        0     2974 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/match.py
--rw-rw-rw-   0        0        0     2649 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/spectator.py
--rw-rw-rw-   0        0        0    15350 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/staticdata.py
--rw-rw-rw-   0        0        0      947 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/status.py
--rw-rw-rw-   0        0        0      933 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/summoner.py
--rw-rw-rw-   0        0        0     1076 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/cassiopeia/transformers/thirdpartycode.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.323072 cassiopeia-5.0.4/cassiopeia.egg-info/
--rw-rw-rw-   0        0        0      858 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3858 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 05:29:30.000000 cassiopeia-5.0.4/cassiopeia.egg-info/zip-safe
--rw-rw-rw-   0        0        0      123 2024-04-10 05:29:30.430435 cassiopeia-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1537 2024-04-10 05:28:02.000000 cassiopeia-5.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:29:30.423147 cassiopeia-5.0.4/test/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/__init__.py
--rw-rw-rw-   0        0        0      532 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/constants.py
--rw-rw-rw-   0        0        0     1369 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_champion.py
--rw-rw-rw-   0        0        0     2201 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_championmastery.py
--rw-rw-rw-   0        0        0      278 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_championrotation.py
--rw-rw-rw-   0        0        0     9347 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_examples.py
--rw-rw-rw-   0        0        0      689 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_items.py
--rw-rw-rw-   0        0        0     2473 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_league.py
--rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_map_location.py
--rw-rw-rw-   0        0        0     1413 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_match.py
--rw-rw-rw-   0        0        0     2329 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_matchhistory.py
--rw-rw-rw-   0        0        0      708 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_patches.py
--rw-rw-rw-   0        0        0      879 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_status.py
--rw-rw-rw-   0        0        0     2023 2023-02-12 18:12:02.000000 cassiopeia-5.0.4/test/test_summoner.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.100221 cassiopeia-5.1.0/
+-rw-rw-rw-   0        0        0     1113 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2024-05-05 03:44:34.100221 cassiopeia-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5799 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:33.954505 cassiopeia-5.1.0/cassiopeia/
+-rw-rw-rw-   0        0        0     1885 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:33.993506 cassiopeia-5.1.0/cassiopeia/_configuration/
+-rw-rw-rw-   0        0        0     1260 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/_configuration/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/_configuration/all_plugins.json
+-rw-rw-rw-   0        0        0      679 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/_configuration/load.py
+-rw-rw-rw-   0        0        0     7929 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/_configuration/settings.py
+-rw-rw-rw-   0        0        0     6743 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/cassiopeia.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.011217 cassiopeia-5.1.0/cassiopeia/core/
+-rw-rw-rw-   0        0        0      791 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/__init__.py
+-rw-rw-rw-   0        0        0     5157 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/account.py
+-rw-rw-rw-   0        0        0     1819 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/champion.py
+-rw-rw-rw-   0        0        0     9656 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/championmastery.py
+-rw-rw-rw-   0        0        0    13675 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/common.py
+-rw-rw-rw-   0        0        0    20498 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/league.py
+-rw-rw-rw-   0        0        0    73137 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/match.py
+-rw-rw-rw-   0        0        0     5384 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/patch.py
+-rw-rw-rw-   0        0        0    11816 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/spectator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.014586 cassiopeia-5.1.0/cassiopeia/core/staticdata/
+-rw-rw-rw-   0        0        0      392 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/__init__.py
+-rw-rw-rw-   0        0        0    30430 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/champion.py
+-rw-rw-rw-   0        0        0     2497 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/common.py
+-rw-rw-rw-   0        0        0    17615 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/item.py
+-rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/language.py
+-rw-rw-rw-   0        0        0     2343 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/languagestrings.py
+-rw-rw-rw-   0        0        0     5877 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/map.py
+-rw-rw-rw-   0        0        0     6330 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/profileicon.py
+-rw-rw-rw-   0        0        0     3040 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/realm.py
+-rw-rw-rw-   0        0        0    10691 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/rune.py
+-rw-rw-rw-   0        0        0    12152 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/summonerspell.py
+-rw-rw-rw-   0        0        0      776 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/staticdata/version.py
+-rw-rw-rw-   0        0        0     5634 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/core/status.py
+-rw-rw-rw-   0        0        0     6902 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/summoner.py
+-rw-rw-rw-   0        0        0     1473 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/core/thirdpartycode.py
+-rw-rw-rw-   0        0        0    28741 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/data.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.027022 cassiopeia-5.1.0/cassiopeia/datastores/
+-rw-rw-rw-   0        0        0      237 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/__init__.py
+-rw-rw-rw-   0        0        0    56546 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/cache.py
+-rw-rw-rw-   0        0        0     9819 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/common.py
+-rw-rw-rw-   0        0        0    31133 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/ddragon.py
+-rw-rw-rw-   0        0        0    31813 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/ghost.py
+-rw-rw-rw-   0        0        0     2145 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/image.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.048358 cassiopeia-5.1.0/cassiopeia/datastores/kernel/
+-rw-rw-rw-   0        0        0     2045 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/__init__.py
+-rw-rw-rw-   0        0        0     2057 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/account.py
+-rw-rw-rw-   0        0        0     2400 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/champion.py
+-rw-rw-rw-   0        0        0     8555 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/championmastery.py
+-rw-rw-rw-   0        0        0     4637 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/common.py
+-rw-rw-rw-   0        0        0    11466 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/leagues.py
+-rw-rw-rw-   0        0        0    12070 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/match.py
+-rw-rw-rw-   0        0        0     3204 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/spectator.py
+-rw-rw-rw-   0        0        0     3038 2024-04-10 05:17:47.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/status.py
+-rw-rw-rw-   0        0        0     2189 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/summoner.py
+-rw-rw-rw-   0        0        0     3474 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/kernel/thirdpartycode.py
+-rw-rw-rw-   0        0        0     4033 2024-04-10 05:26:46.000000 cassiopeia-5.1.0/cassiopeia/datastores/lolwikia.py
+-rw-rw-rw-   0        0        0     2897 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/merakianalyticscdn.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.059425 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/
+-rw-rw-rw-   0        0        0     3819 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/__init__.py
+-rw-rw-rw-   0        0        0     2697 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/account.py
+-rw-rw-rw-   0        0        0     2643 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/champion.py
+-rw-rw-rw-   0        0        0    10255 2024-04-10 05:17:47.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/championmastery.py
+-rw-rw-rw-   0        0        0    17773 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/common.py
+-rw-rw-rw-   0        0        0    15725 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/leagues.py
+-rw-rw-rw-   0        0        0     8276 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/match.py
+-rw-rw-rw-   0        0        0     3668 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/spectator.py
+-rw-rw-rw-   0        0        0     3530 2024-04-10 05:17:47.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/status.py
+-rw-rw-rw-   0        0        0     2742 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/summoner.py
+-rw-rw-rw-   0        0        0     3871 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/datastores/riotapi/thirdpartycode.py
+-rw-rw-rw-   0        0        0    91621 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/datastores/uniquekeys.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.067722 cassiopeia-5.1.0/cassiopeia/dto/
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/dto/account.py
+-rw-rw-rw-   0        0        0       84 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/champion.py
+-rw-rw-rw-   0        0        0      196 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/championmastery.py
+-rw-rw-rw-   0        0        0      407 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/common.py
+-rw-rw-rw-   0        0        0      445 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/league.py
+-rw-rw-rw-   0        0        0      215 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/match.py
+-rw-rw-rw-   0        0        0       77 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/patch.py
+-rw-rw-rw-   0        0        0      133 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/spectator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.075733 cassiopeia-5.1.0/cassiopeia/dto/staticdata/
+-rw-rw-rw-   0        0        0      516 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/__init__.py
+-rw-rw-rw-   0        0        0      334 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/champion.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/common.py
+-rw-rw-rw-   0        0        0      118 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/item.py
+-rw-rw-rw-   0        0        0      130 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/language.py
+-rw-rw-rw-   0        0        0      116 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/map.py
+-rw-rw-rw-   0        0        0      139 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/profileicon.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/realm.py
+-rw-rw-rw-   0        0        0      209 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/rune.py
+-rw-rw-rw-   0        0        0      136 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/summonerspell.py
+-rw-rw-rw-   0        0        0       80 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/staticdata/version.py
+-rw-rw-rw-   0        0        0       79 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/status.py
+-rw-rw-rw-   0        0        0       76 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/summoner.py
+-rw-rw-rw-   0        0        0       86 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/dto/thirdpartycode.py
+-rw-rw-rw-   0        0        0    26420 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/profile_icon_names.json
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.081212 cassiopeia-5.1.0/cassiopeia/resources/
+-rw-rw-rw-   0        0        0    15654 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/resources/summonersRiftAreas.png
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.091784 cassiopeia-5.1.0/cassiopeia/transformers/
+-rw-rw-rw-   0        0        0      943 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/transformers/__init__.py
+-rw-rw-rw-   0        0        0      888 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/transformers/account.py
+-rw-rw-rw-   0        0        0     1091 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/champion.py
+-rw-rw-rw-   0        0        0     2203 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/championmastery.py
+-rw-rw-rw-   0        0        0     5348 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/leagues.py
+-rw-rw-rw-   0        0        0     2974 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/match.py
+-rw-rw-rw-   0        0        0     2732 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/transformers/spectator.py
+-rw-rw-rw-   0        0        0    15350 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/staticdata.py
+-rw-rw-rw-   0        0        0      947 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/status.py
+-rw-rw-rw-   0        0        0      906 2024-05-05 03:37:59.000000 cassiopeia-5.1.0/cassiopeia/transformers/summoner.py
+-rw-rw-rw-   0        0        0     1076 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/cassiopeia/transformers/thirdpartycode.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:33.985464 cassiopeia-5.1.0/cassiopeia.egg-info/
+-rw-rw-rw-   0        0        0      858 2024-05-05 03:44:33.000000 cassiopeia-5.1.0/cassiopeia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4027 2024-05-05 03:44:33.000000 cassiopeia-5.1.0/cassiopeia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 03:44:33.000000 cassiopeia-5.1.0/cassiopeia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-05 03:44:33.000000 cassiopeia-5.1.0/cassiopeia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 03:44:33.000000 cassiopeia-5.1.0/cassiopeia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 05:29:30.000000 cassiopeia-5.1.0/cassiopeia.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      123 2024-05-05 03:44:34.100221 cassiopeia-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1537 2024-05-05 03:42:41.000000 cassiopeia-5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:44:34.100221 cassiopeia-5.1.0/test/
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/constants.py
+-rw-rw-rw-   0        0        0     1369 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_champion.py
+-rw-rw-rw-   0        0        0     2201 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_championmastery.py
+-rw-rw-rw-   0        0        0      278 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_championrotation.py
+-rw-rw-rw-   0        0        0     9347 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_examples.py
+-rw-rw-rw-   0        0        0      689 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_items.py
+-rw-rw-rw-   0        0        0     2473 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_league.py
+-rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_map_location.py
+-rw-rw-rw-   0        0        0     1413 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_match.py
+-rw-rw-rw-   0        0        0     2329 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_matchhistory.py
+-rw-rw-rw-   0        0        0      708 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_patches.py
+-rw-rw-rw-   0        0        0      879 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_status.py
+-rw-rw-rw-   0        0        0     2023 2023-02-12 18:12:02.000000 cassiopeia-5.1.0/test/test_summoner.py
```

### Comparing `cassiopeia-5.0.4/LICENSE.txt` & `cassiopeia-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/PKG-INFO` & `cassiopeia-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassiopeia
-Version: 5.0.4
+Version: 5.1.0
 Summary: Riot Games Developer API Wrapper (3rd Party)
 Home-page: https://github.com/meraki-analytics/cassiopeia
 Author: Jason Maldonis; Rob Rua
 Author-email: team@merakianalytics.com
 License: MIT
 Keywords: LoL,League of Legends,Riot Games,API,REST
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cassiopeia-5.0.4/README.md` & `cassiopeia-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,17 @@
 ```python
 import random
 
 import cassiopeia as cass
 
 cass.set_riot_api_key("YOUR_KEY")  # This overrides the value set in your configuration/settings.
 
-summoner = cass.get_summoner(name="Perkz", region="NA")
-print("{name} is a level {level} summoner on the {region} server.".format(name=summoner.name,
+account = cass.get_account(name="Perkz", tagline="Style", region="NA")
+summoner = account.summoner
+print("{name} is a level {level} summoner on the {region} server.".format(name=account.name_with_tagline,
                                                                           level=summoner.level,
                                                                           region=summoner.region))
 
 champions = cass.get_champions(region="NA")
 random_champion = random.choice(champions)
 print("He enjoys playing champions such as {name}.".format(name=random_champion.name))
```

### Comparing `cassiopeia-5.0.4/cassiopeia/__init__.py` & `cassiopeia-5.1.0/cassiopeia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     get_match,
     get_match_history,
     get_profile_icons,
     get_runes,
     get_status,
     get_summoner,
     get_summoner_spells,
+    get_account,
     get_version,
     get_versions,
     get_champion_rotations,
     get_paginated_league_entries,
     get_verification_string,
 )
 from .cassiopeia import apply_settings, set_riot_api_key, print_calls, _get_pipeline
@@ -47,14 +48,15 @@
     SummonerSpell,
     SummonerSpells,
     ProfileIcon,
     ProfileIcons,
     Versions,
     Maps,
     Summoner,
+    Account,
     ChampionMastery,
     ChampionMasteries,
     Match,
     FeaturedMatches,
     ShardStatus,
     ChallengerLeague,
     GrandmasterLeague,
```

### Comparing `cassiopeia-5.0.4/cassiopeia/_configuration/__init__.py` & `cassiopeia-5.1.0/cassiopeia/_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/_configuration/load.py` & `cassiopeia-5.1.0/cassiopeia/_configuration/load.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/_configuration/settings.py` & `cassiopeia-5.1.0/cassiopeia/_configuration/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TypeVar, Type, Dict, Union, List
 import logging
 import importlib
 import inspect
 import copy
+import os
 
 from datapipelines import (
     DataPipeline,
     DataSink,
     DataSource,
     CompositeDataTransformer,
     DataTransformer,
@@ -122,15 +123,15 @@
 def get_default_config():
     return {
         "global": {"version_from_match": "patch"},
         "plugins": {},
         "pipeline": {
             "Cache": {},
             "DDragon": {},
-            "RiotAPI": {"api_key": "RIOT_API_KEY"},
+            "RiotAPI": {"api_key": "$RIOT_API_KEY"},
         },
         "logging": {
             "print_calls": True,
             "print_riot_api_key": False,
             "default": "WARNING",
             "core": "WARNING",
         },
@@ -159,14 +160,24 @@
         )
         for name in ["default", "core"]:
             logger = logging.getLogger(name)
             level = logging_config.get(name, _defaults["logging"][name])
             logger.setLevel(level)
             for handler in logger.handlers:
                 handler.setLevel(level)
+        if (
+            _defaults.get("pipeline", {})
+            .get("RiotAPI", {})
+            .get("api_key", "")
+            .startswith("$")
+        ):
+            riot_api_key_env_var_name = _defaults["pipeline"]["RiotAPI"]["api_key"][1:]
+            riot_api_key = os.environ.get(riot_api_key_env_var_name, None)
+            if riot_api_key:
+                self.set_riot_api_key(riot_api_key)
 
     @property
     def pipeline(self) -> DataPipeline:
         if self.__pipeline is None:
             self.__pipeline = create_pipeline(
                 service_configs=self.__pipeline_args, verbose=0
             )
```

### Comparing `cassiopeia-5.0.4/cassiopeia/cassiopeia.py` & `cassiopeia-5.1.0/cassiopeia/cassiopeia.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import arrow
 import datetime
 
 from .data import Region, Queue, Tier, Division, Continent, Platform, MatchType
 from .core import (
     Champion,
     Summoner,
+    Account,
     ChampionMastery,
     Rune,
     Item,
     Match,
     Map,
     SummonerSpell,
     Realms,
@@ -164,18 +165,27 @@
     return ChampionMastery(champion=champion, summoner=summoner, region=region)
 
 
 def get_summoner(
     *,
     id: str = None,
     account_id: str = None,
-    name: str = None,
-    region: Union[Region, str] = None
+    puuid: str = None,
+    region: Union[Region, str] = None,
 ) -> Summoner:
-    return Summoner(id=id, account_id=account_id, name=name, region=region)
+    return Summoner(id=id, account_id=account_id, puuid=puuid, region=region)
+
+
+def get_account(
+    *,
+    puuid: str = None,
+    name: str = None,
+    tagline: str = None,
+) -> Account:
+    return Account(puuid=puuid, name=name, tagline=tagline)
 
 
 def get_champion(key: Union[str, int], region: Union[Region, str] = None) -> Champion:
     return get_champions(region=region)[key]
 
 
 def get_champions(region: Union[Region, str] = None) -> Champions:
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/__init__.py` & `cassiopeia-5.1.0/cassiopeia/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Runes,
     SummonerSpells,
     Maps,
     Items,
 )
 from .champion import ChampionRotation
 from .summoner import Summoner
+from .account import Account
 from .championmastery import ChampionMastery, ChampionMasteries
 from .match import Match, MatchHistory
 from .spectator import CurrentMatch, FeaturedMatches
 from .status import ShardStatus
 from .league import (
     League,
     ChallengerLeague,
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/champion.py` & `cassiopeia-5.1.0/cassiopeia/core/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/championmastery.py` & `cassiopeia-5.1.0/cassiopeia/core/championmastery.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,34 +102,32 @@
 )
 class ChampionMastery(CassiopeiaGhost):
     _data_types = {ChampionMasteryData}
 
     def __init__(
         self,
         *,
-        summoner: Union[Summoner, int, str] = None,
+        summoner: Union[Summoner, str] = None,
         champion: Union[Champion, int, str] = None,
         region: Union[Region, str] = None,
         _account_id: str = None
     ):
         kwargs = {"region": region}
 
-        if _account_id is not None:
+        if not isinstance(summoner, Summoner) and _account_id is not None:
             summoner = Summoner(account_id=_account_id, region=region)
-
-        if summoner is not None:
+        elif summoner is not None:
             if isinstance(summoner, Summoner):
                 self.__class__.summoner.fget._lazy_set(self, summoner)
             elif isinstance(summoner, str):
-                if len(summoner) < 35:
-                    # It's a summoner name
-                    summoner = Summoner(name=summoner, region=region)
+                if 70 < len(summoner) < 85:
+                    # puuids should always have 78 characters, but I don't know that for sure. The range 70-85 is likely good.
+                    summoner = Summoner(puuid=summoner, region=region)
                     self.__class__.summoner.fget._lazy_set(self, summoner)
-                else:
-                    # It's probably a summoner id
+                else:  # Assume the summoner is a summonerId
                     kwargs["summonerId"] = summoner
 
         if champion is not None:
             if isinstance(champion, Champion):
                 self.__class__.champion.fget._lazy_set(self, champion)
             elif isinstance(champion, str):
                 champion = Champion(
@@ -143,28 +141,24 @@
 
         super().__init__(**kwargs)
 
     @classmethod
     def __get_query_from_kwargs__(
         cls,
         *,
-        summoner: Union[Summoner, int, str],
+        summoner: Union[Summoner, str],
         champion: Union[Champion, int, str],
         region: Union[Region, str]
     ) -> dict:
         query = {"region": region}
         if isinstance(summoner, Summoner):
             query["summoner.id"] = summoner.id
         elif isinstance(summoner, str):
-            if len(summoner) < 35:
-                # It's a summoner name
-                query["summoner.id"] = Summoner(name=summoner, region=region).id
-            else:
-                # It's probably a summoner id
-                query["summoner.id"] = summoner
+            # It's probably a summoner id
+            query["summoner.id"] = summoner
 
         if isinstance(champion, Champion):
             query["champion.id"] = champion.id
         elif isinstance(champion, str):
             query["champion.id"] = Champion(name=champion, region=region).id
         else:  # int
             query["champion.id"] = champion
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/common.py` & `cassiopeia-5.1.0/cassiopeia/core/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/league.py` & `cassiopeia-5.1.0/cassiopeia/core/league.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,15 +265,14 @@
     def losses(self) -> int:
         return self._data[LeagueEntryData].losses
 
     @lazy_property
     def summoner(self) -> Summoner:
         return Summoner(
             id=self._data[LeagueEntryData].summonerId,
-            name=self._data[LeagueEntryData].summonerName,
             region=self.region,
         )
 
     @property
     def fresh_blood(self) -> bool:
         return self._data[LeagueEntryData].freshBlood
 
@@ -371,20 +370,15 @@
 
     @classmethod
     def __get_query_from_kwargs__(cls, *, summoner: Union[Summoner, str]) -> dict:
         query = {"region": summoner.region}
         if isinstance(summoner, Summoner):
             query["summoner.id"] = summoner.id
         elif isinstance(summoner, str):
-            if len(summoner) < 35:
-                query["summoner.id"] = Summoner(
-                    name=summoner, region=summoner.region
-                ).id
-            else:
-                query["summoner.id"] = summoner
+            query["summoner.id"] = summoner
         assert "summoner.id" in query
         return query
 
     @lazy_property
     def region(self) -> Region:
         return Region(self._data[LeagueSummonerEntriesData].region)
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/match.py` & `cassiopeia-5.1.0/cassiopeia/core/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             elif isinstance(self, ParticipantStats):
                 old_participant = getattr(
                     self, "_{}__participant".format(self.__class__.__name__)
                 )
             else:
                 raise RuntimeError("Impossible!")
             for participant in match.participants:
-                if participant.summoner.name == old_participant.summoner.name:
+                if participant.summoner_name == old_participant.summoner_name:
                     if isinstance(self, Participant):
                         self._data[ParticipantData] = participant._data[ParticipantData]
                     elif isinstance(self, ParticipantStats):
                         self._data[ParticipantStatsData] = participant.stats._data[
                             ParticipantStatsData
                         ]
                     return method(self, *args, **kwargs)
@@ -425,14 +425,27 @@
             participant = ParticipantData(
                 **participant, platformId=kwargs["platformId"]
             )
             self.participants.append(participant)
 
         teams = kwargs.pop("teams", [])
         self.teams = []
+
+        # There's a weird thing where teamIds can be set to 0. Try to fix it.
+        team_ids = set([team["teamId"] for team in teams])
+        if not (len(team_ids) == 2 and 100 in team_ids and 200 in team_ids):
+            if 100 in team_ids:
+                for team in teams:
+                    if team["teamId"] != 100:
+                        team["teamId"] = 200
+            if 200 in team_ids:
+                for team in teams:
+                    if team["teamId"] != 200:
+                        team["teamId"] = 100
+
         for team in teams:
             team_side = Side(team["teamId"])
             participants = []
             for participant in self.participants:
                 if participant.side is team_side:
                     participants.append(participant)
             self.teams.append(TeamData(**team, participants=participants))
@@ -839,15 +852,17 @@
 
     @property
     def frames(self) -> List[ParticipantFrame]:
         timeline: Timeline = self.__match.timeline
         these = []
         for frame in timeline.frames:
             for pid, pframe in frame.participant_frames.items():
-                pframe.timestamp = frame.timestamp  # Assign the match's Frame timestamp to the ParticipantFrame
+                pframe.timestamp = (
+                    frame.timestamp
+                )  # Assign the match's Frame timestamp to the ParticipantFrame
                 if pframe.participant_id == self.id:
                     these.append(pframe)
         return these
 
     @property
     def events(self):
         my_events = []
@@ -1041,17 +1056,15 @@
         latest_frame_ts = self._latest_frame.timestamp
         # Now loop through all events and use the latest event's position if the event was generated later than the frame.
         events = [
             (getattr(event, "timestamp", None), getattr(event, "position", None))
             for event in self._processed_events
         ]
         events_with_ts_and_position = [
-            (ts, p)
-            for ts, p in events
-            if ts is not None and p is not None
+            (ts, p) for ts, p in events if ts is not None and p is not None
         ]
         # If an event exists with both a timestamp and position, and the event was generated later that the frame, return its position.
         if len(events_with_ts_and_position) > 0:
             latest_event_ts, latest_event_position = events_with_ts_and_position[-1]
             if latest_event_ts > latest_frame_ts:
                 return latest_event_position
         # If we got this far, then the latest event (if it exists) is not relevant. Return the position from the latest frame.
@@ -1136,14 +1149,22 @@
                 2057,
                 2424,
                 2059,
                 2060,
                 2013,
                 2421,
                 3600,
+                2145,
+                220000,
+                220001,
+                220002,
+                220003,
+                220004,
+                220005,
+                220006,
             ):  # Something weird can happen with trinkets and klepto items
                 pass
             else:
                 raise error
         self._items.reverse()
 
     def undo(self, event: Event):
@@ -1630,15 +1651,17 @@
 
     @property
     def team_position(self) -> Lane:
         return Lane.from_match_naming_scheme(self._data[ParticipantData].teamPosition)
 
     @property
     def lane(self) -> Lane:
-        return Lane.from_match_naming_scheme(self._data[ParticipantData].individualPosition)
+        return Lane.from_match_naming_scheme(
+            self._data[ParticipantData].individualPosition
+        )
 
     @property
     def role(self) -> Role:
         return Role.from_match_naming_scheme(self._data[ParticipantData].stats.role)
 
     @property
     def skill_order(self) -> List[Key]:
@@ -1766,28 +1789,28 @@
         if self.__match._data[MatchData].privateGame:
             return None
         kwargs = {}
         try:
             kwargs["id"] = self._data[ParticipantData].summonerId
         except AttributeError:
             pass
-        try:
-            kwargs["name"] = self._data[ParticipantData].summonerName
-        except AttributeError:
-            pass
         kwargs["puuid"] = self._data[ParticipantData].puuid
         kwargs["region"] = Platform(self._data[ParticipantData].platformId).region
         summoner = Summoner(**kwargs)
         try:
             summoner(profileIconId=self._data[ParticipantData].profileIconId)
         except AttributeError:
             pass
         return summoner
 
     @property
+    def summoner_name(self) -> str:
+        return self._data[ParticipantData].summonerName
+
+    @property
     def team(self) -> "Team":
         if self.side == Side.blue:
             return self.__match.blue_team
         else:
             return self.__match.red_team
 
     @property
@@ -1840,17 +1863,19 @@
     def first_blood(self) -> bool:
         return self._data[TeamData].objectives["champion"].first
 
     @property
     def bans(self) -> List["Champion"]:
         version = _choose_staticdata_version(self.__match)
         return [
-            Champion(id=ban.championId, version=version, region=self.__match.region)
-            if ban.championId != -1
-            else None
+            (
+                Champion(id=ban.championId, version=version, region=self.__match.region)
+                if ban.championId != -1
+                else None
+            )
             for ban in self._data[TeamData].bans
         ]
 
     @property
     def rift_herald_kills(self) -> int:
         return self._data[TeamData].objectives["riftHerald"].kills
 
@@ -2012,17 +2037,15 @@
 
     @CassiopeiaGhost.property(MatchData)
     @ghost_load_on
     @lazy
     def teams(self) -> List[Team]:
         if not self._Ghost__is_loaded(MatchData):
             self.__load__(MatchData)
-            self._Ghost__set_loaded(
-                MatchData
-            )  # __load__ doesn't trigger __set_loaded.
+            self._Ghost__set_loaded(MatchData)  # __load__ doesn't trigger __set_loaded.
         return [
             Team.from_data(t, match=self)
             for i, t in enumerate(self._data[MatchData].teams)
         ]
 
     @property
     def red_team(self) -> Team:
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/patch.py` & `cassiopeia-5.1.0/cassiopeia/core/patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,31 +84,41 @@
     def __load__(cls):
         data = configuration.settings.pipeline.get(PatchListDto, query={})
         patches = data["patches"]
         shifts = data["shifts"]
         cls.__patches = defaultdict(lambda: [None for _ in range(len(patches))])
         for i, (patch, next_patch) in enumerate(pairwise(patches)):
             for region in Region:
-                start = arrow.get(patch["start"] + shifts[region.platform.value]).to(
+                if region.platform.value in shifts:
+                    region_key = region.platform.value
+                elif region.value in shifts:
+                    region_key = region.value
+                else:
+                    raise ValueError(f"Known region in patch data: {region}")
+                start = arrow.get(patch["start"] + shifts[region_key]).to(
                     region.timezone
                 )
                 name = patch["name"]
-                end = arrow.get(next_patch["start"] + shifts[region.platform.value]).to(
+                end = arrow.get(next_patch["start"] + shifts[region_key]).to(
                     region.timezone
                 )
                 cls.__patches[region][i] = Patch(
                     region=region, name=name, start=start, end=end
                 )
 
         # Since pairwise skips the last patch in the list, add it manually here
         patch = patches[-1]
         for region in Region:
-            start = arrow.get(patch["start"] + shifts[region.platform.value]).to(
-                region.timezone
-            )
+            if region.platform.value in shifts:
+                region_key = region.platform.value
+            elif region.value in shifts:
+                region_key = region.value
+            else:
+                raise ValueError(f"Known region in patch data: {region}")
+            start = arrow.get(patch["start"] + shifts[region_key]).to(region.timezone)
             name = patch["name"]
             end = None
             cls.__patches[region][-1] = Patch(
                 region=region, name=name, start=start, end=end
             )
 
         # Sort each region's patches by start date
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/spectator.py` & `cassiopeia-5.1.0/cassiopeia/core/spectator.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,16 @@
     def summoner(self) -> Summoner:
         ProfileIcon(
             id=self._data[CurrentGameParticipantData].profileIconId,
             region=self.__match.region,
         )
         if hasattr(self._data[CurrentGameParticipantData], "summonerId"):
             return Summoner(
+                puuid=self._data[CurrentGameParticipantData].puuid,
                 id=self._data[CurrentGameParticipantData].summonerId,
-                name=self._data[CurrentGameParticipantData].summonerName,
                 region=self.__match.region,
             )
         else:
             return Summoner(
                 name=self._data[CurrentGameParticipantData].summonerName,
                 region=self.__match.region,
             )
@@ -249,52 +249,47 @@
         summoner: Union[Summoner, str] = None,
         region: Union[Region, str] = None
     ):
         kwargs = {"region": region}
 
         if summoner is not None:
             if isinstance(summoner, str):
-                if len(summoner) < 35:
-                    summoner = Summoner(name=summoner, region=region)
-                else:
-                    summoner = Summoner(id=summoner, region=region)
+                summoner = Summoner(id=summoner, region=region)
             self.__summoner = summoner
         super().__init__(**kwargs)
 
     @classmethod
     def from_data(cls, data: CurrentGameInfoData, summoner: Union[Summoner, str]):
         self = super().from_data(data)
+        # TODO: There's no region here! This is an old bug, ignoring for now.
         if isinstance(summoner, str):
-            if len(summoner) < 35:
-                summoner = Summoner(name=summoner, region=region)
-            else:
-                summoner = Summoner(id=summoner, region=region)
-                self.__summoner = summoner
+            summoner = Summoner(id=summoner, region=region)
+            self.__summoner = summoner
         return self
 
     @classmethod
     def __get_query_from_kwargs__(
         cls, *, summoner: Union[Summoner, str], region: Union[Region, str]
     ) -> dict:
         query = {"region": region}
         if isinstance(summoner, Summoner):
-            query["summoner.id"] = summoner.id
+            query["summoner.puuid"] = summoner.puuid
         elif isinstance(summoner, str):
-            if len(summoner) < 35:
-                query["summoner.id"] = Summoner(name=summoner, region=region).id
+            if 70 < len(summoner) < 85:
+                query["summoner.puuid"] = summoner
             else:
-                query["summoner.id"] = summoner
+                query["summoner.puuid"] = Summoner(id=summoner, region=region).puuid
         assert "summoner.id" in query
         return query
 
     def __get_query__(self):
         return {
             "region": self.region,
             "platform": self.platform,
-            "summoner.id": self.__summoner.id,
+            "summoner.puuid": self.__summoner.puuid,
         }
 
     @property
     def exists(self):
         try:
             if not self._Ghost__all_loaded:
                 self.__load__()
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/champion.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/common.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/item.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/item.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/language.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/language.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/languagestrings.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/languagestrings.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/map.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/map.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/profileicon.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/profileicon.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/realm.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/realm.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/rune.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/rune.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,14 +319,18 @@
         excluded_ids = {
             5001,
             5002,
             5003,
             5005,
             5007,
             5008,
+            5010,
+            5011,
+            5012,
+            5013,
         }  # These are the ids of the stat shard runes which have a tier of 0 but are not keystones
         # alternatively, we could add tier values to the hardcoded stat runes in datastores/ddragon.py
         return self.tier == 0 and self.id not in excluded_ids
 
     @CassiopeiaGhost.property(RuneData)
     @ghost_load_on
     def name(self) -> str:
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/summonerspell.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/summonerspell.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/staticdata/version.py` & `cassiopeia-5.1.0/cassiopeia/core/staticdata/version.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/status.py` & `cassiopeia-5.1.0/cassiopeia/core/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/core/summoner.py` & `cassiopeia-5.1.0/cassiopeia/core/summoner.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime
 from typing import Union
 
 from datapipelines import NotFoundError
 from merakicommons.cache import lazy_property
 from merakicommons.container import searchable
 
-from ..data import Region, Platform, Rank
-from .common import CoreData, CassiopeiaObject, CassiopeiaGhost, ghost_load_on
+from ..data import Region, Platform, Continent, Rank
+from .common import CoreData, CassiopeiaGhost, ghost_load_on
 from .staticdata import ProfileIcon
 from ..dto.summoner import SummonerDto
 
 
 ##############
 # Data Types #
 ##############
@@ -25,62 +25,56 @@
 ##############
 # Core Types #
 ##############
 
 
 @searchable(
     {
-        str: ["name", "region", "platform", "id", "account_id", "puuid"],
+        str: ["region", "platform", "id", "account_id", "puuid"],
         Region: ["region"],
         Platform: ["platform"],
     }
 )
 class Summoner(CassiopeiaGhost):
     _data_types = {SummonerData}
 
     def __init__(
         self,
         *,
         id: str = None,
         account_id: str = None,
         puuid: str = None,
-        name: str = None,
-        region: Union[Region, str] = None
+        region: Union[Region, str] = None,
     ):
         kwargs = {"region": region}
 
         if id is not None:
             kwargs["id"] = id
         if account_id is not None:
             kwargs["accountId"] = account_id
         if puuid is not None:
             kwargs["puuid"] = puuid
-        if name is not None:
-            kwargs["name"] = name
         super().__init__(**kwargs)
 
     @classmethod
     def __get_query_from_kwargs__(
         cls,
         *,
         id: str = None,
         account_id: str = None,
         puuid: str = None,
-        name: str = None,
-        region: Union[Region, str]
+        region: Union[Region, str],
     ) -> dict:
         query = {"region": region}
         if id is not None:
             query["id"] = id
         if account_id is not None:
             query["accountId"] = account_id
         if puuid is not None:
             query["puuid"] = puuid
-        if name is not None:
-            query["name"] = name
         return query
 
     def __get_query__(self):
         query = {"region": self.region, "platform": self.platform}
         try:
             query["puuid"] = self._data[SummonerData].puuid
         except AttributeError:
@@ -89,63 +83,48 @@
             query["id"] = self._data[SummonerData].id
         except AttributeError:
             pass
         try:
             query["accountId"] = self._data[SummonerData].accountId
         except AttributeError:
             pass
-        try:
-            query["name"] = self._data[SummonerData].name
-        except AttributeError:
-            pass
-        assert (
-            "id" in query or "name" in query or "accountId" in query or "puuid" in query
-        )
+        assert "id" in query or "accountId" in query or "puuid" in query
         return query
 
     def __eq__(self, other: "Summoner"):
         if not isinstance(other, Summoner) or self.region != other.region:
             return False
         s = {}
         o = {}
         if hasattr(self._data[SummonerData], "id"):
             s["id"] = self.id
         if hasattr(other._data[SummonerData], "id"):
             o["id"] = other.id
-        if hasattr(self._data[SummonerData], "name"):
-            s["name"] = self.sanitized_name
-        if hasattr(other._data[SummonerData], "name"):
-            o["name"] = other.sanitized_name
         if hasattr(self._data[SummonerData], "accountId"):
             s["accountId"] = self.account_id
         if hasattr(other._data[SummonerData], "accountId"):
             o["accountId"] = other.account_id
         if any(s.get(key, "s") == o.get(key, "o") for key in s):
             return True
         else:
             return self.id == other.id
 
     def __str__(self):
         id_ = "?"
-        name = "?"
         if hasattr(self._data[SummonerData], "id"):
             id_ = self.id
-        if hasattr(self._data[SummonerData], "name"):
-            name = self.name
         try:
             account_id = self._data[SummonerData].accountId
         except AttributeError:
             account_id = "?"
         try:
             puuid = self._data[SummonerData].puuid
         except AttributeError:
             puuid = "?"
-        return "Summoner(id={id_}, account_id={account_id}, name='{name}', puuid='{puuid}')".format(
-            id_=id_, name=name, account_id=account_id, puuid=puuid
-        )
+        return f"Summoner(id={id_}, account_id={account_id}, puuid='{puuid}')"
 
     @property
     def exists(self):
         try:
             if not self._Ghost__all_loaded:
                 self.__load__()
             self.revision_date  # Make sure we can access this attribute
@@ -159,14 +138,19 @@
         return Region(self._data[SummonerData].region)
 
     @lazy_property
     def platform(self) -> Platform:
         """The platform for this summoner."""
         return self.region.platform
 
+    @lazy_property
+    def continent(self) -> Continent:
+        """The continent for this summoner."""
+        return self.region.continent
+
     @CassiopeiaGhost.property(SummonerData)
     @ghost_load_on
     def account_id(self) -> str:
         return self._data[SummonerData].accountId
 
     @CassiopeiaGhost.property(SummonerData)
     @ghost_load_on
@@ -176,23 +160,14 @@
     @CassiopeiaGhost.property(SummonerData)
     @ghost_load_on
     def id(self) -> str:
         return self._data[SummonerData].id
 
     @CassiopeiaGhost.property(SummonerData)
     @ghost_load_on
-    def name(self) -> str:
-        return self._data[SummonerData].name
-
-    @property
-    def sanitized_name(self) -> str:
-        return self.name.replace(" ", "").lower()
-
-    @CassiopeiaGhost.property(SummonerData)
-    @ghost_load_on
     def level(self) -> str:
         return self._data[SummonerData].level
 
     @CassiopeiaGhost.property(SummonerData)
     @ghost_load_on
     def profile_icon(self) -> ProfileIcon:
         return ProfileIcon(
```

### Comparing `cassiopeia-5.0.4/cassiopeia/core/thirdpartycode.py` & `cassiopeia-5.1.0/cassiopeia/core/thirdpartycode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# TODO: Delete this file and surrounding functionality.
+
+
 from typing import Union
 
 from merakicommons.cache import lazy_property
 
 from ..data import Region, Platform
 from .common import CoreData, CassiopeiaGhost, ghost_load_on
 from .summoner import Summoner
```

### Comparing `cassiopeia-5.0.4/cassiopeia/data.py` & `cassiopeia-5.1.0/cassiopeia/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     overcharge = "OVERCHARGE"
     all_random_urf_snow = "SNOWURF"
     practice_tool = "PRACTICETOOL"
     nexus_blitz = "NEXUSBLITZ"
     odyssey = "ODYSSEY"
     utlbook = "ULTBOOK"
     cherry = "CHERRY"
+    wipmode = "WIPMODEWIP"
 
 
 class MasteryTree(Enum):
     cunning = "Cunning"
     ferocity = "Ferocity"
     resolve = "Resolve"
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/cache.py` & `cassiopeia-5.1.0/cassiopeia/datastores/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     ChallengerLeague,
     GrandmasterLeague,
     MasterLeague,
     LeagueEntries,
 )
 from ..core.match import MatchData, TimelineData, Match, Timeline
 from ..core.summoner import SummonerData, Summoner
+from ..core.account import AccountData, Account
 from ..core.status import ShardStatusData, ShardStatus
 from ..core.spectator import (
     CurrentGameInfoData,
     FeaturedGamesData,
     CurrentMatch,
     FeaturedMatches,
 )
@@ -91,14 +92,15 @@
     League: datetime.timedelta(hours=6),
     ChallengerLeague: datetime.timedelta(hours=6),
     GrandmasterLeague: datetime.timedelta(hours=6),
     MasterLeague: datetime.timedelta(hours=6),
     Match: datetime.timedelta(days=3),
     Timeline: datetime.timedelta(days=1),
     Summoner: datetime.timedelta(days=1),
+    Account: datetime.timedelta(days=1),
     ShardStatus: datetime.timedelta(hours=1),
     CurrentMatch: datetime.timedelta(hours=0.5),
     FeaturedMatches: datetime.timedelta(hours=0.5),
 }
 
 
 class Cache(DataSource, DataSink):
@@ -1293,22 +1295,26 @@
             raise NotFoundError
 
     #############
     # Match API #
     #############
 
     @get.register(Match)
-    @validate_query(uniquekeys.validate_match_query, uniquekeys.convert_region_to_platform)
+    @validate_query(
+        uniquekeys.validate_match_query, uniquekeys.convert_region_to_platform
+    )
     def get_match(
         self, query: Mapping[str, Any], context: PipelineContext = None
     ) -> Match:
         return self._get(Match, query, uniquekeys.for_match_query, context)
 
     @get_many.register(Match)
-    @validate_query(uniquekeys.validate_many_match_query, uniquekeys.convert_region_to_platform)
+    @validate_query(
+        uniquekeys.validate_many_match_query, uniquekeys.convert_region_to_platform
+    )
     def get_many_match(
         self, query: Mapping[str, Any], context: PipelineContext = None
     ) -> Generator[Match, None, None]:
         return self._get_many(Match, query, uniquekeys.for_many_match_query, context)
 
     @put.register(Match)
     def put_match(self, item: Match, context: PipelineContext = None) -> None:
@@ -1317,15 +1323,17 @@
     @put_many.register(Match)
     def put_many_match(
         self, items: Iterable[Match], context: PipelineContext = None
     ) -> None:
         self._put_many(Match, items, uniquekeys.for_match, context=context)
 
     @get.register(MatchData)
-    @validate_query(uniquekeys.validate_match_query, uniquekeys.convert_region_to_platform)
+    @validate_query(
+        uniquekeys.validate_match_query, uniquekeys.convert_region_to_platform
+    )
     def get_match_data(
         self, query: Mapping[str, Any], context: PipelineContext = None
     ) -> MatchData:
         result = self.get_match(query=query, context=context)
         if result._data[MatchData] is not None and result._Ghost__is_loaded(MatchData):
             return result._data[MatchData]
         else:
@@ -1340,15 +1348,16 @@
     def get_match_timeline(
         self, query: Mapping[str, Any], context: PipelineContext = None
     ) -> Timeline:
         return self._get(Timeline, query, uniquekeys.for_match_timeline_query, context)
 
     @get_many.register(Timeline)
     @validate_query(
-        uniquekeys.validate_many_match_timeline_query, uniquekeys.convert_region_to_platform
+        uniquekeys.validate_many_match_timeline_query,
+        uniquekeys.convert_region_to_platform,
     )
     def get_many_match_timeline(
         self, query: Mapping[str, Any], context: PipelineContext = None
     ) -> Generator[Timeline, None, None]:
         return self._get_many(
             Timeline, query, uniquekeys.for_many_match_timeline_query, context
         )
@@ -1524,7 +1533,54 @@
         result = self.get_summoner(query=query, context=context)
         if result._data[SummonerData] is not None and result._Ghost__is_loaded(
             SummonerData
         ):
             return result._data[SummonerData]
         else:
             raise NotFoundError
+
+    ###############
+    # Account API #
+    ###############
+
+    @get.register(Account)
+    @validate_query(
+        uniquekeys.validate_account_query, uniquekeys.convert_region_to_platform
+    )
+    def get_account(
+        self, query: Mapping[str, Any], context: PipelineContext = None
+    ) -> Account:
+        return self._get(Account, query, uniquekeys.for_account_query, context)
+
+    @get_many.register(Account)
+    @validate_query(
+        uniquekeys.validate_many_account_query, uniquekeys.convert_region_to_platform
+    )
+    def get_many_account(
+        self, query: Mapping[str, Any], context: PipelineContext = None
+    ) -> Generator[Account, None, None]:
+        return self._get_many(
+            Account, query, uniquekeys.for_many_account_query, context
+        )
+
+    @put.register(Account)
+    def put_account(self, item: Account, context: PipelineContext = None) -> None:
+        self._put(Account, item, uniquekeys.for_account, context=context)
+
+    @put_many.register(Account)
+    def put_many_account(
+        self, items: Iterable[Account], context: PipelineContext = None
+    ) -> None:
+        self._put_many(Account, items, uniquekeys.for_account, context=context)
+
+    @get.register(Account)
+    @validate_query(
+        uniquekeys.validate_account_query, uniquekeys.convert_region_to_platform
+    )
+    def get_account_data(
+        self, query: Mapping[str, Any], context: PipelineContext = None
+    ) -> Account:
+        result = self.get_account(query=query, context=context)
+        if result._data[Account] is not None and result._Ghost__is_loaded(Account):
+            return result._data[Account]
+        else:
+            raise NotFoundError
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/common.py` & `cassiopeia-5.1.0/cassiopeia/datastores/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/ddragon.py` & `cassiopeia-5.1.0/cassiopeia/datastores/ddragon.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,83 +28,14 @@
     import ujson as json
 except ImportError:
     import json
 
 T = TypeVar("T")
 
 
-# Manually add stat runes since Riot doesn't provide static data for them...
-statperk_health = {
-    "id": 5001,
-    "name": "HealthScaling",
-    "key": "HealthScaling",
-    "shortDesc": "+15-90 Health (based on level)",
-    "longDesc": "+15-90 Health (based on level)",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsHealthScalingIcon.png",
-}
-statperk_armor = {
-    "id": 5002,
-    "name": "Armor",
-    "key": "Armor",
-    "shortDesc": "+6 Armor",
-    "longDesc": "+6 Armor",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsArmorIcon.png",
-}
-statperk_magic_resist = {
-    "id": 5003,
-    "name": "MagicResist",
-    "key": "MagicRes",
-    "shortDesc": "+8 Magic Resist",
-    "longDesc": "+8 Magic Resist",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsMagicResIcon.png",
-}
-statperk_attack_speed = {
-    "id": 5005,
-    "name": "AttackSpeed",
-    "key": "AttackSpeed",
-    "shortDesc": "+10% Attack Speed",
-    "longDesc": "+10% Attack Speed",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsAttackSpeedIcon.png",
-}
-statperk_cdr = {
-    "id": 5007,
-    "name": "CDRScaling",
-    "key": "CDRScaling",
-    "shortDesc": "+1-10% <lol-uikit-tooltipped-keyword key='LinkTooltip_Description_CDR'>CDR</lol-uikit-tooltipped-keyword> (based on level)",
-    "longDesc": "+1-10% <lol-uikit-tooltipped-keyword key='LinkTooltip_Description_CDR'>CDR</lol-uikit-tooltipped-keyword> (based on level)",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsCDRScalingIcon.png",
-}
-statperk_adaptive = {
-    "id": 5008,
-    "name": "Adaptive",
-    "key": "Adaptive",
-    "shortDesc": "+9 <lol-uikit-tooltipped-keyword key='LinkTooltip_Description_Adaptive'><font color='#48C4B7'>Adaptive Force</font></lol-uikit-tooltipped-keyword>",
-    "longDesc": "+9 <lol-uikit-tooltipped-keyword key='LinkTooltip_Description_Adaptive'><font color='#48C4B7'>Adaptive Force</font></lol-uikit-tooltipped-keyword>",
-    "icon": "/lol-game-data/assets/v1/perk-images/StatMods/StatModsAdaptiveForceIcon.png",
-}
-statperks = {
-    "id": 5000,
-    "key": "stats",
-    "name": "stats",
-    "icon": "",
-    "slots": [
-        {
-            "runes": [
-                statperk_health,
-                statperk_armor,
-                statperk_magic_resist,
-                statperk_attack_speed,
-                statperk_cdr,
-                statperk_adaptive,
-            ]
-        }
-    ],
-}
-
-
 class DDragon(DataSource):
     def __init__(self, http_client: HTTPClient = None) -> None:
         if http_client is None:
             self._client = HTTPClient()
         else:
             self._client = http_client
 
@@ -583,14 +514,39 @@
             version=query["version"], locale=locale
         )
         try:
             body = json.loads(self._client.get(url)[0])
         except HTTPError as e:
             raise NotFoundError(str(e)) from e
 
+        cdragon_url = "https://raw.communitydragon.org/pbe/plugins/rcp-be-lol-game-data/global/default/v1/perks.json"
+        try:
+            cdragon_body = json.loads(self._client.get(cdragon_url)[0])
+        except HTTPError as e:
+            raise NotFoundError(str(e)) from e
+
+        cdragon_runes = []
+        for rune in cdragon_body:
+            if str(rune["id"]).startswith("50"):
+                rune = {
+                    "id": rune["id"],
+                    "name": rune["name"],
+                    "key": rune["name"].replace(" ", ""),
+                    "shortDesc": rune["shortDesc"].encode("utf-8").decode("utf-8"),
+                    "longDesc": rune["longDesc"].encode("utf-8").decode("utf-8"),
+                    "icon": rune["iconPath"],
+                }
+                cdragon_runes.append(rune)
+        statperks = {
+            "id": 5000,
+            "key": "stats",
+            "name": "stats",
+            "icon": "",
+            "slots": [{"runes": cdragon_runes}],
+        }
         body.append(statperks)
         for path in body:
             for tier, subpath in enumerate(path["slots"]):
                 for i, rune in enumerate(subpath["runes"]):
                     rune["path"] = {
                         "key": path["key"],
                         "name": path["name"],
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/ghost.py` & `cassiopeia-5.1.0/cassiopeia/datastores/ghost.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Type, TypeVar, MutableMapping, Any, Iterable, Union
-import arrow
+from typing import Type, TypeVar, MutableMapping, Any, Iterable
 import copy
 
 from datapipelines import DataSource, PipelineContext, Query, validate_query
 
 from ..data import Region, Platform, Continent, Queue, Tier, Division, MatchType
 from ..core import (
     Champion,
@@ -11,14 +10,15 @@
     Item,
     Map,
     SummonerSpell,
     Realms,
     ProfileIcon,
     LanguageStrings,
     Summoner,
+    Account,
     ChampionMastery,
     Match,
     CurrentMatch,
     ShardStatus,
     ChallengerLeague,
     GrandmasterLeague,
     MasterLeague,
@@ -357,14 +357,25 @@
         .as_(str)
         .or_("name")
         .as_(str)
         .also.has("platform")
         .as_(Platform)
     )
 
+    _validate_get_account_query = (
+        Query.has("puuid")
+        .as_(str)
+        .or_("name")
+        .as_(str)
+        .or_("tagline")
+        .as_(str)
+        .also.has("platform")
+        .as_(Platform)
+    )
+
     _validate_get_verification_string_query = (
         Query.has("platform").as_(Platform).also.has("summoner.id").as_(str)
     )
 
     @get.register(Champion)
     @validate_query(_validate_get_champion_query, convert_region_to_platform)
     def get_champion(
@@ -439,24 +450,33 @@
     ) -> Summoner:
         kwargs = copy.deepcopy(query)
         kwargs["region"] = kwargs.pop("platform").region
         if "accountId" in kwargs:
             kwargs["account_id"] = kwargs.pop("accountId")
         return Summoner._construct_normally(**kwargs)
 
+    @get.register(Account)
+    @validate_query(_validate_get_account_query, convert_region_to_platform)
+    def get_account(
+        self, query: MutableMapping[str, Any], context: PipelineContext = None
+    ) -> Account:
+        kwargs = copy.deepcopy(query)
+        kwargs["region"] = kwargs.pop("platform").region
+        if "name" in kwargs:
+            kwargs["name"] = kwargs.pop("name")
+        return Account._construct_normally(**kwargs)
+
     @get.register(ChampionMastery)
     @validate_query(_validate_get_champion_mastery_query, convert_region_to_platform)
     def get_champion_mastery(
         self, query: MutableMapping[str, Any], context: PipelineContext = None
     ) -> ChampionMastery:
         query["region"] = query.pop("platform").region
         if "summoner.id" in query:
             query["summoner"] = query.pop("summoner.id")
-        if "summoner.name" in query:
-            query["summoner"] = query.pop("summoner.name")
         if "summoner.accountId" in query:
             query["_account_id"] = query.pop("summoner.accountId")
         if "champion.id" in query:
             query["champion"] = query.pop("champion.id")
         if "champion.id" in query:
             query["champion"] = query.pop("champion.name")
         return ChampionMastery._construct_normally(**query)
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/image.py` & `cassiopeia-5.1.0/cassiopeia/datastores/image.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/__init__.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 
 
 def _default_services(server_url: str, port: int) -> Set[KernelSource]:
     from ..common import HTTPClient
     from ..image import ImageDataSource
     from .champion import ChampionAPI
     from .summoner import SummonerAPI
+    from .account import AccountAPI
     from .championmastery import ChampionMasteryAPI
     from .match import MatchAPI
     from .spectator import SpectatorAPI
     from .status import StatusAPI
     from .leagues import LeaguesAPI
     from .thirdpartycode import ThirdPartyCodeAPI
 
     client = HTTPClient()
     services = {
         ImageDataSource(client),
         ChampionAPI(server_url=server_url, port=port, http_client=client),
         SummonerAPI(server_url=server_url, port=port, http_client=client),
+        AccountAPI(server_url=server_url, port=port, http_client=client),
         ChampionMasteryAPI(server_url=server_url, port=port, http_client=client),
         MatchAPI(server_url=server_url, port=port, http_client=client),
         SpectatorAPI(server_url=server_url, port=port, http_client=client),
         StatusAPI(server_url=server_url, port=port, http_client=client),
         LeaguesAPI(server_url=server_url, port=port, http_client=client),
         ThirdPartyCodeAPI(server_url=server_url, port=port, http_client=client),
     }
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/champion.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/championmastery.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/common.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/leagues.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/match.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/spectator.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/spectator.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/status.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/summoner.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/summoner.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     _validate_get_summoner_query = (
         Query.has("id")
         .as_(str)
         .or_("accountId")
         .as_(str)
         .or_("puuid")
         .as_(str)
-        .or_("name")
-        .as_(str)
         .also.has("platform")
         .as_(Platform)
     )
 
     @get.register(SummonerDto)
     @validate_query(_validate_get_summoner_query, convert_region_to_platform)
     def get_summoner(
@@ -57,18 +55,14 @@
             endpoint = "lol/summoner/v4/summoners/{summonerId}".format(
                 summonerId=query["id"]
             )
         elif "accountId" in query:
             endpoint = "lol/summoner/v4/summoners/by-account/{accountId}".format(
                 accountId=query["accountId"]
             )
-        elif "name" in query:
-            endpoint = "lol/summoner/v4/summoners/by-name/{name}".format(
-                name=query["name"].replace(" ", "%20")
-            )
         elif "puuid" in query:
             endpoint = "lol/summoner/v4/summoners/by-puuid/{puuid}".format(
                 puuid=query["puuid"]
             )
         else:
             RuntimeError("Impossible")
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/kernel/thirdpartycode.py` & `cassiopeia-5.1.0/cassiopeia/datastores/kernel/thirdpartycode.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/lolwikia.py` & `cassiopeia-5.1.0/cassiopeia/datastores/lolwikia.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/merakianalyticscdn.py` & `cassiopeia-5.1.0/cassiopeia/datastores/merakianalyticscdn.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/__init__.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def _default_services(
     api_key: str, limiting_share: float = 1.0, request_error_handling: Dict = None
 ) -> Set[RiotAPIService]:
     from ..common import HTTPClient
     from ..image import ImageDataSource
     from .champion import ChampionAPI
     from .summoner import SummonerAPI
+    from .account import AccountAPI
     from .championmastery import ChampionMasteryAPI
     from .match import MatchAPI
     from .spectator import SpectatorAPI
     from .status import StatusAPI
     from .leagues import LeaguesAPI
     from .thirdpartycode import ThirdPartyCodeAPI
     from ...data import Platform, Continent
@@ -37,14 +38,20 @@
         ),
         SummonerAPI(
             api_key,
             app_rate_limiter=app_rate_limiter,
             request_error_handling=request_error_handling,
             http_client=client,
         ),
+        AccountAPI(
+            api_key,
+            app_rate_limiter=app_rate_limiter,
+            request_error_handling=request_error_handling,
+            http_client=client,
+        ),
         ChampionMasteryAPI(
             api_key,
             app_rate_limiter=app_rate_limiter,
             request_error_handling=request_error_handling,
             http_client=client,
         ),
         MatchAPI(
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/champion.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/championmastery.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/common.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/leagues.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/match.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/spectator.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/spectator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,51 +50,51 @@
         pass
 
     ################
     # Current Game #
     ################
 
     _validate_get_current_game_query = (
-        Query.has("platform").as_(Platform).also.has("summoner.id").as_(str)
+        Query.has("platform").as_(Platform).also.has("summoner.puuid").as_(str)
     )
 
     @get.register(CurrentGameInfoDto)
     @validate_query(_validate_get_current_game_query, convert_region_to_platform)
     def get_current_game(
         self, query: MutableMapping[str, Any], context: PipelineContext = None
     ) -> CurrentGameInfoDto:
-        url = "https://{platform}.api.riotgames.com/lol/spectator/v4/active-games/by-summoner/{id}".format(
-            platform=query["platform"].value.lower(), id=query["summoner.id"]
+        url = "https://{platform}.api.riotgames.com/lol/spectator/v5/active-games/by-summoner/{puuid}".format(
+            platform=query["platform"].value.lower(), puuid=query["summoner.puuid"]
         )
         try:
             app_limiter, method_limiter = self._get_rate_limiter(
                 query["platform"], "spectator/active-games/by-summoner"
             )
             data = self._get(
                 url, {}, app_limiter=app_limiter, method_limiter=method_limiter
             )
         except APINotFoundError as error:
             raise NotFoundError(str(error)) from error
 
         data["region"] = query["platform"].region.value
-        data["summonerId"] = query["summoner.id"]
+        data["puuid"] = query["puuid"]
         return CurrentGameInfoDto(data)
 
     #################
     # Featured Game #
     #################
 
     _validate_get_featured_game_query = Query.has("platform").as_(Platform)
 
     @get.register(FeaturedGamesDto)
     @validate_query(_validate_get_featured_game_query, convert_region_to_platform)
     def get_featured_games(
         self, query: MutableMapping[str, Any], context: PipelineContext = None
     ) -> FeaturedGamesDto:
-        url = "https://{platform}.api.riotgames.com/lol/spectator/v4/featured-games".format(
+        url = "https://{platform}.api.riotgames.com/lol/spectator/v5/featured-games".format(
             platform=query["platform"].value.lower()
         )
         try:
             app_limiter, method_limiter = self._get_rate_limiter(
                 query["platform"], "featured-games"
             )
             data = self._get(
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/status.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/summoner.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/summoner.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     _validate_get_summoner_query = (
         Query.has("id")
         .as_(str)
         .or_("accountId")
         .as_(str)
         .or_("puuid")
         .as_(str)
-        .or_("name")
-        .as_(str)
         .also.has("platform")
         .as_(Platform)
     )
 
     @get.register(SummonerDto)
     @validate_query(_validate_get_summoner_query, convert_region_to_platform)
     def get_summoner(
@@ -59,25 +57,19 @@
             )
             endpoint = "summoners/summonerId"
         elif "accountId" in query:
             url = "https://{platform}.api.riotgames.com/lol/summoner/v4/summoners/by-account/{accountId}".format(
                 platform=query["platform"].value.lower(), accountId=query["accountId"]
             )
             endpoint = "summoners/by-account/accountId"
-        elif "name" in query:
-            name = query["name"].replace(" ", "%20")
-            url = "https://{platform}.api.riotgames.com/lol/summoner/v4/summoners/by-name/{name}".format(
-                platform=query["platform"].value.lower(), name=name
-            )
-            endpoint = "summoners/by-name/name"
         elif "puuid" in query:
-            url = (
-                url
-            ) = "https://{platform}.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/{puuid}".format(
-                platform=query["platform"].value.lower(), puuid=query["puuid"]
+            url = url = (
+                "https://{platform}.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/{puuid}".format(
+                    platform=query["platform"].value.lower(), puuid=query["puuid"]
+                )
             )
             endpoint = "summoners/by-puuid/puuid"
         else:
             endpoint = ""
 
         try:
             app_limiter, method_limiter = self._get_rate_limiter(
```

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/riotapi/thirdpartycode.py` & `cassiopeia-5.1.0/cassiopeia/datastores/riotapi/thirdpartycode.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/datastores/uniquekeys.py` & `cassiopeia-5.1.0/cassiopeia/datastores/uniquekeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     MapListDto,
     VersionListDto,
 )
 from ..dto.status import ShardStatusDto
 from ..dto.match import MatchDto, MatchReferenceDto, TimelineDto
 from ..dto.spectator import CurrentGameInfoDto, FeaturedGamesDto
 from ..dto.summoner import SummonerDto
+from ..dto.account import AccountDto
 
 from ..core.championmastery import ChampionMastery, ChampionMasteries
 from ..core.league import (
     LeagueSummonerEntries,
     ChallengerLeague,
     GrandmasterLeague,
     MasterLeague,
@@ -70,23 +71,25 @@
     Maps,
     SummonerSpells,
     Runes,
 )
 from ..core.status import ShardStatus
 from ..core.match import Match, MatchHistory, Timeline
 from ..core.summoner import Summoner
+from ..core.account import Account
 from ..core.spectator import CurrentMatch, FeaturedMatches, CurrentGameParticipantData
 from ..core.champion import ChampionRotation, ChampionRotationData
 
 from ..core.staticdata.champion import ChampionData
 from ..core.staticdata.item import ItemData
 from ..core.staticdata.summonerspell import SummonerSpellData
 from ..core.staticdata.rune import RuneData
 from ..core.staticdata.map import MapData
 from ..core.summoner import SummonerData
+from ..core.account import AccountData
 
 #############
 # Utilities #
 #############
 
 
 def _rgetattr(obj, key):
@@ -1405,14 +1408,70 @@
         try:
             platform = Platform(platform)
             yield platform.value
         except ValueError as e:
             raise QueryValidationError from e
 
 
+###############
+# Account API #
+###############
+
+validate_account_dto_query = (
+    Query.has("platform")
+    .as_(Platform)
+    .also.has("puuid")
+    .as_(str)
+    .or_("name")
+    .as_(str)
+    .or_("tagline")
+    .as_(str)
+)
+
+validate_many_account_dto_query = (
+    Query.has("platform")
+    .as_(Platform)
+    .also.has("puuid")
+    .as_(Iterable)
+    .or_("name")
+    .as_(Iterable)
+    .or_("tagline")
+    .as_(Iterable)
+)
+
+
+def for_account_dto(
+    account: AccountDto, identifier: str = "puuid"
+) -> Tuple[str, Union[int, str]]:
+    return account["platform"], account[identifier]
+
+
+def for_account_dto_query(query: Query) -> Tuple[str, Union[int, str]]:
+    if "puuid" in query:
+        identifier = "puuid"
+    else:
+        identifier = "name"
+    return query["platform"].value, query[identifier]
+
+
+def for_many_account_dto_query(
+    query: Query,
+) -> Generator[Tuple[str, Union[int, str]], None, None]:
+    if "puuids" in query:
+        identifiers, identifier_type = query["puuids"], str
+    else:
+        identifiers, identifier_type = query["names"], str
+    for identifier in identifiers:
+        try:
+            identifier = identifier_type(identifier)
+            yield query["platform"].value, identifier
+        except ValueError as e:
+            raise QueryValidationError from e
+
+
 ################
 # Summoner API #
 ################
 
 
 validate_summoner_dto_query = (
     Query.has("platform")
@@ -1505,32 +1564,28 @@
 validate_champion_mastery_query = (
     Query.has("platform")
     .as_(Platform)
     .also.has("summoner.id")
     .as_(str)
     .or_("summoner.accountId")
     .as_(str)
-    .or_("summoner.name")
-    .as_(str)
     .also.has("champion.id")
     .as_(int)
     .or_("champion.name")
     .as_(str)
 )
 
 
 validate_many_champion_mastery_query = (
     Query.has("platform")
     .as_(Platform)
     .also.has("summoner.id")
     .as_(str)
     .or_("summoner.accountId")
     .as_(str)
-    .or_("summoner.name")
-    .as_(str)
     .also.has("champions.id")
     .as_(Iterable)
     .or_("champions.name")
     .as_(Iterable)
 )
 
 
@@ -1605,22 +1660,14 @@
         keys.append(
             (query["platform"].value, query["summoner.id"], query["champion.id"])
         )
     if "summoner.id" in query and "champion.name" in query:
         keys.append(
             (query["platform"].value, query["summoner.id"], query["champion.name"])
         )
-    if "summoner.name" in query and "champion.id" in query:
-        keys.append(
-            (query["platform"].value, query["summoner.name"], query["champion.id"])
-        )
-    if "summoner.name" in query and "champion.name" in query:
-        keys.append(
-            (query["platform"].value, query["summoner.name"], query["champion.name"])
-        )
     if "summoner.accountId" in query and "champion.id" in query:
         keys.append(
             (query["platform"].value, query["summoner.accountId"], query["champion.id"])
         )
     if "summoner.accountId" in query and "champion.name" in query:
         keys.append(
             (
@@ -1645,18 +1692,14 @@
         identifier_types.append(str)
     for identifiers in zip(*grouped_identifiers):
         keys = []
         for identifier, identifier_type in zip(identifiers, identifier_types):
             identifier = identifier_type(identifier)
             if "summoner.id" in query:
                 keys.append((query["platform"].value, query["summoner.id"], identifier))
-            if "summoner.name" in query:
-                keys.append(
-                    (query["platform"].value, query["summoner.name"], identifier)
-                )
             if "summoner.accountId" in query:
                 keys.append(
                     (query["platform"].value, query["summoner.accountId"], identifier)
                 )
         if len(keys) == 0:
             raise QueryValidationError
         yield keys
@@ -1665,26 +1708,24 @@
 validate_champion_masteries_query = (
     Query.has("platform")
     .as_(Platform)
     .also.has("summoner.id")
     .as_(str)
     .or_("summoner.accountId")
     .as_(int)
-    .or_("summoner.name")
 )
 
 
 validate_many_champion_masteries_query = (
     Query.has("platform")
     .as_(Platform)
     .also.has("summoner.id")
     .as_(str)
     .or_("summoner.accountId")
     .as_(int)
-    .or_("summoner.name")
 )
 
 
 def for_champion_masteries(champion_mastery: ChampionMasteries) -> List[Tuple]:
     keys = []
     try:
         keys.append(
@@ -1695,37 +1736,26 @@
         )
     except AttributeError:
         pass
     try:
         keys.append(
             (
                 champion_mastery.platform.value,
-                champion_mastery.summoner._data[SummonerData].name,
-            )
-        )
-    except AttributeError:
-        pass
-    try:
-        keys.append(
-            (
-                champion_mastery.platform.value,
                 champion_mastery.summoner._data[SummonerData].account_id,
             )
         )
     except AttributeError:
         pass
     return keys
 
 
 def for_champion_masteries_query(query: Query) -> List[Tuple]:
     keys = []
     if "summoner.id" in query:
         keys.append((query["platform"].value, query["summoner.id"]))
-    if "summoner.name" in query:
-        keys.append((query["platform"].value, query["summoner.name"]))
     if "summoner.accountId" in query:
         keys.append((query["platform"].value, query["summoner.accountId"]))
     return keys
 
 
 ##############
 # League API #
@@ -3203,10 +3233,86 @@
         identifier_types.append(str)
     for identifiers in zip(*grouped_identifiers):
         keys = []
         for identifier, identifier_type in zip(identifiers, identifier_types):
             try:
                 identifier = identifier_type(identifier)
                 keys.append((query["platform"].value, identifier))
+            except ValueError as e:
+                raise QueryValidationError from e
+        yield keys
+
+
+###############
+# Account API #
+##############
+
+
+validate_account_query = (
+    Query.has("platform")
+    .as_(Platform)
+    .also.has("puuid")
+    .as_(str)
+    .or_("name")
+    .as_(str)
+    .or_("tagline")
+)
+
+
+validate_many_account_query = (
+    Query.has("platform")
+    .as_(Platform)
+    .also.has("puuids")
+    .as_(Iterable)
+    .or_("names")
+    .as_(Iterable)
+    .or_("taglines")
+    .as_(Iterable)
+)
+
+
+def for_account(account: Account) -> List[Tuple]:
+    keys = []
+    try:
+        keys.append((account.platform.value, "puuid", account._data[AccountData].puuid))
+    except AttributeError:
+        pass
+    try:
+        keys.append(
+            (
+                account.platform.value,
+                "name",
+                account._data[AccountData].name,
+                account.data[AccountData].tagline,
+            )
+        )
+    except AttributeError:
+        pass
+    return keys
+
+
+def for_account_query(query: Query) -> List[Tuple]:
+    keys = []
+    if "puuid" in query:
+        keys.append((query["platform"].value, "puuid", query["puuid"]))
+    if "name" in query and "tagline" in query:
+        keys.append(
+            (query["platform"].value, "gameName", query["name"], query["tagline"])
+        )
+    return keys
+
+
+def for_many_account_query(query: Query) -> Generator[List[Tuple], None, None]:
+    grouped_identifiers = []
+    identifier_types = []
+    if "puuids" in query:
+        grouped_identifiers.append(query["puuids"])
+        identifier_types.append(str)
+    for identifiers in zip(*grouped_identifiers):
+        keys = []
+        for identifier, identifier_type in zip(identifiers, identifier_types):
+            try:
+                identifier = identifier_type(identifier)
+                keys.append((query["platform"].value, identifier))
             except ValueError as e:
                 raise QueryValidationError from e
         yield keys
```

### Comparing `cassiopeia-5.0.4/cassiopeia/dto/staticdata/__init__.py` & `cassiopeia-5.1.0/cassiopeia/dto/staticdata/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/profile_icon_names.json` & `cassiopeia-5.1.0/cassiopeia/profile_icon_names.json`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/resources/summonersRiftAreas.png` & `cassiopeia-5.1.0/cassiopeia/resources/summonersRiftAreas.png`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/__init__.py` & `cassiopeia-5.1.0/cassiopeia/transformers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from datapipelines import CompositeDataTransformer
 
 from .staticdata import StaticDataTransformer
 from .champion import ChampionTransformer
 from .championmastery import ChampionMasteryTransformer
 from .summoner import SummonerTransformer
+from .account import AccountTransformer
 from .match import MatchTransformer
 from .spectator import SpectatorTransformer
 from .status import StatusTransformer
 from .leagues import LeagueTransformer
 from .thirdpartycode import ThirdPartyCodeTransformer
 
 
 riotapi_transformer = CompositeDataTransformer(
     [
         StaticDataTransformer(),
         ChampionTransformer(),
         ChampionMasteryTransformer(),
         SummonerTransformer(),
+        AccountTransformer(),
         MatchTransformer(),
         SpectatorTransformer(),
         StatusTransformer(),
         LeagueTransformer(),
         ThirdPartyCodeTransformer(),
     ]
 )
```

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/champion.py` & `cassiopeia-5.1.0/cassiopeia/transformers/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/championmastery.py` & `cassiopeia-5.1.0/cassiopeia/transformers/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/leagues.py` & `cassiopeia-5.1.0/cassiopeia/transformers/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/match.py` & `cassiopeia-5.1.0/cassiopeia/transformers/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/spectator.py` & `cassiopeia-5.1.0/cassiopeia/transformers/spectator.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,28 +47,29 @@
     # @transform.register(CurrentGameInfoData, CurrentMatch)
     def current_game_data_to_core(
         self, value: CurrentGameInfoData, context: PipelineContext = None
     ) -> CurrentMatch:
         from ..core.summoner import Summoner
 
         summoner = Summoner(
-            name=value.teams[0].participants[0].summoner_name,
+            puuid=value.teams[0].participants[0].puuid,
             id=value.teams[0].participants[0].summoner_id,
             region=value.region,
         )
         return CurrentMatch.from_data(value, summoner=summoner)
 
     # @transform.register(FeaturedGamesData, FeaturedMatches)
     def featured_games_data_to_core(
         self, value: FeaturedGamesData, context: PipelineContext = None
     ) -> FeaturedMatches:
         from ..core.summoner import Summoner
 
         matches = []
         for match in value:
+            # TODO: What do we do here? Do we delete the name field? Do we need a puuid?
             summoner = Summoner(
                 name=match.teams[0].participants[0].summoner_name,
                 id=match.teams[0].participants[0].summoner_id,
                 region=value.region,
             )
             match = CurrentMatch.from_data(match, summoner=summoner)
             matches.append(match)
```

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/staticdata.py` & `cassiopeia-5.1.0/cassiopeia/transformers/staticdata.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/status.py` & `cassiopeia-5.1.0/cassiopeia/transformers/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/summoner.py` & `cassiopeia-5.1.0/cassiopeia/transformers/summoner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Type, TypeVar
-from copy import deepcopy
 
 from datapipelines import DataTransformer, PipelineContext
 
 from ..core.summoner import SummonerData, Summoner
 from ..dto.summoner import SummonerDto
 
 T = TypeVar("T")
```

### Comparing `cassiopeia-5.0.4/cassiopeia/transformers/thirdpartycode.py` & `cassiopeia-5.1.0/cassiopeia/transformers/thirdpartycode.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/cassiopeia.egg-info/PKG-INFO` & `cassiopeia-5.1.0/cassiopeia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassiopeia
-Version: 5.0.4
+Version: 5.1.0
 Summary: Riot Games Developer API Wrapper (3rd Party)
 Home-page: https://github.com/meraki-analytics/cassiopeia
 Author: Jason Maldonis; Rob Rua
 Author-email: team@merakianalytics.com
 License: MIT
 Keywords: LoL,League of Legends,Riot Games,API,REST
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cassiopeia-5.0.4/cassiopeia.egg-info/SOURCES.txt` & `cassiopeia-5.1.0/cassiopeia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 cassiopeia.egg-info/top_level.txt
 cassiopeia.egg-info/zip-safe
 cassiopeia/_configuration/__init__.py
 cassiopeia/_configuration/all_plugins.json
 cassiopeia/_configuration/load.py
 cassiopeia/_configuration/settings.py
 cassiopeia/core/__init__.py
+cassiopeia/core/account.py
 cassiopeia/core/champion.py
 cassiopeia/core/championmastery.py
 cassiopeia/core/common.py
 cassiopeia/core/league.py
 cassiopeia/core/match.py
 cassiopeia/core/patch.py
 cassiopeia/core/spectator.py
@@ -46,34 +47,37 @@
 cassiopeia/datastores/ddragon.py
 cassiopeia/datastores/ghost.py
 cassiopeia/datastores/image.py
 cassiopeia/datastores/lolwikia.py
 cassiopeia/datastores/merakianalyticscdn.py
 cassiopeia/datastores/uniquekeys.py
 cassiopeia/datastores/kernel/__init__.py
+cassiopeia/datastores/kernel/account.py
 cassiopeia/datastores/kernel/champion.py
 cassiopeia/datastores/kernel/championmastery.py
 cassiopeia/datastores/kernel/common.py
 cassiopeia/datastores/kernel/leagues.py
 cassiopeia/datastores/kernel/match.py
 cassiopeia/datastores/kernel/spectator.py
 cassiopeia/datastores/kernel/status.py
 cassiopeia/datastores/kernel/summoner.py
 cassiopeia/datastores/kernel/thirdpartycode.py
 cassiopeia/datastores/riotapi/__init__.py
+cassiopeia/datastores/riotapi/account.py
 cassiopeia/datastores/riotapi/champion.py
 cassiopeia/datastores/riotapi/championmastery.py
 cassiopeia/datastores/riotapi/common.py
 cassiopeia/datastores/riotapi/leagues.py
 cassiopeia/datastores/riotapi/match.py
 cassiopeia/datastores/riotapi/spectator.py
 cassiopeia/datastores/riotapi/status.py
 cassiopeia/datastores/riotapi/summoner.py
 cassiopeia/datastores/riotapi/thirdpartycode.py
 cassiopeia/dto/__init__.py
+cassiopeia/dto/account.py
 cassiopeia/dto/champion.py
 cassiopeia/dto/championmastery.py
 cassiopeia/dto/common.py
 cassiopeia/dto/league.py
 cassiopeia/dto/match.py
 cassiopeia/dto/patch.py
 cassiopeia/dto/spectator.py
@@ -89,14 +93,15 @@
 cassiopeia/dto/staticdata/profileicon.py
 cassiopeia/dto/staticdata/realm.py
 cassiopeia/dto/staticdata/rune.py
 cassiopeia/dto/staticdata/summonerspell.py
 cassiopeia/dto/staticdata/version.py
 cassiopeia/resources/summonersRiftAreas.png
 cassiopeia/transformers/__init__.py
+cassiopeia/transformers/account.py
 cassiopeia/transformers/champion.py
 cassiopeia/transformers/championmastery.py
 cassiopeia/transformers/leagues.py
 cassiopeia/transformers/match.py
 cassiopeia/transformers/spectator.py
 cassiopeia/transformers/staticdata.py
 cassiopeia/transformers/status.py
```

### Comparing `cassiopeia-5.0.4/setup.py` & `cassiopeia-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Require python 3.6
 if sys.version_info.major != 3 and sys.version_info.minor != 6:
     sys.exit("Cassiopeia requires Python 3.6.")
 
 setup(
     name="cassiopeia",
-    version="5.0.4",  # Keep the Cass version at parity with the largest Riot API major version, use the minor version for breaking changes, and the patch version for everything else
+    version="5.1.0",  # Keep the Cass version at parity with the largest Riot API major version, use the minor version for breaking changes, and the patch version for everything else
     author="Jason Maldonis; Rob Rua",
     author_email="team@merakianalytics.com",
     url="https://github.com/meraki-analytics/cassiopeia",
     description="Riot Games Developer API Wrapper (3rd Party)",
     keywords=["LoL", "League of Legends", "Riot Games", "API", "REST"],
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `cassiopeia-5.0.4/test/constants.py` & `cassiopeia-5.1.0/test/constants.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_champion.py` & `cassiopeia-5.1.0/test/test_champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_championmastery.py` & `cassiopeia-5.1.0/test/test_championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_examples.py` & `cassiopeia-5.1.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_items.py` & `cassiopeia-5.1.0/test/test_items.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_league.py` & `cassiopeia-5.1.0/test/test_league.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_map_location.py` & `cassiopeia-5.1.0/test/test_map_location.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_match.py` & `cassiopeia-5.1.0/test/test_match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_matchhistory.py` & `cassiopeia-5.1.0/test/test_matchhistory.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_patches.py` & `cassiopeia-5.1.0/test/test_patches.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_status.py` & `cassiopeia-5.1.0/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.0.4/test/test_summoner.py` & `cassiopeia-5.1.0/test/test_summoner.py`

 * *Files identical despite different names*

