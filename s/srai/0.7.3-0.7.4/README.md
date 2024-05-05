# Comparing `tmp/srai-0.7.3.tar.gz` & `tmp/srai-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.7.3.tar", last modified: Sun Apr 21 17:32:43 2024, max compression
+gzip compressed data, was "srai-0.7.4.tar", last modified: Sun May  5 19:11:38 2024, max compression
```

## Comparing `srai-0.7.3.tar` & `srai-0.7.4.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0    10760 2024-04-21 17:32:24.518289 srai-0.7.3/LICENSE.md
--rw-r--r--   0        0        0    18091 2024-04-21 17:32:24.518289 srai-0.7.3/README.md
--rw-r--r--   0        0        0     5261 2024-04-21 17:32:43.102470 srai-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      428 2024-04-21 17:32:24.530290 srai-0.7.3/srai/__init__.py
--rw-r--r--   0        0        0     2904 2024-04-21 17:32:24.530290 srai-0.7.3/srai/_optional.py
--rw-r--r--   0        0        0      717 2024-04-21 17:32:24.530290 srai-0.7.3/srai/_typing.py
--rw-r--r--   0        0        0      155 2024-04-21 17:32:24.530290 srai-0.7.3/srai/constants.py
--rw-r--r--   0        0        0      854 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/_base.py
--rw-r--r--   0        0        0      482 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/_pytorch_stubs.py
--rw-r--r--   0        0        0     9181 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     8180 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      186 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/__init__.py
--rw-r--r--   0        0        0     6882 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/dataset.py
--rw-r--r--   0        0        0     9809 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/embedder.py
--rw-r--r--   0        0        0    18081 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/geovex/model.py
--rw-r--r--   0        0        0      136 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0    11336 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2278 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0    10941 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6804 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6301 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     7919 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2855 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2024-04-21 17:32:24.534290 srai-0.7.3/srai/exceptions.py
--rw-r--r--   0        0        0     4247 2024-04-21 17:32:24.534290 srai-0.7.3/srai/geometry.py
--rw-r--r--   0        0        0     9060 2024-04-21 17:32:24.534290 srai-0.7.3/srai/h3.py
--rw-r--r--   0        0        0      531 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      820 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/_base.py
--rw-r--r--   0        0        0     1343 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/download.py
--rw-r--r--   0        0        0     2189 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5391 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     7765 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      472 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     4402 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5315 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0    10696 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15751 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2447 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5996 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     9286 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2778 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     5033 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0      124 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7556 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    14142 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      468 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     6176 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     3609 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     4632 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      497 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11418 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14129 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0       55 2024-04-21 17:32:24.534290 srai-0.7.3/srai/py.typed
--rw-r--r--   0        0        0     1006 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    27555 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15629 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2477 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/geocode.py
--rw-r--r--   0        0        0     2610 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3136 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4184 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     6001 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0       29 2024-04-21 17:32:24.534290 srai-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0     7806 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/conftest.py
--rw-r--r--   0        0        0     1015 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/constants.py
--rw-r--r--   0        0        0     6245 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/generation.py
--rw-r--r--   0        0        0     4211 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/test_dataset.py
--rw-r--r--   0        0        0     4049 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/test_embedder.py
--rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_0.pt
--rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_1.pt
--rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_2.pt
--rw-r--r--   0        0        0   339453 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_3.pt
--rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
--rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
--rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
--rw-r--r--   0        0        0     1755 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
--rw-r--r--   0        0        0    75958 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_features.parquet
--rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.542290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_0.pt
--rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_1.pt
--rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_2.pt
--rw-r--r--   0        0        0   678407 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_3.pt
--rw-r--r--   0        0        0     7011 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_1.pt
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_2.pt
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_3.pt
--rw-r--r--   0        0        0    13915 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_regions.parquet
--rw-r--r--   0        0        0    24970 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_result.parquet
--rw-r--r--   0        0        0   272893 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_0.pt
--rw-r--r--   0        0        0   245693 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_1.pt
--rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
--rw-r--r--   0        0        0     2011 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
--rw-r--r--   0        0        0   803774 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0   545287 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_0.pt
--rw-r--r--   0        0        0   490887 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_1.pt
--rw-r--r--   0        0        0    76452 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_1.pt
--rw-r--r--   0        0        0    10162 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    21999 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     4538 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_model.py
--rw-r--r--   0        0        0      579 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2782 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     3013 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1056 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3058 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    27244 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0    12298 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3631 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     2838 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/conftest.py
--rw-r--r--   0        0        0     3035 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/test_ij_coordinates.py
--rw-r--r--   0        0        0     3083 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/test_shapely_conversion.py
--rw-r--r--   0        0        0     1765 2024-04-21 17:32:24.558290 srai-0.7.3/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2530 2024-04-21 17:32:24.558290 srai-0.7.3/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4285 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     4094 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3283 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0   111539 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     3026 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     4921 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3159 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3142 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3803 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_1.pkl
--rw-r--r--   0        0        0     3334 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_2.pkl
--rw-r--r--   0        0        0     5099 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_3.pkl
--rw-r--r--   0        0        0     3803 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_4.pkl
--rw-r--r--   0        0        0    11234 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2182 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3177 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4878 2024-04-21 17:32:24.562290 srai-0.7.3/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     8340 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     9166 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0    11395 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0    11019 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0      765 2024-04-21 17:32:24.562290 srai-0.7.3/tests/plotting/test_folium_wrapper.py
--rw-r--r--   0        0        0     3729 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6509 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2616 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1856 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2690 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     9215 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    20380 1970-01-01 00:00:00.000000 srai-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-05-05 19:10:31.586392 srai-0.7.4/LICENSE.md
+-rw-r--r--   0        0        0    18091 2024-05-05 19:10:31.586392 srai-0.7.4/README.md
+-rw-r--r--   0        0        0     5335 2024-05-05 19:11:38.730404 srai-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-05-05 19:10:31.598392 srai-0.7.4/srai/__init__.py
+-rw-r--r--   0        0        0     2904 2024-05-05 19:10:31.598392 srai-0.7.4/srai/_optional.py
+-rw-r--r--   0        0        0      717 2024-05-05 19:10:31.598392 srai-0.7.4/srai/_typing.py
+-rw-r--r--   0        0        0      155 2024-05-05 19:10:31.598392 srai-0.7.4/srai/constants.py
+-rw-r--r--   0        0        0      854 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4846 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/_base.py
+-rw-r--r--   0        0        0      482 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/_pytorch_stubs.py
+-rw-r--r--   0        0        0    13531 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     8180 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      186 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/geovex/__init__.py
+-rw-r--r--   0        0        0     6882 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/geovex/dataset.py
+-rw-r--r--   0        0        0     9809 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/geovex/embedder.py
+-rw-r--r--   0        0        0    18081 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/geovex/model.py
+-rw-r--r--   0        0        0      136 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11336 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2278 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10941 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6804 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6301 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7919 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2855 2024-05-05 19:10:31.598392 srai-0.7.4/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2024-05-05 19:10:31.598392 srai-0.7.4/srai/exceptions.py
+-rw-r--r--   0        0        0     4247 2024-05-05 19:10:31.598392 srai-0.7.4/srai/geometry.py
+-rw-r--r--   0        0        0     9060 2024-05-05 19:10:31.598392 srai-0.7.4/srai/h3.py
+-rw-r--r--   0        0        0      531 2024-05-05 19:10:31.598392 srai-0.7.4/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-05 19:10:31.598392 srai-0.7.4/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2024-05-05 19:10:31.598392 srai-0.7.4/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      820 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/_base.py
+-rw-r--r--   0        0        0     1343 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/download.py
+-rw-r--r--   0        0        0     2189 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5391 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     7765 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      472 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     4402 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5315 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0    10696 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15751 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2447 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5996 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     9286 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2778 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     5033 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0      124 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7556 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    14142 2024-05-05 19:10:31.598392 srai-0.7.4/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      468 2024-05-05 19:10:31.598392 srai-0.7.4/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     6176 2024-05-05 19:10:31.598392 srai-0.7.4/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     3609 2024-05-05 19:10:31.598392 srai-0.7.4/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     4632 2024-05-05 19:10:31.598392 srai-0.7.4/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      497 2024-05-05 19:10:31.602392 srai-0.7.4/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11418 2024-05-05 19:10:31.602392 srai-0.7.4/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14129 2024-05-05 19:10:31.602392 srai-0.7.4/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0       55 2024-05-05 19:10:31.602392 srai-0.7.4/srai/py.typed
+-rw-r--r--   0        0        0     1006 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    27555 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15629 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2477 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/geocode.py
+-rw-r--r--   0        0        0     2610 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3136 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4184 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     6001 2024-05-05 19:10:31.602392 srai-0.7.4/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0       29 2024-05-05 19:10:31.602392 srai-0.7.4/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/conftest.py
+-rw-r--r--   0        0        0     1015 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/geovex/constants.py
+-rw-r--r--   0        0        0     6245 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/geovex/generation.py
+-rw-r--r--   0        0        0     4211 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/geovex/test_dataset.py
+-rw-r--r--   0        0        0     4049 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/geovex/test_embedder.py
+-rw-r--r--   0        0        0   484605 2024-05-05 19:10:31.602392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_0.pt
+-rw-r--r--   0        0        0   484605 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_1.pt
+-rw-r--r--   0        0        0   484605 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_2.pt
+-rw-r--r--   0        0        0   339453 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_3.pt
+-rw-r--r--   0        0        0     2139 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2139 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
+-rw-r--r--   0        0        0     2139 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
+-rw-r--r--   0        0        0     1755 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
+-rw-r--r--   0        0        0    75958 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_features.parquet
+-rw-r--r--   0        0        0   968711 2024-05-05 19:10:31.606392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_0.pt
+-rw-r--r--   0        0        0   968711 2024-05-05 19:10:31.610392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_1.pt
+-rw-r--r--   0        0        0   968711 2024-05-05 19:10:31.610392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_2.pt
+-rw-r--r--   0        0        0   678407 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_3.pt
+-rw-r--r--   0        0        0     7011 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_joint.parquet
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_1.pt
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_2.pt
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_3.pt
+-rw-r--r--   0        0        0    13915 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_regions.parquet
+-rw-r--r--   0        0        0    24970 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/AL_10_result.parquet
+-rw-r--r--   0        0        0   272893 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_batch_0.pt
+-rw-r--r--   0        0        0   245693 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_batch_1.pt
+-rw-r--r--   0        0        0     2139 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2011 2024-05-05 19:10:31.614392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
+-rw-r--r--   0        0        0   803774 2024-05-05 19:10:31.618392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0   545287 2024-05-05 19:10:31.618392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_forward_0.pt
+-rw-r--r--   0        0        0   490887 2024-05-05 19:10:31.618392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_forward_1.pt
+-rw-r--r--   0        0        0    76452 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_loss_1.pt
+-rw-r--r--   0        0        0    10162 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    21999 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     4538 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/geovex/test_model.py
+-rw-r--r--   0        0        0      579 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2782 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     3013 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1056 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3058 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    28665 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0    12298 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3631 2024-05-05 19:10:31.622392 srai-0.7.4/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     2838 2024-05-05 19:10:31.622392 srai-0.7.4/tests/h3/conftest.py
+-rw-r--r--   0        0        0     3035 2024-05-05 19:10:31.626392 srai-0.7.4/tests/h3/test_ij_coordinates.py
+-rw-r--r--   0        0        0     3083 2024-05-05 19:10:31.626392 srai-0.7.4/tests/h3/test_shapely_conversion.py
+-rw-r--r--   0        0        0     1765 2024-05-05 19:10:31.626392 srai-0.7.4/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2530 2024-05-05 19:10:31.626392 srai-0.7.4/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4285 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     4094 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3283 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0   111539 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     3026 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     4921 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3159 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3142 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3803 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_1.pkl
+-rw-r--r--   0        0        0     3334 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_2.pkl
+-rw-r--r--   0        0        0     5099 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_3.pkl
+-rw-r--r--   0        0        0     3803 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_4.pkl
+-rw-r--r--   0        0        0    11234 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2182 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3177 2024-05-05 19:10:31.626392 srai-0.7.4/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4878 2024-05-05 19:10:31.626392 srai-0.7.4/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     8340 2024-05-05 19:10:31.626392 srai-0.7.4/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     9166 2024-05-05 19:10:31.630392 srai-0.7.4/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0    11395 2024-05-05 19:10:31.630392 srai-0.7.4/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0    11019 2024-05-05 19:10:31.630392 srai-0.7.4/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0      765 2024-05-05 19:10:31.630392 srai-0.7.4/tests/plotting/test_folium_wrapper.py
+-rw-r--r--   0        0        0     3729 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6509 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2616 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1856 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2690 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     9215 2024-05-05 19:10:31.630392 srai-0.7.4/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    20431 1970-01-01 00:00:00.000000 srai-0.7.4/PKG-INFO
```

### Comparing `srai-0.7.3/LICENSE.md` & `srai-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/README.md` & `srai-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/pyproject.toml` & `srai-0.7.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.7.3"
+version = "0.7.4"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "Piotr Gramacki", email = "pgramacki@kraina.ai" },
     { name = "Kacper Leśniara", email = "klesniara@kraina.ai" },
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
     { name = "Szymon Woźniak", email = "swozniak@kraina.ai" },
 ]
