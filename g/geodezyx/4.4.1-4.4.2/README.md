# Comparing `tmp/geodezyx-4.4.1.tar.gz` & `tmp/geodezyx-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodezyx-4.4.1.tar", last modified: Thu Feb  8 14:17:51 2024, max compression
+gzip compressed data, was "geodezyx-4.4.2.tar", last modified: Wed Apr 17 15:45:23 2024, max compression
```

## Comparing `geodezyx-4.4.1.tar` & `geodezyx-4.4.2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.587553 geodezyx-4.4.1/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7652 2024-02-08 10:49:07.000000 geodezyx-4.4.1/LICENSE
--rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2203 2024-02-08 14:17:51.587553 geodezyx-4.4.1/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6140 2024-02-08 14:07:58.000000 geodezyx-4.4.1/README.md
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.567553 geodezyx-4.4.1/geodezyx/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2264 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.567553 geodezyx-4.4.1/geodezyx/athmo/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/athmo/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30501 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/athmo/athmo.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.567553 geodezyx-4.4.1/geodezyx/conv/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9545 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_angle.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23341 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_coords.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9536 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_geometric.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_interpolators.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3876 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_proj_lambert.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6572 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_proj_utm.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10474 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12023 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_rotation_matrices.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79783 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/conv/conv_time.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.567553 geodezyx-4.4.1/geodezyx/externlib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1339 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/externlib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      797 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/externlib/externlib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.575553 geodezyx-4.4.1/geodezyx/files_rw/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      595 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80888 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_athmo.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_coords_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    77981 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_coords_time_series.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_eop.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28653 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_geo_files_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    16649 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_gnss_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7241 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_gnss_qc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_igs_combi.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18109 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_logsheets.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14652 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/read_slr.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37758 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/write_geo_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6422 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/files_rw/write_rinex.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.575553 geodezyx-4.4.1/geodezyx/geodyn/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      136 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/geodyn/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10131 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/geodyn/emsgfz_load_interp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13584 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/geodyn/euler_pole_calc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27563 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/geodyn/velo_field_map_plt.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6087 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/geodyn/volcano_mogi.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.575553 geodezyx-4.4.1/geodezyx/logconfig/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/logconfig/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2214 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/logconfig/loggzyx.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.575553 geodezyx-4.4.1/geodezyx/marine/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      119 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/marine/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2575 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/marine/marine.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9675 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/marine/obp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28897 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/marine/obscom.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.579553 geodezyx-4.4.1/geodezyx/megalib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/genefun.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/geoclass.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/geodetik.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/megalib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/megalib/softs_runner.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.583553 geodezyx-4.4.1/geodezyx/operational/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      635 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10813 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/anubis_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7433 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/cluster_gfz.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7006 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_cddis.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7150 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_dropbox.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14142 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_find_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    33770 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17715 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11236 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/download_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79416 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/gins_runner.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26851 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/groops_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15751 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/hector_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7915 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/midas_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26025 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/rinex_lister_plotter.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32108 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/rinex_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7060 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/rtklib_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9145 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/operational/track_frontend.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.583553 geodezyx-4.4.1/geodezyx/reffram/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/reffram/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43617 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/reffram/geometry.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    56872 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/reffram/gnss_products.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7228 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/reffram/kepler_gzyx.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3864 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/reffram/quaternions.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.583553 geodezyx-4.4.1/geodezyx/stats/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/stats/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30945 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/stats/least_squares.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    44079 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/stats/stats.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.583553 geodezyx-4.4.1/geodezyx/time_series/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/time_series/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48502 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/time_series/ts_class.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/time_series/ts_export.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    38658 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/time_series/ts_fcts.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.583553 geodezyx-4.4.1/geodezyx/toolbox_meta/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/toolbox_meta/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.587553 geodezyx-4.4.1/geodezyx/utils/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2011 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/dict_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13503 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/list_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3622 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/pandas_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7245 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/plot_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18293 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/shell_like.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    25707 2024-02-08 10:49:07.000000 geodezyx-4.4.1/geodezyx/utils/utils_core.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.567553 geodezyx-4.4.1/geodezyx.egg-info/
--rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2203 2024-02-08 14:17:51.000000 geodezyx-4.4.1/geodezyx.egg-info/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3056 2024-02-08 14:17:51.000000 geodezyx-4.4.1/geodezyx.egg-info/SOURCES.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2024-02-08 14:17:51.000000 geodezyx-4.4.1/geodezyx.egg-info/dependency_links.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      215 2024-02-08 14:17:51.000000 geodezyx-4.4.1/geodezyx.egg-info/requires.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2024-02-08 14:17:51.000000 geodezyx-4.4.1/geodezyx.egg-info/top_level.txt
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-02-08 14:17:51.587553 geodezyx-4.4.1/misc/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2024-02-08 10:49:07.000000 geodezyx-4.4.1/misc/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2024-02-08 10:49:07.000000 geodezyx-4.4.1/misc/import_generic.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2024-02-08 10:49:07.000000 geodezyx-4.4.1/misc/refactoring.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2024-02-08 14:17:51.587553 geodezyx-4.4.1/setup.cfg
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10336 2024-02-08 14:17:28.000000 geodezyx-4.4.1/setup.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.930724 geodezyx-4.4.2/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7652 2024-02-08 10:49:07.000000 geodezyx-4.4.2/LICENSE
+-rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-04-17 15:45:23.930724 geodezyx-4.4.2/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6655 2024-04-17 15:03:14.000000 geodezyx-4.4.2/README.md
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.906724 geodezyx-4.4.2/geodezyx/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2350 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.906724 geodezyx-4.4.2/geodezyx/athmo/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/athmo/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30501 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/athmo/athmo.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.910724 geodezyx-4.4.2/geodezyx/conv/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9545 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_angle.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23341 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_coords.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9504 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/conv/conv_geometric.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_interpolators.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3876 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_proj_lambert.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6572 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_proj_utm.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10474 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12023 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_rotation_matrices.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80367 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/conv/conv_time.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.910724 geodezyx-4.4.2/geodezyx/externlib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1339 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/externlib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      797 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/externlib/externlib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/files_rw/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      595 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    81708 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_athmo.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_coords_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79500 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/read_coords_time_series.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_eop.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28653 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_geo_files_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17067 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/read_gnss_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7241 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_gnss_qc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_igs_combi.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18109 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_logsheets.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14652 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_slr.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37758 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/files_rw/write_geo_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6422 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/write_rinex.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/geodyn/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      136 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10131 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/emsgfz_load_interp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13584 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/euler_pole_calc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27563 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/velo_field_map_plt.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6087 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/volcano_mogi.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/logconfig/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/logconfig/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2329 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/logconfig/loggzyx.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/marine/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      119 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2575 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/marine.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9675 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/obp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30838 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/marine/obscom.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.918724 geodezyx-4.4.2/geodezyx/megalib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/genefun.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geoclass.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geodetik.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/megalib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/softs_runner.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/operational/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      672 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10790 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/anubis_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7433 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/cluster_gfz.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7006 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/download_cddis.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7150 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/download_dropbox.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14599 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_find_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    34383 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/operational/download_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    20363 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13921 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79416 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/gins_runner.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26851 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/groops_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15751 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/hector_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7915 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/midas_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14061 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/pride_pppar_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26025 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/rinex_lister_plotter.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32108 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/rinex_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7041 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/rtklib_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9145 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/track_frontend.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/reffram/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/reffram/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43896 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/geometry.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    63732 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/gnss_products.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11346 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/kepler_gzyx.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3864 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/reffram/quaternions.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/stats/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30945 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/least_squares.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    44079 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/stats.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/time_series/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/time_series/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48885 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/time_series/ts_class.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/time_series/ts_export.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    39108 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/time_series/ts_fcts.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/toolbox_meta/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/toolbox_meta/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/utils/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2011 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/dict_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13503 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/list_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3622 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/pandas_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7245 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/plot_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18458 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/utils/shell_like.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    25869 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/utils/utils_core.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx.egg-info/
+-rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3101 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      215 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/requires.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/top_level.txt
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/misc/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/import_generic.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/refactoring.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2024-04-17 15:45:23.930724 geodezyx-4.4.2/setup.cfg
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10322 2024-04-17 14:44:56.000000 geodezyx-4.4.2/setup.py
```

### Comparing `geodezyx-4.4.1/LICENSE` & `geodezyx-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/PKG-INFO` & `geodezyx-4.4.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 4.4.1
-Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
-Home-page: https://github.com/IPGP/geodezyx-toolbox
+Version: 4.4.2
+Summary: geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.
+Home-page: https://github.com/IPGP/geodezyx
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -42,23 +42,23 @@
 Requires-Dist: wheel
 Requires-Dist: xarray
 Provides-Extra: full
 Requires-Dist: netCDF4; extra == "full"
 Requires-Dist: kepler.py; extra == "full"
 Requires-Dist: ncompress; extra == "full"
 
-The purpose of this GeodeZYX toolbox is to provide all the functions which
+geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide all the functions which
 can be useful for Geodesy and Geophysics. 
 
 It includes low level functions, file management functions,
 time and space-coordinates conversion functions, 
 data (especially GNSS observations and orbits) retrieve functions, 
 plots and visual selection functions ...
 
 It is designed for Python 3 on a LINUX Ubuntu-like system.
 Also tested with Anaconda
 
-Documentation: https://geodezyx.github.io/geodezyx-toolbox  
+Documentation: https://ipgp.github.io/geodezyx  
 
-GitHub repository: https://github.com/IPGP/geodezyx-toolbox 
+GitHub repository: https://github.com/IPGP/geodezyx 
 
 PyPi project: https://pypi.org/project/geodezyx
```

### Comparing `geodezyx-4.4.1/README.md` & `geodezyx-4.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <img src="./geodezyx_toolbox_logo.png" width="300">
 
-# GeodeZYX Toolbox
+# geodezyx (aka ___The GeodeZYX Toolbox___) 
 
-**Version 4.4.1 / 2023-02-08**, README Revision: 2024-02-08
+**Version 4.4.2 / 2024-04-17**, README Revision: 2024-04-17
 
 
 **Authors:** Pierre Sakic (IPGP, Paris, France) & Gustavo Mansur (GFZ, Potsdam, Germany)
 
