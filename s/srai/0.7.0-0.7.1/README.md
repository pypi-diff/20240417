# Comparing `tmp/srai-0.7.0.tar.gz` & `tmp/srai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.7.0.tar", last modified: Fri Feb  2 20:10:59 2024, max compression
+gzip compressed data, was "srai-0.7.1.tar", last modified: Wed Apr 17 19:17:29 2024, max compression
```

## Comparing `srai-0.7.0.tar` & `srai-0.7.1.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0    10760 2024-02-02 20:10:06.172602 srai-0.7.0/LICENSE.md
--rw-r--r--   0        0        0    18089 2024-02-02 20:10:06.176602 srai-0.7.0/README.md
--rw-r--r--   0        0        0     5213 2024-02-02 20:10:59.081052 srai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      428 2024-02-02 20:10:06.188602 srai-0.7.0/srai/__init__.py
--rw-r--r--   0        0        0     2904 2024-02-02 20:10:06.188602 srai-0.7.0/srai/_optional.py
--rw-r--r--   0        0        0      717 2024-02-02 20:10:06.188602 srai-0.7.0/srai/_typing.py
--rw-r--r--   0        0        0      155 2024-02-02 20:10:06.188602 srai-0.7.0/srai/constants.py
--rw-r--r--   0        0        0      854 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/__init__.py
--rw-r--r--   0        0        0     4846 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/_base.py
--rw-r--r--   0        0        0      531 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/_pytorch_stubs.py
--rw-r--r--   0        0        0     9181 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     8180 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      186 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/geovex/__init__.py
--rw-r--r--   0        0        0     6774 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/geovex/dataset.py
--rw-r--r--   0        0        0     9806 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/geovex/embedder.py
--rw-r--r--   0        0        0    18081 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/geovex/model.py
--rw-r--r--   0        0        0      136 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0    11335 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2278 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0    10940 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6804 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6301 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     7918 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2855 2024-02-02 20:10:06.188602 srai-0.7.0/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2024-02-02 20:10:06.188602 srai-0.7.0/srai/exceptions.py
--rw-r--r--   0        0        0     4247 2024-02-02 20:10:06.188602 srai-0.7.0/srai/geometry.py
--rw-r--r--   0        0        0     9059 2024-02-02 20:10:06.188602 srai-0.7.0/srai/h3.py
--rw-r--r--   0        0        0      531 2024-02-02 20:10:06.188602 srai-0.7.0/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2024-02-02 20:10:06.188602 srai-0.7.0/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2024-02-02 20:10:06.188602 srai-0.7.0/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      820 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/_base.py
--rw-r--r--   0        0        0     1343 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/download.py
--rw-r--r--   0        0        0     2189 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5391 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     7764 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      472 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     4359 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5315 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0    10696 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15751 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2420 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5996 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     9280 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2778 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     5033 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0      124 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7556 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    14142 2024-02-02 20:10:06.188602 srai-0.7.0/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      468 2024-02-02 20:10:06.188602 srai-0.7.0/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     6071 2024-02-02 20:10:06.188602 srai-0.7.0/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     3609 2024-02-02 20:10:06.188602 srai-0.7.0/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     4622 2024-02-02 20:10:06.188602 srai-0.7.0/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      497 2024-02-02 20:10:06.188602 srai-0.7.0/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11418 2024-02-02 20:10:06.188602 srai-0.7.0/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14129 2024-02-02 20:10:06.188602 srai-0.7.0/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0     1006 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    27497 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15629 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2477 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/geocode.py
--rw-r--r--   0        0        0     2610 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3136 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4184 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     6001 2024-02-02 20:10:06.188602 srai-0.7.0/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0       29 2024-02-02 20:10:06.188602 srai-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     7806 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/conftest.py
--rw-r--r--   0        0        0     1015 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/constants.py
--rw-r--r--   0        0        0     6245 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/generation.py
--rw-r--r--   0        0        0     4197 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/test_dataset.py
--rw-r--r--   0        0        0     4009 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/test_embedder.py
--rw-r--r--   0        0        0   484605 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_0.pt
--rw-r--r--   0        0        0   484605 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_1.pt
--rw-r--r--   0        0        0   484605 2024-02-02 20:10:06.192602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_2.pt
--rw-r--r--   0        0        0   339453 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_3.pt
--rw-r--r--   0        0        0     2139 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
--rw-r--r--   0        0        0     2139 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
--rw-r--r--   0        0        0     2139 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
--rw-r--r--   0        0        0     1755 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
--rw-r--r--   0        0        0    75958 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_features.parquet
--rw-r--r--   0        0        0   968711 2024-02-02 20:10:06.196602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_0.pt
--rw-r--r--   0        0        0   968711 2024-02-02 20:10:06.200602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_1.pt
--rw-r--r--   0        0        0   968711 2024-02-02 20:10:06.200602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_2.pt
--rw-r--r--   0        0        0   678407 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_3.pt
--rw-r--r--   0        0        0     7011 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_joint.parquet
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_0.pt
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_1.pt
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_2.pt
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_3.pt
--rw-r--r--   0        0        0    13915 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_regions.parquet
--rw-r--r--   0        0        0    24970 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/AL_10_result.parquet
--rw-r--r--   0        0        0   272893 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_batch_0.pt
--rw-r--r--   0        0        0   245693 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_batch_1.pt
--rw-r--r--   0        0        0     2139 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
--rw-r--r--   0        0        0     2011 2024-02-02 20:10:06.204602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
--rw-r--r--   0        0        0   803774 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0   545287 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_forward_0.pt
--rw-r--r--   0        0        0   490887 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_forward_1.pt
--rw-r--r--   0        0        0    76452 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_loss_0.pt
--rw-r--r--   0        0        0      762 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_loss_1.pt
--rw-r--r--   0        0        0    10162 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    21999 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     4560 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/geovex/test_model.py
--rw-r--r--   0        0        0      579 2024-02-02 20:10:06.208602 srai-0.7.0/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2782 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2711 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1056 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3058 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    26806 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0    12298 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3631 2024-02-02 20:10:06.212602 srai-0.7.0/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     2514 2024-02-02 20:10:06.212602 srai-0.7.0/tests/h3/conftest.py
--rw-r--r--   0        0        0     3035 2024-02-02 20:10:06.212602 srai-0.7.0/tests/h3/test_ij_coordinates.py
--rw-r--r--   0        0        0     3066 2024-02-02 20:10:06.212602 srai-0.7.0/tests/h3/test_shapely_conversion.py
--rw-r--r--   0        0        0     1765 2024-02-02 20:10:06.212602 srai-0.7.0/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2530 2024-02-02 20:10:06.212602 srai-0.7.0/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     2745 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4285 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     4094 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3283 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-02-02 20:10:06.212602 srai-0.7.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0   111539 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     3026 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     4763 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3157 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3104 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3803 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_1.pkl
--rw-r--r--   0        0        0     3334 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_2.pkl
--rw-r--r--   0        0        0     5099 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_3.pkl
--rw-r--r--   0        0        0     3803 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_4.pkl
--rw-r--r--   0        0        0    11090 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2182 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3177 2024-02-02 20:10:06.216602 srai-0.7.0/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4878 2024-02-02 20:10:06.216602 srai-0.7.0/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     8340 2024-02-02 20:10:06.216602 srai-0.7.0/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     9166 2024-02-02 20:10:06.216602 srai-0.7.0/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0    11409 2024-02-02 20:10:06.216602 srai-0.7.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0    11019 2024-02-02 20:10:06.216602 srai-0.7.0/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0      765 2024-02-02 20:10:06.216602 srai-0.7.0/tests/plotting/test_folium_wrapper.py
--rw-r--r--   0        0        0     3405 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6509 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2616 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1856 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2690 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     9215 2024-02-02 20:10:06.216602 srai-0.7.0/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    20346 1970-01-01 00:00:00.000000 srai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-17 19:17:06.876747 srai-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0    18089 2024-04-17 19:17:06.876747 srai-0.7.1/README.md
+-rw-r--r--   0        0        0     5213 2024-04-17 19:17:29.209238 srai-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-04-17 19:17:06.888747 srai-0.7.1/srai/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-17 19:17:06.888747 srai-0.7.1/srai/_optional.py
+-rw-r--r--   0        0        0      717 2024-04-17 19:17:06.888747 srai-0.7.1/srai/_typing.py
+-rw-r--r--   0        0        0      155 2024-04-17 19:17:06.888747 srai-0.7.1/srai/constants.py
+-rw-r--r--   0        0        0      854 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4846 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/_base.py
+-rw-r--r--   0        0        0      531 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/_pytorch_stubs.py
+-rw-r--r--   0        0        0     9181 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     8180 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      186 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/geovex/__init__.py
+-rw-r--r--   0        0        0     6774 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/dataset.py
+-rw-r--r--   0        0        0     9806 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/embedder.py
+-rw-r--r--   0        0        0    18081 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/model.py
+-rw-r--r--   0        0        0      136 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11335 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2278 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10940 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6804 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6301 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7918 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2855 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2024-04-17 19:17:06.892747 srai-0.7.1/srai/exceptions.py
+-rw-r--r--   0        0        0     4247 2024-04-17 19:17:06.892747 srai-0.7.1/srai/geometry.py
+-rw-r--r--   0        0        0     9059 2024-04-17 19:17:06.892747 srai-0.7.1/srai/h3.py
+-rw-r--r--   0        0        0      531 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      820 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/_base.py
+-rw-r--r--   0        0        0     1343 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/download.py
+-rw-r--r--   0        0        0     2189 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5391 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     7764 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      472 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     4359 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5315 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0    10696 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15751 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2420 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5996 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     9280 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2778 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     5033 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0      124 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7556 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    14142 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      468 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     6071 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     3609 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     4632 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      497 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11418 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14129 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0     1006 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    27497 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15629 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2477 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/geocode.py
+-rw-r--r--   0        0        0     2610 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3136 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4184 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     6001 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0       29 2024-04-17 19:17:06.892747 srai-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/conftest.py
+-rw-r--r--   0        0        0     1015 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/constants.py
+-rw-r--r--   0        0        0     6245 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/generation.py
+-rw-r--r--   0        0        0     4197 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/test_dataset.py
+-rw-r--r--   0        0        0     4009 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/test_embedder.py
+-rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_0.pt
+-rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_1.pt
+-rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_2.pt
+-rw-r--r--   0        0        0   339453 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_3.pt
+-rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
+-rw-r--r--   0        0        0     1755 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
+-rw-r--r--   0        0        0    75958 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_features.parquet
+-rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.900747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_0.pt
+-rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_1.pt
+-rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_2.pt
+-rw-r--r--   0        0        0   678407 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_3.pt
+-rw-r--r--   0        0        0     7011 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_1.pt
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_2.pt
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_3.pt
+-rw-r--r--   0        0        0    13915 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_regions.parquet
+-rw-r--r--   0        0        0    24970 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_result.parquet
+-rw-r--r--   0        0        0   272893 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_0.pt
+-rw-r--r--   0        0        0   245693 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2011 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
+-rw-r--r--   0        0        0   803774 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0   545287 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_0.pt
+-rw-r--r--   0        0        0   490887 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_1.pt
+-rw-r--r--   0        0        0    76452 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_1.pt
+-rw-r--r--   0        0        0    10162 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    21999 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     4560 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_model.py
+-rw-r--r--   0        0        0      579 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2782 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2711 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1056 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3058 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    26806 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0    12298 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3631 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     2514 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/conftest.py
+-rw-r--r--   0        0        0     3035 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/test_ij_coordinates.py
+-rw-r--r--   0        0        0     3066 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/test_shapely_conversion.py
+-rw-r--r--   0        0        0     1765 2024-04-17 19:17:06.916747 srai-0.7.1/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2530 2024-04-17 19:17:06.916747 srai-0.7.1/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     2745 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4285 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     4094 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3283 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0   111539 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     3026 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     4763 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3157 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3104 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3803 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_1.pkl
+-rw-r--r--   0        0        0     3334 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_2.pkl
+-rw-r--r--   0        0        0     5099 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_3.pkl
+-rw-r--r--   0        0        0     3803 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_4.pkl
+-rw-r--r--   0        0        0    11090 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2182 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3177 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4878 2024-04-17 19:17:06.920747 srai-0.7.1/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     8340 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     9166 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0    11409 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0    11019 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0      765 2024-04-17 19:17:06.920747 srai-0.7.1/tests/plotting/test_folium_wrapper.py
+-rw-r--r--   0        0        0     3405 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6509 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2616 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1856 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2690 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     9215 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    20378 1970-01-01 00:00:00.000000 srai-0.7.1/PKG-INFO
```

### Comparing `srai-0.7.0/LICENSE.md` & `srai-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/README.md` & `srai-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/pyproject.toml` & `srai-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.7.0"
+version = "0.7.1"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "Piotr Gramacki", email = "pgramacki@kraina.ai" },
     { name = "Kacper Leśniara", email = "klesniara@kraina.ai" },
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
     { name = "Szymon Woźniak", email = "swozniak@kraina.ai" },
 ]