@@ -35,14 +35,15 @@
     "Topic :: Scientific/Engineering :: GIS",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 
 [project.license]
 text = "Apache-2.0"
@@ -54,15 +55,15 @@
 Changelog = "https://github.com/kraina-ai/srai/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 osm = [
     "overpass",
     "pillow",
     "beautifulsoup4",
-    "quackosm>=0.4.2",
+    "quackosm>=0.7.1",
 ]
 voronoi = [
     "pymap3d",
     "haversine",
     "scipy",
     "spherical-geometry",
 ]
@@ -128,14 +129,15 @@
     "mkdocs-awesome-pages-plugin",
     "mike<2",
     "scikit-learn",
     "umap-learn",
 ]
 license = [
     "licensecheck",
+    "pipdeptree",
 ]
 
 [tool.pdm.scripts]
 post_install = "pre-commit install"
 
 [tool.ruff]
 line-length = 100
@@ -198,15 +200,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.3"
+current_version = "0.7.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
@@ -228,15 +230,15 @@
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
 ]
 log_cli = true
 
 [tool.licensecheck]
 using = "requirements"
-zero = false
+zero = true
 ignore_licenses = [
     "UNKNOWN",
 ]
 ignore_packages = [
     "srai",
     "scalene",
     "docformatter",
@@ -263,8 +265,9 @@
     "nvidia-cufft-cu12",
     "nvidia-curand-cu12",
     "nvidia-cusolver-cu12",
     "nvidia-cusparse-cu12",
     "nvidia-nccl-cu12",
     "nvidia-nvtx-cu12",
     "nvidia-nvjitlink-cu12",
+    "mkl",
 ]