-**Documentation:** [https://ipgp.github.io/geodezyx-toolbox](https://ipgp.github.io/geodezyx-toolbox/)
+**Documentation:** [https://ipgp.github.io/geodezyx](https://ipgp.github.io/geodezyx/)
 
-**GitHub repository:** [https://github.com/IPGP/geodezyx-toolbox](https://github.com/IPGP/geodezyx-toolbox) 
+**GitHub repository:** [https://github.com/IPGP/geodezyx](https://github.com/IPGP/geodezyx) 
 
 **PyPi project:** [https://pypi.org/project/geodezyx](https://pypi.org/project/geodezyx/)
 
 **Contact e-mail:** sakic@ipgp.fr
 
 **Citation:** Sakic, Pierre; Mansur, Gustavo; Chaiyaporn, Kitpracha; Ballu, Valérie (2019):
 *The geodeZYX toolbox: a versatile Python 3 toolbox for geodetic-oriented purposes*. 
@@ -22,67 +22,79 @@
 **Licence:** GNU LGPL v3 (see below) 
 
 **Contributors:**
 * Kitpracha "Na" Chaiyaporn (GFZ, Potsdam, Germany)
 * Valérie Ballu (CNRS/La Rochelle University, France)
 
 
+
 ## Introduction
 
-The purpose of the GeodeZYX toolbox (pronounced *geode-**zeecks***) is to provide all the functions which
+The purpose of _geodezyx_ (pronounced *geode-**zeecks***), also known as _the GeodeZYX toolbox_, is to provide all the functions which
 can be useful for Geodesy and Geophysics. 
 
 It includes low-level functions, file management functions,
 time and space-coordinates conversion functions, 
 data (especially GNSS observations and orbits) retrieve functions, 
 plots and visual selection functions ...
 
 It is designed for Python 3 on a LINUX Ubuntu-like system.
 Also tested with Anaconda
 
 ## Documentation
 
 See the following link:
-[https://geodezyx.github.io/geodezyx-toolbox/](https://geodezyx.github.io/geodezyx-toolbox/)
+[https://ipgp.github.io/geodezyx/](https://ipgp.github.io/geodezyx/)
 
 ## Installation 
 
 See the following link:
-[https://geodezyx.github.io/geodezyx-toolbox/getting_started.html#installation](https://geodezyx.github.io/geodezyx-toolbox/getting_started.html#installation)
+[https://ipgp.github.io/geodezyx/getting_started.html#installation](https://ipgp.github.io/geodezyx/getting_started.html#installation)
 
 ## Installation (detailed legacy instructions)
 
 ### with PyPI and pip
 
 We recommend using `pip` to do a proper installation.  
 To get the latest working version, you can install directly the GitHub-hosted version (recommended):  
 
-``pip install git+https://github.com/IPGP/geodezyx-toolbox``
+``pip install git+https://github.com/IPGP/geodezyx``
 
 You can also install the version hosted on PyPI (but you will not get the latest changes)
 
 ``pip install geodezyx``
 
 ### clone and manually install from GitHub
 
 You can manually fork and clone the GitHub repository
-[https://github.com/GeodeZYX/geodezyx-toolbox/](https://github.com/GeodeZYX/geodezyx-toolbox/)
+[https://github.com/IPGP/geodezyx/](https://github.com/IPGP/geodezyx/)
 
 and install the Toolbox you downloaded with ``python setup.py install``
 
 Alternatively, you can also add the ``geodezyx`` folder in your ``PYTHONPATH`` (for experimented users)
 
 ## Changelog
 
-### v4.4.1, 2023-02-08
+
+### v4.4.2, 2024-04-17
+  * The GitHub repository, and the project in general, has been renamed as ``geodezyx`` (in lower case)
+    to uniformize its multiple spellings and then avoid confusion.
+    * It must be transparent for your clones but updating them is recommended \
+      https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository
+  * misc routine improvements
+  * Refactoring of the GNSS data/products dowmload functions
+      
+### v4.4.1, 2024-02-08
   * The GitHub repository has now been moved under the IPGP organization.
     * It must be transparent for your clones but updating them is recommended \
       https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository  
-  * The numbering goes without a starting zero anymore. The GeodeZYX toolbox is a grown-up project now!
-  * Bugs corrected for `read_rnx2_obs` and `OrbDF` manipulation function.
+  * The version numbering goes without a starting zero from now on.  
+    Initially, this first zero was kept as a "perpetual beta" marker,  
+    but The GeodeZYX toolbox is a grown-up project now!
+  * Bugs corrected for `read_rnx2_obs` and `OrbDF` manipulation functions.
 
 ### v0.4.4.0, 2023-11-24
   * The toolbox turns to the _GNU Lesser General Public License version 3_
   * Module docstring has been updated
   * Angle conversion functions have been refactored
   * sp3/clk DataFrame column names are renamed to better fit the data content:
     * `sat` > `prn`, `const` > `sys`, `sv` > `prni`, `AC` > `ac`
```

### Comparing `geodezyx-4.4.1/geodezyx/__init__.py` & `geodezyx-4.4.2/geodezyx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # import datetime as dt
 # import fnmatch
 # from ftplib import FTP
 # import glob
 # import inspect
 # import itertools
 # import linecache
-import logging
-import logging.config
+#import logging
+import logging.config # MUST remain logging.config for < v3.10 
+# (import logging alone doesn't work for < 3.10)
 # import math
 # import matplotlib
 #matplotlib.use("agg") ### avoid tk import error
 # import matplotlib.pyplot as plt
 # import multiprocessing as mp
 ## from natsort import natsorted, ns
 # import numpy as np
@@ -82,22 +83,16 @@
            'marine',
            'operational',
            'reffram',
            'stats',
            'time_series',
            'utils']
 
-
-
-
 #### Import extern libraires in in the geodezyx namespace
 #from geodezyx.extern import *
 
 # NB : if you want extern in the main namespace 
 #      don't call with 
 #      import geodezyx
 #      but with
 #      from geodezyx import *
 
-
-
-
```

### Comparing `geodezyx-4.4.1/geodezyx/athmo/athmo.py` & `geodezyx-4.4.2/geodezyx/athmo/athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_angle.py` & `geodezyx-4.4.2/geodezyx/conv/conv_angle.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_coords.py` & `geodezyx-4.4.2/geodezyx/conv/conv_coords.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_geometric.py` & `geodezyx-4.4.2/geodezyx/conv/conv_geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import scipy
-from pyorbital import astronomy
 import re
 
 #### geodeZYX modules
 from geodezyx import utils
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
```

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_interpolators.py` & `geodezyx-4.4.2/geodezyx/conv/conv_interpolators.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_proj_lambert.py` & `geodezyx-4.4.2/geodezyx/conv/conv_proj_lambert.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_proj_utm.py` & `geodezyx-4.4.2/geodezyx/conv/conv_proj_utm.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_rinex.py` & `geodezyx-4.4.2/geodezyx/conv/conv_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_rotation_matrices.py` & `geodezyx-4.4.2/geodezyx/conv/conv_rotation_matrices.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/conv/conv_time.py` & `geodezyx-4.4.2/geodezyx/conv/conv_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,23 +443,35 @@
     -------
     L : datetime or list/numpy.array of datetime.
         Datetime(s)
     """
     if not utils.is_iterable(year):
         # All this because Python cant handle int with a starting with 0 (like 08)
         # => SyntaxError: invalid token
-        year    = int(str(year))
-        days    = int(str(days))
-        hours   = float(str(hours))
-        minutes = float(str(minutes))
-        seconds = float(str(seconds))
+        
+        if np.any(np.isnan([year,days,hours,minutes,seconds])):
+            log.error('one input is NaN, abort: %s,%s,%s,%s,%s',
+                      year,days,hours,minutes,seconds)
+            raise Exception
+            
+        
+        try:
+            year    = int(float(str(year)))
+            days    = int(float(str(days)))
+            hours   = int(float(str(hours)))
+            minutes = int(float(str(minutes)))
+            seconds = int(float(str(seconds)))
+        except Exception as e:
+            log.error('error with conversion of %s,%s,%s,%s,%s',
+                      year,days,hours,minutes,seconds)
+            raise e
 
         tempsecs = seconds + 60 * minutes + 3600 * hours
         #finalsecs     = np.floor(tempsecs)
-        finalmicrosec = np.round(tempsecs * 10**6)
+        finalmicrosec = int(np.round(tempsecs * 10**6))
 
         return dt.datetime(year, 1, 1) + dt.timedelta(days - 1) + \
         dt.timedelta(microseconds=finalmicrosec)
 
     else:
         if not utils.is_iterable(hours):
             hours   = [0] * len(year)
@@ -1969,14 +1981,44 @@
                                epoch_flag,
                                nsats,
                                rec_clk_offset)
     
         return epoch_out
 
 
+def utc2gpstime(year,month,day,hour,min,sec):
+    """
+    Convert UTC Time to GPS Time
+
+    Parameters
+    ----------
+    year,month,day,hour,min,sec : int
+        input UTC time.
+
+    Returns
+    -------
+    gpsweek,gpssecs
+        Converted epoch in GPS time, i.e. GPS Week and GPS seconds in week.
+
+    """
+    
+    date_utc = dt.datetime(year,month,day,hour,min,sec)
+    
+    utc_offset = find_leapsecond(date_utc)
+    
+    start_gps_time   = dt.datetime(1980,1,6)
+    date_diff  = date_utc - start_gps_time + dt.timedelta(seconds=utc_offset) - dt.timedelta(seconds=19)
+    
+    gpsweek_decimal = date_diff.days / 7.
+    gpsweek = np.floor(gpsweek_decimal)
+    gpsweek_decimal_part = np.modf(gpsweek_decimal)[0]
+    gpssecs = np.round(86400 * 7 * gpsweek_decimal_part) + date_diff.seconds
+    
+    return int(gpsweek),int(gpssecs)
+
 #### LEAP SECONDS MANAGEMENT
     
 def leap_seconds(f):
     """
     Return a list of tuples of this format: (timestamp, number_of_seconds)
         timestamp: a 32-bit timestamp, seconds since the UNIX epoch
         number_of_seconds: how many leap-seconds occur at timestamp
@@ -2030,18 +2072,18 @@
     return outlist
 
 def get_leapsecond_frontend():
     """
     INTERNAL_FUNCTION
 
     Nota :
-        Le temps universel (UT1) et le Temps atomique international (TAI) ont
-        été définis comme égaux en 1958. Lors de la mise en place d’UTC en
-        1972, UT1 s’était décalé d’environ 10 secondes par rapport au TAI.
-        On choisit donc un décalage initial de 10 secondes entre UTC et TAI .
+    Universal Time (UT1) and International Atomic Time (TAI) were defined as equal 
+    in 1958. When UTC was introduced in 1972, UT1 had shifted by around 10 seconds
+    in relation to TAI. 
+    We therefore chose an initial offset of 10 seconds between UTC and TAI.
 
         the initial 10sec are added in find_leapsecond
     """
     zoneinfo_fname = '/usr/share/zoneinfo/right/UTC'
 
     try:
         ### Linux case : AUTO Mode
@@ -2099,19 +2141,18 @@
     Returns
     -------
     leapsec_out : int
         The leap second for the given epoch
         
     Note
     ----
-    Le temps universel (UT1) et le Temps atomique international (TAI) ont
-    été définis comme égaux en 1958. Lors de la mise en place d’UTC en
-    1972, UT1 s’était décalé d’environ 10 secondes par rapport au TAI.
-    On choisit donc un décalage initial de 10 secondes entre UTC et TAI .
-    
+    Universal Time (UT1) and International Atomic Time (TAI) were defined as equal 
+    in 1958. When UTC was introduced in 1972, UT1 had shifted by around 10 seconds
+    in relation to TAI. 
+    We therefore chose an initial offset of 10 seconds between UTC and TAI.
     
     In 1972, the leap-second system was introduced so that the broadcast UTC 
     seconds could be made exactly equal to the standard SI second, while still
     maintaining the UTC time of day and changes of UTC date synchronized with 
     those of UT1 (the solar time standard that superseded GMT).[11] By then, 
     the UTC clock was already 10 seconds behind TAI, which had been 
     synchronized with UT1 in 1958, but had been counting true SI seconds
@@ -2609,34 +2650,14 @@
     Wrapper of dt_round for legacy reasons
     
     **This function is depreciated !!!**
     **Use round_dt instead         !!!**
     """
     return dt_round(*args)
 
-    
-def utc2gpstime(year,month,day,hour,min,sec):
-    """
-    looks useless and discontinued
-    (210219)
-    """
-    
-    date_utc = dt.datetime(year,month,day,hour,min,sec)
-    
-    utc_offset = find_leapsecond(date_utc)
-    
-    start_gps_time   = dt.datetime(1980,1,6)
-    date_diff  = date_utc - start_gps_time + dt.timedelta(seconds=utc_offset) - dt.timedelta(seconds=19)
-    
-    gpsweek_decimal = date_diff.days / 7.
-    gpsweek = np.floor(gpsweek_decimal)
-    gpsweek_decimal_part = np.modf(gpsweek_decimal)[0]
-    gpssecs = np.round(86400 * 7 * gpsweek_decimal_part) + date_diff.seconds
-    
-    return int(gpsweek),int(gpssecs)
 
 
 def utc2gpstime_bad(year,month,day,hour,min,sec):
     from numpy import mod,array,floor
     """
     [gpsweek,gpssecs] = utc2gpstime(year,month,day,hour,min,sec)
     Converts UTC time to GPS week and seconds, Python version, Nov 2008
```

### Comparing `geodezyx-4.4.1/geodezyx/externlib/__init__.py` & `geodezyx-4.4.2/geodezyx/externlib/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/externlib/externlib.py` & `geodezyx-4.4.2/geodezyx/externlib/externlib.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/__init__.py` & `geodezyx-4.4.2/geodezyx/files_rw/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/geo_files_converter_lib.py` & `geodezyx-4.4.2/geodezyx/files_rw/geo_files_converter_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2021,59 +2021,86 @@
         h5fn = fn.with_suffix('.h5')
         print(('saving NAV data to {}'.format(h5fn)))
         nav.to_hdf(h5fn,key='NAV',mode='a',complevel=6,append=False)
 
     return nav
 
 
-def unzip_gz_Z(inp_gzip_file,out_gzip_file='',remove_inp=False, force = False):
+def unzip_gz_Z(inp_gzip_file,out_gzip_file='',remove_inp=False, 
+               force = False, out_gzip_dir = None):
     """
-    if out_gzip_file if not precised, file will be extracted in the same folder
-    as inp_gzip_file
+    frontend function to unzip files (gzip and legacy Z compression) 
+
+    Parameters
+    ----------
+    inp_gzip_file : str
+        the path of the input file.
+    out_gzip_file : str, optional
+        if out_gzip_file AND out_gzip_dir not precised
+        file will be extracted in the same folder
+        as inp_gzip_file. The default is ''.
+    remove_inp : bool, optional
+        remove the input file. The default is False.
+    force : bool, optional
+        force the decompression. The default is False.
+    out_gzip_dir : str, optional
+        output directory. will be used only if out_gzip_file == ''
+        unzipped file will keep the same 
+        
+
+    Returns
+    -------
+    out_gzip_file : 
+        path of the uncompressed file.
+
+    Warning
+    -------
 
     .Z decompression is implemented, but is very unstable (avoid .Z, prefer .gz)
     """
 
     import gzip
 
     if inp_gzip_file.endswith('.gz'):
         is_gz = True
     elif inp_gzip_file.endswith('.Z'):
         is_gz = False
     else:
         is_gz = True
 
     if out_gzip_file == '':
-        out_gzip_file = os.path.join(os.path.dirname(inp_gzip_file) ,
+        if not out_gzip_dir:
+            out_gzip_dir_use = os.path.dirname(inp_gzip_file)
+        else:
+            out_gzip_dir_use = out_gzip_dir
+        
+        if not os.path.isdir(out_gzip_dir_use):
+            log.error("%s does not exists, unzipping is cancelled",
+                      out_gzip_dir_use)
+            raise Exception
+            
+        out_gzip_file = os.path.join( out_gzip_dir_use ,
                                      '.'.join(os.path.basename(inp_gzip_file).split('.')[:-1]))
 
-
     if os.path.isfile(out_gzip_file) and not force:
-        print('INFO : ' , out_gzip_file , 'already exists, skiping (use force option)')
+        log.info('%s already exists, skiping (use force option)',out_gzip_file)
         pass
     else:
         if is_gz:
             with gzip.open(inp_gzip_file, 'rb') as f_in, open(out_gzip_file, 'wb') as f_out:
                 shutil.copyfileobj(f_in, f_out)
         else:
-            print("WARN : zlib decompress is unstable !! and .Z should be definitly avoided ... ")
-            #str_object1 = open(inp_gzip_file, 'rb').read()
-            #str_object2 = zlib.decompress(str_object1)
-            #f = open(out_gzip_file, 'wb')
-            #f.write(str_object2)
-            #f.close()
-
+            log.warning("zlib decompress is unstable!! and .Z should be definitly avoided...")
             out_gzip_file = utils.uncompress(inp_gzip_file)
 
-        print('INFO : uncompressing ' + inp_gzip_file + " to " + out_gzip_file )
-
+        log.info('uncompress %s to  %s',inp_gzip_file, out_gzip_file)
 
     ### Removing part
-    if remove_inp and os.path.getsize(out_gzip_file) > 0:
-        print("INFO : removing " + inp_gzip_file)
+    if remove_inp and type(remove_inp) is bool and os.path.getsize(out_gzip_file) > 0:
+        log.info("removing %s")
         os.remove(inp_gzip_file)
 
     return out_gzip_file
 
 
  #  ______                _   _                _____                                         _ 
  # |  ____|              | | (_)              / ____|                                       | |
```

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_athmo.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_athmo.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_coords_misc.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_coords_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_coords_time_series.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_coords_time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -822,15 +822,15 @@
             else:
                 namestat = f[-1]
 
 
         if l[0] == '#':
             continue
 
-        Traw = float(f[2])
+        #Traw = float(f[2])
 
         if 'XYZ_SOL' in l:
             coordstype = 'XYZ'
             X =  float(f[4])
             Y =  float(f[6])
             Z =  float(f[8])
 
@@ -1389,15 +1389,15 @@
         tsoutlis = []
         for filein in filelistin:
             log.info(filein)
             if not utils.check_regex(filein,'c o n v e r g e n c e'):
                 continue
             ts = read_gins(filein,kineorstatic='kine',flh_in_rad=flh_in_rad)
             tsoutlis.append(ts)
-        tsout = merge_ts(tsoutlis)
+        tsout = time_series.merge_ts(tsoutlis)
 
     else:
         log.error("check kineorstatic keyword")
 
     tsout.sort()
     return tsout
 
@@ -2319,15 +2319,15 @@
     tsout = time_series.TimeSeriePoint()
     for i in range(len(T)):
         point = time_series.Point(X[i],Y[i],Z[i],T[i],initype,sA=np.nan,sB=np.nan,sC=np.nan)
         tsout.add_point(point)
     tsout.meta_set(filein)
     return tsout
 
-def read_sonardyne_posi(filein):
+def read_sonardyne_posi(filein,dUTCGPS):
     reader = pd.read_csv(open(filein),skip_footer=1)
     T = [ dateutil.parser.parse(e) + dt.timedelta(seconds=dUTCGPS) for e in list(reader['UTCTime'])]
     (L,F,H) = (reader['Longitude'],reader['Latitude'],reader['Altitude'])
     sX,sY,sZ = [] , [] , []
     initype = 'FLH'
     tsout = time_series.TimeSeriePoint()
     for i in range(len(T)):
@@ -2495,45 +2495,99 @@
             tsout.add_point(point)
     
     tsout.meta_set(stat=statname)
     tsout.sort()
 
     return tsout    
 
-def read_pridear(filein):
-    F = open(filein)
-    
-    L = F.readlines()
-    
-    stat = "XXXX"
+
+
+def _pride_pppar_end_header(filein):
     colheader=0
+    stat = "XXXX"
+
+    with open(filein) as F:
+        L = F.readlines()
     
     for i,l in enumerate(L):
         if "STATION" in l:
             stat = l.split()[0]
 
         if "END OF HEADER" in l:
             colheader = i+1
-            break
+            break  
+    return colheader,stat
     
+    
+filein = "/home/psakicki/GFZ_WORK/IPGP_WORK/OVS/GNSS_OVS/2402_test_pride_pppar/240220e_run_pos/run_wo_oload/WUM0MGXFIN/BORG/S/2023/155/pos_2023155_borg"
+
+def read_pride_pppar_pos_mono(filein):
+    colheader,stat_header = _pride_pppar_end_header(filein)
+        
     df = pd.read_csv(filein,skiprows=colheader+1,
-                     delim_whitespace=True,
+                     #delim_whitespace=True,
+                     sep='\s?\*?\s+',
+                     engine='python',
                      header=None)
     
-    t_arr = conv.MJD2dt(df[0]) + df[1].apply(lambda x:dt.timedelta(seconds=x))
     
+    df.columns = ['stat','Mjd','X','Y','Z','Sx','Sy','Sz',
+                  'Rxy','Rxz','Ryz','Sig0','Nobs']
+    
+    df = df.squeeze()
+    
+    T = conv.dt2posix(conv.MJD2dt(df['Mjd']) )
+    
+    pt = time_series.Point(df['X'],df['Y'],df['Z'],T,'XYZ',
+                           df['Sx'],df['Sy'],df['Sz'],
+                           name=df['stat'])
+    
+    return pt
+
+
+def read_pride_pppar_pos(files_list_in):
     tsout = time_series.TimeSeriePoint()
+
+    for file in files_list_in:
+        try:
+            pt = read_pride_pppar_pos_mono(file)
+        except pd.errors.EmptyDataError as e:
+            log.error("%s, %s skipped",e,file)
+            continue
+        
+        tsout.add_point(pt)
+    tsout.meta_set(stat=pt.name)
+    tsout.sort()
+    
+    return tsout
+
+
+def read_pride_pppar_kin(filein):
+    
+    stat = "XXXX"
+
+    colheader,stat = _pride_pppar_end_header(filein)
     
+
+    df = pd.read_csv(filein,skiprows=colheader+1,
+                     #delim_whitespace=True,
+                     sep='\s?\*?\s+',
+                     engine='python',
+                     header=None)
+        
+    t_arr = conv.MJD2dt(df[0]) + df[1].apply(lambda x:dt.timedelta(seconds=x))
+    
+    tsout = time_series.TimeSeriePoint()
     
     tsout = time_series.ts_from_list(df[2].values,
-                                     df[3].values,
-                                     df[4].values,
-                                     t_arr, 'XYZ',
-                                     stat=stat,
-                                     name=stat)
+                                      df[3].values,
+                                      df[4].values,
+                                      t_arr, 'XYZ',
+                                      stat=stat,
+                                      name=stat)
     
     return tsout
     
     
     
 
 def read_webobs(filein,typein="txt",
```

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_eop.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_eop.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_geo_files_misc.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_geo_files_misc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_gnss_prods.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_gnss_prods.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,16 @@
  # | |  | | '__| '_ \| | __| / / \___ \|  ___/|__ <  |  _| | |/ _ \/ __|
  # | |__| | |  | |_) | | |_ / /  ____) | |    ___) | | | | | |  __/\__ \
  #  \____/|_|  |_.__/|_|\__/_/  |_____/|_|   |____/  |_| |_|_|\___||___/
                                                                       
 def read_sp3(file_path_in,returns_pandas = True, name = '',
              epoch_as_pd_index = False,km_conv_coef=1,
              skip_null_epoch=True,
-             new_col_names=True):
+             new_col_names=True,
+             pos_vel_col=False):
     """
     Read a SP3 file (GNSS Orbits standard file) and return X,Y,Z coordinates
     for each satellite and for each epoch
 
     Parameters
     ----------
     file_path_in : str
@@ -267,22 +268,32 @@
         
     skip_null_epoch :bool
         Do not write an epoch if all sats are null (filtering)
         
     new_col_names : bool
         A legacy option to have (or not) consistent column names with read_rinex
         Default is False
-
+        
     Returns
     -------
     df : Pandas DataFrame
         if returns_pandas == True
 
     epoch_stk ,  Xstk , Ystk , Zstk , Clkstk : lists
         if returns_pandas == False
+        
+    Note
+    ----
+    SP3 coordinates are usually given in ITRF, i.e. an ECEF system
+    
+    If the SP3 contains velocity records, this option adds a 'pv' column
+    containing 'P' for position or 'V' for velocity.
+    
+    Warning: velocity 'V' records are in dm/s per default, and the 
+    same km_conv_coef coefficient as the position records will be applied!
 
     """
     
     AC_name =  os.path.basename(file_path_in)[:3]
     
     if file_path_in[-2:] in ("gz","GZ"):
         F = gzip.open(file_path_in, "r+")
@@ -305,23 +316,23 @@
     data_stk    = []
     AC_name_stk = []
    
     # Why this here ?!? (PSa 202104)
     # if returns_pandas:
     #     df = pd.DataFrame(data_stk, columns=['epoch','sat', 'const', 'sv','type',
     #                                        'x','y','z','clk','AC'])
-
+        
     if not new_col_names:
         log.warning("you use old column names (not conventional) set new_col_names as True and adapt your code")
         ### DeprecationWarning
         col_names=['epoch','sat','const','sv',
                    'type','x','y','z','clk','AC']
     else:
         col_names=['epoch','prn','sys','prni',
-                   'rec','x','y','z','clk','ac']   
+                   'rec','x','y','z','clk','ac']
 
     #### read the Header as a 1st check
     Header = read_sp3_header(Lines,AC_name)
     if Header.empty:
         log.warning("The SP3 looks empty: ",file_path_in)
         if returns_pandas:            
             df = pd.DataFrame([], columns=col_names)
```

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_gnss_qc.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_gnss_qc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_igs_combi.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_igs_combi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_logsheets.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_logsheets.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_rinex.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/read_slr.py` & `geodezyx-4.4.2/geodezyx/files_rw/read_slr.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/write_geo_files.py` & `geodezyx-4.4.2/geodezyx/files_rw/write_geo_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     if not "clk" in SP3_DF_wrk.columns:
         SP3_DF_wrk["clk"] = 999999.999999
     
     for epoc in EpochRawList:
         SP3epoc   = pd.DataFrame(SP3_DF_wrk[SP3_DF_wrk["epoch"] == epoc])
         
         ######## if keep_missing_sat_in_epoch:
-        ## manage missing Sats for the current epoc
+        ## manage missing sats for the current epoc
         MissingSats = SatListSet.difference(set(SP3epoc["prn"]))
         
         for miss_sat in MissingSats:
             miss_line = SP3epoc.iloc[0].copy()
             miss_line["prn"]   = miss_sat
             miss_line["sys"] = miss_sat[0]
             ### check the sp3 doc
```

### Comparing `geodezyx-4.4.1/geodezyx/files_rw/write_rinex.py` & `geodezyx-4.4.2/geodezyx/files_rw/write_rinex.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/geodyn/emsgfz_load_interp.py` & `geodezyx-4.4.2/geodezyx/geodyn/emsgfz_load_interp.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/geodyn/euler_pole_calc.py` & `geodezyx-4.4.2/geodezyx/geodyn/euler_pole_calc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/geodyn/velo_field_map_plt.py` & `geodezyx-4.4.2/geodezyx/geodyn/velo_field_map_plt.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/geodyn/volcano_mogi.py` & `geodezyx-4.4.2/geodezyx/geodyn/volcano_mogi.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/logconfig/loggzyx.py` & `geodezyx-4.4.2/geodezyx/logconfig/loggzyx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# THE loggers KEY MUST DESCRIBES THE CURRENT MODULE/PROJECT!!!!
+
 ###### USEFUL TUTOS
 ## https://coderzcolumn.com/tutorials/python/logging-simple-guide-to-log-events-in-python
 ## https://coderzcolumn.com/tutorials/python/logging-config-simple-guide-to-configure-loggers-from-dictionary-and-config-files-in-python#2
 
 log_config_dict = {
     "version":1,
     'disable_existing_loggers': False,
@@ -11,15 +13,15 @@
         "handlers" : ["console_root"],
         "level": "WARN",
         "propagate": False
     },
     
     
     'loggers': {
-        "geodezyx" : {
+        "geodezyx" : {  # THIS KEY MUST DESCRIBES THE CURRENT MODULE!!!!
             "handlers" : ["console_gyxz"],
             "level": "DEBUG",
             "propagate": False
 
         }
     },
```

### Comparing `geodezyx-4.4.1/geodezyx/marine/marine.py` & `geodezyx-4.4.2/geodezyx/marine/marine.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/marine/obp.py` & `geodezyx-4.4.2/geodezyx/marine/obp.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/marine/obscom.py` & `geodezyx-4.4.2/geodezyx/marine/obscom.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,15 +130,32 @@
                       'T5': 0.,
                       'C1':-22682.65,
                       'C2':-1143.743,
                       'C3': 70903.62,
                       'D1': 0.040903,
                       'D2': 0.0}
                 
-    elif sens_id == 158073:
+    elif sens_id == 158073 or sens_id == "T3":
+        ### for the 1st OBSCOM      
+        dic_coeffs = {'U0':5.798999,
+                      'Y1':-3874.954,
+                      'Y2':-10166.55,
+                      'Y3':0,
+                      'C1':-25657.25,
+                      'C2':-645.8024,
+                      'C3':73515.96,
+                      'D1':0.039737,
+                      'D2':0,
+                      'T1':30.00177,
+                      'T2':0.723913,
+                      'T3':53.84611,
+                      'T4':147.1236,
+                      'T5':0}
+        
+    elif sens_id == 158073999 or sens_id == "T3gross": ### 999 suffix = gross
         ### for the 1st OBSCOM      
         dic_coeffs = {'U0':5.799,
                       'Y1':-3874.95,
                       'Y2':-10166.5,
                       'Y3':0,
                       'C1':-25657.2,
                       'C2':-645.802,
@@ -146,16 +163,34 @@
                       'D1':0.0397368,
                       'D2':0,
                       'T1':30.0018,
                       'T2':0.723913,
                       'T3':53.8461,
                       'T4':147.124,
                       'T5':0}
+            
+    elif sens_id == 158076 or sens_id == "T2":
+        ### for the 2nd OBSCOM (T2)
+        dic_coeffs = {'U0':5.765270 ,
+                      'Y1':-3994.585,
+                      'Y2':-10705.43,
+                      'Y3':0        ,
+                      'C1':-25561.86,
+                      'C2':-230.0508,
+                      'C3':79516.88 ,
+                      'D1':0.040172 ,
+                      'D2':0        ,
+                      'T1':30.13945 ,
+                      'T2':0.977439 ,
+                      'T3':56.64988 ,
+                      'T4':158.4542 ,
+                      'T5':0        }
     
-    elif sens_id == 158076:
+
+    elif sens_id == 158076999 or sens_id == "T2gross": ### 999 suffix = gross
         ### for the 2nd OBSCOM (T2)
         dic_coeffs = {'U0':5.76527  ,
                       'Y1':-3994.58 ,
                       'Y2':-10705.4 ,
                       'Y3':0        ,
                       'C1':-25561.9 ,
                       'C2':-230.051 ,
@@ -163,15 +198,34 @@
                       'D1':0.0401721,
                       'D2':0        ,
                       'T1':30.1394  ,
                       'T2':0.977439 ,
                       'T3':56.6499  ,
                       'T4':158.454  ,
                       'T5':0        }
-        
+
+
+    elif sens_id == 158081 or sens_id == "T4":
+        ### for the 2nd OBSCOM (T2)
+        dic_coeffs = {'U0':5.797503 ,
+                      'Y1':-4022.350,
+                      'Y2':-12679.85,
+                      'Y3':0        ,
+                      'C1':-22175.21,
+                      'C2':-1252.800,
+                      'C3':83574.76 ,
+                      'D1':0.037913 ,
+                      'D2':0        ,
+                      'T1':30.23989 ,
+                      'T2':0.124474 ,
+                      'T3':64.95771 ,
+                      'T4':229.3125 ,
+                      'T5':0        }
+    
+    
         
     if sens_type == 'all':
         return dic_coeffs
     elif sens_type == 'f0':
         return _get_coeffs_f0(dic_coeffs) 
     elif sens_type == 'temp':
         return _get_coeffs_temp(dic_coeffs)
```

### Comparing `geodezyx-4.4.1/geodezyx/megalib/geoclass.py` & `geodezyx-4.4.2/geodezyx/megalib/geoclass.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/megalib/softs_runner.py` & `geodezyx-4.4.2/geodezyx/megalib/softs_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/__init__.py` & `geodezyx-4.4.2/geodezyx/operational/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 from .download_find_files    import *
 from .download_prods         import *
 from .download_rinex         import *
 from .download_utils         import *
 from .groops_frontend       import *
 from .hector_frontend       import *
 from .midas_frontend        import *
+from .pride_pppar_frontend  import *
 from .rinex_lister_plotter  import *
 from .rinex_utils           import *
 from .rtklib_frontend       import *
 from .track_frontend        import *
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/anubis_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/anubis_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Jul  5 15:48:26 2022
 
-@author: psakicki
+@author: psakic
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import os 
 import re
@@ -191,21 +191,21 @@
             nav_path = potential_nav_path
 
         #### the nav file does not exsits but we want to download it
         elif not nav_file_exists and download_nav:
             log.debug("%s not found, we downloading it",potential_nav_file)
             statdico = dict()
             statdico['brdc'] = ['BRDC']
-            brdc_list = operational.multi_downloader_rinex(statdico,
-                                                           nav_dir,
-                                                           date_start,date_end,
+            brdc_list = operational.download_gnss_rinex(statdico,
+                                                        nav_dir,
+                                                        date_start, date_end,
                                                            "/",
-                                                           parallel_download=1,
-                                                           sorted_mode=0,
-                                                           final_archive_for_sup_check=nav_dir)    
+                                                        parallel_download=1,
+                                                        sorted_mode=0,
+                                                        final_archive_for_sup_check=nav_dir)
             if brdc_list:
                 nav_path = brdc_list[0]
             else:
                 nav_path = ""
         
         #### we do not consider the nav file
         else:
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/cluster_gfz.py` & `geodezyx-4.4.2/geodezyx/operational/cluster_gfz.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_cddis.py` & `geodezyx-4.4.2/geodezyx/operational/download_cddis.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_dropbox.py` & `geodezyx-4.4.2/geodezyx/operational/download_dropbox.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_find_files.py` & `geodezyx-4.4.2/geodezyx/operational/download_find_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -239,15 +239,16 @@
 
 def find_IGS_products_files(parent_dir, File_type, ACs, date_start, date_end=None,
                             recursive_search=True, severe=True,
                             compressed="incl",
                             regex_old_naming=True,
                             regex_new_naming=True,
                             regex_igs_tfcc_naming=True,
-                            add_weekly_file=False):
+                            add_weekly_file=False,
+                            add_hourly_file=False):
     """
     Find all product files in a parent folder which correspond to file type(s),
     AC(s) and date(s)
 
     Parameters
     ----------
     parent_dir : str or list of str
@@ -296,14 +297,18 @@
     regex_igs_tfcc_naming : bool
         Handle TFCC specific format (for SINEX files)
 
     add_weekly_file : bool
         Also handle the weekly file (day 7)
         Implemented only for the  old naming format (for the moment)
 
+    add_hourly_file : bool
+        Also handle ultra rapide hourly file
+        Implemented only for the new naming format
+
     Returns
     -------
     Files_select_cumul_list : list
         List of files found
 
     """
 
@@ -326,23 +331,32 @@
         date_end_ok = date_start_ok
     elif type(date_end) is dt.datetime:
         date_end_ok = date_end
     else:
         date_end_ok = conv.gpstime2dt(*date_end)
     # generate time period with a while loop
     Dates_list = [date_start_ok]
+    
+    if add_hourly_file:
+        deltat = dt.timedelta(seconds=3600)
+    else:
+        deltat = dt.timedelta(days=1)
+    
     while Dates_list[-1] < date_end_ok:
-        Dates_list.append(Dates_list[-1] + dt.timedelta(days=1))
+        Dates_list.append(Dates_list[-1] + deltat)
 
     # manage weekly file
     Dates_wwwwd_list = [utils.join_improved(
         "", *conv.dt2gpstime(d, outputtype=str)) for d in Dates_list]
-    Dates_yyyyddd_list = [utils.join_improved(
-        "", *reversed(conv.dt2doy_year(d))) for d in Dates_list]
-
+    
+    if add_hourly_file:
+        Dates_yyyyddd_list = [utils.join_improved("", *reversed(conv.dt2doy_year(d)),str(d.hour).zfill(2)) for d in Dates_list]
+    else:
+        Dates_yyyyddd_list = [utils.join_improved("", *reversed(conv.dt2doy_year(d))) for d in Dates_list]
+        
     ###### File type / ACs management ##############
 
     if not utils.is_iterable(File_type):
         File_type = [File_type]
     if not utils.is_iterable(ACs):
         ACs = [ACs]
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_prods.py` & `geodezyx-4.4.2/geodezyx/operational/download_prods.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-from ftplib import FTP, FTP_TLS
+from ftplib import FTP
 # import glob
 import itertools
 import multiprocessing as mp
 import numpy as np
 import os
 # import pandas as pd 
 import re
@@ -57,43 +57,97 @@
                                                                                                       
                                                                                                       
 
 ############################################################################
 ######## PRODUCTS DOWNLOADER
 ############################################################################
 
-def download_products_gnss(archive_dir,
-                           startdate,enddate,
+def download_gnss_products(archive_dir,
+                           startdate, enddate,
                            AC_names = ("wum","cod"),
                            prod_types = ("sp3","clk"),
                            remove_patterns=("ULA",),
                            archtype ='week',
                            new_name_conv = True,
                            parallel_download=4,
                            archive_center='ign',
                            mgex=False,
                            repro=0,
                            sorted_mode=False,
                            return_also_uncompressed_files=True,
                            ftp_download=False,
                            dow_manu=False):
     """
-    dow_manu = False, no dow manu, consider the converted dow from the time span, regular case
-    dow_manu = None, no dow in the REGEX, the crawler will search only for the week
-    dow_manu = 0 or 7: the dow in question    
-    
-    
-    to control the lattency with the new naming convention, simply add it completly in the AC name
-    e.g. IGS0OPSRAP
-    
+    Download GNSS products from different IGS data centers
+
+    Parameters
+    ----------
+    archive_dir : str
+        the parent directory where the products will be stored.
+    startdate : datetime
+        the start date in regular calendar date.
+    enddate : datetime
+        the end date in regular calendar date..
+    AC_names : tuple, optional
+        the names of the wished analysis centers.
+        It also control the product's lattency with the new naming convention: 
+        simply add it completly in the AC name e.g. IGS0OPSRAP
+        The default is ("wum","cod").
+    prod_types : tuple, optional
+        the wished products. 
+        The default is ("sp3","clk").
+    remove_patterns : tuple, optional
+        the patterns you want to exclude. 
+        The default is ("ULA",).
+    archtype : str, optional
+        structure of the local archive sub-directories.
+        see `effective_save_dir_orbit` function for more details.
+        The default is 'week'.
+        an alternatiove can be 'year/doy'.
+    new_name_conv : bool, optional
+        Also handle the new name convention. The default is True.
+    parallel_download : int, optional
+        control parallel download.
+        The default is 4.
+    archive_center : TYPE, optional
+        name of the IGS's archive/data center. The default is 'ign'.
+    mgex : bool, optional
+        get MGEX products. The default is False.
+    repro : int, optional
+        get repro products. The default is 0 i.e. operational products.
+    sorted_mode : bool, optional
+        sort the download or not. The default is False.
+    return_also_uncompressed_files : bool, optional
+        in the final list output, return also already downloaded and 
+        uncompressedfiles. The default is True.
+    ftp_download : bool, optional
+        DESCRIPTION. The default is False.
+    dow_manu : int or bool or None, optional
+        Control the download for weekly files
+        dow_manu = False, no dow manu, 
+        consider the converted dow from the time span, regular case
+        dow_manu = None, 
+        no dow in the REGEX, the crawler will search only for the week
+        dow_manu = 0 or 7,
+        the dow in question    
+        The default is False.
+
+
+    Returns
+    -------
+    list
+        list of the local files's paths.
+
     Note
     ----
     The new naming convention has been fully adopted since GPS Week 2238-0
 
-    
+    to control the lattency with the new naming convention, 
+    simply add it completly in the AC name e.g. IGS0OPSRAP
+        
     """
     
     if mgex:
         mgex_str = "mgex/"
     else:
         mgex_str = ""
         
@@ -153,64 +207,17 @@
         ftp_download = False
         log.info('ACC experimental mgex combi. as data center, HTTP download forced')
 
 
     Dates_list = conv.dt_range(startdate,enddate)
 
     wwww_dir_previous = None
-    pool = mp.Pool(processes=parallel_download) 
-
-    ## internal fct to create the FTP objects
-    
-    class MyFTP_TLS(FTP_TLS):
-        """Explicit FTPS, with shared TLS session"""
-        ### This new class is to avoid the error 
-        ### ssl.SSLEOFError: EOF occurred in violation of protocol (_ssl.c:2396)
-        ### source:
-        ### https://stackoverflow.com/questions/14659154/ftps-with-python-ftplib-session-reuse-required
-        def ntransfercmd(self, cmd, rest=None):
-            conn, size = FTP.ntransfercmd(self, cmd, rest)
-            if self._prot_p:
-                conn = self.context.wrap_socket(conn,
-                                                server_hostname=self.host,
-                                                session=self.sock.session)  # this is the fix
-            return conn, size
-        
-    def ftp_objt_create(secure_ftp_inp,chdir=""):
-        
-        # define the right constructor
-        if secure_ftp_inp:
-            ftp_constuctor = MyFTP_TLS
-            #ftp=ftp_constuctor()
-            #ftp.set_debuglevel(2)
-            #ftp.connect(arch_center_main)
-            #ftp.login('anonymous','')
-            #ftp.prot_p()
-        else:     
-            ftp_constuctor = FTP
-            #ftp = ftp_constuctor(arch_center_main)
-            #ftp.login()
-            
-        ## create a list of FTP object for multiple downloads
-        Ftp_obj_list_out = [ftp_constuctor(arch_center_main) for i in range(parallel_download)]
-        if secure_ftp:
-            [f.login('anonymous','') for f in Ftp_obj_list_out]    
-            [f.prot_p() for f in Ftp_obj_list_out]    
-        else:
-            [f.login() for f in Ftp_obj_list_out]    
-            
-        # define the main obj for crawling
-        ftp_main = Ftp_obj_list_out[0]
-        
-        # change the directory of the main ftp obj if we ask for it
-        if chdir:
-            log.info("Move to: %s",chdir)
-            ftp_main.cwd(chdir)
-        
-        return ftp_main, Ftp_obj_list_out
+    if parallel_download > 1:
+        pool = mp.Pool(processes=parallel_download)  
+   
     
     ###################################################################
     ########### Remote file search      
 
     Potential_localfiles_list_all = []
     
     ### check if the pattern of the wished products are in the listed daily files
@@ -235,15 +242,16 @@
         
         n_ftp_ask = 500 ## Max interrogation of the FTP server to avoid 
                         ## potential errors
                         ## An new FTP instance is created if above it 
         
         if np.mod(ipatt_tup,n_ftp_ask) == 0:
             log.info("Create a new FTP instance")
-            ftp, Ftp_obj_list = ftp_objt_create(secure_ftp)
+            ftp, Ftp_obj_list = dlutils.ftp_objt_create(secure_ftp_inp=secure_ftp,
+                                                        host=arch_center_main)
             
         if wwww_dir_previous != wwww_dir or np.mod(ipatt_tup,n_ftp_ask) == 0:
             log.info("Move to: %s",wwww_dir)
             try:
                 ftp.cwd(wwww_dir)
             except:
                 log.warning("%s do not exists, skiping...",wwww_dir)
@@ -265,41 +273,40 @@
             
             if dow is None:
                 log.error("dow == None and search for new name convention, Error ...")
                 raise  Exception()
                 
             ac_newnam   = ac_cur.upper()
 
-            doy_newnam  = "".join(reversed(conv.dt2doy_year(conv.gpstime2dt(wwww,dow))))
+            doy_newnam  = "".join(reversed(conv.dt2doy_year(dt_cur))) + str(dt_cur.hour).zfill(2)
             prod_newnam = prod_cur.upper()
             
             pattern_new_nam = utils.join_improved(".*",ac_newnam,doy_newnam,prod_newnam)
             pattern_new_nam = ".*" + pattern_new_nam + "\..*"
 
             Files_new_nam   = [f for f in Files_listed_in_FTP if re.search(pattern_new_nam,f)]
         
         
         log.info("Regex : %s %s",pattern_old_nam,pattern_new_nam)        
         Files = Files + Files_new_nam
         
         if len(Files) == 0:
             log.warning("no product found for" + " %s"*len(patt_tup),
                         *patt_tup)
+            #log.warning("found files: %s",Files_listed_in_FTP)
         
         Files_remote_date_list = Files_remote_date_list + Files
             
         ### exclude some pattern
         for negpatt in remove_patterns:
             Files_remote_date_list = [e for e in Files_remote_date_list if not re.search(negpatt,e)]
             
             
         ###################################################################
         ########### Download
-            
-
         archive_dir_specif = dlutils.effective_save_dir_orbit(archive_dir,
                                                               ac_cur,
                                                               dt_cur,
                                                               archtype)
         
         if len(Files_remote_date_list) > 0:
             utils.create_dir(archive_dir_specif)
@@ -309,20 +316,25 @@
                                                  parallel_download)
         Downld_tuples_list = []
         Potential_localfiles_list = []
 
         if ftp_download: ### FTP Download
             for ftpobj , Chunk in zip(Ftp_obj_list,Files_remote_date_chunck):
                 for filchunk in Chunk:
-                    Potential_localfiles_list.append(os.path.join(archive_dir_specif,filchunk))
+                    Potential_localfiles_list.append(os.path.join(archive_dir_specif,
+                                                                  filchunk))
                     if parallel_download == 1:
-                        Downld_tuples_list.append((ftpobj,filchunk,archive_dir_specif))
+                        Downld_tuples_list.append((ftpobj,
+                                                   filchunk,
+                                                   archive_dir_specif))
                     else:
-                        Downld_tuples_list.append((arch_center_main,wwww_dir,
-                                                   filchunk,archive_dir_specif))
+                        Downld_tuples_list.append((arch_center_main,
+                                                   wwww_dir,
+                                                   filchunk,
+                                                   archive_dir_specif))
         else: ### HTTP download
             Downld_tuples_list = itertools.product(["/".join(('ftp://' + arch_center_main,wwww_dir,f)) for f in Files_remote_date_list],[archive_dir_specif])
             [Potential_localfiles_list.append(os.path.join(archive_dir_specif,f)) for f in Files_remote_date_list]
         
         Potential_localfiles_list_all = Potential_localfiles_list_all +  Potential_localfiles_list 
 
         ### Actual Download
@@ -355,21 +367,22 @@
             
             Pot_locfiles_list_use = Pot_locfiles_list_use + Pot_compress_name_list
             
     for pot_localfile in Pot_locfiles_list_use:
         if os.path.isfile(pot_localfile):
             Localfiles_lis.append(pot_localfile)
     
-    pool.close()
+    if parallel_download > 1:
+        pool.close()
     return Localfiles_lis
 
 
-def multi_downloader_orbs_clks_2():
-    log.warn('multi_downloader_orbs_clks_2 is a legacy alias for the newly renamed function download_products_gnss')
-    #return download_products_gnss(**kwargs)
+def multi_downloader_orbs_clks_2(**kwargs):
+    log.warn('multi_downloader_orbs_clks_2 is a legacy alias for the newly renamed function download_gnss_products')
+    return download_gnss_products(**kwargs)
 
 
 def orbclk_long2short_name(longname_filepath_in,
                            rm_longname_file=False,
                            center_id_last_letter=None,
                            center_manual_short_name=None,
                            force=False,
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_rinex.py` & `geodezyx-4.4.2/geodezyx/operational/download_rinex.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,227 +28,259 @@
 # import ftplib
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 import geodezyx.operational.download_utils as dlutils
 
-
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 
 #### Import the logger
 import logging
+
 log = logging.getLogger(__name__)
 
-##########  END IMPORT  ##########
 
+##########  END IMPORT  ##########
 
 
 #_____________ _   _ ________   __  _____                      _                 _
 #|  __ \|_   _| \ | |  ____\ \ / / |  __ \                    | |               | |
 #| |__) | | | |  \| | |__   \ V /  | |  | | _____      ___ __ | | ___   __ _  __| | ___ _ __
 #|  _  /  | | | . ` |  __|   > <   | |  | |/ _ \ \ /\ / / '_ \| |/ _ \ / _` |/ _` |/ _ \ '__|
 #| | \ \ _| |_| |\  | |____ / . \  | |__| | (_) \ V  V /| | | | | (_) | (_| | (_| |  __/ |
 #|_|  \_\_____|_| \_|______/_/ \_\ |_____/ \___/ \_/\_/ |_| |_|_|\___/ \__,_|\__,_|\___|_|
 
 
-
 ############################################################################
 ######## RINEX DOWNLOADER
 ############################################################################
 
 
-def igs_garner_server(stat,date):
+def igs_sopac_server(stat, date):
     # plante si trop de requete
     urlserver = "ftp://garner.ucsd.edu/pub/rinex/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join( urlserver , str(date.year) , conv.dt2doy(date) , rnxname )
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
-def igs_cddis_server(stat,date):
+
+def igs_cddis_server(stat, date, user = '', passwd = ''):
     # a privilegier
-    urlserver = "ftp://cddis.gsfc.nasa.gov/gps/data/daily/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , date.strftime('%y') + 'd' , rnxname)
-    return url
+    urlserver = "ftp://gdc.cddis.eosdis.nasa.gov/gps/data/daily/"
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), date.strftime('%y') + 'd', rnxname)
+    if not passwd:
+        passwd = 'sakic@ipgp.fr'
+    return url, user, passwd
 
-def igs_cddis_nav_server(stat,date):
+
+def igs_cddis_nav_server(stat, date):
     # a privilegier
     urlserver = "ftp://cddis.gsfc.nasa.gov/gps/data/daily/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date,'n.Z')
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , date.strftime('%y') + 'n' , rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date, 'n.Z')
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), date.strftime('%y') + 'n', rnxname)
     return url
 
-def rob_nav_server(stat,date):
-    # a privilegier
+
+def nav_bkg_server(stat, date):
+    urlserver = "ftp://igs-ftp.bkg.bund.de/IGS/BRDC/"
+    #ftp://igs-ftp.bkg.bund.de/IGS/BRDC/2024/082/BRDC00WRD_S_20240820000_01D_MN.rnx.gz
+    rnxname = "BRDC00WRD_S_" + conv.dt2str(date, '%Y%j') + "0000_01D_MN.rnx.gz"
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
+    return url
+
+
+def nav_rob_server(stat, date):
     urlserver = "ftp://epncb.oma.be/pub/obs/BRDC/"
     #ftp://epncb.oma.be/pub/obs/BRDC/2018/BRDC00GOP_R_20180010000_01D_MN.rnx.gz
-    rnxname = "BRDC00GOP_R_" + conv.dt2str(date,'%Y%j') + "0000_01D_MN.rnx.gz"
-    url = os.path.join(urlserver , str(date.year) , rnxname)
+    rnxname = "BRDC00GOP_R_" + conv.dt2str(date, '%Y%j') + "0000_01D_MN.rnx.gz"
+    url = os.path.join(urlserver, str(date.year), rnxname)
     return url
 
-def rgp_ign_smn_server(stat,date):
+
+def rgp_ign_smn_server(stat, date):
     urlserver = "ftp://rgpdata.ign.fr/pub/data/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , 'data_30' , rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'data_30', rnxname)
     return url
 
-def rgp_ign_mlv_server(stat,date):
+
+def rgp_ign_mlv_server(stat, date):
     urlserver = "ftp://rgpdata.ensg.eu/pub/data/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , 'data_30' , rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'data_30', rnxname)
     return url
 
-def rgp_ign_smn_1Hz_server(stat,date):
+
+def rgp_ign_smn_1Hz_server(stat, date):
     urlserver = "ftp://rgpdata.ign.fr/pub/data/"
 
     urls = []
 
     for h in range(24):
         date_session = date
         date_session = date_session.replace(hour=h)
 
-        log.info('%s session %s' , date_session , h)
-        rnxname = conv.statname_dt2rinexname(stat.lower(),date_session ,
-                                             session_a_instead_of_daily_session = 1)
-        url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) ,
-                           'data_1' , rnxname)
+        log.info('%s session %s', date_session, h)
+        rnxname = conv.statname_dt2rinexname(stat.lower(), date_session,
+                                             session_a_instead_of_daily_session=1)
+        url = os.path.join(urlserver, str(date.year), conv.dt2doy(date),
+                           'data_1', rnxname)
 
         urls.append(url)
 
     return urls
 
-def unavco_server(stat,date):
-    urlserver='ftp://data-out.unavco.org/pub/rinex'
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , 'obs', str(date.year) , conv.dt2doy(date) , rnxname)
+
+def unavco_server(stat, date):
+    urlserver = 'ftp://data-out.unavco.org/pub/rinex'
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, 'obs', str(date.year), conv.dt2doy(date), rnxname)
     return url
 
