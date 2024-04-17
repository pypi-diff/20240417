# Comparing `tmp/ficture-0.0.2.tar.gz` & `tmp/ficture-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ficture-0.0.2.tar", last modified: Thu Apr  4 13:58:05 2024, max compression
+gzip compressed data, was "ficture-0.0.3.tar", last modified: Wed Apr 17 18:52:04 2024, max compression
```

## Comparing `ficture-0.0.2.tar` & `ficture-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.804289 ficture-0.0.2/
--rw-r--r--   0 bluebear   (501) staff       (20)    19347 2024-04-04 10:02:06.000000 ficture-0.0.2/LICENSE
--rw-r--r--   0 bluebear   (501) staff       (20)       57 2024-04-04 13:57:26.000000 ficture-0.0.2/MANIFEST.in
--rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-04 13:58:05.804216 ficture-0.0.2/PKG-INFO
--rw-r--r--   0 bluebear   (501) staff       (20)     1058 2024-04-04 07:30:11.000000 ficture-0.0.2/README.md
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.787746 ficture-0.0.2/ficture/
--rw-r--r--   0 bluebear   (501) staff       (20)      263 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     1562 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/cli.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.789446 ficture-0.0.2/ficture/loaders/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10715 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/data_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4077 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_factor_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)    12685 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10013 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_to_unit_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7907 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/unit_loader.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.790153 ficture-0.0.2/ficture/models/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/lda_minibatch.py
--rw-r--r--   0 bluebear   (501) staff       (20)    28506 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/online_lda.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10460 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/online_slda.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2350 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/slda_minibatch.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.792728 ficture-0.0.2/ficture/scripts/
--rw-r--r--   0 bluebear   (501) staff       (20)      212 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     6411 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/choose_color.py
--rw-r--r--   0 bluebear   (501) staff       (20)     5394 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/de_bulk.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10343 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/factor_report.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/factor_report.template.html
--rw-r--r--   0 bluebear   (501) staff       (20)     4738 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_boundary.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7726 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_density.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10560 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_poly.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11914 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/init_model_selection.py
--rw-r--r--   0 bluebear   (501) staff       (20)    12193 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/lda_univ.py
--rw-r--r--   0 bluebear   (501) staff       (20)     9058 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/make_dge_univ.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7437 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/make_spatial_minibatch.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11623 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_base.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11866 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_hexagon.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7246 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_full.py
--rw-r--r--   0 bluebear   (501) staff       (20)     6782 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_multi.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4698 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_single.py
--rw-r--r--   0 bluebear   (501) staff       (20)     9333 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/slda_decode.py
--rw-r--r--   0 bluebear   (501) staff       (20)     8932 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/transform_univ.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.793869 ficture-0.0.2/ficture/utils/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4501 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/filter_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2123 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/hexagon_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11956 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/image_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     1447 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/layout_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     3767 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/mds_color_circle.py
--rw-r--r--   0 bluebear   (501) staff       (20)    14775 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/utilt.py
--rw-r--r--   0 bluebear   (501) staff       (20)     5885 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/visualize_factors.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.803974 ficture-0.0.2/ficture.egg-info/
--rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/PKG-INFO
--rw-r--r--   0 bluebear   (501) staff       (20)     1923 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/SOURCES.txt
--rw-r--r--   0 bluebear   (501) staff       (20)        1 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/dependency_links.txt
--rw-r--r--   0 bluebear   (501) staff       (20)       45 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/entry_points.txt
--rw-r--r--   0 bluebear   (501) staff       (20)      127 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/requires.txt
--rw-r--r--   0 bluebear   (501) staff       (20)        8 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/top_level.txt
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.803756 ficture-0.0.2/info/
--rw-r--r--   0 bluebear   (501) staff       (20)   743896 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Homo_sapiens.GRCh38.107.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   953535 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Mus_musculus.GRCm38.102.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   957882 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Mus_musculus.GRCm39.107.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   323108 2024-03-20 18:43:57.000000 ficture-0.0.2/info/gencode.human.mouse.combined.gene.types.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   356994 2024-03-20 18:43:57.000000 ficture-0.0.2/info/gencode.human.mouse.combined.gene_names.clean.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       43 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.l1.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.l2.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)     1518 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.layout.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)      320 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.tile_list.txt
--rw-r--r--   0 bluebear   (501) staff       (20)      840 2024-04-04 13:57:26.000000 ficture-0.0.2/pyproject.toml
--rw-r--r--   0 bluebear   (501) staff       (20)      268 2024-04-04 13:58:05.804528 ficture-0.0.2/setup.cfg
--rw-r--r--   0 bluebear   (501) staff       (20)       38 2024-04-04 13:57:26.000000 ficture-0.0.2/setup.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.236161 ficture-0.0.3/
+-rw-r--r--   0 bluebear   (501) staff       (20)    19347 2024-04-04 10:02:06.000000 ficture-0.0.3/LICENSE
+-rw-r--r--   0 bluebear   (501) staff       (20)       57 2024-04-04 13:57:26.000000 ficture-0.0.3/MANIFEST.in
+-rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-17 18:52:04.236099 ficture-0.0.3/PKG-INFO
+-rw-r--r--   0 bluebear   (501) staff       (20)     1058 2024-04-04 07:30:11.000000 ficture-0.0.3/README.md
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.216858 ficture-0.0.3/ficture/
+-rw-r--r--   0 bluebear   (501) staff       (20)      263 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     1604 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/cli.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.219176 ficture-0.0.3/ficture/loaders/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10715 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/data_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4077 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_factor_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    12685 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10013 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_to_unit_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7907 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/unit_loader.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.220037 ficture-0.0.3/ficture/models/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/lda_minibatch.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    28506 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/online_lda.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10460 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/online_slda.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2350 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/slda_minibatch.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.226083 ficture-0.0.3/ficture/scripts/
+-rw-r--r--   0 bluebear   (501) staff       (20)      212 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     6411 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/choose_color.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     5394 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/de_bulk.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10343 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/factor_report.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/factor_report.template.html
+-rw-r--r--   0 bluebear   (501) staff       (20)     4738 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_boundary.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7726 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_density.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10560 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_poly.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11914 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/init_model_selection.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    12193 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/lda_univ.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     9058 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/make_dge_univ.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7444 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/make_spatial_minibatch.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11623 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_base.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11866 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_hexagon.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7246 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_full.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     6782 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_multi.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4698 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_single.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    20563 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/run_together.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     9333 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/slda_decode.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     8932 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/transform_univ.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.227310 ficture-0.0.3/ficture/utils/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4501 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/filter_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2123 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/hexagon_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11956 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/image_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     1447 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/layout_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     3767 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/mds_color_circle.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2457 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/utils/minimake.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    14775 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/utilt.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     5885 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/visualize_factors.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.235852 ficture-0.0.3/ficture.egg-info/
+-rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/PKG-INFO
+-rw-r--r--   0 bluebear   (501) staff       (20)     1981 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/SOURCES.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)        1 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/dependency_links.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)       45 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/entry_points.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)      127 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/requires.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)        8 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/top_level.txt
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.235632 ficture-0.0.3/info/
+-rw-r--r--   0 bluebear   (501) staff       (20)   743896 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Homo_sapiens.GRCh38.107.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   953535 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Mus_musculus.GRCm38.102.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   957882 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Mus_musculus.GRCm39.107.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   323108 2024-03-20 18:43:57.000000 ficture-0.0.3/info/gencode.human.mouse.combined.gene.types.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   356994 2024-03-20 18:43:57.000000 ficture-0.0.3/info/gencode.human.mouse.combined.gene_names.clean.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       43 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.l1.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.l2.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)     1518 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.layout.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)      320 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.tile_list.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)      840 2024-04-17 18:51:54.000000 ficture-0.0.3/pyproject.toml
+-rw-r--r--   0 bluebear   (501) staff       (20)      268 2024-04-17 18:52:04.236400 ficture-0.0.3/setup.cfg
+-rw-r--r--   0 bluebear   (501) staff       (20)       38 2024-04-04 13:57:26.000000 ficture-0.0.3/setup.py
```

### Comparing `ficture-0.0.2/LICENSE` & `ficture-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/PKG-INFO` & `ficture-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ficture
-Version: 0.0.2
+Version: 0.0.3
 Summary: Segmentation free factor analysis for sub-micron resolution spatial transcriptomics
 Author-email: Yichen Si <ycsi@umich.edu>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://seqscope.github.io/ficture/
 Project-URL: Bug Tracker, https://github.com/seqscope/ficture/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ficture-0.0.2/README.md` & `ficture-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/cli.py` & `ficture-0.0.3/ficture/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         "slda_decode": "slda_decode", \
 
         "plot_base": "plot_base", \
         "plot_hexagon": "plot_hexagon", \
         "plot_pixel_multi": "plot_pixel_multi", \
         "plot_pixel_full": "plot_pixel_full", \
         "plot_pixel_single": "plot_pixel_single", \
