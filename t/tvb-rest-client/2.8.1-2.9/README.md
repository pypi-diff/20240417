# Comparing `tmp/tvb-rest-client-2.8.1.tar.gz` & `tmp/tvb-rest-client-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-rest-client-2.8.1.tar", last modified: Tue May 23 12:09:33 2023, max compression
+gzip compressed data, was "tvb-rest-client-2.9.tar", last modified: Fri Apr 12 19:21:42 2024, max compression
```

## Comparing `tvb-rest-client-2.8.1.tar` & `tvb-rest-client-2.9.tar`

### file list

```diff
@@ -1,385 +1,386 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.567260 tvb-rest-client-2.8.1/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/MANIFEST_rest_client.in
--rw-r--r--   0 root         (0) root         (0)     4288 2023-05-23 12:09:33.566260 tvb-rest-client-2.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4235 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     3716 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/README_rest_client.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:33.567260 tvb-rest-client-2.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3133 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.404252 tvb-rest-client-2.8.1/tvb/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.404252 tvb-rest-client-2.8.1/tvb/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.410252 tvb-rest-client-2.8.1/tvb/adapters/analyzers/
--rw-r--r--   0 root         (0) root         (0)     1811 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8953 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_adapters.py
--rw-r--r--   0 root         (0) root         (0)     9731 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_centrality_adapters.py
--rw-r--r--   0 root         (0) root         (0)     5845 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_clustering_adapters.py
--rw-r--r--   0 root         (0) root         (0)     8009 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_degree_adapters.py
--rw-r--r--   0 root         (0) root         (0)    17019 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/cross_correlation_adapter.py
--rw-r--r--   0 root         (0) root         (0)    20045 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fcd_adapter.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fmri_balloon_adapter.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fourier_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/ica_adapter.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/metrics_group_timeseries.py
--rw-r--r--   0 root         (0) root         (0)     7956 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_coherence_adapter.py
--rw-r--r--   0 root         (0) root         (0)    11026 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_complex_coherence_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_covariance_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7446 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/pca_adapter.py
--rw-r--r--   0 root         (0) root         (0)    11610 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/wavelet_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.413253 tvb-rest-client-2.8.1/tvb/adapters/creators/
--rw-r--r--   0 root         (0) root         (0)     1377 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33529 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/allen_creator.py
--rw-r--r--   0 root         (0) root         (0)    11384 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/connectivity_creator.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/local_connectivity_creator.py
--rw-r--r--   0 root         (0) root         (0)    21351 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_base.py
--rw-r--r--   0 root         (0) root         (0)     9827 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_creator.py
--rw-r--r--   0 root         (0) root         (0)    12706 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/stimulus_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.413253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.421253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/
--rw-r--r--   0 root         (0) root         (0)     2553 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5450 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/annotation.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/fcd.py
--rw-r--r--   0 root         (0) root         (0)     5801 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/graph.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     3795 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mapped_value.py
--rw-r--r--   0 root         (0) root         (0)     3742 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mode_decompositions.py
--rw-r--r--   0 root         (0) root         (0)     3680 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/patterns.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/projections.py
--rw-r--r--   0 root         (0) root         (0)     5471 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/region_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.424253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/
--rw-r--r--   0 root         (0) root         (0)     3568 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_region_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2949 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_sensor.py
--rw-r--r--   0 root         (0) root         (0)     4074 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_surface.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_timeseries.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_volume.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/sensors.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/simulation_history.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/spectral.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/structural.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/surface.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/temporal_correlations.py
--rw-r--r--   0 root         (0) root         (0)    12512 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/tracts.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.433254 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/annotation_h5.py
--rw-r--r--   0 root         (0) root         (0)     3086 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/connectivity_h5.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/fcd_h5.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/graph_h5.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/local_connectivity_h5.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mapped_value_h5.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mode_decompositions_h5.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/patterns_h5.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/projections_h5.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/region_mapping_h5.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/sensors_h5.py
--rw-r--r--   0 root         (0) root         (0)     8931 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/spectral_h5.py
--rw-r--r--   0 root         (0) root         (0)     3663 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/structural_h5.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/surface_h5.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/temporal_correlations_h5.py
--rw-r--r--   0 root         (0) root         (0)    14867 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/time_series_h5.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/tracts_h5.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/volumes_h5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.436254 tvb-rest-client-2.8.1/tvb/adapters/exporters/
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8179 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/abcexporter.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/export_manager.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_export.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_linked_export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.442254 tvb-rest-client-2.8.1/tvb/adapters/forms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4713 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/coupling_forms.py
--rw-r--r--   0 root         (0) root         (0)     7218 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/equation_forms.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/equation_plot_forms.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/form_with_ranges.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/integrator_forms.py
--rw-r--r--   0 root         (0) root         (0)    42482 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/model_forms.py
--rw-r--r--   0 root         (0) root         (0)    10872 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/monitor_forms.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/noise_forms.py
--rw-r--r--   0 root         (0) root         (0)    16528 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/simulator_fragments.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/surface_model_parameters_form.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/transfer_vector_form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.444254 tvb-rest-client-2.8.1/tvb/adapters/simulator/
--rw-r--r--   0 root         (0) root         (0)     1275 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7644 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/hpc_simulator_adapter.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/range_parameters.py
--rw-r--r--   0 root         (0) root         (0)    14600 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/simulator_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.452255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/
--rw-r--r--   0 root         (0) root         (0)     1877 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/bids_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.453255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5884 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/parser.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco_importer.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/connectivity_measure_importer.py
--rw-r--r--   0 root         (0) root         (0)     8851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/csv_connectivity_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.454255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8341 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/parser.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_surface_importer.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_timeseries_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.455255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/parser.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py
--rw-r--r--   0 root         (0) root         (0)     9047 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.456255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6830 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/parser.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.457255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3244 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/parser.py
--rw-r--r--   0 root         (0) root         (0)    10869 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.458255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/parser.py
--rw-r--r--   0 root         (0) root         (0)     3863 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/surface.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj_importer.py
--rw-r--r--   0 root         (0) root         (0)     7796 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/projection_matrix_importer.py
--rw-r--r--   0 root         (0) root         (0)     7637 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/region_mapping_importer.py
--rw-r--r--   0 root         (0) root         (0)     5676 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/sensors_importer.py
--rw-r--r--   0 root         (0) root         (0)    10129 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tract_importer.py
--rw-r--r--   0 root         (0) root         (0)    10997 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tumor_dataset_importer.py
--rw-r--r--   0 root         (0) root         (0)     7532 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tvb_importer.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_connectivity_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.459255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6445 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/parser.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.477256 tvb-rest-client-2.8.1/tvb/adapters/visualizers/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12080 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/annotations_viewer.py
--rw-r--r--   0 root         (0) root         (0)    21242 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/brain.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/complex_imaginary_coherence.py
--rw-r--r--   0 root         (0) root         (0)    24356 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     3548 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity_edge_bundle.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_coherence.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_correlation.py
--rw-r--r--   0 root         (0) root         (0)    17334 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/eeg_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5293 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/fourier_spectrum.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/histogram.py
--rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/ica.py
--rw-r--r--   0 root         (0) root         (0)     4520 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/local_connectivity_view.py
--rw-r--r--   0 root         (0) root         (0)     8139 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/matrix_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pca.py
--rw-r--r--   0 root         (0) root         (0)     4768 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_cross_correlation.py
--rw-r--r--   0 root         (0) root         (0)     3969 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_edge_bundle.py
--rw-r--r--   0 root         (0) root         (0)    11964 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/phase_plane_interactive.py
--rw-r--r--   0 root         (0) root         (0)    17234 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse.py
--rw-r--r--   0 root         (0) root         (0)     4398 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_discrete.py
--rw-r--r--   0 root         (0) root         (0)     8421 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_isocline.py
--rw-r--r--   0 root         (0) root         (0)    25048 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/region_volume_mapping.py
--rw-r--r--   0 root         (0) root         (0)    10855 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/sensors.py
--rw-r--r--   0 root         (0) root         (0)    25212 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/surface_view.py
--rw-r--r--   0 root         (0) root         (0)     7919 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series.py
--rw-r--r--   0 root         (0) root         (0)     8697 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series_volume.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/topographic.py
--rw-r--r--   0 root         (0) root         (0)     4565 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/tract.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/wavelet_spectrogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.478256 tvb-rest-client-2.8.1/tvb/config/
--rw-r--r--   0 root         (0) root         (0)     2391 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/algorithm_categories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.481256 tvb-rest-client-2.8.1/tvb/config/init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.481256 tvb-rest-client-2.8.1/tvb/config/init/alembic/
--rw-r--r--   0 root         (0) root         (0)     2238 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.484256 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12427 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/datatypes_registry.py
--rw-r--r--   0 root         (0) root         (0)     9460 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/initializer.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/introspector_registry.py
--rw-r--r--   0 root         (0) root         (0)     5505 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/model_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.486256 tvb-rest-client-2.8.1/tvb/config/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/cluster_handler.py
--rw-r--r--   0 root         (0) root         (0)     3465 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/dev_logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5445 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/elasticsearch_handler.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5820 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/profile_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.489256 tvb-rest-client-2.8.1/tvb/core/
--rw-r--r--   0 root         (0) root         (0)     1571 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.493257 tvb-rest-client-2.8.1/tvb/core/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22960 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcadapter.py
--rw-r--r--   0 root         (0) root         (0)     8032 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcdisplayer.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcremover.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcuploader.py
--rw-r--r--   0 root         (0) root         (0)     5639 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/arguments_serialisation.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/constants.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/inputs_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.495257 tvb-rest-client-2.8.1/tvb/core/code_versions/
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/base_classes.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.499257 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/
--rw-r--r--   0 root         (0) root         (0)     3101 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4455_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4750_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/5454_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6093_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6600_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6728_update_code.py
--rw-r--r--   0 root         (0) root         (0)     9996 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7350_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7450_update_code.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/9444_update_code.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.502257 tvb-rest-client-2.8.1/tvb/core/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/exportable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.503257 tvb-rest-client-2.8.1/tvb/core/entities/file/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.507257 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/
--rw-r--r--   0 root         (0) root         (0)    10820 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/002_update_files.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/003_update_files.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/004_update_files.py
--rw-r--r--   0 root         (0) root         (0)    69315 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/005_update_files.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11892 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/files_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.510257 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/burst_configuration_h5.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/datatype_measure_h5.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/simulation_history_h5.py
--rw-r--r--   0 root         (0) root         (0)    12551 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/view_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.512257 tvb-rest-client-2.8.1/tvb/core/entities/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14738 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/chain.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/factory.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/generic_attributes.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.515258 tvb-rest-client-2.8.1/tvb/core/entities/model/
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5744 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_burst.py
--rw-r--r--   0 root         (0) root         (0)    16256 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_datatype.py
--rw-r--r--   0 root         (0) root         (0)    20454 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_operation.py
--rw-r--r--   0 root         (0) root         (0)     9071 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.520258 tvb-rest-client-2.8.1/tvb/core/entities/storage/
--rw-r--r--   0 root         (0) root         (0)     2179 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/burst_dao.py
--rw-r--r--   0 root         (0) root         (0)    26852 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/datatype_dao.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    23487 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/operation_dao.py
--rw-r--r--   0 root         (0) root         (0)    15003 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/project_dao.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/root_dao.py
--rw-r--r--   0 root         (0) root         (0)    14395 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/session_maker.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/workflow_dao.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.523258 tvb-rest-client-2.8.1/tvb/core/entities/transient/
--rw-r--r--   0 root         (0) root         (0)     1291 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11723 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/context_overlay.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/range_parameter.py
--rw-r--r--   0 root         (0) root         (0)    13225 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/structure_entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.525258 tvb-rest-client-2.8.1/tvb/core/neocom/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17618 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/_h5loader.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/_registry.py
--rw-r--r--   0 root         (0) root         (0)    11003 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/h5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.531258 tvb-rest-client-2.8.1/tvb/core/neotraits/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18223 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/_h5accessors.py
--rw-r--r--   0 root         (0) root         (0)    15188 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/_h5core.py
--rw-r--r--   0 root         (0) root         (0)     4592 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/db.py
--rw-r--r--   0 root         (0) root         (0)    20754 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/forms.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/h5.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/spatial_model.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/uploader_view_model.py
--rw-r--r--   0 root         (0) root         (0)     3466 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/view_model.py
--rw-r--r--   0 root         (0) root         (0)     5224 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/operation_async_launcher.py
--rw-r--r--   0 root         (0) root         (0)     6933 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/operation_hpc_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.532259 tvb-rest-client-2.8.1/tvb/core/project_versions/
--rw-r--r--   0 root         (0) root         (0)     1407 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.534259 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/
--rw-r--r--   0 root         (0) root         (0)     3200 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/1_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/2_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/3_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/removers_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.543259 tvb-rest-client-2.8.1/tvb/core/services/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17253 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/algorithm_service.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/authorization.py
--rw-r--r--   0 root         (0) root         (0)     3455 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_client_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.545259 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/backend_client.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/cluster_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)    20257 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/hpc_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)    11834 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/standalone_client.py
--rw-r--r--   0 root         (0) root         (0)     4063 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/burst_config_serialization.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/burst_service.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/email_sender.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8322 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/figure_service.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/hpc_operation_service.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/import_service.py
--rw-r--r--   0 root         (0) root         (0)    19683 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/operation_service.py
--rw-r--r--   0 root         (0) root         (0)    49199 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/project_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.546259 tvb-rest-client-2.8.1/tvb/core/services/resources/
--rw-r--r--   0 root         (0) root         (0)    20092 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.png
--rw-r--r--   0 root         (0) root         (0)    21014 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.svg
--rw-r--r--   0 root         (0) root         (0)    13153 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/settings_service.py
--rw-r--r--   0 root         (0) root         (0)    14266 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/simulator_service.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/texture_to_json.py
--rw-r--r--   0 root         (0) root         (0)    16498 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/user_service.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.547259 tvb-rest-client-2.8.1/tvb/interfaces/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.547259 tvb-rest-client-2.8.1/tvb/interfaces/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.550259 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
--rw-r--r--   0 root         (0) root         (0)     8764 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.551259 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10056 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.553259 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/client_decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.553259 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/
--rw-r--r--   0 root         (0) root         (0)     5682 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/datatype_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.555260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/
--rw-r--r--   0 root         (0) root         (0)     7767 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/fire_simulation.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/launch_operation.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/utils.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/main_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.555260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/
--rw-r--r--   0 root         (0) root         (0)     4096 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/operation_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.556260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/
--rw-r--r--   0 root         (0) root         (0)     2868 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/project_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.557260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/
--rw-r--r--   0 root         (0) root         (0)     2500 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/simulation_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.558260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/rest_test.py
--rw-r--r--   0 root         (0) root         (0)    11305 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tvb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.559260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.562260 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/decoders.py
--rw-r--r--   0 root         (0) root         (0)     5717 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/dtos.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/files_helper.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.565260 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4288 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13697 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.906287 tvb-rest-client-2.9/
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/MANIFEST_rest_client.in
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-12 19:21:42.906287 tvb-rest-client-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4206 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/README_rest_client.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 19:21:42.906287 tvb-rest-client-2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3192 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.817282 tvb-rest-client-2.9/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.817282 tvb-rest-client-2.9/tvb/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.826283 tvb-rest-client-2.9/tvb/adapters/analyzers/
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/bct_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     9731 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/bct_centrality_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     5845 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/bct_clustering_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     8009 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/bct_degree_adapters.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/cross_correlation_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    20045 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/fcd_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/fmri_balloon_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/fourier_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/ica_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/metrics_group_timeseries.py
+-rw-r--r--   0 root         (0) root         (0)     7956 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/node_coherence_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    11026 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/node_complex_coherence_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/node_covariance_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7446 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/pca_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    11610 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/analyzers/wavelet_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.828283 tvb-rest-client-2.9/tvb/adapters/creators/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33529 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/allen_creator.py
+-rw-r--r--   0 root         (0) root         (0)    11384 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/connectivity_creator.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/local_connectivity_creator.py
+-rw-r--r--   0 root         (0) root         (0)    20682 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/siibra_base.py
+-rw-r--r--   0 root         (0) root         (0)     9585 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/siibra_creator.py
+-rw-r--r--   0 root         (0) root         (0)    12706 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/creators/stimulus_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.828283 tvb-rest-client-2.9/tvb/adapters/datatypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.833283 tvb-rest-client-2.9/tvb/adapters/datatypes/db/
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/annotation.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/fcd.py
+-rw-r--r--   0 root         (0) root         (0)     5801 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/mapped_value.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/mode_decompositions.py
+-rw-r--r--   0 root         (0) root         (0)     3680 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/projections.py
+-rw-r--r--   0 root         (0) root         (0)     5471 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/region_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.835283 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/
+-rw-r--r--   0 root         (0) root         (0)     3568 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2949 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_surface.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_timeseries.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_volume.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/sensors.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/simulation_history.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/spectral.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/structural.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/surface.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/temporal_correlations.py
+-rw-r--r--   0 root         (0) root         (0)    12512 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/tracts.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/db/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.840283 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/annotation_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/connectivity_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/fcd_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/graph_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/local_connectivity_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/mapped_value_h5.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/mode_decompositions_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/patterns_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/projections_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/region_mapping_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/sensors_h5.py
+-rw-r--r--   0 root         (0) root         (0)     8931 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/spectral_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3663 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/structural_h5.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/surface_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/temporal_correlations_h5.py
+-rw-r--r--   0 root         (0) root         (0)    14867 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/time_series_h5.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/tracts_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/datatypes/h5/volumes_h5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.841283 tvb-rest-client-2.9/tvb/adapters/exporters/
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/abcexporter.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/export_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/tvb_export.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/exporters/tvb_linked_export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.844283 tvb-rest-client-2.9/tvb/adapters/forms/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4713 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/coupling_forms.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/equation_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/equation_plot_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/form_with_ranges.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/integrator_forms.py
+-rw-r--r--   0 root         (0) root         (0)    42482 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/model_forms.py
+-rw-r--r--   0 root         (0) root         (0)    10872 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/monitor_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/noise_forms.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/simulator_fragments.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/surface_model_parameters_form.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/forms/transfer_vector_form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.845283 tvb-rest-client-2.9/tvb/adapters/simulator/
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7644 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/simulator/hpc_simulator_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/simulator/range_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    14600 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/simulator/simulator_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.851284 tvb-rest-client-2.9/tvb/adapters/uploaders/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/bids_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.852284 tvb-rest-client-2.9/tvb/adapters/uploaders/brco/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/brco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5884 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/brco/parser.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/brco_importer.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/connectivity_measure_importer.py
+-rw-r--r--   0 root         (0) root         (0)     8850 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/csv_connectivity_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.852284 tvb-rest-client-2.9/tvb/adapters/uploaders/gifti/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/gifti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8341 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/gifti/parser.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/gifti_surface_importer.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/gifti_timeseries_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.852284 tvb-rest-client-2.9/tvb/adapters/uploaders/mat/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/mat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/mat/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py
+-rw-r--r--   0 root         (0) root         (0)     9047 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/mat_timeseries_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.853284 tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_connectivity/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_connectivity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_connectivity/parser.py
+-rw-r--r--   0 root         (0) root         (0)     5062 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.853284 tvb-rest-client-2.9/tvb/adapters/uploaders/nifti/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/nifti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/nifti/parser.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/nifti_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.854284 tvb-rest-client-2.9/tvb/adapters/uploaders/obj/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/obj/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/obj/parser.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/obj/surface.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/obj_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7796 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/projection_matrix_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7637 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/region_mapping_importer.py
+-rw-r--r--   0 root         (0) root         (0)     5676 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/sensors_importer.py
+-rw-r--r--   0 root         (0) root         (0)    10129 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/tract_importer.py
+-rw-r--r--   0 root         (0) root         (0)    10997 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/tumor_dataset_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7532 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/tvb_importer.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/zip_connectivity_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.854284 tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6445 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface/parser.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.861284 tvb-rest-client-2.9/tvb/adapters/visualizers/
+-rw-r--r--   0 root         (0) root         (0)     1955 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12080 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/annotations_viewer.py
+-rw-r--r--   0 root         (0) root         (0)    21242 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/brain.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/complex_imaginary_coherence.py
+-rw-r--r--   0 root         (0) root         (0)    24356 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/connectivity_edge_bundle.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/cross_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/cross_correlation.py
+-rw-r--r--   0 root         (0) root         (0)    17334 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/eeg_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/fourier_spectrum.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/histogram.py
+-rw-r--r--   0 root         (0) root         (0)     4662 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/ica.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/local_connectivity_view.py
+-rw-r--r--   0 root         (0) root         (0)     8139 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/matrix_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pca.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pearson_cross_correlation.py
+-rw-r--r--   0 root         (0) root         (0)     3969 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pearson_edge_bundle.py
+-rw-r--r--   0 root         (0) root         (0)    11757 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/phase_plane_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    17234 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pse.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pse_discrete.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/pse_isocline.py
+-rw-r--r--   0 root         (0) root         (0)    25048 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/region_volume_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    10855 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    25212 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/surface_view.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     8697 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/time_series_volume.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/topographic.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/tract.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/adapters/visualizers/wavelet_spectrogram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.862284 tvb-rest-client-2.9/tvb/config/
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/algorithm_categories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.863284 tvb-rest-client-2.9/tvb/config/init/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.863284 tvb-rest-client-2.9/tvb/config/init/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.864284 tvb-rest-client-2.9/tvb/config/init/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/versions/32d4bf9f8ghj_update_db_004.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12427 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/datatypes_registry.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/initializer.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/introspector_registry.py
+-rw-r--r--   0 root         (0) root         (0)     5505 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/init/model_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.866284 tvb-rest-client-2.9/tvb/config/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/logger/cluster_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/logger/dev_logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5445 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/logger/elasticsearch_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/logger/logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5820 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/config/profile_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.868285 tvb-rest-client-2.9/tvb/core/
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.870285 tvb-rest-client-2.9/tvb/core/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22960 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/abcadapter.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/abcdisplayer.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/abcremover.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/abcuploader.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/arguments_serialisation.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/adapters/inputs_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.871285 tvb-rest-client-2.9/tvb/core/code_versions/
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/base_classes.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.873285 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)     3101 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/4455_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/4750_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/5454_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6093_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6600_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6728_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     9996 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/7350_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/7450_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/9444_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.874285 tvb-rest-client-2.9/tvb/core/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/exportable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.875285 tvb-rest-client-2.9/tvb/core/entities/file/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.876285 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)    10820 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/002_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/003_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/004_update_files.py
+-rw-r--r--   0 root         (0) root         (0)    69315 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/005_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/files_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.877285 tvb-rest-client-2.9/tvb/core/entities/file/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/simulator/burst_configuration_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/simulator/datatype_measure_h5.py
+-rw-r--r--   0 root         (0) root         (0)     6508 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/simulator/simulation_history_h5.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/file/simulator/view_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.879285 tvb-rest-client-2.9/tvb/core/entities/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14738 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/filters/chain.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/filters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/filters/factory.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/generic_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.880285 tvb-rest-client-2.9/tvb/core/entities/model/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/model/model_burst.py
+-rw-r--r--   0 root         (0) root         (0)    16256 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/model/model_datatype.py
+-rw-r--r--   0 root         (0) root         (0)    20528 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/model/model_operation.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/model/model_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.883285 tvb-rest-client-2.9/tvb/core/entities/storage/
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/burst_dao.py
+-rw-r--r--   0 root         (0) root         (0)    26852 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/datatype_dao.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    23487 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/operation_dao.py
+-rw-r--r--   0 root         (0) root         (0)    15003 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/project_dao.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/root_dao.py
+-rw-r--r--   0 root         (0) root         (0)    14395 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/session_maker.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/storage/workflow_dao.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.884285 tvb-rest-client-2.9/tvb/core/entities/transient/
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/transient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11723 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/transient/context_overlay.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/transient/range_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    13225 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/entities/transient/structure_entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.885285 tvb-rest-client-2.9/tvb/core/neocom/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neocom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17618 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neocom/_h5loader.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neocom/_registry.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neocom/h5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.888286 tvb-rest-client-2.9/tvb/core/neotraits/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/_h5accessors.py
+-rw-r--r--   0 root         (0) root         (0)    15188 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/_h5core.py
+-rw-r--r--   0 root         (0) root         (0)     4592 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/db.py
+-rw-r--r--   0 root         (0) root         (0)    20754 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/h5.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/spatial_model.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/uploader_view_model.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/neotraits/view_model.py
+-rw-r--r--   0 root         (0) root         (0)     5224 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/operation_async_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     6933 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/operation_hpc_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.888286 tvb-rest-client-2.9/tvb/core/project_versions/
+-rw-r--r--   0 root         (0) root         (0)     1407 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/project_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.889286 tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)     3200 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/1_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/2_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/3_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/removers_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.893286 tvb-rest-client-2.9/tvb/core/services/
+-rw-r--r--   0 root         (0) root         (0)     1378 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17253 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/algorithm_service.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_client_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.894286 tvb-rest-client-2.9/tvb/core/services/backend_clients/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_clients/backend_client.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_clients/cluster_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)    20257 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_clients/hpc_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)    12273 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/backend_clients/standalone_client.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/burst_config_serialization.py
+-rw-r--r--   0 root         (0) root         (0)    18549 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/burst_service.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/email_sender.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/figure_service.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/hpc_operation_service.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/import_service.py
+-rw-r--r--   0 root         (0) root         (0)    19683 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/operation_service.py
+-rw-r--r--   0 root         (0) root         (0)    49199 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/project_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.895286 tvb-rest-client-2.9/tvb/core/services/resources/
+-rw-r--r--   0 root         (0) root         (0)    20092 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/resources/branding_bar.png
+-rw-r--r--   0 root         (0) root         (0)    21014 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/resources/branding_bar.svg
+-rw-r--r--   0 root         (0) root         (0)    13376 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/settings_service.py
+-rw-r--r--   0 root         (0) root         (0)    14266 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/simulator_service.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/texture_to_json.py
+-rw-r--r--   0 root         (0) root         (0)    16204 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/services/user_service.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.895286 tvb-rest-client-2.9/tvb/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.895286 tvb-rest-client-2.9/tvb/interfaces/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.896286 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8764 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.897286 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10056 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.898286 tvb-rest-client-2.9/tvb/interfaces/rest/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/client_decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.898286 tvb-rest-client-2.9/tvb/interfaces/rest/client/datatype/
+-rw-r--r--   0 root         (0) root         (0)     5682 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/datatype/datatype_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.899286 tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/
+-rw-r--r--   0 root         (0) root         (0)     7767 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/fire_simulation.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/launch_operation.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/main_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.899286 tvb-rest-client-2.9/tvb/interfaces/rest/client/operation/
+-rw-r--r--   0 root         (0) root         (0)     4096 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/operation/operation_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.900286 tvb-rest-client-2.9/tvb/interfaces/rest/client/project/
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/project/project_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.900286 tvb-rest-client-2.9/tvb/interfaces/rest/client/simulator/
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/simulator/simulation_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.901286 tvb-rest-client-2.9/tvb/interfaces/rest/client/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/tests/rest_test.py
+-rw-r--r--   0 root         (0) root         (0)    11305 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/tvb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.901286 tvb-rest-client-2.9/tvb/interfaces/rest/client/user/
+-rw-r--r--   0 root         (0) root         (0)     4989 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/client/user/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.903286 tvb-rest-client-2.9/tvb/interfaces/rest/commons/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/decoders.py
+-rw-r--r--   0 root         (0) root         (0)     5717 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/dtos.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/files_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2024-04-12 19:06:40.000000 tvb-rest-client-2.9/tvb/interfaces/rest/commons/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:42.905286 tvb-rest-client-2.9/tvb_rest_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-12 19:21:42.000000 tvb-rest-client-2.9/tvb_rest_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13760 2024-04-12 19:21:42.000000 tvb-rest-client-2.9/tvb_rest_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:21:42.000000 tvb-rest-client-2.9/tvb_rest_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-12 19:21:42.000000 tvb-rest-client-2.9/tvb_rest_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-12 19:21:42.000000 tvb-rest-client-2.9/tvb_rest_client.egg-info/top_level.txt
```

### Comparing `tvb-rest-client-2.8.1/AUTHORS` & `tvb-rest-client-2.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/LICENSE` & `tvb-rest-client-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/PKG-INFO` & `tvb-rest-client-2.9/README_rest_client.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tvb-rest-client
-Version: 2.8.1
-Summary: A helper package for preparing and sending requests towards the TVB REST API
-Home-page: https://www.thevirtualbrain.org
-Download-URL: https://github.com/the-virtual-brain/tvb-root
-Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
-Author-email: tvb.admin@thevirtualbrain.org
-License: GPL-3.0-or-later
-Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
-Provides-Extra: postgres
-Provides-Extra: test
-License-File: LICENSE
-License-File: AUTHORS
-
 TVB REST client
 ===============
 
 The `tvb-rest-client` is a helper package built with the intention to simplify a
 Python client interaction with TVB REST Server.
 All the logic necessary to prepare and send requests towards the REST server, is embedded under this client API.
 