-def renag_server(stat,date):
+
+def renag_server(stat, date):
     urlserver = "ftp://renag.unice.fr/data/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
-def uwiseismic_server(stat,date,user='',passwd=''):
+def uwiseismic_server(stat, date, user='', passwd=''):
     urlserver = "ftp://www2.uwiseismic.com/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , 'rinex' , str(date.year) , conv.dt2doy(date) , rnxname)
-    return url,user,passwd
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, 'rinex', str(date.year), conv.dt2doy(date), rnxname)
+    return url, user, passwd
 
-def orpheon_server(stat,date,user='',passwd=''):
+
+def orpheon_server(stat, date, user='', passwd=''):
     urlserver = "ftp://renag.unice.fr/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , rnxname)
-    return url,user,passwd
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
+    return url, user, passwd
 
 
-def ovsg_server(stat,date,user='',passwd=''):
-    if dt.datetime(2009,1,1) <= date <= dt.datetime(2014,2,10):
+def ovsg_server(stat, date, user='', passwd=''):
+    if dt.datetime(2009, 1, 1) <= date <= dt.datetime(2014, 2, 10):
         urlserver = "http://webobs.ovsg.univ-ag.fr/rawdata/GPS-GPSDATA.backtemp_20140210/"
     else:
         urlserver = "http://webobs.ovsg.univ-ag.fr/rawdata/GPS/GPSDATA/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , 'rinex' , rnxname)