```

### Comparing `srai-0.7.3/srai/_optional.py` & `srai-0.7.4/srai/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/_typing.py` & `srai-0.7.4/srai/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/__init__.py` & `srai-0.7.4/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/_base.py` & `srai-0.7.4/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/count_embedder.py` & `srai-0.7.4/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/geovex/dataset.py` & `srai-0.7.4/srai/embedders/geovex/dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/geovex/embedder.py` & `srai-0.7.4/srai/embedders/geovex/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/geovex/model.py` & `srai-0.7.4/srai/embedders/geovex/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/gtfs2vec/embedder.py` & `srai-0.7.4/srai/embedders/gtfs2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/gtfs2vec/model.py` & `srai-0.7.4/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/hex2vec/embedder.py` & `srai-0.7.4/srai/embedders/hex2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/hex2vec/model.py` & `srai-0.7.4/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.7.4/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/highway2vec/embedder.py` & `srai-0.7.4/srai/embedders/highway2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/embedders/highway2vec/model.py` & `srai-0.7.4/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/exceptions.py` & `srai-0.7.4/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/geometry.py` & `srai-0.7.4/srai/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/h3.py` & `srai-0.7.4/srai/h3.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/joiners/__init__.py` & `srai-0.7.4/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/joiners/_base.py` & `srai-0.7.4/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/joiners/intersection_joiner.py` & `srai-0.7.4/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/__init__.py` & `srai-0.7.4/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/_base.py` & `srai-0.7.4/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/download.py` & `srai-0.7.4/srai/loaders/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/geoparquet_loader.py` & `srai-0.7.4/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/gtfs_loader.py` & `srai-0.7.4/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/_base.py` & `srai-0.7.4/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.7.4/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.7.4/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.7.4/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.7.4/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.7.4/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.7.4/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.7.4/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.7.4/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.7.4/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_way_loader/constants.py` & `srai-0.7.4/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.7.4/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/neighbourhoods/_base.py` & `srai-0.7.4/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.7.4/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.7.4/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/plotting/folium_wrapper.py` & `srai-0.7.4/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/plotting/plotly_wrapper.py` & `srai-0.7.4/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/__init__.py` & `srai-0.7.4/srai/regionalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/_base.py` & `srai-0.7.4/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/_spherical_voronoi.py` & `srai-0.7.4/srai/regionalizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.7.4/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/geocode.py` & `srai-0.7.4/srai/regionalizers/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/h3_regionalizer.py` & `srai-0.7.4/srai/regionalizers/h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/s2_regionalizer.py` & `srai-0.7.4/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.7.4/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.7.4/srai/regionalizers/voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/conftest.py` & `srai-0.7.4/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/constants.py` & `srai-0.7.4/tests/embedders/geovex/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/generation.py` & `srai-0.7.4/tests/embedders/geovex/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_dataset.py` & `srai-0.7.4/tests/embedders/geovex/test_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_embedder.py` & `srai-0.7.4/tests/embedders/geovex/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_2.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_3.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_batch_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_features.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_2.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_3.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_joint.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_2.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_3.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_loss_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_regions.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_result.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/AL_10_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_features.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_joint.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_0.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_1.pt` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_regions.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_result.parquet` & `srai-0.7.4/tests/embedders/geovex/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/geovex/test_model.py` & `srai-0.7.4/tests/embedders/geovex/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/constants.py` & `srai-0.7.4/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/generation.py` & `srai-0.7.4/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_embedder.py` & `srai-0.7.4/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.7.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_model.py` & `srai-0.7.4/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.7.4/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/test_contextual_count_embedder.py` & `srai-0.7.4/tests/embedders/test_contextual_count_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """ContextualCountEmbedder tests."""
 
 from contextlib import nullcontext as does_not_raise
-from typing import TYPE_CHECKING, Any, Union
+from pathlib import Path
+from typing import Any, Union
 
+import geopandas as gpd
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal
 from parametrization import Parametrization as P
+from shapely.geometry import Polygon
 
-from srai.constants import REGIONS_INDEX
+from srai.constants import REGIONS_INDEX, WGS84_CRS
 from srai.embedders import ContextualCountEmbedder
-from srai.loaders.osm_loaders.filters import OsmTagsFilter
+from srai.joiners import IntersectionJoiner
+from srai.loaders.osm_loaders import OSMPbfLoader
+from srai.loaders.osm_loaders.filters import GEOFABRIK_LAYERS, OsmTagsFilter
 from srai.neighbourhoods import H3Neighbourhood
-
-if TYPE_CHECKING:  # pragma: no cover
-    import geopandas as gpd
+from srai.regionalizers import H3Regionalizer
 
 
 def _create_features_dataframe(data: dict[str, Any]) -> pd.DataFrame:
     return pd.DataFrame(data).set_index(REGIONS_INDEX)
 
 
 @pytest.fixture  # type: ignore
@@ -717,15 +720,17 @@
     )
     embedding_df = embedder.transform(
         regions_gdf=gdf_regions, features_gdf=gdf_features, joint_gdf=gdf_joint
     )
 
     expected_result_df = request.getfixturevalue(expected_embedding_fixture)
     assert_frame_equal(
-        embedding_df.sort_index(axis=1), expected_result_df.sort_index(axis=1), check_dtype=False
+        embedding_df.sort_index(axis=1),
+        expected_result_df.sort_index(axis=1),
+        check_dtype=False,
     )
 
 
 def test_negative_nighbourhood_distance() -> None:
     """Test checks if negative neighbouthood distance is disallowed."""
     with pytest.raises(ValueError):
         ContextualCountEmbedder(neighbourhood=H3Neighbourhood(), neighbourhood_distance=-1)
@@ -869,7 +874,43 @@
     with expectation:
         ContextualCountEmbedder(
             neighbourhood=H3Neighbourhood(),
             count_subcategories=count_subcategories,
             concatenate_vectors=concatenate_features,
             neighbourhood_distance=neighbourhood_distance,
         ).transform(regions_gdf=regions_gdf, features_gdf=features_gdf, joint_gdf=joint_gdf)
+
+
+def test_bigger_example() -> None:
+    """Test bigger example to get multiprocessing in action."""
+    geometry = gpd.GeoDataFrame(
+        geometry=[
+            Polygon(
+                [
+                    (7.416769421059001, 43.7346112362936),
+                    (7.416769421059001, 43.730681304758946),
+                    (7.4218262821731, 43.730681304758946),
+                    (7.4218262821731, 43.7346112362936),
+                ]
+            )
+        ],
+        crs=WGS84_CRS,
+    )
+
+    regions = H3Regionalizer(resolution=13).transform(geometry)
+    features = OSMPbfLoader(
+        pbf_file=Path(__file__).parent.parent
+        / "loaders"
+        / "osm_loaders"
+        / "test_files"
+        / "monaco.osm.pbf"
+    ).load(area=regions, tags=GEOFABRIK_LAYERS)
+    joint = IntersectionJoiner().transform(regions=regions, features=features)
+    embeddings = ContextualCountEmbedder(
+        neighbourhood=H3Neighbourhood(),
+        neighbourhood_distance=10,
+        expected_output_features=GEOFABRIK_LAYERS,
+    ).transform(regions_gdf=regions, features_gdf=features, joint_gdf=joint)
+
+    assert len(embeddings) == len(
+        regions
+    ), f"Mismatched number of rows ({len(embeddings)}, {len(regions)})"
```