@@ -32,15 +17,15 @@
 =====
 You should have a TVB REST server running, or access to a public one.
 Then into `tvb-rest-client` you need to provide the URL towards this TVB REST server.
 For the following example, we will suppose TVB REST server runs on *http://localhost:9090*
 
 To launch a TVB REST server locally, you should download `tvb-framework` version >2.0. and launch it::
 
-    $ python -m tvb.interfaces.web.run WEB_PROFILE  # Launch TVB web and REST servers locally
+    $ python -m tvb.interfaces.rest.server.run   # Launch TVB REST server locally
 
 
 Accessing the client API entry-point
 -------------------------------------
 
 If the TVB REST server you want to access runs at another address, change the parameter
 in the bellow TVBClient instantiation.
@@ -103,8 +88,8 @@
     monitor_operation(tvb_client, operation_gid)
 ..
 
 Acknowledgments
 ===============
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and
 Innovation under the Specific Grant Agreement Nos. 785907 (Human Brain Project SGA2), 945539 (Human Brain Project SGA3)
-and VirtualBrainCloud 826421.
+and VirtualBrainCloud 826421.
```

### Comparing `tvb-rest-client-2.8.1/README.rst` & `tvb-rest-client-2.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 |
                 |
             tvb.config.init
                 |
                 |
             tvb.interfaces
 