-    return url,user,passwd
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'rinex', rnxname)
+    return url, user, passwd
+
 
-def geoaus_server(stat,date):
+def geoaus_server(stat, date):
     """ Geosciences Australia
         ex : ftp://ftp.ga.gov.au/geodesy-outgoing/gnss/data/daily/2010/10063/ """
     urlserver = "ftp://ftp.ga.gov.au/geodesy-outgoing/gnss/data/daily/"
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , date.strftime('%y') + conv.dt2doy(date) , rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), date.strftime('%y') + conv.dt2doy(date), rnxname)
     return url
 
-def sonel_server(stat,date):
+
+def sonel_server(stat, date):
     """ex : ftp://ftp.sonel.org/gps/data/2015/001/ """
     urlserver = 'ftp://ftp.sonel.org/gps/data/'
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver,str(date.year),conv.dt2doy(date),rnxname)
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
-def effective_save_dir(parent_archive_dir,stat,date,archtype ='stat'):    
+def ens_fr(stat, date):
+    urlserver = 'ftp://gnss.ens.fr/pub/public/crl/GPS/rinex/'
+    rnxname = conv.statname_dt2rinexname(stat.lower(), date)
+    url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
+    return url
+
+
+def effective_save_dir(parent_archive_dir, stat, date, archtype='stat'):
     """
     INTERNAL_FUNCTION
 
     archtype =
         stat
         stat/year
         stat/year/doy
         year/doy
         year/stat
         week/dow
         OR only '/' for a dirty saving in the parent folder
         ... etc ... """
     if archtype == '/':
         return parent_archive_dir