### Comparing `srai-0.7.3/tests/embedders/test_count_embedder.py` & `srai-0.7.4/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.7.4/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/embedders/test_highway2vec_embedder.py` & `srai-0.7.4/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/h3/conftest.py` & `srai-0.7.4/tests/h3/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/h3/test_ij_coordinates.py` & `srai-0.7.4/tests/h3/test_ij_coordinates.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/h3/test_shapely_conversion.py` & `srai-0.7.4/tests/h3/test_shapely_conversion.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/joiners/conftest.py` & `srai-0.7.4/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/joiners/test_intersection_joiner.py` & `srai-0.7.4/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/conftest.py` & `srai-0.7.4/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/conftest.py` & `srai-0.7.4/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.7.4/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.7.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.7.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/monaco.osm.pbf` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.7.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.7.4/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.7.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.7.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.7.4/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_1.pkl` & `srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_1.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_2.pkl` & `srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_3.pkl` & `srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_3.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_4.pkl` & `srai-0.7.4/tests/loaders/osm_way_loader/test_files/graph_4.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.7.4/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/test_files/example.parquet` & `srai-0.7.4/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/test_geoparquet_loader.py` & `srai-0.7.4/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/loaders/test_gtfs_loader.py` & `srai-0.7.4/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.7.4/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.7.4/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.7.4/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.7.4/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.7.4/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/plotting/test_folium_wrapper.py` & `srai-0.7.4/tests/plotting/test_folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/conftest.py` & `srai-0.7.4/tests/regionalizers/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.7.4/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.7.4/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.7.4/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.7.4/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/tests/regionalizers/test_voronoi_regionalizer.py` & `srai-0.7.4/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.3/PKG-INFO` & `srai-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.7.3
+Version: 0.7.4
 Summary: A set of python modules for geospatial machine learning and data mining
 Author-Email: Piotr Gramacki <pgramacki@kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?= <klesniara@kraina.ai>, Kamil Raczycki <kraczycki@kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?= <swozniak@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Project-URL: Homepage, https://kraina-ai.github.io/srai
 Project-URL: Repository, https://github.com/kraina-ai/srai
 Project-URL: Documentation, https://kraina-ai.github.io/srai
 Project-URL: Changelog, https://github.com/kraina-ai/srai/blob/main/CHANGELOG.md
