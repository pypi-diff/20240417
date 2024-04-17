# Comparing `tmp/tvb-library-2.8.2.tar.gz` & `tmp/tvb-library-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-library-2.8.2.tar", last modified: Tue Sep 19 06:19:05 2023, max compression
+gzip compressed data, was "tvb-library-2.9.tar", last modified: Fri Apr 12 19:21:37 2024, max compression
```

## Comparing `tvb-library-2.8.2.tar` & `tvb-library-2.9.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.562108 tvb-library-2.8.2/
--rw-r--r--   0 root         (0) root         (0)      946 2023-09-19 05:59:29.000000 tvb-library-2.8.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-09-19 05:59:29.000000 tvb-library-2.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      168 2023-09-19 05:59:29.000000 tvb-library-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5739 2023-09-19 06:19:05.562108 tvb-library-2.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4949 2023-09-19 05:59:29.000000 tvb-library-2.8.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 06:19:05.562108 tvb-library-2.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3292 2023-09-19 05:59:29.000000 tvb-library-2.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.504105 tvb-library-2.8.2/tvb/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.507105 tvb-library-2.8.2/tvb/analyzers/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4686 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/fft.py
--rw-r--r--   0 root         (0) root         (0)    14371 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/fmri_balloon.py
--rw-r--r--   0 root         (0) root         (0)    14416 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/graph.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/ica.py
--rw-r--r--   0 root         (0) root         (0)    13711 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/ica_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     4098 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/info.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/metric_kuramoto_index.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/metric_proxy_metastability.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/metric_variance_global.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/metric_variance_of_node_variance.py
--rw-r--r--   0 root         (0) root         (0)     5015 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/node_coherence.py
--rw-r--r--   0 root         (0) root         (0)    12504 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/node_complex_coherence.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/pca.py
--rw-r--r--   0 root         (0) root         (0)     7060 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/analyzers/wavelet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.508105 tvb-library-2.8.2/tvb/basic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.510105 tvb-library-2.8.2/tvb/basic/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6020 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/environment.py
--rw-r--r--   0 root         (0) root         (0)     9210 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/profile_settings.py
--rw-r--r--   0 root         (0) root         (0)    16346 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/settings.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/stored.py
--rw-r--r--   0 root         (0) root         (0)       15 2023-09-19 06:14:20.000000 tvb-library-2.8.2/tvb/basic/config/tvb.version
--rw-r--r--   0 root         (0) root         (0)     1666 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/config/utils.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.511105 tvb-library-2.8.2/tvb/basic/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4101 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/logger/builder.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/logger/library_logger.conf
--rw-r--r--   0 root         (0) root         (0)     1728 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/logger/library_logger_test.conf
--rw-r--r--   0 root         (0) root         (0)     2027 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/logger/simple_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.513105 tvb-library-2.8.2/tvb/basic/neotraits/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25350 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/_attr.py
--rw-r--r--   0 root         (0) root         (0)    12087 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/_core.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/_declarative_base.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/api.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/ex.py
--rw-r--r--   0 root         (0) root         (0)     6755 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/neotraits/info.py
--rw-r--r--   0 root         (0) root         (0)     5928 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/profile.py
--rw-r--r--   0 root         (0) root         (0)     8553 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/basic/readers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.518105 tvb-library-2.8.2/tvb/datatypes/
--rw-r--r--   0 root         (0) root         (0)     1590 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33607 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     9158 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/cortex.py
--rw-r--r--   0 root         (0) root         (0)    19941 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/equations.py
--rw-r--r--   0 root         (0) root         (0)     3650 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/fcd.py
--rw-r--r--   0 root         (0) root         (0)     3308 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/graph.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     8235 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/mode_decompositions.py
--rw-r--r--   0 root         (0) root         (0)     9306 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/patterns.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/projections.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/region_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11811 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/sensors.py
--rw-r--r--   0 root         (0) root         (0)    12479 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/spectral.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/structural.py
--rw-r--r--   0 root         (0) root         (0)    29883 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/surfaces.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/temporal_correlations.py
--rw-r--r--   0 root         (0) root         (0)    12200 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/tracts.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/datatypes/volumes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.519106 tvb-library-2.8.2/tvb/rateML/
--rwxr-xr-x   0 root         (0) root         (0)    22851 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/README.md
--rwxr-xr-x   0 root         (0) root         (0)    15067 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XML2model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.522106 tvb-library-2.8.2/tvb/rateML/XMLmodels/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/epileptor.xml
--rw-r--r--   0 root         (0) root         (0)     2107 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/kuramoto.xml
--rw-r--r--   0 root         (0) root         (0)     4396 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/model_template.xml
--rw-r--r--   0 root         (0) root         (0)     5096 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/montbrio.xml
--rw-r--r--   0 root         (0) root         (0)     3916 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/oscillator.xml
--rw-r--r--   0 root         (0) root         (0)     5966 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/rwongwang.xml
--rw-r--r--   0 root         (0) root         (0)     6318 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/rwongwang_deco.xml
--rw-r--r--   0 root         (0) root         (0)    12080 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/XMLmodels/zerlaut.xml
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.525106 tvb-library-2.8.2/tvb/rateML/generatedModels/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.527106 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10351 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/epileptorref.c
--rw-r--r--   0 root         (0) root         (0)     6901 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c
--rw-r--r--   0 root         (0) root         (0)     7865 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/montbrioref.c
--rw-r--r--   0 root         (0) root         (0)     7862 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c
--rw-r--r--   0 root         (0) root         (0)     8667 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c
--rw-r--r--   0 root         (0) root         (0)     9812 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/epileptor.c
--rw-r--r--   0 root         (0) root         (0)     5461 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/epileptor.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/kuramoto.c
--rw-r--r--   0 root         (0) root         (0)     1571 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/kuramoto.py
--rw-r--r--   0 root         (0) root         (0)     7745 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio.c
--rw-r--r--   0 root         (0) root         (0)     3181 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio.py
--rw-r--r--   0 root         (0) root         (0)     8939 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio_heun.c
--rw-r--r--   0 root         (0) root         (0)     7858 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/oscillator.c
--rw-r--r--   0 root         (0) root         (0)     3359 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/oscillator.py
--rw-r--r--   0 root         (0) root         (0)     8433 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/rwongwang.c
--rw-r--r--   0 root         (0) root         (0)     5577 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/rwongwang.py
--rw-r--r--   0 root         (0) root         (0)    17337 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/zerlaut.c
--rw-r--r--   0 root         (0) root         (0)     7711 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/generatedModels/zerlaut_func.h
--rw-r--r--   0 root         (0) root         (0)    25374 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/rML_v0.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.528106 tvb-library-2.8.2/tvb/rateML/run/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17732 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/model_driver.py
--rw-r--r--   0 root         (0) root         (0)    18267 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/model_driver_bold.py
--rw-r--r--   0 root         (0) root         (0)    17347 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/model_driver_heun.py
--rw-r--r--   0 root         (0) root         (0)    18301 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/model_driver_zerlaut.py
--rwxr-xr-x   0 root         (0) root         (0)     2972 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/run/regular_run.py
--rwxr-xr-x   0 root         (0) root         (0)    13603 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/tmpl8_cuda.py
--rw-r--r--   0 root         (0) root         (0)    17614 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/tmpl8_driver.py
--rwxr-xr-x   0 root         (0) root         (0)     5191 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/rateML/tmpl8_python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.531106 tvb-library-2.8.2/tvb/simulator/
--rw-r--r--   0 root         (0) root         (0)     1397 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.532106 tvb-library-2.8.2/tvb/simulator/_numba/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6168 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/coupling.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/gpu_bench.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/integrators.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/loops.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/models.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/_numba/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.535106 tvb-library-2.8.2/tvb/simulator/backend/
--rw-r--r--   0 root         (0) root         (0)     1295 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/base.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/cu.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/nb.py
--rw-r--r--   0 root         (0) root         (0)     9404 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/nb_mpr.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/np.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/ref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.538106 tvb-library-2.8.2/tvb/simulator/backend/templates/
--rw-r--r--   0 root         (0) root         (0)     2131 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/cu-base.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2141 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/cu-coupling.cu.mako
--rw-r--r--   0 root         (0) root         (0)     3245 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/cu-defs.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2027 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/cu-dfuns.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2639 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/cu-sim-ode.cu.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.539106 tvb-library-2.8.2/tvb/simulator/backend/templates/generated/
--rw-r--r--   0 root         (0) root         (0)       17 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/generated/.gitignore
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-coupling.py.mako
--rw-r--r--   0 root         (0) root         (0)     2145 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-coupling2.py.mako
--rw-r--r--   0 root         (0) root         (0)     1950 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-dfuns.py.mako
--rw-r--r--   0 root         (0) root         (0)     6061 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-integrate.py.mako
--rw-r--r--   0 root         (0) root         (0)     5359 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-montbrio.py.mako
--rw-r--r--   0 root         (0) root         (0)     3234 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/nb-sim.py.mako
--rw-r--r--   0 root         (0) root         (0)     2492 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/np-coupling.py.mako
--rw-r--r--   0 root         (0) root         (0)     1786 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/np-dfuns.py.mako
--rw-r--r--   0 root         (0) root         (0)     3739 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/np-integrate.py.mako
--rw-r--r--   0 root         (0) root         (0)     2219 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/backend/templates/np-sim.py.mako
--rw-r--r--   0 root         (0) root         (0)     6271 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/common.py
--rw-r--r--   0 root         (0) root         (0)    16501 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/coupling.py
--rw-r--r--   0 root         (0) root         (0)     6283 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/descriptors.py
--rw-r--r--   0 root         (0) root         (0)    12555 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/history.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/integrators.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/lab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.543107 tvb-library-2.8.2/tvb/simulator/models/
--rw-r--r--   0 root         (0) root         (0)     6448 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11018 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/base.py
--rw-r--r--   0 root         (0) root         (0)    21582 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/epileptor.py
--rw-r--r--   0 root         (0) root         (0)    16115 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/epileptor_rs.py
--rw-r--r--   0 root         (0) root         (0)    29904 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/epileptorcodim3.py
--rw-r--r--   0 root         (0) root         (0)     7902 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/hopfield.py
--rw-r--r--   0 root         (0) root         (0)    35533 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/infinite_theta.py
--rw-r--r--   0 root         (0) root         (0)    23147 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/jansen_rit.py
--rw-r--r--   0 root         (0) root         (0)    12504 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/k_ion_exchange.py
--rw-r--r--   0 root         (0) root         (0)    18473 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/larter_breakspear.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/linear.py
--rw-r--r--   0 root         (0) root         (0)    22719 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/oscillator.py
--rw-r--r--   0 root         (0) root         (0)    25605 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/stefanescu_jirsa.py
--rw-r--r--   0 root         (0) root         (0)    16734 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/wilson_cowan.py
--rw-r--r--   0 root         (0) root         (0)     6739 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/wong_wang.py
--rw-r--r--   0 root         (0) root         (0)    15293 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/wong_wang_exc_inh.py
--rw-r--r--   0 root         (0) root         (0)    40228 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/models/zerlaut.py
--rw-r--r--   0 root         (0) root         (0)    43225 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/monitors.py
--rw-r--r--   0 root         (0) root         (0)    10525 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/noise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.547107 tvb-library-2.8.2/tvb/simulator/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23618 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/base_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.547107 tvb-library-2.8.2/tvb/simulator/plot/colourmaps/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/colourmaps/BlackToBlue
--rw-r--r--   0 root         (0) root         (0)     9150 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/compare_integrators.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/config.py
--rw-r--r--   0 root         (0) root         (0)    14154 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/epileptor_plotter.py
--rw-r--r--   0 root         (0) root         (0)     8068 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/head_plotter.py
--rw-r--r--   0 root         (0) root         (0)     5029 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/head_plotter_3d.py
--rw-r--r--   0 root         (0) root         (0)    35926 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/phase_plane_interactive.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/plotter.py
--rw-r--r--   0 root         (0) root         (0)    20529 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/power_spectra_interactive.py
--rw-r--r--   0 root         (0) root         (0)    32161 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/time_series_plotter.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/timeseries_interactive.py
--rw-r--r--   0 root         (0) root         (0)    22865 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/tools.py
--rw-r--r--   0 root         (0) root         (0)    10714 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/plot/utils.py
--rw-r--r--   0 root         (0) root         (0)    28923 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/simulator/simulator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.548107 tvb-library-2.8.2/tvb/tests/
--rw-r--r--   0 root         (0) root         (0)     2099 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/bench.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/bench_against_mpr_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.548107 tvb-library-2.8.2/tvb/tests/library/
--rw-r--r--   0 root         (0) root         (0)     1653 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/base_testcase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.549107 tvb-library-2.8.2/tvb/tests/library/basic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.549107 tvb-library-2.8.2/tvb/tests/library/basic/neotraits/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/basic/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/basic/neotraits/_attr_test.py
--rw-r--r--   0 root         (0) root         (0)    27593 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/basic/neotraits/neotraits_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.554107 tvb-library-2.8.2/tvb/tests/library/datatypes/
--rw-r--r--   0 root         (0) root         (0)   115069 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/Edited_Connectivity.h5
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/connectivity_test.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/equations_test.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/graph_test.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/mode_decompositions_test.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/patterns_test.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/projections_test.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/sensors_test.py
--rw-r--r--   0 root         (0) root         (0)     5725 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/spectral_test.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/surfaces_test.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/temporal_correlations_test.py
--rw-r--r--   0 root         (0) root         (0)     4446 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/timeseries_test.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/datatypes/volumes_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.558107 tvb-library-2.8.2/tvb/tests/library/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15561 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/_numba_tests.py
--rw-r--r--   0 root         (0) root         (0)    10929 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/_opencl_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.560108 tvb-library-2.8.2/tvb/tests/library/simulator/backend/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/backendtestbase.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/cubackend_test.py
--rw-r--r--   0 root         (0) root         (0)    14631 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py
--rw-r--r--   0 root         (0) root         (0)    11349 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbbackend_test.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbmprperf_test.py
--rw-r--r--   0 root         (0) root         (0)     9706 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/backend/npbackend_test.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/common_test.py
--rw-r--r--   0 root         (0) root         (0)     5840 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/coupling_test.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/descriptors_test.py
--rw-r--r--   0 root         (0) root         (0)     3913 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/history_test.py
--rw-r--r--   0 root         (0) root         (0)     9442 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/integrators_test.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/modelir_test.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/models_test.py
--rw-r--r--   0 root         (0) root         (0)    10916 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/monitors_test.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/noise_test.py
--rw-r--r--   0 root         (0) root         (0)    10229 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/rateml_test.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/regionmapping_test.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/rngperf_test.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/simulator_step_test.py
--rw-r--r--   0 root         (0) root         (0)    15884 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/simulator_test.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/library/simulator/stimulation_test.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-09-19 05:59:29.000000 tvb-library-2.8.2/tvb/tests/validate_model_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 06:19:05.561107 tvb-library-2.8.2/tvb_library.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5739 2023-09-19 06:19:05.000000 tvb-library-2.8.2/tvb_library.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8450 2023-09-19 06:19:05.000000 tvb-library-2.8.2/tvb_library.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 06:19:05.000000 tvb-library-2.8.2/tvb_library.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2023-09-19 06:19:05.000000 tvb-library-2.8.2/tvb_library.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-09-19 06:19:05.000000 tvb-library-2.8.2/tvb_library.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.756026 tvb-library-2.9/
+-rw-r--r--   0 root         (0) root         (0)      946 2024-04-12 19:06:40.000000 tvb-library-2.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2024-04-12 19:06:40.000000 tvb-library-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-12 19:06:40.000000 tvb-library-2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6314 2024-04-12 19:21:37.755026 tvb-library-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4949 2024-04-12 19:06:40.000000 tvb-library-2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 19:21:37.756026 tvb-library-2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-04-12 19:06:40.000000 tvb-library-2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.603018 tvb-library-2.9/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.618019 tvb-library-2.9/tvb/analyzers/
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/fft.py
+-rw-r--r--   0 root         (0) root         (0)    14371 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/fmri_balloon.py
+-rw-r--r--   0 root         (0) root         (0)    14416 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/ica.py
+-rw-r--r--   0 root         (0) root         (0)    13711 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/ica_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     4098 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/info.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/metric_kuramoto_index.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/metric_proxy_metastability.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/metric_variance_global.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/metric_variance_of_node_variance.py
+-rw-r--r--   0 root         (0) root         (0)     5015 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/node_coherence.py
+-rw-r--r--   0 root         (0) root         (0)    12504 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/node_complex_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/pca.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/analyzers/wavelet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.620019 tvb-library-2.9/tvb/basic/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.624019 tvb-library-2.9/tvb/basic/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6020 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/environment.py
+-rw-r--r--   0 root         (0) root         (0)     9210 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/profile_settings.py
+-rw-r--r--   0 root         (0) root         (0)    16341 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/stored.py
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-12 19:17:42.000000 tvb-library-2.9/tvb/basic/config/tvb.version
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/config/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.626019 tvb-library-2.9/tvb/basic/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/logger/builder.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/logger/library_logger.conf
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/logger/library_logger_test.conf
+-rw-r--r--   0 root         (0) root         (0)     2027 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/logger/simple_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.633020 tvb-library-2.9/tvb/basic/neotraits/
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25350 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/_attr.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/_core.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/_declarative_base.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/api.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/ex.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/neotraits/info.py
+-rw-r--r--   0 root         (0) root         (0)     5928 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8553 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/basic/readers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.643020 tvb-library-2.9/tvb/datatypes/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33607 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/cortex.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/equations.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/fcd.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/graph.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     8235 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/mode_decompositions.py
+-rw-r--r--   0 root         (0) root         (0)     9306 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/projections.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11811 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    12479 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/spectral.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/structural.py
+-rw-r--r--   0 root         (0) root         (0)    29883 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/surfaces.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/temporal_correlations.py
+-rw-r--r--   0 root         (0) root         (0)    12200 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/tracts.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/datatypes/volumes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.648020 tvb-library-2.9/tvb/rateML/
+-rwxr-xr-x   0 root         (0) root         (0)    22851 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/README.md
+-rwxr-xr-x   0 root         (0) root         (0)    15067 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XML2model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.654021 tvb-library-2.9/tvb/rateML/XMLmodels/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/epileptor.xml
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/kuramoto.xml
+-rw-r--r--   0 root         (0) root         (0)     4396 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/model_template.xml
+-rw-r--r--   0 root         (0) root         (0)     5096 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/montbrio.xml
+-rw-r--r--   0 root         (0) root         (0)     3916 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/oscillator.xml
+-rw-r--r--   0 root         (0) root         (0)     5966 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/rwongwang.xml
+-rw-r--r--   0 root         (0) root         (0)     6318 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/rwongwang_deco.xml
+-rw-r--r--   0 root         (0) root         (0)    12080 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/XMLmodels/zerlaut.xml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.663021 tvb-library-2.9/tvb/rateML/generatedModels/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.666021 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10351 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/epileptorref.c
+-rw-r--r--   0 root         (0) root         (0)     6901 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c
+-rw-r--r--   0 root         (0) root         (0)     7865 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/montbrioref.c
+-rw-r--r--   0 root         (0) root         (0)     7862 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c
+-rw-r--r--   0 root         (0) root         (0)     8667 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c
+-rw-r--r--   0 root         (0) root         (0)     9812 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/epileptor.c
+-rw-r--r--   0 root         (0) root         (0)     5461 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/kuramoto.c
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/kuramoto.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/montbrio.c
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/montbrio.py
+-rw-r--r--   0 root         (0) root         (0)     8939 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/montbrio_heun.c
+-rw-r--r--   0 root         (0) root         (0)     7858 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/oscillator.c
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/oscillator.py
+-rw-r--r--   0 root         (0) root         (0)     8433 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/rwongwang.c
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/rwongwang.py
+-rw-r--r--   0 root         (0) root         (0)    17337 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/zerlaut.c
+-rw-r--r--   0 root         (0) root         (0)     7711 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/generatedModels/zerlaut_func.h
+-rw-r--r--   0 root         (0) root         (0)    25374 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/rML_v0.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.669021 tvb-library-2.9/tvb/rateML/run/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17732 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/model_driver.py
+-rw-r--r--   0 root         (0) root         (0)    18267 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/model_driver_bold.py
+-rw-r--r--   0 root         (0) root         (0)    17347 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/model_driver_heun.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/model_driver_zerlaut.py
+-rwxr-xr-x   0 root         (0) root         (0)     2972 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/run/regular_run.py
+-rwxr-xr-x   0 root         (0) root         (0)    13603 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/tmpl8_cuda.py
+-rw-r--r--   0 root         (0) root         (0)    17614 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/tmpl8_driver.py
+-rwxr-xr-x   0 root         (0) root         (0)     5191 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/rateML/tmpl8_python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.676022 tvb-library-2.9/tvb/simulator/
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.680022 tvb-library-2.9/tvb/simulator/_numba/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/coupling.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/gpu_bench.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/integrators.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/loops.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/models.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/_numba/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.683022 tvb-library-2.9/tvb/simulator/backend/
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/base.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/cu.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/nb.py
+-rw-r--r--   0 root         (0) root         (0)     9404 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/nb_mpr.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/np.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/ref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.692023 tvb-library-2.9/tvb/simulator/backend/templates/
+-rw-r--r--   0 root         (0) root         (0)     2131 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/cu-base.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2141 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/cu-coupling.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     3245 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/cu-defs.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2027 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/cu-dfuns.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/cu-sim-ode.cu.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.693023 tvb-library-2.9/tvb/simulator/backend/templates/generated/
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/generated/.gitignore
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-coupling.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2145 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-coupling2.py.mako
+-rw-r--r--   0 root         (0) root         (0)     1950 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-dfuns.py.mako
+-rw-r--r--   0 root         (0) root         (0)     6061 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-integrate.py.mako
+-rw-r--r--   0 root         (0) root         (0)     5359 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-montbrio.py.mako
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/nb-sim.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/np-coupling.py.mako
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/np-dfuns.py.mako
+-rw-r--r--   0 root         (0) root         (0)     3739 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/np-integrate.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/backend/templates/np-sim.py.mako
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/common.py
+-rw-r--r--   0 root         (0) root         (0)    16501 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/coupling.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/descriptors.py
+-rw-r--r--   0 root         (0) root         (0)    12555 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/history.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/integrators.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/lab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.703023 tvb-library-2.9/tvb/simulator/models/
+-rw-r--r--   0 root         (0) root         (0)     6448 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11018 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/base.py
+-rw-r--r--   0 root         (0) root         (0)    21582 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)    16115 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/epileptor_rs.py
+-rw-r--r--   0 root         (0) root         (0)    29904 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/epileptorcodim3.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/hopfield.py
+-rw-r--r--   0 root         (0) root         (0)    35533 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/infinite_theta.py
+-rw-r--r--   0 root         (0) root         (0)    23147 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/jansen_rit.py
+-rw-r--r--   0 root         (0) root         (0)    12504 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/k_ion_exchange.py
+-rw-r--r--   0 root         (0) root         (0)    18473 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/larter_breakspear.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/linear.py
+-rw-r--r--   0 root         (0) root         (0)    22719 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/oscillator.py
+-rw-r--r--   0 root         (0) root         (0)    25605 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/stefanescu_jirsa.py
+-rw-r--r--   0 root         (0) root         (0)    16734 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/wilson_cowan.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/wong_wang.py
+-rw-r--r--   0 root         (0) root         (0)    15293 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/wong_wang_exc_inh.py
+-rw-r--r--   0 root         (0) root         (0)    40228 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/models/zerlaut.py
+-rw-r--r--   0 root         (0) root         (0)    43225 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/monitors.py
+-rw-r--r--   0 root         (0) root         (0)    10525 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/noise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.716024 tvb-library-2.9/tvb/simulator/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23618 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/base_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.716024 tvb-library-2.9/tvb/simulator/plot/colourmaps/
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/colourmaps/BlackToBlue
+-rw-r--r--   0 root         (0) root         (0)     9150 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/compare_integrators.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/config.py
+-rw-r--r--   0 root         (0) root         (0)    14154 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/epileptor_plotter.py
+-rw-r--r--   0 root         (0) root         (0)     8068 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/head_plotter.py
+-rw-r--r--   0 root         (0) root         (0)     5029 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/head_plotter_3d.py
+-rw-r--r--   0 root         (0) root         (0)    35926 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/phase_plane_interactive.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/plotter.py
+-rw-r--r--   0 root         (0) root         (0)    20529 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/power_spectra_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    32161 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/time_series_plotter.py
+-rw-r--r--   0 root         (0) root         (0)    29755 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/timeseries_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    22865 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/tools.py
+-rw-r--r--   0 root         (0) root         (0)    10714 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/plot/utils.py
+-rw-r--r--   0 root         (0) root         (0)    28923 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/simulator/simulator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.718024 tvb-library-2.9/tvb/tests/
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/bench.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/bench_against_mpr_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.719024 tvb-library-2.9/tvb/tests/library/
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/base_testcase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.720024 tvb-library-2.9/tvb/tests/library/basic/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.721024 tvb-library-2.9/tvb/tests/library/basic/neotraits/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/basic/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/basic/neotraits/_attr_test.py
+-rw-r--r--   0 root         (0) root         (0)    27593 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/basic/neotraits/neotraits_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.734025 tvb-library-2.9/tvb/tests/library/datatypes/
+-rw-r--r--   0 root         (0) root         (0)   115069 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/Edited_Connectivity.h5
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/connectivity_test.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/equations_test.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/graph_test.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/mode_decompositions_test.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/patterns_test.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/projections_test.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/sensors_test.py
+-rw-r--r--   0 root         (0) root         (0)     5725 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/spectral_test.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/surfaces_test.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/temporal_correlations_test.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/timeseries_test.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/datatypes/volumes_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.744025 tvb-library-2.9/tvb/tests/library/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15561 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/_numba_tests.py
+-rw-r--r--   0 root         (0) root         (0)    10929 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/_opencl_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.747025 tvb-library-2.9/tvb/tests/library/simulator/backend/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/backendtestbase.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/cubackend_test.py
+-rw-r--r--   0 root         (0) root         (0)    14631 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/nbbackend_test.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/nbmprperf_test.py
+-rw-r--r--   0 root         (0) root         (0)     9706 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/backend/npbackend_test.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/common_test.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/coupling_test.py
+-rw-r--r--   0 root         (0) root         (0)     5221 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/descriptors_test.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/history_test.py
+-rw-r--r--   0 root         (0) root         (0)     9442 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/integrators_test.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/modelir_test.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/models_test.py
+-rw-r--r--   0 root         (0) root         (0)    10916 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/monitors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/noise_test.py
+-rw-r--r--   0 root         (0) root         (0)    10229 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/rateml_test.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/regionmapping_test.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/rngperf_test.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/simulator_step_test.py
+-rw-r--r--   0 root         (0) root         (0)    15884 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/simulator_test.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/library/simulator/stimulation_test.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2024-04-12 19:06:40.000000 tvb-library-2.9/tvb/tests/validate_model_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:37.751026 tvb-library-2.9/tvb_library.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6314 2024-04-12 19:21:37.000000 tvb-library-2.9/tvb_library.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8450 2024-04-12 19:21:37.000000 tvb-library-2.9/tvb_library.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:21:37.000000 tvb-library-2.9/tvb_library.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-12 19:21:37.000000 tvb-library-2.9/tvb_library.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-12 19:21:37.000000 tvb-library-2.9/tvb_library.egg-info/top_level.txt
```

### Comparing `tvb-library-2.8.2/AUTHORS` & `tvb-library-2.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/LICENSE` & `tvb-library-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/PKG-INFO` & `tvb-library-2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 Metadata-Version: 2.1
 Name: tvb-library