-    
+
     if len(archtype) > 0 and archtype[0] == "/":
         log.warn("The archive type description starts with a /, remove it to avoid an error")
 
     out_save_dir = parent_archive_dir
     fff = archtype.split('/')
-    #year = str(date.year)
-    #doy = conv.dt2doy(date)
+    year = str(date.year)
+    doy = conv.dt2doy(date)
+    _,_ = year,doy ## simply to remove the unused linter warning...
     week, dow = conv.dt2gpstime(date)
     for f in fff:
-        out_save_dir = os.path.join(out_save_dir,eval(f))
+        out_save_dir = os.path.join(out_save_dir, eval(f))
     return out_save_dir
 
+def multi_downloader_rinex(**kwargs):
+    log.warn('multi_downloader_rinex is a legacy alias for the newly renamed function download_gnss_rinex')
+    return download_gnss_rinex(**kwargs)
 
-def ens_fr(stat,date):    
-    urlserver='ftp://gnss.ens.fr/pub/public/crl/GPS/rinex/'
-    rnxname = conv.statname_dt2rinexname(stat.lower(),date)
-    url = os.path.join(urlserver , str(date.year) , conv.dt2doy(date) , rnxname)
-    return url
 
-def multi_downloader_rinex(statdico,archive_dir,startdate,enddate,
-                           archtype ='stat',parallel_download=4,
-                           sorted_mode=False,user='',passwd='',
-                           filter_ftp_crawler=True,
-                           path_ftp_crawled_files_save=None,
-                           path_ftp_crawled_files_load=None,
-                           silent_mode=False,
-                           final_archive_for_sup_check=None):
+def download_gnss_rinex(statdico, archive_dir, startdate, enddate,
+                        archtype='stat', parallel_download=4,
+                        sorted_mode=False, user='', passwd='',
+                        filter_ftp_crawler=True,
+                        path_ftp_crawled_files_save=None,
+                        path_ftp_crawled_files_load=None,
+                        quiet_mode=False,
+                        final_archive_for_sup_check=None,
+                        force=False):
     """
     Parameters
     ----------
     statdico : dict
         a statdico is a dictionary associating Archives Centers to list of stations
 
         Exemple:
             >>> statdico['archive center 1'] = ['STA1','STA2','STA3', ...]
             >>> statdico['archive center 2'] = ['STA2','STA1','STA4', ...]
 
         the supported archive center are (july 2015):
-            igs (cddis center)
+            igs_cddis or igs (cddis center)
 
-            igs_garner (for the garner center, but not very reliable)
+            igs_sopac (for the sopac/ucsd/sio center, but not very reliable)
 
-            rgp (St Mandé center)
+            rgp (IGN's RGP St Mandé center)
 
-            rgp_mlv (Marne la Vallée center)
+            rgp_mlv (IGN's RGP Marne la Vallée center)
 
-            rgp_1Hz (all the 24 hourly rinex for the day will be downloaded)
+            rgp_1Hz (IGN's RGP, all the 24 hourly rinex for the day will be downloaded)
 
             renag
 
             ovsg
 
             unavco
 
             sonel
 
             geoaus (Geosciences Australia)
+            
+            ens_fr
+
+            nav or brdc as archive center allows to download nav files (using 'BRDC' as station name)
+            from the ROB server, using GOP files
 
-            nav or brdc as archive center allows to download nav files (using 'BRDC' as station name) from the CDDIS server
+            nav_rt or brdc_rt as archive center allows to download *real time* nav files
+            from the BKG server
 
 
     archtype : str
         string describing how the archive directory is structured, e.g :
 
             stat
 
@@ -260,15 +292,14 @@
 
             year/stat
 
             week/dow/stat
 
             ... etc ...
 
-
     sorted_mode : bool
         if False:
             using the map multiprocess fct so the download order will
             be scrambled
         if True:
             using the apply multiprocess fct so the download order will be
             in the chrono. order
@@ -288,25 +319,28 @@
         It allows to use this list directly if one face a timeout during 
         the download part.
         NB for advanced users: the pickle is a tuple (urllist,savedirlist)
     
     path_ftp_crawled_files_load : str
         load and use the list of the existing RINEXs found on the FTP server,
         generated by a previous run of the FTP crawler (called by 
-        multi_downloader_rinex or directly by ftp_files_crawler).
+        download_gnss_rinex or directly by ftp_files_crawler).
         overrides an internal call of ftp_files_crawler.
         
-    silent_mode : bool
+    quiet_mode : bool
         List the available RINEXs without downloading them. 
         Useful only if path_ftp_crawled_files_save is given
         
     final_archive_for_sup_check : str
         The final archive path or a file containing the archived RINEXs in
         their final destination. 
         useful if the final archive is different from archive_dir
+        
+    force : bool
+        Force the download even if the file already exists locally
 
     Returns
     -------
     url_list : list of str
         list of URLs
 
     savedir_list : list of str
@@ -316,153 +350,185 @@
     curdate = startdate
 
     pool = mp.Pool(processes=parallel_download)
 
     urllist = []
     savedirlist = []
 
-
     log.info("generating the list of potential RINEXs ...")
     while curdate <= enddate:
-        for netwk , statlis in list(statdico.items()):
+        for netwk, statlis in list(statdico.items()):
+            
+            if not utils.is_iterable(statlis):
+                log.warning("%s given in the 'statdico' should be a list and it is not.",
+                            statlis)
+            
             for stat in statlis:
                 stat = stat.lower()
                 mode1Hz = False
+                secure_ftp = False
 
-                if netwk == 'igs':
-                    url = igs_cddis_server(stat,curdate)
-                elif netwk == 'igs_garner':
-                    url = igs_garner_server(stat,curdate)
+                if netwk in ('igs_cddis','igs'):
+                    secure_ftp = True
+                    url = igs_cddis_server(stat, curdate, user, passwd)
+                elif netwk == 'igs_sopac':
+                    url = igs_sopac_server(stat, curdate)
                 elif netwk == 'rgp':
-                    url = rgp_ign_smn_server(stat,curdate)
+                    url = rgp_ign_smn_server(stat, curdate)
                 elif netwk == 'rgp_mlv':
-                    url = rgp_ign_mlv_server(stat,curdate)
+                    url = rgp_ign_mlv_server(stat, curdate)
                 elif netwk == 'rgp_1Hz':
-                    urls = rgp_ign_smn_1Hz_server(stat,curdate)
+                    urls = rgp_ign_smn_1Hz_server(stat, curdate)
                     mode1Hz = True
                 elif netwk == 'renag':
-                    url = renag_server(stat,curdate)
+                    url = renag_server(stat, curdate)
                 elif netwk == 'orpheon':
-                    url = orpheon_server(stat,curdate,user,passwd)
+                    url = orpheon_server(stat, curdate, user, passwd)
                 elif netwk == 'uwiseismic':
-                    url = uwiseismic_server(stat,curdate,user,passwd)
+                    url = uwiseismic_server(stat, curdate, user, passwd)
                 elif netwk == 'ovsg':
-                    url = ovsg_server(stat,curdate,user,passwd)
+                    url = ovsg_server(stat, curdate, user, passwd)
                 elif netwk == 'unavco':
-                    url = unavco_server(stat,curdate)
+                    url = unavco_server(stat, curdate)
                 elif netwk == 'sonel':
-                    url = sonel_server(stat,curdate)
+                    url = sonel_server(stat, curdate)
                 elif netwk == 'geoaus':
-                    url = geoaus_server(stat,curdate)
-                elif netwk in ('nav' , 'brdc'):
-                    url = rob_nav_server(stat,curdate)
+                    url = geoaus_server(stat, curdate)
+                elif netwk in ('nav', 'brdc'):
+                    url = nav_rob_server(stat, curdate)
+                elif netwk in ('nav_rt', 'brdc_rt'):
+                    url = nav_bkg_server(stat, curdate)
                 elif netwk == 'ens_fr':
-                    url = ens_fr(stat,curdate)
+                    url = ens_fr(stat, curdate)
                 else:
                     log.warning('unkwn server dic in the dico, skip ...')
                     continue
 
-                savedir = effective_save_dir(archive_dir,stat,curdate,archtype)
+                savedir = effective_save_dir(archive_dir, stat, curdate, archtype)
 
                 if not mode1Hz:
                     urllist.append(url)
                     savedirlist.append(savedir)
                 else:
                     urllist = urllist + urls
                     savedirlist = savedirlist + [savedir] * len(urls)
 
         curdate = curdate + dt.timedelta(days=1)
 
     #savedirlist = [x for (y,x) in sorted(zip(urllist,savedirlist))]
     #urllist     = sorted(urllist)
-    
+
     try:
-        urllist,savedirlist = utils.sort_binom_list(urllist,savedirlist)
+        urllist, savedirlist = utils.sort_binom_list(urllist, savedirlist)
     except TypeError as err:
-        log.error("unable to sort the URL and the save directory") 
-        log.error("TIP: you maybe asked for servers with & without password in the same statdico") 
+        log.error("unable to sort the URL and the save directory")
+        log.error("TIP: you maybe asked for servers with & without password in the same statdico")
         raise err
 
     log.info(" ... done")
     log.info(str(len(urllist)) + " potential RINEXs")
 
     ### Use of the advanced FTP Crawler
     if filter_ftp_crawler:
-        if path_ftp_crawled_files_load:
-            urllist,savedirlist = utils.pickle_loader(path_ftp_crawled_files_load)
-        else:
-            urllist,savedirlist = dlutils.ftp_files_crawler(urllist,savedirlist)
+        if path_ftp_crawled_files_load: ## if the previous files are loaded
+            urllist, savedirlist = utils.pickle_loader(path_ftp_crawled_files_load)
+        else: ## regular case
+            urllist, savedirlist = dlutils.ftp_files_crawler(urllist,
+                                                             savedirlist, 
+                                                             secure_ftp=secure_ftp)
             if path_ftp_crawled_files_save:
-                savetup = (urllist,savedirlist)
+                savetup = (urllist, savedirlist)
                 utils.pickle_saver(savetup,
                                    full_path=path_ftp_crawled_files_save)
-                
+
     ##### Check if the rinex file already exists in the final archive
-    if final_archive_for_sup_check:
+    if final_archive_for_sup_check and not force:
         Files_final_arch = utils.find_recursive(final_archive_for_sup_check,
                                                 "*")
         Files_final_arch_basename = [os.path.basename(e) for e in Files_final_arch]
-        
-        urllist_new,savedirlist_new = [],[]
-        
-        for u,sd in zip(urllist,savedirlist):
+
+        urllist_new, savedirlist_new = [], []
+
+        for u, sd in zip(urllist, savedirlist):
             if not os.path.basename(u) in Files_final_arch_basename:
                 urllist_new.append(u)
                 savedirlist_new.append(sd)
-        
-        urllist,savedirlist = urllist_new,savedirlist_new
-                    
-    if not silent_mode:
-        if sorted_mode:
-            _ = [pool.apply_async(dlutils.downloader , args=(u,sd)) for u,sd in zip(urllist,savedirlist)]
-        else:
-            _ = pool.map(dlutils.downloader_wrap,list(zip(urllist,savedirlist)))
 
+        urllist, savedirlist = urllist_new, savedirlist_new
+
+    if not quiet_mode:
+        if not secure_ftp:
+            if sorted_mode:
+                _ = [pool.apply_async(dlutils.downloader, args=(u, sd, force)) for u, sd in zip(urllist, savedirlist)]
+            else:
+                forcelis = [force] * len(urllist)
+                _ = pool.map(dlutils.downloader_wrap, list(zip(urllist,
+                                                               savedirlist,
+                                                               forcelis)))
+        else: ## secure FTP i.e. CDDIS
+            ftp_obj , _ = dlutils.ftp_objt_create(secure_ftp_inp=secure_ftp,
+                                                  host=url[0].split("/")[2],
+                                                  user=url[1],
+                                                  passwd=url[2])
+            
+            for iurl,isavedir in zip(urllist,savedirlist):
+                localpath , bool_dl = dlutils.FTP_downloader_full_remote_path(ftp_obj,
+                                                                              iurl[0],
+                                                                              isavedir)
+                
 
     localfiles_lis = []
     skiped_url = 0
-    for url , savedir in zip(urllist,savedirlist):
+    for url, savedir in zip(urllist, savedirlist):
         try:
-            localfile = os.path.join(savedir,os.path.basename(url))
+            if type(url) is tuple:
+                url0 = url[0]
+            else:
+                url0 = url
+            localfile = os.path.join(savedir, os.path.basename(url0))
             if os.path.isfile(localfile):
                 localfiles_lis.append(localfile)
-        except:
+        except Exception as e:
             # because of a weird error
             # i = p.rfind('/') + 1
             # AttributeError: 'tuple' object has no attribute 'rfind'
             skiped_url += 1
+            log.warning(e)
             continue
 
     pool.close()
-    log.debug(str(skiped_url) +  ' returned url skiped because of a weird error, but it is not important...')
-    return localfiles_lis , savedirlist
+    if skiped_url > 0:
+        log.debug(str(skiped_url) + ' returned url skipped because of an Exception')
+    return localfiles_lis, savedirlist
+
 
 #    return zip(urllist,savedirlist)
 
 
 def rnx_long2short_name(longname_filepath_in):
     """
     MUST BE IMPROVED
     """
-    
+
     longname_basename = os.path.basename(longname_filepath_in)
-    longname_dirname  = os.path.dirname(longname_filepath_in)
-    
+    longname_dirname = os.path.dirname(longname_filepath_in)
+
     Longname_basename_splitted = longname_basename.split("_")
-    
+
     datepart_str = Longname_basename_splitted[2]
     yyyy = datepart_str[:4]
-    ddd  = datepart_str[4:7]
+    ddd = datepart_str[4:7]
 
     shortname_basename = longname_basename[:4].lower() + ddd + "0." + yyyy[2:] + "o"
-    
-    return os.path.join(longname_dirname,shortname_basename)
 
-def multi_archiver_rinex(rinex_lis,parent_archive_dir,archtype='stat',
-                         move=True,force_mv_or_cp=True):
+    return os.path.join(longname_dirname, shortname_basename)
+
+
+def multi_archiver_rinex(rinex_lis, parent_archive_dir, archtype='stat',
+                         move=True, force_mv_or_cp=False):
     """
     from rinex_lis, a list of rinex (generated by the function
     multi_finder_rinex)
 
     move (if move=True) of copy (if move=False) those rinexs in the
     parent_archive_dir according to the archtype,
     string describing how the archive directory is structured, e.g :