@@ -37,15 +38,15 @@
 Requires-Dist: typeguard
 Requires-Dist: requests
 Requires-Dist: h3ronpy>=0.18.0
 Requires-Dist: osmnx
 Requires-Dist: overpass; extra == "osm"
 Requires-Dist: pillow; extra == "osm"
 Requires-Dist: beautifulsoup4; extra == "osm"
-Requires-Dist: quackosm>=0.4.2; extra == "osm"
+Requires-Dist: quackosm>=0.7.1; extra == "osm"
 Requires-Dist: pymap3d; extra == "voronoi"
 Requires-Dist: haversine; extra == "voronoi"
 Requires-Dist: scipy; extra == "voronoi"
 Requires-Dist: spherical-geometry; extra == "voronoi"
 Requires-Dist: gtfs-kit; extra == "gtfs"
 Requires-Dist: folium; extra == "plotting"
 Requires-Dist: mapclassify; extra == "plotting"
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: srai Version: 0.7.3 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.7.4 Summary: A set of python
 modules for geospatial machine learning and data mining Author-Email: Piotr
 Gramacki
 kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?=
 kraina.ai>, Kamil Raczycki
 kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?=
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Operating System :: Unix Classifier: Operating
-System :: MacOS Classifier: Operating System :: Microsoft :: Windows Project-
-URL: Homepage, https://kraina-ai.github.io/srai Project-URL: Repository, https:
-//github.com/kraina-ai/srai Project-URL: Documentation, https://kraina-
-ai.github.io/srai Project-URL: Changelog, https://github.com/kraina-ai/srai/
-blob/main/CHANGELOG.md Requires-Python: >=3.9 Requires-Dist: pandas Requires-
-Dist: geopandas Requires-Dist: shapely Requires-Dist: h3>=4.0.0b1 Requires-
-Dist: numpy Requires-Dist: geoparquet Requires-Dist: pyfunctional Requires-
-Dist: rtree Requires-Dist: pyarrow>=13.0.0 Requires-Dist: topojson Requires-
-Dist: tqdm Requires-Dist: s2 Requires-Dist: typeguard Requires-Dist: requests
-Requires-Dist: h3ronpy>=0.18.0 Requires-Dist: osmnx Requires-Dist: overpass;
-extra == "osm" Requires-Dist: pillow; extra == "osm" Requires-Dist:
-beautifulsoup4; extra == "osm" Requires-Dist: quackosm>=0.4.2; extra == "osm"
-Requires-Dist: pymap3d; extra == "voronoi" Requires-Dist: haversine; extra ==
-"voronoi" Requires-Dist: scipy; extra == "voronoi" Requires-Dist: spherical-
-geometry; extra == "voronoi" Requires-Dist: gtfs-kit; extra == "gtfs" Requires-
-Dist: folium; extra == "plotting" Requires-Dist: mapclassify; extra ==
-"plotting" Requires-Dist: matplotlib; extra == "plotting" Requires-Dist:
-plotly; extra == "plotting" Requires-Dist: kaleido<=0.2.1; extra == "plotting"
-Requires-Dist: pytorch-lightning; extra == "torch" Requires-Dist: torch; extra
-== "torch" Requires-Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all"
-Provides-Extra: osm Provides-Extra: voronoi Provides-Extra: gtfs Provides-
-Extra: plotting Provides-Extra: torch Provides-Extra: all Description-Content-
-Type: text/markdown
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Operating System :: Unix Classifier: Operating System :: MacOS Classifier:
+Operating System :: Microsoft :: Windows Project-URL: Homepage, https://kraina-
+ai.github.io/srai Project-URL: Repository, https://github.com/kraina-ai/srai
+Project-URL: Documentation, https://kraina-ai.github.io/srai Project-URL:
+Changelog, https://github.com/kraina-ai/srai/blob/main/CHANGELOG.md Requires-
+Python: >=3.9 Requires-Dist: pandas Requires-Dist: geopandas Requires-Dist:
+shapely Requires-Dist: h3>=4.0.0b1 Requires-Dist: numpy Requires-Dist:
+geoparquet Requires-Dist: pyfunctional Requires-Dist: rtree Requires-Dist:
+pyarrow>=13.0.0 Requires-Dist: topojson Requires-Dist: tqdm Requires-Dist: s2
+Requires-Dist: typeguard Requires-Dist: requests Requires-Dist: h3ronpy>=0.18.0
+Requires-Dist: osmnx Requires-Dist: overpass; extra == "osm" Requires-Dist:
+pillow; extra == "osm" Requires-Dist: beautifulsoup4; extra == "osm" Requires-
+Dist: quackosm>=0.7.1; extra == "osm" Requires-Dist: pymap3d; extra ==
+"voronoi" Requires-Dist: haversine; extra == "voronoi" Requires-Dist: scipy;
+extra == "voronoi" Requires-Dist: spherical-geometry; extra == "voronoi"
+Requires-Dist: gtfs-kit; extra == "gtfs" Requires-Dist: folium; extra ==
+"plotting" Requires-Dist: mapclassify; extra == "plotting" Requires-Dist:
+matplotlib; extra == "plotting" Requires-Dist: plotly; extra == "plotting"
+Requires-Dist: kaleido<=0.2.1; extra == "plotting" Requires-Dist: pytorch-
+lightning; extra == "torch" Requires-Dist: torch; extra == "torch" Requires-
+Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm
+Provides-Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-
+Extra: torch Provides-Extra: all Description-Content-Type: text/markdown
 [https://raw.githubusercontent.com/kraina-ai/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
  [GitHub][Checks]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _-_ _D_E_V_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _-_ _P_R_O_D_]
  _[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_C_o_d_e_c_o_v_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d
                       _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 # Spatial Representations for Artificial Intelligence
   â ï¸ð§ This library is under HEAVY development. Expect breaking changes
```