+        "run_together": "run_together", \
     }
 
     if len(sys.argv) < 2:
         print("Usage: ficture <command> <args>, ficture <command> -h to see arguments for each command")
         print("Available commands:\n"+"\t".join(list(module_map.keys()) ))
         return
     elif sys.argv[1] not in module_map:
```

### Comparing `ficture-0.0.2/ficture/loaders/data_loader.py` & `ficture-0.0.3/ficture/loaders/data_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/loaders/pixel_factor_loader.py` & `ficture-0.0.3/ficture/loaders/pixel_factor_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/loaders/pixel_loader.py` & `ficture-0.0.3/ficture/loaders/pixel_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/loaders/pixel_to_unit_loader.py` & `ficture-0.0.3/ficture/loaders/pixel_to_unit_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/loaders/unit_loader.py` & `ficture-0.0.3/ficture/loaders/unit_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/models/lda_minibatch.py` & `ficture-0.0.3/ficture/models/lda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/models/online_lda.py` & `ficture-0.0.3/ficture/models/online_lda.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/models/online_slda.py` & `ficture-0.0.3/ficture/models/online_slda.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/models/slda_minibatch.py` & `ficture-0.0.3/ficture/models/slda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/choose_color.py` & `ficture-0.0.3/ficture/scripts/choose_color.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/de_bulk.py` & `ficture-0.0.3/ficture/scripts/de_bulk.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/factor_report.py` & `ficture-0.0.3/ficture/scripts/factor_report.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/factor_report.template.html` & `ficture-0.0.3/ficture/scripts/factor_report.template.html`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/filter_boundary.py` & `ficture-0.0.3/ficture/scripts/filter_boundary.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/filter_density.py` & `ficture-0.0.3/ficture/scripts/filter_density.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/filter_poly.py` & `ficture-0.0.3/ficture/scripts/filter_poly.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/init_model_selection.py` & `ficture-0.0.3/ficture/scripts/init_model_selection.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/lda_univ.py` & `ficture-0.0.3/ficture/scripts/lda_univ.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/make_dge_univ.py` & `ficture-0.0.3/ficture/scripts/make_dge_univ.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/make_spatial_minibatch.py` & `ficture-0.0.3/ficture/scripts/make_spatial_minibatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             l = v.split(':')[0]
             st, ed = v.split(':')[1].split('-')
             st = str(int(float(st) * args.mu_scale) )
             ed = str(int(float(ed) * args.mu_scale) )
             reg_list.append(l+':'+'-'.join([st,ed]) )
         cmd = ["tabix", args.input] + reg_list
     if len(cmd) == 0:
-        p0 = sp.Popen(["zcat", args.input], stdout=sp.PIPE)
+        p0 = sp.Popen(["gzip", "-cd", args.input], stdout=sp.PIPE)
         process = sp.Popen(["tail", "-n", "+2"], stdin=p0.stdout, stdout=sp.PIPE)
     else:
         process = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.STDOUT)
 
     ### Group pixels into minibatches
     output_header = copy.copy(input_header)
     output_header.insert(1, "random_index")
```