-**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/7574266/files/tvb_data.zip?download=1.
+**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/10128131.
 After download, unzip and execute `python setup.py develop` in the correct env.
 
 Usage
 -----
 
 To use TVB code, clone from GitHub (https://github.com/the-virtual-brain/tvb-root), or get from Pypi::
```

### Comparing `tvb-rest-client-2.8.1/README_rest_client.rst` & `tvb-rest-client-2.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: tvb-rest-client
+Version: 2.9
+Summary: A helper package for preparing and sending requests towards the TVB REST API
+Home-page: https://www.thevirtualbrain.org
+Download-URL: https://github.com/the-virtual-brain/tvb-root
+Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
+Author-email: tvb.admin@thevirtualbrain.org
+License: GPL-3.0-or-later
+Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: alembic
+Requires-Dist: h5py
+Requires-Dist: nibabel
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: psutil
+Requires-Dist: pyAesCrypt
+Requires-Dist: requests
+Requires-Dist: scipy
+Requires-Dist: simplejson
+Requires-Dist: sqlalchemy
+Requires-Dist: tvb-data
+Requires-Dist: tvb-gdist
+Requires-Dist: tvb-library
+Requires-Dist: tvb-storage
+Requires-Dist: werkzeug
+Provides-Extra: postgres
+Requires-Dist: psycopg2; extra == "postgres"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
+
 TVB REST client
 ===============
 
 The `tvb-rest-client` is a helper package built with the intention to simplify a
 Python client interaction with TVB REST Server.
 All the logic necessary to prepare and send requests towards the REST server, is embedded under this client API.
 
@@ -17,15 +52,15 @@
 =====
 You should have a TVB REST server running, or access to a public one.
 Then into `tvb-rest-client` you need to provide the URL towards this TVB REST server.
 For the following example, we will suppose TVB REST server runs on *http://localhost:9090*
 
 To launch a TVB REST server locally, you should download `tvb-framework` version >2.0. and launch it::
 
-    $ python -m tvb.interfaces.web.run WEB_PROFILE  # Launch TVB web and REST servers locally
+    $ python -m tvb.interfaces.rest.server.run   # Launch TVB REST server locally
 
 
 Accessing the client API entry-point
 -------------------------------------
 
 If the TVB REST server you want to access runs at another address, change the parameter
 in the bellow TVBClient instantiation.
@@ -88,8 +123,8 @@
     monitor_operation(tvb_client, operation_gid)
 ..
 
 Acknowledgments
 ===============
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and
 Innovation under the Specific Grant Agreement Nos. 785907 (Human Brain Project SGA2), 945539 (Human Brain Project SGA3)
-and VirtualBrainCloud 826421.
+and VirtualBrainCloud 826421.
```

### Comparing `tvb-rest-client-2.8.1/setup.py` & `tvb-rest-client-2.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import shutil
 
 import setuptools
 from setuptools.command.egg_info import manifest_maker
 
 manifest_maker.template = 'MANIFEST_rest_client.in'
 
-VERSION = "2.8.1"
+VERSION = "2.9"
 
 TVB_TEAM = "Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze"
 
 TVB_INSTALL_REQUIREMENTS = ["alembic", "h5py", "nibabel", "numpy", "Pillow", "psutil",
                             "pyAesCrypt", "requests", "scipy", "simplejson", "sqlalchemy",
                             "tvb-data", "tvb-gdist", "tvb-library", "tvb-storage", "werkzeug"]
 
@@ -55,14 +55,15 @@
                               'tvb.interfaces.command.*', 'tvb.tests', 'tvb.tests.*']),
                  include_package_data=True,
                  install_requires=TVB_INSTALL_REQUIREMENTS,
                  extras_require={'postgres': ["psycopg2"],
                                  'test': ["pytest", "pytest-benchmark"]},
                  description='A helper package for preparing and sending requests towards the TVB REST API',
                  long_description=DESCRIPTION,
+                 long_description_content_type="text/x-rst",
                  license="GPL-3.0-or-later",
                  author=TVB_TEAM,
                  author_email='tvb.admin@thevirtualbrain.org',
                  url='https://www.thevirtualbrain.org',
                  download_url='https://github.com/the-virtual-brain/tvb-root',
                  keywords='tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay')
```

### Comparing `tvb-rest-client-2.8.1/tvb/__init__.py` & `tvb-rest-client-2.9/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_adapters.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/bct_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_centrality_adapters.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/bct_centrality_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_clustering_adapters.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/bct_clustering_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_degree_adapters.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/bct_degree_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/cross_correlation_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/cross_correlation_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fcd_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/fcd_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fmri_balloon_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/fmri_balloon_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fourier_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/fourier_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/ica_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/ica_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/metrics_group_timeseries.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/metrics_group_timeseries.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_coherence_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/node_coherence_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_complex_coherence_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/node_complex_coherence_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_covariance_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/node_covariance_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/pca_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/pca_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/analyzers/wavelet_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/analyzers/wavelet_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/allen_creator.py` & `tvb-rest-client-2.9/tvb/adapters/creators/allen_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/connectivity_creator.py` & `tvb-rest-client-2.9/tvb/adapters/creators/connectivity_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/local_connectivity_creator.py` & `tvb-rest-client-2.9/tvb/adapters/creators/local_connectivity_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_base.py` & `tvb-rest-client-2.9/tvb/adapters/creators/siibra_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,32 +34,39 @@
 from enum import Enum
 from tvb.basic.logger.builder import get_logger
 from tvb.datatypes import connectivity
 from tvb.datatypes.graph import ConnectivityMeasure
 
 LOGGER = get_logger(__name__)
 
-DEFAULT_ATLAS = 'Multilevel Human Atlas'
-DEFAULT_PARCELLATION = 'Julich-Brain Cytoarchitectonic Maps 2.9'
-DEFAULT_COHORT = 'HCP'
+# Concepts names
+# atlases
+HUMAN_ATLAS = 'Multilevel Human Atlas'  # DEFAULT, only this atlas has Struct. Conn.
+
+# parcellations
+JULICH_3_0 = 'Julich-Brain Cytoarchitectonic Atlas (v3.0.3)'  # DEFAULT
+JULICH_2_9 = 'Julich-Brain Cytoarchitectonic Atlas (v2.9)'
+parcellations = [JULICH_3_0, JULICH_2_9]
+
+# cohorts
+HCP_COHORT = 'HCP'  # DEFAULT
 THOUSAND_BRAINS_COHORT = '1000BRAINS'
 
 
 class Component2Modality(Enum):
     WEIGHTS = siibra.features.connectivity.StreamlineCounts
     TRACTS = siibra.features.connectivity.StreamlineLengths
     FUNCTIONAL_CONNECTIVITY = siibra.features.connectivity.FunctionalConnectivity
 
 
 # ########################################## SIIBRA CREATOR INITIALIZATION #############################################
 def get_cohorts_for_sc(parcellation_name):
     """
     Given a parcellation name, return the name of all the cohorts related to it and containing data about
-    Structural Connectivities. We chose to return the options for Struct. Conn., as, for the moment, the same values
-    are returned for Functional Conn.
+    Structural Connectivities.
     """
     parcellation = siibra.parcellations[parcellation_name]
     features = siibra.features.get(parcellation, siibra.features.connectivity.StreamlineCounts)
     return [f.cohort.upper() for f in features]
 
 
 # ######################################## SIIBRA PARAMETERS CONFIGURATION #############################################