@@ -200,15 +200,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `srai-0.7.0/srai/_optional.py` & `srai-0.7.1/srai/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/_typing.py` & `srai-0.7.1/srai/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/__init__.py` & `srai-0.7.1/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/_base.py` & `srai-0.7.1/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/_pytorch_stubs.py` & `srai-0.7.1/srai/embedders/_pytorch_stubs.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/contextual_count_embedder.py` & `srai-0.7.1/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/count_embedder.py` & `srai-0.7.1/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/geovex/dataset.py` & `srai-0.7.1/srai/embedders/geovex/dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/geovex/embedder.py` & `srai-0.7.1/srai/embedders/geovex/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/geovex/model.py` & `srai-0.7.1/srai/embedders/geovex/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/gtfs2vec/embedder.py` & `srai-0.7.1/srai/embedders/gtfs2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/gtfs2vec/model.py` & `srai-0.7.1/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/hex2vec/embedder.py` & `srai-0.7.1/srai/embedders/hex2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/hex2vec/model.py` & `srai-0.7.1/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.7.1/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/highway2vec/embedder.py` & `srai-0.7.1/srai/embedders/highway2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/embedders/highway2vec/model.py` & `srai-0.7.1/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/exceptions.py` & `srai-0.7.1/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/geometry.py` & `srai-0.7.1/srai/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/h3.py` & `srai-0.7.1/srai/h3.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/joiners/__init__.py` & `srai-0.7.1/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/joiners/_base.py` & `srai-0.7.1/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/joiners/intersection_joiner.py` & `srai-0.7.1/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/__init__.py` & `srai-0.7.1/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/_base.py` & `srai-0.7.1/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/download.py` & `srai-0.7.1/srai/loaders/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/geoparquet_loader.py` & `srai-0.7.1/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/gtfs_loader.py` & `srai-0.7.1/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/_base.py` & `srai-0.7.1/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.7.1/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.7.1/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.7.1/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.7.1/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.7.1/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.7.1/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.7.1/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.7.1/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.7.1/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_way_loader/constants.py` & `srai-0.7.1/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.7.1/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/neighbourhoods/_base.py` & `srai-0.7.1/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.7.1/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.7.1/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         Returns:
             Set[str]: Indexes of the neighbours up to the given distance.
         """
         if self._distance_incorrect(distance):
             return set()
 
-        neighbours: set[str] = h3.grid_disk(index, distance)
+        neighbours: set[str] = set(h3.grid_disk(index, distance))
         neighbours = self._handle_center(
             index, distance, neighbours, at_distance=False, include_center_override=include_center
         )
         if unchecked:
             return neighbours
         return self._select_available(neighbours)
 
@@ -104,15 +104,15 @@
 
         Returns:
             Set[str]: Indexes of the neighbours at the given distance.
         """
         if self._distance_incorrect(distance):
             return set()
 
-        neighbours: set[str] = h3.grid_ring(index, distance)
+        neighbours: set[str] = set(h3.grid_ring(index, distance))
         neighbours = self._handle_center(
             index, distance, neighbours, at_distance=True, include_center_override=include_center
         )
         return self._select_available(neighbours)
 
     def _select_available(self, indices: set[str]) -> set[str]:
         if self._available_indices is None:
```