@@ -477,36 +543,34 @@
             year/stat
 
             week/dow/stat
 
             ... etc ...
     """
 
-    mv_cnt   = 0
+    mv_cnt = 0
     skip_cnt = 0
-    log.info('RINEXs as input : %s' , len(rinex_lis))
+    log.info('RINEXs as input : %s', len(rinex_lis))
 
     if move:
         mv_fct = utils.move
     else:
         mv_fct = utils.copy2
 
     for rnx in rinex_lis:
         date = conv.rinexname2dt(rnx)
         rnxname = os.path.basename(rnx)
         stat = rnxname[0:4]
         savedir = effective_save_dir(parent_archive_dir, stat, date, archtype)
         utils.create_dir(savedir)
 
-        if not force_mv_or_cp and os.path.isfile(os.path.join(savedir,rnxname)):
+        if not force_mv_or_cp and os.path.isfile(os.path.join(savedir, rnxname)):
             skip_cnt += 1
             continue
         else:
-            mv_fct(rnx,savedir)
+            mv_fct(rnx, savedir)
             mv_cnt += 1
 
     log.info('RINEXs skiped :' + str(skip_cnt) + ' (because already exist)')
     log.info('RINEXs moved  :' + str(mv_cnt))
 
     return None
-
-
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/download_utils.py` & `geodezyx-4.4.2/geodezyx/operational/download_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 # import datetime as dt
-from ftplib import FTP
+from ftplib import FTP, FTP_TLS
 # import glob
 # import itertools
 # import multiprocessing as mp
 import os
 import pandas as pd 
 # import re
 import shutil
@@ -89,16 +89,16 @@
         ... etc ...
     """
     if archtype == '/':
         return parent_archive_dir
 
     out_save_dir = parent_archive_dir
     fff = archtype.split('/')
-    #year = str(date.year)
-    #doy = conv.dt2doy(date)
+    year = str(date.year)
+    doy = conv.dt2doy(date)
     week, dow = conv.dt2gpstime(date)
 
     for f in fff:
         if "wkwwww" in f:
             f_evaluated = "wk" + str(week).zfill(4)
         else:
             f_evaluated = eval(f)
@@ -130,73 +130,84 @@
     if type(url) is tuple:
         need_auth = True
         username = url[1]
         password = url[2]
         url = url[0]
     else:
         need_auth = False
-
+        username = ''
+        password = ''
+        
     url_print = str(url)
 
     rnxname = os.path.basename(url)
 
     Pot_compress_files_list = [os.path.join(savedir , rnxname)]
 
     if check_if_file_already_exists_uncompressed:
-        Pot_compress_files_list.append(os.path.join(savedir , rnxname.replace(".gz","")))
-        Pot_compress_files_list.append(os.path.join(savedir , rnxname.replace(".Z","")))
+        Pot_compress_files_list.append(os.path.join(savedir ,
+                                                    rnxname.replace(".gz","")))
+        Pot_compress_files_list.append(os.path.join(savedir ,
+                                                    rnxname.replace(".Z","")))
         Pot_compress_files_list = list(set(Pot_compress_files_list))
 
     for f in Pot_compress_files_list:
         if os.path.isfile(f) and (not force):
             log.info(os.path.basename(f) + " already exists locally ;)")
             return None
         
     ##### LOCAL FILE (particular case for GFZ)
     if os.path.isfile(url):
         log.info("INFO : downloader : the is a local file, a simple copy will be used")
         log.info("       URL : %s",url)
         shutil.copy(url,savedir)
     
     ##### REMOTE FILE (General case)
-    elif ("ftp" in url) or ("http" in url) :
+    elif ("http" in url)  or (("ftp" in url) and not need_auth):
         # managing a authentification
-        if need_auth:
-            if 'ftp://' in url: # FTP with Auth
-                url = url.replace('ftp://','ftp://' + username + ':' + password + '@')
-                opener = urllib.request.build_opener()
-            else: # HTTP with Auth
-                password_mgr = urllib.request.HTTPPasswordMgrWithDefaultRealm()
-                top_level_url = url
-                password_mgr.add_password(None, top_level_url, username, password)
-                handler = urllib.request.HTTPBasicAuthHandler(password_mgr)
-                # create "opener" (OpenerDirector instance)
-                opener = urllib.request.build_opener(handler)
+        if need_auth: # HTTP with Auth
+            password_mgr = urllib.request.HTTPPasswordMgrWithDefaultRealm()
+            top_level_url = url
+            password_mgr.add_password(None, top_level_url, username, password)
+            handler = urllib.request.HTTPBasicAuthHandler(password_mgr)
+            # create "opener" (OpenerDirector instance)
+            opener = urllib.request.build_opener(handler)
         else: # FTP or HTTP without Auth
             opener = urllib.request.build_opener()
     
         # use the opener to fetch a URL
         try:
             f = opener.open(url)
-        except (urllib.error.HTTPError , urllib.error.URLError):
+        except (urllib.error.HTTPError , urllib.error.URLError) as exp:
             log.warning("%s not found :(",rnxname)
             log.warning(url_print)
+            log.warning(exp)
             return ""
+        
         log.info("%s found, downloading :)",rnxname)
         data = f.read()
         if not os.path.exists(savedir):
             os.makedirs(savedir)
         outpath = os.path.join(savedir , rnxname)
         with open(outpath, "wb") as code:
             code.write(data)
         return_str = outpath
+        
+    elif (("ftp" in url) and need_auth):
+        log.critical("MUST BE IMPEMENTED")
+        return_str = ""
+
+
+        
+        
     else:
         log.error("something goes wrong with the URL")
         log.error(url)
         return_str = ""
+        
 
     return return_str
 
 
 def downloader_wrap(intup):
     downloader(*intup)
     return None
@@ -205,31 +216,83 @@
 #  ______ _______ _____    _____                      _                 _ 
 # |  ____|__   __|  __ \  |  __ \                    | |               | |
 # | |__     | |  | |__) | | |  | | _____      ___ __ | | ___   __ _  __| |
 # |  __|    | |  |  ___/  | |  | |/ _ \ \ /\ / / '_ \| |/ _ \ / _` |/ _` |
 # | |       | |  | |      | |__| | (_) \ V  V /| | | | | (_) | (_| | (_| |
 # |_|       |_|  |_|      |_____/ \___/ \_/\_/ |_| |_|_|\___/ \__,_|\__,_|
                                                                         
- 
-#### FTP DOWNLOAD                                                                                      
+
+#### FTP DOWNLOAD
+
+class MyFTP_TLS(FTP_TLS):
+    """Explicit FTPS, with shared TLS session"""
+    ### This new class is to avoid the error
+    ### ssl.SSLEOFError: EOF occurred in violation of protocol (_ssl.c:2396)
+    ### source:
+    ### https://stackoverflow.com/questions/14659154/ftps-with-python-ftplib-session-reuse-required
+    def ntransfercmd(self, cmd, rest=None):
+        conn, size = FTP.ntransfercmd(self, cmd, rest)
+        if self._prot_p:
+            conn = self.context.wrap_socket(conn,
+                                            server_hostname=self.host,
+                                            session=self.sock.session)  # this is the fix
+        return conn, size
+
+
 def _ftp_dir_list_files(ftp_obj_in):
     files = []
     try:
         files = ftp_obj_in.nlst()
     except ftplib.error_perm as resp:
         if str(resp) == "550 No files found":
             log.warning("No files in this directory" + ftp_obj_in.pwd())
         else:
             raise
     return files
 
 
-def ftp_files_crawler(urllist,savedirlist):
+def ftp_objt_create(secure_ftp_inp,host="",chdir="",
+                    parallel_download=1, 
+                    user="anonymous",passwd=""):
+    # define the right constructor
+    if secure_ftp_inp:
+        ftp_constuctor = MyFTP_TLS
+        #ftp=ftp_constuctor()
+        #ftp.set_debuglevel(2)
+        #ftp.connect(arch_center_main)
+        #ftp.login('anonymous','')
+        #ftp.prot_p()
+    else:     
+        ftp_constuctor = FTP
+        #ftp = ftp_constuctor(arch_center_main)
+        #ftp.login()
+        
+    ## create a list of FTP object for multiple downloads
+    Ftp_obj_list_out = [ftp_constuctor(host) for i in range(parallel_download)]
+    if secure_ftp_inp:
+        [f.login(user,passwd) for f in Ftp_obj_list_out]
+        [f.prot_p() for f in Ftp_obj_list_out]    
+    else:
+        [f.login() for f in Ftp_obj_list_out]    
+        
+    # define the main obj for crawling
+    ftp_main = Ftp_obj_list_out[0]
+    
+    # change the directory of the main ftp obj if we ask for it
+    if chdir:
+        log.info("Move to: %s",chdir)
+        ftp_main.cwd(chdir)
+    
+    return ftp_main, Ftp_obj_list_out
+
+
+
+def ftp_files_crawler(urllist,savedirlist,secure_ftp):
     """
-    filter urllist,savedirlist generated with multi_downloader_rinex with an
+    filter urllist,savedirlist generated with download_gnss_rinex with an
     optimized FTP crawl
 
     """
     ### create a DataFrame based on the urllist and savedirlist lists
     DF = pd.concat((pd.DataFrame(urllist),pd.DataFrame(savedirlist)),axis=1)
     DF_orig = DF.copy()
     
@@ -238,15 +301,15 @@
         loginftp = True 
         DF.columns = ('url','user','pass','savedir')
     else:
         loginftp = False
         DF.columns = ('url','savedir')
         DF['user'] = "anonymous"
         DF['pass'] = ""