@@ -72,57 +79,51 @@
     """ Given a parcelation, return all the atlases that contain it """
     atlases = siibra.atlases
     atlases = [a for a in atlases if parcelation in list(a.parcellations)]
     return atlases
 
 
 def get_parcellations_for_atlas(atlas):
-    """ Given the name of an atlas, return all the parcellations inside it """
-    return list(atlas.parcellations)
+    """ Given an atlas, return a list of all the parcellations inside it, which contain Structural conns. """
+    parcellations_available = [p for p in list(atlas.parcellations) if p.name in parcellations]
+    return parcellations_available
 
 
 def parse_subject_ids(subject_ids, cohort):
     """
     Given a string representing subject ids or a range of subject ids; return the list containing all the included ids
     """
     parsed_ids_as_str = []
     individual_splits = subject_ids.split(';')
+    zfill_value = 3 if cohort == HCP_COHORT else 4  # used in case of ranges
 
-    if cohort == THOUSAND_BRAINS_COHORT:
-        for s in individual_splits:
+    for s in individual_splits:
+        # if a range was specified
+        if '-' in s:
+            start, end = s.split('-')
+            start_int = int(start)
+            end_int = int(end) + 1  # so that the last element in range is also included
+            ids_list_from_range = list(range(start_int, end_int))
+            parsed_ids_as_str.extend([str(id).zfill(zfill_value) for id in ids_list_from_range])
+        else:
             parsed_ids_as_str.append(s)
-    elif cohort == DEFAULT_COHORT:
-        parsed_ids = []
-        for s in individual_splits:
-            # if a range was written
-            if '-' in s:
-                start, end = s.split('-')
-                start_int = int(start)
-                end_int = int(end) + 1  # so that the last element in range is also included
-                ids_list_from_range = list(range(start_int, end_int))
-                parsed_ids.extend(ids_list_from_range)
-            else:
-                s_int = int(s)
-                parsed_ids.append(s_int)
-
-        # convert the subject ids list back to strings into the required format
-        parsed_ids_as_str = [str(id).zfill(3) for id in parsed_ids]
 
+    parsed_ids_as_str = sorted(set(parsed_ids_as_str))
     return parsed_ids_as_str
 
 
 def init_siibra_params(atlas_name, parcellation_name, cohort_name, subject_ids):
     """
     Initialize siibra parameters (if some were not given) and check the compatibility of the provided parameters.
     :param: atlas_name - name of atlas as str
     :param: parcellation_name - name of parcellation as str
     :param: cohort_name - name of cohort as str
     :param: subject_ids - list of unparsed subject ids given as str
     :return: (atlas, parcellation, cohort_name, subject_ids) - tuple containing a siibra atlas object,
-    a siibra parcellation object and a cohort name all compatible with each other and a list of parsed ids
+    a siibra parcellation object and a cohort name, all compatible with each other, and a list of parsed ids
     """
     # check that the atlas and the parcellation exist within siibra
     atlas = siibra.atlases[atlas_name] if atlas_name else None
     parcellation = siibra.parcellations[parcellation_name] if parcellation_name else None
 
     # check compatibility of atlas and parcellation
     if atlas and parcellation:
@@ -133,50 +134,52 @@
 
     if atlas and not parcellation:
         LOGGER.warning(f'No parcellation was provided, so a default one will be selected.')
         parcellations = get_parcellations_for_atlas(atlas)
         no_parcellations = len(parcellations)
         if no_parcellations < 1:
             raise AttributeError(f'No default parcellation was found for atlas {atlas.name}!')
-        if no_parcellations > 1:
+        elif no_parcellations > 1:
             LOGGER.info(
                 f'Multiple parcellations were found for atlas {atlas.name}. An arbitrary one will be selected.')
-        parcellation = parcellations[0]
+        # select the newest parcellation version
+        parcellation = [p for p in parcellations if p.is_newest_version][0]
 
     if not atlas and parcellation:
         LOGGER.warning('A parcellation was provided without an atlas, so a default atlas will be selected.')
         atlases = get_atlases_for_parcellation(parcellation)
         no_atlases = len(atlases)
         if no_atlases < 1:
             raise AttributeError(f'No default atlas containing parcellation {parcellation.name} was found!')
-        if no_atlases > 1:
+        elif no_atlases > 1:
             LOGGER.info(
                 f'Multiple atlases containing parcellation {parcellation_name} were found. '
                 f'An arbitrary one will be selected')
         atlas = atlases[0]
 
     if not atlas and not parcellation:
         LOGGER.warning(f'No atlas and no parcellation were provided, so default ones will be selected.')
-        atlas = siibra.atlases[DEFAULT_ATLAS]
-        parcellation = siibra.parcellations[DEFAULT_PARCELLATION]
+        atlas = siibra.atlases[HUMAN_ATLAS]
+        parcellation = siibra.parcellations[JULICH_3_0]
 
     LOGGER.info(f'Using atlas {atlas.name} and parcellation {parcellation.name}')
 
-    # check the compatibility of cohort and parcellation
-    cohort_options = get_cohorts_for_sc(parcellation.name)
-    if cohort_name is None:
-        cohort_name = DEFAULT_COHORT
-    elif cohort_name not in cohort_options:
-        raise ValueError(f'The cohort \"{cohort_name}\" is not available for parcellation \"{parcellation.name}\"!')
+    if cohort_name:
+        # check the compatibility of cohort and parcellation
+        cohort_options = get_cohorts_for_sc(parcellation.name)
+        if cohort_name not in cohort_options:
+            raise ValueError(f'The cohort \"{cohort_name}\" is not available for parcellation \"{parcellation.name}\"! '
+                             f'Please choose one of the following cohorts: {cohort_options} or change '
+                             f'the parcellation.')
+    else:
+        cohort_name = HCP_COHORT  # compatible with all parcellations
 
     # check subject ids
     if not subject_ids:
-        LOGGER.info(
-            f'The mean across all connectivities from cohort {cohort_name} will be computed.')
-        subject_ids = [None]
+        raise ValueError(f'Please provide at least one subject ID!')
     else:
         subject_ids = parse_subject_ids(subject_ids, cohort_name)
 
     return atlas, parcellation, cohort_name, subject_ids
 
 
 # ############################################# CONNECTIVITY METHODS ###################################################
@@ -188,35 +191,34 @@
     :return: hemi - list of ints indicating the hemisphere for each region in `region_names`
     """
     LOGGER.info(f'Computing hemispheres for regions')
     hemi = []
     for name in region_names:
         if 'right' in name:
             hemi.append(1)
-        # TODO: regions referring to both hemispheres are put in the left hemisphere; change this?
         else:
             hemi.append(0)
 
     return hemi
 
 
 def get_regions_positions(regions):
     """
     Given a list of siibra regions, compute the positions of their centroids.
-    :param: regions - list of siibra region objects
-    :return: positions - list of tuples; each tuple represents the position of a region in `regions` and contains
+    :param: regions - list of siibra Regions
+    :return: positions - list of tuples; each tuple represents the position of a region and contains
     3 floating point coordinates
     """
     LOGGER.info(f'Computing positions for regions')
     positions = []
-    space = siibra.spaces.MNI_152_ICBM_2009C_NONLINEAR_ASYMMETRIC  # commonly used space in the documentation
 
     for r in regions:
-        centroid = r.spatial_props(space)['components'][0]['centroid'].coordinate
-        positions.append(centroid)
+        space = r.supported_spaces[0]  # choose first space that is available for that region
+        centroid = r.spatial_props(space=space).components[0].centroid
+        positions.append(centroid.coordinate)
 
     return positions
 
 
 # ###################################### STRUCTURAL CONNECTIVITY METHODS ###############################################
 def get_connectivity_matrix(parcellation, cohort, subjects, component):
     # type: (siibra.core.parcellation.Parcellation, str, list, Component2Modality) -> {}
@@ -224,39 +226,38 @@
     Retrieve the structural connectivity components (weights/tracts) for all the subjects provided, for the specified
     parcellation and cohort. The matrices are returned inside a dictionary, where the keys are the subject ids and the
     values represent the connectivity matrix.
     :param: parcellation - siibra Parcellation object for which we compute the connectivity matrices
     :param: cohort - name of cohort for which we compute the connectivity matrices
     :param: subjects - list containing the subject ids as strings
     :param: component - enum value specifying the connectivity component we want, weights or tracts
-    return: conn_matrices - dict containing the conn. matrices (values) for the specified subject ids (keys)
+    return: conn_matrices - dict where key is the subject id and value is the conn. matrix
     """
     modality = component.value
     features = siibra.features.get(parcellation, modality)
     conn_for_cohort = None  # conn. obj. (StreamlineCounts/StreamlineLengths) for specified cohort
     conn_matrices = {}  # dict containing connectivity matrices for the specified users
     # select the connectivities for the specific cohort
     for f in features:
         if f.cohort == cohort:
             conn_for_cohort = f
             break
 
     if conn_for_cohort is None:
-        LOGGER.info("NO conn_for_cohort was found")
-        return conn_matrices
+        raise AttributeError(f"NO {modality} was found for cohort {cohort}")
 
     # for 1000BRAINS cohort, if the user did not specify a suffix (_1, _2), get all the possible ids for that subject
     if cohort == THOUSAND_BRAINS_COHORT and subjects is not None:
-        subjects = [s for s in sorted(conn_for_cohort.subjects) if any(x in s for x in subjects)]
+        all_subjects = sorted([conn.subject for conn in conn_for_cohort.elements])
+        subjects = [s for s in all_subjects if any(x in s for x in subjects)]
 
     # get the conn. matrices for each specified subject
     for s in subjects:
-        if s is None:
-            s = 'mean'
-        matrix = conn_for_cohort.get_matrix(s)
+        conn = [c for c in conn_for_cohort if c.subject == s][0]
+        matrix = conn.data
         conn_matrices[s] = matrix
         LOGGER.info(f'{component.name} for subject {s} retrieved successfully.')
 
     return conn_matrices
 
 
 def create_tvb_structural_connectivity(weights_matrix, tracts_matrix, region_names, hemispheres, positions):
@@ -284,148 +285,130 @@
 def get_structural_connectivities_from_kg(atlas=None, parcellation=None, cohort=None, subject_ids=None):
     """
     Return a dictionary of TVB Structural Connectivities using data from siibra and the KG, based on the specified
     atlas, parcelation and cohort, and for the specified subjects
     :param: atlas - str specifying the atlas name
     :param: parcellation - str specifying the parcellation name
     :param: cohort - str specifying the cohort name
-    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be retrived
     :return: connectivities - dict containing tvb structural Connectivities as values and the subject ids as keys
     """
     atlas, parcellation, cohort, subject_ids = init_siibra_params(atlas, parcellation, cohort, subject_ids)
     connectivities = {}
     weights = get_connectivity_matrix(parcellation, cohort, subject_ids, Component2Modality.WEIGHTS)
     tracts = get_connectivity_matrix(parcellation, cohort, subject_ids, Component2Modality.TRACTS)
 
     # regions are the same for all weights and tract lengths matrices, so they can be computed only once
     regions = list(weights.values())[0].index.values
-    # because siibra sometimes returns tuples instead of actual regions, change list to contain only regions
-    regions = [r[1] if type(r) == tuple else r for r in regions]
     region_names = [r.name for r in regions]
     hemi = get_hemispheres_for_regions(region_names)
     positions = get_regions_positions(regions)
 
     LOGGER.info(f'Computing TVB Connectivities')
     for subject, matrix in weights.items():
         weights_matrix = matrix
         tracts_matrix = tracts[subject]
         tvb_conn = create_tvb_structural_connectivity(weights_matrix, tracts_matrix, region_names, hemi, positions)
 
