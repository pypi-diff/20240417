# Comparing `tmp/tvb-contrib-2.8.2.tar.gz` & `tmp/tvb-contrib-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-contrib-2.8.2.tar", last modified: Tue Sep 19 14:12:28 2023, max compression
+gzip compressed data, was "tvb-contrib-2.9.tar", last modified: Fri Apr 12 19:21:39 2024, max compression
```

## Comparing `tvb-contrib-2.8.2.tar` & `tvb-contrib-2.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.585169 tvb-contrib-2.8.2/
--rw-r--r--   0 root         (0) root         (0)    36777 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1778 2023-09-19 14:12:28.584169 tvb-contrib-2.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1256 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 14:12:28.585169 tvb-contrib-2.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2216 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.203171 tvb-contrib-2.8.2/tvb/
--rw-r--r--   0 root         (0) root         (0)     1363 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.203171 tvb-contrib-2.8.2/tvb/contrib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.267171 tvb-contrib-2.8.2/tvb/contrib/cosimulation/
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/cosimulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3918 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosim_history.py
--rw-r--r--   0 root         (0) root         (0)    10127 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosim_monitors.py
--rw-r--r--   0 root         (0) root         (0)    18267 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosimulator.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/cosimulation/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.290171 tvb-contrib-2.8.2/tvb/contrib/from_articles/
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py
--rw-r--r--   0 root         (0) root         (0)     6259 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py
--rw-r--r--   0 root         (0) root         (0)     6068 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py
--rw-r--r--   0 root         (0) root         (0)     7195 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py
--rw-r--r--   0 root         (0) root         (0)     7440 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py
--rw-r--r--   0 root         (0) root         (0)     6542 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.292171 tvb-contrib-2.8.2/tvb/contrib/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.384170 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3489 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/base.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/connectivity.py
--rw-r--r--   0 root         (0) root         (0)    16694 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/head.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/projections.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/region_mapping.py
--rw-r--r--   0 root         (0) root         (0)     7049 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/sensors.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/structural.py
--rw-r--r--   0 root         (0) root         (0)     5775 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/surface.py
--rw-r--r--   0 root         (0) root         (0)    26326 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/time_series.py
--rw-r--r--   0 root         (0) root         (0)    57272 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/time_series_xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.412170 tvb-contrib-2.8.2/tvb/contrib/scripts/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7178 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/linear_with_stimulus.py
--rw-r--r--   0 root         (0) root         (0)    13150 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py
--rw-r--r--   0 root         (0) root         (0)    13470 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py
--rw-r--r--   0 root         (0) root         (0)    34444 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py
--rw-r--r--   0 root         (0) root         (0)     9841 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/models/wilson_cowan_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.425170 tvb-contrib-2.8.2/tvb/contrib/scripts/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/plot/plotter.py
--rw-r--r--   0 root         (0) root         (0)    19366 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/plot/time_series_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.433170 tvb-contrib-2.8.2/tvb/contrib/scripts/service/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/service/head_service.py
--rw-r--r--   0 root         (0) root         (0)    16449 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/service/time_series_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.458170 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/command_line_utils.py
--rw-r--r--   0 root         (0) root         (0)     8983 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/computations_utils.py
--rw-r--r--   0 root         (0) root         (0)    30981 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/data_structures_utils.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/log_error_utils.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/parcellation_utils.py
--rw-r--r--   0 root         (0) root         (0)    10411 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/scripts/utils/time_series_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.459170 tvb-contrib-2.8.2/tvb/contrib/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.462170 tvb-contrib-2.8.2/tvb/contrib/simulator/demos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.479170 tvb-contrib-2.8.2/tvb/contrib/simulator/files/
--rw-r--r--   0 root         (0) root         (0)   240542 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/files/nerf_int.npz
--rw-r--r--   0 root         (0) root         (0)   240542 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/files/psi.npz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.502170 tvb-contrib-2.8.2/tvb/contrib/simulator/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19277 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/brunel_wang.py
--rw-r--r--   0 root         (0) root         (0)     8671 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/epileptor.py
--rw-r--r--   0 root         (0) root         (0)     7010 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/generic_2d_oscillator.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/hindmarsh_rose.py
--rw-r--r--   0 root         (0) root         (0)     7687 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/jansen_rit_david.py
--rw-r--r--   0 root         (0) root         (0)     9840 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/larter.py
--rw-r--r--   0 root         (0) root         (0)    15305 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/larter_breakspear.py
--rw-r--r--   0 root         (0) root         (0)    12813 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/liley_steynross.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/morris_lecar.py
--rw-r--r--   0 root         (0) root         (0)     8444 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/simulator/models/wong_wang.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.504170 tvb-contrib-2.8.2/tvb/contrib/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.508170 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.529169 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/
--rw-r--r--   0 root         (0) root         (0)     3458 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3983 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py
--rw-r--r--   0 root         (0) root         (0)     8857 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/function_tvb.py
--rw-r--r--   0 root         (0) root         (0)     6378 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     7011 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/monitors_test.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py
--rw-r--r--   0 root         (0) root         (0)     3300 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/update_function_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.561169 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8540 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_double_sync_test.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py
--rw-r--r--   0 root         (0) root         (0)    16684 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py
--rw-r--r--   0 root         (0) root         (0)    14188 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py
--rw-r--r--   0 root         (0) root         (0)     3947 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/update_function_test.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/synchronization_time_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.566169 tvb-contrib-2.8.2/tvb/contrib/tests/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4392 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/model/model_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.572169 tvb-contrib-2.8.2/tvb/contrib/tests/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14798 2023-09-19 13:48:30.000000 tvb-contrib-2.8.2/tvb/contrib/tests/scripts/time_series_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 14:12:28.580169 tvb-contrib-2.8.2/tvb_contrib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1778 2023-09-19 14:12:27.000000 tvb-contrib-2.8.2/tvb_contrib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5514 2023-09-19 14:12:28.000000 tvb-contrib-2.8.2/tvb_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 14:12:27.000000 tvb-contrib-2.8.2/tvb_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-09-19 14:12:27.000000 tvb-contrib-2.8.2/tvb_contrib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-09-19 14:12:27.000000 tvb-contrib-2.8.2/tvb_contrib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.635121 tvb-contrib-2.9/
+-rw-r--r--   0 root         (0) root         (0)    36777 2024-04-12 19:06:38.000000 tvb-contrib-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-12 19:06:38.000000 tvb-contrib-2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-04-12 19:21:39.634121 tvb-contrib-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-04-12 19:06:38.000000 tvb-contrib-2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 19:21:39.635121 tvb-contrib-2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-12 19:06:38.000000 tvb-contrib-2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.576118 tvb-contrib-2.9/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.576118 tvb-contrib-2.9/tvb/contrib/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.576118 tvb-contrib-2.9/tvb/contrib/cosimulation/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/cosimulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3918 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/cosimulation/cosim_history.py
+-rw-r--r--   0 root         (0) root         (0)    10127 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/cosimulation/cosim_monitors.py
+-rw-r--r--   0 root         (0) root         (0)    18275 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/cosimulation/cosimulator.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/cosimulation/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.583118 tvb-contrib-2.9/tvb/contrib/from_articles/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py
+-rw-r--r--   0 root         (0) root         (0)     6259 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py
+-rw-r--r--   0 root         (0) root         (0)     7195 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py
+-rw-r--r--   0 root         (0) root         (0)     7440 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py
+-rw-r--r--   0 root         (0) root         (0)     6542 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.584118 tvb-contrib-2.9/tvb/contrib/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.594119 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/base.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)    16694 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/head.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/projections.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     7049 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/sensors.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/structural.py
+-rw-r--r--   0 root         (0) root         (0)     5775 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/surface.py
+-rw-r--r--   0 root         (0) root         (0)    26326 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/time_series.py
+-rw-r--r--   0 root         (0) root         (0)    57272 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/datatypes/time_series_xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.598119 tvb-contrib-2.9/tvb/contrib/scripts/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7178 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/linear_with_stimulus.py
+-rw-r--r--   0 root         (0) root         (0)    13150 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py
+-rw-r--r--   0 root         (0) root         (0)    13470 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py
+-rw-r--r--   0 root         (0) root         (0)    34444 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/models/wilson_cowan_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.601119 tvb-contrib-2.9/tvb/contrib/scripts/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/plot/plotter.py
+-rw-r--r--   0 root         (0) root         (0)    19366 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/plot/time_series_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.602119 tvb-contrib-2.9/tvb/contrib/scripts/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/service/head_service.py
+-rw-r--r--   0 root         (0) root         (0)    16449 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/service/time_series_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.606119 tvb-contrib-2.9/tvb/contrib/scripts/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/command_line_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8983 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/computations_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30981 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/data_structures_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/log_error_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/parcellation_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/scripts/utils/time_series_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.606119 tvb-contrib-2.9/tvb/contrib/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.607120 tvb-contrib-2.9/tvb/contrib/simulator/demos/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.609120 tvb-contrib-2.9/tvb/contrib/simulator/files/
+-rw-r--r--   0 root         (0) root         (0)   240542 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/files/nerf_int.npz
+-rw-r--r--   0 root         (0) root         (0)   240542 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/files/psi.npz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.614120 tvb-contrib-2.9/tvb/contrib/simulator/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19277 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/brunel_wang.py
+-rw-r--r--   0 root         (0) root         (0)     8671 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)     7010 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/generic_2d_oscillator.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/hindmarsh_rose.py
+-rw-r--r--   0 root         (0) root         (0)     7687 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/jansen_rit_david.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/larter.py
+-rw-r--r--   0 root         (0) root         (0)    15305 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/larter_breakspear.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/liley_steynross.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/morris_lecar.py
+-rw-r--r--   0 root         (0) root         (0)     8444 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/simulator/models/wong_wang.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.615120 tvb-contrib-2.9/tvb/contrib/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.616120 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.623120 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3983 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/function_tvb.py
+-rw-r--r--   0 root         (0) root         (0)     6378 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/monitors_test.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/update_function_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.628121 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8540 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_double_sync_test.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py
+-rw-r--r--   0 root         (0) root         (0)    16684 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)    14188 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/update_function_test.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/cosimulation/synchronization_time_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.630121 tvb-contrib-2.9/tvb/contrib/tests/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4392 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/model/model_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.631121 tvb-contrib-2.9/tvb/contrib/tests/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14798 2024-04-12 19:06:38.000000 tvb-contrib-2.9/tvb/contrib/tests/scripts/time_series_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:39.633121 tvb-contrib-2.9/tvb_contrib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-04-12 19:21:39.000000 tvb-contrib-2.9/tvb_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-12 19:21:39.000000 tvb-contrib-2.9/tvb_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:21:39.000000 tvb-contrib-2.9/tvb_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-12 19:21:39.000000 tvb-contrib-2.9/tvb_contrib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-12 19:21:39.000000 tvb-contrib-2.9/tvb_contrib.egg-info/top_level.txt
```

### Comparing `tvb-contrib-2.8.2/LICENSE` & `tvb-contrib-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/PKG-INFO` & `tvb-contrib-2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: tvb-contrib
-Version: 2.8.2
+Version: 2.9
 Summary: A package with TVB contributed additions to the simulator, useful for scripting.
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience contrib
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: tvb-library
+Requires-Dist: xarray
+Requires-Dist: scikit-learn
 
 THE VIRTUAL BRAIN CONTRIB LIBRARY
 ====================================
 
 The Virtual Brain Project (TVB Project) has the purpose of offering some
 modern tools to the Neurosciences community, for computing, simulating
 and analyzing functional and structural data of human brains.