### Comparing `ficture-0.0.2/ficture/scripts/plot_base.py` & `ficture-0.0.3/ficture/scripts/plot_base.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/plot_hexagon.py` & `ficture-0.0.3/ficture/scripts/plot_hexagon.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/plot_pixel_full.py` & `ficture-0.0.3/ficture/scripts/plot_pixel_full.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/plot_pixel_multi.py` & `ficture-0.0.3/ficture/scripts/plot_pixel_multi.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/plot_pixel_single.py` & `ficture-0.0.3/ficture/scripts/plot_pixel_single.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/slda_decode.py` & `ficture-0.0.3/ficture/scripts/slda_decode.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/scripts/transform_univ.py` & `ficture-0.0.3/ficture/scripts/transform_univ.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,9 +173,9 @@
 
     out_f = args.output + ".posterior.count.tsv.gz"
     pd.concat([pd.DataFrame({'gene': feature_kept}),\
             pd.DataFrame(post_count.T, dtype='float64',\
                             columns = factor_header)],\
                 axis = 1).to_csv(out_f, sep='\t', index=False, float_format='%.2f', compression={"method":"gzip"})
 
-if __name__ is '__main__':
+if __name__ == '__main__':
     transform(sys.argv[1:])
```

### Comparing `ficture-0.0.2/ficture/utils/filter_fn.py` & `ficture-0.0.3/ficture/utils/filter_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/hexagon_fn.py` & `ficture-0.0.3/ficture/utils/hexagon_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/image_fn.py` & `ficture-0.0.3/ficture/utils/image_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/layout_fn.py` & `ficture-0.0.3/ficture/utils/layout_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/mds_color_circle.py` & `ficture-0.0.3/ficture/utils/mds_color_circle.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/utilt.py` & `ficture-0.0.3/ficture/utils/utilt.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture/utils/visualize_factors.py` & `ficture-0.0.3/ficture/utils/visualize_factors.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/ficture.egg-info/PKG-INFO` & `ficture-0.0.3/ficture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ficture
-Version: 0.0.2
+Version: 0.0.3
 Summary: Segmentation free factor analysis for sub-micron resolution spatial transcriptomics
 Author-email: Yichen Si <ycsi@umich.edu>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://seqscope.github.io/ficture/
 Project-URL: Bug Tracker, https://github.com/seqscope/ficture/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ficture-0.0.2/ficture.egg-info/SOURCES.txt` & `ficture-0.0.3/ficture.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,22 +36,24 @@
 ficture/scripts/make_dge_univ.py
 ficture/scripts/make_spatial_minibatch.py
 ficture/scripts/plot_base.py
 ficture/scripts/plot_hexagon.py
 ficture/scripts/plot_pixel_full.py
 ficture/scripts/plot_pixel_multi.py
 ficture/scripts/plot_pixel_single.py