-        # structural connectivities stored as dict, to link a functional connectivity with the correct
-        # structural connectivity when creating connectivity measures
+        # structural connectivities stored as dict, where key is subject id, as we need it when computing connectivity
+        # measures
         connectivities[subject] = tvb_conn
 
     return connectivities
 
 
 # #################################### FUNCTIONAL CONNECTIVITY METHODS #################################################
 def get_functional_connectivity_matrix(parcellation, cohort, subject):
     """
     Get all the functional connectivities for the specified parcellation, cohort and just ONE specific subject;
-    In v0.4a35 of siibra, functional connectivities belonging to the same cohort can be split into multiple (5)
-    siibra FunctionalConnectivity objects
+    In v1.0a5 of siibra, for HCP cohort there are 5 groups of functional connectivities; each group contains
+    1 Functional connectivity for each subject addressed in the research
     :param: parcellation - siibra Parcellation object
     :param: cohort - str specifying the cohort name
     :param: subject - str specifying exactly one subject id
     :return: (fcs_list, fcs_names_list) - tuple containing 2 lists; `fcs_list` contains pandas.Dataframe matrices and
     `fcs_names_list` contains the name for each matrix from the previous list, obtained from the file they are stored
-    in in the KG
+    in the KG
     """
     modality = Component2Modality.FUNCTIONAL_CONNECTIVITY.value
     features = siibra.features.get(parcellation, modality)
     fcs_list = []  # the FC matrices
     fcs_names_list = []  # the name of the files containing the FC matrices in fcs_list
 
     for f in features:
         if f.cohort == cohort:
-            fc_matrix = f.get_matrix(subject)
-            fcs_names_list.append(f._files[subject])
+            f_conn = [c for c in f.elements if c.subject == subject][0]
+            fc_matrix = f_conn.data
+            fcs_names_list.append(f_conn.name)
             fcs_list.append(fc_matrix)
 
     return fcs_list, fcs_names_list
 
 
-def get_fc_name_from_file_path(path_to_file):
-    """
-    Given the entire path to a file containing a siibra FunctionalConnectivity, return just the filename
-    Note: highly dependent on KG/siibra storage conventions
-    :param: path_to_file - str representing the path to a Functional Connectivity from the KG
-    :return: filename - just the filename (without the extension)
-    """
-    file_with_extension = path_to_file.rsplit('/', 1)[1]
-    filename = file_with_extension.rsplit('.', 1)[0]
-
-    return filename
-
-
-def create_tvb_connectivity_measure(siibra_fc, structural_connectivity, siibra_fc_filename):
+def create_tvb_connectivity_measure(siibra_fc, structural_connectivity, siibra_fc_name):
     """
     Given a FunctionalConnectivity from siibra TVB Structural Connectivity (both for the same subject),
     return a TVB ConnectivityMeasure containing those 2 connectivities
     :param: siibra_fc - pandas.Dataframe matrix from siibra containing a functional connectivity
     :param: structural_connectivity - a TVB structural connectivity
-    :param: siibra_fc_filename - the name of the file containing the functional connectivity from siibra
+    :param: siibra_fc_name - the name of the siibra functional connectivity object
     :return: conn_measure - tvb.datatypes.graph.ConnectivityMeasure representing a functional connectivity
     """
     fc_matrix = siibra_fc.to_numpy()
     conn_measure = ConnectivityMeasure(array_data=fc_matrix, connectivity=structural_connectivity)
-    conn_measure.title = get_fc_name_from_file_path(siibra_fc_filename)
-
+    conn_measure.title = siibra_fc_name
     return conn_measure
 
 
 def get_connectivity_measures_from_kg(atlas=None, parcellation=None, cohort=None, subject_ids=None,
                                       structural_connectivities=None):
     """
     Return a dictionary of TVB Connectivity Measures using data from siibra and the KG, based on the specified
     atlas, parcelation and cohort, and for the specified subjects
     :param: atlas - str specifying the atlas name
     :param: parcellation - str specifying the parcellation name
     :param: cohort - str specifying the cohort name
-    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be retrieved
     :param: structural_connectivities - dict of TVB Structural Connectivities computed for the subjects from
     `subject_ids`, where subject ids are keys and the structural connectivities are values
     :return: conn_measures - dict containing TVB Connectivity Measures as values and the subject ids as keys
     """
     atlas, parcellation, cohort, subject_ids = init_siibra_params(atlas, parcellation, cohort, subject_ids)
     conn_measures = {}
 
     # for 1000BRAINS cohort, if the user did not specify a suffix (_1, _2), get all the possible ids for that subject
     if cohort == THOUSAND_BRAINS_COHORT and any('_' not in s for s in subject_ids):
         f = [f for f in siibra.features.get(parcellation, siibra.features.connectivity.FunctionalConnectivity)
-             if f.cohort == THOUSAND_BRAINS_COHORT]
-        f = f[0]  # get the first feature from the feature list, we just want to know the subject names
-        subjects_for_cohort = f.subjects
+             if f.cohort == THOUSAND_BRAINS_COHORT][0]  # there is only one FC group for this 1000BRAINS
+        subjects_for_cohort = [f_conn.subject for f_conn in f]
         subject_ids = [s for s in sorted(subjects_for_cohort) if any(x in s for x in subject_ids)]
 
     for s in subject_ids:
-        if s is None:
-            s = 'mean'
         conn_measures[s] = []
         sc = structural_connectivities[s]
 
         fcs, fcs_names = get_functional_connectivity_matrix(parcellation, cohort, s)
 
         # create a tvb conn measure from a siibra fc and append it in the final dict for the specified subject
         for i in range(len(fcs)):
             conn_measure = create_tvb_connectivity_measure(fcs[i], sc, fcs_names[i])
             conn_measures[s].append(conn_measure)
 
     return conn_measures
 
 
 # ################################################# FINAL API ##########################################################