```

### Comparing `tvb-contrib-2.8.2/README.rst` & `tvb-contrib-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/setup.py` & `tvb-contrib-2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 #
 
 import os
 import shutil
 import setuptools
 
-CONTRIB_VERSION = "2.8.2"
+CONTRIB_VERSION = "2.9"
 CONTRIB_DEPENDENCIES = ["tvb-library", "xarray", "scikit-learn"]
 TEAM = "Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman"
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as fd:
     DESCRIPTION = fd.read()
 
 setuptools.setup(name='tvb-contrib',
```

### Comparing `tvb-contrib-2.8.2/tvb/__init__.py` & `tvb-contrib-2.9/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosim_history.py` & `tvb-contrib-2.9/tvb/contrib/cosimulation/cosim_history.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosim_monitors.py` & `tvb-contrib-2.9/tvb/contrib/cosimulation/cosim_monitors.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/cosimulation/cosimulator.py` & `tvb-contrib-2.9/tvb/contrib/cosimulation/cosimulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         # for delayed state [synchronization_step+1, n_var, n_node, n_mode],
         # including, initialization of the delayed state from the simulator's history,
         # which must be already configured.
         self.cosim_history = CosimHistory.from_simulator(self)
 
         # Reconfigure the connectivity for regions modelled by the other cosimulator exclusively:
         if self.exclusive:
-            self.connectivity.weights[self.proxy_inds][:, self.proxy_inds] = 0.0
+            self.connectivity.weights[numpy.ix_(self.proxy_inds, self.proxy_inds)] = 0.0
             self.connectivity.configure()
 
         # Configure the cosimulator monitor
         self.number_of_cosim_monitors = len(self.cosim_monitors)
         self._cosim_monitors_noncoupling_indices = list(range(self.number_of_cosim_monitors))
         self._cosim_monitors_coupling_indices = []
         for iM, monitor in enumerate(self.cosim_monitors):
```

### Comparing `tvb-contrib-2.8.2/tvb/contrib/cosimulation/exception.py` & `tvb-contrib-2.9/tvb/contrib/cosimulation/exception.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py` & `tvb-contrib-2.9/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/base.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/connectivity.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/head.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/head.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/local_connectivity.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/local_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/lookup_tables.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/projections.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/region_mapping.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/sensors.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/structural.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/surface.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/time_series.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/datatypes/time_series_xarray.py` & `tvb-contrib-2.9/tvb/contrib/scripts/datatypes/time_series_xarray.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/linear_with_stimulus.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/linear_with_stimulus.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/models/wilson_cowan_constraint.py` & `tvb-contrib-2.9/tvb/contrib/scripts/models/wilson_cowan_constraint.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/plot/plotter.py` & `tvb-contrib-2.9/tvb/contrib/scripts/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py` & `tvb-contrib-2.9/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/plot/time_series_plotter.py` & `tvb-contrib-2.9/tvb/contrib/scripts/plot/time_series_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/service/head_service.py` & `tvb-contrib-2.9/tvb/contrib/scripts/service/head_service.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/service/time_series_service.py` & `tvb-contrib-2.9/tvb/contrib/scripts/service/time_series_service.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/command_line_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/computations_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/computations_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/data_structures_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/data_structures_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/file_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/log_error_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/log_error_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/parcellation_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/parcellation_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/scripts/utils/time_series_utils.py` & `tvb-contrib-2.9/tvb/contrib/scripts/utils/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py` & `tvb-contrib-2.9/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/files/nerf_int.npz` & `tvb-contrib-2.9/tvb/contrib/simulator/files/nerf_int.npz`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/files/psi.npz` & `tvb-contrib-2.9/tvb/contrib/simulator/files/psi.npz`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/brunel_wang.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/brunel_wang.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/epileptor.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/generic_2d_oscillator.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/generic_2d_oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/hindmarsh_rose.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/hindmarsh_rose.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/jansen_rit_david.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/jansen_rit_david.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/larter.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/larter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/larter_breakspear.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/larter_breakspear.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/liley_steynross.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/liley_steynross.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/morris_lecar.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/morris_lecar.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/simulator/models/wong_wang.py` & `tvb-contrib-2.9/tvb/contrib/simulator/models/wong_wang.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/function_tvb.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/function_tvb.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/monitors_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/monitors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/parallel/update_function_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/parallel/update_function_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_double_sync_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_double_sync_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/simple/update_function_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/simple/update_function_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/cosimulation/synchronization_time_set.py` & `tvb-contrib-2.9/tvb/contrib/tests/cosimulation/synchronization_time_set.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/model/model_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/model/model_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb/contrib/tests/scripts/time_series_test.py` & `tvb-contrib-2.9/tvb/contrib/tests/scripts/time_series_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.8.2/tvb_contrib.egg-info/PKG-INFO` & `tvb-contrib-2.9/tvb_contrib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: tvb-contrib
-Version: 2.8.2
+Version: 2.9
 Summary: A package with TVB contributed additions to the simulator, useful for scripting.
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience contrib
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: tvb-library
+Requires-Dist: xarray
+Requires-Dist: scikit-learn
 
 THE VIRTUAL BRAIN CONTRIB LIBRARY
 ====================================
 
 The Virtual Brain Project (TVB Project) has the purpose of offering some
 modern tools to the Neurosciences community, for computing, simulating
 and analyzing functional and structural data of human brains.
```

### Comparing `tvb-contrib-2.8.2/tvb_contrib.egg-info/SOURCES.txt` & `tvb-contrib-2.9/tvb_contrib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