-        
+                
     ### Do the correct split for the URLs
     DF = DF.sort_values('url')
     DF["url"]      = DF['url'].str.replace("ftp://","")
     DF["dirname"]  = DF["url"].apply(os.path.dirname)
     DF["basename"] = DF["url"].apply(os.path.basename)
     DF["root"]     = [e.split("/")[0] for e in DF["dirname"].values]
     DF["dir"]      = [e1.replace(e2,"")[1:] for (e1,e2) in zip(DF["dirname"],
@@ -255,27 +318,30 @@
     
     #### Initialisation of the 1st variables for the loop
     prev_row_ftpobj = DF.iloc[0]
     prev_row_cwd    = DF.iloc[0]
     FTP_files_list = []
     count_loop = 0  # restablish the connexion after 50 loops (avoid freezing)
     #### Initialisation of the FTP object
-    FTPobj = ftplib.FTP(prev_row_ftpobj.root,
-                        prev_row_ftpobj.user, 
-                        prev_row_ftpobj['pass'])
+        
+    FTPobj , _  = ftp_objt_create(secure_ftp_inp=secure_ftp,
+                                  host=prev_row_ftpobj.root,
+                                  user=prev_row_ftpobj.user,
+                                  passwd=prev_row_ftpobj['pass'])
     
     for irow,row in DF.iterrows():
         count_loop += 1
         
         ####### we recreate a new FTP object if the root URL is not the same
         if row.root != prev_row_ftpobj.root or count_loop > 20:
-    
-            FTPobj = ftplib.FTP(row.root,
-                                row.user, 
-                                row['pass'])
+            
+            FTPobj , _ = ftp_objt_create(secure_ftp_inp=secure_ftp,
+                                         host=prev_row_ftpobj.root,
+                                         user=prev_row_ftpobj.user,
+                                         passwd=prev_row_ftpobj['pass'])
             
             prev_row_ftpobj = row
             count_loop = 0
             
         ####### we recreate a new file list if the date path is not the same        
         if (prev_row_cwd.dir != row.dir) or irow == 0:
             log.info("chdir " + row.dirname)
@@ -311,33 +377,51 @@
     savedirlist_out = list(DFgood.savedir)
     
     return urllist_out, savedirlist_out
 
 def FTP_downloader(ftp_obj,filename,localdir):   
     localpath = os.path.join(localdir,filename)
     
+    if not os.path.isdir(localdir):
+        utils.create_dir(localdir)
+    
     if not utils.empty_file_check(localpath):
         log.info(filename + " already exists ;)")
         bool_dl = True
     else:
         try:
             localfile = open(localpath, 'wb')
             ftp_obj.retrbinary('RETR ' + filename, localfile.write, 1024)
             localfile.close()
             bool_dl = True
             log.info(filename + " downloaded :)")
     
-        except:
-            log.info(localpath + " download failed :(")
+        except Exception as e:
+            log.warning(localpath + " download failed :(")
+            log.warning(e)
             bool_dl = False
     
     return localpath , bool_dl
 
+def FTP_downloader_full_remote_path(ftp_obj,full_remote_path,localdir):   
+    
+    #host = full_remote_path[0].split("/")[2]          
+    
+    filename = os.path.basename(full_remote_path)
+    intermed_path = full_remote_path.split("/")[3:]
+    intermed_path.remove(filename)
+    intermed_path = "/" + "/".join(intermed_path)
+
+    ftp_obj.cwd(intermed_path)
+    
+    return FTP_downloader(ftp_obj, filename, localdir)
+
 def FTP_downloader_wo_objects(tupin):
     arch_center_main,wwww_dir,filename,localdir = tupin
     ftp_obj_wk = FTP(arch_center_main)
     ftp_obj_wk.login()
     ftp_obj_wk.cwd(wwww_dir)
     localpath , bool_dl = FTP_downloader(ftp_obj_wk,filename,localdir)
     ftp_obj_wk.close()
     return localpath , bool_dl
     
+
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/gins_runner.py` & `geodezyx-4.4.2/geodezyx/operational/gins_runner.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/groops_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/groops_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/hector_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/hector_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/midas_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/midas_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/rinex_lister_plotter.py` & `geodezyx-4.4.2/geodezyx/operational/rinex_lister_plotter.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/rinex_utils.py` & `geodezyx-4.4.2/geodezyx/operational/rinex_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/operational/rtklib_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/rtklib_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,20 +171,20 @@
     sp3Z = orblis[0]
     sp3 = utils.uncompress(sp3Z)
 
     # BRDC
     statdic = dict()
     statdic['nav'] = ['BRDC']
     nav_srt = dt.datetime(bas_srt.year, bas_srt.month , bas_srt.day )
-    orblis = operational.multi_downloader_rinex(statdic,
-                                                temp_dir,
-                                                nav_srt,
-                                                bas_end ,
-                                                archtype='/',
-                                                sorted_mode=False)
+    orblis = operational.download_gnss_rinex(statdic,
+                                             temp_dir,
+                                             nav_srt,
+                                             bas_end,
+                                             archtype='/',
+                                             sorted_mode=False)
     navZ = orblis[0]
     nav = utils.uncompress(navZ)
 
     # Command
     com_config  = "-k " + out_conf_fil
     com_interval="-ti " + str(rov_itv)
     com_mode = ""
```

### Comparing `geodezyx-4.4.1/geodezyx/operational/track_frontend.py` & `geodezyx-4.4.2/geodezyx/operational/track_frontend.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/reffram/geometry.py` & `geodezyx-4.4.2/geodezyx/reffram/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,40 +470,43 @@
     """
     estimates 7 parameters of a 3D Helmert transformation between a set of points
     X1 and a set of points X2 (compute transformation X1 => X2)
     
     Parameters
     ----------
     
-    X1list & X2list : list of N (x,y,z) points, or an (N,3)-shaped numpy array
-        Input point sets
+    X1list & X2list : list or np.array
+        Input point set
+        list of N (x,y,z) points, or an (N,3)-shaped numpy array
 
     Weights : list of N Weights,
         or an numpy array of shape (N,)
     
     Returns
     -------
     
     HParam :
         7 Helmert params. : x,y,z translations, x,y,z rotations, scale
+        translations are given in meters, rotations in arcsec, 
+        scale in unitless ratio
     A :
         Design matrix    
     l :
         Differences X2 - X1 (before transformation !!!)
         
     References
     ----------
     https://elib.uni-stuttgart.de/bitstream/11682/9661/1/BscThesis_GaoYueqing.pdf
     """
 
     l_stk = []
     A_stk = []
     Bool_stk = []
     
-    log.error("we have %s points",len(X1list))
+    log.info("we have %s points",len(X1list))
     
     for X1 , X2 in zip(X1list , X2list):
         
         if np.sum(np.isnan(X1)) or np.sum(np.isnan(X2)):
             log.warning("one point component is nan, skipping")
             Bool_stk.append(False)
             continue
@@ -537,16 +540,17 @@
 def helmert_trans_apply(Xin,SevenParam_in,legacy_mode=False):
     """
     Apply an Helmert transformation (7-parameters)
     to a set of points
 
     Parameters
     ----------
-    Xin : list of N (x,y,z) points, or an (N,3)-shaped numpy array.
-        input set points
+    Xin : list or np.array
+        input point set 
+        list of N (x,y,z) points, or an (N,3)-shaped numpy array.
         
     SevenParam_in : 7 element list or array
         7 Helmert params. : x,y,z translations, x,y,z rotations, scale.
         
     legacy_mode : bool, optional
         Use a non-optimized and slow computation approach (but same result).
         This option should be removed in the Future.
@@ -592,18 +596,20 @@
     estimates 7 parameters of a 3D Helmert transformation between a set of points
     X1 and a set of points X2 (compute transformation X1 => X2) 
     using a Minimization approach (and not a Least Square inversion)
     
     Parameters
     ----------
     
-    X1in & X2in : list of N (x,y,z) points, or an (N,3)-shaped numpy array
-        Input point sets
+    X1in & X2in :  list or np.array
+        Input point set
+        list of N (x,y,z) points, or an (N,3)-shaped numpy array
 
-    HParam_apri : list of 7 values,
+    HParam_apri : list 
+        list of 7 values,
         The Apriori for the Helmert parameter 
     
     L1norm : bool
         Use the L1-norm as a criteria, use the quadratic sum instead if False
         
     tol : float
         tolerence for the convergence
@@ -616,14 +622,16 @@
         see scipy.optimize.minimize for details
         The default is "Powell".
     
     Returns
     -------
     Res :
         7 Helmert params. : x,y,z translations, x,y,z rotations, scale
+        translations are given in meters, rotations in arcsec, 
+        scale in unitless ratio
     """
     
     def minimiz_helmert_fct(HParam_mini_in,X1in,X2in,L1norm_mini=L1norm):
         """
         This fct is the input for the scipy optimization fct
         """
         HParam_mini_wk = HParam_mini_in.copy()
```

### Comparing `geodezyx-4.4.1/geodezyx/reffram/gnss_products.py` & `geodezyx-4.4.2/geodezyx/reffram/gnss_products.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,22 +26,25 @@
 import matplotlib.pyplot as plt
 import natsort
 import numpy as np
 import os 
 import pandas as pd
 import re
 
+import pyorbital.astronomy
+
 ### disabled and imported directly in the needed fct
 ## import geodezyx.reffram.sofa18 as sofa
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
 from geodezyx import stats
 from geodezyx import utils
+from geodezyx.reffram import kepler_gzyx
 
 #### Import the logger
 import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
@@ -1058,14 +1061,233 @@
 # | |  | | '__| '_ \| | __| | |  | |/ _` | __/ _` |  __| '__/ _` | '_ ` _ \ / _ \/ __|
 # | |__| | |  | |_) | | |_  | |__| | (_| | || (_| | |  | | | (_| | | | | | |  __/\__ \
 #  \____/|_|  |_.__/|_|\__| |_____/ \__,_|\__\__,_|_|  |_|  \__,_|_| |_| |_|\___||___/
 #                                                                                     
        
 ### Orbit DataFrames   
 
+
+def DFOrb_velocity_calc(DFOrb_in,
+                        drop_nan=False):
+    """
+    Compute the velocity of satellites from a DFOrb dataframe
+    (differentiate the position)
+
+    Parameters
+    ----------
+    DFOrb_in : Pandas DataFrame
+        an Orbit DataFrame.
+    drop_nan : bool, optional
+        Remove the nan values 
+        (the first ones, since it is a numerical differentiation).
+        The default is False.
+        It is recommended to keep the NaN values, thus the output will keep
+        same size and index as input
+
+    Returns
+    -------
+    df_vel : Pandas DataFrame
+        an Orbit DataFrame with velocities (vx, vy ,vz columns).
+
+    """
+    
+    dfgrp = DFOrb_in.groupby('prn')
+    
+    dfprn_stk = []
+    for prn,dfprn in dfgrp:    
+        for coord in ['x','y','z']:
+            dcoord = dfprn[coord].diff()
+            dtime = (np.float64(dfprn['epoch'].diff()) * 10**-9) 
+            #timedelta in ns per defalut
+            dfprn['v' + coord] = dcoord / dtime 
+        dfprn_stk.append(dfprn)
+            
+    df_vel = pd.concat(dfprn_stk)
+    
+    df_vel.sort_index(inplace=True)
+    
+    if drop_nan:
+        df_vel.dropna(inplace=True)
+    
+    return df_vel 
+
+
+def beta_sun_ra_dec(sun_dec,sun_ra,sat_i,sat_o_lan):
+    """
+    Compute beta angle based on Sun's right ascension and declination
+    Angles are in radians
+
+    Parameters
+    ----------
+    sun_dec : float
+        Sun's declination.
+    sun_ra : float
+        Sun's right ascension.
+    sat_i : float
+        Satellite's inclination.
+    sat_o_lan : float
+        Satellite's Longitude of the ascending node.
+
+    Returns
+    -------
+    beta : float
+        beta angle (in radians).
+        
+    Source
+    ------
+    `Satellites: de Kepler au GPS`, Michel Capderou (2012)
+    
+    simpler formula here:
+        https://www.fxsolver.com/browse/formulas/Beta+Angle
+        
+    
+    Note
+    ----
+    you can use ``pyorbital.astronomy.sun_ra_dec()`` to compute ``sun_dec``
+    and ``sun_ra``
+    
+    If so, Sun's right ascension and declination computation polynoms are 
+    based on: `Astronomical algorithms`, Jean Meeus (1st edition, 1991)
+    """
+    beta = np.arcsin(np.cos(sun_dec)*np.sin(sat_i)*np.sin(sat_o_lan-sun_ra)+
+                     np.sin(sun_dec)*np.cos(sat_i))
+    return beta
+
+def beta_sun_eclip_long(sun_ecl_long,sat_o_lan,sat_i,earth_i):
+    """
+    Compute beta angle based on Sun's Ecliptic longitude
+    Angles are in radians
+
+    Parameters
+    ----------
+    sun_ecl_long : float
+        Sun's Ecliptic longitude.
+    sat_i : float
+        Satellite's inclination.
+    sat_o_lan : float
+        Satellite's Longitude of the ascending node.
+    earth_i : float
+        Earth's inclination.
+
+    Returns
+    -------
+    beta : float
+        beta angle (in radians).
+        
+    Source
+    ------
+    `Calculation of the Eclipse Factor for Elliptical Satellite Orbits` NASA (1962)
+    https://ntrs.nasa.gov/citations/19630000622
+    `Computation of Eclipse Time for Low-Earth Orbiting Small Satellites` Sumanth R M (2019)
+    https://commons.erau.edu/ijaaa/vol6/iss5/15/
+
+    Simpler formula:
+        https://en.wikipedia.org/wiki/Beta_angle
+    
+    Note
+    ----
+    you can use ``pyorbital.astronomy.sun_ecliptic_longitude()``
+    to compute ``sun_ecl_long``
+    
+    If so, Sun's right ascension and declination computation polynoms are 
+    based on: `Astronomical algorithms`, Jean Meeus (1st edition, 1991)
+
+    """
+    p1 = np.cos(sun_ecl_long)*np.sin(sat_o_lan)*np.sin(sat_i)
+    p2 = np.sin(sun_ecl_long)*np.cos(earth_i)*np.cos(sat_o_lan)*np.sin(sat_i)
+    p3 = np.sin(sun_ecl_long)*np.sin(earth_i)*np.cos(sat_i)
+    beta = np.arcsin(p1-p2+p3)
+    return beta
+
+def beta_angle_calc(DFOrb_in,
+                    calc_beta_sun_ra_dec=True,
+                    calc_beta_sun_eclip_long=True,
+                    beta_rad2deg=True):
+    """
+    Compute beta angle for GNSS satellite's orbits stored in an orbit 
+    DataFrame
+    
+
+    Parameters
+    ----------
+    DFOrb_in : Pandas DataFrame
+        an Orbit DataFrame (ECEF frame).
+    calc_beta_sun_ra_dec : bool, optional
+        compute beta angle with Sun's right ascension and declination.
+        The default is True.
+    calc_beta_sun_eclip_long : bool, optional
+        compute beta angle with Sun's Ecliptic longitude.
+        The default is True.
+    beta_rad2deg : bool, optional
+        convert beta angle to degrees. The default is True.
+
+    Returns
+    -------
+    df_out : Pandas DataFrame
+        DFOrb_in with a new 'beta' column.
+    df_wrk : Pandas DataFrame
+        intermediate values dataframe for debug.
+        here, coordinates are in ECI frame
+    """
+    
+    #### convert in ECI
+    df_eci = DFOrb_in.copy()
+    df_eci[['x','y','z']] = conv.ECEF2ECI(DFOrb_in[['x','y','z']].values,
+                                          DFOrb_in['epoch'].values)
+    
+    #### compute velocity
+    df_wrk = DFOrb_velocity_calc(df_eci,drop_nan=False)
+    ##keep drop nan False, thus the DF will keep same size and index as input
+    
+    #### compute Kepler's parameters
+    p = df_wrk[['x','y','z']].values * 1000
+    v = df_wrk[['vx','vy','vz']].values * 1000
+    
+    kep_col = ['a','ecc','i','o_peri','o_lan','m']
+    kep_params = kepler_gzyx.ECI_2_kepler_elts(p,v,rad2deg=False)
+    df_wrk[kep_col] = np.column_stack(kep_params)
+    ######### COMPUTE BETA
+    
+    #### cosmetic changes
+    if calc_beta_sun_ra_dec and calc_beta_sun_eclip_long:
+        b1="1"
+        b2="2"
+    else:
+        b1=""
+        b2=""    
+    
+    if beta_rad2deg:
+        r2dfct = np.rad2deg
+    else:
+        r2dfct = lambda x:x 
+    
+    ##### Beta computed based on sun declination / right ascension
+    if calc_beta_sun_ra_dec:
+        ##### sun_ra_dec output in RADIANS
+        df_wrk[['sun_ra','sun_dec']] = np.column_stack(pyorbital.astronomy.sun_ra_dec(df_wrk['epoch']))
+        df_wrk['beta'+b1] = beta_sun_ra_dec(df_wrk['sun_dec'], 
+                                            df_wrk['sun_ra'],
+                                            df_wrk['i'],
+                                            df_wrk['o_lan']).apply(r2dfct)
+        
+    ##### Beta computed based on Ecliptic longitude of the sun  
+    if calc_beta_sun_eclip_long:
+        ### sun_ecliptic_longitude output in RADIANS but NO MODULO !!!
+        df_wrk['sun_ecl_long'] = np.mod(pyorbital.astronomy.sun_ecliptic_longitude(df_wrk['epoch']),np.pi*2)
+        df_wrk['beta'+b2] = beta_sun_eclip_long(df_wrk['sun_ecl_long'],
+                                                df_wrk['o_lan'],
+                                                df_wrk['i'],
+                                                np.deg2rad(23.45)).apply(r2dfct)
+    df_out = DFOrb_in.copy()
+    df_out['beta'] = df_wrk['beta'+b1]
+
+    return df_out, df_wrk
+
+
+
 def OrbDF_lagrange_interpolate(DForb_in,Titrp,n=10,
                                append_to_input_DF = False,
                                plot=False):
     """
     High level function to interpolate an orbit DataFrame
 
     Parameters
```

### Comparing `geodezyx-4.4.1/geodezyx/reffram/kepler_gzyx.py` & `geodezyx-4.4.2/geodezyx/reffram/kepler_gzyx.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,35 +31,168 @@
 #### Import the logger
 import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
-def ECI_2_kepler_elts(P,V,rad2deg=True,
+def ECI_2_kepler_elts(pos,vel,rad2deg=True,
                       mu=3.9860044188e14):
     """
     Convert ECI coordinates > Kepler's elements
 
     Parameters
     ----------
+    pos : array
+        Position in m. 
+        Can be a 3-element (x,y,z) array (simple point) 
+        or a (N,3)-shaped numpy array
+    vel : array
+        Velocity in m/s.
+        Can be a 3-element (vx,vy,vz) array (simple point) 
+        or a (N,3)-shaped numpy array
+    rad2deg : bool, optional
+        convert Keplerian's angles (anomalies) to deg. The default is True.
+    mu : float, optional
+        Standard gravitational parameter. The default is 3.9860044188e14.
+
+    Returns
+    -------
+    a,ecc,i,o_peri,o_lan,m: floats
+        Kepler's elements:  
+            
+        * a : semi-major axis
+        * ecc : orbit eccentricity
+        * i : orbit inclination
+        * o_peri : argument of periapsis ω
+        * o_lan : longitude of the ascending node Ω
+        * m : mean anomaly m
+
+    Note
+    ----
+    Be sure your input is in ECI (SP3 are in ECEF for instance).  
+
+    If neeeded, use ``conv.ECEF2ECI()`` (gross results) 
+    or ``reffram.OrbDF_crf2trf(inv_trf2crf=True)`` (precise results)
+    
+    You can get the velocity with ``reffram.DFOrb_velocity_calc()``
+    
+    Source
+    ------
+    https://downloads.rene-schwarz.com/download/M002-Cartesian_State_Vectors_to_Keplerian_Orbit_Elements.pdf
+
+    """
+    p = np.array(pos)
+    v = np.array(vel)
+    
+    #### case for one point only
+    if len(p.shape) < 2:
+        p = np.expand_dims(p,axis=-1).T
+    if len(v.shape) < 2:
+        v = np.expand_dims(v,axis=-1).T
+        
+    pnorm = np.linalg.norm(p,axis=1)
+    vnorm = np.linalg.norm(v,axis=1)
+    
+    ### orbital momentum vector h
+    h = np.cross(p,v)
+    hnorm = np.linalg.norm(h,axis=1)
+    
+    ### eccentricity vector eccvec & orbit eccentricity ecc
+    eccvec = (np.cross(v,h)/mu) - (p/np.expand_dims(pnorm,axis=-1))
+    ecc = np.linalg.norm(eccvec,axis=1)
+    
+    ### true anomaly ν (nu)
+    n = np.cross(np.array([0,0,1]),h)
+    nnorm = np.linalg.norm(n,axis=1)
+    
+    dot_pv_sup0 = np.einsum('ij,ij->i',p,v) >= 0
+    nu_sup0 = np.arccos(np.einsum('ij,ij->i',eccvec,p)/(ecc*pnorm))
+    nu_inf0 = 2*np.pi - nu_sup0
+        
+    nu = np.zeros(len(dot_pv_sup0))
+    nu = nu + nu_sup0 * dot_pv_sup0
+    nu = nu + nu_inf0 * np.logical_not(dot_pv_sup0)
+    
+    ### orbit inclination i
+    i = np.arccos(h[:,2]/hnorm)
+
+    ### eccentric anomaly E (called e here)
+    #e1 = 2*np.arctan(np.tan(nu/2)/np.sqrt((1+ecc)/(1-ecc)))
+    e2 = 2*np.arctan2(np.tan(nu/2),np.sqrt((1+ecc)/(1-ecc)))
+    e=e2
+    
+    ### longitude of the ascending node Ω (o_lan)
+    n1_sup0 = n[:,1] >= 0
+        
+    omega_lan_sup0 = np.arccos(n[:,0]/nnorm)
+    omega_lan_inf0 = 2*np.pi - omega_lan_sup0
+    
+    o_lan = np.zeros(len(n1_sup0))
+    o_lan = o_lan + omega_lan_sup0 * n1_sup0
+    o_lan = o_lan + omega_lan_inf0 * np.logical_not(n1_sup0)
+    
+    ### argument of periapsis ω (o_peri)
+    eccvec2_sup0 = eccvec[:,2] >= 0
+    o_peri_sup0 = np.arccos((np.einsum('ij,ij->i',n, eccvec))/(ecc*nnorm))
+    o_peri_inf0 = 2 * np.pi - o_peri_sup0
+    
+    o_peri = np.zeros(len(eccvec2_sup0))
+    o_peri = o_peri + o_peri_sup0 * eccvec2_sup0
+    o_peri = o_peri + o_peri_inf0 * np.logical_not(eccvec2_sup0)
+    
+    ### mean anomaly m, (Kepler’s Equation)
+    m = e - ecc*np.sin(e)
+    
+    ### semi-major axis a
+    a = ((2/pnorm) - (vnorm**2 / mu))**-1
+
+    #### case for one point only (bring it back to a scalar)
+    sqzflt = lambda x: np.float64(x.squeeze())
+
+    a = sqzflt(a)
+    ecc = sqzflt(ecc)
+    i = sqzflt(i)
+    o_lan = sqzflt(o_lan)
+    o_peri = sqzflt(o_peri)
+    m = sqzflt(m)
+
+    if rad2deg:
+        i=np.rad2deg(i)
+        o_peri=np.rad2deg(o_peri)
+        o_lan=np.rad2deg(o_lan)
+        m=np.rad2deg(m)
+        
+    #### o_peri and m seems to be inverted, must be investigated!!!
+    return a,ecc,i,o_peri,o_lan,m
+
+def ECI_2_kepler_elts_mono(P,V,rad2deg=True,
+                           mu=3.9860044188e14):
+    """
+    **Kept for debug purposes, use** ``ECI_2_kepler_elts(pos, vel)`` **instead**
+    
+    Convert ECI coordinates > Kepler's elements
+
+    Parameters
+    ----------
     P : array
         Position.
     V : array
         Velocity.
     rad2deg : bool, optional
         canvert Keplerian's angles (anomalies) to deg. The default is True.
     mu : float, optional
         Standard gravitational parameter. The default is 3.9860044188e14.
 
     Returns
     -------
     a,ecc,i,omega_periarg,omega_LAN,m : floats
         Kepler's elements.
     """
+    log.warning('use this function for debug purposes only, use ECI_2_kepler_elts instead')
     Pnorm = np.linalg.norm(P)
     Vnorm = np.linalg.norm(V)
     
     ### orbital momentum vector H
     H = np.cross(P,V)
     Hnorm = np.linalg.norm(H)
     
@@ -108,16 +241,14 @@
         i=np.rad2deg(i)
         omega_periarg=np.rad2deg(omega_periarg)
         omega_LAN=np.rad2deg(omega_LAN)
         m=np.rad2deg(m)
 
     return a,ecc,i,omega_periarg,omega_LAN,m
 
-
-
 def extrapolate_orbit_kepler(P,V,t,t0,mu=3.9860044188e14):
     orbit = TwoBodyOrbit("", mu=mu)   # create an instance
     orbit.setOrbCart(t0, P, V)        # define the orbit
     Pout, Vout = orbit.posvelatt(t)   # get position and velocity at t1
     kepl = orbit.elmKepl()            # get classical orbital elements
     
     return Pout,Vout,kepl
```

### Comparing `geodezyx-4.4.1/geodezyx/reffram/quaternions.py` & `geodezyx-4.4.2/geodezyx/reffram/quaternions.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/stats/least_squares.py` & `geodezyx-4.4.2/geodezyx/stats/least_squares.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/stats/stats.py` & `geodezyx-4.4.2/geodezyx/stats/stats.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/time_series/ts_class.py` & `geodezyx-4.4.2/geodezyx/time_series/ts_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1316,14 +1316,25 @@
             pts_stk = []
             i_stk = []
             for i,p in enumerate(self.pts):
                 if np.abs(p.T - tin) < tol:
                     pts_stk.append(p)
                     i_stk.append(i)
             return pts_stk  , i_stk
+        
+    def remove_duplicate_pts(self,coortype="XYZ"):
+        T = self.to_dataframe(coortype)["T"] 
+        
+        dup_bool = T.duplicated()
+        
+        if dup_bool.sum() > 0:
+            log.warn("%s duplicated point(s) removed for %s",
+                     dup_bool.sum(), self.name)
+            
+        self.pts = list(pd.Series(self.pts)[np.logical_not(dup_bool)])
     
     
     
 
 
  #  ______                      _                      _        _    _____ _                         
  # |  ____|                    (_)                    | |      | |  / ____| |
```

### Comparing `geodezyx-4.4.1/geodezyx/time_series/ts_export.py` & `geodezyx-4.4.2/geodezyx/time_series/ts_export.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/time_series/ts_fcts.py` & `geodezyx-4.4.2/geodezyx/time_series/ts_fcts.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,14 +545,16 @@
                            python_dt_out=True)
 
     tsout.bool_interp_uptodate = False
     
     for pt,t in zip(tsout,Tdtout):
         pt.Tset(conv.numpy_dt2dt(t))
         
+    tsout.remove_duplicate_pts(tsin.initype())
+        
     tsout.interp_set()
         
     return tsout
 
 def mad_cleaner(tsin,seuil=3.5,method='dist',coortype='ABC',
                 detrend_first=False,output_detrended=False, verbose=False):
     '''
@@ -822,35 +824,56 @@
     T = ((np.max(Tlis) - np.min(Tlis)) / 2.) + np.min(Tlis)
     pt = time_series.Point(E,N,U,T,'ENU',sE,sN,sU,ptslisin[0].name)
 
     return pt
 
 
 def merge(tsin,N):
-    """ merge N points in one """
+    """ 
+    merge N points in one
+    """
     tsin.sort()
     tsout = copy.deepcopy(tsin)
     tsout.del_data()
     slic = utils.sliceIt(tsin.pts,N)
     for sl in slic:
         pt = mean_list_of_pts(sl)
         tsout.add_point(pt)
     tsout.interval_nominal()
     return tsout
 
 def merge_ts(ts_list_in):
+    """
+    Merge several TimeSeriePoint into one
+
+    Parameters
+    ----------
+    ts_list_in : list of TimeSeriePoint
+        list of TimeSeriePoint.
+
+    Returns
+    -------
+    ts_out : TimeSeriePoint
+        merged TimeSeriePoint.
+
+    """
     pts_list_merged = []
+    boolENU_stk = []
     for ts in ts_list_in:
         pts_list_merged = pts_list_merged + ts.pts
+        boolENU_stk.append(ts.boolENU)
 
     ts_out = time_series.TimeSeriePoint()
     ts_out.pts = pts_list_merged
     ts_out.anex = ts_list_in[0].anex
+    ts_out.boolENU = np.all(boolENU_stk)
     ts_out.interval_nominal()
+    ts_out.stat = ts_list_in[0].stat
     ts_out.sort()
+
     return ts_out
 
 
 def time_win(tsin,windows,mode='keep',outbool=False):
     if type(windows[0][0]) == dt.datetime:
         Ttype = 'Tdt'
     else:
```

### Comparing `geodezyx-4.4.1/geodezyx/utils/dict_utils.py` & `geodezyx-4.4.2/geodezyx/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/utils/list_utils.py` & `geodezyx-4.4.2/geodezyx/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/utils/pandas_utils.py` & `geodezyx-4.4.2/geodezyx/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/utils/plot_utils.py` & `geodezyx-4.4.2/geodezyx/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/geodezyx/utils/shell_like.py` & `geodezyx-4.4.2/geodezyx/utils/shell_like.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,19 @@
 
 def tail(filename, count=1, offset=1024):
     """
     A more efficent way of getting the last few lines of a file.
     Depending on the length of your lines, you will want to modify offset
     to get better performance.
     """
+    
     f_size = os.stat(filename).st_size
     if f_size == 0:
         return []
-    with open(filename, 'r') as f:
+    with open(filename, 'r',errors='ignore') as f:
         if f_size <= offset:
             offset = int(f_size / 2)
         while True:
             seek_to = min(f_size - offset, 0)
             f.seek(seek_to)
             lines = f.readlines()
             # Empty file
@@ -114,15 +115,21 @@
                 return lines[count * -1:]
 
 def head(filename, count=1):
     """
     This one is fairly trivial to implement but it is here for completeness.
     """
     with open(filename, 'r') as f:
-        lines = [f.readline() for line in range(1, count+1)]
+        lines = []
+        for iline in range(1, count+1):
+            try:
+                lines.append(f.readline())
+            except Exception as e:
+                log.warn(e)
+                continue
         return list(filter(len, lines))
 
 
 
 def grep(file_in,search_string,only_first_occur=False,
          invert=False,regex=False,line_number=False,col=(None,None),
          force_list_output=False):
@@ -378,16 +385,16 @@
                 continue
                 
             matches_ext.append((f,stat))
         matches = matches_ext
         
     if warn_if_empty and len(matches) == 0:
         log.warning("no files found! check parent folder and pattern")
-        log.info("Parent folder  :%s",parent_folder)
-        log.info("Pattern        :%s",pattern)
+        log.info("Parent folder: %s",parent_folder)
+        log.info("Pattern      : %s",pattern)
                 
     return matches
 
 def glob_smart(dir_path,file_pattern=None,verbose=True):
     if file_pattern:
         dir_path_ok = os.join.path(dir_path,file_pattern)
     else:
```

### Comparing `geodezyx-4.4.1/geodezyx/utils/utils_core.py` & `geodezyx-4.4.2/geodezyx/utils/utils_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,17 @@
     Check if the code is run inside Spyder IDE
     """
     if any('SPYDER' in name for name in os.environ):
         return True
     else:
         return False
 
-def is_iterable(inp,consider_str_as_iterable=False):
+def is_iterable(inp,
+                consider_str_as_iterable=False,
+                consider_dict_as_iterable=False):
     """
     Test if the input is an iterable like a list or a numpy array or not
 
     Parameters
     ----------
     inp : list, numpy.array, ...
 
@@ -83,14 +85,17 @@
     -------
     out : bool
         True if inp is iterable, False either
     """
     if not consider_str_as_iterable and type(inp) is str:
         return False
 
+    if not consider_dict_as_iterable and type(inp) is dict:
+        return False
+
     try:
         iter(inp)
     except TypeError:
         out = False
     else:
         out = True
     return out
@@ -898,20 +903,22 @@
         return list(string.ascii_lowercase)
     else:
         return alphabet_reverse().index(letter)
 
 
 def dday():
     """
-    Give the time span between prensent and toolbox author's PhD defense
+    Give the time span between present and toolbox author's PhD defense date
+    
     (tests also the console messages)
         
     Note
     ----
     https://fr.wiktionary.org/wiki/quille#Dérivés_2
+    
     https://en.wiktionary.org/wiki/quille
 
     Returns
     -------
     D : datetime
         elapsed time.
```

### Comparing `geodezyx-4.4.1/geodezyx.egg-info/PKG-INFO` & `geodezyx-4.4.2/geodezyx.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 4.4.1
-Summary: The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.
-Home-page: https://github.com/IPGP/geodezyx-toolbox
+Version: 4.4.2
+Summary: geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.
+Home-page: https://github.com/IPGP/geodezyx
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -42,23 +42,23 @@
 Requires-Dist: wheel
 Requires-Dist: xarray
 Provides-Extra: full
 Requires-Dist: netCDF4; extra == "full"
 Requires-Dist: kepler.py; extra == "full"
 Requires-Dist: ncompress; extra == "full"
 
-The purpose of this GeodeZYX toolbox is to provide all the functions which
+geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide all the functions which
 can be useful for Geodesy and Geophysics. 
 
 It includes low level functions, file management functions,
 time and space-coordinates conversion functions, 
 data (especially GNSS observations and orbits) retrieve functions, 
 plots and visual selection functions ...
 
 It is designed for Python 3 on a LINUX Ubuntu-like system.
 Also tested with Anaconda
 
-Documentation: https://geodezyx.github.io/geodezyx-toolbox  
+Documentation: https://ipgp.github.io/geodezyx  
 
-GitHub repository: https://github.com/IPGP/geodezyx-toolbox 
+GitHub repository: https://github.com/IPGP/geodezyx 
 
 PyPi project: https://pypi.org/project/geodezyx
```

### Comparing `geodezyx-4.4.1/geodezyx.egg-info/SOURCES.txt` & `geodezyx-4.4.2/geodezyx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 geodezyx/operational/download_prods.py
 geodezyx/operational/download_rinex.py
 geodezyx/operational/download_utils.py
 geodezyx/operational/gins_runner.py
 geodezyx/operational/groops_frontend.py
 geodezyx/operational/hector_frontend.py
 geodezyx/operational/midas_frontend.py
+geodezyx/operational/pride_pppar_frontend.py
 geodezyx/operational/rinex_lister_plotter.py
 geodezyx/operational/rinex_utils.py
 geodezyx/operational/rtklib_frontend.py
 geodezyx/operational/track_frontend.py
 geodezyx/reffram/__init__.py
 geodezyx/reffram/geometry.py
 geodezyx/reffram/gnss_products.py
```

### Comparing `geodezyx-4.4.1/misc/import_generic.py` & `geodezyx-4.4.2/misc/import_generic.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/misc/refactoring.py` & `geodezyx-4.4.2/misc/refactoring.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.1/setup.py` & `geodezyx-4.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,43 +33,43 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='4.4.1',  # Required
+    version='4.4.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='The GeodeZYX toolbox aims to provide simple but useful functions for Geodesy and Geophysics.',  # Optional
+    description='geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
-    long_description="""The purpose of this GeodeZYX toolbox is to provide all the functions which
+    long_description="""geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide all the functions which
 can be useful for Geodesy and Geophysics. 
 
 It includes low level functions, file management functions,
 time and space-coordinates conversion functions, 
 data (especially GNSS observations and orbits) retrieve functions, 
 plots and visual selection functions ...
 
 It is designed for Python 3 on a LINUX Ubuntu-like system.
 Also tested with Anaconda
 
-Documentation: https://geodezyx.github.io/geodezyx-toolbox  
+Documentation: https://ipgp.github.io/geodezyx  
 
-GitHub repository: https://github.com/IPGP/geodezyx-toolbox 
+GitHub repository: https://github.com/IPGP/geodezyx 
 
 PyPi project: https://pypi.org/project/geodezyx
 """,  # Optional
 
     # Denotes that our long_description is in Markdown; valid values are
     # text/plain, text/x-rst, and text/markdown
     #
@@ -82,15 +82,15 @@
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
     # long_description_content_type='text/markdown',  # Optional (see note above)
     long_description_content_type='text/x-rst',  # Optional (see note above)
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url='https://github.com/IPGP/geodezyx-toolbox',  # Optional
+    url='https://github.com/IPGP/geodezyx',  # Optional
 
     # This should be your name or the name of the organization which owns the
     # project.
     author='Pierre Sakic & Gustavo Mansur',  # Optional
 
     # This should be a valid email address corresponding to the author listed
     # above.
@@ -239,10 +239,10 @@
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     #project_urls={  # Optional
     #    'Bug Reports': 'https://github.com/pypa/sampleproject/issues',
     #    'Funding': 'https://donate.pypi.org',
     #    'Say Thanks!': 'http://saythanks.io/to/example',
-    #    'Source': 'https://github.com/IPGP/geodezyx-toolbox' #,
+    #    'Source': 'https://github.com/IPGP/geodezyx' #,
     #}
 )
```