-Version: 2.8.2
+Version: 2.9
 Summary: A package for performing whole brain simulations
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience human animal neuronal dynamics models delay
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: autopep8
+Requires-Dist: Deprecated
+Requires-Dist: docutils
+Requires-Dist: ipywidgets
+Requires-Dist: lxml
+Requires-Dist: mako>=1.1.4
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: numba
+Requires-Dist: numexpr
+Requires-Dist: numpy
+Requires-Dist: pylems
+Requires-Dist: scipy
+Requires-Dist: six
+Provides-Extra: test
+Requires-Dist: h5py; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: tvb-gdist; extra == "test"
+Requires-Dist: tvb-data; extra == "test"
 
 THE VIRTUAL BRAIN SCIENTIFIC LIBRARY
 ====================================
 
 The Virtual Brain Project (TVB Project) has the purpose of offering some
 modern tools to the Neurosciences community, for computing, simulating
 and analyzing functional and structural data of human brains.
```

### Comparing `tvb-library-2.8.2/README.rst` & `tvb-library-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/setup.py` & `tvb-library-2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     python setup.py install/develop
 """
 
 import os
 import shutil
 import setuptools
 
-LIBRARY_VERSION = "2.8.2"
+LIBRARY_VERSION = "2.9"
 
 LIBRARY_TEAM = "Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa"
 
 LIBRARY_REQUIRED_PACKAGES = ["autopep8", "Deprecated", "docutils", "ipywidgets", "lxml", "mako>=1.1.4", "matplotlib",
                              "networkx", "numba", "numexpr", "numpy", "pylems", "scipy", "six"]
 
 LIBRARY_REQUIRED_EXTRA = ["h5py", "pytest", "pytest-benchmark", "pytest-xdist", "tvb-gdist", "tvb-data"]
```

### Comparing `tvb-library-2.8.2/tvb/__init__.py` & `tvb-library-2.9/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/__init__.py` & `tvb-library-2.9/tvb/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/fft.py` & `tvb-library-2.9/tvb/analyzers/fft.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/fmri_balloon.py` & `tvb-library-2.9/tvb/analyzers/fmri_balloon.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/graph.py` & `tvb-library-2.9/tvb/analyzers/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/ica.py` & `tvb-library-2.9/tvb/analyzers/ica.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/ica_algorithm.py` & `tvb-library-2.9/tvb/analyzers/ica_algorithm.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/info.py` & `tvb-library-2.9/tvb/analyzers/info.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/metric_kuramoto_index.py` & `tvb-library-2.9/tvb/analyzers/metric_kuramoto_index.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/metric_proxy_metastability.py` & `tvb-library-2.9/tvb/analyzers/metric_proxy_metastability.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/metric_variance_global.py` & `tvb-library-2.9/tvb/analyzers/metric_variance_global.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/metric_variance_of_node_variance.py` & `tvb-library-2.9/tvb/analyzers/metric_variance_of_node_variance.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/node_coherence.py` & `tvb-library-2.9/tvb/analyzers/node_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/node_complex_coherence.py` & `tvb-library-2.9/tvb/analyzers/node_complex_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/pca.py` & `tvb-library-2.9/tvb/analyzers/pca.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/analyzers/wavelet.py` & `tvb-library-2.9/tvb/analyzers/wavelet.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/config/environment.py` & `tvb-library-2.9/tvb/basic/config/environment.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/config/profile_settings.py` & `tvb-library-2.9/tvb/basic/config/profile_settings.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/config/settings.py` & `tvb-library-2.9/tvb/basic/config/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     """
     Gather settings related to various version numbers of TVB application
     """
 
     SVN_GIT_MIGRATION_REVISION = 10000
 
     # Current release number
-    BASE_VERSION = "2.8.2"
+    BASE_VERSION = "2.9"
 
     # Current DB version. Create a new migration script from command line and copy its gid here
-    DB_STRUCTURE_VERSION = '32d4bf9f8def'
+    DB_STRUCTURE_VERSION = '32d4bf9f8ghj'
 
     # This is the version of the data stored in H5 and XML files
     # and should be used by next versions to know how to import
     # data in TVB format, in case data structure changes.
     # Value should be updated every time data structure is changed.
     DATA_VERSION = 5
     DATA_VERSION_ATTRIBUTE = "Data_version"
@@ -238,20 +238,21 @@
         try:
             import tvb.interfaces
             self.CURRENT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(tvb.interfaces.__file__)))
         except ImportError:
             pass
 
         self.SERVER_PORT = manager.get_attribute(stored.KEY_PORT, 8080, int)
+        self.REST_PORT = manager.get_attribute(stored.KEY_PORT_REST, 9090, int)
 
-        self.OPENSHIFT_DEPLOY = manager.get_attribute(stored.KEY_OPENSHIFT_DEPLOY, False, eval)
-        self.OPENSHIFT_NAMESPACE = manager.get_attribute(stored.KEY_OPENSHIFT_NAMESPACE, "")
-        self.OPENSHIFT_APPLICATION = manager.get_attribute(stored.KEY_OPENSHIFT_APPLICATION, "")
-        self.OPENSHIFT_PROCESSING_OPERATIONS_APPLICATION = manager.get_attribute(stored.KEY_PROCESSING_OPERATIONS_APPLICATION, "")
-        self.OPENSHIFT_DATA_ENCRYPTION_HANDLER_APPLICATION = manager.get_attribute(stored.KEY_DATA_ENCRYPTION_HANDLER_APPLICATION, self.OPENSHIFT_APPLICATION)
+        self.IS_CLOUD_DEPLOY = manager.get_attribute(stored.KEY_IS_CLOUD_DEPLOY, False, eval)
+        self.IS_CLOUD_HTTPS = manager.get_attribute(stored.KEY_IS_CLOUD_HTTPS, False, eval)
+        self.CLOUD_APP_EXEC_NAME = manager.get_attribute(stored.KEY_CLOUD_APP_EXEC, "")
+        self.CLOUD_APP_EXEC_MAX_PODS_NO = manager.get_attribute(stored.KEY_CLOUD_APP_EXEC_MAX_PODS, 2)
+        self.CLOUD_APP_ENCRYPTION_HANDLER_NAME = manager.get_attribute(stored.KEY_CLOUD_APP_ENCRYPTION_HANDLER, "")
         # Compute reference towards the current web application, valid FROM localhost
         server_IP = manager.get_attribute(stored.KEY_IP, self.LOCALHOST)
         self.BASE_LOCAL_URL = "http://%s:%s/" % (server_IP, str(self.SERVER_PORT))
 
         # Compute PUBLIC reference towards the current web application, it will be used in the emails text
         self.BASE_URL = ""
         self.DEPLOY_CONTEXT = manager.get_attribute(stored.KEY_DEPLOY_CONTEXT, "")
```

### Comparing `tvb-library-2.8.2/tvb/basic/config/stored.py` & `tvb-library-2.9/tvb/basic/config/stored.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 KEY_UPLOAD_PRIVATE_KEY_PATH = 'UPLOAD_KEY_PATH'
 KEY_KC_CONFIGURATION = 'KEYCLOAK_CONFIGURATION'
 KEY_KC_WEB_CONFIGURATION = 'KEYCLOAK_WEB_CONFIGURATION'
 KEY_ENABLE_KC_LOGIN = 'ENABLE_KEYCLOAK_LOGIN'
 KEY_MAX_DISK_SPACE_USR = 'USR_DISK_SPACE'
 KEY_IP = 'SERVER_IP'
 KEY_PORT = 'WEB_SERVER_PORT'
+KEY_PORT_REST = 'REST_SERVER_PORT'
 KEY_SELECTED_DB = 'SELECTED_DB'
 KEY_DB_URL = 'URL_VALUE'
 KEY_MAX_CONNECTIONS = 'MAX_CONNECTIONS'
 KEY_MAX_ASYNC_CONNECTIONS = 'MAX_ASYNC_CONNECTIONS'
 KEY_URL_VERSION = 'URL_TVB_VERSION'
 KEY_CLUSTER = 'DEPLOY_CLUSTER'
 KEY_CLUSTER_SCHEDULER = 'CLUSTER_SCHEDULER'
@@ -67,19 +68,19 @@
 KEY_LAST_CHECKED_FILE_VERSION = 'LAST_CHECKED_FILE_VERSION'
 KEY_LAST_CHECKED_CODE_VERSION = 'LAST_CHECKED_CODE_VERSION'
 KEY_FILE_STORAGE_UPDATE_STATUS = 'FILE_STORAGE_UPDATE_STATUS'
 KEY_TRACE_USER_ACTIONS = "TRACE_USER_ACTIONS"
 KEY_ENCRYPT_STORAGE = "ENCRYPT_STORAGE"
 KEY_DECRYPT_PATH = "DECRYPT_PATH"
 KEY_FILE_STORAGE = "FILE_STORAGE"
-KEY_OPENSHIFT_DEPLOY = "OPENSHIFT_DEPLOY"
-KEY_OPENSHIFT_NAMESPACE = "OPENSHIFT_NAMESPACE"
-KEY_OPENSHIFT_APPLICATION = "OPENSHIFT_APPLICATION"
-KEY_PROCESSING_OPERATIONS_APPLICATION = "PROCESSING_OPERATIONS_APPLICATION"
-KEY_DATA_ENCRYPTION_HANDLER_APPLICATION = "DATA_ENCRYPTION_HANDLER_APPLICATION"
+KEY_IS_CLOUD_DEPLOY = "IS_CLOUD_DEPLOY"
+KEY_IS_CLOUD_HTTPS = "IS_CLOUD_HTTPS"
+KEY_CLOUD_APP_EXEC = "PROCESSING_OPERATIONS_APPLICATION"
+KEY_CLOUD_APP_EXEC_MAX_PODS = "PROCESSING_OPERATIONS_PODS_MAX_NO"
+KEY_CLOUD_APP_ENCRYPTION_HANDLER = "DATA_ENCRYPTION_HANDLER_APPLICATION"
 KEY_DEPLOY_CONTEXT = "DEPLOY_CONTEXT"
 KEY_REST_DEPLOY_CONTEXT = "REST_DEPLOY_CONTEXT"
 KEY_ELASTICSEARCH_API_KEY = "ELASTICSEARCH_API_KEY"
 KEY_ELASTICSEARCH_URL = "ELASTICSEARCH_URL"
 KEY_ELASTICSEARCH_LOGGING_INDEX = "ELASTICSEARCH_LOGGING_INDEX"
 KEY_ELASTICSEARCH_REQUEST_TIMEOUT = "ELASTICSEARCH_REQUEST_TIMEOUT"
 KEY_ELASTICSEARCH_BUFFER_THRESHOLD = "ELASTICSEARCH_BUFFER_THRESHOLD"
```

### Comparing `tvb-library-2.8.2/tvb/basic/config/utils.py` & `tvb-library-2.9/tvb/basic/config/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/exceptions.py` & `tvb-library-2.9/tvb/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/logger/builder.py` & `tvb-library-2.9/tvb/basic/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/logger/library_logger.conf` & `tvb-library-2.9/tvb/basic/logger/library_logger.conf`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/logger/library_logger_test.conf` & `tvb-library-2.9/tvb/basic/logger/library_logger_test.conf`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/logger/simple_handler.py` & `tvb-library-2.9/tvb/basic/logger/simple_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/__init__.py` & `tvb-library-2.9/tvb/basic/neotraits/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/_attr.py` & `tvb-library-2.9/tvb/basic/neotraits/_attr.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/_core.py` & `tvb-library-2.9/tvb/basic/neotraits/_core.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/_declarative_base.py` & `tvb-library-2.9/tvb/basic/neotraits/_declarative_base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/api.py` & `tvb-library-2.9/tvb/basic/neotraits/api.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/ex.py` & `tvb-library-2.9/tvb/basic/neotraits/ex.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/neotraits/info.py` & `tvb-library-2.9/tvb/basic/neotraits/info.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/profile.py` & `tvb-library-2.9/tvb/basic/profile.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/basic/readers.py` & `tvb-library-2.9/tvb/basic/readers.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/__init__.py` & `tvb-library-2.9/tvb/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/connectivity.py` & `tvb-library-2.9/tvb/datatypes/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/cortex.py` & `tvb-library-2.9/tvb/datatypes/cortex.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/equations.py` & `tvb-library-2.9/tvb/datatypes/equations.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/fcd.py` & `tvb-library-2.9/tvb/datatypes/fcd.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/graph.py` & `tvb-library-2.9/tvb/datatypes/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/local_connectivity.py` & `tvb-library-2.9/tvb/datatypes/local_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/mode_decompositions.py` & `tvb-library-2.9/tvb/datatypes/mode_decompositions.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/patterns.py` & `tvb-library-2.9/tvb/datatypes/patterns.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/projections.py` & `tvb-library-2.9/tvb/datatypes/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/region_mapping.py` & `tvb-library-2.9/tvb/datatypes/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/sensors.py` & `tvb-library-2.9/tvb/datatypes/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/spectral.py` & `tvb-library-2.9/tvb/datatypes/spectral.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/structural.py` & `tvb-library-2.9/tvb/datatypes/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/surfaces.py` & `tvb-library-2.9/tvb/datatypes/surfaces.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/temporal_correlations.py` & `tvb-library-2.9/tvb/datatypes/temporal_correlations.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/time_series.py` & `tvb-library-2.9/tvb/datatypes/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/tracts.py` & `tvb-library-2.9/tvb/datatypes/tracts.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/datatypes/volumes.py` & `tvb-library-2.9/tvb/datatypes/volumes.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/README.md` & `tvb-library-2.9/tvb/rateML/README.md`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XML2model.py` & `tvb-library-2.9/tvb/rateML/XML2model.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/epileptor.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/epileptor.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/kuramoto.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/kuramoto.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/model_template.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/model_template.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/montbrio.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/montbrio.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/oscillator.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/oscillator.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/rwongwang.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/rwongwang.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/rwongwang_deco.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/rwongwang_deco.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/XMLmodels/zerlaut.xml` & `tvb-library-2.9/tvb/rateML/XMLmodels/zerlaut.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/epileptorref.c` & `tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/epileptorref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c` & `tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/montbrioref.c` & `tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/montbrioref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c` & `tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c` & `tvb-library-2.9/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/epileptor.c` & `tvb-library-2.9/tvb/rateML/generatedModels/epileptor.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/epileptor.py` & `tvb-library-2.9/tvb/rateML/generatedModels/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/kuramoto.c` & `tvb-library-2.9/tvb/rateML/generatedModels/kuramoto.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/kuramoto.py` & `tvb-library-2.9/tvb/rateML/generatedModels/kuramoto.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio.c` & `tvb-library-2.9/tvb/rateML/generatedModels/montbrio.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio.py` & `tvb-library-2.9/tvb/rateML/generatedModels/montbrio.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/montbrio_heun.c` & `tvb-library-2.9/tvb/rateML/generatedModels/montbrio_heun.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/oscillator.c` & `tvb-library-2.9/tvb/rateML/generatedModels/oscillator.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/oscillator.py` & `tvb-library-2.9/tvb/rateML/generatedModels/oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/rwongwang.c` & `tvb-library-2.9/tvb/rateML/generatedModels/rwongwang.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/rwongwang.py` & `tvb-library-2.9/tvb/rateML/generatedModels/rwongwang.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/zerlaut.c` & `tvb-library-2.9/tvb/rateML/generatedModels/zerlaut.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/generatedModels/zerlaut_func.h` & `tvb-library-2.9/tvb/rateML/generatedModels/zerlaut_func.h`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/rML_v0.xsd` & `tvb-library-2.9/tvb/rateML/rML_v0.xsd`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/run/model_driver.py` & `tvb-library-2.9/tvb/rateML/run/model_driver.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/run/model_driver_bold.py` & `tvb-library-2.9/tvb/rateML/run/model_driver_bold.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/run/model_driver_heun.py` & `tvb-library-2.9/tvb/rateML/run/model_driver_heun.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/run/model_driver_zerlaut.py` & `tvb-library-2.9/tvb/rateML/run/model_driver_zerlaut.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/run/regular_run.py` & `tvb-library-2.9/tvb/rateML/run/regular_run.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/tmpl8_cuda.py` & `tvb-library-2.9/tvb/rateML/tmpl8_cuda.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/tmpl8_driver.py` & `tvb-library-2.9/tvb/rateML/tmpl8_driver.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/rateML/tmpl8_python.py` & `tvb-library-2.9/tvb/rateML/tmpl8_python.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/__init__.py` & `tvb-library-2.9/tvb/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/coupling.py` & `tvb-library-2.9/tvb/simulator/_numba/coupling.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/gpu_bench.py` & `tvb-library-2.9/tvb/simulator/_numba/gpu_bench.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/integrators.py` & `tvb-library-2.9/tvb/simulator/_numba/integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/loops.py` & `tvb-library-2.9/tvb/simulator/_numba/loops.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/models.py` & `tvb-library-2.9/tvb/simulator/_numba/models.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/_numba/util.py` & `tvb-library-2.9/tvb/simulator/_numba/util.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/__init__.py` & `tvb-library-2.9/tvb/simulator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/base.py` & `tvb-library-2.9/tvb/simulator/backend/base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/cu.py` & `tvb-library-2.9/tvb/simulator/backend/cu.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/nb.py` & `tvb-library-2.9/tvb/simulator/backend/nb.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/nb_mpr.py` & `tvb-library-2.9/tvb/simulator/backend/nb_mpr.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/np.py` & `tvb-library-2.9/tvb/simulator/backend/np.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/ref.py` & `tvb-library-2.9/tvb/simulator/backend/ref.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/__init__.py` & `tvb-library-2.9/tvb/simulator/backend/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/cu-base.cu.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/cu-base.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/cu-coupling.cu.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/cu-coupling.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/cu-defs.cu.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/cu-defs.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/cu-dfuns.cu.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/cu-dfuns.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/cu-sim-ode.cu.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/cu-sim-ode.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-coupling.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-coupling.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-coupling2.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-coupling2.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-dfuns.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-dfuns.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-integrate.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-integrate.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-montbrio.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-montbrio.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/nb-sim.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/nb-sim.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/np-coupling.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/np-coupling.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/np-dfuns.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/np-dfuns.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/np-integrate.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/np-integrate.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/backend/templates/np-sim.py.mako` & `tvb-library-2.9/tvb/simulator/backend/templates/np-sim.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/common.py` & `tvb-library-2.9/tvb/simulator/common.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/coupling.py` & `tvb-library-2.9/tvb/simulator/coupling.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/descriptors.py` & `tvb-library-2.9/tvb/simulator/descriptors.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/history.py` & `tvb-library-2.9/tvb/simulator/history.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/integrators.py` & `tvb-library-2.9/tvb/simulator/integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/lab.py` & `tvb-library-2.9/tvb/simulator/lab.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/__init__.py` & `tvb-library-2.9/tvb/simulator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/base.py` & `tvb-library-2.9/tvb/simulator/models/base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/epileptor.py` & `tvb-library-2.9/tvb/simulator/models/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/epileptor_rs.py` & `tvb-library-2.9/tvb/simulator/models/epileptor_rs.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/epileptorcodim3.py` & `tvb-library-2.9/tvb/simulator/models/epileptorcodim3.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/hopfield.py` & `tvb-library-2.9/tvb/simulator/models/hopfield.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/infinite_theta.py` & `tvb-library-2.9/tvb/simulator/models/infinite_theta.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/jansen_rit.py` & `tvb-library-2.9/tvb/simulator/models/jansen_rit.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/k_ion_exchange.py` & `tvb-library-2.9/tvb/simulator/models/k_ion_exchange.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/larter_breakspear.py` & `tvb-library-2.9/tvb/simulator/models/larter_breakspear.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/linear.py` & `tvb-library-2.9/tvb/simulator/models/linear.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/oscillator.py` & `tvb-library-2.9/tvb/simulator/models/oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/stefanescu_jirsa.py` & `tvb-library-2.9/tvb/simulator/models/stefanescu_jirsa.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/wilson_cowan.py` & `tvb-library-2.9/tvb/simulator/models/wilson_cowan.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/wong_wang.py` & `tvb-library-2.9/tvb/simulator/models/wong_wang.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/wong_wang_exc_inh.py` & `tvb-library-2.9/tvb/simulator/models/wong_wang_exc_inh.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/models/zerlaut.py` & `tvb-library-2.9/tvb/simulator/models/zerlaut.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/monitors.py` & `tvb-library-2.9/tvb/simulator/monitors.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/noise.py` & `tvb-library-2.9/tvb/simulator/noise.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/base_plotter.py` & `tvb-library-2.9/tvb/simulator/plot/base_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/colourmaps/BlackToBlue` & `tvb-library-2.9/tvb/simulator/plot/colourmaps/BlackToBlue`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/compare_integrators.py` & `tvb-library-2.9/tvb/simulator/plot/compare_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/config.py` & `tvb-library-2.9/tvb/simulator/plot/config.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/epileptor_plotter.py` & `tvb-library-2.9/tvb/simulator/plot/epileptor_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/head_plotter.py` & `tvb-library-2.9/tvb/simulator/plot/head_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/head_plotter_3d.py` & `tvb-library-2.9/tvb/simulator/plot/head_plotter_3d.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/phase_plane_interactive.py` & `tvb-library-2.9/tvb/simulator/plot/phase_plane_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/plotter.py` & `tvb-library-2.9/tvb/simulator/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/power_spectra_interactive.py` & `tvb-library-2.9/tvb/simulator/plot/power_spectra_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/time_series_plotter.py` & `tvb-library-2.9/tvb/simulator/plot/time_series_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/timeseries_interactive.py` & `tvb-library-2.9/tvb/simulator/plot/timeseries_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/tools.py` & `tvb-library-2.9/tvb/simulator/plot/tools.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/plot/utils.py` & `tvb-library-2.9/tvb/simulator/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/simulator/simulator.py` & `tvb-library-2.9/tvb/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/__init__.py` & `tvb-library-2.9/tvb/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/bench.py` & `tvb-library-2.9/tvb/tests/bench.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/bench_against_mpr_backend.py` & `tvb-library-2.9/tvb/tests/bench_against_mpr_backend.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/__init__.py` & `tvb-library-2.9/tvb/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/base_testcase.py` & `tvb-library-2.9/tvb/tests/library/base_testcase.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/basic/neotraits/_attr_test.py` & `tvb-library-2.9/tvb/tests/library/basic/neotraits/_attr_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/basic/neotraits/neotraits_test.py` & `tvb-library-2.9/tvb/tests/library/basic/neotraits/neotraits_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/Edited_Connectivity.h5` & `tvb-library-2.9/tvb/tests/library/datatypes/Edited_Connectivity.h5`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/connectivity_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/connectivity_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/equations_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/equations_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/graph_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/graph_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/mode_decompositions_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/mode_decompositions_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/patterns_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/patterns_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/projections_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/projections_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/sensors_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/sensors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/spectral_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/spectral_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/surfaces_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/surfaces_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/temporal_correlations_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/temporal_correlations_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/timeseries_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/timeseries_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/datatypes/volumes_test.py` & `tvb-library-2.9/tvb/tests/library/datatypes/volumes_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/_numba_tests.py` & `tvb-library-2.9/tvb/tests/library/simulator/_numba_tests.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/_opencl_tests.py` & `tvb-library-2.9/tvb/tests/library/simulator/_opencl_tests.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/backendtestbase.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/backendtestbase.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/cubackend_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/cubackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbbackend_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/nbbackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/nbmprperf_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/nbmprperf_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/backend/npbackend_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/backend/npbackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/common_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/common_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/coupling_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/coupling_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/descriptors_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/descriptors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/history_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/history_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/integrators_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/integrators_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/modelir_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/modelir_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/models_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/models_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/monitors_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/monitors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/noise_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/noise_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/rateml_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/rateml_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/regionmapping_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/regionmapping_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/rngperf_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/rngperf_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/simulator_step_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/simulator_step_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/simulator_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/simulator_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/library/simulator/stimulation_test.py` & `tvb-library-2.9/tvb/tests/library/simulator/stimulation_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb/tests/validate_model_parameters.py` & `tvb-library-2.9/tvb/tests/validate_model_parameters.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8.2/tvb_library.egg-info/PKG-INFO` & `tvb-library-2.9/tvb_library.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 Metadata-Version: 2.1
 Name: tvb-library
-Version: 2.8.2
+Version: 2.9
 Summary: A package for performing whole brain simulations
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience human animal neuronal dynamics models delay
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: autopep8
+Requires-Dist: Deprecated
+Requires-Dist: docutils
+Requires-Dist: ipywidgets
+Requires-Dist: lxml
+Requires-Dist: mako>=1.1.4
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: numba
+Requires-Dist: numexpr
+Requires-Dist: numpy
+Requires-Dist: pylems
+Requires-Dist: scipy
+Requires-Dist: six
+Provides-Extra: test
+Requires-Dist: h5py; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: tvb-gdist; extra == "test"
+Requires-Dist: tvb-data; extra == "test"
 
 THE VIRTUAL BRAIN SCIENTIFIC LIBRARY
 ====================================
 
 The Virtual Brain Project (TVB Project) has the purpose of offering some
 modern tools to the Neurosciences community, for computing, simulating
 and analyzing functional and structural data of human brains.
```

### Comparing `tvb-library-2.8.2/tvb_library.egg-info/SOURCES.txt` & `tvb-library-2.9/tvb_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