### Comparing `srai-0.7.0/srai/plotting/folium_wrapper.py` & `srai-0.7.1/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/plotting/plotly_wrapper.py` & `srai-0.7.1/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/__init__.py` & `srai-0.7.1/srai/regionalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/_base.py` & `srai-0.7.1/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/_spherical_voronoi.py` & `srai-0.7.1/srai/regionalizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.7.1/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/geocode.py` & `srai-0.7.1/srai/regionalizers/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/h3_regionalizer.py` & `srai-0.7.1/srai/regionalizers/h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/s2_regionalizer.py` & `srai-0.7.1/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.7.1/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.7.1/srai/regionalizers/voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/conftest.py` & `srai-0.7.1/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/constants.py` & `srai-0.7.1/tests/embedders/geovex/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/generation.py` & `srai-0.7.1/tests/embedders/geovex/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_dataset.py` & `srai-0.7.1/tests/embedders/geovex/test_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_embedder.py` & `srai-0.7.1/tests/embedders/geovex/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_2.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_batch_3.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_features.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_2.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_forward_3.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_joint.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_2.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_loss_3.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_regions.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/AL_10_result.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_batch_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_batch_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_features.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_forward_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_forward_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_joint.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_loss_0.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_loss_1.pt` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_regions.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_files/wro_9_result.parquet` & `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/geovex/test_model.py` & `srai-0.7.1/tests/embedders/geovex/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/constants.py` & `srai-0.7.1/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/generation.py` & `srai-0.7.1/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_embedder.py` & `srai-0.7.1/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_model.py` & `srai-0.7.1/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.7.1/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/test_contextual_count_embedder.py` & `srai-0.7.1/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/test_count_embedder.py` & `srai-0.7.1/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.7.1/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/embedders/test_highway2vec_embedder.py` & `srai-0.7.1/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/h3/conftest.py` & `srai-0.7.1/tests/h3/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/h3/test_ij_coordinates.py` & `srai-0.7.1/tests/h3/test_ij_coordinates.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/h3/test_shapely_conversion.py` & `srai-0.7.1/tests/h3/test_shapely_conversion.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/joiners/conftest.py` & `srai-0.7.1/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/joiners/test_intersection_joiner.py` & `srai-0.7.1/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/conftest.py` & `srai-0.7.1/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/conftest.py` & `srai-0.7.1/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.7.1/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.7.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.7.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/monaco.osm.pbf` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.7.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.7.1/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.7.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_1.pkl` & `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_1.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_2.pkl` & `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_3.pkl` & `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_3.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_way_loader/test_files/graph_4.pkl` & `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_4.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.7.1/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/test_files/example.parquet` & `srai-0.7.1/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/test_geoparquet_loader.py` & `srai-0.7.1/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/loaders/test_gtfs_loader.py` & `srai-0.7.1/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.7.1/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.7.1/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.7.1/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.7.1/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.7.1/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/plotting/test_folium_wrapper.py` & `srai-0.7.1/tests/plotting/test_folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/conftest.py` & `srai-0.7.1/tests/regionalizers/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.7.1/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.7.1/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.7.1/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.7.1/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/tests/regionalizers/test_voronoi_regionalizer.py` & `srai-0.7.1/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.0/PKG-INFO` & `srai-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.7.0
+Version: 0.7.1
 Summary: A set of python modules for geospatial machine learning and data mining
-Author-Email: Piotr Gramacki <pgramacki@kraina.ai>, Kacper Leśniara <klesniara@kraina.ai>, Kamil Raczycki <kraczycki@kraina.ai>, Szymon Woźniak <swozniak@kraina.ai>
+Author-Email: Piotr Gramacki <pgramacki@kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?= <klesniara@kraina.ai>, Kamil Raczycki <kraczycki@kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?= <swozniak@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: srai Version: 0.7.0 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.7.1 Summary: A set of python
 modules for geospatial machine learning and data mining Author-Email: Piotr
 Gramacki
-kraina.ai>, Kacper LeÅniara
+kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?=
 kraina.ai>, Kamil Raczycki
-kraina.ai>, Szymon WoÅºniak
+kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?=
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