-def get_connectivities_from_kg(atlas=None, parcellation=None, cohort=DEFAULT_COHORT,
+def get_connectivities_from_kg(atlas=None, parcellation=None, cohort=HCP_COHORT,
                                subject_ids=None, compute_fc=False):
     """
     Compute the TVB Structural Connectivities and optionally Functional Connectivities for the selected subjects
     :param: atlas - str specifying the atlas name
     :param: parcellation - str specifying the parcellation name
     :param: cohort - str specifying the cohort name
-    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be retrieved
     :param: compute_fc - boolean value indicating if for the specified subjects the functional connectivities should
     also be retrieved
     :return: (sc_dict, conn_measures_dict) - tuple containing 2 dictionaries: one with structural connectivities and
     one for functional connectivities; for each dictionary, the keys are the subject ids and the values are the
     connectivities
     """
     conn_measures_dict = {}
```

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_creator.py` & `tvb-rest-client-2.9/tvb/adapters/creators/siibra_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,33 +37,28 @@
 from tvb.adapters.datatypes.db.connectivity import ConnectivityIndex
 from tvb.adapters.datatypes.db.graph import ConnectivityMeasureIndex
 from tvb.basic.neotraits._attr import Attr, EnumAttr
 from tvb.basic.neotraits._core import TVBEnum
 from tvb.core.adapters.abcadapter import ABCAdapterForm, ABCAdapter
 from tvb.core.neotraits.forms import StrField, SelectField, BoolField, UserSessionStrField
 from tvb.core.neotraits.view_model import ViewModel, Str
-from tvb.core.services.user_service import KEY_AUTH_TOKEN
-
-CLB_AUTH_TOKEN_KEY = 'HBP_AUTH_TOKEN'
 
 
 # Following code is executed only once, when the application starts running
 def init_siibra_options():
     """"
-    Initialize siibra options for atlas and parcellations
+    Initialize siibra options for atlas, parcellations and cohorts.
+    These options were manually selected and are the only ones having struct. conn. right now. This may change in the
+    future.
     """
-    # should use `atlases = [a.name for a in list(siibra.atlases)]`, but only the default one has data
-    atlases = [siibra_base.DEFAULT_ATLAS]  # list with atlases names
-    # should get only valid parcellations for default atlas, but only newest version of Julich parcellation
-    # has data and corresponds with the current API of siibra
-    parcellations = [siibra_base.DEFAULT_PARCELLATION]
-
-    # get available cohorts
-    cohorts = siibra_base.get_cohorts_for_sc(parcellations[0])
+    atlases = [siibra_base.HUMAN_ATLAS]
+    parcellations = [siibra_base.JULICH_3_0, siibra_base.JULICH_2_9]
+    cohorts = [siibra_base.HCP_COHORT, siibra_base.THOUSAND_BRAINS_COHORT]
 
+    # create dicts needed for TVB Enums
     atlas_dict = {a_name: a_name for a_name in atlases}
     parcellation_dict = {p_name: p_name for p_name in parcellations}
     cohort_dict = {(y := c_name.upper()): y for c_name in cohorts}
 
     atlas_options = TVBEnum('AtlasOptions', atlas_dict)
     parcellation_options = TVBEnum('ParcellationOptions', parcellation_dict)
     cohort_options = TVBEnum('CohortOptions', cohort_dict)
@@ -73,39 +68,33 @@
 
 if 'SIIBRA_INIT_DONE' not in globals():
     ATLAS_OPTS, PARCELLATION_OPTS, COHORT_OPTS = init_siibra_options()
     SIIBRA_INIT_DONE = True
 
 
 class SiibraModel(ViewModel):
-    ebrains_token = Str(
-        label='EBRAINS token',
-        required=True,
-        doc='Auth Token provided by EBRAINS lab `clb_oauth.get_token()` for accessing the Knowledge Graph'
-    )
-
     atlas = EnumAttr(
         field_type=ATLAS_OPTS,
-        default=ATLAS_OPTS[siibra_base.DEFAULT_ATLAS],
+        default=ATLAS_OPTS[siibra_base.HUMAN_ATLAS],
         label='Atlas',
         required=True,
-        doc='Atlas to be used (only the compatible ones listed)'
+        doc='Atlas to be used'
     )
 
     parcellation = EnumAttr(
         field_type=PARCELLATION_OPTS,
-        default=PARCELLATION_OPTS[siibra_base.DEFAULT_PARCELLATION],
+        default=PARCELLATION_OPTS[siibra_base.JULICH_3_0],
         label='Parcellation',
         required=True,
-        doc='Parcellation to be used (only TVB compatible ones listed here)'
+        doc='Parcellation to be used'
     )
 
     cohort = EnumAttr(
         field_type=COHORT_OPTS,
-        default=COHORT_OPTS[siibra_base.DEFAULT_COHORT],
+        default=COHORT_OPTS[siibra_base.HCP_COHORT],
         label='Cohort',
         required=True,
         doc='Cohort to be used'
     )
 
     subject_ids = Str(
         label='Subjects',
@@ -116,36 +105,41 @@
         a) For the "HCP" cohort, the subject IDs are: 000,001,002, etc. Each subject has exactly one 
         subject ID associated to them. Thus, there are 3 ways to specify the IDs:<br/>
         1. individually, delimited by a semicolon symbol: 000;001;002. <br/>
         2. As a range, specifying the first and last IDs: 000-050 will retrieve all the subjects starting with 
         subject 000 until subject 050 (51 subjects). <br/>
         A combination of the 2 methods is also supported: 000-005;010 will retrieve all the subjects starting with 
         subject 000 until subject 005 (6 subjects) AND subject 010 (so 7 subjects in total)<br/> <br/>
-        b) For "1000BRAINS" cohort, the subject IDs are: 0001_1, 0001_2, 0002_1, 0002_2, etc. Each subject can have 
-        multiple subjects IDs associated to them, indicated by the "_1", "_2" suffix, but most of subjects have 
-        just one ID, ending in "_1". Thus, there are 2 ways to specify the IDs: <br/>
-        1. individually and specifying the exact ID, so including "_1" or "_2". Multiple IDs can be mentioned 
-        by using a semicolon symbol to delimitate them: 0001_1;0017_1;0017_2. <br/>
-        2. individually, and specifying just the prefix for a subject. Multiple IDs can be mentioned by using a 
-        semicolon symbol to delimitate them: 0001;0017 will be converted to 4 IDs: 0001_1, 0001_2, 0017_1, 0017_2.
+        b) For "1000BRAINS" cohort, the subject IDs have to parts: first part is the subject ID, which has the form:
+         0001, 0002, etc., and the second part is the scanning session index, which has the form _1, _2. All subjects 
+         had between 1 and 2 scanning sessions. Thus, the final IDs will look like: 0001_1, 0001_2, 0002_1, etc. and 
+         there are 3 ways to specify the IDs: <br/>
+        1. individually and specifying the exact ID, including the session index "_1" or "_2". Multiple IDs can be 
+        mentioned by using a semicolon symbol to delimit them: 0001_1;0017_1;0017_2. <br/>
+        2. individually, and without specifying the session index. In this case, all available sessions for that subject 
+        will be retrieved. Multiple IDs can be mentioned by using a semicolon symbol to delimit them: 0001;0017 will be 
+        converted to 4 IDs: 0001_1, 0001_2, 0017_1, 0017_2. <br/>
+        3. As a range, specifying only the subject ids and not the session ids: 0001-0003 will retrieve all the 
+        available sessions for subjects 1, 2, 3, i.e.: 0001_1, 0001_2, 0002_1, 0002_2, 0003_1 and 0003_2. <br/>
+        A combination of the 3 methods is also supported: 0001-0003;0005_1;0009 will retrieve connectivities for the 
+        following IDs: 0001_1, 0001_2, 0002_1, 0002_2, 0003_1, 0003_2, 0005_1, 0009_1, 0009_2.
         """)
 
     fc = Attr(
         field_type=bool,
         label="Compute Functional Connectivities",
         default=True,
         required=True,
-        doc="Set if the functional connectivities for the specified subjects should also be computed"
+        doc="Flag to specify if the functional connectivities for the selected subjects should also be computed"
     )
 
 
 class SiibraCreatorForm(ABCAdapterForm):
     def __init__(self):
         super(SiibraCreatorForm, self).__init__()
-        self.ebrains_token = UserSessionStrField(SiibraModel.ebrains_token, name="ebrains_token", key=KEY_AUTH_TOKEN)
         self.atlas = SelectField(SiibraModel.atlas, name='atlas')
         self.parcellation = SelectField(SiibraModel.parcellation, name='parcellation')
         self.cohort = SelectField(SiibraModel.cohort, name='cohort')
         self.subject_ids = StrField(SiibraModel.subject_ids, name='subject_ids')
         self.fc = BoolField(SiibraModel.fc, name='fc')
 
     @staticmethod
@@ -165,46 +159,41 @@
         return None
 
 
 class SiibraCreator(ABCAdapter):
     """ The purpose of this creator is to use siibra in order to create Structural and Functional Connectivities """
 
     _ui_name = "Siibra Connectivity Creator"
-    _ui_description = "Create Structural and Functional Connectivities from the EBRAINS KG using siibra"
+    _ui_description = "Create Structural and Functional Connectivities with data from the EBRAINS KG using siibra"
 
     def get_form_class(self):
         return SiibraCreatorForm
 
     def get_output(self):
         return [ConnectivityIndex, ConnectivityMeasureIndex]
 
     def launch(self, view_model):
-        ebrains_token = view_model.ebrains_token
         atlas = view_model.atlas.value
         parcellation = view_model.parcellation.value
         cohort = view_model.cohort.value
         subject_ids = view_model.subject_ids
         compute_fc = view_model.fc
 
-        os.environ[CLB_AUTH_TOKEN_KEY] = ebrains_token
-
         # list of all resulting indices for connectivities and possibly connectivity measures
         results = []
 
         try:
             conn_dict, conn_measures_dict = siibra_base.get_connectivities_from_kg(atlas, parcellation, cohort,
                                                                                    subject_ids, compute_fc)
-        except SiibraHttpRequestError as e:
-            if e.response.status_code in [401, 403]:
-                raise ConnectionError('Invalid EBRAINS authentication token. Please provide a new one.')
-            else:
-                raise ConnectionError('We could not complete the operation. '
-                                      'Please check the logs and contact the development team from TVB, siibra or EBRAINS KG.')
+        except SiibraHttpRequestError:
+            raise ConnectionError('We could not complete the operation. '
+                                  'Please check the logs and contact the development team from TVB, siibra or '
+                                  'EBRAINS KG.')
 
-        # list of indexes for stored the Struct. Conn. and Conn. Measures
+        # list of indexes of stored Struct. Conn. and Conn. Measures
         conn_indices = []
         conn_measures_indices = []
 
         for subject_id, conn in conn_dict.items():
             generic_attrs = view_model.generic_attributes
             generic_attrs.subject = subject_id
```

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/creators/stimulus_creator.py` & `tvb-rest-client-2.9/tvb/adapters/creators/stimulus_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/annotation.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/annotation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/connectivity.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/fcd.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/fcd.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/graph.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/local_connectivity.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/local_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,11 @@
     matrix_non_zero_min = Column(Float)
     matrix_non_zero_max = Column(Float)
     matrix_non_zero_mean = Column(Float)
 
     def fill_from_has_traits(self, datatype):
         # type: (LocalConnectivity)  -> None
         super(LocalConnectivityIndex, self).fill_from_has_traits(datatype)
-        I, J, V = scipy.sparse.find(datatype.matrix)
-        self.matrix_non_zero_min, self.matrix_non_zero_max, self.matrix_non_zero_mean = from_ndarray(V)
+        if datatype.matrix is not None:
+            I, J, V = scipy.sparse.find(datatype.matrix)
+            self.matrix_non_zero_min, self.matrix_non_zero_max, self.matrix_non_zero_mean = from_ndarray(V)
         self.fk_surface_gid = datatype.surface.gid.hex
```

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mapped_value.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/mapped_value.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mode_decompositions.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/mode_decompositions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/patterns.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/patterns.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/projections.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/region_mapping.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_connectivity.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_region_mapping.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_sensor.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_sensor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_surface.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_timeseries.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_timeseries.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_volume.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/removers/remover_volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/sensors.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/simulation_history.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/simulation_history.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/spectral.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/spectral.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/structural.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/surface.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/temporal_correlations.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/temporal_correlations.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/time_series.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/tracts.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/tracts.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/volume.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/db/volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/annotation_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/annotation_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/connectivity_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/connectivity_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/fcd_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/fcd_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/graph_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/graph_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/local_connectivity_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/local_connectivity_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mapped_value_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/mapped_value_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mode_decompositions_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/mode_decompositions_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/patterns_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/patterns_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/projections_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/projections_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/region_mapping_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/region_mapping_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/sensors_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/sensors_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/spectral_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/spectral_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/structural_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/structural_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/surface_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/surface_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/temporal_correlations_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/temporal_correlations_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/time_series_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/time_series_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/tracts_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/tracts_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/volumes_h5.py` & `tvb-rest-client-2.9/tvb/adapters/datatypes/h5/volumes_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/abcexporter.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/abcexporter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/exceptions.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/export_manager.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/export_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_export.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/tvb_export.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_linked_export.py` & `tvb-rest-client-2.9/tvb/adapters/exporters/tvb_linked_export.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/coupling_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/coupling_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/equation_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/equation_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/equation_plot_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/equation_plot_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/form_with_ranges.py` & `tvb-rest-client-2.9/tvb/adapters/forms/form_with_ranges.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/integrator_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/integrator_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/model_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/monitor_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/monitor_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/noise_forms.py` & `tvb-rest-client-2.9/tvb/adapters/forms/noise_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/simulator_fragments.py` & `tvb-rest-client-2.9/tvb/adapters/forms/simulator_fragments.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/surface_model_parameters_form.py` & `tvb-rest-client-2.9/tvb/adapters/forms/surface_model_parameters_form.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/forms/transfer_vector_form.py` & `tvb-rest-client-2.9/tvb/adapters/forms/transfer_vector_form.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/simulator/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/simulator/hpc_simulator_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/simulator/hpc_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/simulator/range_parameters.py` & `tvb-rest-client-2.9/tvb/adapters/simulator/range_parameters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/simulator/simulator_adapter.py` & `tvb-rest-client-2.9/tvb/adapters/simulator/simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/bids_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/bids_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/brco/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/brco_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/connectivity_measure_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/connectivity_measure_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/csv_connectivity_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/csv_connectivity_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         return [ConnectivityIndex]
 
     def _read_csv_file(self, csv_file, delimiter):
         """
         Read a CSV file, arrange rows/columns in the correct order,
         to obtain Weight/Tract data in TVB compatible format.
         """
-        with open(csv_file, 'rU') as f:
+        with open(csv_file, 'r') as f:
             result_conn = CSVConnectivityParser(f, delimiter).result_conn
             self.logger.debug("Read Connectivity file of size %d" % len(result_conn))
             return numpy.array(result_conn)
 
     def launch(self, view_model):
         # type: (CSVConnectivityImporterModel) -> ConnectivityIndex
         """
```

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/gifti/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_surface_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/gifti_surface_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_timeseries_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/gifti_timeseries_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/mat/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/mat_timeseries_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_connectivity/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/networkx_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/nifti/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/nifti_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/obj/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/surface.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/obj/surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/obj_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/projection_matrix_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/projection_matrix_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/region_mapping_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/region_mapping_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/sensors_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/sensors_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tract_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/tract_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tumor_dataset_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/tumor_dataset_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tvb_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/tvb_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_connectivity_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/zip_connectivity_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/parser.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface_importer.py` & `tvb-rest-client-2.9/tvb/adapters/uploaders/zip_surface_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/__init__.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/annotations_viewer.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/annotations_viewer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/brain.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/brain.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/complex_imaginary_coherence.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/complex_imaginary_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity_edge_bundle.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/connectivity_edge_bundle.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_coherence.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/cross_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_correlation.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/eeg_monitor.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/eeg_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/fourier_spectrum.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/fourier_spectrum.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/histogram.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/histogram.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/ica.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/ica.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/local_connectivity_view.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/local_connectivity_view.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/matrix_viewer.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/matrix_viewer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pca.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pca.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_cross_correlation.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pearson_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_edge_bundle.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pearson_edge_bundle.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/phase_plane_interactive.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/phase_plane_interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,38 +33,32 @@
 
 # To plot nullclines we need a function that computes contours of a scalar field.
 # We use the internal matplotlib one.
 # Now that newer matplotlib versions have changed this internal API it would be a
 # good idea to use a proper library for this.
 
 try:
-    from matplotlib import _cntr
-    # older matplotlib
-
-    def nullcline(x, y, z):
-        c = _cntr.Cntr(x, y, z)
-        # trace a contour
-        res = c.trace(0.0)
-        if not res:
-            return numpy.array([])
-        # result is a list of arrays of vertices and path codes
-        # (see docs for matplotlib.path.Path)
-        nseg = len(res) // 2
-        segments, codes = res[:nseg], res[nseg:]
-        return segments
-
-except ImportError:
     from matplotlib import _contour
-    # newer matplotlib >= 2.2
+    # old matplotlib
 
     def nullcline(x, y, z):
         c = _contour.QuadContourGenerator(x, y, z, None, True, 0)
         segments = c.create_contour(0.0)
         return segments[0]
 
+
+except ImportError:
+    import matplotlib.pyplot as plt
+    # new matplotlib, version 3.8.3
+
+    def nullcline(x, y, z):
+        c = plt.contour(x, y, z, levels=[0.0])
+        segments = c.collections[0].get_paths()
+        return segments
+
 # how much courser is the grid used to show the vectors
 GRID_SUBSAMPLE = 2
 # Set the resolution of the phase-plane and sample trajectories.
 NUMBEROFGRIDPOINTS = GRID_SUBSAMPLE * 42
 
 
 class _PhaseSpace(object):
@@ -208,16 +202,16 @@
         :return: A json representation of the phase plane.
         """
         x, y = self._get_mesh_grid(self.x_range, self.y_range, noise=self._jitter)
 
         u, v = self._calc_phase_plane(self.default_sv, self.svx_ind, self.svy_ind, x, y)
         u = u[..., self.mode]  # project on active mode
         v = v[..., self.mode]
-        xnull = [{'path': segment.tolist(), 'nullcline_index': 0} for segment in nullcline(x, y, u)]
-        ynull = [{'path': segment.tolist(), 'nullcline_index': 1} for segment in nullcline(x, y, v)]
+        xnull = [{'path': segment.vertices.tolist(), 'nullcline_index': 0} for segment in nullcline(x, y, u)]
+        ynull = [{'path': segment.vertices.tolist(), 'nullcline_index': 1} for segment in nullcline(x, y, v)]
 
         # a courser mesh for the arrows
         xsmall = x[::GRID_SUBSAMPLE, ::GRID_SUBSAMPLE]
         ysmall = y[::GRID_SUBSAMPLE, ::GRID_SUBSAMPLE]
         usmall = u[::GRID_SUBSAMPLE, ::GRID_SUBSAMPLE]
         vsmall = v[::GRID_SUBSAMPLE, ::GRID_SUBSAMPLE]
```

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pse.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_discrete.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pse_discrete.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_isocline.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/pse_isocline.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/region_volume_mapping.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/region_volume_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/sensors.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/surface_view.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/surface_view.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series_volume.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/time_series_volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/topographic.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/topographic.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/tract.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/tract.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/adapters/visualizers/wavelet_spectrogram.py` & `tvb-rest-client-2.9/tvb/adapters/visualizers/wavelet_spectrogram.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/__init__.py` & `tvb-rest-client-2.9/tvb/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/algorithm_categories.py` & `tvb-rest-client-2.9/tvb/config/algorithm_categories.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/alembic/env.py` & `tvb-rest-client-2.9/tvb/config/init/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py` & `tvb-rest-client-2.9/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py` & `tvb-rest-client-2.9/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py` & `tvb-rest-client-2.9/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/datatypes_registry.py` & `tvb-rest-client-2.9/tvb/config/init/datatypes_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/initializer.py` & `tvb-rest-client-2.9/tvb/config/init/initializer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/introspector_registry.py` & `tvb-rest-client-2.9/tvb/config/init/introspector_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/init/model_manager.py` & `tvb-rest-client-2.9/tvb/config/init/model_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/logger/cluster_handler.py` & `tvb-rest-client-2.9/tvb/config/logger/cluster_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/logger/dev_logger_config.conf` & `tvb-rest-client-2.9/tvb/config/logger/dev_logger_config.conf`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/logger/elasticsearch_handler.py` & `tvb-rest-client-2.9/tvb/config/logger/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/logger/logger_config.conf` & `tvb-rest-client-2.9/tvb/config/logger/logger_config.conf`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/config/profile_settings.py` & `tvb-rest-client-2.9/tvb/config/profile_settings.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/__init__.py` & `tvb-rest-client-2.9/tvb/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/abcadapter.py` & `tvb-rest-client-2.9/tvb/core/adapters/abcadapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/abcdisplayer.py` & `tvb-rest-client-2.9/tvb/core/adapters/abcdisplayer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/abcremover.py` & `tvb-rest-client-2.9/tvb/core/adapters/abcremover.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/abcuploader.py` & `tvb-rest-client-2.9/tvb/core/adapters/abcuploader.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/arguments_serialisation.py` & `tvb-rest-client-2.9/tvb/core/adapters/arguments_serialisation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/constants.py` & `tvb-rest-client-2.9/tvb/core/adapters/constants.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/exceptions.py` & `tvb-rest-client-2.9/tvb/core/adapters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/adapters/inputs_processor.py` & `tvb-rest-client-2.9/tvb/core/adapters/inputs_processor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/__init__.py` & `tvb-rest-client-2.9/tvb/core/code_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/base_classes.py` & `tvb-rest-client-2.9/tvb/core/code_versions/base_classes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_manager.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4455_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/4455_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4750_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/4750_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/5454_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/5454_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6093_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6093_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6600_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6600_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6728_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/6728_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7350_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/7350_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7450_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/7450_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/9444_update_code.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/9444_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/__init__.py` & `tvb-rest-client-2.9/tvb/core/code_versions/code_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/decorators.py` & `tvb-rest-client-2.9/tvb/core/decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/exportable.py` & `tvb-rest-client-2.9/tvb/core/entities/exportable.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/002_update_files.py` & `tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/002_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/003_update_files.py` & `tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/003_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/004_update_files.py` & `tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/004_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/005_update_files.py` & `tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/005_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/__init__.py` & `tvb-rest-client-2.9/tvb/core/entities/file/file_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/files_update_manager.py` & `tvb-rest-client-2.9/tvb/core/entities/file/files_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/burst_configuration_h5.py` & `tvb-rest-client-2.9/tvb/core/entities/file/simulator/burst_configuration_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/datatype_measure_h5.py` & `tvb-rest-client-2.9/tvb/core/entities/file/simulator/datatype_measure_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/simulation_history_h5.py` & `tvb-rest-client-2.9/tvb/core/entities/file/simulator/simulation_history_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/view_model.py` & `tvb-rest-client-2.9/tvb/core/entities/file/simulator/view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/filters/chain.py` & `tvb-rest-client-2.9/tvb/core/entities/filters/chain.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/filters/exceptions.py` & `tvb-rest-client-2.9/tvb/core/entities/filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/filters/factory.py` & `tvb-rest-client-2.9/tvb/core/entities/filters/factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/generic_attributes.py` & `tvb-rest-client-2.9/tvb/core/entities/generic_attributes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/load.py` & `tvb-rest-client-2.9/tvb/core/entities/load.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/model/__init__.py` & `tvb-rest-client-2.9/tvb/core/entities/model/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/model/model_burst.py` & `tvb-rest-client-2.9/tvb/core/entities/model/model_burst.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/model/model_datatype.py` & `tvb-rest-client-2.9/tvb/core/entities/model/model_datatype.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/model/model_operation.py` & `tvb-rest-client-2.9/tvb/core/entities/model/model_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,21 +411,23 @@
     """
     __tablename__ = "OPERATION_PROCESS_IDENTIFIERS"
 
     id = Column(Integer, primary_key=True)
     fk_from_operation = Column(Integer, ForeignKey('OPERATIONS.id', ondelete="CASCADE"))
     pid = Column(String)
     job_id = Column(String)
+    host_ip = Column(String)
 
     operation = relationship(Operation, backref=backref('OPERATION_PROCESS_IDENTIFIERS', order_by=id, cascade="delete"))
 
-    def __init__(self, operation_id, pid=None, job_id=None):
+    def __init__(self, operation_id, pid=None, job_id=None, host_ip=None):
         self.fk_from_operation = operation_id
         self.pid = pid
         self.job_id = job_id
+        self.host_ip = host_ip
 
 
 class ResultFigure(Base, Exportable):
     """
     Class for storing figures from results, visualize them eventually next to each other.
     A group of results, with the same session_name will be displayed 
     """
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/model/model_project.py` & `tvb-rest-client-2.9/tvb/core/entities/model/model_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/__init__.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/burst_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/burst_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/datatype_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/datatype_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/exceptions.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/operation_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/operation_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/project_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/project_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/root_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/root_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/session_maker.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/session_maker.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/storage/workflow_dao.py` & `tvb-rest-client-2.9/tvb/core/entities/storage/workflow_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/transient/__init__.py` & `tvb-rest-client-2.9/tvb/core/entities/transient/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/transient/context_overlay.py` & `tvb-rest-client-2.9/tvb/core/entities/transient/context_overlay.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/transient/range_parameter.py` & `tvb-rest-client-2.9/tvb/core/entities/transient/range_parameter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/entities/transient/structure_entities.py` & `tvb-rest-client-2.9/tvb/core/entities/transient/structure_entities.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neocom/_h5loader.py` & `tvb-rest-client-2.9/tvb/core/neocom/_h5loader.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neocom/_registry.py` & `tvb-rest-client-2.9/tvb/core/neocom/_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neocom/h5.py` & `tvb-rest-client-2.9/tvb/core/neocom/h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/_h5accessors.py` & `tvb-rest-client-2.9/tvb/core/neotraits/_h5accessors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/_h5core.py` & `tvb-rest-client-2.9/tvb/core/neotraits/_h5core.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/db.py` & `tvb-rest-client-2.9/tvb/core/neotraits/db.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/forms.py` & `tvb-rest-client-2.9/tvb/core/neotraits/forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/h5.py` & `tvb-rest-client-2.9/tvb/core/neotraits/h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/spatial_model.py` & `tvb-rest-client-2.9/tvb/core/neotraits/spatial_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/uploader_view_model.py` & `tvb-rest-client-2.9/tvb/core/neotraits/uploader_view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/neotraits/view_model.py` & `tvb-rest-client-2.9/tvb/core/neotraits/view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/operation_async_launcher.py` & `tvb-rest-client-2.9/tvb/core/operation_async_launcher.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/operation_hpc_launcher.py` & `tvb-rest-client-2.9/tvb/core/operation_hpc_launcher.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/__init__.py` & `tvb-rest-client-2.9/tvb/core/project_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_manager.py` & `tvb-rest-client-2.9/tvb/core/project_versions/project_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/1_update_project.py` & `tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/1_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/2_update_project.py` & `tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/2_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/3_update_project.py` & `tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/3_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/__init__.py` & `tvb-rest-client-2.9/tvb/core/project_versions/project_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/removers_factory.py` & `tvb-rest-client-2.9/tvb/core/removers_factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/__init__.py` & `tvb-rest-client-2.9/tvb/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/algorithm_service.py` & `tvb-rest-client-2.9/tvb/core/services/algorithm_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/authorization.py` & `tvb-rest-client-2.9/tvb/core/services/authorization.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/backend_client_factory.py` & `tvb-rest-client-2.9/tvb/core/services/backend_client_factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/backend_client.py` & `tvb-rest-client-2.9/tvb/core/services/backend_clients/backend_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/cluster_scheduler_client.py` & `tvb-rest-client-2.9/tvb/core/services/backend_clients/cluster_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/hpc_scheduler_client.py` & `tvb-rest-client-2.9/tvb/core/services/backend_clients/hpc_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/standalone_client.py` & `tvb-rest-client-2.9/tvb/core/services/backend_clients/standalone_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 .. moduleauthor:: Yann Gordon <yann@invalid.tvb>
 """
 
 import os
 import queue
 import signal
 import sys
+import socket
 from subprocess import Popen, PIPE
 from threading import Thread, Event
-
 from tvb.basic.exceptions import TVBException
 from tvb.basic.logger.builder import get_logger
 from tvb.basic.profile import TvbProfile
 from tvb.core.adapters.abcadapter import AdapterLaunchModeEnum, ABCAdapter
 from tvb.core.entities.model.model_operation import OperationProcessIdentifier, STATUS_ERROR, STATUS_CANCELED, Operation
 from tvb.core.entities.storage import dao
 from tvb.core.services.backend_clients.backend_client import BackendClient
@@ -53,17 +53,26 @@
 CURRENT_ACTIVE_THREADS = []
 
 LOCKS_QUEUE = queue.Queue(0)
 for i in range(TvbProfile.current.MAX_THREADS_NUMBER):
     LOCKS_QUEUE.put(1)
 
 
+def get_host_current_host_ip():
+    """
+    :return: current host ip address
+    """
+    hostname = socket.gethostname()
+    ip_addr = socket.gethostbyname(hostname)
+    return ip_addr
+
+
 class OperationExecutor(Thread):
     """
-    Thread in charge for starting an operation, used both on cluster and with stand-alone installations.
+    Thread in charge of starting an operation, used both on cluster and with stand-alone installations.
     """
 
     def __init__(self, op_id):
         Thread.__init__(self)
         self.operation_id = op_id
         self._stop_ev = Event()
 
@@ -87,18 +96,20 @@
         if self.stopped() is False:
 
             env = os.environ.copy()
             env['PYTHONPATH'] = os.pathsep.join(sys.path)
             # anything that was already in $PYTHONPATH should have been reproduced in sys.path
 
             launched_process = Popen(run_params, stdout=PIPE, stderr=PIPE, env=env)
+            current_ip = get_host_current_host_ip()
 
-            LOGGER.debug("Storing pid=%s for operation id=%s launched on local machine." % (operation_id,
-                                                                                            launched_process.pid))
-            op_ident = OperationProcessIdentifier(operation_id, pid=launched_process.pid)
+            LOGGER.info("Storing pid=%s and IP %s for operation id=%s launched on local machine." % (operation_id,
+                                                                                                     current_ip,
+                                                                                                     launched_process.pid))
+            op_ident = OperationProcessIdentifier(operation_id, pid=launched_process.pid, host_ip=current_ip)
             dao.store_entity(op_ident)
 
             if self.stopped():
                 # In the exceptional case where the user pressed stop while the Thread startup is done.
                 # and stop_operation is concurrently asking about OperationProcessIdentity.
                 self.stop_pid(launched_process.pid)
 
@@ -204,15 +215,15 @@
                 raise TVBException(operation.additional_info)
         else:
             thread.start()
 
     @staticmethod
     def execute(operation_id, user_name_label, adapter_instance):
         """Start asynchronous operation locally"""
-        if TvbProfile.current.web.OPENSHIFT_DEPLOY or LOCKS_QUEUE.qsize() == 0:
+        if TvbProfile.current.web.IS_CLOUD_DEPLOY or LOCKS_QUEUE.qsize() == 0:
             operation = dao.get_operation_by_id(operation_id)
             operation.queue_full = True
             dao.store_entity(operation)
             return
 
         LOCKS_QUEUE.get(True)
         StandAloneClient.start_operation(operation_id)
@@ -231,19 +242,21 @@
         stopped = StandAloneClient.stop_operation_process(operation_id, True)
         # Mark operation as canceled in DB and on disk
         BurstService().persist_operation_state(operation, STATUS_CANCELED)
         return stopped
 
     @staticmethod
     def stop_operation_process(operation_id, notify_pods=False):
-        if notify_pods and TvbProfile.current.web.OPENSHIFT_DEPLOY:
+        if notify_pods and TvbProfile.current.web.IS_CLOUD_DEPLOY:
             try:
-                LOGGER.info("Notify pods to stop operation process for {}".format(operation_id))
-                KubeNotifier.notify_pods("/kube/stop_operation_process/{}".format(operation_id),
-                                        TvbProfile.current.web.OPENSHIFT_PROCESSING_OPERATIONS_APPLICATION)
+                executor_ip = dao.get_operation_process_for_operation(operation_id)
+                executor_ip = executor_ip.host_ip
+                LOGGER.info("Notifying pod {} to stop operation {}".format(executor_ip, operation_id))
+                KubeNotifier.do_rest_call_to_pod(executor_ip, "stop_operation_process", operation_id),
+
                 return True
             except Exception as e:
                 LOGGER.error("Stop operation notify error", e)
                 return False
         else:
             # Set the thread stop flag to true
             operation_threads = []
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/burst_config_serialization.py` & `tvb-rest-client-2.9/tvb/core/services/burst_config_serialization.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/burst_service.py` & `tvb-rest-client-2.9/tvb/core/services/burst_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/email_sender.py` & `tvb-rest-client-2.9/tvb/core/services/email_sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,33 +20,42 @@
 #
 #   CITATION:
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 """
+.. moduleauthor:: Adrian Ciu <adrian.ciu@codemart.ro>
 .. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 """
 
 import smtplib
 from email.mime.text import MIMEText
+from tvb.basic.logger.builder import get_logger
+from tvb.core.services.exceptions import EmailException
 
+LOGGER = get_logger(__name__)
 
 
-def send(address_from, address_to, email_subject, email_content):
+def send(address_from, address_to, email_subject, email_content, ignore_exception=True):
     """
     Sends an Email Message
     """
-    email = MIMEText(email_content)
-    email['From'] = address_from
-    email['To'] = address_to
-    email['Subject'] = email_subject
-
-    server = smtplib.SMTP('mail.thevirtualbrain.org', 587)
-    server.ehlo()
-    server.starttls()
-    server.ehlo()
-    server.login('tvb_appserver', 'du5rEpratHAc')
-    server.sendmail(address_from, address_to, email.as_string())
-    server.quit()
-    
-
+    try:
+        email = MIMEText(email_content)
+        email['From'] = address_from
+        email['To'] = address_to
+        email['Subject'] = email_subject
+
+        server = smtplib.SMTP('mail.thevirtualbrain.org', 587)
+        server.ehlo()
+        server.starttls()
+        server.ehlo()
+        server.login('tvb_appserver', 'du5rEpratHAc')
+        server.sendmail(address_from, address_to, email.as_string())
+        server.quit()
+        LOGGER.debug(f"Email sent to {address_to} with subject {email_subject}")
+    except Exception as e:
+        LOGGER.warn(f"Could not send email to {address_to}")
+        if ignore_exception:
+            return
+        raise EmailException('Email could not be sent to user.', e)
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/exceptions.py` & `tvb-rest-client-2.9/tvb/core/services/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,7 +96,13 @@
 
 
 class RemoveDataTypeException(ServicesBaseException):
     """
     Exception to be thrown in case some one tries to remove an
     entity that is used by other entities.
     """
+
+
+class EmailException(ServicesBaseException):
+    """
+    Exception to be thrown in case an email cannot be sent to a user
+    """
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/figure_service.py` & `tvb-rest-client-2.9/tvb/core/services/figure_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/hpc_operation_service.py` & `tvb-rest-client-2.9/tvb/core/services/hpc_operation_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/import_service.py` & `tvb-rest-client-2.9/tvb/core/services/import_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/operation_service.py` & `tvb-rest-client-2.9/tvb/core/services/operation_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/project_service.py` & `tvb-rest-client-2.9/tvb/core/services/project_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.png` & `tvb-rest-client-2.9/tvb/core/services/resources/branding_bar.png`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.svg` & `tvb-rest-client-2.9/tvb/core/services/resources/branding_bar.svg`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/settings_service.py` & `tvb-rest-client-2.9/tvb/core/services/settings_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         storage_changed = new_storage != previous_storage
 
         if TvbProfile.is_first_run() or storage_changed:
             self._check_tvb_folder(new_storage)
 
         # Storage changed but DB didn't, just copy TVB storage to new one.
         if storage_changed and not db_changed:
-            shutil.copytree(previous_storage, new_storage)
+            shutil.copytree(previous_storage, new_storage, dirs_exist_ok=True)
 
         if not os.path.isdir(new_storage):
             os.makedirs(new_storage)
         max_space = data[self.KEY_MAX_DISK_SPACE_USR]
         available_mem_kb = SettingsService.get_disk_free_space(new_storage)
         kb_value = int(max_space) * 2 ** 10
         if not (0 < kb_value < available_mem_kb):
@@ -237,12 +237,15 @@
 
         if not os.access(storage_path, os.W_OK):
             raise InvalidSettingsException('TVB Storage folder should have write access for tvb process')
 
         list_content = os.listdir(storage_path)
         if "TEMP" in list_content:
             list_content.remove("TEMP")
+        # database was already created and validated in the folder
+        if len(list_content) == 1 and list_content[0] in TvbProfile.current.db.DB_URL:
+            list_content.remove(list_content[0])
         if len(list_content) > 0:
             raise InvalidSettingsException(
                 'TVB Storage should be empty, please set another folder than {}.'.format(storage_path))
 
         return True
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/simulator_service.py` & `tvb-rest-client-2.9/tvb/core/services/simulator_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/texture_to_json.py` & `tvb-rest-client-2.9/tvb/core/services/texture_to_json.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/core/services/user_service.py` & `tvb-rest-client-2.9/tvb/core/services/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,17 +109,15 @@
 
             if role != ROLE_ADMINISTRATOR and email is not None and not skip_sending_email:
                 admins = UserService.get_administrators()
                 admin = admins[random.randint(0, len(admins) - 1)]
                 if admin.email is not None and (admin.email != TvbProfile.current.web.admin.DEFAULT_ADMIN_EMAIL):
                     # Do not send validation email in case default admin email remained unchanged
                     email_sender.send(FROM_ADDRESS, admin.email, SUBJECT_REGISTER, admin_msg)
-                    self.logger.debug("Email sent to:" + admin.email + " for validating user:" + username + " !")
                 email_sender.send(FROM_ADDRESS, email, SUBJECT_REGISTER, email_msg)
-                self.logger.debug("Email sent to:" + email + " for notifying new user:" + username + " !")
 
             user = dao.store_entity(user)
 
             if role == ROLE_ADMINISTRATOR and not skip_import:
                 to_upload = os.path.join(os.path.dirname(tvb_data.__file__), "Default_Project.zip")
                 if not os.path.exists(to_upload):
                     self.logger.warning("Could not find DEFAULT PROJECT at path %s. You might want to import it "
@@ -188,18 +186,18 @@
             else:
                 user = dao.get_user_by_name(name)
             if user is None or user.validated:
                 self.logger.debug("UserName not found or already validated:" + name)
                 return False
             user.validated = True
             user = dao.store_entity(user)
-            self.logger.debug("Sending validation email for userName=" + user.username + " to address=" + user.email)
+            self.logger.info("Validating user with userName=" + user.username)
             email_sender.send(FROM_ADDRESS, user.email, SUBJECT_VALIDATE,
                               "Hello " + user.username + TEXT_VALIDATED + TvbProfile.current.web.BASE_URL + "/user/")
-            self.logger.info("User:" + user.username + " was validated successfully" + " and notification email sent!")
+            self.logger.info("User:" + user.username + " was validated successfully")
             return True
         except Exception as excep:
             self.logger.warning('Could not validate user:')
             self.logger.warning('WARNING : ' + str(excep))
             return False
 
     @staticmethod
```

### Comparing `tvb-rest-client-2.8.1/tvb/core/utils.py` & `tvb-rest-client-2.9/tvb/core/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/__init__.py` & `tvb-rest-client-2.9/tvb/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/bids_data_builder.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/client_decorators.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/client_decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/datatype_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/datatype/datatype_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/fire_simulation.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/fire_simulation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/launch_operation.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/launch_operation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/utils.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/examples/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/main_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/main_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/operation_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/operation/operation_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/project_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/project/project_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/simulation_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/simulator/simulation_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/rest_test.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tvb_client.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/tvb_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/user_api.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/client/user/user_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/decoders.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/decoders.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/dtos.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/dtos.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/exceptions.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/files_helper.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/files_helper.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/status_codes.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/status_codes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/strings.py` & `tvb-rest-client-2.9/tvb/interfaces/rest/commons/strings.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.8.1/tvb_rest_client.egg-info/PKG-INFO` & `tvb-rest-client-2.9/tvb_rest_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,41 @@
 Metadata-Version: 2.1
 Name: tvb-rest-client
-Version: 2.8.1
+Version: 2.9
 Summary: A helper package for preparing and sending requests towards the TVB REST API
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
-Provides-Extra: postgres
-Provides-Extra: test
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: alembic
+Requires-Dist: h5py
+Requires-Dist: nibabel
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: psutil
+Requires-Dist: pyAesCrypt
+Requires-Dist: requests
+Requires-Dist: scipy
+Requires-Dist: simplejson
+Requires-Dist: sqlalchemy
+Requires-Dist: tvb-data
+Requires-Dist: tvb-gdist
+Requires-Dist: tvb-library
+Requires-Dist: tvb-storage
+Requires-Dist: werkzeug
+Provides-Extra: postgres
+Requires-Dist: psycopg2; extra == "postgres"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
 
 TVB REST client
 ===============
 
 The `tvb-rest-client` is a helper package built with the intention to simplify a
 Python client interaction with TVB REST Server.
 All the logic necessary to prepare and send requests towards the REST server, is embedded under this client API.
@@ -32,15 +52,15 @@
 =====
 You should have a TVB REST server running, or access to a public one.
 Then into `tvb-rest-client` you need to provide the URL towards this TVB REST server.
 For the following example, we will suppose TVB REST server runs on *http://localhost:9090*
 
 To launch a TVB REST server locally, you should download `tvb-framework` version >2.0. and launch it::
 
-    $ python -m tvb.interfaces.web.run WEB_PROFILE  # Launch TVB web and REST servers locally
+    $ python -m tvb.interfaces.rest.server.run   # Launch TVB REST server locally
 
 
 Accessing the client API entry-point
 -------------------------------------
 
 If the TVB REST server you want to access runs at another address, change the parameter
 in the bellow TVBClient instantiation.
```

### Comparing `tvb-rest-client-2.8.1/tvb_rest_client.egg-info/SOURCES.txt` & `tvb-rest-client-2.9/tvb_rest_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 tvb/config/init/datatypes_registry.py
 tvb/config/init/initializer.py
 tvb/config/init/introspector_registry.py
 tvb/config/init/model_manager.py
 tvb/config/init/alembic/env.py
 tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
 tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+tvb/config/init/alembic/versions/32d4bf9f8ghj_update_db_004.py
 tvb/config/init/alembic/versions/__init__.py
 tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
 tvb/config/logger/__init__.py
 tvb/config/logger/cluster_handler.py
 tvb/config/logger/dev_logger_config.conf
 tvb/config/logger/elasticsearch_handler.py
 tvb/config/logger/logger_config.conf
```