+ficture/scripts/run_together.py
 ficture/scripts/slda_decode.py
 ficture/scripts/transform_univ.py
 ficture/utils/__init__.py
 ficture/utils/filter_fn.py
 ficture/utils/hexagon_fn.py
 ficture/utils/image_fn.py
 ficture/utils/layout_fn.py
 ficture/utils/mds_color_circle.py
+ficture/utils/minimake.py
 ficture/utils/utilt.py
 ficture/utils/visualize_factors.py
 info/Homo_sapiens.GRCh38.107.names.tsv.gz
 info/Mus_musculus.GRCm38.102.names.tsv.gz
 info/Mus_musculus.GRCm39.107.names.tsv.gz
 info/gencode.human.mouse.combined.gene.types.tsv.gz
 info/gencode.human.mouse.combined.gene_names.clean.tsv
```

### Comparing `ficture-0.0.2/info/Homo_sapiens.GRCh38.107.names.tsv.gz` & `ficture-0.0.3/info/Homo_sapiens.GRCh38.107.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/info/Mus_musculus.GRCm38.102.names.tsv.gz` & `ficture-0.0.3/info/Mus_musculus.GRCm38.102.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/info/Mus_musculus.GRCm39.107.names.tsv.gz` & `ficture-0.0.3/info/Mus_musculus.GRCm39.107.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/info/gencode.human.mouse.combined.gene.types.tsv.gz` & `ficture-0.0.3/info/gencode.human.mouse.combined.gene.types.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/info/gencode.human.mouse.combined.gene_names.clean.tsv` & `ficture-0.0.3/info/gencode.human.mouse.combined.gene_names.clean.tsv`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/info/hiseq.layout.tsv` & `ficture-0.0.3/info/hiseq.layout.tsv`

 * *Files identical despite different names*

### Comparing `ficture-0.0.2/pyproject.toml` & `ficture-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "ficture"
 description = "Segmentation free factor analysis for sub-micron resolution spatial transcriptomics"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{name = "Yichen Si", email = "ycsi@umich.edu"}]
 license = {text = "CC BY-NC 4.0"}
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "numpy", "pandas",
     "scipy", "scikit-learn",
```

