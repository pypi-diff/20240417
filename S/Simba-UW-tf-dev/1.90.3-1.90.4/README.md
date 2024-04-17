# Comparing `tmp/Simba-UW-tf-dev-1.90.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.90.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.90.3.tar", last modified: Tue Apr 16 14:56:22 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.90.4.tar", last modified: Wed Apr 17 20:00:43 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.90.3.tar` & `Simba-UW-tf-dev-1.90.4.tar`

### file list

```diff
@@ -1,640 +1,641 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9734 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    24905 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7979 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3402 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10747 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2741 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.90.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.90.3/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-10 01:59:19.000000 Simba-UW-tf-dev-1.90.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.90.3/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.90.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    48428 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56305 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    32080 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24046 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35642 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   154174 2024-04-16 14:45:49.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    86733 2024-04-15 21:17:25.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    56822 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15278 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.90.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.3/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    49882 2024-04-15 15:19:23.000000 Simba-UW-tf-dev-1.90.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    77633 2024-04-15 16:29:01.000000 Simba-UW-tf-dev-1.90.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    15356 2024-04-12 00:53:11.000000 Simba-UW-tf-dev-1.90.3/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    44962 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)      717 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/utils/keyboard_listener.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:37:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.90.3/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17927 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11843 2024-04-15 15:19:23.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10376 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17433 2024-04-15 16:29:01.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    22893 2024-02-21 04:33:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13622 2024-02-21 04:25:14.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    11075 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9368 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    25934 2024-04-16 14:26:56.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14075 2024-02-24 20:34:51.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    25355 2024-04-15 16:29:01.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9311 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    16754 2024-04-15 20:55:33.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    22994 2024-02-21 04:08:15.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12286 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.90.3/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    14926 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20288 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4793 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    16335 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    23780 2024-04-16 13:40:08.000000 Simba-UW-tf-dev-1.90.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.90.3/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.90.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    12190 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1803 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50018 2024-03-11 20:20:39.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    30615 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15704 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    13394 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29730 2024-03-14 14:41:12.000000 Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   119688 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.90.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.90.3/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    23144 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-16 14:56:21.000000 Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.90.3/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.90.3/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.90.3/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.90.3/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.90.3/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3992 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.3/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.90.3/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18403 2024-02-12 00:49:21.000000 Simba-UW-tf-dev-1.90.3/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-16 14:56:20.000000 Simba-UW-tf-dev-1.90.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-16 14:56:22.000000 Simba-UW-tf-dev-1.90.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9734 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25835 2024-04-17 19:20:44.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7979 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3402 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10747 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2741 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.90.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.90.4/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-10 01:59:19.000000 Simba-UW-tf-dev-1.90.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.90.4/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.90.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    48428 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56305 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    32080 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24046 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35642 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   154174 2024-04-16 14:45:49.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    88755 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    56822 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15278 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.90.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.4/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    49882 2024-04-15 15:19:23.000000 Simba-UW-tf-dev-1.90.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    77633 2024-04-15 16:29:01.000000 Simba-UW-tf-dev-1.90.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.90.4/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    44962 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)      717 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/utils/keyboard_listener.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:37:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.90.4/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17927 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11843 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10376 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17433 2024-04-15 16:29:01.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    22893 2024-02-21 04:33:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13622 2024-02-21 04:25:14.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12949 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9368 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22069 2024-04-17 19:37:05.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14075 2024-02-24 20:34:51.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19312 2024-04-17 19:37:05.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9311 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    16812 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    22994 2024-02-21 04:08:15.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12286 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.90.4/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    14926 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20288 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4793 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    16335 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.90.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.90.4/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.90.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    12190 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1803 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50018 2024-03-11 20:20:39.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    30615 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15704 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    13394 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29730 2024-03-14 14:41:12.000000 Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   119697 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.90.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.90.4/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-17 20:00:42.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    23176 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-17 20:00:42.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-17 20:00:42.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-17 20:00:42.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-17 20:00:42.000000 Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.90.4/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.90.4/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.90.4/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.90.4/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.90.4/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3992 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.4/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.90.4/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.4/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-17 19:59:45.000000 Simba-UW-tf-dev-1.90.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-17 20:00:43.000000 Simba-UW-tf-dev-1.90.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.90.3/PKG-INFO` & `Simba-UW-tf-dev-1.90.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.90.3
+Version: 1.90.4
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 __author__ = "Simon Nilsson"
 
 import os
-from collections import defaultdict
+import threading
 from copy import deepcopy
 from tkinter import *
+from typing import Union
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.plotting.path_plotter import PathPlotterSingleCore
 from simba.plotting.path_plotter_mp import PathPlotterMulticore
 from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu,
                                         Entry_Box)
 from simba.utils.checks import (check_if_filepath_list_is_empty,
                                 check_if_string_value_is_valid_video_timestamp,
                                 check_if_valid_rgb_str, check_int,
                                 check_that_hhmmss_start_is_before_end)
 from simba.utils.enums import Formats, Keys, Links, Paths
 from simba.utils.errors import FrameRangeError
 from simba.utils.read_write import get_file_name_info_in_directory
+from simba.utils.lookups import get_color_dict
+
 
 
 class PathPlotPopUp(PopUpMixin, ConfigReader):
-    def __init__(self, config_path: str):
+    def __init__(self, config_path: Union[str, os.PathLike]):
         ConfigReader.__init__(self, config_path=config_path)
         self.data_path = os.path.join(
             self.project_path, Paths.MACHINE_RESULTS_DIR.value
         )
         self.files_found_dict = get_file_name_info_in_directory(
             directory=self.data_path, file_type=self.file_type
         )
@@ -456,19 +459,15 @@
             check_int(
                 name="PATH FONT SIZE", value=self.font_size.entry_get, min_value=1
             )
             check_int(
                 name="FONT THICKNESS", value=self.font_thickness.entry_get, min_value=1
             )
             if self.bg_clr_dropdown.getChoices() == "Video - static frame":
-                check_int(
-                    name="Static frame index",
-                    value=self.static_frm_index_eb.entry_get,
-                    min_value=0,
-                )
+                check_int(name="Static frame index", value=self.static_frm_index_eb.entry_get, min_value=0,)
                 bg_clr = {
                     "type": "static",
                     "opacity": int(
                         "".join(
                             c
                             for c in self.bg_opacity_dropdown.getChoices()
                             if c.isdigit()
@@ -484,15 +483,15 @@
                             c
                             for c in self.bg_opacity_dropdown.getChoices()
                             if c.isdigit()
                         )
                     ),
                 }
             else:
-                bg_clr = self.bg_clr_dropdown.getChoices()
+                bg_clr = get_color_dict()[self.bg_clr_dropdown.getChoices()]
 
             style_attr = {
                 "width": width,
                 "height": height,
                 "line width": int(self.line_width.entry_get),
                 "font size": int(self.font_size.entry_get),
                 "font thickness": int(self.font_thickness.entry_get),
@@ -500,40 +499,35 @@
                 "bg color": bg_clr,
                 "clf locations": self.include_clf_locations_var.get(),
             }
 
             if self.max_prior_lines_dropdown.getChoices() == "Entire video":
                 style_attr["max lines"] = "entire video"
             else:
-                check_int(
-                    name="PATH MAX LINES",
-                    value=self.max_lines_entry.entry_get,
-                    min_value=1,
-                )
-                style_attr["max lines"] = self.max_lines_entry.entry_get
+                check_int(name="PATH MAX LINES", value=self.max_lines_entry.entry_get, min_value=1)
+                style_attr["max lines"] = int(self.max_lines_entry.entry_get)
 
-        animal_attr = defaultdict(list)
-        for attr in (self.bp_dropdowns, self.bp_colors):
-            for key, value in attr.items():
-                animal_attr[key].append(value.getChoices())
-        for c, (k, v) in enumerate(animal_attr.items()):
-            if v[1] == "Custom":
-                custom_rgb_val = self.custom_rgb_selections[c].entry_get
-                custom_rgb_val = check_if_valid_rgb_str(input=custom_rgb_val)
-                animal_attr[k] = [v[0], custom_rgb_val]
+        animal_attr = {}
+        for cnt, (key, value) in enumerate(self.bp_colors.items()):
+            if cnt not in animal_attr.keys(): animal_attr[cnt] = {}
+            clr = value.getChoices()
+            if clr == "Custom":
+                clr = self.custom_rgb_selections[cnt].entry_get
+                clr = check_if_valid_rgb_str(input=clr)
+                animal_attr[cnt]['color'] = clr
+            else:
+                animal_attr[cnt]['color'] = get_color_dict()[value.getChoices()]
+        for cnt, (key, value) in enumerate(self.bp_dropdowns.items()):
+            if cnt not in animal_attr.keys(): animal_attr[cnt] = {}
+            animal_attr[cnt]['bp'] = value.getChoices()
 
         self.slicing = None
         if self.slice_var.get():
-            check_if_string_value_is_valid_video_timestamp(
-                value=self.video_start_time_entry.entry_get,
-                name="Video slicing START TIME",
-            )
-            check_if_string_value_is_valid_video_timestamp(
-                value=self.video_end_time_entry.entry_get, name="Video slicing END TIME"
-            )
+            check_if_string_value_is_valid_video_timestamp(value=self.video_start_time_entry.entry_get, name="Video slicing START TIME")
+            check_if_string_value_is_valid_video_timestamp(value=self.video_end_time_entry.entry_get, name="Video slicing END TIME")
             if (
                 self.video_start_time_entry.entry_get
                 == self.video_end_time_entry.entry_get
             ):
                 raise FrameRangeError(
                     msg="The sliced start and end times cannot be identical",
                     source=self.__class__.__name__,
@@ -546,53 +540,53 @@
             self.slicing = {
                 "start_time": self.video_start_time_entry.entry_get,
                 "end_time": self.video_end_time_entry.entry_get,
             }
 
         clf_attr = None
         if self.include_clf_locations_var.get():
-            clf_attr = defaultdict(list)
-            for attr in (self.clf_name, self.clf_clr, self.clf_size):
-                for key, value in attr.items():
-                    clf_attr[key].append(value.getChoices())
+            clf_attr = {}
+            for cnt, (key, value) in enumerate(self.clf_name.items()):
+                clf_attr[value.getChoices()] = {}
+                clf_attr[value.getChoices()]['color'] = get_color_dict()[self.clf_clr[cnt].getChoices()]
+                size = "".join(filter(str.isdigit, self.clf_size[cnt].getChoices()))
+                clf_attr[value.getChoices()]['size'] = int(size)
 
         if multiple_videos:
             data_paths = list(self.files_found_dict.values())
         else:
-            data_paths = [
-                self.files_found_dict[self.single_video_dropdown.getChoices()]
-            ]
+            data_paths = [self.files_found_dict[self.single_video_dropdown.getChoices()]]
 
         if not self.multiprocessing_var.get():
-            path_plotter = PathPlotterSingleCore(
-                config_path=self.config_path,
-                frame_setting=self.path_frames_var.get(),
-                video_setting=self.path_videos_var.get(),
-                last_frame=self.path_last_frm_var.get(),
-                files_found=data_paths,
-                input_style_attr=style_attr,
-                print_animal_names=self.include_animal_names_var.get(),
-                animal_attr=animal_attr,
-                input_clf_attr=clf_attr,
-                slicing=self.slicing,
-            )
+            path_plotter = PathPlotterSingleCore(config_path=self.config_path,
+                                                 frame_setting=self.path_frames_var.get(),
+                                                 video_setting=self.path_videos_var.get(),
+                                                 last_frame=self.path_last_frm_var.get(),
+                                                 files_found=data_paths,
+                                                 input_style_attr=style_attr,
+                                                 print_animal_names=self.include_animal_names_var.get(),
+                                                 animal_attr=animal_attr,
+                                                 clf_attr=clf_attr,
+                                                 slicing=self.slicing)
         else:
-            path_plotter = PathPlotterMulticore(
-                config_path=self.config_path,
-                frame_setting=self.path_frames_var.get(),
-                video_setting=self.path_videos_var.get(),
-                last_frame=self.path_last_frm_var.get(),
-                files_found=data_paths,
-                input_style_attr=style_attr,
-                print_animal_names=self.include_animal_names_var.get(),
-                animal_attr=animal_attr,
-                input_clf_attr=clf_attr,
-                cores=int(self.multiprocess_dropdown.getChoices()),
-                slicing=self.slicing,
+            path_plotter = PathPlotterMulticore(config_path=self.config_path,
+                                                frame_setting=self.path_frames_var.get(),
+                                                video_setting=self.path_videos_var.get(),
+                                                last_frame=self.path_last_frm_var.get(),
+                                                files_found=data_paths,
+                                                input_style_attr=style_attr,
+                                                print_animal_names=self.include_animal_names_var.get(),
+                                                animal_attr=animal_attr,
+                                                clf_attr=clf_attr,
+                                                cores=int(self.multiprocess_dropdown.getChoices()),
+                                                slicing=self.slicing,
             )
 
-        path_plotter.run()
+        threading.Thread(target=path_plotter.run()).start()
+
+
 
+# _ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini')
 
 # _ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 
 # _ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.90.4/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.90.4/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.90.4/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.90.4/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.90.4/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.90.4/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.90.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.90.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.90.4/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.90.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/plotting_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 except:
     from typing_extensions import Literal
 
 import simba
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_if_dir_exists, check_instance, check_str,
                                 check_that_column_exist, check_valid_array,
-                                check_valid_lst)
+                                check_valid_lst, check_if_valid_rgb_tuple, check_int, check_float, check_if_keys_exist_in_dict)
 from simba.utils.enums import Formats, Options, TextOptions
 from simba.utils.errors import InvalidInputError
 from simba.utils.lookups import (get_categorical_palettes, get_color_dict,
                                  get_named_colors)
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.utils.read_write import get_fn_ext, read_frm_of_video
 
@@ -320,118 +320,14 @@
         cv2.imwrite(save_path, img)
         stdout_success(
             msg=f"Final distance plot saved at {save_path}",
             elapsed_time=timer.elapsed_time_str,
             source=self.__class__.__name__,
         )
 
-    def make_path_plot(
-        self,
-        data_df: pd.DataFrame,
-        video_info: pd.DataFrame,
-        style_attr: dict,
-        deque_dict: dict,
-        clf_attr: dict,
-        save_path: str,
-        print_animal_names: bool = True,
-    ) -> None:
-        """
-        Helper to make a path plot.
-
-        :param pd.DataFrame data_df: Dataframe holding body-part coordinates
-        :param pd.DataFrame video_info: Video info dataframe (parsed project_folder/logs/video_info.csv)
-        :param dict style_attr: Dict holding image style attributes. E.g., {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
-        :param dict deque_dict: Dict with deque holsing all paths to visualize
-        :param dict clf_attr: Dict holding image classifictaion attributes e.g., {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
-        :param str save_path: Location to save image
-        """
-
-        video_timer = SimbaTimer(start=True)
-        for frm_cnt in range(len(data_df)):
-            for animal_cnt, (animal_name, animal_data) in enumerate(deque_dict.items()):
-                bp_x = int(data_df.iloc[frm_cnt][f'{animal_data["bp"]}_{"x"}'])
-                bp_y = int(data_df.iloc[frm_cnt][f'{animal_data["bp"]}_{"y"}'])
-                deque_dict[animal_name]["deque"].appendleft((bp_x, bp_y))
-
-        font = cv2.FONT_HERSHEY_COMPLEX
-        color_dict = get_color_dict()
-
-        if not isinstance(style_attr["bg color"], np.ndarray):
-            img = np.zeros(
-                (
-                    int(video_info["Resolution_height"].values[0]),
-                    int(video_info["Resolution_width"].values[0]),
-                    3,
-                )
-            )
-        else:
-            img = np.zeros(
-                (
-                    int(style_attr["bg color"].shape[0]),
-                    int(style_attr["bg color"].shape[1]),
-                    3,
-                )
-            )
-        img[:] = style_attr["bg color"]
-
-        for animal_name, animal_data in deque_dict.items():
-            cv2.circle(
-                img,
-                (deque_dict[animal_name]["deque"][0]),
-                0,
-                deque_dict[animal_name]["clr"],
-                style_attr["circle size"],
-            )
-            if print_animal_names:
-                cv2.putText(
-                    img,
-                    animal_name,
-                    (deque_dict[animal_name]["deque"][0]),
-                    font,
-                    style_attr["font size"],
-                    deque_dict[animal_name]["clr"],
-                    style_attr["font thickness"],
-                )
-
-        for animal_name, animal_data in deque_dict.items():
-            for i in range(len(deque_dict[animal_name]["deque"]) - 1):
-                line_clr = deque_dict[animal_name]["clr"]
-                position_1 = deque_dict[animal_name]["deque"][i]
-                position_2 = deque_dict[animal_name]["deque"][i + 1]
-                cv2.line(
-                    img, position_1, position_2, line_clr, style_attr["line width"]
-                )
-
-        if clf_attr:
-            for clf_cnt, clf_name in enumerate(clf_attr["data"].columns):
-                clf_size = int(clf_attr["attr"][clf_cnt][-1].split(": ")[-1])
-                clf_clr = color_dict[clf_attr["attr"][clf_cnt][1]]
-                clf_sliced_idx = list(
-                    clf_attr["data"][clf_attr["data"][clf_name] == 1].index
-                )
-                positions = (
-                    clf_attr["positions"]
-                    .loc[clf_sliced_idx]
-                    .reset_index(drop=True)
-                    .values
-                )
-                for i in range(positions.shape[0]):
-                    cv2.circle(
-                        img, (positions[i][0], positions[i][1]), 0, clf_clr, clf_size
-                    )
-
-        video_timer.stop_timer()
-        img = cv2.resize(img, (style_attr["width"], style_attr["height"]))
-        cv2.imwrite(save_path, img)
-        stdout_success(
-            msg=f"Final path plot saved at {save_path}",
-            elapsed_time=video_timer.elapsed_time_str,
-            source=self.__class__.__name__,
-        )
-
     def make_gantt_plot(
         self,
         data_df: pd.DataFrame,
         bouts_df: pd.DataFrame,
         clf_names: List[str],
         fps: int,
         style_attr: dict,
@@ -1579,15 +1475,17 @@
                 input_style_attr["bg color"]["type"]
             ) == "moving":
                 check_file_exist_and_readable(file_path=video_path)
                 video_cap = cv2.VideoCapture(video_path)
 
         for i in range(data.shape[0]):
             if input_style_attr is not None:
-                if (type(input_style_attr["bg color"]) == dict) and (input_style_attr["bg color"]["type"]) == "moving":
+                if (type(input_style_attr["bg color"]) == dict) and (
+                    input_style_attr["bg color"]["type"]
+                ) == "moving":
                     style_attr["bg color"] = input_style_attr["bg color"]
             frame_id = int(data[i][1])
             frame_data = data[i][2:].astype(int)
             frame_data = np.split(frame_data, len(list(animal_attr.keys())), axis=0)
             img = np.zeros(
                 (
                     int(video_info["Resolution_height"].values[0]),
@@ -1604,16 +1502,24 @@
                     frame_index=frame_id,
                 )
 
             img[:] = style_attr["bg color"]
             for animal_cnt, animal_data in enumerate(frame_data):
                 animal_clr = style_attr["animal clrs"][animal_cnt]
                 print(animal_data)
-                cv2.line(img, tuple(animal_data), animal_clr, int(style_attr["line width"]))
-                cv2.circle(img, tuple(animal_data[-1]), 0, animal_clr, style_attr["circle size"],)
+                cv2.line(
+                    img, tuple(animal_data), animal_clr, int(style_attr["line width"])
+                )
+                cv2.circle(
+                    img,
+                    tuple(animal_data[-1]),
+                    0,
+                    animal_clr,
+                    style_attr["circle size"],
+                )
                 if print_animal_names:
                     cv2.putText(
                         img,
                         style_attr["animal names"][animal_cnt],
                         tuple(animal_data[-1]),
                         cv2.FONT_HERSHEY_COMPLEX,
                         style_attr["font size"],
@@ -2244,7 +2150,102 @@
             pio.write_image(fig, save_path)
             stdout_success(msg=f"Line plot saved at {save_path}")
         else:
             img_bytes = fig.to_image(format="png")
             img = PIL.Image.open(io.BytesIO(img_bytes))
             fig = None
             return np.array(img).astype(np.uint8)
+
+    @staticmethod
+    def make_path_plot(data: List[np.ndarray],
+                       colors: List[Tuple[int, int, int]],
+                       width: Optional[int] = 640,
+                       height: Optional[int] = 480,
+                       max_lines: Optional[int] = None,
+                       bg_clr: Optional[Union[Tuple[int, int, int], np.ndarray]] = (255, 255, 255),
+                       circle_size: Optional[Union[int, None]] = 3,
+                       font_size: Optional[float] = 2.0,
+                       font_thickness: Optional[int] = 2,
+                       line_width: Optional[int] = 2,
+                       animal_names: Optional[List[str]] = None,
+                       clf_attr: Optional[Dict[str, Any]] = None,
+                       save_path: Optional[Union[str, os.PathLike]] = None) -> Union[None, np.ndarray]:
+
+        """
+        Creates a path plot visualization from the given data.
+
+        .. image:: _static/img/make_path_plot.png
+           :width: 500
+           :align: center
+
+        :param List[np.ndarray] data: List of numpy arrays containing path data.
+        :param List[Tuple[int, int, int]] colors: List of RGB tuples representing colors for each path.
+        :param width: Width of the output image (default is 640 pixels).
+        :param height: Height of the output image (default is 480 pixels).
+        :param max_lines: Maximum number of lines to plot from each path data.
+        :param bg_clr: Background color of the plot (default is white).
+        :param circle_size: Size of the circle marker at the end of each path (default is 3).
+        :param font_size: Font size for displaying animal names (default is 2.0).
+        :param font_thickness: Thickness of the font for displaying animal names (default is 2).
+        :param line_width: Width of the lines representing paths (default is 2).
+        :param animal_names: List of names for the animals corresponding to each path.
+        :param clf_attr: Dictionary containing attributes for classification markers.
+        :param save_path: Path to save the generated plot image.
+        :return: If save_path is None, returns the generated image as a numpy array, otherwise, returns None.
+
+
+        :example:
+        >>> x = np.random.randint(0, 500, (100, 2))
+        >>> y = np.random.randint(0, 500, (100, 2))
+        >>> position_data = np.random.randint(0, 500, (100, 2))
+        >>> clf_data_1 = np.random.randint(0, 2, (100,))
+        >>> clf_data_2 = np.random.randint(0, 2, (100,))
+        >>> clf_data = {'Attack': {'color': (155, 1, 10), 'size': 30, 'positions': position_data, 'clfs': clf_data_1},  'Sniffing': {'color': (155, 90, 10), 'size': 30, 'positions': position_data, 'clfs': clf_data_2}}
+        >>> PlottingMixin.make_path_plot(data=[x, y], colors=[(0, 255, 0), (255, 0, 0)], clf_attr=clf_data)
+        """
+
+        check_valid_lst(data=data, source=PlottingMixin.make_path_plot.__name__, valid_dtypes=(np.ndarray,), min_len=1)
+        for i in data: check_valid_array(data=i, source=PlottingMixin.make_path_plot.__name__, accepted_ndims=(2,),
+                                         accepted_axis_1_shape=(2,),
+                                         accepted_dtypes=(int, float, np.int32, np.int64, np.float32, np.float64))
+        check_valid_lst(data=colors, source=PlottingMixin.make_path_plot.__name__, valid_dtypes=(tuple,), exact_len=len(data))
+        for i in colors: check_if_valid_rgb_tuple(data=i)
+        check_instance(source='bg_clr', instance=bg_clr, accepted_types=(np.ndarray, tuple))
+        if isinstance(bg_clr, tuple):
+            check_if_valid_rgb_tuple(data=bg_clr)
+        check_int(name=f'{PlottingMixin.make_path_plot.__name__} height', value=height, min_value=1)
+        check_int(name=f'{PlottingMixin.make_path_plot.__name__} height', value=width, min_value=1)
+        check_float(name=f'{PlottingMixin.make_path_plot.__name__} font_size', value=font_size)
+        check_int(name=f'{PlottingMixin.make_path_plot.__name__} font_thickness', value=font_thickness)
+        check_int(name=f'{PlottingMixin.make_path_plot.__name__} line_width', value=line_width)
+        timer = SimbaTimer(start=True)
+        img = np.zeros((height, width, 3))
+        img[:] = bg_clr
+        for line_cnt in range(len(data)):
+            clr = colors[line_cnt]
+            line_data = data[line_cnt]
+            if max_lines is not None:
+                check_int(name=f'{PlottingMixin.make_path_plot.__name__} max_lines', value=max_lines, min_value=1)
+                line_data = line_data[-max_lines:]
+            for i in range(1, line_data.shape[0]):
+                cv2.line(img, tuple(line_data[i]), tuple(line_data[i - 1]), clr, line_width)
+            if circle_size is not None:
+                cv2.circle(img, tuple(line_data[-1]), 0, clr, circle_size)
+            if animal_names is not None:
+                cv2.putText(img, animal_names[line_cnt], tuple(line_data[-1]), cv2.FONT_HERSHEY_COMPLEX, font_size, clr,
+                            font_thickness)
+        if clf_attr is not None:
+            check_instance(source=PlottingMixin.make_path_plot.__name__, instance=clf_attr, accepted_types=(dict,))
+            for k, v in clf_attr.items():
+                check_if_keys_exist_in_dict(data=v, key=['color', 'size', 'positions', 'clfs'], name='clf_attr')
+            for clf_name, clf_data in clf_attr.items():
+                clf_positions = clf_data['positions'][np.argwhere(clf_data['clfs'] == 1).flatten()]
+                for i in clf_positions:
+                    cv2.circle(img, tuple(i), 0, clf_data['color'], clf_data['size'])
+        img = cv2.resize(img, (width, height)).astype(np.uint8)
+        if save_path is not None:
+            check_if_dir_exists(in_dir=os.path.dirname(save_path))
+            timer.stop_timer()
+            cv2.imwrite(save_path, img)
+            stdout_success(msg=f"Path plot saved at {save_path}", elapsed_time=timer.elapsed_time_str, source=PlottingMixin.make_path_plot.__name__, )
+        else:
+            return img
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.90.4/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.90.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/lookups.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,14 @@
     }
 
 
 def video_quality_to_preset_lookup() -> Dict[str, str]:
     """
     Create dictionary that matches human-readable video quality settings to FFmpeg presets for GPU codecs.
     """
-
     return {"Low": "fast", "Medium": "medium", "High": "slow"}
 
 
 def get_log_config():
     return {
         "version": 1,
         "disable_existing_loggers": False,
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/keyboard_listener.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.90.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.90.4/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.90.4/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/distance_plotter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,235 +1,252 @@
 __author__ = "Simon Nilsson"
 
-import functools
-import multiprocessing
 import os
-import platform
-import shutil
-from typing import Dict, List
+from typing import Dict, List, Optional, Union
 
 import cv2
 import numpy as np
-import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.plotting_mixin import PlottingMixin
-from simba.utils.checks import check_that_column_exist
-from simba.utils.enums import Formats
-from simba.utils.errors import ColumnNotFoundError, NoSpecifiedOutputError
+from simba.utils.checks import (
+    check_all_file_names_are_represented_in_video_log,
+    check_file_exist_and_readable, check_instance, check_valid_lst)
+from simba.utils.errors import (CountError, InvalidInputError,
+                                NoSpecifiedOutputError)
+from simba.utils.lookups import get_color_dict
 from simba.utils.printing import SimbaTimer, stdout_success
-from simba.utils.read_write import (concatenate_videos_in_folder, get_fn_ext,
-                                    read_df)
+from simba.utils.read_write import get_fn_ext, read_df
 
 
-class TresholdPlotCreatorMultiprocess(ConfigReader, PlottingMixin):
+class DistancePlotterSingleCore(ConfigReader):
     """
-    Class for line chart visualizations displaying the classification probabilities of a single classifier.
-    Uses multiprocessing.
-
-    :param str config_path: path to SimBA project config file in Configparser format
-    :param str clf_name: Name of the classifier to create visualizations for
-    :param bool frame_setting: When True, SimBA creates indidvidual frames in png format
-    :param bool video_setting: When True, SimBA creates compressed video in mp4 format
-    :param bool last_image: When True, creates image .png representing last frame of the video.
-    :param dict style_attr: User-defined style attributes of the visualization (line size, color etc).
-    :param List[str] files_found: Files to create threshold plots for.
-    :param int cores: Number of cores to use.
+    Class for visualizing the distance between two pose-estimated body-parts (e.g., two animals) through line
+    charts. Results are saved as individual line charts, and/or videos of line charts.
 
     .. note::
-       `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
+       For better runtime, use :meth:`simba.plotting.distance_plotter_mp.DistancePlotterMultiCore`.
+       `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
-    .. image:: _static/img/prob_plot.png
+    .. image:: _static/img/distance_plot.png
        :width: 300
        :align: center
 
-    Examples
-    ----------
-    >>> plot_creator = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', frame_setting=True, video_setting=True, clf_name='Attack', style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'magneta', 'circle size': 20}, cores=5)
-    >>> plot_creator.run()
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter bool frame_setting: If True, creates individual frames.
+    :parameter bool video_setting: If True, creates videos
+
+    :examples:
+
+    >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'opacity': 0.5}
+    >>> line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
+    >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', files_found=['test/two_c57s/project_folder/csv/outlier_corrected_movement_location/Video_1.csv'], frame_setting=False, video_setting=True, final_img=True)
+    >>> distance_plotter.run()
     """
 
     def __init__(
         self,
-        config_path: str,
-        clf_name: str,
-        frame_setting: bool,
-        video_setting: bool,
-        last_frame: bool,
-        cores: int,
+        config_path: Union[str, os.PathLike],
+        data_paths: List[Union[str, os.PathLike]],
         style_attr: Dict[str, int],
-        files_found: List[str],
+        line_attr: List[List[str]],
+        frame_setting: Optional[bool] = False,
+        video_setting: Optional[bool] = False,
+        final_img: Optional[bool] = False,
     ):
+
+        if (not frame_setting) and (not video_setting) and (not final_img):
+            raise NoSpecifiedOutputError(
+                msg="Please choice to create frames and/or video distance plots",
+                source=self.__class__.__name__,
+            )
+        check_instance(
+            source=f"{self.__class__.__name__} line_attr",
+            instance=line_attr,
+            accepted_types=(list,),
+        )
+        for cnt, i in enumerate(line_attr):
+            check_valid_lst(
+                source=f"{self.__class__.__name__} line_attr {cnt}",
+                data=i,
+                valid_dtypes=(str,),
+                exact_len=3,
+            )
+        check_valid_lst(data=data_paths, valid_dtypes=(str,), min_len=1)
+        _ = [check_file_exist_and_readable(i) for i in data_paths]
         ConfigReader.__init__(self, config_path=config_path)
-        PlottingMixin.__init__(self)
-        if platform.system() == "Darwin":
-            multiprocessing.set_start_method("spawn", force=True)
         (
-            self.frame_setting,
             self.video_setting,
-            self.cores,
+            self.frame_setting,
+            self.data_paths,
             self.style_attr,
-            self.last_frame,
-        ) = (frame_setting, video_setting, cores, style_attr, last_frame)
-        if (
-            (not self.frame_setting)
-            and (not self.video_setting)
-            and (not self.last_frame)
-        ):
-            raise NoSpecifiedOutputError(
-                "SIMBA ERROR: Please choose to create either probability videos, frames, and/or last frame.",
-                show_window=True,
-            )
-        self.clf_name, self.files_found = clf_name, files_found
-        self.probability_col = "Probability_" + self.clf_name
-        self.fontsize = self.style_attr["font size"]
-        self.out_width, self.out_height = (
-            self.style_attr["width"],
-            self.style_attr["height"],
-        )
-        self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
-        if not os.path.exists(self.probability_plot_dir):
-            os.makedirs(self.probability_plot_dir)
-        print(f"Processing {str(len(self.files_found))} video(s)...")
+            self.line_attr,
+            self.final_img,
+        ) = (video_setting, frame_setting, data_paths, style_attr, line_attr, final_img)
+        self.color_names = get_color_dict()
 
     def run(self):
-        for file_cnt, file_path in enumerate(self.files_found):
+        print(f"Processing {len(self.data_paths)} videos...")
+        check_all_file_names_are_represented_in_video_log(
+            video_info_df=self.video_info_df, data_paths=self.data_paths
+        )
+        for file_cnt, file_path in enumerate(self.data_paths):
             video_timer = SimbaTimer(start=True)
-            _, self.video_name, _ = get_fn_ext(file_path)
-            video_info, self.px_per_mm, self.fps = self.read_video_info(
-                video_name=self.video_name
-            )
             data_df = read_df(file_path, self.file_type)
-            if self.probability_col not in data_df.columns:
-                raise ColumnNotFoundError(
-                    column_name=self.probability_col, file_name=file_path
+            _, video_name, _ = get_fn_ext(file_path)
+            self.video_info, px_per_mm, fps = self.read_video_info(
+                video_name=video_name
+            )
+            self.save_video_folder = os.path.join(self.line_plot_dir, video_name)
+            self.save_frame_folder_dir = os.path.join(self.line_plot_dir, video_name)
+
+            try:
+                data_df.columns = self.bp_headers
+            except ValueError:
+                raise CountError(
+                    msg=f"SimBA expects {self.bp_headers} columns but found {len(data_df)} columns in {file_path}",
+                    source=self.__class__.__name__,
+                )
+            distances = []
+            colors = []
+            for cnt, i in enumerate(self.line_attr):
+                if i[2] not in list(self.color_names.keys()):
+                    raise InvalidInputError(
+                        msg=f"{i[2]} is not a valid color. Options: {list(self.color_names.keys())}.",
+                        source=self.__class__.__name__,
+                    )
+                colors.append(i[2])
+                bp_1, bp_2 = [f"{i[0]}_x", f"{i[0]}_y"], [f"{i[1]}_x", f"{i[1]}_y"]
+                if len(list(set(bp_1) - set(data_df.columns))) > 0:
+                    raise InvalidInputError(
+                        msg=f"Could not find fields {bp_1} in {file_path}",
+                        source=self.__class__.__name__,
+                    )
+                if len(list(set(bp_2) - set(data_df.columns))) > 0:
+                    raise InvalidInputError(
+                        msg=f"Could not find fields {bp_2} in {file_path}",
+                        source=self.__class__.__name__,
+                    )
+                distances.append(
+                    FeatureExtractionMixin.framewise_euclidean_distance(
+                        location_1=data_df[bp_1].values,
+                        location_2=data_df[bp_2].values,
+                        px_per_mm=px_per_mm,
+                        centimeter=True,
+                    )
                 )
-            check_that_column_exist(
-                df=data_df, column_name=self.clf_name, file_name=self.video_name
-            )
-            self.save_frame_folder_dir = os.path.join(
-                self.probability_plot_dir, self.video_name + "_" + self.clf_name
-            )
-            self.video_folder = os.path.join(
-                self.probability_plot_dir, self.video_name + "_" + self.clf_name
-            )
-            self.temp_folder = os.path.join(
-                self.probability_plot_dir, self.video_name + "_" + self.clf_name, "temp"
-            )
             if self.frame_setting:
                 if os.path.exists(self.save_frame_folder_dir):
-                    shutil.rmtree(self.save_frame_folder_dir)
-                if not os.path.exists(self.save_frame_folder_dir):
-                    os.makedirs(self.save_frame_folder_dir)
+                    self.remove_a_folder(self.save_frame_folder_dir)
+                os.makedirs(self.save_frame_folder_dir)
             if self.video_setting:
-                if os.path.exists(self.temp_folder):
-                    shutil.rmtree(self.temp_folder)
-                    shutil.rmtree(self.video_folder)
-                os.makedirs(self.temp_folder)
-                self.save_video_path = os.path.join(
-                    self.probability_plot_dir,
-                    "{}_{}.mp4".format(self.video_name, self.clf_name),
+                save_video_path = os.path.join(self.line_plot_dir, f"{video_name}.avi")
+                fourcc = cv2.VideoWriter_fourcc(*"DIVX")
+                video_writer = cv2.VideoWriter(
+                    save_video_path,
+                    fourcc,
+                    fps,
+                    (self.style_attr["width"], self.style_attr["height"]),
                 )
 
-            probability_lst = list(data_df[self.probability_col])
-
-            if self.last_frame:
-                _ = self.make_probability_plot(
-                    data=pd.Series(probability_lst),
-                    style_attr=self.style_attr,
-                    clf_name=self.clf_name,
-                    fps=self.fps,
+            if self.final_img:
+                _ = PlottingMixin.make_line_plot(
+                    data=distances,
+                    colors=colors,
+                    width=self.style_attr["width"],
+                    height=self.style_attr["height"],
+                    line_width=self.style_attr["line width"],
+                    font_size=self.style_attr["font size"],
+                    title="Animal distances",
+                    y_lbl="distance (cm)",
+                    x_lbl="time (s)",
+                    x_lbl_divisor=fps,
+                    y_max=self.style_attr["y_max"],
+                    line_opacity=self.style_attr["opacity"],
                     save_path=os.path.join(
-                        self.probability_plot_dir,
-                        self.video_name
-                        + "_{}_{}.png".format(self.clf_name, "final_image"),
+                        self.line_plot_dir, f"{video_name}_final_distances.png"
                     ),
                 )
 
             if self.video_setting or self.frame_setting:
-                if self.style_attr["y_max"] == "auto":
-                    highest_p = data_df[self.probability_col].max()
-                else:
-                    highest_p = float(self.style_attr["y_max"])
-                data_split = np.array_split(list(data_df.index), self.cores)
-                frm_per_core = len(data_split[0])
-                for group_cnt, rng in enumerate(data_split):
-                    data_split[group_cnt] = np.insert(rng, 0, group_cnt)
-
-                print(
-                    "Creating probability images, multiprocessing (determined chunksize: {}, cores: {})...".format(
-                        str(self.multiprocess_chunksize), str(self.cores)
-                    )
-                )
-                with multiprocessing.Pool(
-                    self.cores, maxtasksperchild=self.maxtasksperchild
-                ) as pool:
-                    constants = functools.partial(
-                        self.probability_plot_mp,
-                        clf_name=self.clf_name,
-                        probability_lst=probability_lst,
-                        highest_p=highest_p,
-                        video_setting=self.video_setting,
-                        frame_setting=self.frame_setting,
-                        fps=self.fps,
-                        video_dir=self.temp_folder,
-                        frame_dir=self.save_frame_folder_dir,
-                        style_attr=self.style_attr,
-                        video_name=self.video_name,
-                    )
-                    for cnt, result in enumerate(
-                        pool.imap(
-                            constants, data_split, chunksize=self.multiprocess_chunksize
+                if self.style_attr["y_max"] == -1:
+                    self.style_attr["y_max"] = max([np.max(x) for x in distances])
+                for frm_cnt in range(distances[0].shape[0]):
+                    line_data = [x[:frm_cnt] for x in distances]
+                    img = PlottingMixin.make_line_plot_plotly(
+                        data=line_data,
+                        colors=colors,
+                        width=self.style_attr["width"],
+                        height=self.style_attr["height"],
+                        line_width=self.style_attr["line width"],
+                        font_size=self.style_attr["font size"],
+                        title="Animal distances",
+                        y_lbl="distance (cm)",
+                        x_lbl="frame count",
+                        x_lbl_divisor=fps,
+                        y_max=self.style_attr["y_max"],
+                        line_opacity=self.style_attr["opacity"],
+                        save_path=None,
+                    ).astype(np.uint8)
+                    if self.video_setting:
+                        video_writer.write(img[:, :, :3])
+                    if self.frame_setting:
+                        frm_name = os.path.join(
+                            self.save_frame_folder_dir, f"{frm_cnt}.png"
                         )
-                    ):
-                        print(
-                            "Image {}/{}, Video {}/{}...".format(
-                                str(int(frm_per_core * (result + 1))),
-                                str(len(data_df)),
-                                str(file_cnt + 1),
-                                str(len(self.files_found)),
-                            )
-                        )
-
-                pool.join()
-                pool.terminate()
+                        cv2.imwrite(frm_name, np.uint8(img))
+                    print(f"Distance frame created: {frm_cnt}, Video: {video_name} ...")
                 if self.video_setting:
-                    print("Joining {} multiprocessed video...".format(self.video_name))
-                    concatenate_videos_in_folder(
-                        in_folder=self.temp_folder, save_path=self.save_video_path
-                    )
-
+                    video_writer.release()
                 video_timer.stop_timer()
-                print(
-                    "Probability video {} complete (elapsed time: {}s) ...".format(
-                        self.video_name, video_timer.elapsed_time_str
-                    )
+                stdout_success(
+                    msg=f"Distance visualizations created for {video_name} saved at {self.line_plot_dir}",
+                    elapsed_time=video_timer.elapsed_time_str,
                 )
-
         self.timer.stop_timer()
         stdout_success(
-            msg=f"Probability visualizations for {str(len(self.files_found))} videos created in project_folder/frames/output/gantt_plots directory",
+            msg=f"Distance visualizations complete for {len(self.data_paths)} video(s)",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
-# test = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
-#                                         frame_setting=False,
-#                                         video_setting=True,
-#                                         last_frame=False,
-#                                         clf_name='Attack',
-#                                         cores=5,
-#                                         files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/csv/machine_results/Together_1.csv'],
-#                                         style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'blue', 'circle size': 20, 'y_max': 'auto'})
-# #test = TresholdPlotCreatorSingleProcess(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', frame_setting=False, video_setting=True, clf_name='Attack')
-# test.create_plots()
-
-
-# test = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                         frame_setting=False,
-#                                         video_setting=True,
-#                                         last_frame=True,
-#                                         clf_name='Attack',
-#                                         cores=5,
-#                                         files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
-#                                         style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 3, 'color': 'blue', 'circle size': 20, 'y_max': 'auto'})
-# test.create_plots()
+# style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 12, 'y_max': -1, 'opacity': 0.5}
+# line_attr = [['Center_1', 'Center_2', 'Green'], ['Ear_left_2', 'Ear_right_2', 'Red']]
+# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                  frame_setting=True,
+#                                  video_setting=True,
+#                                  style_attr=style_attr,
+#                                  final_img=True,
+#                                  data_paths=['/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location/Together_1.csv'],
+#                                  line_attr=line_attr)
+# test.run()
+
+
+#
+# style_attr = {'width': 640,
+#               'height': 480,
+#               'line width': 6,
+#               'font size': 8,
+#               'y_max': 'auto',
+#               'opacity': 0.9}
+# line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
+#
+# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                  frame_setting=False,
+#                                  video_setting=True,
+#                                  style_attr=style_attr,
+#                                  final_img=True,
+#                                  files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
+#                                  line_attr=line_attr)
+# test.create_distance_plot()
+
+# style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8}
+# line_attr = {0: ['Termite_1_Head_1', 'Termite_1_Thorax_1', 'Dark-red']}
+
+# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini',
+#                                  frame_setting=False,
+#                        video_setting=True,
+#                        style_attr=style_attr,
+#                        files_found=['/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/csv/outlier_corrected_movement_location/termites_1.csv'],
+#                        line_attr=line_attr)
+# test.create_distance_plot()
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/path_plotter_mp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 __author__ = "Simon Nilsson"
 
 import functools
 import multiprocessing
 import os
-import pandas as pd
 import platform
-import cv2
-from collections import deque
 from copy import deepcopy
-from typing import Dict, List, Optional, Union
-
+from typing import Dict, List, Optional, Union, Any, Tuple
+import cv2
 import numpy as np
-from numba import jit, prange
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
-from simba.utils.checks import (check_if_filepath_list_is_empty,
+from simba.utils.checks import (check_file_exist_and_readable,
+                                check_if_keys_exist_in_dict,
                                 check_if_valid_rgb_str, check_int,
-                                check_that_column_exist,
-                                check_file_exist_and_readable)
+                                check_that_column_exist, check_valid_lst, check_instance)
 from simba.utils.data import find_frame_numbers_from_time_stamp
-from simba.utils.enums import TagNames, Formats
+from simba.utils.enums import Formats, TagNames
 from simba.utils.errors import FrameRangeError, NoSpecifiedOutputError
 from simba.utils.printing import SimbaTimer, log_event, stdout_success
 from simba.utils.read_write import (concatenate_videos_in_folder,
-                                    find_video_of_file, get_fn_ext,
-                                    get_video_meta_data, read_df,
-                                    read_frm_of_video, remove_a_folder, find_core_cnt)
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.lookups import get_color_dict
+                                    find_core_cnt, find_video_of_file,
+                                    get_fn_ext, get_video_meta_data, read_df,
+                                    read_frm_of_video, remove_a_folder)
+from simba.mixins.plotting_mixin import PlottingMixin
 
 
-def path_plot_mp(batch_id: np.ndarray,
+def path_plot_mp(frm_rng: np.ndarray,
                  data: np.array,
+                 colors: List[Tuple],
                  video_setting: bool,
                  frame_setting: bool,
                  video_save_dir: str,
                  video_name: str,
                  frame_folder_dir: str,
                  style_attr: dict,
-                 print_animal_names: bool,
-                 animal_attr: dict,
+                 animal_names: Union[None, List[str]],
                  fps: int,
-                 video_info: pd.DataFrame,
                  clf_attr: dict,
                  input_style_attr: dict,
                  video_path: Optional[Union[str, os.PathLike]] = None):
 
-    batch_id = batch_id[0]
-    batch_data = data[np.argwhere(data[:, 0] == batch_id)].reshape(-1, data.shape[1])
-    frm_cnts = batch_data[:, 1]
-    color_dict = get_color_dict()
+    batch_id, frm_rng = frm_rng[0], frm_rng[1]
     if video_setting:
         fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
         video_save_path = os.path.join(video_save_dir, f"{batch_id}.mp4")
         video_writer = cv2.VideoWriter(video_save_path, fourcc, fps, (style_attr["width"], style_attr["height"]))
 
     if input_style_attr is not None:
         if (isinstance(input_style_attr["bg color"], dict)) and (input_style_attr["bg color"]["type"]) == "moving":
             check_file_exist_and_readable(file_path=video_path)
             video_cap = cv2.VideoCapture(video_path)
 
     bg_clr = style_attr["bg color"]
-    for frame_id in frm_cnts:
-        frm_data = data[np.argwhere(data[:, 1] <= frame_id)].reshape(-1, data.shape[1])[:, 2:]
-        frm_data = np.split(frm_data, len(list(animal_attr.keys())), axis=1)
+    for frame_id in frm_rng:
         if (isinstance(style_attr["bg color"], dict)) and (style_attr["bg color"]["type"]) == "moving":
-            bg_clr = read_frm_of_video(video_path=video_cap, opacity=style_attr["bg color"]["opacity"], frame_index=frame_id)
-        img = np.zeros((int(video_info["Resolution_height"].values[0]), int(video_info["Resolution_width"].values[0]), 3))
-        img[:] = bg_clr
-        for animal_cnt, pose_data in enumerate(frm_data):
-            animal_clr = style_attr["animal clrs"][animal_cnt]
-            for j in range(pose_data.shape[0]):
-                cv2.line(img, (pose_data[j][0], pose_data[j][1]), (pose_data[j][2], pose_data[j][3]), animal_clr, int(style_attr["line width"]))
-            cv2.circle(img, (pose_data[-1][2], pose_data[-1][3]), 0, animal_clr, style_attr["circle size"], )
-            if print_animal_names:
-                cv2.putText(img, style_attr["animal names"][animal_cnt], (pose_data[-1][2], pose_data[-1][3]), cv2.FONT_HERSHEY_COMPLEX,style_attr["font size"],animal_clr,style_attr["font thickness"])
-        if clf_attr:
-            for clf_cnt, clf_name in enumerate(clf_attr["data"].columns):
-                clf_size = int(clf_attr["attr"][clf_cnt][-1].split(": ")[-1])
-                clf_clr = color_dict[clf_attr["attr"][clf_cnt][1]]
-                clf_sliced = clf_attr["data"][clf_name].loc[0:frame_id]
-                clf_sliced_idx = list(clf_sliced[clf_sliced == 1].index)
-                locations = clf_attr["positions"][clf_sliced_idx, :]
-                for i in range(locations.shape[0]):
-                    cv2.circle(img, (locations[i][0], locations[i][1]), 0, clf_clr, clf_size)
-        img = cv2.resize(img, (style_attr["width"], style_attr["height"]))
+            bg_clr = read_frm_of_video(video_path=video_cap, opacity=style_attr["bg color"]["opacity"],frame_index=frame_id)
+        plot_arrs = [x[:frame_id, :] for x in data]
+
+        clf_attr_cpy = deepcopy(clf_attr)
+        if clf_attr is not None:
+            for k, v in clf_attr.items():
+                clf_attr_cpy[k]['clfs'][frame_id + 1:] = 0
+
+        img = PlottingMixin.make_path_plot(data=plot_arrs,
+                             colors=colors,
+                             width=style_attr['width'],
+                             height=style_attr['height'],
+                             max_lines=style_attr['max lines'],
+                             bg_clr=bg_clr,
+                             circle_size=style_attr["circle size"],
+                             font_size=style_attr["font size"],
+                             font_thickness=style_attr["font thickness"],
+                             line_width=style_attr["line width"],
+                             animal_names=animal_names,
+                             clf_attr=clf_attr_cpy,
+                             save_path=None)
+
         if video_setting:
             video_writer.write(np.uint8(img))
         if frame_setting:
             frm_name = os.path.join(frame_folder_dir, f"{frame_id}.png")
             cv2.imwrite(frm_name, np.uint8(img))
         print(f"Path frame created: {frame_id}, Video: {video_name}, Processing core: {batch_id}")
     if video_setting:
@@ -112,299 +103,232 @@
     :param Optional[dict] input_clf_attr: Dict reprenting classified behavior locations, their color and size. If None, then no classified behavior locations are shown.
     :param Optional[dict] slicing: If Dict, start time and end time of video slice to create path plot from. E.g., {'start_time': '00:00:01', 'end_time': '00:00:03'}. If None, creates path plot for entire video.
     :param int cores: Number of cores to use.
 
     .. note::
        `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
-    .. important::
-       See :meth:`simba.utils.lookups.get_color_dict` for keys for named color options.
-
     .. image:: _static/img/path_plot.png
        :width: 300
        :align: center
 
+    .. image:: _static/img/path_plot_mp.gif
+       :width: 500
+       :align: center
+
     :example:
     >>> input_style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
     >>> animal_attr = {0: ['Ear_right_1', 'Red']}
     >>> input_clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
     >>> path_plotter = PathPlotterMulticore(config_path=r'MyConfigPath', frame_setting=False, video_setting=True, style_attr=style_attr, animal_attr=animal_attr, files_found=['project_folder/csv/machine_results/MyVideo.csv'], cores=5, clf_attr=clf_attr, print_animal_names=True)
     >>> path_plotter.run()
     """
 
-    def __init__(
-        self,
-        config_path: Union[str, os.PathLike],
-        files_found: List[str],
-        frame_setting: Optional[bool] = False,
-        video_setting: Optional[bool] = False,
-        last_frame: Optional[bool] = True,
-        cores: Optional[int] = -1,
-        print_animal_names: Optional[bool] = False,
-        input_style_attr: Optional[Dict] = None,
-        animal_attr: Dict[int, List[str]] = None,
-        input_clf_attr: Optional[Dict[int, List[str]]] = None,
-        slicing: Optional[Dict] = None):
+    def __init__(self,
+                 config_path: Union[str, os.PathLike],
+                 files_found: List[str],
+                 frame_setting: Optional[bool] = False,
+                 video_setting: Optional[bool] = False,
+                 last_frame: Optional[bool] = True,
+                 cores: Optional[int] = -1,
+                 print_animal_names: Optional[bool] = False,
+                 input_style_attr: Optional[Dict] = None,
+                 animal_attr: Dict[int, Any] = None,
+                 clf_attr: Optional[Dict[int, List[str]]] = None,
+                 slicing: Optional[Dict[str, str]] = None):
 
         if platform.system() == "Darwin":
             multiprocessing.set_start_method("spawn", force=True)
         if (not frame_setting) and (not video_setting) and (not last_frame):
             raise NoSpecifiedOutputError(msg="SIMBA ERROR: Please choice to create path frames and/or video path plots", source=self.__class__.__name__)
-        check_if_filepath_list_is_empty(filepaths=files_found, error_msg="SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. To plot paths without performing machine classifications, use path plotter functions in [ROI] tab.")
+        check_valid_lst(data=files_found, source=self.__class__.__name__, valid_dtypes=(str,))
+
         check_int(name=f"{self.__class__.__name__} core_cnt", value=cores, min_value=-1, max_value=find_core_cnt()[0])
         if cores == -1: cores = find_core_cnt()[0]
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         log_event(logger_name=str(__class__.__name__), log_type=TagNames.CLASS_INIT.value, msg=self.create_log_msg_from_init_args(locals=locals()))
-        self.video_setting, self.frame_setting, self.input_style_attr, self.files_found, self.animal_attr, self.input_clf_attr, self.last_frame, self.cores = video_setting, frame_setting, input_style_attr, files_found, animal_attr, input_clf_attr, last_frame, cores
-        self.print_animal_names = print_animal_names
-        self.no_animals_path_plot, self.clf_attr, self.slicing = (len(animal_attr.keys()), None, slicing)
+        self.video_setting, self.frame_setting, self.input_style_attr, self.files_found, self.animal_attr, self.input_clf_attr, self.last_frame, self.cores = video_setting,frame_setting,input_style_attr,files_found,animal_attr,clf_attr,last_frame,cores
+        self.print_animal_names, self.clf_attr, self.slicing = print_animal_names, clf_attr, slicing
         if not os.path.exists(self.path_plot_dir):
             os.makedirs(self.path_plot_dir)
         print(f"Processing {len(self.files_found)} videos...")
 
     def __get_styles(self):
         self.style_attr = {}
         if self.input_style_attr is not None:
-            if not type(self.input_style_attr["bg color"]) == dict:
-                self.style_attr["bg color"] = self.color_dict[
-                    self.input_style_attr["bg color"]
-                ]
-            else:
-                self.style_attr["bg color"] = self.input_style_attr["bg color"]
+            self.style_attr["bg color"] = self.input_style_attr["bg color"]
             if self.input_style_attr["max lines"] == "entire video":
                 self.style_attr["max lines"] = len(self.data_df)
             else:
-                self.style_attr["max lines"] = int(
-                    int(self.input_style_attr["max lines"])
-                    * (int(self.video_info["fps"].values[0]) / 1000)
-                )
+                self.style_attr["max lines"] = max(1, int(int(self.input_style_attr["max lines"] / 1000) * (int(self.video_info["fps"].values[0]))))
             self.style_attr["font thickness"] = self.input_style_attr["font thickness"]
             self.style_attr["line width"] = self.input_style_attr["line width"]
             self.style_attr["font size"] = self.input_style_attr["font size"]
             self.style_attr["circle size"] = self.input_style_attr["circle size"]
             self.style_attr["print_animal_names"] = self.print_animal_names
             if self.input_style_attr["width"] == "As input":
-                self.style_attr["width"], self.style_attr["height"] = int(
-                    self.video_info["Resolution_width"].values[0]
-                ), int(self.video_info["Resolution_height"].values[0])
+                self.style_attr["width"], self.style_attr["height"] = int(self.video_info["Resolution_width"].values[0]), int(self.video_info["Resolution_height"].values[0])
             else:
                 pass
         else:
             space_scaler, radius_scaler, res_scaler, font_scaler = 25, 10, 1500, 0.8
-            self.style_attr["width"] = int(
-                self.video_info["Resolution_width"].values[0]
-            )
-            self.style_attr["height"] = int(
-                self.video_info["Resolution_height"].values[0]
-            )
+            self.style_attr["width"] = int(self.video_info["Resolution_width"].values[0])
+            self.style_attr["height"] = int(self.video_info["Resolution_height"].values[0])
             max_res = max(self.style_attr["width"], self.style_attr["height"])
             self.style_attr["circle size"] = int(radius_scaler / (res_scaler / max_res))
             self.style_attr["font size"] = font_scaler / (res_scaler / max_res)
             self.style_attr["bg color"] = self.color_dict["White"]
             self.style_attr["print_animal_names"] = self.print_animal_names
             self.style_attr["max lines"] = len(self.data_df)
             self.style_attr["font thickness"] = 2
             self.style_attr["line width"] = 2
 
-        self.style_attr["animal names"] = []
-        self.style_attr["animal clrs"] = []
-        for animal_cnt, animal_data in self.animal_attr.items():
-            self.style_attr["animal names"].append(
-                self.find_animal_name_from_body_part_name(
-                    bp_name=animal_data[0], bp_dict=self.animal_bp_dict
-                )
-            )
-
-        for animal_cnt, animal_data in self.animal_attr.items():
-            if type(self.animal_attr[animal_cnt][1]) == tuple:
-                check_if_valid_rgb_str(
-                    str(self.animal_attr[animal_cnt][1]), return_cleaned_rgb_tuple=False
-                )
-                self.style_attr["animal clrs"] = self.animal_attr[animal_cnt][1]
-            else:
-                self.style_attr["animal clrs"].append(
-                    self.color_dict[self.animal_attr[animal_cnt][1]]
-                )
-
-    @staticmethod
-    @jit(nopython=True)
-    def __insert_group_idx_column(data: np.array, group: int):
-        group_col = np.full((data.shape[0], 1), group)
-        return np.hstack((group_col, data))
-
-    @staticmethod
-    #@jit(nopython=True)
-    def __split_array_into_max_lines(data: np.array, max_lines: int):
-        results = np.full((data.shape[0], max_lines, data.shape[1]), np.nan, data.dtype)
-        for i in prange(data.shape[0]):
-            start = int(i - max_lines)
-            if start < 0:
-                start = 0
-            frm_data = data[start:i, :]
-
-            missing_cnt = max_lines - frm_data.shape[0]
-            if missing_cnt > 0:
-                frm_data = np.vstack((np.full((missing_cnt, frm_data.shape[1]), -1.0, frm_data.dtype), frm_data)).astype(float)
-                mask = frm_data == -1.0
-                frm_data[mask] = np.nan
-                frm_data = pd.DataFrame(frm_data)
-                for col in frm_data.columns:
-                    frm_data = frm_data.fillna(method='ffill').fillna(method='bfill')
-            results[i] = frm_data.values
-        return results
-
-    def __get_deque_lookups(self):
-        self.deque_dict = {}
-        for animal_cnt, animal in enumerate(self.style_attr["animal names"]):
-            self.deque_dict[animal] = {}
-            self.deque_dict[animal]["deque"] = deque(
-                maxlen=self.style_attr["max lines"]
-            )
-            self.deque_dict[animal]["bp"] = self.animal_attr[animal_cnt][0]
-            if type(self.animal_attr[animal_cnt][1]) == tuple:
-                check_if_valid_rgb_str(
-                    str(self.animal_attr[animal_cnt][1]), return_cleaned_rgb_tuple=False
-                )
-                self.deque_dict[animal]["clr"] = self.animal_attr[animal_cnt][1]
-            else:
-                self.deque_dict[animal]["clr"] = self.color_dict[
-                    self.animal_attr[animal_cnt][1]
-                ]
-
     def run(self):
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, _, self.fps = self.read_video_info(video_name=self.video_name)
             self.data_df = read_df(file_path, self.file_type)
+            line_data, colors, animal_names = [], [], []
+            for k, v in self.animal_attr.items():
+                check_if_keys_exist_in_dict(data=v, key=['bp', 'color'], name=f'animal attr {k}')
+                line_data.append(self.data_df[[f'{v["bp"]}_x', f'{v["bp"]}_y']].values.astype(np.int64))
+                colors.append(v['color'])
+                if self.print_animal_names:
+                    animal_names.append(self.find_animal_name_from_body_part_name(bp_name=v["bp"], bp_dict=self.animal_bp_dict))
+            if not self.print_animal_names: animal_names = None
             if self.slicing:
-                frm_numbers = find_frame_numbers_from_time_stamp(start_time=self.slicing["start_time"], end_time=self.slicing["end_time"], fps=self.fps)
+                check_if_keys_exist_in_dict(data=self.slicing, key=['start_time', 'end_time'], name='slicing')
+                frm_numbers = find_frame_numbers_from_time_stamp(start_time=self.slicing["start_time"], end_time=self.slicing["end_time"], fps=self.fps,)
                 if len(set(frm_numbers) - set(self.data_df.index)) > 0:
                     raise FrameRangeError(msg=f'The chosen time-period ({self.slicing["start_time"]} - {self.slicing["end_time"]}) does not exist in {self.video_name}.', source=self.__class__.__name__)
-                else:
-                    self.data_df = self.data_df.loc[frm_numbers[0] : frm_numbers[-1]]
+                for i in range(len(line_data)):
+                    line_data[i] = line_data[i][frm_numbers, :]
             self.__get_styles()
 
             self.temp_folder = os.path.join(self.path_plot_dir, self.video_name, "temp")
             self.save_frame_folder_dir = os.path.join(self.path_plot_dir, self.video_name)
+
             if self.frame_setting:
                 if os.path.exists(self.save_frame_folder_dir):
                     remove_a_folder(self.save_frame_folder_dir)
-                if not os.path.exists(self.save_frame_folder_dir):
-                    os.makedirs(self.save_frame_folder_dir)
+                os.makedirs(self.save_frame_folder_dir)
+
             if self.video_setting:
                 self.video_folder = os.path.join(self.path_plot_dir, self.video_name)
                 if os.path.exists(self.temp_folder):
                     remove_a_folder(self.temp_folder)
                     remove_a_folder(self.video_folder)
                 os.makedirs(self.temp_folder)
-                self.save_video_path = os.path.join(self.path_plot_dir, self.video_name + ".mp4")
+                self.save_video_path = os.path.join(self.path_plot_dir, f"{self.video_name}.mp4")
 
-            if self.input_clf_attr:
-                clf_names, self.clf_attr = [], {}
-                self.clf_attr["attr"] = deepcopy(self.input_clf_attr)
-                for v in self.input_clf_attr.values():
-                    clf_names.append(v[0])
-                check_that_column_exist(df=self.data_df, column_name=clf_names, file_name=self.video_name)
-                self.clf_attr["data"] = self.data_df[clf_names]
-                self.clf_attr["positions"] = self.data_df[[self.animal_attr[0][0] + "_x", self.animal_attr[0][0] + "_y"]]
+            if self.clf_attr is not None:
+                self.clf_attr_appended = {}
+                check_instance(source=self.__class__.__name__, instance=self.clf_attr, accepted_types=(dict,))
+                for k, v in self.clf_attr.items():
+                    check_if_keys_exist_in_dict(data=v, key=['color', 'size'], name=f'clf_attr {k}')
+                    check_that_column_exist(df=self.data_df, column_name=k, file_name=file_path)
+                    self.clf_attr_appended[k] = self.clf_attr[k]
+                    self.clf_attr_appended[k]["clfs"] = self.data_df[k].values.astype(np.int8)
+                    self.clf_attr_appended[k]["positions"] = self.data_df[
+                        [self.animal_attr[0]['bp'] + "_x", self.animal_attr[0]['bp'] + "_y"]].values.astype(np.int64)
+                self.clf_attr = deepcopy(self.clf_attr_appended); del self.clf_attr_appended
+
+            bg_clr = self.style_attr["bg color"]
+            self.video_path = None
+            if isinstance(self.style_attr["bg color"], dict):
+                self.video_path = find_video_of_file(video_dir=self.video_dir, filename=self.video_name, raise_error=True)
+                if "frame_index" in self.style_attr["bg color"].keys():
+                    check_int(name="Static frame index", value=self.style_attr["bg color"]["frame_index"], min_value=0)
+                    frame_index = self.style_attr["bg color"]["frame_index"]
+                else:
+                    video_meta_data = get_video_meta_data(video_path=self.video_path)
+                    frame_index = video_meta_data["frame_count"] - 1
+                bg_clr = read_frm_of_video(video_path=self.video_path,
+                                                                opacity=self.style_attr["bg color"]["opacity"],
+                                                                frame_index=frame_index)
 
             if self.last_frame:
-                self.__get_deque_lookups()
-                if isinstance(self.style_attr["bg color"], dict):
-                    self.video_path = find_video_of_file(video_dir=self.video_dir, filename=self.video_name, raise_error=True)
-                    if "frame_index" in self.style_attr["bg color"].keys():
-                        check_int(name="Static frame index", value=self.style_attr["bg color"]["frame_index"], min_value=0)
-                        frame_index = self.style_attr["bg color"]["frame_index"]
-                    else:
-                        video_meta_data = get_video_meta_data(video_path=self.video_path)
-                        frame_index = video_meta_data["frame_count"] - 1
-                    self.style_attr["bg color"] = read_frm_of_video(video_path=self.video_path, opacity=self.style_attr["bg color"]["opacity"], frame_index=frame_index)
-                self.make_path_plot(data_df=self.data_df, video_info=self.video_info, style_attr=self.style_attr, print_animal_names=self.print_animal_names, deque_dict=self.deque_dict, clf_attr=self.clf_attr, save_path=os.path.join(self.path_plot_dir, self.video_name + "_final_frame.png"))
+                PlottingMixin.make_path_plot(data=line_data,
+                               colors=colors,
+                               width=self.style_attr['width'],
+                               height=self.style_attr['height'],
+                               max_lines=self.style_attr['max lines'],
+                               bg_clr=bg_clr,
+                               circle_size=self.style_attr["circle size"],
+                               font_size=self.style_attr["font size"],
+                               font_thickness=self.style_attr["font thickness"],
+                               line_width=self.style_attr["line width"],
+                               animal_names=animal_names,
+                               clf_attr=self.clf_attr,
+                               save_path=os.path.join(self.path_plot_dir, f"{self.video_name}_final_frame.png"))
 
             if self.video_setting or self.frame_setting:
-                data_arr = np.array(list(self.data_df.index)).reshape(-1, 1)
-                for animal_cnt, animal_data in self.animal_attr.items():
-                    bp_x_name = f"{animal_data[0]}_x"
-                    bp_y_name = f"{animal_data[0]}_y"
-                    check_that_column_exist(df=self.data_df, column_name=[bp_x_name, bp_y_name], file_name=self.video_name)
-                    animal_df = self.data_df[[bp_x_name, bp_y_name]]
-                    animal_vals = FeatureExtractionMixin.create_shifted_df(df=animal_df).values.astype(int)
-                    data_arr = np.hstack((data_arr, animal_vals))
-                if self.clf_attr:
-                    self.clf_attr["positions"] = deepcopy(data_arr[:, 1:3])
-                frm_range = [[x] for x in range(self.cores)]
-                data_arr = np.array_split(data_arr, self.cores)
-                data_arr = [self.__insert_group_idx_column(data=i, group=cnt) for cnt, i in enumerate(data_arr)]
-                data_arr = np.concatenate(data_arr, axis=0)
-                self.video_path = None
-                if isinstance(self.input_style_attr["bg color"], dict):
-                    self.video_path = find_video_of_file(video_dir=self.video_dir, filename=self.video_name, raise_error=True)
-                    if self.input_style_attr["bg color"]["type"] == "static":
-                        self.style_attr["bg color"] = read_frm_of_video(video_path=self.video_path, opacity=self.style_attr["bg color"]["opacity"], frame_index=self.style_attr["bg color"]["frame_index"])
-                    else:
-                        self.style_attr["bg color"] = self.input_style_attr["bg color"]
+                frm_range = np.arange(1, line_data[0].shape[0])
+                frm_range = np.array_split(frm_range, self.cores)
+                frm_range = [(cnt, x) for cnt, x in enumerate(frm_range)]
                 print(f"Creating path plots, multiprocessing (chunksize: {self.multiprocess_chunksize}, cores: {self.cores})...")
-
                 with multiprocessing.Pool(self.cores, maxtasksperchild=self.maxtasksperchild) as pool:
                     constants = functools.partial(path_plot_mp,
-                                                  data=data_arr,
+                                                  data=line_data,
+                                                  colors=colors,
                                                   video_setting=self.video_setting,
                                                   video_name=self.video_name,
                                                   frame_setting=self.frame_setting,
                                                   video_save_dir=self.temp_folder,
                                                   frame_folder_dir=self.save_frame_folder_dir,
                                                   style_attr=self.style_attr,
-                                                  print_animal_names=self.print_animal_names,
+                                                  animal_names=animal_names,
                                                   fps=self.fps,
-                                                  animal_attr=self.animal_attr,
-                                                  video_info=self.video_info,
                                                   clf_attr=self.clf_attr,
                                                   input_style_attr=self.input_style_attr,
                                                   video_path=self.video_path)
                     for cnt, result in enumerate(pool.imap(constants, frm_range, chunksize=self.multiprocess_chunksize)):
-                        print(f'Path batch {result+1}/{self.cores} complete...')
+                        print(f"Path batch {result+1}/{self.cores} complete...")
                     pool.terminate()
                     pool.join()
 
                 if self.video_setting:
                     print(f"Joining {self.video_name} multiprocessed video...")
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
-
                 video_timer.stop_timer()
                 print(f"Path plot video {self.video_name} complete (elapsed time: {video_timer.elapsed_time_str}s) ...")
 
         self.timer.stop_timer()
         stdout_success(msg=f"Path plot visualizations for {len(self.files_found)} videos created in {self.path_plot_dir} directory", elapsed_time=self.timer.elapsed_time_str, source=self.__class__.__name__)
 
 
-# style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 2, 'font thickness': 2, 'circle size': 5, 'bg color': {'type': 'moving', 'opacity': 100, 'frame_index': 100}, 'max lines': 'entire video'}
-# animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
-# clf_attr = {0: ['Nose to Nose', 'Black', 'Size: 30']}
-# # #
-# clf_attr = None
-# style_attr = None
+# animal_attr = {0: {'bp': 'Ear_right_1', 'color': (255, 0, 0)}, 1: {'bp': 'Ear_right_2', 'color': (0, 0, 255)}}  #['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
+# style_attr = {'width': 'As input',
+#               'height': 'As input',
+#               'line width': 2,
+#               'font size': 0.9,
+#               'font thickness': 2,
+#               'circle size': 5,
+#               'bg color': {'type': 'moving', 'opacity': 50, 'frame_index': 200}, #{'type': 'static', 'opacity': 100, 'frame_index': 200}
+#               'max lines': 'entire video'}
+# clf_attr = {'Nose to Nose': {'color': (155, 1, 10), 'size': 30}, 'Nose to Tailbase': {'color': (155, 90, 10), 'size': 30}}
+# #clf_attr=None
 
 # path_plotter = PathPlotterMulticore(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini',
 #                                     frame_setting=False,
 #                                     video_setting=True,
 #                                     last_frame=True,
-#                                     input_clf_attr=clf_attr,
+#                                     clf_attr=clf_attr,
 #                                     input_style_attr=style_attr,
 #                                     animal_attr=animal_attr,
 #                                     files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/csv/machine_results/Trial    10.csv'],
 #                                     cores=-1,
-#                                     slicing = None, # {'start_time': '00:00:00', 'end_time': '00:00:05'}, # , #None,
+#                                     slicing = {'start_time': '00:00:00', 'end_time': '00:00:05'}, # {'start_time': '00:00:00', 'end_time': '00:00:05'}, # , #None,
 #                                     print_animal_names=False)
 # path_plotter.run()
 
 
-
 # style_attr = {'width': 'As input',
 #               'height': 'As input',
 #               'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': {'type': 'static', 'opacity': 100, 'frame_index': 100}, 'max lines': 'entire video'}
 # animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
 # # clf_attr = {0: ['Attack', 'Black', 'Size: 30']}
 # # # #
 # clf_attr = None
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/data_plotter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 __author__ = "Simon Nilsson"
 
 import os
-from typing import Dict, List
+from typing import Any, Dict, List, Optional, Union
 
 import cv2
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 
 from simba.data_processors.movement_calculator import MovementCalculator
 from simba.mixins.config_reader import ConfigReader
+from simba.utils.checks import (
+    check_all_file_names_are_represented_in_video_log,
+    check_if_keys_exist_in_dict, check_valid_lst)
 from simba.utils.enums import Formats
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.lookups import get_color_dict
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.utils.read_write import get_fn_ext
 
+BG_COLOR = "bg_color"
+HEADER_COLOR = "header_color"
+FONT_THICKNESS = "font_thickness"
+SIZE = "size"
+DATA_ACCURACY = "data_accuracy"
+STYLE_KEYS = [BG_COLOR, HEADER_COLOR, FONT_THICKNESS, SIZE, DATA_ACCURACY]
+
 
 class DataPlotter(ConfigReader):
     """
     Tabular data visualization of animal movement and distances in the current frame and their aggregate
     statistics.
 
     :parameter str config_path: path to SimBA project config file in Configparser format
@@ -33,26 +43,38 @@
 
     :examples:
     >>> _ = DataPlotter(config_path='MyConfigPath').run()
     """
 
     def __init__(
         self,
-        config_path: str,
-        style_attr: Dict,
+        config_path: Union[str, os.PathLike],
+        style_attr: Dict[str, Any],
         body_part_attr: List[List[str]],
         data_paths: List[str],
-        video_setting: bool,
-        frame_setting: bool,
+        video_setting: Optional[bool] = True,
+        frame_setting: Optional[bool] = True,
     ):
-        super().__init__(config_path=config_path)
+
         if (not video_setting) and (not frame_setting):
             raise NoSpecifiedOutputError(
                 msg="SIMBA ERROR: Please choose to create video and/or frames data plots. SimBA found that you ticked neither video and/or frames"
             )
+        check_valid_lst(
+            data=data_paths, source=self.__class__.__name__, valid_dtypes=(str,)
+        )
+        check_valid_lst(
+            data=body_part_attr, source=self.__class__.__name__, valid_dtypes=(list,)
+        )
+        for i in body_part_attr:
+            check_valid_lst(
+                data=i, source=self.__class__.__name__, valid_dtypes=(str,), exact_len=2
+            )
+        check_if_keys_exist_in_dict(data=style_attr, key=STYLE_KEYS)
+        ConfigReader.__init__(self, config_path=config_path)
         self.video_setting, self.frame_setting = video_setting, frame_setting
         self.files_found, self.style_attr, self.body_part_attr = (
             data_paths,
             style_attr,
             body_part_attr,
         )
         if not os.path.exists(self.data_table_path):
@@ -171,24 +193,27 @@
                     cv2.FONT_HERSHEY_TRIPLEX,
                     0.5,
                     clr,
                     1,
                 )
             return img
 
+        check_all_file_names_are_represented_in_video_log(
+            video_info_df=self.video_info_df, data_paths=self.files_found
+        )
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(file_path)
             self.video_data = pd.DataFrame(self.movement[video_name])
             self.__compute_spacings()
             _, _, self.fps = self.read_video_info(video_name=video_name)
             if self.video_setting:
                 self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
                 self.video_save_path = os.path.join(
-                    self.data_table_path, video_name + ".mp4"
+                    self.data_table_path, f"{video_name}.mp4"
                 )
                 self.writer = cv2.VideoWriter(
                     self.video_save_path, self.fourcc, self.fps, self.style_attr["size"]
                 )
             if self.frame_setting:
                 self.frame_save_path = os.path.join(self.data_table_path, video_name)
                 if not os.path.exists(self.frame_save_path):
@@ -244,19 +269,19 @@
         stdout_success(
             msg=f"All data table videos created inside {self.data_table_path}",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
 # style_attr = {'bg_color': 'White', 'header_color': 'Black', 'font_thickness': 1, 'size': (640, 480), 'data_accuracy': 2}
-# body_part_attr = [['Ear_left_1', 'Grey'], ['Ear_right_2', 'Red']]
-# data_paths = ['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv']
+# body_part_attr = [['Ear_left_1', 'Green'], ['Ear_right_2', 'Red']]
+# data_paths = ['/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/csv/machine_results/Trial    10.csv']
 #
 #
-# test = DataPlotter(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+# test = DataPlotter(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini',
 #                    style_attr=style_attr,
 #                    body_part_attr=body_part_attr,
 #                    data_paths=data_paths,
 #                    video_setting=True,
 #                    frame_setting=False)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/distance_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,18 @@
                 if self.style_attr["y_max"] == -1:
                     self.style_attr["y_max"] = max([np.max(x) for x in distances])
                 distances = np.stack(distances, axis=1)
                 frm_range = np.arange(0, distances.shape[0])
                 frm_range = np.array_split(frm_range, self.core_cnt)
 
                 distances = np.array_split(distances, self.core_cnt)
-                distances = [self.__insert_group_idx_column(data=i, group=cnt) for cnt, i in enumerate(distances)]
+                distances = [
+                    self.__insert_group_idx_column(data=i, group=cnt)
+                    for cnt, i in enumerate(distances)
+                ]
                 distances = np.concatenate(distances, axis=0)
                 print(
                     f"Creating distance plots, multiprocessing, follow progress in terminal (chunksize: {self.multiprocess_chunksize}, cores: {self.core_cnt})"
                 )
                 with multiprocessing.Pool(
                     self.core_cnt, maxtasksperchild=self.maxtasksperchild
                 ) as pool:
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,252 +1,287 @@
 __author__ = "Simon Nilsson"
 
+import functools
+import multiprocessing
 import os
-from typing import Dict, List, Optional, Union
+import platform
+import shutil
+from typing import Any, Dict, List, Optional, Union
 
 import cv2
 import numpy as np
+import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.checks import (
-    check_all_file_names_are_represented_in_video_log,
-    check_file_exist_and_readable, check_instance, check_valid_lst)
-from simba.utils.errors import (CountError, InvalidInputError,
-                                NoSpecifiedOutputError)
-from simba.utils.lookups import get_color_dict
+    check_all_file_names_are_represented_in_video_log, check_int, check_str,
+    check_that_column_exist, check_valid_lst)
+from simba.utils.enums import Formats
+from simba.utils.errors import ColumnNotFoundError, NoSpecifiedOutputError
 from simba.utils.printing import SimbaTimer, stdout_success
-from simba.utils.read_write import get_fn_ext, read_df
+from simba.utils.read_write import (concatenate_videos_in_folder,
+                                    find_core_cnt, get_fn_ext, read_df)
 
 
-class DistancePlotterSingleCore(ConfigReader):
+def probability_plot_mp(
+    data: list,
+    probability_lst: list,
+    clf_name: str,
+    video_setting: bool,
+    frame_setting: bool,
+    video_dir: str,
+    frame_dir: str,
+    highest_p: float,
+    fps: int,
+    style_attr: dict,
+    video_name: str,
+):
+    group, data = data[0], data[1:]
+    start_frm, end_frm, current_frm = data[0], data[-1], data[0]
+
+    if video_setting:
+        fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
+        video_save_path = os.path.join(video_dir, f"{group}.mp4")
+        video_writer = cv2.VideoWriter(
+            video_save_path, fourcc, fps, (style_attr["width"], style_attr["height"])
+        )
+
+    while current_frm < end_frm:
+        current_lst = [np.array(probability_lst[0 : current_frm + 1])]
+        current_frm += 1
+        img = PlottingMixin.make_line_plot_plotly(
+            data=current_lst,
+            colors=[style_attr["color"]],
+            width=style_attr["width"],
+            height=style_attr["height"],
+            line_width=style_attr["line width"],
+            font_size=style_attr["font size"],
+            y_lbl=f"{clf_name} probability",
+            title=clf_name,
+            y_max=highest_p,
+        )
+
+        if video_setting:
+            video_writer.write(img[:, :, :3])
+        if frame_setting:
+            frame_save_name = os.path.join(frame_dir, f"{current_frm}.png")
+            cv2.imwrite(frame_save_name, img)
+        current_frm += 1
+        print(
+            f"Probability frame created: {current_frm + 1}, Video: {video_name}, Processing core: {group}"
+        )
+    return group
+
+
+class TresholdPlotCreatorMultiprocess(ConfigReader, PlottingMixin):
     """
-    Class for visualizing the distance between two pose-estimated body-parts (e.g., two animals) through line
-    charts. Results are saved as individual line charts, and/or videos of line charts.
+    Class for line chart visualizations displaying the classification probabilities of a single classifier.
+    Uses multiprocessing.
+
+    :param str config_path: path to SimBA project config file in Configparser format
+    :param str clf_name: Name of the classifier to create visualizations for
+    :param bool frame_setting: When True, SimBA creates indidvidual frames in png format
+    :param bool video_setting: When True, SimBA creates compressed video in mp4 format
+    :param bool last_image: When True, creates image .png representing last frame of the video.
+    :param dict style_attr: User-defined style attributes of the visualization (line size, color etc).
+    :param List[str] files_found: Files to create threshold plots for.
+    :param int cores: Number of cores to use.
 
     .. note::
-       For better runtime, use :meth:`simba.plotting.distance_plotter_mp.DistancePlotterMultiCore`.
-       `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
+       `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
-    .. image:: _static/img/distance_plot.png
+    .. image:: _static/img/prob_plot.png
        :width: 300
        :align: center
 
-    :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter bool frame_setting: If True, creates individual frames.
-    :parameter bool video_setting: If True, creates videos
-
-    :examples:
-
-    >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'opacity': 0.5}
-    >>> line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
-    >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', files_found=['test/two_c57s/project_folder/csv/outlier_corrected_movement_location/Video_1.csv'], frame_setting=False, video_setting=True, final_img=True)
-    >>> distance_plotter.run()
+    :example:
+    >>> plot_creator = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', frame_setting=True, video_setting=True, clf_name='Attack', style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'magneta', 'circle size': 20}, cores=5)
+    >>> plot_creator.run()
     """
 
     def __init__(
         self,
         config_path: Union[str, os.PathLike],
-        data_paths: List[Union[str, os.PathLike]],
-        style_attr: Dict[str, int],
-        line_attr: List[List[str]],
+        files_found: List[Union[str, os.PathLike]],
+        style_attr: Dict[str, Any],
+        clf_name: str,
         frame_setting: Optional[bool] = False,
         video_setting: Optional[bool] = False,
-        final_img: Optional[bool] = False,
+        last_frame: Optional[bool] = True,
+        cores: Optional[int] = -1,
     ):
 
-        if (not frame_setting) and (not video_setting) and (not final_img):
+        # if platform.system() == "Darwin":
+        #     multiprocessing.set_start_method("spawn", force=True)
+        if (not video_setting) and (not frame_setting) and (not frame_setting):
             raise NoSpecifiedOutputError(
-                msg="Please choice to create frames and/or video distance plots",
-                source=self.__class__.__name__,
-            )
-        check_instance(
-            source=f"{self.__class__.__name__} line_attr",
-            instance=line_attr,
-            accepted_types=(list,),
-        )
-        for cnt, i in enumerate(line_attr):
-            check_valid_lst(
-                source=f"{self.__class__.__name__} line_attr {cnt}",
-                data=i,
-                valid_dtypes=(str,),
-                exact_len=3,
+                msg="SIMBA ERROR: Please choose to create video and/or frames data plots. SimBA found that you ticked neither video and/or frames"
             )
-        check_valid_lst(data=data_paths, valid_dtypes=(str,), min_len=1)
-        _ = [check_file_exist_and_readable(i) for i in data_paths]
+        check_valid_lst(
+            data=files_found, source=self.__class__.__name__, valid_dtypes=(str,)
+        )
+        check_int(
+            name=f"{self.__class__.__name__} core_cnt",
+            value=cores,
+            min_value=-1,
+            max_value=find_core_cnt()[0],
+        )
+        if cores == -1:
+            cores = find_core_cnt()[0]
         ConfigReader.__init__(self, config_path=config_path)
+        PlottingMixin.__init__(self)
+        check_str(
+            name=f"{self.__class__.__name__} clf_name",
+            value=clf_name,
+            options=(self.clf_names),
+        )
         (
-            self.video_setting,
             self.frame_setting,
-            self.data_paths,
+            self.video_setting,
+            self.cores,
             self.style_attr,
-            self.line_attr,
-            self.final_img,
-        ) = (video_setting, frame_setting, data_paths, style_attr, line_attr, final_img)
-        self.color_names = get_color_dict()
+            self.last_frame,
+        ) = (frame_setting, video_setting, cores, style_attr, last_frame)
+        self.clf_name, self.files_found = clf_name, files_found
+        self.probability_col = f"Probability_{self.clf_name}"
+        self.fontsize = self.style_attr["font size"]
+        self.out_width, self.out_height = (
+            self.style_attr["width"],
+            self.style_attr["height"],
+        )
+        self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
+        if not os.path.exists(self.probability_plot_dir):
+            os.makedirs(self.probability_plot_dir)
+        print(f"Processing {len(self.files_found)} video(s)...")
 
     def run(self):
-        print(f"Processing {len(self.data_paths)} videos...")
         check_all_file_names_are_represented_in_video_log(
-            video_info_df=self.video_info_df, data_paths=self.data_paths
+            video_info_df=self.video_info_df, data_paths=self.files_found
         )
-        for file_cnt, file_path in enumerate(self.data_paths):
+        for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer(start=True)
+            _, self.video_name, _ = get_fn_ext(file_path)
+            video_info, self.px_per_mm, self.fps = self.read_video_info(
+                video_name=self.video_name
+            )
             data_df = read_df(file_path, self.file_type)
-            _, video_name, _ = get_fn_ext(file_path)
-            self.video_info, px_per_mm, fps = self.read_video_info(
-                video_name=video_name
-            )
-            self.save_video_folder = os.path.join(self.line_plot_dir, video_name)
-            self.save_frame_folder_dir = os.path.join(self.line_plot_dir, video_name)
-
-            try:
-                data_df.columns = self.bp_headers
-            except ValueError:
-                raise CountError(
-                    msg=f"SimBA expects {self.bp_headers} columns but found {len(data_df)} columns in {file_path}",
-                    source=self.__class__.__name__,
-                )
-            distances = []
-            colors = []
-            for cnt, i in enumerate(self.line_attr):
-                if i[2] not in list(self.color_names.keys()):
-                    raise InvalidInputError(
-                        msg=f"{i[2]} is not a valid color. Options: {list(self.color_names.keys())}.",
-                        source=self.__class__.__name__,
-                    )
-                colors.append(i[2])
-                bp_1, bp_2 = [f"{i[0]}_x", f"{i[0]}_y"], [f"{i[1]}_x", f"{i[1]}_y"]
-                if len(list(set(bp_1) - set(data_df.columns))) > 0:
-                    raise InvalidInputError(
-                        msg=f"Could not find fields {bp_1} in {file_path}",
-                        source=self.__class__.__name__,
-                    )
-                if len(list(set(bp_2) - set(data_df.columns))) > 0:
-                    raise InvalidInputError(
-                        msg=f"Could not find fields {bp_2} in {file_path}",
-                        source=self.__class__.__name__,
-                    )
-                distances.append(
-                    FeatureExtractionMixin.framewise_euclidean_distance(
-                        location_1=data_df[bp_1].values,
-                        location_2=data_df[bp_2].values,
-                        px_per_mm=px_per_mm,
-                        centimeter=True,
-                    )
-                )
+            check_that_column_exist(
+                df=data_df,
+                column_name=[self.clf_name, self.probability_col],
+                file_name=file_path,
+            )
+            self.save_frame_folder_dir = os.path.join(
+                self.probability_plot_dir, self.video_name + f"_{self.clf_name}"
+            )
+            self.video_folder = os.path.join(
+                self.probability_plot_dir, self.video_name + f"_{self.clf_name}"
+            )
+            self.temp_folder = os.path.join(
+                self.probability_plot_dir, f"{self.video_name}_{self.clf_name}", "temp"
+            )
             if self.frame_setting:
                 if os.path.exists(self.save_frame_folder_dir):
-                    self.remove_a_folder(self.save_frame_folder_dir)
+                    shutil.rmtree(self.save_frame_folder_dir)
                 os.makedirs(self.save_frame_folder_dir)
             if self.video_setting:
-                save_video_path = os.path.join(self.line_plot_dir, f"{video_name}.avi")
-                fourcc = cv2.VideoWriter_fourcc(*"DIVX")
-                video_writer = cv2.VideoWriter(
-                    save_video_path,
-                    fourcc,
-                    fps,
-                    (self.style_attr["width"], self.style_attr["height"]),
+                if os.path.exists(self.temp_folder):
+                    shutil.rmtree(self.temp_folder)
+                    shutil.rmtree(self.video_folder)
+                os.makedirs(self.temp_folder)
+                self.save_video_path = os.path.join(
+                    self.probability_plot_dir, f"{self.video_name}_{self.clf_name}.mp4"
                 )
 
-            if self.final_img:
-                _ = PlottingMixin.make_line_plot(
-                    data=distances,
-                    colors=colors,
-                    width=self.style_attr["width"],
-                    height=self.style_attr["height"],
-                    line_width=self.style_attr["line width"],
-                    font_size=self.style_attr["font size"],
-                    title="Animal distances",
-                    y_lbl="distance (cm)",
-                    x_lbl="time (s)",
-                    x_lbl_divisor=fps,
-                    y_max=self.style_attr["y_max"],
-                    line_opacity=self.style_attr["opacity"],
+            probability_lst = list(data_df[self.probability_col])
+            # probability_lst = list(np.random.random(size=(len(data_df))))
+
+            if self.last_frame:
+                _ = self.make_probability_plot(
+                    data=pd.Series(probability_lst),
+                    style_attr=self.style_attr,
+                    clf_name=self.clf_name,
+                    fps=self.fps,
                     save_path=os.path.join(
-                        self.line_plot_dir, f"{video_name}_final_distances.png"
+                        self.probability_plot_dir,
+                        f"{self.video_name}_{self.clf_name}_final_image.png",
                     ),
                 )
 
             if self.video_setting or self.frame_setting:
-                if self.style_attr["y_max"] == -1:
-                    self.style_attr["y_max"] = max([np.max(x) for x in distances])
-                for frm_cnt in range(distances[0].shape[0]):
-                    line_data = [x[:frm_cnt] for x in distances]
-                    img = PlottingMixin.make_line_plot_plotly(
-                        data=line_data,
-                        colors=colors,
-                        width=self.style_attr["width"],
-                        height=self.style_attr["height"],
-                        line_width=self.style_attr["line width"],
-                        font_size=self.style_attr["font size"],
-                        title="Animal distances",
-                        y_lbl="distance (cm)",
-                        x_lbl="frame count",
-                        x_lbl_divisor=fps,
-                        y_max=self.style_attr["y_max"],
-                        line_opacity=self.style_attr["opacity"],
-                        save_path=None,
-                    ).astype(np.uint8)
-                    if self.video_setting:
-                        video_writer.write(img[:, :, :3])
-                    if self.frame_setting:
-                        frm_name = os.path.join(
-                            self.save_frame_folder_dir, f"{frm_cnt}.png"
+                if self.style_attr["y_max"] == "auto":
+                    highest_p = data_df[self.probability_col].max()
+                else:
+                    highest_p = float(self.style_attr["y_max"])
+                data_split = np.array_split(list(data_df.index), self.cores)
+                frm_per_core = len(data_split[0])
+                for group_cnt, rng in enumerate(data_split):
+                    data_split[group_cnt] = np.insert(rng, 0, group_cnt)
+                print(
+                    f"Creating probability images, multiprocessing (determined chunksize: {self.multiprocess_chunksize}, cores: {self.cores})..."
+                )
+                with multiprocessing.Pool(
+                    self.cores, maxtasksperchild=self.maxtasksperchild
+                ) as pool:
+                    constants = functools.partial(
+                        probability_plot_mp,
+                        clf_name=self.clf_name,
+                        probability_lst=probability_lst,
+                        highest_p=highest_p,
+                        video_setting=self.video_setting,
+                        frame_setting=self.frame_setting,
+                        fps=self.fps,
+                        video_dir=self.temp_folder,
+                        frame_dir=self.save_frame_folder_dir,
+                        style_attr=self.style_attr,
+                        video_name=self.video_name,
+                    )
+                    for cnt, result in enumerate(
+                        pool.imap(
+                            constants, data_split, chunksize=self.multiprocess_chunksize
+                        )
+                    ):
+                        print(
+                            f"Image {int(frm_per_core * (result + 1))}/{len(data_df)}, Video {file_cnt + 1}/{len(self.files_found)}..."
                         )
-                        cv2.imwrite(frm_name, np.uint8(img))
-                    print(f"Distance frame created: {frm_cnt}, Video: {video_name} ...")
+
+                pool.join()
+                pool.terminate()
                 if self.video_setting:
-                    video_writer.release()
+                    print(f"Joining {self.video_name} multiprocessed video...")
+                    concatenate_videos_in_folder(
+                        in_folder=self.temp_folder, save_path=self.save_video_path
+                    )
+
                 video_timer.stop_timer()
-                stdout_success(
-                    msg=f"Distance visualizations created for {video_name} saved at {self.line_plot_dir}",
-                    elapsed_time=video_timer.elapsed_time_str,
+                print(
+                    f"Probability video {self.video_name} complete (elapsed time: {video_timer.elapsed_time_str}s) ..."
                 )
+
         self.timer.stop_timer()
         stdout_success(
-            msg=f"Distance visualizations complete for {len(self.data_paths)} video(s)",
+            msg=f"Probability visualizations for {str(len(self.files_found))} videos created in project_folder/frames/output/gantt_plots directory",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
-# style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 12, 'y_max': -1, 'opacity': 0.5}
-# line_attr = [['Center_1', 'Center_2', 'Green'], ['Ear_left_2', 'Ear_right_2', 'Red']]
-# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                  frame_setting=True,
-#                                  video_setting=True,
-#                                  style_attr=style_attr,
-#                                  final_img=True,
-#                                  data_paths=['/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location/Together_1.csv'],
-#                                  line_attr=line_attr)
+# test = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini',
+#                                         frame_setting=False,
+#                                         video_setting=True,
+#                                         last_frame=True,
+#                                         clf_name='Nose to Nose',
+#                                         cores=-1,
+#                                         files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/csv/machine_results/Trial    10.csv'],
+#                                         style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'Red', 'circle size': 20, 'y_max': 'auto'})
+# #test = TresholdPlotCreatorSingleProcess(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', frame_setting=False, video_setting=True, clf_name='Attack')
 # test.run()
 
 
-#
-# style_attr = {'width': 640,
-#               'height': 480,
-#               'line width': 6,
-#               'font size': 8,
-#               'y_max': 'auto',
-#               'opacity': 0.9}
-# line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
-#
-# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                  frame_setting=False,
-#                                  video_setting=True,
-#                                  style_attr=style_attr,
-#                                  final_img=True,
-#                                  files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
-#                                  line_attr=line_attr)
-# test.create_distance_plot()
-
-# style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8}
-# line_attr = {0: ['Termite_1_Head_1', 'Termite_1_Thorax_1', 'Dark-red']}
-
-# test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini',
-#                                  frame_setting=False,
-#                        video_setting=True,
-#                        style_attr=style_attr,
-#                        files_found=['/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/csv/outlier_corrected_movement_location/termites_1.csv'],
-#                        line_attr=line_attr)
-# test.create_distance_plot()
+# test = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                         frame_setting=False,
+#                                         video_setting=True,
+#                                         last_frame=True,
+#                                         clf_name='Attack',
+#                                         cores=5,
+#                                         files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
+#                                         style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 3, 'color': 'blue', 'circle size': 20, 'y_max': 'auto'})
+# test.create_plots()
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.90.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.90.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.90.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.90.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.90.4/simba/model/train_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,15 @@
             source=self.__class__.__name__,
         )
         stdout_success(
             msg=f"Evaluation files are in models/generated_models/model_evaluations folders",
             source=self.__class__.__name__,
         )
 
+
 #
 # test = TrainRandomForestClassifier(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini')
 # test.run()
 # test.save()
 
 
 # test = TrainRandomForestClassifier(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/mouse_open_field/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.90.4/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.90.4/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.90.4/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.90.4/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.90.4/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.90.4/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.90.4/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.90.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.90.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.90.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/video_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -3916,3566 +3916,3567 @@
 0000f4b0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
 0000f4c0: 6b65 5d2c 0a20 2020 2020 2020 2067 7075  ke],.        gpu
 0000f4d0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
 0000f4e0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
 0000f4f0: 2020 6666 6d70 6567 3a20 4f70 7469 6f6e    ffmpeg: Option
 0000f500: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
 0000f510: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0000f520: 0a20 2020 2020 2020 2069 6620 6770 7520  .        if gpu 
-0000f530: 616e 6420 6e6f 7420 6368 6563 6b5f 6e76  and not check_nv
-0000f540: 6964 6561 5f67 7075 5f61 7661 696c 6162  idea_gpu_availab
-0000f550: 6c65 2829 3a0a 2020 2020 2020 2020 2020  le():.          
-0000f560: 2020 7261 6973 6520 4646 4d50 4547 436f    raise FFMPEGCo
-0000f570: 6465 6347 5055 4572 726f 7228 0a20 2020  decGPUError(.   
-0000f580: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-0000f590: 3d22 4e6f 2047 5055 2066 6f75 6e64 2028  ="No GPU found (
-0000f5a0: 6173 2065 7661 6c75 6174 6564 2062 7920  as evaluated by 
-0000f5b0: 6e76 6964 6561 2d73 6d69 2072 6574 7572  nvidea-smi retur
-0000f5c0: 6e69 6e67 204e 6f6e 6529 222c 0a20 2020  ning None)",.   
-0000f5d0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-0000f5e0: 7263 653d 7365 6c66 2e5f 5f63 6c61 7373  rce=self.__class
-0000f5f0: 5f5f 2e5f 5f6e 616d 655f 5f2c 0a20 2020  __.__name__,.   
-0000f600: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000f610: 2020 2069 6620 6666 6d70 6567 2061 6e64     if ffmpeg and
-0000f620: 206e 6f74 2063 6865 636b 5f66 666d 7065   not check_ffmpe
-0000f630: 675f 6176 6169 6c61 626c 6528 293a 0a20  g_available():. 
-0000f640: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000f650: 2046 464d 5045 474e 6f74 466f 756e 6445   FFMPEGNotFoundE
-0000f660: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000f670: 2020 2020 2020 6d73 673d 2746 464d 5045        msg='FFMPE
-0000f680: 4720 6e6f 7420 666f 756e 6420 6f6e 2074  G not found on t
-0000f690: 6865 2063 6f6d 7075 7465 7220 2861 7320  he computer (as 
-0000f6a0: 6576 616c 7561 7465 6420 6279 2022 6666  evaluated by "ff
-0000f6b0: 6d70 6567 2220 7265 7475 726e 696e 6720  mpeg" returning 
-0000f6c0: 4e6f 6e65 2927 2c0a 2020 2020 2020 2020  None)',.        
-0000f6d0: 2020 2020 2020 2020 736f 7572 6365 3d73          source=s
-0000f6e0: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
-0000f6f0: 6e61 6d65 5f5f 2c0a 2020 2020 2020 2020  name__,.        
-0000f700: 2020 2020 290a 2020 2020 2020 2020 5f2c      ).        _,
-0000f710: 2073 656c 662e 6370 755f 636e 7420 3d20   self.cpu_cnt = 
-0000f720: 6669 6e64 5f63 6f72 655f 636e 7428 290a  find_core_cnt().
-0000f730: 2020 2020 2020 2020 7365 6c66 2e67 7075          self.gpu
-0000f740: 2c20 7365 6c66 2e66 666d 7065 6720 3d20  , self.ffmpeg = 
-0000f750: 6770 752c 2066 666d 7065 670a 2020 2020  gpu, ffmpeg.    
-0000f760: 2020 2020 7365 6c66 2e73 6176 655f 6469      self.save_di
-0000f770: 7220 3d20 6f75 7470 7574 5f64 6972 0a20  r = output_dir. 
-0000f780: 2020 2020 2020 2073 656c 662e 6461 7465         self.date
-0000f790: 7469 6d65 203d 2064 6174 6574 696d 652e  time = datetime.
-0000f7a0: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
-0000f7b0: 2559 256d 2564 2548 254d 2553 2229 0a20  %Y%m%d%H%M%S"). 
-0000f7c0: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-0000f7d0: 682e 6973 6669 6c65 2869 6e70 7574 5f70  h.isfile(input_p
-0000f7e0: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
-0000f7f0: 2020 7365 6c66 2e76 6964 656f 5f70 6174    self.video_pat
-0000f800: 6873 203d 205b 696e 7075 745f 7061 7468  hs = [input_path
-0000f810: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0000f820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f830: 2e76 6964 656f 5f70 6174 6873 203d 2066  .video_paths = f
-0000f840: 696e 645f 616c 6c5f 7669 6465 6f73 5f69  ind_all_videos_i
-0000f850: 6e5f 6469 7265 6374 6f72 7928 0a20 2020  n_directory(.   
-0000f860: 2020 2020 2020 2020 2020 2020 2064 6972               dir
-0000f870: 6563 746f 7279 3d69 6e70 7574 5f70 6174  ectory=input_pat
-0000f880: 682c 2061 735f 6469 6374 3d54 7275 650a  h, as_dict=True.
-0000f890: 2020 2020 2020 2020 2020 2020 292e 7661              ).va
-0000f8a0: 6c75 6573 2829 0a20 2020 2020 2020 2020  lues().         
-0000f8b0: 2020 2063 6865 636b 5f69 665f 6669 6c65     check_if_file
-0000f8c0: 7061 7468 5f6c 6973 745f 6973 5f65 6d70  path_list_is_emp
-0000f8d0: 7479 280a 2020 2020 2020 2020 2020 2020  ty(.            
-0000f8e0: 2020 2020 6669 6c65 7061 7468 733d 7365      filepaths=se
-0000f8f0: 6c66 2e76 6964 656f 5f70 6174 6873 2c0a  lf.video_paths,.
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 6572 726f 725f 6d73 673d 6622 4e6f 2076  error_msg=f"No v
-0000f920: 6964 656f 7320 666f 756e 6420 696e 207b  ideos found in {
-0000f930: 696e 7075 745f 7061 7468 7d20 6469 7265  input_path} dire
-0000f940: 6374 6f72 7922 2c0a 2020 2020 2020 2020  ctory",.        
-0000f950: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
-0000f960: 5f69 6e73 6572 745f 696d 6728 7365 6c66  _insert_img(self
-0000f970: 2c20 696d 673a 206e 702e 6172 7261 7929  , img: np.array)
-0000f980: 3a0a 2020 2020 2020 2020 6375 7272 656e  :.        curren
-0000f990: 745f 6672 6d5f 7069 6c20 3d20 496d 6167  t_frm_pil = Imag
-0000f9a0: 652e 6672 6f6d 6172 7261 7928 696d 6729  e.fromarray(img)
-0000f9b0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-0000f9c0: 5f66 726d 5f70 696c 2e74 6875 6d62 6e61  _frm_pil.thumbna
-0000f9d0: 696c 284d 4158 5f46 524d 5f53 495a 452c  il(MAX_FRM_SIZE,
-0000f9e0: 2049 6d61 6765 2e41 4e54 4941 4c49 4153   Image.ANTIALIAS
-0000f9f0: 290a 2020 2020 2020 2020 6375 7272 656e  ).        curren
-0000fa00: 745f 6672 6d5f 7069 6c20 3d20 496d 6167  t_frm_pil = Imag
-0000fa10: 6554 6b2e 5068 6f74 6f49 6d61 6765 280a  eTk.PhotoImage(.
-0000fa20: 2020 2020 2020 2020 2020 2020 6d61 7374              mast
-0000fa30: 6572 3d73 656c 662e 6d61 696e 5f66 726d  er=self.main_frm
-0000fa40: 2c20 696d 6167 653d 6375 7272 656e 745f  , image=current_
-0000fa50: 6672 6d5f 7069 6c0a 2020 2020 2020 2020  frm_pil.        
-0000fa60: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0000fa70: 6964 656f 5f66 7261 6d65 203d 204c 6162  ideo_frame = Lab
-0000fa80: 656c 2873 656c 662e 6d61 696e 5f66 726d  el(self.main_frm
-0000fa90: 2c20 696d 6167 653d 6375 7272 656e 745f  , image=current_
-0000faa0: 6672 6d5f 7069 6c29 0a20 2020 2020 2020  frm_pil).       
-0000fab0: 2073 656c 662e 7669 6465 6f5f 6672 616d   self.video_fram
-0000fac0: 652e 696d 6167 6520 3d20 6375 7272 656e  e.image = curren
-0000fad0: 745f 6672 6d5f 7069 6c0a 2020 2020 2020  t_frm_pil.      
-0000fae0: 2020 7365 6c66 2e76 6964 656f 5f66 7261    self.video_fra
-0000faf0: 6d65 2e67 7269 6428 726f 773d 302c 2063  me.grid(row=0, c
-0000fb00: 6f6c 756d 6e3d 3029 0a0a 2020 2020 6465  olumn=0)..    de
-0000fb10: 6620 5f5f 726f 7461 7465 2873 656c 662c  f __rotate(self,
-0000fb20: 2076 616c 7565 3a20 696e 742c 2069 6d67   value: int, img
-0000fb30: 3a20 6e70 2e61 7272 6179 293a 0a20 2020  : np.array):.   
-0000fb40: 2020 2020 2073 656c 662e 6469 665f 616e       self.dif_an
-0000fb50: 676c 6520 2b3d 2076 616c 7565 0a20 2020  gle += value.   
-0000fb60: 2020 2020 2072 6f74 6174 696f 6e5f 6d61       rotation_ma
-0000fb70: 7472 6978 203d 2063 7632 2e67 6574 526f  trix = cv2.getRo
-0000fb80: 7461 7469 6f6e 4d61 7472 6978 3244 280a  tationMatrix2D(.
-0000fb90: 2020 2020 2020 2020 2020 2020 2873 656c              (sel
-0000fba0: 662e 7669 6465 6f5f 6d65 7461 5f64 6174  f.video_meta_dat
-0000fbb0: 615b 2277 6964 7468 225d 202f 2032 2c20  a["width"] / 2, 
-0000fbc0: 7365 6c66 2e76 6964 656f 5f6d 6574 615f  self.video_meta_
-0000fbd0: 6461 7461 5b22 6865 6967 6874 225d 202f  data["height"] /
-0000fbe0: 2032 292c 0a20 2020 2020 2020 2020 2020   2),.           
-0000fbf0: 2073 656c 662e 6469 665f 616e 676c 652c   self.dif_angle,
-0000fc00: 0a20 2020 2020 2020 2020 2020 2031 2c0a  .            1,.
-0000fc10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000fc20: 2020 696d 6720 3d20 6376 322e 7761 7270    img = cv2.warp
-0000fc30: 4166 6669 6e65 280a 2020 2020 2020 2020  Affine(.        
-0000fc40: 2020 2020 696d 672c 0a20 2020 2020 2020      img,.       
-0000fc50: 2020 2020 2072 6f74 6174 696f 6e5f 6d61       rotation_ma
-0000fc60: 7472 6978 2c0a 2020 2020 2020 2020 2020  trix,.          
-0000fc70: 2020 2873 656c 662e 7669 6465 6f5f 6d65    (self.video_me
-0000fc80: 7461 5f64 6174 615b 2277 6964 7468 225d  ta_data["width"]
-0000fc90: 2c20 7365 6c66 2e76 6964 656f 5f6d 6574  , self.video_met
-0000fca0: 615f 6461 7461 5b22 6865 6967 6874 225d  a_data["height"]
-0000fcb0: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-0000fcc0: 2020 2020 2073 656c 662e 5f5f 696e 7365       self.__inse
-0000fcd0: 7274 5f69 6d67 2869 6d67 3d69 6d67 290a  rt_img(img=img).
-0000fce0: 0a20 2020 2064 6566 205f 5f72 756e 5f72  .    def __run_r
-0000fcf0: 6f74 6174 696f 6e28 7365 6c66 293a 0a20  otation(self):. 
-0000fd00: 2020 2020 2020 2073 656c 662e 6d61 696e         self.main
-0000fd10: 5f66 726d 2e64 6573 7472 6f79 2829 0a20  _frm.destroy(). 
-0000fd20: 2020 2020 2020 2073 7461 7274 203d 2074         start = t
-0000fd30: 696d 652e 7469 6d65 2829 0a20 2020 2020  ime.time().     
-0000fd40: 2020 2069 6620 7365 6c66 2e66 666d 7065     if self.ffmpe
-0000fd50: 6720 6f72 2073 656c 662e 6770 753a 0a20  g or self.gpu:. 
-0000fd60: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
-0000fd70: 6964 656f 5f63 6e74 2c20 2876 6964 656f  ideo_cnt, (video
-0000fd80: 5f70 6174 682c 2072 6f74 6174 696f 6e29  _path, rotation)
-0000fd90: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-0000fda0: 6c66 2e72 6573 756c 7473 2e69 7465 6d73  lf.results.items
-0000fdb0: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-0000fdc0: 2020 2020 205f 2c20 6e61 6d65 2c20 5f20       _, name, _ 
-0000fdd0: 3d20 6765 745f 666e 5f65 7874 2866 696c  = get_fn_ext(fil
-0000fde0: 6570 6174 683d 7669 6465 6f5f 7061 7468  epath=video_path
-0000fdf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fe00: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
-0000fe10: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
+0000f520: 0a0a 2020 2020 2020 2020 6966 2067 7075  ..        if gpu
+0000f530: 2061 6e64 206e 6f74 2063 6865 636b 5f6e   and not check_n
+0000f540: 7669 6465 615f 6770 755f 6176 6169 6c61  videa_gpu_availa
+0000f550: 626c 6528 293a 0a20 2020 2020 2020 2020  ble():.         
+0000f560: 2020 2072 6169 7365 2046 464d 5045 4743     raise FFMPEGC
+0000f570: 6f64 6563 4750 5545 7272 6f72 280a 2020  odecGPUError(.  
+0000f580: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+0000f590: 673d 224e 6f20 4750 5520 666f 756e 6420  g="No GPU found 
+0000f5a0: 2861 7320 6576 616c 7561 7465 6420 6279  (as evaluated by
+0000f5b0: 206e 7669 6465 612d 736d 6920 7265 7475   nvidea-smi retu
+0000f5c0: 726e 696e 6720 4e6f 6e65 2922 2c0a 2020  rning None)",.  
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+0000f5e0: 7572 6365 3d73 656c 662e 5f5f 636c 6173  urce=self.__clas
+0000f5f0: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c0a 2020  s__.__name__,.  
+0000f600: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f610: 2020 2020 6966 2066 666d 7065 6720 616e      if ffmpeg an
+0000f620: 6420 6e6f 7420 6368 6563 6b5f 6666 6d70  d not check_ffmp
+0000f630: 6567 5f61 7661 696c 6162 6c65 2829 3a0a  eg_available():.
+0000f640: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000f650: 6520 4646 4d50 4547 4e6f 7446 6f75 6e64  e FFMPEGNotFound
+0000f660: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000f670: 2020 2020 2020 206d 7367 3d27 4646 4d50         msg='FFMP
+0000f680: 4547 206e 6f74 2066 6f75 6e64 206f 6e20  EG not found on 
+0000f690: 7468 6520 636f 6d70 7574 6572 2028 6173  the computer (as
+0000f6a0: 2065 7661 6c75 6174 6564 2062 7920 2266   evaluated by "f
+0000f6b0: 666d 7065 6722 2072 6574 7572 6e69 6e67  fmpeg" returning
+0000f6c0: 204e 6f6e 6529 272c 0a20 2020 2020 2020   None)',.       
+0000f6d0: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+0000f6e0: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+0000f6f0: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
+0000f700: 2020 2020 2029 0a20 2020 2020 2020 205f       ).        _
+0000f710: 2c20 7365 6c66 2e63 7075 5f63 6e74 203d  , self.cpu_cnt =
+0000f720: 2066 696e 645f 636f 7265 5f63 6e74 2829   find_core_cnt()
+0000f730: 0a20 2020 2020 2020 2073 656c 662e 6770  .        self.gp
+0000f740: 752c 2073 656c 662e 6666 6d70 6567 203d  u, self.ffmpeg =
+0000f750: 2067 7075 2c20 6666 6d70 6567 0a20 2020   gpu, ffmpeg.   
+0000f760: 2020 2020 2073 656c 662e 7361 7665 5f64       self.save_d
+0000f770: 6972 203d 206f 7574 7075 745f 6469 720a  ir = output_dir.
+0000f780: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+0000f790: 6574 696d 6520 3d20 6461 7465 7469 6d65  etime = datetime
+0000f7a0: 2e6e 6f77 2829 2e73 7472 6674 696d 6528  .now().strftime(
+0000f7b0: 2225 5925 6d25 6425 4825 4d25 5322 290a  "%Y%m%d%H%M%S").
+0000f7c0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+0000f7d0: 7468 2e69 7366 696c 6528 696e 7075 745f  th.isfile(input_
+0000f7e0: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+0000f7f0: 2020 2073 656c 662e 7669 6465 6f5f 7061     self.video_pa
+0000f800: 7468 7320 3d20 5b69 6e70 7574 5f70 6174  ths = [input_pat
+0000f810: 685d 0a20 2020 2020 2020 2065 6c73 653a  h].        else:
+0000f820: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f830: 662e 7669 6465 6f5f 7061 7468 7320 3d20  f.video_paths = 
+0000f840: 6669 6e64 5f61 6c6c 5f76 6964 656f 735f  find_all_videos_
+0000f850: 696e 5f64 6972 6563 746f 7279 280a 2020  in_directory(.  
+0000f860: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000f870: 7265 6374 6f72 793d 696e 7075 745f 7061  rectory=input_pa
+0000f880: 7468 2c20 6173 5f64 6963 743d 5472 7565  th, as_dict=True
+0000f890: 0a20 2020 2020 2020 2020 2020 2029 2e76  .            ).v
+0000f8a0: 616c 7565 7328 290a 2020 2020 2020 2020  alues().        
+0000f8b0: 2020 2020 6368 6563 6b5f 6966 5f66 696c      check_if_fil
+0000f8c0: 6570 6174 685f 6c69 7374 5f69 735f 656d  epath_list_is_em
+0000f8d0: 7074 7928 0a20 2020 2020 2020 2020 2020  pty(.           
+0000f8e0: 2020 2020 2066 696c 6570 6174 6873 3d73       filepaths=s
+0000f8f0: 656c 662e 7669 6465 6f5f 7061 7468 732c  elf.video_paths,
+0000f900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f910: 2065 7272 6f72 5f6d 7367 3d66 224e 6f20   error_msg=f"No 
+0000f920: 7669 6465 6f73 2066 6f75 6e64 2069 6e20  videos found in 
+0000f930: 7b69 6e70 7574 5f70 6174 687d 2064 6972  {input_path} dir
+0000f940: 6563 746f 7279 222c 0a20 2020 2020 2020  ectory",.       
+0000f950: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0000f960: 5f5f 696e 7365 7274 5f69 6d67 2873 656c  __insert_img(sel
+0000f970: 662c 2069 6d67 3a20 6e70 2e61 7272 6179  f, img: np.array
+0000f980: 293a 0a20 2020 2020 2020 2063 7572 7265  ):.        curre
+0000f990: 6e74 5f66 726d 5f70 696c 203d 2049 6d61  nt_frm_pil = Ima
+0000f9a0: 6765 2e66 726f 6d61 7272 6179 2869 6d67  ge.fromarray(img
+0000f9b0: 290a 2020 2020 2020 2020 6375 7272 656e  ).        curren
+0000f9c0: 745f 6672 6d5f 7069 6c2e 7468 756d 626e  t_frm_pil.thumbn
+0000f9d0: 6169 6c28 4d41 585f 4652 4d5f 5349 5a45  ail(MAX_FRM_SIZE
+0000f9e0: 2c20 496d 6167 652e 414e 5449 414c 4941  , Image.ANTIALIA
+0000f9f0: 5329 0a20 2020 2020 2020 2063 7572 7265  S).        curre
+0000fa00: 6e74 5f66 726d 5f70 696c 203d 2049 6d61  nt_frm_pil = Ima
+0000fa10: 6765 546b 2e50 686f 746f 496d 6167 6528  geTk.PhotoImage(
+0000fa20: 0a20 2020 2020 2020 2020 2020 206d 6173  .            mas
+0000fa30: 7465 723d 7365 6c66 2e6d 6169 6e5f 6672  ter=self.main_fr
+0000fa40: 6d2c 2069 6d61 6765 3d63 7572 7265 6e74  m, image=current
+0000fa50: 5f66 726d 5f70 696c 0a20 2020 2020 2020  _frm_pil.       
+0000fa60: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000fa70: 7669 6465 6f5f 6672 616d 6520 3d20 4c61  video_frame = La
+0000fa80: 6265 6c28 7365 6c66 2e6d 6169 6e5f 6672  bel(self.main_fr
+0000fa90: 6d2c 2069 6d61 6765 3d63 7572 7265 6e74  m, image=current
+0000faa0: 5f66 726d 5f70 696c 290a 2020 2020 2020  _frm_pil).      
+0000fab0: 2020 7365 6c66 2e76 6964 656f 5f66 7261    self.video_fra
+0000fac0: 6d65 2e69 6d61 6765 203d 2063 7572 7265  me.image = curre
+0000fad0: 6e74 5f66 726d 5f70 696c 0a20 2020 2020  nt_frm_pil.     
+0000fae0: 2020 2073 656c 662e 7669 6465 6f5f 6672     self.video_fr
+0000faf0: 616d 652e 6772 6964 2872 6f77 3d30 2c20  ame.grid(row=0, 
+0000fb00: 636f 6c75 6d6e 3d30 290a 0a20 2020 2064  column=0)..    d
+0000fb10: 6566 205f 5f72 6f74 6174 6528 7365 6c66  ef __rotate(self
+0000fb20: 2c20 7661 6c75 653a 2069 6e74 2c20 696d  , value: int, im
+0000fb30: 673a 206e 702e 6172 7261 7929 3a0a 2020  g: np.array):.  
+0000fb40: 2020 2020 2020 7365 6c66 2e64 6966 5f61        self.dif_a
+0000fb50: 6e67 6c65 202b 3d20 7661 6c75 650a 2020  ngle += value.  
+0000fb60: 2020 2020 2020 726f 7461 7469 6f6e 5f6d        rotation_m
+0000fb70: 6174 7269 7820 3d20 6376 322e 6765 7452  atrix = cv2.getR
+0000fb80: 6f74 6174 696f 6e4d 6174 7269 7832 4428  otationMatrix2D(
+0000fb90: 0a20 2020 2020 2020 2020 2020 2028 7365  .            (se
+0000fba0: 6c66 2e76 6964 656f 5f6d 6574 615f 6461  lf.video_meta_da
+0000fbb0: 7461 5b22 7769 6474 6822 5d20 2f20 322c  ta["width"] / 2,
+0000fbc0: 2073 656c 662e 7669 6465 6f5f 6d65 7461   self.video_meta
+0000fbd0: 5f64 6174 615b 2268 6569 6768 7422 5d20  _data["height"] 
+0000fbe0: 2f20 3229 2c0a 2020 2020 2020 2020 2020  / 2),.          
+0000fbf0: 2020 7365 6c66 2e64 6966 5f61 6e67 6c65    self.dif_angle
+0000fc00: 2c0a 2020 2020 2020 2020 2020 2020 312c  ,.            1,
+0000fc10: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000fc20: 2020 2069 6d67 203d 2063 7632 2e77 6172     img = cv2.war
+0000fc30: 7041 6666 696e 6528 0a20 2020 2020 2020  pAffine(.       
+0000fc40: 2020 2020 2069 6d67 2c0a 2020 2020 2020       img,.      
+0000fc50: 2020 2020 2020 726f 7461 7469 6f6e 5f6d        rotation_m
+0000fc60: 6174 7269 782c 0a20 2020 2020 2020 2020  atrix,.         
+0000fc70: 2020 2028 7365 6c66 2e76 6964 656f 5f6d     (self.video_m
+0000fc80: 6574 615f 6461 7461 5b22 7769 6474 6822  eta_data["width"
+0000fc90: 5d2c 2073 656c 662e 7669 6465 6f5f 6d65  ], self.video_me
+0000fca0: 7461 5f64 6174 615b 2268 6569 6768 7422  ta_data["height"
+0000fcb0: 5d29 2c0a 2020 2020 2020 2020 290a 2020  ]),.        ).  
+0000fcc0: 2020 2020 2020 7365 6c66 2e5f 5f69 6e73        self.__ins
+0000fcd0: 6572 745f 696d 6728 696d 673d 696d 6729  ert_img(img=img)
+0000fce0: 0a0a 2020 2020 6465 6620 5f5f 7275 6e5f  ..    def __run_
+0000fcf0: 726f 7461 7469 6f6e 2873 656c 6629 3a0a  rotation(self):.
+0000fd00: 2020 2020 2020 2020 7365 6c66 2e6d 6169          self.mai
+0000fd10: 6e5f 6672 6d2e 6465 7374 726f 7928 290a  n_frm.destroy().
+0000fd20: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
+0000fd30: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
+0000fd40: 2020 2020 6966 2073 656c 662e 6666 6d70      if self.ffmp
+0000fd50: 6567 206f 7220 7365 6c66 2e67 7075 3a0a  eg or self.gpu:.
+0000fd60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000fd70: 7669 6465 6f5f 636e 742c 2028 7669 6465  video_cnt, (vide
+0000fd80: 6f5f 7061 7468 2c20 726f 7461 7469 6f6e  o_path, rotation
+0000fd90: 2920 696e 2065 6e75 6d65 7261 7465 2873  ) in enumerate(s
+0000fda0: 656c 662e 7265 7375 6c74 732e 6974 656d  elf.results.item
+0000fdb0: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+0000fdc0: 2020 2020 2020 5f2c 206e 616d 652c 205f        _, name, _
+0000fdd0: 203d 2067 6574 5f66 6e5f 6578 7428 6669   = get_fn_ext(fi
+0000fde0: 6c65 7061 7468 3d76 6964 656f 5f70 6174  lepath=video_pat
+0000fdf0: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+0000fe00: 2020 2073 6176 655f 7061 7468 203d 206f     save_path = o
+0000fe10: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
 0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 7365 6c66 2e73 6176 655f 6469 722c 2066  self.save_dir, f
-0000fe40: 227b 6e61 6d65 7d5f 726f 7461 7465 645f  "{name}_rotated_
-0000fe50: 7b73 656c 662e 6461 7465 7469 6d65 7d2e  {self.datetime}.
-0000fe60: 6d70 3422 0a20 2020 2020 2020 2020 2020  mp4".           
-0000fe70: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000fe80: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
-0000fe90: 7075 3a0a 2020 2020 2020 2020 2020 2020  pu:.            
-0000fea0: 2020 2020 2020 2020 636d 6420 3d20 6627          cmd = f'
-0000feb0: 6666 6d70 6567 202d 6877 6163 6365 6c20  ffmpeg -hwaccel 
-0000fec0: 6175 746f 202d 6920 7b76 6964 656f 5f70  auto -i {video_p
-0000fed0: 6174 687d 202d 7666 2022 6877 7570 6c6f  ath} -vf "hwuplo
-0000fee0: 6164 5f63 7564 612c 726f 7461 7465 3d7b  ad_cuda,rotate={
-0000fef0: 726f 7461 7469 6f6e 7d2a 2850 492f 3138  rotation}*(PI/18
-0000ff00: 3029 2c66 6f72 6d61 743d 6e76 3132 7c63  0),format=nv12|c
-0000ff10: 7564 6122 202d 633a 7620 6832 3634 5f6e  uda" -c:v h264_n
-0000ff20: 7665 6e63 207b 7361 7665 5f70 6174 687d  venc {save_path}
-0000ff30: 202d 7927 0a20 2020 2020 2020 2020 2020   -y'.           
-0000ff40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000ff60: 6d64 203d 2066 2766 666d 7065 6720 2d69  md = f'ffmpeg -i
-0000ff70: 207b 7669 6465 6f5f 7061 7468 7d20 2d76   {video_path} -v
-0000ff80: 6620 2272 6f74 6174 653d 7b72 6f74 6174  f "rotate={rotat
-0000ff90: 696f 6e7d 2a28 5049 2f31 3830 2922 207b  ion}*(PI/180)" {
-0000ffa0: 7361 7665 5f70 6174 687d 202d 7927 0a20  save_path} -y'. 
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ffc0: 7562 7072 6f63 6573 732e 6361 6c6c 2863  ubprocess.call(c
-0000ffd0: 6d64 2c20 7368 656c 6c3d 5472 7565 2c20  md, shell=True, 
-0000ffe0: 7374 646f 7574 3d73 7562 7072 6f63 6573  stdout=subproces
-0000fff0: 732e 5049 5045 290a 2020 2020 2020 2020  s.PIPE).        
-00010000: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00010010: 2020 666f 7220 7669 6465 6f5f 636e 742c    for video_cnt,
-00010020: 2028 7669 6465 6f5f 7061 7468 2c20 726f   (video_path, ro
-00010030: 7461 7469 6f6e 2920 696e 2065 6e75 6d65  tation) in enume
-00010040: 7261 7465 2873 656c 662e 7265 7375 6c74  rate(self.result
-00010050: 732e 6974 656d 7328 2929 3a0a 2020 2020  s.items()):.    
-00010060: 2020 2020 2020 2020 2020 2020 6361 7020              cap 
-00010070: 3d20 6376 322e 5669 6465 6f43 6170 7475  = cv2.VideoCaptu
-00010080: 7265 2876 6964 656f 5f70 6174 6829 0a20  re(video_path). 
-00010090: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000100a0: 2c20 6e61 6d65 2c20 5f20 3d20 6765 745f  , name, _ = get_
-000100b0: 666e 5f65 7874 2866 696c 6570 6174 683d  fn_ext(filepath=
-000100c0: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-000100d0: 2020 2020 2020 2020 2020 2020 726f 7461              rota
-000100e0: 7469 6f6e 5f6d 6174 7269 7820 3d20 6376  tion_matrix = cv
-000100f0: 322e 6765 7452 6f74 6174 696f 6e4d 6174  2.getRotationMat
-00010100: 7269 7832 4428 0a20 2020 2020 2020 2020  rix2D(.         
-00010110: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010130: 2020 2020 2073 656c 662e 7669 6465 6f5f       self.video_
-00010140: 6d65 7461 5f64 6174 615b 2277 6964 7468  meta_data["width
-00010150: 225d 202f 2032 2c0a 2020 2020 2020 2020  "] / 2,.        
-00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 7365 6c66 2e76 6964 656f 5f6d 6574 615f  self.video_meta_
-00010180: 6461 7461 5b22 6865 6967 6874 225d 202f  data["height"] /
-00010190: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
-000101a0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000101b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000101c0: 6f74 6174 696f 6e2c 0a20 2020 2020 2020  otation,.       
-000101d0: 2020 2020 2020 2020 2020 2020 2031 2c0a               1,.
-000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010200: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
-00010210: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 7365 6c66 2e73 6176 655f 6469 722c 2066  self.save_dir, f
-00010240: 227b 6e61 6d65 7d5f 726f 7461 7465 645f  "{name}_rotated_
-00010250: 7b73 656c 662e 6461 7465 7469 6d65 7d2e  {self.datetime}.
-00010260: 6d70 3422 0a20 2020 2020 2020 2020 2020  mp4".           
-00010270: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010280: 2020 2020 2020 2076 6964 656f 5f6d 6574         video_met
-00010290: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
-000102a0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
-000102b0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000102d0: 6f75 7263 6320 3d20 6376 322e 5669 6465  ourcc = cv2.Vide
-000102e0: 6f57 7269 7465 725f 666f 7572 6363 282a  oWriter_fourcc(*
-000102f0: 466f 726d 6174 732e 4d50 345f 434f 4445  Formats.MP4_CODE
-00010300: 432e 7661 6c75 6529 0a20 2020 2020 2020  C.value).       
-00010310: 2020 2020 2020 2020 2077 7269 7465 7220           writer 
-00010320: 3d20 6376 322e 5669 6465 6f57 7269 7465  = cv2.VideoWrite
-00010330: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00010340: 2020 2020 2020 2073 6176 655f 7061 7468         save_path
-00010350: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010360: 2020 2020 2020 666f 7572 6363 2c0a 2020        fourcc,.  
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 7669 6465 6f5f 6d65 7461 5b22 6670    video_meta["fp
-00010390: 7322 5d2c 0a20 2020 2020 2020 2020 2020  s"],.           
-000103a0: 2020 2020 2020 2020 2028 7669 6465 6f5f           (video_
-000103b0: 6d65 7461 5b22 7769 6474 6822 5d2c 2076  meta["width"], v
-000103c0: 6964 656f 5f6d 6574 615b 2268 6569 6768  ideo_meta["heigh
-000103d0: 7422 5d29 2c0a 2020 2020 2020 2020 2020  t"]),.          
-000103e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000103f0: 2020 2020 2020 2020 696d 675f 636e 7420          img_cnt 
-00010400: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00010410: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2020 2020 7265 742c 2069 6d67 203d 2063      ret, img = c
-00010440: 6170 2e72 6561 6428 290a 2020 2020 2020  ap.read().      
-00010450: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010460: 206e 6f74 2072 6574 3a0a 2020 2020 2020   not ret:.      
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00010490: 2020 2020 2020 2020 2020 2020 696d 6720              img 
-000104a0: 3d20 6376 322e 7761 7270 4166 6669 6e65  = cv2.warpAffine
-000104b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000104c0: 2020 2020 2020 2020 2020 696d 672c 0a20            img,. 
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 2020 2020 2020 2072 6f74 6174 696f 6e5f         rotation_
-000104f0: 6d61 7472 6978 2c0a 2020 2020 2020 2020  matrix,.        
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 2873 656c 662e 7669 6465 6f5f 6d65 7461  (self.video_meta
-00010520: 5f64 6174 615b 2277 6964 7468 225d 2c20  _data["width"], 
-00010530: 7365 6c66 2e76 6964 656f 5f6d 6574 615f  self.video_meta_
-00010540: 6461 7461 5b22 6865 6967 6874 225d 292c  data["height"]),
-00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010560: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010570: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00010580: 722e 7772 6974 6528 696d 6729 0a20 2020  r.write(img).   
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2069 6d67 5f63 6e74 202b 3d20 310a 2020   img_cnt += 1.  
-000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105c0: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2066 2752 6f74 6174 696e 6720 6672 616d   f'Rotating fram
-000105f0: 6520 7b69 6d67 5f63 6e74 7d2f 7b76 6964  e {img_cnt}/{vid
-00010600: 656f 5f6d 6574 615b 2266 7261 6d65 5f63  eo_meta["frame_c
-00010610: 6f75 6e74 225d 7d20 2856 6964 656f 207b  ount"]} (Video {
-00010620: 7669 6465 6f5f 636e 7420 2b20 317d 2f7b  video_cnt + 1}/{
-00010630: 6c65 6e28 7365 6c66 2e72 6573 756c 7473  len(self.results
-00010640: 2e6b 6579 7328 2929 7d29 2027 0a20 2020  .keys())}) '.   
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00010670: 2020 2063 6170 2e72 656c 6561 7365 2829     cap.release()
-00010680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010690: 2077 7269 7465 722e 7265 6c65 6173 6528   writer.release(
-000106a0: 290a 2020 2020 2020 2020 7374 646f 7574  ).        stdout
-000106b0: 5f73 7563 6365 7373 280a 2020 2020 2020  _success(.      
-000106c0: 2020 2020 2020 6d73 673d 6622 416c 6c20        msg=f"All 
-000106d0: 7669 6465 6f73 2072 6f74 6174 6564 2061  videos rotated a
-000106e0: 6e64 2073 6176 6564 2069 6e20 7b73 656c  nd saved in {sel
-000106f0: 662e 7361 7665 5f64 6972 7d22 2c0a 2020  f.save_dir}",.  
-00010700: 2020 2020 2020 2020 2020 656c 6170 7365            elapse
-00010710: 645f 7469 6d65 3d73 7472 2872 6f75 6e64  d_time=str(round
-00010720: 2828 7469 6d65 2e74 696d 6528 2920 2d20  ((time.time() - 
-00010730: 7374 6172 7429 2c20 3229 292c 0a20 2020  start), 2)),.   
-00010740: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
-00010750: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
-00010760: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
-00010770: 2029 0a0a 2020 2020 6465 6620 5f5f 7361   )..    def __sa
-00010780: 7665 2873 656c 6629 3a0a 2020 2020 2020  ve(self):.      
-00010790: 2020 7072 6f63 6573 7320 3d20 4e6f 6e65    process = None
-000107a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000107b0: 7375 6c74 735b 7365 6c66 2e66 696c 655f  sults[self.file_
-000107c0: 7061 7468 5d20 3d20 7365 6c66 2e64 6966  path] = self.dif
-000107d0: 5f61 6e67 6c65 0a20 2020 2020 2020 2069  _angle.        i
-000107e0: 6620 6c65 6e28 7365 6c66 2e72 6573 756c  f len(self.resul
-000107f0: 7473 2e6b 6579 7328 2929 203d 3d20 6c65  ts.keys()) == le
-00010800: 6e28 7365 6c66 2e76 6964 656f 5f70 6174  n(self.video_pat
-00010810: 6873 293a 0a20 2020 2020 2020 2020 2020  hs):.           
-00010820: 2070 726f 6365 7373 203d 206d 756c 7469   process = multi
-00010830: 7072 6f63 6573 7369 6e67 2e50 726f 6365  processing.Proce
-00010840: 7373 2874 6172 6765 743d 7365 6c66 2e5f  ss(target=self._
-00010850: 5f72 756e 5f72 6f74 6174 696f 6e28 2929  _run_rotation())
-00010860: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00010870: 6365 7373 2e73 7461 7274 2829 0a20 2020  cess.start().   
-00010880: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010890: 2020 2020 2020 2073 656c 662e 5f5f 7275         self.__ru
-000108a0: 6e5f 696e 7465 7266 6163 6528 0a20 2020  n_interface(.   
-000108b0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000108c0: 655f 7061 7468 3d73 656c 662e 7669 6465  e_path=self.vide
-000108d0: 6f5f 7061 7468 735b 6c65 6e28 7365 6c66  o_paths[len(self
-000108e0: 2e72 6573 756c 7473 2e6b 6579 7328 2929  .results.keys())
-000108f0: 202d 2031 5d0a 2020 2020 2020 2020 2020   - 1].          
-00010900: 2020 290a 2020 2020 2020 2020 6966 2070    ).        if p
-00010910: 726f 6365 7373 2069 7320 6e6f 7420 4e6f  rocess is not No
-00010920: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00010930: 7072 6f63 6573 732e 6a6f 696e 2829 0a0a  process.join()..
-00010940: 2020 2020 6465 6620 5f5f 6269 6e64 5f6b      def __bind_k
-00010950: 6579 7328 7365 6c66 293a 0a20 2020 2020  eys(self):.     
-00010960: 2020 2073 656c 662e 6d61 696e 5f66 726d     self.main_frm
-00010970: 2e62 696e 6428 0a20 2020 2020 2020 2020  .bind(.         
-00010980: 2020 2022 3c4c 6566 743e 222c 206c 616d     "<Left>", lam
-00010990: 6264 6120 783a 2073 656c 662e 5f5f 726f  bda x: self.__ro
-000109a0: 7461 7465 2876 616c 7565 3d31 2c20 696d  tate(value=1, im
-000109b0: 673d 7365 6c66 2e5f 6f72 6967 5f69 6d67  g=self._orig_img
-000109c0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-000109d0: 2020 2020 7365 6c66 2e6d 6169 6e5f 6672      self.main_fr
-000109e0: 6d2e 6269 6e64 280a 2020 2020 2020 2020  m.bind(.        
-000109f0: 2020 2020 223c 5269 6768 743e 222c 206c      "<Right>", l
-00010a00: 616d 6264 6120 783a 2073 656c 662e 5f5f  ambda x: self.__
-00010a10: 726f 7461 7465 2876 616c 7565 3d2d 312c  rotate(value=-1,
-00010a20: 2069 6d67 3d73 656c 662e 5f6f 7269 675f   img=self._orig_
-00010a30: 696d 6729 0a20 2020 2020 2020 2029 0a20  img).        ). 
-00010a40: 2020 2020 2020 2073 656c 662e 6d61 696e         self.main
-00010a50: 5f66 726d 2e62 696e 6428 223c 4573 6361  _frm.bind("<Esca
-00010a60: 7065 3e22 2c20 6c61 6d62 6461 2078 3a20  pe>", lambda x: 
-00010a70: 7365 6c66 2e5f 5f73 6176 6528 2929 0a0a  self.__save())..
-00010a80: 2020 2020 6465 6620 5f5f 7275 6e5f 696e      def __run_in
-00010a90: 7465 7266 6163 6528 7365 6c66 2c20 6669  terface(self, fi
-00010aa0: 6c65 5f70 6174 683a 2073 7472 293a 0a20  le_path: str):. 
-00010ab0: 2020 2020 2020 2073 656c 662e 6469 665f         self.dif_
-00010ac0: 616e 676c 6520 3d20 300a 2020 2020 2020  angle = 0.      
-00010ad0: 2020 7072 696e 7428 6669 6c65 5f70 6174    print(file_pat
-00010ae0: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
-00010af0: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
-00010b00: 3d20 6765 745f 7669 6465 6f5f 6d65 7461  = get_video_meta
-00010b10: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
-00010b20: 3d66 696c 655f 7061 7468 290a 2020 2020  =file_path).    
-00010b30: 2020 2020 7365 6c66 2e66 696c 655f 7061      self.file_pa
-00010b40: 7468 203d 2066 696c 655f 7061 7468 0a20  th = file_path. 
-00010b50: 2020 2020 2020 205f 2c20 7365 6c66 2e76         _, self.v
-00010b60: 6964 656f 5f6e 616d 652c 205f 203d 2067  ideo_name, _ = g
-00010b70: 6574 5f66 6e5f 6578 7428 6669 6c65 7061  et_fn_ext(filepa
-00010b80: 7468 3d66 696c 655f 7061 7468 290a 2020  th=file_path).  
-00010b90: 2020 2020 2020 7365 6c66 2e6d 6169 6e5f        self.main_
-00010ba0: 6672 6d20 3d20 546f 706c 6576 656c 2829  frm = Toplevel()
-00010bb0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-00010bc0: 696e 5f66 726d 2e74 6974 6c65 2866 2252  in_frm.title(f"R
-00010bd0: 4f54 4154 4520 5649 4445 4f20 7b73 656c  OTATE VIDEO {sel
-00010be0: 662e 7669 6465 6f5f 6e61 6d65 7d22 290a  f.video_name}").
-00010bf0: 2020 2020 2020 2020 7365 6c66 2e76 6964          self.vid
-00010c00: 656f 5f66 726d 203d 2046 7261 6d65 2873  eo_frm = Frame(s
-00010c10: 656c 662e 6d61 696e 5f66 726d 290a 2020  elf.main_frm).  
-00010c20: 2020 2020 2020 7365 6c66 2e76 6964 656f        self.video
-00010c30: 5f66 726d 2e67 7269 6428 726f 773d 302c  _frm.grid(row=0,
-00010c40: 2063 6f6c 756d 6e3d 3029 0a20 2020 2020   column=0).     
-00010c50: 2020 2073 656c 662e 696e 7374 7275 6374     self.instruct
-00010c60: 696f 6e5f 6672 6d20 3d20 4672 616d 6528  ion_frm = Frame(
-00010c70: 7365 6c66 2e6d 6169 6e5f 6672 6d2c 2077  self.main_frm, w
-00010c80: 6964 7468 3d31 3030 2c20 6865 6967 6874  idth=100, height
-00010c90: 3d31 3030 290a 2020 2020 2020 2020 7365  =100).        se
-00010ca0: 6c66 2e69 6e73 7472 7563 7469 6f6e 5f66  lf.instruction_f
-00010cb0: 726d 2e67 7269 6428 726f 773d 302c 2063  rm.grid(row=0, c
-00010cc0: 6f6c 756d 6e3d 322c 2073 7469 636b 793d  olumn=2, sticky=
-00010cd0: 4e57 290a 2020 2020 2020 2020 7365 6c66  NW).        self
-00010ce0: 2e6b 6579 5f6c 626c 7320 3d20 4c61 6265  .key_lbls = Labe
-00010cf0: 6c28 0a20 2020 2020 2020 2020 2020 2073  l(.            s
-00010d00: 656c 662e 696e 7374 7275 6374 696f 6e5f  elf.instruction_
-00010d10: 6672 6d2c 0a20 2020 2020 2020 2020 2020  frm,.           
-00010d20: 2074 6578 743d 225c 6e5c 6e20 4e61 7669   text="\n\n Navi
-00010d30: 6761 7469 6f6e 3a20 220a 2020 2020 2020  gation: ".      
-00010d40: 2020 2020 2020 225c 6e20 4c65 6674 2061        "\n Left a
-00010d50: 7272 6f77 203d 2031 c2b0 206c 6566 7422  rrow = 1.. left"
-00010d60: 0a20 2020 2020 2020 2020 2020 2022 5c6e  .            "\n
-00010d70: 2052 6967 6874 2061 7272 6f77 203d 2031   Right arrow = 1
-00010d80: c2b0 2072 6967 6874 220a 2020 2020 2020  .. right".      
-00010d90: 2020 2020 2020 225c 6e20 4573 6320 3d20        "\n Esc = 
-00010da0: 5361 7665 222c 0a20 2020 2020 2020 2029  Save",.        )
-00010db0: 0a0a 2020 2020 2020 2020 7365 6c66 2e6b  ..        self.k
-00010dc0: 6579 5f6c 626c 732e 6772 6964 2873 7469  ey_lbls.grid(sti
-00010dd0: 636b 793d 4e57 290a 2020 2020 2020 2020  cky=NW).        
-00010de0: 7365 6c66 2e63 6170 203d 2063 7632 2e56  self.cap = cv2.V
-00010df0: 6964 656f 4361 7074 7572 6528 6669 6c65  ideoCapture(file
-00010e00: 5f70 6174 6829 0a20 2020 2020 2020 205f  _path).        _
-00010e10: 2c20 7365 6c66 2e69 6d67 203d 2073 656c  , self.img = sel
-00010e20: 662e 6361 702e 7265 6164 2829 0a20 2020  f.cap.read().   
-00010e30: 2020 2020 2073 656c 662e 5f6f 7269 675f       self._orig_
-00010e40: 696d 6720 3d20 6376 322e 6376 7443 6f6c  img = cv2.cvtCol
-00010e50: 6f72 2873 656c 662e 696d 672c 2063 7632  or(self.img, cv2
-00010e60: 2e43 4f4c 4f52 5f52 4742 3242 4752 290a  .COLOR_RGB2BGR).
-00010e70: 2020 2020 2020 2020 7365 6c66 2e5f 5f69          self.__i
-00010e80: 6e73 6572 745f 696d 6728 696d 673d 7365  nsert_img(img=se
-00010e90: 6c66 2e5f 6f72 6967 5f69 6d67 290a 2020  lf._orig_img).  
-00010ea0: 2020 2020 2020 7365 6c66 2e5f 5f62 696e        self.__bin
-00010eb0: 645f 6b65 7973 2829 0a0a 2020 2020 6465  d_keys()..    de
-00010ec0: 6620 7275 6e28 7365 6c66 293a 0a20 2020  f run(self):.   
-00010ed0: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
-00010ee0: 7320 3d20 7b7d 0a20 2020 2020 2020 2066  s = {}.        f
-00010ef0: 6f72 2076 6964 656f 5f70 6174 6820 696e  or video_path in
-00010f00: 2073 656c 662e 7669 6465 6f5f 7061 7468   self.video_path
-00010f10: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00010f20: 656c 662e 5f5f 7275 6e5f 696e 7465 7266  elf.__run_interf
-00010f30: 6163 6528 7669 6465 6f5f 7061 7468 290a  ace(video_path).
-00010f40: 2020 2020 2020 2020 7365 6c66 2e6d 6169          self.mai
-00010f50: 6e5f 6672 6d2e 6d61 696e 6c6f 6f70 2829  n_frm.mainloop()
-00010f60: 0a0a 0a64 6566 2065 7874 7261 6374 5f66  ...def extract_f
-00010f70: 7261 6d65 735f 6672 6f6d 5f61 6c6c 5f76  rames_from_all_v
-00010f80: 6964 656f 735f 696e 5f64 6972 6563 746f  ideos_in_directo
-00010f90: 7279 280a 2020 2020 636f 6e66 6967 5f70  ry(.    config_p
-00010fa0: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00010fb0: 6f73 2e50 6174 684c 696b 655d 2c20 6469  os.PathLike], di
-00010fc0: 7265 6374 6f72 793a 2055 6e69 6f6e 5b73  rectory: Union[s
-00010fd0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-00010fe0: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-00010ff0: 2222 220a 2020 2020 4578 7472 6163 7420  """.    Extract 
-00011000: 616c 6c20 6672 616d 6573 2066 726f 6d20  all frames from 
-00011010: 616c 6c20 7669 6465 6f73 2069 6e20 6120  all videos in a 
-00011020: 6469 7265 6374 6f72 792e 2054 6865 2072  directory. The r
-00011030: 6573 756c 7473 2061 7265 2073 6176 6564  esults are saved
-00011040: 2069 6e20 7468 6520 7072 6f6a 6563 745f   in the project_
-00011050: 666f 6c64 6572 2f66 7261 6d65 732f 696e  folder/frames/in
-00011060: 7075 7420 6469 7265 6374 6f72 7920 6f66  put directory of
-00011070: 2074 6865 2053 696d 4241 2070 726f 6a65   the SimBA proje
-00011080: 6374 0a0a 2020 2020 3a70 6172 616d 6574  ct..    :paramet
-00011090: 6572 2073 7472 2063 6f6e 6669 675f 7061  er str config_pa
-000110a0: 7468 3a20 7061 7468 2074 6f20 5369 6d42  th: path to SimB
-000110b0: 4120 7072 6f6a 6563 7420 636f 6e66 6967  A project config
-000110c0: 2066 696c 6520 696e 2043 6f6e 6669 6770   file in Configp
-000110d0: 6172 7365 7220 666f 726d 6174 2e0a 2020  arser format..  
-000110e0: 2020 3a70 6172 616d 6574 6572 2073 7472    :parameter str
-000110f0: 2064 6972 6563 746f 7279 3a20 7061 7468   directory: path
-00011100: 2074 6f20 6669 6c65 206f 7220 666f 6c64   to file or fold
-00011110: 6572 2063 6f6e 7461 696e 696e 6720 7669  er containing vi
-00011120: 6465 6f73 2069 6e20 6d70 3420 616e 642f  deos in mp4 and/
-00011130: 6f72 2061 7669 2066 6f72 6d61 742e 0a0a  or avi format...
-00011140: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
-00011150: 2020 3e3e 3e20 6578 7472 6163 745f 6672    >>> extract_fr
-00011160: 616d 6573 5f66 726f 6d5f 616c 6c5f 7669  ames_from_all_vi
-00011170: 6465 6f73 5f69 6e5f 6469 7265 6374 6f72  deos_in_director
-00011180: 7928 636f 6e66 6967 5f70 6174 683d 2770  y(config_path='p
-00011190: 726f 6a65 6374 5f66 6f6c 6465 722f 7072  roject_folder/pr
-000111a0: 6f6a 6563 745f 636f 6e66 6967 2e69 6e69  oject_config.ini
-000111b0: 272c 2073 6f75 7263 653d 272f 7465 7374  ', source='/test
-000111c0: 732f 7465 7374 5f64 6174 612f 7669 6465  s/test_data/vide
-000111d0: 6f5f 7465 7374 7327 290a 2020 2020 2222  o_tests').    ""
-000111e0: 220a 0a20 2020 2074 696d 6572 203d 2053  "..    timer = S
-000111f0: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
-00011200: 5472 7565 290a 2020 2020 7669 6465 6f5f  True).    video_
-00011210: 7061 7468 732c 2076 6964 656f 5f74 7970  paths, video_typ
-00011220: 6573 203d 205b 5d2c 205b 222e 6176 6922  es = [], [".avi"
-00011230: 2c20 222e 6d70 3422 5d0a 2020 2020 6669  , ".mp4"].    fi
-00011240: 6c65 735f 696e 5f66 6f6c 6465 7220 3d20  les_in_folder = 
-00011250: 676c 6f62 2e67 6c6f 6228 6469 7265 6374  glob.glob(direct
-00011260: 6f72 7920 2b20 222f 2a22 290a 2020 2020  ory + "/*").    
-00011270: 666f 7220 6669 6c65 5f70 6174 6820 696e  for file_path in
-00011280: 2066 696c 6573 5f69 6e5f 666f 6c64 6572   files_in_folder
-00011290: 3a0a 2020 2020 2020 2020 5f2c 205f 2c20  :.        _, _, 
-000112a0: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
-000112b0: 2866 696c 6570 6174 683d 6669 6c65 5f70  (filepath=file_p
-000112c0: 6174 6829 0a20 2020 2020 2020 2069 6620  ath).        if 
-000112d0: 6578 742e 6c6f 7765 7228 2920 696e 2076  ext.lower() in v
-000112e0: 6964 656f 5f74 7970 6573 3a0a 2020 2020  ideo_types:.    
-000112f0: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
-00011300: 7468 732e 6170 7065 6e64 2866 696c 655f  ths.append(file_
-00011310: 7061 7468 290a 2020 2020 6966 206c 656e  path).    if len
-00011320: 2876 6964 656f 5f70 6174 6873 2920 3d3d  (video_paths) ==
-00011330: 2030 3a0a 2020 2020 2020 2020 7261 6973   0:.        rais
-00011340: 6520 4e6f 4669 6c65 7346 6f75 6e64 4572  e NoFilesFoundEr
-00011350: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00011360: 206d 7367 3d66 2253 494d 4241 2045 5252   msg=f"SIMBA ERR
-00011370: 4f52 3a20 3020 7669 6465 6f20 6669 6c65  OR: 0 video file
-00011380: 7320 696e 206d 7034 206f 7220 6176 6920  s in mp4 or avi 
-00011390: 666f 726d 6174 2066 6f75 6e64 2069 6e20  format found in 
-000113a0: 7b64 6972 6563 746f 7279 7d22 2c0a 2020  {directory}",.  
-000113b0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000113c0: 3d65 7874 7261 6374 5f66 7261 6d65 735f  =extract_frames_
-000113d0: 6672 6f6d 5f61 6c6c 5f76 6964 656f 735f  from_all_videos_
-000113e0: 696e 5f64 6972 6563 746f 7279 2e5f 5f6e  in_directory.__n
-000113f0: 616d 655f 5f2c 0a20 2020 2020 2020 2029  ame__,.        )
-00011400: 0a20 2020 2063 6f6e 6669 6720 3d20 7265  .    config = re
-00011410: 6164 5f63 6f6e 6669 675f 6669 6c65 2863  ad_config_file(c
-00011420: 6f6e 6669 675f 7061 7468 290a 2020 2020  onfig_path).    
-00011430: 7072 6f6a 6563 745f 7061 7468 203d 2072  project_path = r
-00011440: 6561 645f 636f 6e66 6967 5f65 6e74 7279  ead_config_entry
-00011450: 280a 2020 2020 2020 2020 636f 6e66 6967  (.        config
-00011460: 2c20 2247 656e 6572 616c 2073 6574 7469  , "General setti
-00011470: 6e67 7322 2c20 2270 726f 6a65 6374 5f70  ngs", "project_p
-00011480: 6174 6822 2c20 6461 7461 5f74 7970 653d  ath", data_type=
-00011490: 2266 6f6c 6465 725f 7061 7468 220a 2020  "folder_path".  
-000114a0: 2020 290a 0a20 2020 2070 7269 6e74 280a    )..    print(.
-000114b0: 2020 2020 2020 2020 2245 7874 7261 6374          "Extract
-000114c0: 696e 6720 6672 616d 6573 2066 6f72 207b  ing frames for {
-000114d0: 7d20 7669 6465 6f73 2069 6e74 6f20 7072  } videos into pr
-000114e0: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
-000114f0: 6d65 732f 696e 7075 7420 6469 7265 6374  mes/input direct
-00011500: 6f72 792e 2e2e 222e 666f 726d 6174 280a  ory...".format(.
-00011510: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-00011520: 7669 6465 6f5f 7061 7468 7329 0a20 2020  video_paths).   
-00011530: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
-00011540: 2066 6f72 2076 6964 656f 5f70 6174 6820   for video_path 
-00011550: 696e 2076 6964 656f 5f70 6174 6873 3a0a  in video_paths:.
-00011560: 2020 2020 2020 2020 6469 725f 6e61 6d65          dir_name
-00011570: 2c20 7669 6465 6f5f 6e61 6d65 2c20 6578  , video_name, ex
-00011580: 7420 3d20 6765 745f 666e 5f65 7874 2876  t = get_fn_ext(v
-00011590: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
-000115a0: 2020 2073 6176 655f 7061 7468 203d 206f     save_path = o
-000115b0: 732e 7061 7468 2e6a 6f69 6e28 7072 6f6a  s.path.join(proj
-000115c0: 6563 745f 7061 7468 2c20 2266 7261 6d65  ect_path, "frame
-000115d0: 7322 2c20 2269 6e70 7574 222c 2076 6964  s", "input", vid
-000115e0: 656f 5f6e 616d 6529 0a20 2020 2020 2020  eo_name).       
-000115f0: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-00011600: 6578 6973 7473 2873 6176 655f 7061 7468  exists(save_path
-00011610: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
-00011620: 732e 6d61 6b65 6469 7273 2873 6176 655f  s.makedirs(save_
-00011630: 7061 7468 290a 2020 2020 2020 2020 656c  path).        el
-00011640: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00011650: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00011660: 2020 2020 2020 2066 2246 7261 6d65 7320         f"Frames 
-00011670: 666f 7220 7669 6465 6f20 7b76 6964 656f  for video {video
-00011680: 5f6e 616d 657d 2061 6c72 6561 6479 2065  _name} already e
-00011690: 7874 7261 6374 6564 2e20 5369 6d42 4120  xtracted. SimBA 
-000116a0: 6973 206f 7665 7277 7269 7469 6e67 2070  is overwriting p
-000116b0: 7269 6f72 2066 7261 6d65 732e 2e2e 220a  rior frames...".
-000116c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000116d0: 2020 2020 2020 7669 6465 6f5f 746f 5f66        video_to_f
-000116e0: 7261 6d65 7328 7669 6465 6f5f 7061 7468  rames(video_path
-000116f0: 2c20 7361 7665 5f70 6174 682c 206f 7665  , save_path, ove
-00011700: 7277 7269 7465 3d54 7275 652c 2065 7665  rwrite=True, eve
-00011710: 7279 3d31 2c20 6368 756e 6b5f 7369 7a65  ry=1, chunk_size
-00011720: 3d31 3030 3029 0a20 2020 2074 696d 6572  =1000).    timer
-00011730: 2e73 746f 705f 7469 6d65 7228 290a 2020  .stop_timer().  
-00011740: 2020 7374 646f 7574 5f73 7563 6365 7373    stdout_success
-00011750: 280a 2020 2020 2020 2020 6622 4672 616d  (.        f"Fram
-00011760: 6573 2063 7265 6174 6564 2066 6f72 207b  es created for {
-00011770: 7374 7228 6c65 6e28 7669 6465 6f5f 7061  str(len(video_pa
-00011780: 7468 7329 297d 2076 6964 656f 7322 2c0a  ths))} videos",.
-00011790: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
-000117a0: 7469 6d65 3d74 696d 6572 2e65 6c61 7073  time=timer.elaps
-000117b0: 6564 5f74 696d 655f 7374 722c 0a20 2020  ed_time_str,.   
-000117c0: 2020 2020 2073 6f75 7263 653d 6578 7472       source=extr
-000117d0: 6163 745f 6672 616d 6573 5f66 726f 6d5f  act_frames_from_
-000117e0: 616c 6c5f 7669 6465 6f73 5f69 6e5f 6469  all_videos_in_di
-000117f0: 7265 6374 6f72 792e 5f5f 6e61 6d65 5f5f  rectory.__name__
-00011800: 2c0a 2020 2020 290a 0a0a 6465 6620 636f  ,.    )...def co
-00011810: 7079 5f69 6d67 5f66 6f6c 6465 7228 0a20  py_img_folder(. 
-00011820: 2020 2063 6f6e 6669 675f 7061 7468 3a20     config_path: 
-00011830: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-00011840: 7468 4c69 6b65 5d2c 2073 6f75 7263 653a  thLike], source:
-00011850: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00011860: 6174 684c 696b 655d 0a29 202d 3e20 4e6f  athLike].) -> No
-00011870: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
-00011880: 436f 7079 2064 6972 6563 746f 7279 206f  Copy directory o
-00011890: 6620 706e 6720 6669 6c65 7320 746f 2074  f png files to t
-000118a0: 6865 2053 696d 4241 2070 726f 6a65 6374  he SimBA project
-000118b0: 2e20 5468 6520 6469 7265 6374 6f72 7920  . The directory 
-000118c0: 6973 2073 746f 7265 6420 696e 2074 6865  is stored in the
-000118d0: 2070 726f 6a65 6374 5f66 6f6c 6465 722f   project_folder/
-000118e0: 6672 616d 6573 2f69 6e70 7574 2066 6f6c  frames/input fol
-000118f0: 6465 7220 6f66 2074 6865 2053 696d 4241  der of the SimBA
-00011900: 2070 726f 6a65 6374 0a0a 2020 2020 3a70   project..    :p
-00011910: 6172 616d 6574 6572 2073 7472 2063 6f6e  arameter str con
-00011920: 6669 675f 7061 7468 3a20 7061 7468 2074  fig_path: path t
-00011930: 6f20 5369 6d42 4120 7072 6f6a 6563 7420  o SimBA project 
-00011940: 636f 6e66 6967 2066 696c 6520 696e 2043  config file in C
-00011950: 6f6e 6669 6770 6172 7365 7220 666f 726d  onfigparser form
-00011960: 6174 2e0a 2020 2020 3a70 6172 616d 6574  at..    :paramet
-00011970: 6572 2073 7472 2073 6f75 7263 653a 2070  er str source: p
-00011980: 6174 6820 746f 2069 6d61 6765 2066 6f6c  ath to image fol
-00011990: 6465 7220 6f75 7473 6964 6520 5369 6d42  der outside SimB
-000119a0: 4120 7072 6f6a 6563 742e 0a0a 2020 2020  A project...    
-000119b0: 3a65 7861 6d70 6c65 3a0a 2020 2020 3e3e  :example:.    >>
-000119c0: 3e20 636f 7079 5f69 6d67 5f66 6f6c 6465  > copy_img_folde
-000119d0: 7228 636f 6e66 6967 5f70 6174 683d 274d  r(config_path='M
-000119e0: 7953 696d 4241 7072 6f6a 6563 7443 6f6e  ySimBAprojectCon
-000119f0: 6669 6727 2c20 736f 7572 6365 3d27 2f44  fig', source='/D
-00011a00: 6972 6563 746f 7279 5769 7468 5669 6465  irectoryWithVide
-00011a10: 6f73 2f27 290a 0a20 2020 2022 2222 0a20  os/')..    """. 
-00011a20: 2020 2074 696d 6572 203d 2053 696d 6261     timer = Simba
-00011a30: 5469 6d65 7228 7374 6172 743d 5472 7565  Timer(start=True
-00011a40: 290a 2020 2020 6966 206e 6f74 206f 732e  ).    if not os.
-00011a50: 7061 7468 2e69 7364 6972 2873 6f75 7263  path.isdir(sourc
-00011a60: 6529 3a0a 2020 2020 2020 2020 7261 6973  e):.        rais
-00011a70: 6520 4e6f 7444 6972 6563 746f 7279 4572  e NotDirectoryEr
-00011a80: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00011a90: 206d 7367 3d66 2253 494d 4241 2045 5252   msg=f"SIMBA ERR
-00011aa0: 4f52 3a20 736f 7572 6365 207b 736f 7572  OR: source {sour
-00011ab0: 6365 7d20 6973 206e 6f74 2061 2064 6972  ce} is not a dir
-00011ac0: 6563 746f 7279 2e22 2c0a 2020 2020 2020  ectory.",.      
-00011ad0: 2020 2020 2020 736f 7572 6365 3d63 6f70        source=cop
-00011ae0: 795f 696d 675f 666f 6c64 6572 2e5f 5f6e  y_img_folder.__n
-00011af0: 616d 655f 5f2c 0a20 2020 2020 2020 2029  ame__,.        )
-00011b00: 0a20 2020 2069 6620 6c65 6e28 676c 6f62  .    if len(glob
-00011b10: 2e67 6c6f 6228 736f 7572 6365 202b 2022  .glob(source + "
-00011b20: 2f2a 2e70 6e67 2229 2920 3d3d 2030 3a0a  /*.png")) == 0:.
-00011b30: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00011b40: 4669 6c65 7346 6f75 6e64 4572 726f 7228  FilesFoundError(
-00011b50: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00011b60: 3d66 2253 494d 4241 2045 5252 4f52 3a20  =f"SIMBA ERROR: 
-00011b70: 736f 7572 6365 207b 736f 7572 6365 7d20  source {source} 
-00011b80: 646f 6573 206e 6f74 2063 6f6e 7461 696e  does not contain
-00011b90: 2061 6e79 202e 706e 6720 6669 6c65 732e   any .png files.
-00011ba0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00011bb0: 6f75 7263 653d 636f 7079 5f69 6d67 5f66  ource=copy_img_f
-00011bc0: 6f6c 6465 722e 5f5f 6e61 6d65 5f5f 2c0a  older.__name__,.
-00011bd0: 2020 2020 2020 2020 290a 2020 2020 696e          ).    in
-00011be0: 7075 745f 6261 7365 6e61 6d65 203d 206f  put_basename = o
-00011bf0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-00011c00: 736f 7572 6365 290a 2020 2020 636f 6e66  source).    conf
-00011c10: 6967 203d 2072 6561 645f 636f 6e66 6967  ig = read_config
-00011c20: 5f66 696c 6528 636f 6e66 6967 5f70 6174  _file(config_pat
-00011c30: 6829 0a20 2020 2070 726f 6a65 6374 5f70  h).    project_p
-00011c40: 6174 6820 3d20 7265 6164 5f63 6f6e 6669  ath = read_confi
-00011c50: 675f 656e 7472 7928 0a20 2020 2020 2020  g_entry(.       
-00011c60: 2063 6f6e 6669 672c 0a20 2020 2020 2020   config,.       
-00011c70: 2043 6f6e 6669 674b 6579 2e47 454e 4552   ConfigKey.GENER
-00011c80: 414c 5f53 4554 5449 4e47 532e 7661 6c75  AL_SETTINGS.valu
-00011c90: 652c 0a20 2020 2020 2020 2043 6f6e 6669  e,.        Confi
-00011ca0: 674b 6579 2e50 524f 4a45 4354 5f50 4154  gKey.PROJECT_PAT
-00011cb0: 482e 7661 6c75 652c 0a20 2020 2020 2020  H.value,.       
-00011cc0: 2064 6174 615f 7479 7065 3d22 666f 6c64   data_type="fold
-00011cd0: 6572 5f70 6174 6822 2c0a 2020 2020 290a  er_path",.    ).
-00011ce0: 2020 2020 696e 7075 745f 6672 616d 6573      input_frames
-00011cf0: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
-00011d00: 6f69 6e28 7072 6f6a 6563 745f 7061 7468  oin(project_path
-00011d10: 2c20 5061 7468 732e 494e 5055 545f 4652  , Paths.INPUT_FR
-00011d20: 414d 4553 5f44 4952 2e76 616c 7565 290a  AMES_DIR.value).
-00011d30: 2020 2020 6465 7374 696e 6174 696f 6e20      destination 
-00011d40: 3d20 6f73 2e70 6174 682e 6a6f 696e 2869  = os.path.join(i
-00011d50: 6e70 7574 5f66 7261 6d65 735f 6469 722c  nput_frames_dir,
-00011d60: 2069 6e70 7574 5f62 6173 656e 616d 6529   input_basename)
-00011d70: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-00011d80: 6973 6469 7228 6465 7374 696e 6174 696f  isdir(destinatio
-00011d90: 6e29 3a0a 2020 2020 2020 2020 7261 6973  n):.        rais
-00011da0: 6520 4469 7265 6374 6f72 7945 7869 7374  e DirectoryExist
-00011db0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00011dc0: 2020 206d 7367 3d66 2253 494d 4241 2045     msg=f"SIMBA E
-00011dd0: 5252 4f52 3a20 7b64 6573 7469 6e61 7469  RROR: {destinati
-00011de0: 6f6e 7d20 616c 7265 6164 7920 6578 6973  on} already exis
-00011df0: 7420 696e 2053 696d 4241 2070 726f 6a65  t in SimBA proje
-00011e00: 6374 2e22 2c0a 2020 2020 2020 2020 2020  ct.",.          
-00011e10: 2020 736f 7572 6365 3d63 6f70 795f 696d    source=copy_im
-00011e20: 675f 666f 6c64 6572 2e5f 5f6e 616d 655f  g_folder.__name_
-00011e30: 5f2c 0a20 2020 2020 2020 2029 0a20 2020  _,.        ).   
-00011e40: 2070 7269 6e74 2866 2249 6d70 6f72 7469   print(f"Importi
-00011e50: 6e67 2069 6d61 6765 2066 696c 6573 2066  ng image files f
-00011e60: 6f72 207b 696e 7075 745f 6261 7365 6e61  or {input_basena
-00011e70: 6d65 7d2e 2e2e 2229 0a20 2020 2073 6875  me}...").    shu
-00011e80: 7469 6c2e 636f 7079 7472 6565 2873 6f75  til.copytree(sou
-00011e90: 7263 652c 2064 6573 7469 6e61 7469 6f6e  rce, destination
-00011ea0: 290a 2020 2020 7469 6d65 722e 7374 6f70  ).    timer.stop
-00011eb0: 5f74 696d 6572 2829 0a20 2020 2073 7464  _timer().    std
-00011ec0: 6f75 745f 7375 6363 6573 7328 0a20 2020  out_success(.   
-00011ed0: 2020 2020 206d 7367 3d66 227b 6465 7374       msg=f"{dest
-00011ee0: 696e 6174 696f 6e7d 2069 6d70 6f72 7465  ination} importe
-00011ef0: 6420 746f 2053 696d 4241 2070 726f 6a65  d to SimBA proje
-00011f00: 6374 222c 0a20 2020 2020 2020 2065 6c61  ct",.        ela
-00011f10: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
-00011f20: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
-00011f30: 2c0a 2020 2020 2020 2020 736f 7572 6365  ,.        source
-00011f40: 3d63 6f70 795f 696d 675f 666f 6c64 6572  =copy_img_folder
-00011f50: 2e5f 5f6e 616d 655f 5f2c 0a20 2020 2029  .__name__,.    )
-00011f60: 0a0a 0a64 6566 2061 7070 656e 645f 6175  ...def append_au
-00011f70: 6469 6f28 0a20 2020 2076 6964 656f 5f70  dio(.    video_p
-00011f80: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00011f90: 6f73 2e50 6174 684c 696b 655d 2c0a 2020  os.PathLike],.  
-00011fa0: 2020 6175 6469 6f5f 7061 7468 3a20 556e    audio_path: Un
-00011fb0: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00011fc0: 4c69 6b65 5d2c 0a20 2020 2061 7564 696f  Like],.    audio
-00011fd0: 5f73 7263 5f74 7970 653a 204c 6974 6572  _src_type: Liter
-00011fe0: 616c 5b22 7669 6465 6f22 2c20 2261 7564  al["video", "aud
-00011ff0: 696f 225d 203d 2022 7669 6465 6f22 2c0a  io"] = "video",.
-00012000: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00012010: 2222 0a20 2020 2041 7070 656e 6420 6175  "".    Append au
-00012020: 6469 6f20 7472 6163 6b20 6672 6f6d 206f  dio track from o
-00012030: 6e65 2076 6964 656f 2074 6f20 616e 6f74  ne video to anot
-00012040: 6865 7220 7669 6465 6f20 7769 7468 6f75  her video withou
-00012050: 7420 616e 2061 7564 696f 2074 7261 636b  t an audio track
-00012060: 2e0a 0a20 2020 203a 7061 7261 6d20 556e  ...    :param Un
-00012070: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00012080: 4c69 6b65 5d20 7669 6465 6f5f 6f6e 655f  Like] video_one_
-00012090: 7061 7468 3a20 5061 7468 2074 6f20 7669  path: Path to vi
-000120a0: 6465 6f20 6669 6c65 2077 6974 686f 7574  deo file without
-000120b0: 2061 7564 696f 2074 7261 636b 2e0a 2020   audio track..  
-000120c0: 2020 3a70 6172 616d 2055 6e69 6f6e 5b73    :param Union[s
-000120d0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-000120e0: 2061 7564 696f 5f70 6174 683a 2050 6174   audio_path: Pat
-000120f0: 6820 746f 2066 696c 6520 2865 2e67 2e2c  h to file (e.g.,
-00012100: 2076 6964 656f 2920 7769 7468 2061 7564   video) with aud
-00012110: 696f 2074 7261 636b 2e0a 2020 2020 3a70  io track..    :p
-00012120: 6172 616d 204c 6974 6572 616c 5b27 7669  aram Literal['vi
-00012130: 6465 6f27 2c20 2761 7564 696f 275d 2061  deo', 'audio'] a
-00012140: 7564 696f 5f73 7263 5f74 7970 653a 2054  udio_src_type: T
-00012150: 7970 6520 6f66 2061 7564 696f 2073 6f75  ype of audio sou
-00012160: 7263 6520 6f66 2022 7669 6465 6f5f 7477  rce of "video_tw
-00012170: 6f5f 7061 7468 2220 2865 2e67 2e2c 2076  o_path" (e.g., v
-00012180: 6964 656f 206f 7220 6175 6469 6f20 6669  ideo or audio fi
-00012190: 6c65 292e 0a0a 2020 2020 3a65 7861 6d70  le)...    :examp
-000121a0: 6c65 3a0a 2020 2020 3e3e 3e20 6170 7065  le:.    >>> appe
-000121b0: 6e64 5f61 7564 696f 2876 6964 656f 5f70  nd_audio(video_p
-000121c0: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
-000121d0: 6e2f 4465 736b 746f 702f 656e 7673 2f74  n/Desktop/envs/t
-000121e0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f74  roubleshooting/t
-000121f0: 776f 5f62 6c61 636b 5f61 6e69 6d61 6c73  wo_black_animals
-00012200: 5f31 3462 702f 7072 6f6a 6563 745f 666f  _14bp/project_fo
-00012210: 6c64 6572 2f76 6964 656f 732f 6d65 7267  lder/videos/merg
-00012220: 6564 5f76 6964 656f 5f32 3032 3330 3432  ed_video_2023042
-00012230: 3532 3031 3633 372e 6d70 3427 2c0a 2020  5201637.mp4',.  
-00012240: 2020 3e3e 3e20 6175 6469 6f5f 7061 7468    >>> audio_path
-00012250: 3d22 2f55 7365 7273 2f73 696d 6f6e 2f44  ="/Users/simon/D
-00012260: 6f63 756d 656e 7473 2f5a 6f6f 6d2f 6464  ocuments/Zoom/dd
-00012270: 642f 7669 6465 6f31 3138 3037 3332 3233  d/video118073223
-00012280: 332e 6d70 3422 290a 2020 2020 2222 220a  3.mp4").    """.
-00012290: 0a20 2020 2069 6620 6e6f 7420 6368 6563  .    if not chec
-000122a0: 6b5f 6666 6d70 6567 5f61 7661 696c 6162  k_ffmpeg_availab
-000122b0: 6c65 2829 3a0a 2020 2020 2020 2020 7261  le():.        ra
-000122c0: 6973 6520 4646 4d50 4547 4e6f 7446 6f75  ise FFMPEGNotFou
-000122d0: 6e64 4572 726f 7228 0a20 2020 2020 2020  ndError(.       
-000122e0: 2020 2020 206d 7367 3d22 4646 4d70 6567       msg="FFMpeg
-000122f0: 206e 6f74 2066 6f75 6e64 206f 6e20 636f   not found on co
-00012300: 6d70 7574 6572 2e20 5365 6520 5369 6d42  mputer. See SimB
-00012310: 4120 646f 6373 2066 6f72 2069 6e73 7461  A docs for insta
-00012320: 6c6c 2069 6e73 7472 7563 7469 6f6e 732e  ll instructions.
-00012330: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00012340: 6f75 7263 653d 6170 7065 6e64 5f61 7564  ource=append_aud
-00012350: 696f 2e5f 5f6e 616d 655f 5f2c 0a20 2020  io.__name__,.   
-00012360: 2020 2020 2029 0a20 2020 2063 6865 636b       ).    check
-00012370: 5f66 696c 655f 6578 6973 745f 616e 645f  _file_exist_and_
-00012380: 7265 6164 6162 6c65 2866 696c 655f 7061  readable(file_pa
-00012390: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
-000123a0: 2020 2063 6865 636b 5f66 696c 655f 6578     check_file_ex
-000123b0: 6973 745f 616e 645f 7265 6164 6162 6c65  ist_and_readable
-000123c0: 2866 696c 655f 7061 7468 3d61 7564 696f  (file_path=audio
-000123d0: 5f70 6174 6829 0a20 2020 2076 6964 656f  _path).    video
-000123e0: 5f6d 6574 615f 6461 7461 203d 2067 6574  _meta_data = get
-000123f0: 5f76 6964 656f 5f6d 6574 615f 6461 7461  _video_meta_data
-00012400: 2876 6964 656f 5f70 6174 683d 7669 6465  (video_path=vide
-00012410: 6f5f 7061 7468 290a 2020 2020 6175 6469  o_path).    audi
-00012420: 6f5f 7372 635f 6d65 7461 5f64 6174 6120  o_src_meta_data 
-00012430: 3d20 6765 745f 7669 6465 6f5f 6d65 7461  = get_video_meta
-00012440: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
-00012450: 3d61 7564 696f 5f70 6174 6829 0a20 2020  =audio_path).   
-00012460: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
-00012470: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00012480: 2020 206f 732e 7061 7468 2e64 6972 6e61     os.path.dirna
-00012490: 6d65 2876 6964 656f 5f70 6174 6829 2c20  me(video_path), 
-000124a0: 6765 745f 666e 5f65 7874 2866 696c 6570  get_fn_ext(filep
-000124b0: 6174 683d 7669 6465 6f5f 7061 7468 295b  ath=video_path)[
-000124c0: 315d 202b 2022 5f77 5f61 7564 696f 2e6d  1] + "_w_audio.m
-000124d0: 7034 220a 2020 2020 290a 2020 2020 636d  p4".    ).    cm
-000124e0: 6420 3d20 5b0a 2020 2020 2020 2020 2266  d = [.        "f
-000124f0: 6670 726f 6265 222c 0a20 2020 2020 2020  fprobe",.       
-00012500: 2022 2d76 222c 0a20 2020 2020 2020 2022   "-v",.        "
-00012510: 6572 726f 7222 2c0a 2020 2020 2020 2020  error",.        
-00012520: 222d 7365 6c65 6374 5f73 7472 6561 6d73  "-select_streams
-00012530: 222c 0a20 2020 2020 2020 2022 613a 3022  ",.        "a:0"
-00012540: 2c0a 2020 2020 2020 2020 222d 7368 6f77  ,.        "-show
-00012550: 5f65 6e74 7269 6573 222c 0a20 2020 2020  _entries",.     
-00012560: 2020 2022 7374 7265 616d 3d63 6f64 6563     "stream=codec
-00012570: 5f6e 616d 6522 2c0a 2020 2020 2020 2020  _name",.        
-00012580: 222d 6f66 222c 0a20 2020 2020 2020 2022  "-of",.        "
-00012590: 6465 6661 756c 743d 6e6f 7072 696e 745f  default=noprint_
-000125a0: 7772 6170 7065 7273 3d31 3a6e 6f6b 6579  wrappers=1:nokey
-000125b0: 3d31 222c 0a20 2020 2020 2020 2061 7564  =1",.        aud
-000125c0: 696f 5f70 6174 682c 0a20 2020 205d 0a20  io_path,.    ]. 
-000125d0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000125e0: 7472 6163 6b5f 7479 7065 203d 2028 0a20  track_type = (. 
-000125f0: 2020 2020 2020 2020 2020 2073 7562 7072             subpr
-00012600: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-00012610: 7574 2863 6d64 2c20 7374 6465 7272 3d73  ut(cmd, stderr=s
-00012620: 7562 7072 6f63 6573 732e 5354 444f 5554  ubprocess.STDOUT
-00012630: 290a 2020 2020 2020 2020 2020 2020 2e64  ).            .d
-00012640: 6563 6f64 6528 2275 7466 2d38 2229 0a20  ecode("utf-8"). 
-00012650: 2020 2020 2020 2020 2020 202e 7374 7269             .stri
-00012660: 7028 290a 2020 2020 2020 2020 290a 2020  p().        ).  
-00012670: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
-00012680: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
-00012690: 7345 7272 6f72 3a0a 2020 2020 2020 2020  sError:.        
-000126a0: 7261 6973 6520 4e6f 4461 7461 4572 726f  raise NoDataErro
-000126b0: 7228 0a20 2020 2020 2020 2020 2020 206d  r(.            m
-000126c0: 7367 3d66 224e 6f20 6175 6469 6f20 7472  sg=f"No audio tr
-000126d0: 6163 6b20 666f 756e 6420 696e 2066 696c  ack found in fil
-000126e0: 6520 7b61 7564 696f 5f70 6174 687d 222c  e {audio_path}",
-000126f0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-00012700: 7263 653d 6170 7065 6e64 5f61 7564 696f  rce=append_audio
-00012710: 2e5f 5f6e 616d 655f 5f2c 0a20 2020 2020  .__name__,.     
-00012720: 2020 2029 0a0a 2020 2020 6966 2076 6964     )..    if vid
-00012730: 656f 5f6d 6574 615f 6461 7461 5b22 6672  eo_meta_data["fr
-00012740: 616d 655f 636f 756e 7422 5d20 213d 2061  ame_count"] != a
-00012750: 7564 696f 5f73 7263 5f6d 6574 615f 6461  udio_src_meta_da
-00012760: 7461 5b22 6672 616d 655f 636f 756e 7422  ta["frame_count"
-00012770: 5d3a 0a20 2020 2020 2020 2049 6e56 616c  ]:.        InVal
-00012780: 6964 5573 6572 496e 7075 7457 6172 6e69  idUserInputWarni
-00012790: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-000127a0: 6d73 673d 6627 5468 6520 7669 6465 6f20  msg=f'The video 
-000127b0: 287b 7669 6465 6f5f 6d65 7461 5f64 6174  ({video_meta_dat
-000127c0: 615b 2266 7261 6d65 5f63 6f75 6e74 225d  a["frame_count"]
-000127d0: 7d29 2061 6e64 2061 7564 696f 2073 6f75  }) and audio sou
-000127e0: 7263 6520 287b 6175 6469 6f5f 7372 635f  rce ({audio_src_
-000127f0: 6d65 7461 5f64 6174 615b 2266 7261 6d65  meta_data["frame
-00012800: 5f63 6f75 6e74 225d 7d29 2064 6f65 7320  _count"]}) does 
-00012810: 6e6f 7420 6861 7665 2061 6e20 6571 7561  not have an equa
-00012820: 6c20 6e75 6d62 6572 206f 6620 6672 616d  l number of fram
-00012830: 6573 2e27 2c0a 2020 2020 2020 2020 2020  es.',.          
-00012840: 2020 736f 7572 6365 3d61 7070 656e 645f    source=append_
-00012850: 6175 6469 6f2e 5f5f 6e61 6d65 5f5f 2c0a  audio.__name__,.
-00012860: 2020 2020 2020 2020 290a 0a20 2020 2063          )..    c
-00012870: 6d64 203d 2066 2766 666d 7065 6720 2d69  md = f'ffmpeg -i
-00012880: 2022 7b76 6964 656f 5f70 6174 687d 2220   "{video_path}" 
-00012890: 2d69 2022 7b61 7564 696f 5f70 6174 687d  -i "{audio_path}
-000128a0: 2220 2d63 3a76 2063 6f70 7920 2d6d 6170  " -c:v copy -map
-000128b0: 2030 3a76 3a30 202d 6d61 7020 313a 613a   0:v:0 -map 1:a:
-000128c0: 3020 227b 7361 7665 5f70 6174 687d 2220  0 "{save_path}" 
-000128d0: 2d79 270a 0a20 2020 2074 7279 3a0a 2020  -y'..    try:.  
-000128e0: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
-000128f0: 2e72 756e 2863 6d64 2c20 7368 656c 6c3d  .run(cmd, shell=
-00012900: 5472 7565 2c20 6368 6563 6b3d 5472 7565  True, check=True
-00012910: 290a 2020 2020 6578 6365 7074 2073 7562  ).    except sub
-00012920: 7072 6f63 6573 732e 4361 6c6c 6564 5072  process.CalledPr
-00012930: 6f63 6573 7345 7272 6f72 2061 7320 653a  ocessError as e:
-00012940: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00012950: 4572 726f 723a 222c 2065 290a 0a20 2020  Error:", e)..   
-00012960: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
-00012970: 0a20 2020 2020 2020 206d 7367 3d66 2241  .        msg=f"A
-00012980: 7564 696f 206d 6572 6765 6420 7375 6363  udio merged succ
-00012990: 6573 7366 756c 6c79 2c20 6669 6c65 2073  essfully, file s
-000129a0: 6176 6564 2061 7420 7b73 6176 655f 7061  aved at {save_pa
-000129b0: 7468 7d21 222c 0a20 2020 2020 2020 2073  th}!",.        s
-000129c0: 6f75 7263 653d 6170 7065 6e64 5f61 7564  ource=append_aud
-000129d0: 696f 2e5f 5f6e 616d 655f 5f2c 0a20 2020  io.__name__,.   
-000129e0: 2029 0a0a 0a64 6566 2063 726f 705f 7369   )...def crop_si
-000129f0: 6e67 6c65 5f76 6964 656f 5f63 6972 636c  ngle_video_circl
-00012a00: 6528 6669 6c65 5f70 6174 683a 2055 6e69  e(file_path: Uni
-00012a10: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00012a20: 696b 655d 2920 2d3e 204e 6f6e 653a 0a20  ike]) -> None:. 
-00012a30: 2020 2022 2222 0a20 2020 2043 726f 7020     """.    Crop 
-00012a40: 6120 7669 6465 6f20 6261 7365 6420 6f6e  a video based on
-00012a50: 2063 6972 6375 6c61 7220 7265 6769 6f6e   circular region
-00012a60: 7320 6f66 2069 6e74 6572 6573 7420 2852  s of interest (R
-00012a70: 4f49 7329 2073 656c 6563 7465 6420 6279  OIs) selected by
-00012a80: 2074 6865 2075 7365 722e 0a0a 2020 2020   the user...    
-00012a90: 3a70 6172 616d 2020 556e 696f 6e5b 7374  :param  Union[st
-00012aa0: 722c 206f 732e 5061 7468 4c69 6b65 5d20  r, os.PathLike] 
-00012ab0: 6669 6c65 5f70 6174 683a 2054 6865 2070  file_path: The p
-00012ac0: 6174 6820 746f 2074 6865 2069 6e70 7574  ath to the input
-00012ad0: 2076 6964 656f 2066 696c 652e 0a0a 2020   video file...  
-00012ae0: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
-00012af0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
-00012b00: 2063 726f 7073 2074 6865 2069 6e70 7574   crops the input
-00012b10: 2076 6964 656f 2062 6173 6564 206f 6e20   video based on 
-00012b20: 6369 7263 756c 6172 2072 6567 696f 6e73  circular regions
-00012b30: 206f 6620 696e 7465 7265 7374 2028 524f   of interest (RO
-00012b40: 4973 2920 7365 6c65 6374 6564 2062 7920  Is) selected by 
-00012b50: 7468 6520 7573 6572 2e0a 2020 2020 2020  the user..      
-00012b60: 2054 6865 2075 7365 7220 6973 2070 726f   The user is pro
-00012b70: 6d70 7465 6420 746f 2073 656c 6563 7420  mpted to select 
-00012b80: 6120 6369 7263 756c 6172 2052 4f49 206f  a circular ROI o
-00012b90: 6e20 7468 6520 7669 6465 6f20 6672 616d  n the video fram
-00012ba0: 652c 2061 6e64 2074 6865 2066 756e 6374  e, and the funct
-00012bb0: 696f 6e20 7468 656e 2063 726f 7073 2074  ion then crops t
-00012bc0: 6865 2076 6964 656f 0a20 2020 2020 2020  he video.       
-00012bd0: 6261 7365 6420 6f6e 2074 6865 2073 656c  based on the sel
-00012be0: 6563 7465 6420 524f 492e 2054 6865 2063  ected ROI. The c
-00012bf0: 726f 7070 6564 2076 6964 656f 2069 7320  ropped video is 
-00012c00: 7361 7665 6420 7769 7468 2022 5f63 6972  saved with "_cir
-00012c10: 636c 655f 6372 6f70 7065 6422 2073 7566  cle_cropped" suf
-00012c20: 6669 7820 696e 2074 6865 2073 616d 6520  fix in the same 
-00012c30: 6469 7265 6374 6f72 790a 2020 2020 2020  directory.      
-00012c40: 2061 7320 7468 6520 696e 7075 7420 7669   as the input vi
-00012c50: 6465 6f20 6669 6c65 2e0a 0a20 2020 203a  deo file...    :
-00012c60: 6578 616d 706c 653a 0a20 2020 203e 3e3e  example:.    >>>
-00012c70: 2063 726f 705f 7369 6e67 6c65 5f76 6964   crop_single_vid
-00012c80: 656f 5f63 6972 636c 6528 6669 6c65 5f70  eo_circle(file_p
-00012c90: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
-00012ca0: 6e2f 4465 736b 746f 702f 4147 4752 4553  n/Desktop/AGGRES
-00012cb0: 5349 5649 5459 5f34 5f31 315f 3231 5f54  SIVITY_4_11_21_T
-00012cc0: 7269 616c 5f32 5f63 616d 6572 6131 5f72  rial_2_camera1_r
-00012cd0: 6f74 6174 6564 5f32 3032 3430 3231 3131  otated_202402111
-00012ce0: 3433 3335 352e 6d70 3427 290a 2020 2020  43355.mp4').    
-00012cf0: 2222 220a 0a20 2020 2064 6972 2c20 7669  """..    dir, vi
-00012d00: 6465 6f5f 6e61 6d65 2c20 5f20 3d20 6765  deo_name, _ = ge
-00012d10: 745f 666e 5f65 7874 2866 696c 6570 6174  t_fn_ext(filepat
-00012d20: 683d 6669 6c65 5f70 6174 6829 0a20 2020  h=file_path).   
-00012d30: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
-00012d40: 7061 7468 2e6a 6f69 6e28 6469 722c 2066  path.join(dir, f
-00012d50: 227b 7669 6465 6f5f 6e61 6d65 7d5f 6369  "{video_name}_ci
-00012d60: 7263 6c65 5f63 726f 7070 6564 2e6d 7034  rcle_cropped.mp4
-00012d70: 2229 0a20 2020 2076 6964 656f 5f6d 6574  ").    video_met
-00012d80: 615f 6461 7461 203d 2067 6574 5f76 6964  a_data = get_vid
-00012d90: 656f 5f6d 6574 615f 6461 7461 2876 6964  eo_meta_data(vid
-00012da0: 656f 5f70 6174 683d 6669 6c65 5f70 6174  eo_path=file_pat
-00012db0: 6829 0a20 2020 2063 6865 636b 5f66 696c  h).    check_fil
-00012dc0: 655f 6578 6973 745f 616e 645f 7265 6164  e_exist_and_read
-00012dd0: 6162 6c65 2866 696c 655f 7061 7468 3d66  able(file_path=f
-00012de0: 696c 655f 7061 7468 290a 2020 2020 6369  ile_path).    ci
-00012df0: 7263 6c65 5f73 656c 6563 746f 7220 3d20  rcle_selector = 
-00012e00: 524f 4953 656c 6563 746f 7243 6972 636c  ROISelectorCircl
-00012e10: 6528 7061 7468 3d66 696c 655f 7061 7468  e(path=file_path
-00012e20: 290a 2020 2020 6369 7263 6c65 5f73 656c  ).    circle_sel
-00012e30: 6563 746f 722e 7275 6e28 290a 2020 2020  ector.run().    
-00012e40: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
-00012e50: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
-00012e60: 2020 2072 203d 2063 6972 636c 655f 7365     r = circle_se
-00012e70: 6c65 6374 6f72 2e63 6972 636c 655f 7261  lector.circle_ra
-00012e80: 6469 7573 0a20 2020 2078 2c20 7920 3d20  dius.    x, y = 
-00012e90: 6369 7263 6c65 5f73 656c 6563 746f 722e  circle_selector.
-00012ea0: 6369 7263 6c65 5f63 656e 7465 725b 305d  circle_center[0]
-00012eb0: 2c20 6369 7263 6c65 5f73 656c 6563 746f  , circle_selecto
-00012ec0: 722e 6369 7263 6c65 5f63 656e 7465 725b  r.circle_center[
-00012ed0: 315d 0a20 2020 2070 6f6c 7967 6f6e 203d  1].    polygon =
-00012ee0: 2050 6f6c 7967 6f6e 280a 2020 2020 2020   Polygon(.      
-00012ef0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00012f00: 2878 202b 2072 202a 206e 702e 636f 7328  (x + r * np.cos(
-00012f10: 616e 676c 6529 2c20 7920 2b20 7220 2a20  angle), y + r * 
-00012f20: 6e70 2e73 696e 2861 6e67 6c65 2929 0a20  np.sin(angle)). 
-00012f30: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-00012f40: 6e67 6c65 2069 6e20 6e70 2e6c 696e 7370  ngle in np.linsp
-00012f50: 6163 6528 302c 2032 202a 206e 702e 7069  ace(0, 2 * np.pi
-00012f60: 2c20 3130 3029 0a20 2020 2020 2020 205d  , 100).        ]
-00012f70: 0a20 2020 2029 0a20 2020 2070 6f6c 7967  .    ).    polyg
-00012f80: 6f6e 7320 3d20 5b70 6f6c 7967 6f6e 2066  ons = [polygon f
-00012f90: 6f72 2078 2069 6e20 7261 6e67 6528 7669  or x in range(vi
-00012fa0: 6465 6f5f 6d65 7461 5f64 6174 615b 2266  deo_meta_data["f
-00012fb0: 7261 6d65 5f63 6f75 6e74 225d 295d 0a20  rame_count"])]. 
-00012fc0: 2020 2069 6620 2870 6c61 7466 6f72 6d2e     if (platform.
-00012fd0: 7379 7374 656d 2829 203d 3d20 2244 6172  system() == "Dar
-00012fe0: 7769 6e22 2920 616e 6420 286d 756c 7469  win") and (multi
-00012ff0: 7072 6f63 6573 7369 6e67 2e67 6574 5f73  processing.get_s
-00013000: 7461 7274 5f6d 6574 686f 6428 2920 6973  tart_method() is
-00013010: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00013020: 6d75 6c74 6970 726f 6365 7373 696e 672e  multiprocessing.
-00013030: 7365 745f 7374 6172 745f 6d65 7468 6f64  set_start_method
-00013040: 2822 7370 6177 6e22 2c20 666f 7263 653d  ("spawn", force=
-00013050: 5472 7565 290a 2020 2020 706f 6c79 676f  True).    polygo
-00013060: 6e73 203d 2049 6d61 6765 4d69 7869 6e28  ns = ImageMixin(
-00013070: 292e 736c 6963 655f 7368 6170 6573 5f69  ).slice_shapes_i
-00013080: 6e5f 696d 6773 280a 2020 2020 2020 2020  n_imgs(.        
-00013090: 696d 6773 3d66 696c 655f 7061 7468 2c20  imgs=file_path, 
-000130a0: 7368 6170 6573 3d70 6f6c 7967 6f6e 732c  shapes=polygons,
-000130b0: 2076 6572 626f 7365 3d46 616c 7365 0a20   verbose=False. 
-000130c0: 2020 2029 0a20 2020 2074 696d 652e 736c     ).    time.sl
-000130d0: 6565 7028 3329 0a20 2020 205f 203d 2049  eep(3).    _ = I
-000130e0: 6d61 6765 4d69 7869 6e2e 696d 675f 7374  mageMixin.img_st
-000130f0: 6163 6b5f 746f 5f76 6964 656f 280a 2020  ack_to_video(.  
-00013100: 2020 2020 2020 696d 6773 3d70 6f6c 7967        imgs=polyg
-00013110: 6f6e 732c 2073 6176 655f 7061 7468 3d73  ons, save_path=s
-00013120: 6176 655f 7061 7468 2c20 6670 733d 7669  ave_path, fps=vi
-00013130: 6465 6f5f 6d65 7461 5f64 6174 615b 2266  deo_meta_data["f
-00013140: 7073 225d 0a20 2020 2029 0a20 2020 2074  ps"].    ).    t
-00013150: 696d 6572 2e73 746f 705f 7469 6d65 7228  imer.stop_timer(
-00013160: 290a 2020 2020 7374 646f 7574 5f73 7563  ).    stdout_suc
-00013170: 6365 7373 280a 2020 2020 2020 2020 6d73  cess(.        ms
-00013180: 673d 6622 4369 7263 6c65 2d62 6173 6564  g=f"Circle-based
-00013190: 2063 726f 7070 6564 2073 6176 6564 2061   cropped saved a
-000131a0: 7420 746f 207b 7361 7665 5f70 6174 687d  t to {save_path}
-000131b0: 222c 0a20 2020 2020 2020 2065 6c61 7073  ",.        elaps
-000131c0: 6564 5f74 696d 653d 7469 6d65 722e 656c  ed_time=timer.el
-000131d0: 6170 7365 645f 7469 6d65 5f73 7472 2c0a  apsed_time_str,.
-000131e0: 2020 2020 290a 0a0a 6465 6620 6372 6f70      )...def crop
-000131f0: 5f6d 756c 7469 706c 655f 7669 6465 6f73  _multiple_videos
-00013200: 5f63 6972 636c 6573 280a 2020 2020 696e  _circles(.    in
-00013210: 5f64 6972 3a20 556e 696f 6e5b 7374 722c  _dir: Union[str,
-00013220: 206f 732e 5061 7468 4c69 6b65 5d2c 206f   os.PathLike], o
-00013230: 7574 5f64 6972 3a20 556e 696f 6e5b 7374  ut_dir: Union[st
-00013240: 722c 206f 732e 5061 7468 4c69 6b65 5d0a  r, os.PathLike].
-00013250: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00013260: 2222 0a20 2020 2043 726f 7020 6d75 6c74  "".    Crop mult
-00013270: 6970 6c65 2076 6964 656f 7320 6261 7365  iple videos base
-00013280: 6420 6f6e 2063 6972 6375 6c61 7220 7265  d on circular re
-00013290: 6769 6f6e 7320 6f66 2069 6e74 6572 6573  gions of interes
-000132a0: 7420 2852 4f49 7329 2073 656c 6563 7465  t (ROIs) selecte
-000132b0: 6420 6279 2074 6865 2075 7365 722e 0a0a  d by the user...
-000132c0: 2020 2020 3a70 6172 616d 2020 556e 696f      :param  Unio
-000132d0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-000132e0: 6b65 5d20 696e 5f64 6972 3a20 5468 6520  ke] in_dir: The 
-000132f0: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
-00013300: 6e69 6e67 2069 6e70 7574 2076 6964 656f  ning input video
-00013310: 2066 696c 6573 2e0a 2020 2020 3a70 6172   files..    :par
-00013320: 616d 2020 556e 696f 6e5b 7374 722c 206f  am  Union[str, o
-00013330: 732e 5061 7468 4c69 6b65 5d20 6f75 745f  s.PathLike] out_
-00013340: 6469 723a 2054 6865 2064 6972 6563 746f  dir: The directo
-00013350: 7279 2074 6f20 7361 7665 2074 6865 2063  ry to save the c
-00013360: 726f 7070 6564 2076 6964 656f 2066 696c  ropped video fil
-00013370: 6573 2e0a 0a20 2020 202e 2e20 6e6f 7465  es...    .. note
-00013380: 3a3a 0a20 2020 2020 2020 5468 6973 2066  ::.       This f
-00013390: 756e 6374 696f 6e20 6372 6f70 7320 6d75  unction crops mu
-000133a0: 6c74 6970 6c65 2076 6964 656f 7320 6261  ltiple videos ba
-000133b0: 7365 6420 6f6e 2063 6972 6375 6c61 7220  sed on circular 
-000133c0: 524f 4973 2073 656c 6563 7465 6420 6279  ROIs selected by
-000133d0: 2074 6865 2075 7365 722e 0a20 2020 2020   the user..     
-000133e0: 2020 5468 6520 7573 6572 2069 7320 6173    The user is as
-000133f0: 6b65 6420 746f 2064 6566 696e 6520 6120  ked to define a 
-00013400: 6369 7263 6c65 206d 616e 7561 6c6c 7920  circle manually 
-00013410: 696e 206f 6e65 2076 6964 656f 2077 6974  in one video wit
-00013420: 6869 6e20 7468 6520 696e 7075 7420 6469  hin the input di
-00013430: 7265 6374 6f72 792e 0a20 2020 2020 2020  rectory..       
-00013440: 5468 6520 6675 6e63 7469 6f6e 2074 6865  The function the
-00013450: 6e20 6372 6f70 7320 616c 6c20 7468 6520  n crops all the 
-00013460: 7669 6465 6f20 696e 2074 6865 2069 6e70  video in the inp
-00013470: 7574 2064 6972 6563 746f 7279 2061 6363  ut directory acc
-00013480: 6f72 6469 6e67 2074 6f20 7468 6520 7368  ording to the sh
-00013490: 6170 6520 6465 6669 6e65 640a 2020 2020  ape defined.    
-000134a0: 2020 2075 7369 6e67 2074 6865 2066 6972     using the fir
-000134b0: 7374 2076 6964 656f 2061 6e64 2073 6176  st video and sav
-000134c0: 6573 2074 6865 2076 6964 656f 7320 696e  es the videos in
-000134d0: 2074 6865 2060 606f 7574 5f64 6972 6060   the ``out_dir``
-000134e0: 2077 6974 6820 7468 6520 7361 6d65 2066   with the same f
-000134f0: 696c 656e 616d 6573 2061 7320 7468 6520  ilenames as the 
-00013500: 6f72 6967 696e 616c 2076 6964 656f 732e  original videos.
-00013510: 2e0a 0a20 2020 203a 6578 616d 706c 653a  ...    :example:
-00013520: 0a20 2020 203e 3e3e 2063 726f 705f 6d75  .    >>> crop_mu
-00013530: 6c74 6970 6c65 5f76 6964 656f 735f 6369  ltiple_videos_ci
-00013540: 7263 6c65 7328 696e 5f64 6972 3d27 2f55  rcles(in_dir='/U
-00013550: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-00013560: 6f70 2f65 6469 7465 642f 7465 7374 7327  op/edited/tests'
-00013570: 2c20 6f75 745f 6469 723d 272f 5573 6572  , out_dir='/User
-00013580: 732f 7369 6d6f 6e2f 4465 736b 746f 7027  s/simon/Desktop'
-00013590: 290a 2020 2020 2222 220a 0a20 2020 2063  ).    """..    c
-000135a0: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
-000135b0: 7473 2869 6e5f 6469 723d 696e 5f64 6972  ts(in_dir=in_dir
-000135c0: 290a 2020 2020 6368 6563 6b5f 6966 5f64  ).    check_if_d
-000135d0: 6972 5f65 7869 7374 7328 696e 5f64 6972  ir_exists(in_dir
-000135e0: 3d6f 7574 5f64 6972 290a 2020 2020 7669  =out_dir).    vi
-000135f0: 6465 6f5f 6669 6c65 7320 3d20 6669 6e64  deo_files = find
-00013600: 5f61 6c6c 5f76 6964 656f 735f 696e 5f64  _all_videos_in_d
-00013610: 6972 6563 746f 7279 2864 6972 6563 746f  irectory(directo
-00013620: 7279 3d69 6e5f 6469 7229 0a20 2020 2063  ry=in_dir).    c
-00013630: 6972 636c 655f 7365 6c65 6374 6f72 203d  ircle_selector =
-00013640: 2052 4f49 5365 6c65 6374 6f72 4369 7263   ROISelectorCirc
-00013650: 6c65 2870 6174 683d 6f73 2e70 6174 682e  le(path=os.path.
-00013660: 6a6f 696e 2869 6e5f 6469 722c 2076 6964  join(in_dir, vid
-00013670: 656f 5f66 696c 6573 5b30 5d29 290a 2020  eo_files[0])).  
-00013680: 2020 6369 7263 6c65 5f73 656c 6563 746f    circle_selecto
-00013690: 722e 7275 6e28 290a 2020 2020 7220 3d20  r.run().    r = 
-000136a0: 6369 7263 6c65 5f73 656c 6563 746f 722e  circle_selector.
-000136b0: 6369 7263 6c65 5f72 6164 6975 730a 2020  circle_radius.  
-000136c0: 2020 782c 2079 203d 2063 6972 636c 655f    x, y = circle_
-000136d0: 7365 6c65 6374 6f72 2e63 6972 636c 655f  selector.circle_
-000136e0: 6365 6e74 6572 5b30 5d2c 2063 6972 636c  center[0], circl
-000136f0: 655f 7365 6c65 6374 6f72 2e63 6972 636c  e_selector.circl
-00013700: 655f 6365 6e74 6572 5b31 5d0a 2020 2020  e_center[1].    
-00013710: 706f 6c79 676f 6e20 3d20 506f 6c79 676f  polygon = Polygo
-00013720: 6e28 0a20 2020 2020 2020 205b 0a20 2020  n(.        [.   
-00013730: 2020 2020 2020 2020 2028 7820 2b20 7220           (x + r 
-00013740: 2a20 6e70 2e63 6f73 2861 6e67 6c65 292c  * np.cos(angle),
-00013750: 2079 202b 2072 202a 206e 702e 7369 6e28   y + r * np.sin(
-00013760: 616e 676c 6529 290a 2020 2020 2020 2020  angle)).        
-00013770: 2020 2020 666f 7220 616e 676c 6520 696e      for angle in
-00013780: 206e 702e 6c69 6e73 7061 6365 2830 2c20   np.linspace(0, 
-00013790: 3220 2a20 6e70 2e70 692c 2031 3030 290a  2 * np.pi, 100).
-000137a0: 2020 2020 2020 2020 5d0a 2020 2020 290a          ].    ).
-000137b0: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
-000137c0: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
-000137d0: 6529 0a20 2020 2069 6620 2870 6c61 7466  e).    if (platf
-000137e0: 6f72 6d2e 7379 7374 656d 2829 203d 3d20  orm.system() == 
-000137f0: 2244 6172 7769 6e22 2920 616e 6420 286d  "Darwin") and (m
-00013800: 756c 7469 7072 6f63 6573 7369 6e67 2e67  ultiprocessing.g
-00013810: 6574 5f73 7461 7274 5f6d 6574 686f 6428  et_start_method(
-00013820: 2920 6973 204e 6f6e 6529 3a0a 2020 2020  ) is None):.    
-00013830: 2020 2020 6d75 6c74 6970 726f 6365 7373      multiprocess
-00013840: 696e 672e 7365 745f 7374 6172 745f 6d65  ing.set_start_me
-00013850: 7468 6f64 2822 7370 6177 6e22 2c20 666f  thod("spawn", fo
-00013860: 7263 653d 4661 6c73 6529 0a20 2020 2066  rce=False).    f
-00013870: 6f72 2076 6964 656f 5f63 6e74 2c20 7669  or video_cnt, vi
-00013880: 6465 6f5f 7061 7468 2069 6e20 656e 756d  deo_path in enum
-00013890: 6572 6174 6528 7669 6465 6f5f 6669 6c65  erate(video_file
-000138a0: 7329 3a0a 2020 2020 2020 2020 7072 696e  s):.        prin
-000138b0: 7428 0a20 2020 2020 2020 2020 2020 2066  t(.            f
-000138c0: 2243 6972 636c 6520 6372 6f70 7069 6e67  "Circle cropping
-000138d0: 2076 6964 656f 207b 7669 6465 6f5f 7061   video {video_pa
-000138e0: 7468 7d20 287b 7669 6465 6f5f 636e 742b  th} ({video_cnt+
-000138f0: 317d 2f7b 6c65 6e28 7669 6465 6f5f 6669  1}/{len(video_fi
-00013900: 6c65 7329 7d29 2e2e 2e22 0a20 2020 2020  les)})...".     
-00013910: 2020 2029 0a20 2020 2020 2020 2076 6964     ).        vid
-00013920: 656f 5f70 6174 6820 3d20 6f73 2e70 6174  eo_path = os.pat
-00013930: 682e 6a6f 696e 2869 6e5f 6469 722c 2076  h.join(in_dir, v
-00013940: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
-00013950: 2020 205f 2c20 7669 6465 6f5f 6e61 6d65     _, video_name
-00013960: 2c20 5f20 3d20 6765 745f 666e 5f65 7874  , _ = get_fn_ext
-00013970: 2866 696c 6570 6174 683d 7669 6465 6f5f  (filepath=video_
-00013980: 7061 7468 290a 2020 2020 2020 2020 7361  path).        sa
-00013990: 7665 5f70 6174 6820 3d20 6f73 2e70 6174  ve_path = os.pat
-000139a0: 682e 6a6f 696e 286f 7574 5f64 6972 2c20  h.join(out_dir, 
-000139b0: 6622 7b76 6964 656f 5f6e 616d 657d 2e6d  f"{video_name}.m
-000139c0: 7034 2229 0a20 2020 2020 2020 2076 6964  p4").        vid
-000139d0: 656f 5f6d 6574 615f 6461 7461 203d 2067  eo_meta_data = g
-000139e0: 6574 5f76 6964 656f 5f6d 6574 615f 6461  et_video_meta_da
-000139f0: 7461 2876 6964 656f 5f70 6174 683d 7669  ta(video_path=vi
-00013a00: 6465 6f5f 7061 7468 290a 2020 2020 2020  deo_path).      
-00013a10: 2020 706f 6c79 676f 6e73 203d 205b 706f    polygons = [po
-00013a20: 6c79 676f 6e20 666f 7220 7820 696e 2072  lygon for x in r
-00013a30: 616e 6765 2876 6964 656f 5f6d 6574 615f  ange(video_meta_
-00013a40: 6461 7461 5b22 6672 616d 655f 636f 756e  data["frame_coun
-00013a50: 7422 5d29 5d0a 2020 2020 2020 2020 706f  t"])].        po
-00013a60: 6c79 676f 6e73 203d 2049 6d61 6765 4d69  lygons = ImageMi
-00013a70: 7869 6e28 292e 736c 6963 655f 7368 6170  xin().slice_shap
-00013a80: 6573 5f69 6e5f 696d 6773 280a 2020 2020  es_in_imgs(.    
-00013a90: 2020 2020 2020 2020 696d 6773 3d76 6964          imgs=vid
-00013aa0: 656f 5f70 6174 682c 2073 6861 7065 733d  eo_path, shapes=
-00013ab0: 706f 6c79 676f 6e73 2c20 7665 7262 6f73  polygons, verbos
-00013ac0: 653d 4661 6c73 650a 2020 2020 2020 2020  e=False.        
-00013ad0: 290a 2020 2020 2020 2020 7469 6d65 2e73  ).        time.s
-00013ae0: 6c65 6570 2831 290a 2020 2020 2020 2020  leep(1).        
-00013af0: 5f20 3d20 496d 6167 654d 6978 696e 2e69  _ = ImageMixin.i
-00013b00: 6d67 5f73 7461 636b 5f74 6f5f 7669 6465  mg_stack_to_vide
-00013b10: 6f28 0a20 2020 2020 2020 2020 2020 2069  o(.            i
-00013b20: 6d67 733d 706f 6c79 676f 6e73 2c20 7361  mgs=polygons, sa
-00013b30: 7665 5f70 6174 683d 7361 7665 5f70 6174  ve_path=save_pat
-00013b40: 682c 2066 7073 3d76 6964 656f 5f6d 6574  h, fps=video_met
-00013b50: 615f 6461 7461 5b22 6670 7322 5d0a 2020  a_data["fps"].  
-00013b60: 2020 2020 2020 290a 2020 2020 7469 6d65        ).    time
-00013b70: 722e 7374 6f70 5f74 696d 6572 2829 0a20  r.stop_timer(). 
-00013b80: 2020 2073 7464 6f75 745f 7375 6363 6573     stdout_succes
-00013b90: 7328 0a20 2020 2020 2020 206d 7367 3d66  s(.        msg=f
-00013ba0: 2243 6972 636c 652d 6261 7365 6420 6372  "Circle-based cr
-00013bb0: 6f70 7065 6420 7b6c 656e 2876 6964 656f  opped {len(video
-00013bc0: 5f66 696c 6573 297d 2066 696c 6573 2074  _files)} files t
-00013bd0: 6f20 6469 7265 6374 6f72 7920 7b6f 7574  o directory {out
-00013be0: 5f64 6972 7d22 2c0a 2020 2020 2020 2020  _dir}",.        
-00013bf0: 656c 6170 7365 645f 7469 6d65 3d74 696d  elapsed_time=tim
-00013c00: 6572 2e65 6c61 7073 6564 5f74 696d 655f  er.elapsed_time_
-00013c10: 7374 722c 0a20 2020 2029 0a0a 0a64 6566  str,.    )...def
-00013c20: 2063 726f 705f 7369 6e67 6c65 5f76 6964   crop_single_vid
-00013c30: 656f 5f70 6f6c 7967 6f6e 2866 696c 655f  eo_polygon(file_
-00013c40: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
-00013c50: 206f 732e 5061 7468 4c69 6b65 5d29 202d   os.PathLike]) -
-00013c60: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
-00013c70: 2020 2020 4372 6f70 2061 2076 6964 656f      Crop a video
-00013c80: 2062 6173 6564 206f 6e20 706f 6c79 676f   based on polygo
-00013c90: 6e61 6c20 7265 6769 6f6e 7320 6f66 2069  nal regions of i
-00013ca0: 6e74 6572 6573 7420 2852 4f49 7329 2073  nterest (ROIs) s
-00013cb0: 656c 6563 7465 6420 6279 2074 6865 2075  elected by the u
-00013cc0: 7365 722e 0a0a 2020 2020 3a70 6172 616d  ser...    :param
-00013cd0: 2020 556e 696f 6e5b 7374 722c 206f 732e    Union[str, os.
-00013ce0: 5061 7468 4c69 6b65 5d20 6669 6c65 5f70  PathLike] file_p
-00013cf0: 6174 683a 2054 6865 2070 6174 6820 746f  ath: The path to
-00013d00: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
-00013d10: 2066 696c 652e 0a0a 2020 2020 2e2e 206e   file...    .. n
-00013d20: 6f74 653a 3a0a 2020 2020 2020 2054 6869  ote::.       Thi
-00013d30: 7320 6675 6e63 7469 6f6e 2063 726f 7073  s function crops
-00013d40: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
-00013d50: 2062 6173 6564 206f 6e20 706f 6c79 676f   based on polygo
-00013d60: 6e61 6c20 7265 6769 6f6e 7320 6f66 2069  nal regions of i
-00013d70: 6e74 6572 6573 7420 2852 4f49 7329 2073  nterest (ROIs) s
-00013d80: 656c 6563 7465 6420 6279 2074 6865 2075  elected by the u
-00013d90: 7365 722e 0a20 2020 2020 2020 5468 6520  ser..       The 
-00013da0: 7573 6572 2069 7320 7072 6f6d 7074 6564  user is prompted
-00013db0: 2074 6f20 7365 6c65 6374 2061 2070 6f6c   to select a pol
-00013dc0: 7967 6f6e 616c 2052 4f49 206f 6e20 7468  ygonal ROI on th
-00013dd0: 6520 7669 6465 6f20 6672 616d 652c 2061  e video frame, a
-00013de0: 6e64 2074 6865 2066 756e 6374 696f 6e20  nd the function 
-00013df0: 7468 656e 2063 726f 7073 2074 6865 2076  then crops the v
-00013e00: 6964 656f 0a20 2020 2020 2020 6261 7365  ideo.       base
-00013e10: 6420 6f6e 2074 6865 2073 656c 6563 7465  d on the selecte
-00013e20: 6420 524f 492e 2054 6865 2063 726f 7070  d ROI. The cropp
-00013e30: 6564 2076 6964 656f 2069 7320 7361 7665  ed video is save
-00013e40: 6420 7769 7468 2022 5f70 6f6c 7967 6f6e  d with "_polygon
-00013e50: 5f63 726f 7070 6564 2220 7375 6666 6978  _cropped" suffix
-00013e60: 2069 6e20 7468 6520 7361 6d65 2064 6972   in the same dir
-00013e70: 6563 746f 7279 0a20 2020 2020 2020 6173  ectory.       as
-00013e80: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
-00013e90: 2066 696c 652e 0a0a 2020 2020 3a65 7861   file...    :exa
-00013ea0: 6d70 6c65 3a0a 2020 2020 3e3e 3e20 6372  mple:.    >>> cr
-00013eb0: 6f70 5f73 696e 676c 655f 7669 6465 6f5f  op_single_video_
-00013ec0: 706f 6c79 676f 6e28 6669 6c65 5f70 6174  polygon(file_pat
-00013ed0: 683d 272f 5573 6572 732f 7369 6d6f 6e2f  h='/Users/simon/
-00013ee0: 4465 736b 746f 702f 4147 4752 4553 5349  Desktop/AGGRESSI
-00013ef0: 5649 5459 5f34 5f31 315f 3231 5f54 7269  VITY_4_11_21_Tri
-00013f00: 616c 5f32 5f63 616d 6572 6131 5f72 6f74  al_2_camera1_rot
-00013f10: 6174 6564 5f32 3032 3430 3231 3131 3433  ated_20240211143
-00013f20: 3335 352e 6d70 3427 290a 2020 2020 2222  355.mp4').    ""
-00013f30: 220a 0a20 2020 2064 6972 2c20 7669 6465  "..    dir, vide
-00013f40: 6f5f 6e61 6d65 2c20 5f20 3d20 6765 745f  o_name, _ = get_
-00013f50: 666e 5f65 7874 2866 696c 6570 6174 683d  fn_ext(filepath=
-00013f60: 6669 6c65 5f70 6174 6829 0a20 2020 2073  file_path).    s
-00013f70: 6176 655f 7061 7468 203d 206f 732e 7061  ave_path = os.pa
-00013f80: 7468 2e6a 6f69 6e28 6469 722c 2066 227b  th.join(dir, f"{
-00013f90: 7669 6465 6f5f 6e61 6d65 7d5f 706f 6c79  video_name}_poly
-00013fa0: 676f 6e5f 6372 6f70 7065 642e 6d70 3422  gon_cropped.mp4"
-00013fb0: 290a 2020 2020 7669 6465 6f5f 6d65 7461  ).    video_meta
-00013fc0: 5f64 6174 6120 3d20 6765 745f 7669 6465  _data = get_vide
-00013fd0: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
-00013fe0: 6f5f 7061 7468 3d66 696c 655f 7061 7468  o_path=file_path
-00013ff0: 290a 2020 2020 6368 6563 6b5f 6669 6c65  ).    check_file
-00014000: 5f65 7869 7374 5f61 6e64 5f72 6561 6461  _exist_and_reada
-00014010: 626c 6528 6669 6c65 5f70 6174 683d 6669  ble(file_path=fi
-00014020: 6c65 5f70 6174 6829 0a20 2020 2070 6f6c  le_path).    pol
-00014030: 7967 6f6e 5f73 656c 6563 746f 7220 3d20  ygon_selector = 
-00014040: 524f 4953 656c 6563 746f 7250 6f6c 7967  ROISelectorPolyg
-00014050: 6f6e 2870 6174 683d 6669 6c65 5f70 6174  on(path=file_pat
-00014060: 6829 0a20 2020 2070 6f6c 7967 6f6e 5f73  h).    polygon_s
-00014070: 656c 6563 746f 722e 7275 6e28 290a 2020  elector.run().  
-00014080: 2020 7469 6d65 7220 3d20 5369 6d62 6154    timer = SimbaT
-00014090: 696d 6572 2873 7461 7274 3d54 7275 6529  imer(start=True)
-000140a0: 0a20 2020 2076 6572 7469 6365 7320 3d20  .    vertices = 
-000140b0: 706f 6c79 676f 6e5f 7365 6c65 6374 6f72  polygon_selector
-000140c0: 2e70 6f6c 7967 6f6e 5f76 6572 7469 6365  .polygon_vertice
-000140d0: 730a 2020 2020 706f 6c79 676f 6e20 3d20  s.    polygon = 
-000140e0: 506f 6c79 676f 6e28 7665 7274 6963 6573  Polygon(vertices
-000140f0: 290a 2020 2020 706f 6c79 676f 6e73 203d  ).    polygons =
-00014100: 205b 706f 6c79 676f 6e20 666f 7220 7820   [polygon for x 
-00014110: 696e 2072 616e 6765 2876 6964 656f 5f6d  in range(video_m
-00014120: 6574 615f 6461 7461 5b22 6672 616d 655f  eta_data["frame_
-00014130: 636f 756e 7422 5d29 5d0a 2020 2020 6966  count"])].    if
-00014140: 2028 706c 6174 666f 726d 2e73 7973 7465   (platform.syste
-00014150: 6d28 2920 3d3d 2022 4461 7277 696e 2229  m() == "Darwin")
-00014160: 2061 6e64 2028 6d75 6c74 6970 726f 6365   and (multiproce
-00014170: 7373 696e 672e 6765 745f 7374 6172 745f  ssing.get_start_
-00014180: 6d65 7468 6f64 2829 2069 7320 4e6f 6e65  method() is None
-00014190: 293a 0a20 2020 2020 2020 206d 756c 7469  ):.        multi
-000141a0: 7072 6f63 6573 7369 6e67 2e73 6574 5f73  processing.set_s
-000141b0: 7461 7274 5f6d 6574 686f 6428 2273 7061  tart_method("spa
-000141c0: 776e 222c 2066 6f72 6365 3d46 616c 7365  wn", force=False
-000141d0: 290a 2020 2020 706f 6c79 676f 6e73 203d  ).    polygons =
-000141e0: 2049 6d61 6765 4d69 7869 6e28 292e 736c   ImageMixin().sl
-000141f0: 6963 655f 7368 6170 6573 5f69 6e5f 696d  ice_shapes_in_im
-00014200: 6773 280a 2020 2020 2020 2020 696d 6773  gs(.        imgs
-00014210: 3d66 696c 655f 7061 7468 2c20 7368 6170  =file_path, shap
-00014220: 6573 3d70 6f6c 7967 6f6e 732c 2076 6572  es=polygons, ver
-00014230: 626f 7365 3d54 7275 650a 2020 2020 290a  bose=True.    ).
-00014240: 2020 2020 5f20 3d20 496d 6167 654d 6978      _ = ImageMix
-00014250: 696e 2e69 6d67 5f73 7461 636b 5f74 6f5f  in.img_stack_to_
-00014260: 7669 6465 6f28 0a20 2020 2020 2020 2069  video(.        i
-00014270: 6d67 733d 706f 6c79 676f 6e73 2c20 7361  mgs=polygons, sa
-00014280: 7665 5f70 6174 683d 7361 7665 5f70 6174  ve_path=save_pat
-00014290: 682c 2066 7073 3d76 6964 656f 5f6d 6574  h, fps=video_met
-000142a0: 615f 6461 7461 5b22 6670 7322 5d0a 2020  a_data["fps"].  
-000142b0: 2020 290a 2020 2020 7469 6d65 722e 7374    ).    timer.st
-000142c0: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
-000142d0: 7464 6f75 745f 7375 6363 6573 7328 0a20  tdout_success(. 
-000142e0: 2020 2020 2020 206d 7367 3d66 2250 6f6c         msg=f"Pol
-000142f0: 7967 6f6e 2d62 6173 6564 2063 726f 7070  ygon-based cropp
-00014300: 6564 2073 6176 6564 2061 7420 746f 207b  ed saved at to {
-00014310: 7361 7665 5f70 6174 687d 222c 0a20 2020  save_path}",.   
-00014320: 2020 2020 2065 6c61 7073 6564 5f74 696d       elapsed_tim
-00014330: 653d 7469 6d65 722e 656c 6170 7365 645f  e=timer.elapsed_
-00014340: 7469 6d65 5f73 7472 2c0a 2020 2020 290a  time_str,.    ).
-00014350: 0a0a 6465 6620 6372 6f70 5f6d 756c 7469  ..def crop_multi
-00014360: 706c 655f 7669 6465 6f73 5f70 6f6c 7967  ple_videos_polyg
-00014370: 6f6e 7328 0a20 2020 2069 6e5f 6469 723a  ons(.    in_dir:
-00014380: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00014390: 6174 684c 696b 655d 2c20 6f75 745f 6469  athLike], out_di
-000143a0: 723a 2055 6e69 6f6e 5b73 7472 2c20 6f73  r: Union[str, os
-000143b0: 2e50 6174 684c 696b 655d 0a29 202d 3e20  .PathLike].) -> 
-000143c0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-000143d0: 2020 4372 6f70 206d 756c 7469 706c 6520    Crop multiple 
-000143e0: 7669 6465 6f73 2062 6173 6564 206f 6e20  videos based on 
-000143f0: 706f 6c79 676f 6e61 6c20 7265 6769 6f6e  polygonal region
-00014400: 7320 6f66 2069 6e74 6572 6573 7420 2852  s of interest (R
-00014410: 4f49 7329 2073 656c 6563 7465 6420 6279  OIs) selected by
-00014420: 2074 6865 2075 7365 722e 0a0a 2020 2020   the user...    
-00014430: 3a70 6172 616d 2020 556e 696f 6e5b 7374  :param  Union[st
-00014440: 722c 206f 732e 5061 7468 4c69 6b65 5d20  r, os.PathLike] 
-00014450: 696e 5f64 6972 3a20 5468 6520 6469 7265  in_dir: The dire
-00014460: 6374 6f72 7920 636f 6e74 6169 6e69 6e67  ctory containing
-00014470: 2069 6e70 7574 2076 6964 656f 2066 696c   input video fil
-00014480: 6573 2e0a 2020 2020 3a70 6172 616d 2020  es..    :param  
-00014490: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-000144a0: 7468 4c69 6b65 5d20 6f75 745f 6469 723a  thLike] out_dir:
-000144b0: 2054 6865 2064 6972 6563 746f 7279 2074   The directory t
-000144c0: 6f20 7361 7665 2074 6865 2063 726f 7070  o save the cropp
-000144d0: 6564 2076 6964 656f 2066 696c 6573 2e0a  ed video files..
-000144e0: 0a20 2020 202e 2e20 6e6f 7465 3a3a 0a20  .    .. note::. 
-000144f0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00014500: 696f 6e20 6372 6f70 7320 6d75 6c74 6970  ion crops multip
-00014510: 6c65 2076 6964 656f 7320 6261 7365 6420  le videos based 
-00014520: 6f6e 2070 6f6c 7967 6f6e 616c 2052 4f49  on polygonal ROI
-00014530: 7320 7365 6c65 6374 6564 2062 7920 7468  s selected by th
-00014540: 6520 7573 6572 2e0a 2020 2020 2020 2054  e user..       T
-00014550: 6865 2075 7365 7220 6973 2061 736b 6564  he user is asked
-00014560: 2074 6f20 6465 6669 6e65 2061 2070 6f6c   to define a pol
-00014570: 7967 6f6e 206d 616e 7561 6c6c 7920 696e  ygon manually in
-00014580: 206f 6e65 2076 6964 656f 2077 6974 6869   one video withi
-00014590: 6e20 7468 6520 696e 7075 7420 6469 7265  n the input dire
-000145a0: 6374 6f72 792e 0a20 2020 2020 2020 5468  ctory..       Th
-000145b0: 6520 6675 6e63 7469 6f6e 2074 6865 6e20  e function then 
-000145c0: 6372 6f70 7320 616c 6c20 7468 6520 7669  crops all the vi
-000145d0: 6465 6f20 696e 2074 6865 2069 6e70 7574  deo in the input
-000145e0: 2064 6972 6563 746f 7279 2061 6363 6f72   directory accor
-000145f0: 6469 6e67 2074 6f20 7468 6520 7368 6170  ding to the shap
-00014600: 6520 6465 6669 6e65 640a 2020 2020 2020  e defined.      
-00014610: 2075 7369 6e67 2074 6865 2066 6972 7374   using the first
-00014620: 2076 6964 656f 2061 6e64 2073 6176 6573   video and saves
-00014630: 2074 6865 2076 6964 656f 7320 696e 2074   the videos in t
-00014640: 6865 2060 606f 7574 5f64 6972 6060 2077  he ``out_dir`` w
-00014650: 6974 6820 7468 6520 7361 6d65 2066 696c  ith the same fil
-00014660: 656e 616d 6573 2061 7320 7468 6520 6f72  enames as the or
-00014670: 6967 696e 616c 2076 6964 656f 732e 2e0a  iginal videos...
-00014680: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
-00014690: 2020 203e 3e3e 2063 726f 705f 6d75 6c74     >>> crop_mult
-000146a0: 6970 6c65 5f76 6964 656f 735f 706f 6c79  iple_videos_poly
-000146b0: 676f 6e73 2869 6e5f 6469 723d 272f 5573  gons(in_dir='/Us
-000146c0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-000146d0: 702f 6564 6974 6564 2f74 6573 7473 272c  p/edited/tests',
-000146e0: 206f 7574 5f64 6972 3d27 2f55 7365 7273   out_dir='/Users
-000146f0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2729  /simon/Desktop')
-00014700: 0a20 2020 2022 2222 0a0a 2020 2020 6368  .    """..    ch
-00014710: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
-00014720: 7328 696e 5f64 6972 3d69 6e5f 6469 7229  s(in_dir=in_dir)
-00014730: 0a20 2020 2063 6865 636b 5f69 665f 6469  .    check_if_di
-00014740: 725f 6578 6973 7473 2869 6e5f 6469 723d  r_exists(in_dir=
-00014750: 6f75 745f 6469 7229 0a20 2020 2076 6964  out_dir).    vid
-00014760: 656f 5f66 696c 6573 203d 2066 696e 645f  eo_files = find_
-00014770: 616c 6c5f 7669 6465 6f73 5f69 6e5f 6469  all_videos_in_di
-00014780: 7265 6374 6f72 7928 6469 7265 6374 6f72  rectory(director
-00014790: 793d 696e 5f64 6972 290a 2020 2020 706f  y=in_dir).    po
-000147a0: 6c79 676f 6e5f 7365 6c65 6374 6f72 203d  lygon_selector =
-000147b0: 2052 4f49 5365 6c65 6374 6f72 506f 6c79   ROISelectorPoly
-000147c0: 676f 6e28 7061 7468 3d6f 732e 7061 7468  gon(path=os.path
-000147d0: 2e6a 6f69 6e28 696e 5f64 6972 2c20 7669  .join(in_dir, vi
-000147e0: 6465 6f5f 6669 6c65 735b 305d 2929 0a20  deo_files[0])). 
-000147f0: 2020 2070 6f6c 7967 6f6e 5f73 656c 6563     polygon_selec
-00014800: 746f 722e 7275 6e28 290a 2020 2020 7665  tor.run().    ve
-00014810: 7274 6963 6573 203d 2070 6f6c 7967 6f6e  rtices = polygon
-00014820: 5f73 656c 6563 746f 722e 706f 6c79 676f  _selector.polygo
-00014830: 6e5f 7665 7274 6963 6573 0a20 2020 2070  n_vertices.    p
-00014840: 6f6c 7967 6f6e 203d 2050 6f6c 7967 6f6e  olygon = Polygon
-00014850: 2876 6572 7469 6365 7329 0a20 2020 2074  (vertices).    t
-00014860: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
-00014870: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
-00014880: 2020 666f 7220 7669 6465 6f5f 636e 742c    for video_cnt,
-00014890: 2076 6964 656f 5f70 6174 6820 696e 2065   video_path in e
-000148a0: 6e75 6d65 7261 7465 2876 6964 656f 5f66  numerate(video_f
-000148b0: 696c 6573 293a 0a20 2020 2020 2020 2070  iles):.        p
-000148c0: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
-000148d0: 2020 6622 506f 6c79 676f 6e20 6372 6f70    f"Polygon crop
-000148e0: 7069 6e67 2076 6964 656f 207b 7669 6465  ping video {vide
-000148f0: 6f5f 7061 7468 7d20 287b 7669 6465 6f5f  o_path} ({video_
-00014900: 636e 742b 317d 2f7b 6c65 6e28 7669 6465  cnt+1}/{len(vide
-00014910: 6f5f 6669 6c65 7329 7d29 2e2e 2e22 0a20  o_files)})...". 
-00014920: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00014930: 2076 6964 656f 5f70 6174 6820 3d20 6f73   video_path = os
-00014940: 2e70 6174 682e 6a6f 696e 2869 6e5f 6469  .path.join(in_di
-00014950: 722c 2076 6964 656f 5f70 6174 6829 0a20  r, video_path). 
-00014960: 2020 2020 2020 205f 2c20 7669 6465 6f5f         _, video_
-00014970: 6e61 6d65 2c20 5f20 3d20 6765 745f 666e  name, _ = get_fn
-00014980: 5f65 7874 2866 696c 6570 6174 683d 7669  _ext(filepath=vi
-00014990: 6465 6f5f 7061 7468 290a 2020 2020 2020  deo_path).      
-000149a0: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
-000149b0: 2e70 6174 682e 6a6f 696e 286f 7574 5f64  .path.join(out_d
-000149c0: 6972 2c20 6622 7b76 6964 656f 5f6e 616d  ir, f"{video_nam
-000149d0: 657d 2e6d 7034 2229 0a20 2020 2020 2020  e}.mp4").       
-000149e0: 2076 6964 656f 5f6d 6574 615f 6461 7461   video_meta_data
-000149f0: 203d 2067 6574 5f76 6964 656f 5f6d 6574   = get_video_met
-00014a00: 615f 6461 7461 2876 6964 656f 5f70 6174  a_data(video_pat
-00014a10: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-00014a20: 2020 2020 2020 706f 6c79 676f 6e73 203d        polygons =
-00014a30: 205b 706f 6c79 676f 6e20 666f 7220 7820   [polygon for x 
-00014a40: 696e 2072 616e 6765 2876 6964 656f 5f6d  in range(video_m
-00014a50: 6574 615f 6461 7461 5b22 6672 616d 655f  eta_data["frame_
-00014a60: 636f 756e 7422 5d29 5d0a 2020 2020 2020  count"])].      
-00014a70: 2020 706f 6c79 676f 6e73 203d 2049 6d61    polygons = Ima
-00014a80: 6765 4d69 7869 6e28 292e 736c 6963 655f  geMixin().slice_
-00014a90: 7368 6170 6573 5f69 6e5f 696d 6773 280a  shapes_in_imgs(.
-00014aa0: 2020 2020 2020 2020 2020 2020 696d 6773              imgs
-00014ab0: 3d76 6964 656f 5f70 6174 682c 2073 6861  =video_path, sha
-00014ac0: 7065 733d 706f 6c79 676f 6e73 2c20 7665  pes=polygons, ve
-00014ad0: 7262 6f73 653d 4661 6c73 650a 2020 2020  rbose=False.    
-00014ae0: 2020 2020 290a 2020 2020 2020 2020 5f20      ).        _ 
-00014af0: 3d20 496d 6167 654d 6978 696e 2e69 6d67  = ImageMixin.img
-00014b00: 5f73 7461 636b 5f74 6f5f 7669 6465 6f28  _stack_to_video(
-00014b10: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
-00014b20: 733d 706f 6c79 676f 6e73 2c20 7361 7665  s=polygons, save
-00014b30: 5f70 6174 683d 7361 7665 5f70 6174 682c  _path=save_path,
-00014b40: 2066 7073 3d76 6964 656f 5f6d 6574 615f   fps=video_meta_
-00014b50: 6461 7461 5b22 6670 7322 5d0a 2020 2020  data["fps"].    
-00014b60: 2020 2020 290a 2020 2020 7469 6d65 722e      ).    timer.
-00014b70: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
-00014b80: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
-00014b90: 0a20 2020 2020 2020 206d 7367 3d66 2250  .        msg=f"P
-00014ba0: 6f6c 7967 6f6e 2d62 6173 6564 2063 726f  olygon-based cro
-00014bb0: 7070 6564 207b 6c65 6e28 7669 6465 6f5f  pped {len(video_
-00014bc0: 6669 6c65 7329 7d20 6669 6c65 7320 746f  files)} files to
-00014bd0: 2064 6972 6563 746f 7279 207b 6f75 745f   directory {out_
-00014be0: 6469 727d 222c 0a20 2020 2020 2020 2065  dir}",.        e
-00014bf0: 6c61 7073 6564 5f74 696d 653d 7469 6d65  lapsed_time=time
-00014c00: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
-00014c10: 7472 2c0a 2020 2020 290a 0a0a 6465 6620  tr,.    )...def 
-00014c20: 7265 7369 7a65 5f76 6964 656f 735f 6279  resize_videos_by
-00014c30: 5f68 6569 6768 7428 0a20 2020 2076 6964  _height(.    vid
-00014c40: 656f 5f70 6174 6873 3a20 4c69 7374 5b55  eo_paths: List[U
-00014c50: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-00014c60: 684c 696b 655d 5d2c 0a20 2020 2068 6569  hLike]],.    hei
-00014c70: 6768 743a 2055 6e69 6f6e 5b69 6e74 2c20  ght: Union[int, 
-00014c80: 7374 725d 2c0a 2020 2020 6f76 6572 7772  str],.    overwr
-00014c90: 6974 653a 204f 7074 696f 6e61 6c5b 626f  ite: Optional[bo
-00014ca0: 6f6c 5d20 3d20 4661 6c73 652c 0a20 2020  ol] = False,.   
-00014cb0: 2073 6176 655f 6469 723a 204f 7074 696f   save_dir: Optio
-00014cc0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
-00014cd0: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
-00014ce0: 6f6e 652c 0a20 2020 2067 7075 3a20 4f70  one,.    gpu: Op
-00014cf0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
-00014d00: 616c 7365 2c0a 2020 2020 7665 7262 6f73  alse,.    verbos
-00014d10: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
-00014d20: 5d20 3d20 5472 7565 2c0a 2920 2d3e 2055  ] = True,.) -> U
-00014d30: 6e69 6f6e 5b4e 6f6e 652c 204c 6973 745b  nion[None, List[
-00014d40: 556e 696f 6e5b 4e6f 6e65 2c20 7374 722c  Union[None, str,
-00014d50: 206f 732e 5061 7468 4c69 6b65 5d5d 5d3a   os.PathLike]]]:
-00014d60: 0a20 2020 2022 2222 0a20 2020 2052 652d  .    """.    Re-
-00014d70: 7369 7a65 2061 206c 6973 7420 6f66 2076  size a list of v
-00014d80: 6964 656f 7320 746f 2061 2073 7065 6369  ideos to a speci
-00014d90: 6669 6564 2068 6569 6768 7420 7768 696c  fied height whil
-00014da0: 6520 7265 7461 696e 696e 6720 7468 6569  e retaining thei
-00014db0: 7220 6173 7065 6374 2072 6174 696f 732e  r aspect ratios.
-00014dc0: 0a0a 2020 2020 3a70 6172 616d 204c 6973  ..    :param Lis
-00014dd0: 745b 556e 696f 6e5b 7374 722c 206f 732e  t[Union[str, os.
-00014de0: 5061 7468 4c69 6b65 5d5d 2076 6964 656f  PathLike]] video
-00014df0: 5f70 6174 6873 3a20 4c69 7374 206f 6620  _paths: List of 
-00014e00: 7061 7468 2074 6f20 7669 6465 6f73 2e0a  path to videos..
-00014e10: 2020 2020 3a70 6172 616d 2055 6e69 6f6e      :param Union
-00014e20: 5b69 6e74 2c20 7374 725d 2068 6569 6768  [int, str] heigh
-00014e30: 743a 2054 6865 2068 6569 6768 7420 6f66  t: The height of
-00014e40: 2074 6865 206f 7574 7075 7420 7669 6465   the output vide
-00014e50: 6f73 2e20 4966 2069 6e74 2c20 7468 656e  os. If int, then
-00014e60: 2074 6865 2068 6569 6768 7420 696e 2070   the height in p
-00014e70: 6978 656c 732e 2049 6620 7374 722c 2074  ixels. If str, t
-00014e80: 6865 6e20 7468 6520 696e 6465 7820 696e  hen the index in
-00014e90: 2060 6076 6964 656f 5f70 6174 6873 6060   ``video_paths``
-00014ea0: 2066 726f 6d20 7768 6963 6820 746f 2067   from which to g
-00014eb0: 7261 6220 7468 6520 6865 6967 6874 2e0a  rab the height..
-00014ec0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-00014ed0: 6e61 6c5b 626f 6f6c 5d20 6f76 6572 7772  nal[bool] overwr
-00014ee0: 6974 653a 2049 6620 5472 7565 2c20 7468  ite: If True, th
-00014ef0: 656e 206f 7665 7277 7269 7465 7320 7468  en overwrites th
-00014f00: 6520 6f72 6967 696e 616c 2076 6964 656f  e original video
-00014f10: 732e 2044 6566 6175 6c74 2046 616c 7365  s. Default False
-00014f20: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00014f30: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-00014f40: 206f 732e 5061 7468 4c69 6b65 5d5d 2073   os.PathLike]] s
-00014f50: 6176 655f 6469 723a 2049 6620 6e6f 7420  ave_dir: If not 
-00014f60: 4e6f 6e65 2c20 7468 656e 2074 6865 2064  None, then the d
-00014f70: 6972 6563 746f 7279 2077 6865 7265 2074  irectory where t
-00014f80: 6f20 7374 6f72 6520 7468 6520 7265 2d73  o store the re-s
-00014f90: 697a 6564 2076 6964 656f 732e 0a20 2020  ized videos..   
-00014fa0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00014fb0: 5b62 6f6f 6c5d 2067 7075 3a20 4966 2054  [bool] gpu: If T
-00014fc0: 7275 652c 2074 6865 6e20 7573 6520 4646  rue, then use FF
-00014fd0: 6d70 6567 2047 5055 2063 6f64 6563 732e  mpeg GPU codecs.
-00014fe0: 2044 6566 6175 6c74 2046 616c 7365 2e0a   Default False..
-00014ff0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-00015000: 6e61 6c5b 626f 6f6c 5d20 7665 7262 6f73  nal[bool] verbos
-00015010: 653a 2049 6620 5472 7565 2c20 7072 696e  e: If True, prin
-00015020: 7473 2070 726f 6772 6573 732e 2044 6566  ts progress. Def
-00015030: 6175 6c74 2054 7275 652e 0a20 2020 203a  ault True..    :
-00015040: 7265 7475 726e 2055 6e69 6f6e 5b4e 6f6e  return Union[Non
-00015050: 652c 204c 6973 745b 556e 696f 6e5b 7374  e, List[Union[st
-00015060: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
-00015070: 5d3a 2049 6620 7361 7665 5f64 6972 2069  ]: If save_dir i
-00015080: 7320 6e6f 7420 4e6f 6e65 2c20 7265 7475  s not None, retu
-00015090: 726e 7320 7468 6520 7061 7468 7320 6f66  rns the paths of
-000150a0: 2074 6865 2072 652d 7369 7a65 6420 7669   the re-sized vi
-000150b0: 6465 6f73 2e20 456c 7365 2072 6574 7572  deos. Else retur
-000150c0: 6e73 2065 6d70 7479 206c 6973 742e 0a0a  ns empty list...
-000150d0: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
-000150e0: 2020 3e3e 3e20 7669 6465 6f5f 7061 7468    >>> video_path
-000150f0: 733d 205b 272f 5573 6572 732f 7369 6d6f  s= ['/Users/simo
-00015100: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
-00015110: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
-00015120: 7469 6e67 2f52 4154 5f4e 4f52 2f70 726f  ting/RAT_NOR/pro
-00015130: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
-00015140: 6f73 2f74 6573 742f 3038 3130 3230 3231  os/test/08102021
-00015150: 5f44 4f54 5f52 6174 375f 3828 3229 2e6d  _DOT_Rat7_8(2).m
-00015160: 7034 272c 2027 2f55 7365 7273 2f73 696d  p4', '/Users/sim
-00015170: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-00015180: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-00015190: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
-000151a0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-000151b0: 656f 732f 7465 7374 2f30 3831 3032 3032  eos/test/0810202
-000151c0: 315f 444f 545f 5261 7431 315f 3132 2e6d  1_DOT_Rat11_12.m
-000151d0: 7034 275d 0a20 2020 203e 3e3e 205f 203d  p4'].    >>> _ =
-000151e0: 2072 6573 697a 655f 7669 6465 6f73 5f62   resize_videos_b
-000151f0: 795f 6865 6967 6874 2876 6964 656f 5f70  y_height(video_p
-00015200: 6174 6873 3d76 6964 656f 5f70 6174 6873  aths=video_paths
-00015210: 2c20 6865 6967 6874 3d33 3030 2c20 6f76  , height=300, ov
-00015220: 6572 7772 6974 653d 4661 6c73 652c 2073  erwrite=False, s
-00015230: 6176 655f 6469 723d 272f 5573 6572 732f  ave_dir='/Users/
-00015240: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-00015250: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-00015260: 7368 6f6f 7469 6e67 2f52 4154 5f4e 4f52  shooting/RAT_NOR
-00015270: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
-00015280: 7669 6465 6f73 2f74 6573 742f 6e65 7727  videos/test/new'
-00015290: 290a 2020 2020 2222 220a 2020 2020 7469  ).    """.    ti
-000152a0: 6d65 7220 3d20 5369 6d62 6154 696d 6572  mer = SimbaTimer
-000152b0: 2873 7461 7274 3d54 7275 6529 0a20 2020  (start=True).   
-000152c0: 2069 6620 286e 6f74 206f 7665 7277 7269   if (not overwri
-000152d0: 7465 2920 616e 6420 2873 6176 655f 6469  te) and (save_di
-000152e0: 7220 6973 204e 6f6e 6529 3a0a 2020 2020  r is None):.    
-000152f0: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
-00015300: 6449 6e70 7574 4572 726f 7228 0a20 2020  dInputError(.   
-00015310: 2020 2020 2020 2020 206d 7367 3d22 5061           msg="Pa
-00015320: 7373 2061 2073 6176 655f 6469 7220 4f52  ss a save_dir OR
-00015330: 2073 6574 206f 7665 7277 7269 7465 2074   set overwrite t
-00015340: 6f20 5472 7565 222c 0a20 2020 2020 2020  o True",.       
-00015350: 2020 2020 2073 6f75 7263 653d 7265 7369       source=resi
-00015360: 7a65 5f76 6964 656f 735f 6279 5f68 6569  ze_videos_by_hei
-00015370: 6768 742e 5f5f 6e61 6d65 5f5f 2c0a 2020  ght.__name__,.  
-00015380: 2020 2020 2020 290a 2020 2020 656c 6966        ).    elif
-00015390: 2028 6f76 6572 7772 6974 6529 2061 6e64   (overwrite) and
-000153a0: 2028 7361 7665 5f64 6972 2069 7320 6e6f   (save_dir is no
-000153b0: 7420 4e6f 6e65 293a 0a20 2020 2020 2020  t None):.       
-000153c0: 2072 6169 7365 2049 6e76 616c 6964 496e   raise InvalidIn
-000153d0: 7075 7445 7272 6f72 280a 2020 2020 2020  putError(.      
-000153e0: 2020 2020 2020 6d73 673d 2250 6173 7320        msg="Pass 
-000153f0: 4549 5448 4552 206f 7665 7277 7269 7465  EITHER overwrite
-00015400: 2061 7320 5472 7565 204f 5220 7061 7373   as True OR pass
-00015410: 2061 2073 6176 655f 6469 7222 2c0a 2020   a save_dir",.  
-00015420: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00015430: 3d72 6573 697a 655f 7669 6465 6f73 5f62  =resize_videos_b
-00015440: 795f 6865 6967 6874 2e5f 5f6e 616d 655f  y_height.__name_
-00015450: 5f2c 0a20 2020 2020 2020 2029 0a20 2020  _,.        ).   
-00015460: 2069 6620 7361 7665 5f64 6972 2069 7320   if save_dir is 
-00015470: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00015480: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
-00015490: 2e69 7364 6972 2873 6176 655f 6469 7229  .isdir(save_dir)
-000154a0: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-000154b0: 2e6d 616b 6564 6972 7328 7361 7665 5f64  .makedirs(save_d
-000154c0: 6972 290a 2020 2020 6368 6563 6b5f 7661  ir).    check_va
-000154d0: 6c69 645f 6c73 7428 0a20 2020 2020 2020  lid_lst(.       
-000154e0: 2064 6174 613d 7669 6465 6f5f 7061 7468   data=video_path
-000154f0: 732c 2073 6f75 7263 653d 7265 7369 7a65  s, source=resize
-00015500: 5f76 6964 656f 735f 6279 5f68 6569 6768  _videos_by_heigh
-00015510: 742e 5f5f 6e61 6d65 5f5f 2c20 6d69 6e5f  t.__name__, min_
-00015520: 6c65 6e3d 310a 2020 2020 290a 2020 2020  len=1.    ).    
-00015530: 5f20 3d20 5b63 6865 636b 5f66 696c 655f  _ = [check_file_
-00015540: 6578 6973 745f 616e 645f 7265 6164 6162  exist_and_readab
-00015550: 6c65 2878 2920 666f 7220 7820 696e 2076  le(x) for x in v
-00015560: 6964 656f 5f70 6174 6873 5d0a 2020 2020  ideo_paths].    
-00015570: 6e65 775f 7669 6465 6f5f 7061 7468 7320  new_video_paths 
-00015580: 3d20 5b5d 0a20 2020 2069 6620 6973 696e  = [].    if isin
-00015590: 7374 616e 6365 2868 6569 6768 742c 2073  stance(height, s
-000155a0: 7472 293a 0a20 2020 2020 2020 2063 6865  tr):.        che
-000155b0: 636b 5f69 6e74 280a 2020 2020 2020 2020  ck_int(.        
-000155c0: 2020 2020 6e61 6d65 3d66 227b 7265 7369      name=f"{resi
-000155d0: 7a65 5f76 6964 656f 735f 6279 5f68 6569  ze_videos_by_hei
-000155e0: 6768 742e 5f5f 6e61 6d65 5f5f 7d20 6865  ght.__name__} he
-000155f0: 6967 6874 222c 0a20 2020 2020 2020 2020  ight",.         
-00015600: 2020 2076 616c 7565 3d68 6569 6768 742c     value=height,
-00015610: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
-00015620: 5f76 616c 7565 3d30 2c0a 2020 2020 2020  _value=0,.      
-00015630: 2020 2020 2020 6d61 785f 7661 6c75 653d        max_value=
-00015640: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
-00015650: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00015660: 2020 2020 7669 6465 6f5f 6865 6967 6874      video_height
-00015670: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-00015680: 6f72 2069 2069 6e20 7669 6465 6f5f 7061  or i in video_pa
-00015690: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
-000156a0: 2076 6964 656f 5f68 6569 6768 7473 2e61   video_heights.a
-000156b0: 7070 656e 6428 6765 745f 7669 6465 6f5f  ppend(get_video_
-000156c0: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
-000156d0: 7061 7468 3d69 295b 2268 6569 6768 7422  path=i)["height"
-000156e0: 5d29 0a20 2020 2020 2020 2068 6569 6768  ]).        heigh
-000156f0: 7420 3d20 7669 6465 6f5f 6865 6967 6874  t = video_height
-00015700: 735b 696e 7428 6865 6967 6874 295d 0a20  s[int(height)]. 
-00015710: 2020 2066 6f72 2063 6e74 2c20 7669 6465     for cnt, vide
-00015720: 6f5f 7061 7468 2069 6e20 656e 756d 6572  o_path in enumer
-00015730: 6174 6528 7669 6465 6f5f 7061 7468 7329  ate(video_paths)
-00015740: 3a0a 2020 2020 2020 2020 6469 725f 6e61  :.        dir_na
-00015750: 6d65 2c20 7669 6465 6f5f 6e61 6d65 2c20  me, video_name, 
-00015760: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
-00015770: 2876 6964 656f 5f70 6174 6829 0a20 2020  (video_path).   
-00015780: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-00015790: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000157a0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-000157b0: 2020 2020 6622 5265 7369 7a69 6e67 2068      f"Resizing h
-000157c0: 6569 6768 7420 7669 6465 6f20 7b76 6964  eight video {vid
-000157d0: 656f 5f6e 616d 657d 2028 5669 6465 6f20  eo_name} (Video 
-000157e0: 7b63 6e74 2b31 7d2f 7b6c 656e 2876 6964  {cnt+1}/{len(vid
-000157f0: 656f 5f70 6174 6873 297d 292e 2e2e 220a  eo_paths)})...".
-00015800: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00015810: 2020 2020 2020 6966 206f 7665 7277 7269        if overwri
-00015820: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-00015830: 6474 203d 2064 6174 6574 696d 652e 6e6f  dt = datetime.no
-00015840: 7728 292e 7374 7266 7469 6d65 2822 2559  w().strftime("%Y
-00015850: 256d 2564 2548 254d 2553 2229 0a20 2020  %m%d%H%M%S").   
-00015860: 2020 2020 2020 2020 2073 6176 655f 7061           save_pa
-00015870: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-00015880: 6e28 6469 725f 6e61 6d65 2c20 6622 7b76  n(dir_name, f"{v
-00015890: 6964 656f 5f6e 616d 657d 5f7b 6474 7d2e  ideo_name}_{dt}.
-000158a0: 6d70 3422 290a 2020 2020 2020 2020 656c  mp4").        el
-000158b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000158c0: 7361 7665 5f70 6174 6820 3d20 6f73 2e70  save_path = os.p
-000158d0: 6174 682e 6a6f 696e 2873 6176 655f 6469  ath.join(save_di
-000158e0: 722c 2066 227b 7669 6465 6f5f 6e61 6d65  r, f"{video_name
-000158f0: 7d2e 6d70 3422 290a 2020 2020 2020 2020  }.mp4").        
-00015900: 2020 2020 6e65 775f 7669 6465 6f5f 7061      new_video_pa
-00015910: 7468 732e 6170 7065 6e64 2873 6176 655f  ths.append(save_
-00015920: 7061 7468 290a 2020 2020 2020 2020 6966  path).        if
-00015930: 2067 7075 3a0a 2020 2020 2020 2020 2020   gpu:.          
-00015940: 2020 636d 6420 3d20 6627 6666 6d70 6567    cmd = f'ffmpeg
-00015950: 202d 7920 2d68 7761 6363 656c 2061 7574   -y -hwaccel aut
-00015960: 6f20 2d63 3a76 2068 3236 345f 6375 7669  o -c:v h264_cuvi
-00015970: 6420 2d69 2022 7b76 6964 656f 5f70 6174  d -i "{video_pat
-00015980: 687d 2220 2d76 6620 7363 616c 655f 6e70  h}" -vf scale_np
-00015990: 703d 2d32 3a7b 6865 6967 6874 7d20 2d63  p=-2:{height} -c
-000159a0: 3a76 2068 3236 345f 6e76 656e 6320 227b  :v h264_nvenc "{
-000159b0: 7361 7665 5f70 6174 687d 2220 2d68 6964  save_path}" -hid
-000159c0: 655f 6261 6e6e 6572 202d 6c6f 676c 6576  e_banner -loglev
-000159d0: 656c 2065 7272 6f72 202d 7927 0a20 2020  el error -y'.   
-000159e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000159f0: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
-00015a00: 666d 7065 6720 2d79 202d 6920 227b 7669  fmpeg -y -i "{vi
-00015a10: 6465 6f5f 7061 7468 7d22 202d 7666 2073  deo_path}" -vf s
-00015a20: 6361 6c65 3d2d 323a 7b68 6569 6768 747d  cale=-2:{height}
-00015a30: 2022 7b73 6176 655f 7061 7468 7d22 202d   "{save_path}" -
-00015a40: 6869 6465 5f62 616e 6e65 7220 2d6c 6f67  hide_banner -log
-00015a50: 6c65 7665 6c20 6572 726f 7220 2d79 270a  level error -y'.
-00015a60: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
-00015a70: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
-00015a80: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
-00015a90: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
-00015aa0: 0a20 2020 2020 2020 2069 6620 6f76 6572  .        if over
-00015ab0: 7772 6974 653a 0a20 2020 2020 2020 2020  write:.         
-00015ac0: 2020 2073 6875 7469 6c2e 636f 7079 2873     shutil.copy(s
-00015ad0: 6176 655f 7061 7468 2c20 7669 6465 6f5f  ave_path, video_
-00015ae0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-00015af0: 2020 6f73 2e72 656d 6f76 6528 7361 7665    os.remove(save
-00015b00: 5f70 6174 6829 0a20 2020 2074 696d 6572  _path).    timer
-00015b10: 2e73 746f 705f 7469 6d65 7228 290a 2020  .stop_timer().  
-00015b20: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00015b30: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
-00015b40: 2020 2020 2020 2020 2066 2252 6573 697a           f"Resiz
-00015b50: 6564 2068 6569 6768 7420 7b6c 656e 2876  ed height {len(v
-00015b60: 6964 656f 5f70 6174 6873 297d 2076 6964  ideo_paths)} vid
-00015b70: 656f 2873 292e 2045 6c61 7073 6564 2074  eo(s). Elapsed t
-00015b80: 696d 653a 207b 7469 6d65 722e 656c 6170  ime: {timer.elap
-00015b90: 7365 645f 7469 6d65 5f73 7472 7d73 2e22  sed_time_str}s."
-00015ba0: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
-00015bb0: 6574 7572 6e20 6e65 775f 7669 6465 6f5f  eturn new_video_
-00015bc0: 7061 7468 730a 0a0a 6465 6620 7265 7369  paths...def resi
-00015bd0: 7a65 5f76 6964 656f 735f 6279 5f77 6964  ze_videos_by_wid
-00015be0: 7468 280a 2020 2020 7669 6465 6f5f 7061  th(.    video_pa
-00015bf0: 7468 733a 204c 6973 745b 556e 696f 6e5b  ths: List[Union[
-00015c00: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
-00015c10: 5d5d 2c0a 2020 2020 7769 6474 683a 2055  ]],.    width: U
-00015c20: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2c0a  nion[int, str],.
-00015c30: 2020 2020 6f76 6572 7772 6974 653a 204f      overwrite: O
-00015c40: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00015c50: 4661 6c73 652c 0a20 2020 2073 6176 655f  False,.    save_
-00015c60: 6469 723a 204f 7074 696f 6e61 6c5b 556e  dir: Optional[Un
-00015c70: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00015c80: 4c69 6b65 5d5d 203d 204e 6f6e 652c 0a20  Like]] = None,. 
-00015c90: 2020 2067 7075 3a20 4f70 7469 6f6e 616c     gpu: Optional
-00015ca0: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
-00015cb0: 2020 2020 7665 7262 6f73 653a 204f 7074      verbose: Opt
-00015cc0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
-00015cd0: 7565 2c0a 2920 2d3e 2055 6e69 6f6e 5b4e  ue,.) -> Union[N
-00015ce0: 6f6e 652c 204c 6973 745b 556e 696f 6e5b  one, List[Union[
-00015cf0: 4e6f 6e65 2c20 7374 722c 206f 732e 5061  None, str, os.Pa
-00015d00: 7468 4c69 6b65 5d5d 5d3a 0a20 2020 2022  thLike]]]:.    "
-00015d10: 2222 0a20 2020 2052 652d 7369 7a65 2061  "".    Re-size a
-00015d20: 206c 6973 7420 6f66 2076 6964 656f 7320   list of videos 
-00015d30: 746f 2061 2073 7065 6369 6669 6564 2077  to a specified w
-00015d40: 6964 7468 2077 6869 6c65 2072 6574 6169  idth while retai
-00015d50: 6e69 6e67 2074 6865 6972 2061 7370 6563  ning their aspec
-00015d60: 7420 7261 7469 6f73 2e0a 0a20 2020 203a  t ratios...    :
-00015d70: 7061 7261 6d20 4c69 7374 5b55 6e69 6f6e  param List[Union
-00015d80: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-00015d90: 655d 5d20 7669 6465 6f5f 7061 7468 733a  e]] video_paths:
-00015da0: 204c 6973 7420 6f66 2070 6174 6820 746f   List of path to
-00015db0: 2076 6964 656f 732e 0a20 2020 203a 7061   videos..    :pa
-00015dc0: 7261 6d20 556e 696f 6e5b 696e 742c 2073  ram Union[int, s
-00015dd0: 7472 5d20 7769 6474 683a 2054 6865 2077  tr] width: The w
-00015de0: 6964 7468 206f 6620 7468 6520 6f75 7470  idth of the outp
-00015df0: 7574 2076 6964 656f 732e 2049 6620 696e  ut videos. If in
-00015e00: 742c 2074 6865 6e20 7468 6520 7769 6474  t, then the widt
-00015e10: 6820 696e 2070 6978 656c 732e 2049 6620  h in pixels. If 
-00015e20: 7374 722c 2074 6865 6e20 7468 6520 696e  str, then the in
-00015e30: 6465 7820 696e 2060 6076 6964 656f 5f70  dex in ``video_p
-00015e40: 6174 6873 6060 2066 726f 6d20 7768 6963  aths`` from whic
-00015e50: 6820 746f 2067 7261 6220 7468 6520 7769  h to grab the wi
-00015e60: 6474 682e 0a20 2020 203a 7061 7261 6d20  dth..    :param 
-00015e70: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 206f  Optional[bool] o
-00015e80: 7665 7277 7269 7465 3a20 4966 2054 7275  verwrite: If Tru
-00015e90: 652c 2074 6865 6e20 6f76 6572 7772 6974  e, then overwrit
-00015ea0: 6573 2074 6865 206f 7269 6769 6e61 6c20  es the original 
-00015eb0: 7669 6465 6f73 2e20 4465 6661 756c 7420  videos. Default 
-00015ec0: 4661 6c73 652e 0a20 2020 203a 7061 7261  False..    :para
-00015ed0: 6d20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  m Optional[Union
-00015ee0: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-00015ef0: 655d 5d20 7361 7665 5f64 6972 3a20 4966  e]] save_dir: If
-00015f00: 206e 6f74 204e 6f6e 652c 2074 6865 6e20   not None, then 
-00015f10: 7468 6520 6469 7265 6374 6f72 7920 7768  the directory wh
-00015f20: 6572 6520 746f 2073 746f 7265 2074 6865  ere to store the
-00015f30: 2072 652d 7369 7a65 6420 7669 6465 6f73   re-sized videos
-00015f40: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00015f50: 696f 6e61 6c5b 626f 6f6c 5d20 6770 753a  ional[bool] gpu:
-00015f60: 2049 6620 5472 7565 2c20 7468 656e 2075   If True, then u
-00015f70: 7365 2046 466d 7065 6720 4750 5520 636f  se FFmpeg GPU co
-00015f80: 6465 6373 2e20 4465 6661 756c 7420 4661  decs. Default Fa
-00015f90: 6c73 652e 0a20 2020 203a 7061 7261 6d20  lse..    :param 
-00015fa0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 2076  Optional[bool] v
-00015fb0: 6572 626f 7365 3a20 4966 2054 7275 652c  erbose: If True,
-00015fc0: 2070 7269 6e74 7320 7072 6f67 7265 7373   prints progress
-00015fd0: 2e20 4465 6661 756c 7420 5472 7565 2e0a  . Default True..
-00015fe0: 2020 2020 3a72 6574 7572 6e20 556e 696f      :return Unio
-00015ff0: 6e5b 4e6f 6e65 2c20 4c69 7374 5b55 6e69  n[None, List[Uni
-00016000: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00016010: 696b 655d 5d5d 3a20 4966 2073 6176 655f  ike]]]: If save_
-00016020: 6469 7220 6973 206e 6f74 204e 6f6e 652c  dir is not None,
-00016030: 2072 6574 7572 6e73 2074 6865 2070 6174   returns the pat
-00016040: 6873 206f 6620 7468 6520 7265 2d73 697a  hs of the re-siz
-00016050: 6564 2076 6964 656f 732e 2045 6c73 6520  ed videos. Else 
-00016060: 7265 7475 726e 7320 656d 7074 7920 6c69  returns empty li
-00016070: 7374 2e0a 0a20 2020 203a 6578 616d 706c  st...    :exampl
-00016080: 653a 0a20 2020 203e 3e3e 2076 6964 656f  e:.    >>> video
-00016090: 5f70 6174 6873 3d20 5b27 2f55 7365 7273  _paths= ['/Users
-000160a0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-000160b0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-000160c0: 6573 686f 6f74 696e 672f 5241 545f 4e4f  eshooting/RAT_NO
-000160d0: 522f 7072 6f6a 6563 745f 666f 6c64 6572  R/project_folder
-000160e0: 2f76 6964 656f 732f 7465 7374 2f30 3831  /videos/test/081
-000160f0: 3032 3032 315f 444f 545f 5261 7437 5f38  02021_DOT_Rat7_8
-00016100: 2832 292e 6d70 3427 2c20 272f 5573 6572  (2).mp4', '/User
-00016110: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
-00016120: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
-00016130: 6c65 7368 6f6f 7469 6e67 2f52 4154 5f4e  leshooting/RAT_N
-00016140: 4f52 2f70 726f 6a65 6374 5f66 6f6c 6465  OR/project_folde
-00016150: 722f 7669 6465 6f73 2f74 6573 742f 3038  r/videos/test/08
-00016160: 3130 3230 3231 5f44 4f54 5f52 6174 3131  102021_DOT_Rat11
-00016170: 5f31 322e 6d70 3427 5d0a 2020 2020 3e3e  _12.mp4'].    >>
-00016180: 3e20 5f20 3d20 7265 7369 7a65 5f76 6964  > _ = resize_vid
-00016190: 656f 735f 6279 5f77 6964 7468 2876 6964  eos_by_width(vid
-000161a0: 656f 5f70 6174 6873 3d76 6964 656f 5f70  eo_paths=video_p
-000161b0: 6174 6873 2c20 7769 6474 683d 3330 302c  aths, width=300,
-000161c0: 206f 7665 7277 7269 7465 3d46 616c 7365   overwrite=False
-000161d0: 2c20 7361 7665 5f64 6972 3d27 2f55 7365  , save_dir='/Use
-000161e0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-000161f0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-00016200: 626c 6573 686f 6f74 696e 672f 5241 545f  bleshooting/RAT_
-00016210: 4e4f 522f 7072 6f6a 6563 745f 666f 6c64  NOR/project_fold
-00016220: 6572 2f76 6964 656f 732f 7465 7374 2f6e  er/videos/test/n
-00016230: 6577 2729 0a20 2020 2022 2222 0a0a 2020  ew').    """..  
-00016240: 2020 7469 6d65 7220 3d20 5369 6d62 6154    timer = SimbaT
-00016250: 696d 6572 2873 7461 7274 3d54 7275 6529  imer(start=True)
-00016260: 0a20 2020 2069 6620 286e 6f74 206f 7665  .    if (not ove
-00016270: 7277 7269 7465 2920 616e 6420 2873 6176  rwrite) and (sav
-00016280: 655f 6469 7220 6973 204e 6f6e 6529 3a0a  e_dir is None):.
-00016290: 2020 2020 2020 2020 7261 6973 6520 496e          raise In
-000162a0: 7661 6c69 6449 6e70 7574 4572 726f 7228  validInputError(
-000162b0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-000162c0: 3d22 5072 6f76 6964 6520 6120 7361 7665  ="Provide a save
-000162d0: 5f64 6972 206f 7220 7365 7420 6f76 6572  _dir or set over
-000162e0: 7772 6974 6520 746f 2054 7275 6522 2c0a  write to True",.
-000162f0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00016300: 6365 3d72 6573 697a 655f 7669 6465 6f73  ce=resize_videos
-00016310: 5f62 795f 7769 6474 682e 5f5f 6e61 6d65  _by_width.__name
-00016320: 5f5f 2c0a 2020 2020 2020 2020 290a 2020  __,.        ).  
-00016330: 2020 656c 6966 2028 6f76 6572 7772 6974    elif (overwrit
-00016340: 6529 2061 6e64 2028 7361 7665 5f64 6972  e) and (save_dir
-00016350: 2069 7320 6e6f 7420 4e6f 6e65 293a 0a20   is not None):. 
-00016360: 2020 2020 2020 2072 6169 7365 2049 6e76         raise Inv
-00016370: 616c 6964 496e 7075 7445 7272 6f72 280a  alidInputError(.
-00016380: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-00016390: 2253 6574 2045 4954 4845 5220 6f76 6572  "Set EITHER over
-000163a0: 7772 6974 6520 746f 2054 7275 6520 4f52  write to True OR
-000163b0: 2050 726f 7669 6465 2061 2073 6176 655f   Provide a save_
-000163c0: 6469 7222 2c0a 2020 2020 2020 2020 2020  dir",.          
-000163d0: 2020 736f 7572 6365 3d72 6573 697a 655f    source=resize_
-000163e0: 7669 6465 6f73 5f62 795f 7769 6474 682e  videos_by_width.
-000163f0: 5f5f 6e61 6d65 5f5f 2c0a 2020 2020 2020  __name__,.      
-00016400: 2020 290a 2020 2020 6966 2073 6176 655f    ).    if save_
-00016410: 6469 7220 6973 206e 6f74 204e 6f6e 653a  dir is not None:
-00016420: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00016430: 6f73 2e70 6174 682e 6973 6469 7228 7361  os.path.isdir(sa
-00016440: 7665 5f64 6972 293a 0a20 2020 2020 2020  ve_dir):.       
-00016450: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
-00016460: 2873 6176 655f 6469 7229 0a20 2020 2063  (save_dir).    c
-00016470: 6865 636b 5f76 616c 6964 5f6c 7374 2864  heck_valid_lst(d
-00016480: 6174 613d 7669 6465 6f5f 7061 7468 732c  ata=video_paths,
-00016490: 2073 6f75 7263 653d 7265 7369 7a65 5f76   source=resize_v
-000164a0: 6964 656f 735f 6279 5f77 6964 7468 2e5f  ideos_by_width._
-000164b0: 5f6e 616d 655f 5f2c 206d 696e 5f6c 656e  _name__, min_len
-000164c0: 3d31 290a 2020 2020 5f20 3d20 5b63 6865  =1).    _ = [che
-000164d0: 636b 5f66 696c 655f 6578 6973 745f 616e  ck_file_exist_an
-000164e0: 645f 7265 6164 6162 6c65 2878 2920 666f  d_readable(x) fo
-000164f0: 7220 7820 696e 2076 6964 656f 5f70 6174  r x in video_pat
-00016500: 6873 5d0a 2020 2020 6e65 775f 7669 6465  hs].    new_vide
-00016510: 6f5f 7061 7468 7320 3d20 5b5d 0a20 2020  o_paths = [].   
-00016520: 2069 6620 6973 696e 7374 616e 6365 2877   if isinstance(w
-00016530: 6964 7468 2c20 7374 7229 3a0a 2020 2020  idth, str):.    
-00016540: 2020 2020 6368 6563 6b5f 696e 7428 0a20      check_int(. 
-00016550: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00016560: 6622 7b72 6573 697a 655f 7669 6465 6f73  f"{resize_videos
-00016570: 5f62 795f 7769 6474 682e 5f5f 6e61 6d65  _by_width.__name
-00016580: 5f5f 7d20 6865 6967 6874 222c 0a20 2020  __} height",.   
-00016590: 2020 2020 2020 2020 2076 616c 7565 3d77           value=w
-000165a0: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
-000165b0: 2020 6d69 6e5f 7661 6c75 653d 302c 0a20    min_value=0,. 
-000165c0: 2020 2020 2020 2020 2020 206d 6178 5f76             max_v
-000165d0: 616c 7565 3d6c 656e 2876 6964 656f 5f70  alue=len(video_p
-000165e0: 6174 6873 292c 0a20 2020 2020 2020 2029  aths),.        )
-000165f0: 0a20 2020 2020 2020 2076 6964 656f 5f77  .        video_w
-00016600: 6964 7468 7320 3d20 5b5d 0a20 2020 2020  idths = [].     
-00016610: 2020 2066 6f72 2069 2069 6e20 7669 6465     for i in vide
-00016620: 6f5f 7061 7468 733a 0a20 2020 2020 2020  o_paths:.       
-00016630: 2020 2020 2076 6964 656f 5f77 6964 7468       video_width
-00016640: 732e 6170 7065 6e64 2867 6574 5f76 6964  s.append(get_vid
-00016650: 656f 5f6d 6574 615f 6461 7461 2876 6964  eo_meta_data(vid
-00016660: 656f 5f70 6174 683d 6929 5b22 7769 6474  eo_path=i)["widt
-00016670: 6822 5d29 0a20 2020 2020 2020 2077 6964  h"]).        wid
-00016680: 7468 203d 2076 6964 656f 5f77 6964 7468  th = video_width
-00016690: 735b 696e 7428 7769 6474 6829 5d0a 2020  s[int(width)].  
-000166a0: 2020 666f 7220 636e 742c 2076 6964 656f    for cnt, video
-000166b0: 5f70 6174 6820 696e 2065 6e75 6d65 7261  _path in enumera
-000166c0: 7465 2876 6964 656f 5f70 6174 6873 293a  te(video_paths):
-000166d0: 0a20 2020 2020 2020 2064 6972 5f6e 616d  .        dir_nam
-000166e0: 652c 2076 6964 656f 5f6e 616d 652c 2065  e, video_name, e
-000166f0: 7874 203d 2067 6574 5f66 6e5f 6578 7428  xt = get_fn_ext(
-00016700: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-00016710: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00016720: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016730: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00016740: 2020 2066 2252 6573 697a 696e 6720 7769     f"Resizing wi
-00016750: 6474 6820 7669 6465 6f20 7b76 6964 656f  dth video {video
-00016760: 5f6e 616d 657d 2028 5669 6465 6f20 7b63  _name} (Video {c
-00016770: 6e74 2b31 7d2f 7b6c 656e 2876 6964 656f  nt+1}/{len(video
-00016780: 5f70 6174 6873 297d 292e 2e2e 220a 2020  _paths)})...".  
-00016790: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000167a0: 2020 2020 6966 206f 7665 7277 7269 7465      if overwrite
-000167b0: 3a0a 2020 2020 2020 2020 2020 2020 6474  :.            dt
-000167c0: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
-000167d0: 292e 7374 7266 7469 6d65 2822 2559 256d  ).strftime("%Y%m
-000167e0: 2564 2548 254d 2553 2229 0a20 2020 2020  %d%H%M%S").     
-000167f0: 2020 2020 2020 2073 6176 655f 7061 7468         save_path
-00016800: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00016810: 6469 725f 6e61 6d65 2c20 6622 7b76 6964  dir_name, f"{vid
-00016820: 656f 5f6e 616d 657d 5f7b 6474 7d2e 6d70  eo_name}_{dt}.mp
-00016830: 3422 290a 2020 2020 2020 2020 656c 7365  4").        else
-00016840: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
-00016850: 7665 5f70 6174 6820 3d20 6f73 2e70 6174  ve_path = os.pat
-00016860: 682e 6a6f 696e 2873 6176 655f 6469 722c  h.join(save_dir,
-00016870: 2066 227b 7669 6465 6f5f 6e61 6d65 7d2e   f"{video_name}.
-00016880: 6d70 3422 290a 2020 2020 2020 2020 2020  mp4").          
-00016890: 2020 6e65 775f 7669 6465 6f5f 7061 7468    new_video_path
-000168a0: 732e 6170 7065 6e64 2873 6176 655f 7061  s.append(save_pa
-000168b0: 7468 290a 2020 2020 2020 2020 6966 2067  th).        if g
-000168c0: 7075 3a0a 2020 2020 2020 2020 2020 2020  pu:.            
-000168d0: 636d 6420 3d20 6627 6666 6d70 6567 202d  cmd = f'ffmpeg -
-000168e0: 7920 2d68 7761 6363 656c 2061 7574 6f20  y -hwaccel auto 
-000168f0: 2d69 2022 7b76 6964 656f 5f70 6174 687d  -i "{video_path}
-00016900: 2220 2d76 6620 7363 616c 655f 6e70 703d  " -vf scale_npp=
-00016910: 7b77 6964 7468 7d3a 2d32 202d 633a 7620  {width}:-2 -c:v 
-00016920: 6832 3634 5f6e 7665 6e63 2022 7b73 6176  h264_nvenc "{sav
-00016930: 655f 7061 7468 7d22 202d 6869 6465 5f62  e_path}" -hide_b
-00016940: 616e 6e65 7220 2d6c 6f67 6c65 7665 6c20  anner -loglevel 
-00016950: 6572 726f 7220 2d79 270a 2020 2020 2020  error -y'.      
-00016960: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00016970: 2020 2020 636d 6420 3d20 6627 6666 6d70      cmd = f'ffmp
-00016980: 6567 202d 7920 2d69 2022 7b76 6964 656f  eg -y -i "{video
-00016990: 5f70 6174 687d 2220 2d76 6620 7363 616c  _path}" -vf scal
-000169a0: 653d 7b77 6964 7468 7d3a 2d32 2022 7b73  e={width}:-2 "{s
-000169b0: 6176 655f 7061 7468 7d22 202d 6869 6465  ave_path}" -hide
-000169c0: 5f62 616e 6e65 7220 2d6c 6f67 6c65 7665  _banner -logleve
-000169d0: 6c20 6572 726f 7220 2d79 270a 2020 2020  l error -y'.    
-000169e0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
-000169f0: 616c 6c28 636d 642c 2073 6865 6c6c 3d54  all(cmd, shell=T
-00016a00: 7275 652c 2073 7464 6f75 743d 7375 6270  rue, stdout=subp
-00016a10: 726f 6365 7373 2e50 4950 4529 0a20 2020  rocess.PIPE).   
-00016a20: 2020 2020 2069 6620 6f76 6572 7772 6974       if overwrit
-00016a30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00016a40: 6875 7469 6c2e 636f 7079 2873 6176 655f  hutil.copy(save_
-00016a50: 7061 7468 2c20 7669 6465 6f5f 7061 7468  path, video_path
-00016a60: 290a 2020 2020 2020 2020 2020 2020 6f73  ).            os
-00016a70: 2e72 656d 6f76 6528 7361 7665 5f70 6174  .remove(save_pat
-00016a80: 6829 0a20 2020 2074 696d 6572 2e73 746f  h).    timer.sto
-00016a90: 705f 7469 6d65 7228 290a 2020 2020 6966  p_timer().    if
-00016aa0: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00016ab0: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
-00016ac0: 2020 2020 2066 2252 6573 697a 6564 2077       f"Resized w
-00016ad0: 6964 7468 207b 6c65 6e28 7669 6465 6f5f  idth {len(video_
-00016ae0: 7061 7468 7329 7d20 7669 6465 6f28 7329  paths)} video(s)
-00016af0: 2e20 456c 6170 7365 6420 7469 6d65 3a20  . Elapsed time: 
-00016b00: 7b74 696d 6572 2e65 6c61 7073 6564 5f74  {timer.elapsed_t
-00016b10: 696d 655f 7374 727d 732e 220a 2020 2020  ime_str}s.".    
-00016b20: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00016b30: 206e 6577 5f76 6964 656f 5f70 6174 6873   new_video_paths
-00016b40: 0a0a 0a64 6566 2063 7265 6174 655f 626c  ...def create_bl
-00016b50: 616e 6b5f 7669 6465 6f28 0a20 2020 2070  ank_video(.    p
-00016b60: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00016b70: 6f73 2e50 6174 684c 696b 655d 2c0a 2020  os.PathLike],.  
-00016b80: 2020 6c65 6e67 7468 3a20 696e 742c 0a20    length: int,. 
-00016b90: 2020 2077 6964 7468 3a20 696e 742c 0a20     width: int,. 
-00016ba0: 2020 2068 6569 6768 743a 2069 6e74 2c0a     height: int,.
-00016bb0: 2020 2020 636f 6c6f 723a 204f 7074 696f      color: Optio
-00016bc0: 6e61 6c5b 7374 725d 203d 2022 626c 6163  nal[str] = "blac
-00016bd0: 6b22 2c0a 2020 2020 6770 753a 204f 7074  k",.    gpu: Opt
-00016be0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4661  ional[bool] = Fa
-00016bf0: 6c73 652c 0a20 2020 2076 6572 626f 7365  lse,.    verbose
-00016c00: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00016c10: 203d 2046 616c 7365 2c0a 2920 2d3e 204e   = False,.) -> N
-00016c20: 6f6e 653a 0a20 2020 2022 2222 0a20 2020  one:.    """.   
-00016c30: 2043 7265 6174 6520 6120 2262 6c61 6e6b   Create a "blank
-00016c40: 2220 756e 692d 636f 6c6f 7265 6420 7669  " uni-colored vi
-00016c50: 6465 6f20 6f66 2073 7065 6369 6669 6564  deo of specified
-00016c60: 2073 697a 6520 616e 6420 6c65 6e67 7468   size and length
-00016c70: 2e0a 0a20 2020 203a 7061 7261 6d20 556e  ...    :param Un
-00016c80: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00016c90: 4c69 6b65 5d20 7061 7468 3a20 4c6f 6361  Like] path: Loca
-00016ca0: 7469 6f6e 2077 6865 7265 2074 6f20 7374  tion where to st
-00016cb0: 6f72 6520 7468 6520 626c 616e 6b20 7669  ore the blank vi
-00016cc0: 6465 6f2e 0a20 2020 203a 7061 7261 6d20  deo..    :param 
-00016cd0: 696e 7420 6c65 6e67 7468 3a20 4c65 6e67  int length: Leng
-00016ce0: 7468 206f 6620 7468 6520 626c 616e 6b20  th of the blank 
-00016cf0: 7669 6465 6f20 696e 2073 6563 6f6e 6473  video in seconds
-00016d00: 2e0a 2020 2020 3a70 6172 616d 2069 6e74  ..    :param int
-00016d10: 2077 6964 7468 3a20 5769 6474 6820 6f66   width: Width of
-00016d20: 2074 6865 2062 6c61 6e6b 2076 6964 656f   the blank video
-00016d30: 2069 6e20 7069 7865 6c73 2e0a 2020 2020   in pixels..    
-00016d40: 3a70 6172 616d 2069 6e74 2068 6569 6768  :param int heigh
-00016d50: 743a 2048 6569 6768 7420 6f66 2074 6865  t: Height of the
-00016d60: 2062 6c61 6e6b 2076 6964 656f 2069 6e20   blank video in 
-00016d70: 7069 7865 6c73 2e0a 2020 2020 3a70 6172  pixels..    :par
-00016d80: 616d 204f 7074 696f 6e61 6c5b 7374 725d  am Optional[str]
-00016d90: 2063 6f6c 6f72 3a20 436f 6c6f 7220 6f66   color: Color of
-00016da0: 2074 6865 2062 6c61 6e6b 2076 6964 656f   the blank video
-00016db0: 2e20 4465 6661 756c 7420 626c 6163 6b2e  . Default black.
-00016dc0: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-00016dd0: 6f6e 616c 5b62 6f6f 6c5d 2067 7075 3a20  onal[bool] gpu: 
-00016de0: 4966 2054 7275 652c 2074 6865 6e20 7573  If True, then us
-00016df0: 6520 4646 6d70 6567 2047 5055 2063 6f64  e FFmpeg GPU cod
-00016e00: 6563 732e 2044 6566 6175 6c74 2046 616c  ecs. Default Fal
-00016e10: 7365 2e0a 2020 2020 3a70 6172 616d 204f  se..    :param O
-00016e20: 7074 696f 6e61 6c5b 626f 6f6c 5d20 7665  ptional[bool] ve
-00016e30: 7262 6f73 653a 2049 6620 5472 7565 2c20  rbose: If True, 
-00016e40: 7072 696e 7473 2070 726f 6772 6573 732e  prints progress.
-00016e50: 2044 6566 6175 6c74 2054 7275 652e 0a20   Default True.. 
-00016e60: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
-00016e70: 2e0a 0a20 2020 203a 6578 616d 706c 653a  ...    :example:
-00016e80: 0a20 2020 203e 3e3e 205f 203d 2063 7265  .    >>> _ = cre
-00016e90: 6174 655f 626c 616e 6b5f 7669 6465 6f28  ate_blank_video(
-00016ea0: 7061 7468 3d27 2f55 7365 7273 2f73 696d  path='/Users/sim
-00016eb0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-00016ec0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-00016ed0: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
-00016ee0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-00016ef0: 656f 732f 7465 7374 2f6e 6577 2f62 6c61  eos/test/new/bla
-00016f00: 6e6b 5f74 6573 742e 6d70 3427 2c20 6c65  nk_test.mp4', le
-00016f10: 6e67 7468 3d35 2c20 7769 6474 683d 3330  ngth=5, width=30
-00016f20: 302c 2068 6569 6768 743d 3430 302c 2067  0, height=400, g
-00016f30: 7075 3d46 616c 7365 2c20 7665 7262 6f73  pu=False, verbos
-00016f40: 653d 5472 7565 2c20 636f 6c6f 723d 276f  e=True, color='o
-00016f50: 7261 6e67 6527 290a 2020 2020 2222 220a  range').    """.
-00016f60: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
-00016f70: 616d 653d 6622 7b63 7265 6174 655f 626c  ame=f"{create_bl
-00016f80: 616e 6b5f 7669 6465 6f2e 5f5f 6e61 6d65  ank_video.__name
-00016f90: 5f5f 7d20 6c65 6e67 7468 222c 2076 616c  __} length", val
-00016fa0: 7565 3d6c 656e 6774 682c 206d 696e 5f76  ue=length, min_v
-00016fb0: 616c 7565 3d31 290a 2020 2020 6368 6563  alue=1).    chec
-00016fc0: 6b5f 696e 7428 6e61 6d65 3d66 227b 6372  k_int(name=f"{cr
-00016fd0: 6561 7465 5f62 6c61 6e6b 5f76 6964 656f  eate_blank_video
-00016fe0: 2e5f 5f6e 616d 655f 5f7d 2077 6964 7468  .__name__} width
-00016ff0: 222c 2076 616c 7565 3d77 6964 7468 2c20  ", value=width, 
-00017000: 6d69 6e5f 7661 6c75 653d 3129 0a20 2020  min_value=1).   
-00017010: 2063 6865 636b 5f69 6e74 286e 616d 653d   check_int(name=
-00017020: 6622 7b63 7265 6174 655f 626c 616e 6b5f  f"{create_blank_
-00017030: 7669 6465 6f2e 5f5f 6e61 6d65 5f5f 7d20  video.__name__} 
-00017040: 6865 6967 6874 222c 2076 616c 7565 3d68  height", value=h
-00017050: 6569 6768 742c 206d 696e 5f76 616c 7565  eight, min_value
-00017060: 3d31 290a 2020 2020 6368 6563 6b5f 6966  =1).    check_if
-00017070: 5f64 6972 5f65 7869 7374 7328 0a20 2020  _dir_exists(.   
-00017080: 2020 2020 2069 6e5f 6469 723d 6f73 2e70       in_dir=os.p
-00017090: 6174 682e 6469 726e 616d 6528 7061 7468  ath.dirname(path
-000170a0: 292c 0a20 2020 2020 2020 2073 6f75 7263  ),.        sourc
-000170b0: 653d 6372 6561 7465 5f62 6c61 6e6b 5f76  e=create_blank_v
-000170c0: 6964 656f 2e5f 5f6e 616d 655f 5f2c 0a20  ideo.__name__,. 
-000170d0: 2020 2020 2020 2063 7265 6174 655f 6966         create_if
-000170e0: 5f6e 6f74 5f65 7869 7374 3d54 7275 652c  _not_exist=True,
-000170f0: 0a20 2020 2029 0a20 2020 2074 696d 6572  .    ).    timer
-00017100: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
-00017110: 6172 743d 5472 7565 290a 2020 2020 6966  art=True).    if
-00017120: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00017130: 2020 7072 696e 7428 2243 7265 6174 696e    print("Creatin
-00017140: 6720 626c 616e 6b20 7669 6465 6f2e 2e2e  g blank video...
-00017150: 2229 0a20 2020 2069 6620 6770 753a 0a20  ").    if gpu:. 
-00017160: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
-00017170: 666d 7065 6720 2d79 202d 7420 7b6c 656e  fmpeg -y -t {len
-00017180: 6774 687d 202d 6620 6c61 7666 6920 2d69  gth} -f lavfi -i
-00017190: 2063 6f6c 6f72 3d63 3d7b 636f 6c6f 727d   color=c={color}
-000171a0: 3a73 3d7b 7769 6474 687d 787b 6865 6967  :s={width}x{heig
-000171b0: 6874 7d20 2d63 3a76 2068 3236 345f 6e76  ht} -c:v h264_nv
-000171c0: 656e 6320 2d70 7265 7365 7420 736c 6f77  enc -preset slow
-000171d0: 202d 7475 6e65 2073 7469 6c6c 696d 6167   -tune stillimag
-000171e0: 6520 2d70 6978 5f66 6d74 2079 7576 3432  e -pix_fmt yuv42
-000171f0: 3070 2022 7b70 6174 687d 2220 2d68 6964  0p "{path}" -hid
-00017200: 655f 6261 6e6e 6572 202d 6c6f 676c 6576  e_banner -loglev
-00017210: 656c 2065 7272 6f72 202d 7927 0a20 2020  el error -y'.   
-00017220: 2065 6c73 653a 0a20 2020 2020 2020 2063   else:.        c
-00017230: 6d64 203d 2066 2766 666d 7065 6720 2d79  md = f'ffmpeg -y
-00017240: 202d 7420 7b6c 656e 6774 687d 202d 6620   -t {length} -f 
-00017250: 6c61 7666 6920 2d69 2063 6f6c 6f72 3d63  lavfi -i color=c
-00017260: 3d7b 636f 6c6f 727d 3a73 3d7b 7769 6474  ={color}:s={widt
-00017270: 687d 787b 6865 6967 6874 7d20 2d63 3a76  h}x{height} -c:v
-00017280: 206c 6962 7832 3634 202d 7475 6e65 2073   libx264 -tune s
-00017290: 7469 6c6c 696d 6167 6520 2d70 6978 5f66  tillimage -pix_f
-000172a0: 6d74 2079 7576 3432 3070 2022 7b70 6174  mt yuv420p "{pat
-000172b0: 687d 2220 2d68 6964 655f 6261 6e6e 6572  h}" -hide_banner
-000172c0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
-000172d0: 202d 7927 0a20 2020 2073 7562 7072 6f63   -y'.    subproc
-000172e0: 6573 732e 6361 6c6c 2863 6d64 2c20 7368  ess.call(cmd, sh
-000172f0: 656c 6c3d 5472 7565 2c20 7374 646f 7574  ell=True, stdout
-00017300: 3d73 7562 7072 6f63 6573 732e 5049 5045  =subprocess.PIPE
-00017310: 290a 2020 2020 7469 6d65 722e 7374 6f70  ).    timer.stop
-00017320: 5f74 696d 6572 2829 0a20 2020 2069 6620  _timer().    if 
-00017330: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-00017340: 2070 7269 6e74 280a 2020 2020 2020 2020   print(.        
-00017350: 2020 2020 6622 426c 616e 6b20 7669 6465      f"Blank vide
-00017360: 6f20 636f 6d70 6c65 7465 2e20 5361 7665  o complete. Save
-00017370: 6420 6174 207b 7061 7468 7d2e 2045 6c61  d at {path}. Ela
-00017380: 7073 6564 2074 696d 653a 207b 7469 6d65  psed time: {time
-00017390: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
-000173a0: 7472 7d73 2e22 0a20 2020 2020 2020 2029  tr}s.".        )
-000173b0: 0a0a 0a64 6566 2068 6f72 697a 6f6e 7461  ...def horizonta
-000173c0: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-000173d0: 6174 6f72 280a 2020 2020 7669 6465 6f5f  ator(.    video_
-000173e0: 7061 7468 733a 204c 6973 745b 556e 696f  paths: List[Unio
-000173f0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00017400: 6b65 5d5d 2c0a 2020 2020 7361 7665 5f70  ke]],.    save_p
-00017410: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00017420: 6f73 2e50 6174 684c 696b 655d 2c0a 2020  os.PathLike],.  
-00017430: 2020 6865 6967 6874 5f70 783a 204f 7074    height_px: Opt
-00017440: 696f 6e61 6c5b 556e 696f 6e5b 696e 742c  ional[Union[int,
-00017450: 2073 7472 5d5d 203d 204e 6f6e 652c 0a20   str]] = None,. 
-00017460: 2020 2068 6569 6768 745f 6964 783a 204f     height_idx: O
-00017470: 7074 696f 6e61 6c5b 556e 696f 6e5b 696e  ptional[Union[in
-00017480: 742c 2073 7472 5d5d 203d 204e 6f6e 652c  t, str]] = None,
-00017490: 0a20 2020 2067 7075 3a20 4f70 7469 6f6e  .    gpu: Option
-000174a0: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
-000174b0: 2c0a 2020 2020 7665 7262 6f73 653a 204f  ,.    verbose: O
-000174c0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-000174d0: 5472 7565 2c0a 2920 2d3e 204e 6f6e 653a  True,.) -> None:
-000174e0: 0a20 2020 2022 2222 0a20 2020 2043 6f6e  .    """.    Con
-000174f0: 6361 7465 6e61 7465 7320 6d75 6c74 6970  catenates multip
-00017500: 6c65 2076 6964 656f 7320 686f 7269 7a6f  le videos horizo
-00017510: 6e74 616c 6c79 2e0a 0a20 2020 202e 2e20  ntally...    .. 
-00017520: 696d 6167 653a 3a20 5f73 7461 7469 632f  image:: _static/
-00017530: 696d 672f 686f 7269 7a6f 6e74 616c 5f76  img/horizontal_v
-00017540: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
-00017550: 722e 6769 660a 2020 2020 2020 203a 7769  r.gif.       :wi
-00017560: 6474 683a 2036 3030 0a20 2020 2020 2020  dth: 600.       
-00017570: 3a61 6c69 676e 3a20 6365 6e74 6572 0a0a  :align: center..
-00017580: 2020 2020 3a70 6172 616d 204c 6973 745b      :param List[
-00017590: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-000175a0: 7468 4c69 6b65 5d5d 2076 6964 656f 5f70  thLike]] video_p
-000175b0: 6174 6873 3a20 4c69 7374 206f 6620 696e  aths: List of in
-000175c0: 7075 7420 7669 6465 6f20 6669 6c65 2070  put video file p
-000175d0: 6174 6873 2e0a 2020 2020 3a70 6172 616d  aths..    :param
-000175e0: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-000175f0: 6174 684c 696b 655d 2073 6176 655f 7061  athLike] save_pa
-00017600: 7468 3a20 4669 6c65 2070 6174 6820 746f  th: File path to
-00017610: 2073 6176 6520 7468 6520 636f 6e63 6174   save the concat
-00017620: 656e 6174 6564 2076 6964 656f 2e0a 2020  enated video..  
-00017630: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00017640: 6c5b 696e 745d 2068 6569 6768 745f 7078  l[int] height_px
-00017650: 3a20 4865 6967 6874 206f 6620 7468 6520  : Height of the 
-00017660: 6f75 7470 7574 2076 6964 656f 2069 6e20  output video in 
-00017670: 7069 7865 6c73 2e0a 2020 2020 3a70 6172  pixels..    :par
-00017680: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
-00017690: 2068 6569 6768 745f 6964 783a 2049 6e64   height_idx: Ind
-000176a0: 6578 206f 6620 7468 6520 7669 6465 6f20  ex of the video 
-000176b0: 746f 2075 7365 2066 6f72 2064 6574 6572  to use for deter
-000176c0: 6d69 6e69 6e67 2048 6569 6768 742e 0a20  mining Height.. 
-000176d0: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
-000176e0: 616c 5b62 6f6f 6c5d 2067 7075 3a20 5768  al[bool] gpu: Wh
-000176f0: 6574 6865 7220 746f 2075 7365 2047 5055  ether to use GPU
-00017700: 2d61 6363 656c 6572 6174 6564 2063 6f64  -accelerated cod
-00017710: 6563 2028 6465 6661 756c 743a 2046 616c  ec (default: Fal
-00017720: 7365 292e 0a20 2020 203a 7061 7261 6d20  se)..    :param 
-00017730: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 2076  Optional[bool] v
-00017740: 6572 626f 7365 3a57 6865 7468 6572 2074  erbose:Whether t
-00017750: 6f20 7072 696e 7420 7072 6f67 7265 7373  o print progress
-00017760: 206d 6573 7361 6765 7320 2864 6566 6175   messages (defau
-00017770: 6c74 3a20 5472 7565 292e 0a0a 2020 2020  lt: True)...    
-00017780: 3a65 7861 6d70 6c65 3a0a 2020 2020 3e3e  :example:.    >>
-00017790: 3e20 7669 6465 6f5f 7061 7468 7320 3d20  > video_paths = 
-000177a0: 5b27 7669 6465 6f31 2e6d 7034 272c 2027  ['video1.mp4', '
-000177b0: 7669 6465 6f32 2e6d 7034 275d 0a20 2020  video2.mp4'].   
-000177c0: 203e 3e3e 2078 203d 2068 6f72 697a 6f6e   >>> x = horizon
-000177d0: 7461 6c5f 7669 6465 6f5f 636f 6e63 6174  tal_video_concat
-000177e0: 656e 6174 6f72 2876 6964 656f 5f70 6174  enator(video_pat
-000177f0: 6873 3d76 6964 656f 5f70 6174 6873 2c20  hs=video_paths, 
-00017800: 6865 6967 6874 5f70 783d 3530 2c20 7361  height_px=50, sa
-00017810: 7665 5f70 6174 683d 272f 5573 6572 732f  ve_path='/Users/
-00017820: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-00017830: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-00017840: 7368 6f6f 7469 6e67 2f52 4154 5f4e 4f52  shooting/RAT_NOR
-00017850: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
-00017860: 7669 6465 6f73 2f74 6573 742f 6e65 772f  videos/test/new/
-00017870: 3038 3130 3230 3231 5f44 4f54 5f52 6174  08102021_DOT_Rat
-00017880: 375f 3828 3229 5f2e 6d70 3427 2c20 6770  7_8(2)_.mp4', gp
-00017890: 753d 4661 6c73 6529 0a20 2020 2022 2222  u=False).    """
-000178a0: 0a20 2020 2063 6865 636b 5f66 666d 7065  .    check_ffmpe
-000178b0: 675f 6176 6169 6c61 626c 6528 290a 2020  g_available().  
-000178c0: 2020 6966 2067 7075 2061 6e64 206e 6f74    if gpu and not
-000178d0: 2063 6865 636b 5f6e 7669 6465 615f 6770   check_nvidea_gp
-000178e0: 755f 6176 6169 6c61 626c 6528 293a 0a20  u_available():. 
-000178f0: 2020 2020 2020 2072 6169 7365 2046 464d         raise FFM
-00017900: 5045 4743 6f64 6563 4750 5545 7272 6f72  PEGCodecGPUError
-00017910: 280a 2020 2020 2020 2020 2020 2020 6d73  (.            ms
-00017920: 673d 224e 5649 4445 4120 4750 5520 6e6f  g="NVIDEA GPU no
-00017930: 7420 6176 6169 6c61 626c 6520 2861 7320  t available (as 
-00017940: 6576 616c 7561 7465 6420 6279 206e 7669  evaluated by nvi
-00017950: 6465 612d 736d 6920 7265 7475 726e 696e  dea-smi returnin
-00017960: 6720 4e6f 6e65 2922 2c0a 2020 2020 2020  g None)",.      
-00017970: 2020 2020 2020 736f 7572 6365 3d68 6f72        source=hor
-00017980: 697a 6f6e 7461 6c5f 7669 6465 6f5f 636f  izontal_video_co
-00017990: 6e63 6174 656e 6174 6f72 2e5f 5f6e 616d  ncatenator.__nam
-000179a0: 655f 5f2c 0a20 2020 2020 2020 2029 0a20  e__,.        ). 
-000179b0: 2020 2074 696d 6572 203d 2053 696d 6261     timer = Simba
-000179c0: 5469 6d65 7228 7374 6172 743d 5472 7565  Timer(start=True
-000179d0: 290a 2020 2020 6368 6563 6b5f 7661 6c69  ).    check_vali
-000179e0: 645f 6c73 7428 0a20 2020 2020 2020 2064  d_lst(.        d
-000179f0: 6174 613d 7669 6465 6f5f 7061 7468 732c  ata=video_paths,
-00017a00: 2073 6f75 7263 653d 686f 7269 7a6f 6e74   source=horizont
-00017a10: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
-00017a20: 6e61 746f 722e 5f5f 6e61 6d65 5f5f 2c20  nator.__name__, 
-00017a30: 6d69 6e5f 6c65 6e3d 320a 2020 2020 290a  min_len=2.    ).
-00017a40: 2020 2020 6368 6563 6b5f 6966 5f64 6972      check_if_dir
-00017a50: 5f65 7869 7374 7328 0a20 2020 2020 2020  _exists(.       
-00017a60: 2069 6e5f 6469 723d 6f73 2e70 6174 682e   in_dir=os.path.
-00017a70: 6469 726e 616d 6528 7361 7665 5f70 6174  dirname(save_pat
-00017a80: 6829 2c20 736f 7572 6365 3d68 6f72 697a  h), source=horiz
-00017a90: 6f6e 7461 6c5f 7669 6465 6f5f 636f 6e63  ontal_video_conc
-00017aa0: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
-00017ab0: 5f0a 2020 2020 290a 2020 2020 7669 6465  _.    ).    vide
-00017ac0: 6f5f 6d65 7461 5f64 6174 6120 3d20 5b0a  o_meta_data = [.
-00017ad0: 2020 2020 2020 2020 6765 745f 7669 6465          get_vide
-00017ae0: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
-00017af0: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
-00017b00: 6829 2066 6f72 2076 6964 656f 5f70 6174  h) for video_pat
-00017b10: 6820 696e 2076 6964 656f 5f70 6174 6873  h in video_paths
-00017b20: 0a20 2020 205d 0a20 2020 2069 6620 2828  .    ].    if ((
-00017b30: 6865 6967 6874 5f70 7820 6973 204e 6f6e  height_px is Non
-00017b40: 6529 2061 6e64 2028 6865 6967 6874 5f69  e) and (height_i
-00017b50: 6478 2069 7320 4e6f 6e65 2929 206f 7220  dx is None)) or 
-00017b60: 280a 2020 2020 2020 2020 2868 6569 6768  (.        (heigh
-00017b70: 745f 7078 2069 7320 6e6f 7420 4e6f 6e65  t_px is not None
-00017b80: 2920 616e 6420 2868 6569 6768 745f 6964  ) and (height_id
-00017b90: 7820 6973 206e 6f74 204e 6f6e 6529 0a20  x is not None). 
-00017ba0: 2020 2029 3a0a 2020 2020 2020 2020 7261     ):.        ra
-00017bb0: 6973 6520 496e 7661 6c69 6449 6e70 7574  ise InvalidInput
-00017bc0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00017bd0: 2020 206d 7367 3d22 5072 6f76 6964 6520     msg="Provide 
-00017be0: 6120 6865 6967 6874 5f70 7820 4f52 2068  a height_px OR h
-00017bf0: 6569 6768 745f 6964 7822 2c0a 2020 2020  eight_idx",.    
-00017c00: 2020 2020 2020 2020 736f 7572 6365 3d68          source=h
-00017c10: 6f72 697a 6f6e 7461 6c5f 7669 6465 6f5f  orizontal_video_
-00017c20: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
-00017c30: 616d 655f 5f2c 0a20 2020 2020 2020 2029  ame__,.        )
-00017c40: 0a20 2020 2069 6620 6865 6967 6874 5f69  .    if height_i
-00017c50: 6478 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dx is not None:.
-00017c60: 2020 2020 2020 2020 6368 6563 6b5f 696e          check_in
-00017c70: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
-00017c80: 616d 653d 6622 7b68 6f72 697a 6f6e 7461  ame=f"{horizonta
-00017c90: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-00017ca0: 6174 6f72 2e5f 5f6e 616d 655f 5f7d 2068  ator.__name__} h
-00017cb0: 6569 6768 7422 2c0a 2020 2020 2020 2020  eight",.        
-00017cc0: 2020 2020 7661 6c75 653d 6865 6967 6874      value=height
-00017cd0: 5f69 6478 2c0a 2020 2020 2020 2020 2020  _idx,.          
-00017ce0: 2020 6d69 6e5f 7661 6c75 653d 302c 0a20    min_value=0,. 
-00017cf0: 2020 2020 2020 2020 2020 206d 6178 5f76             max_v
-00017d00: 616c 7565 3d6c 656e 2876 6964 656f 5f70  alue=len(video_p
-00017d10: 6174 6873 2920 2d20 312c 0a20 2020 2020  aths) - 1,.     
-00017d20: 2020 2029 0a20 2020 2020 2020 2068 6569     ).        hei
-00017d30: 6768 7420 3d20 696e 7428 7669 6465 6f5f  ght = int(video_
-00017d40: 6d65 7461 5f64 6174 615b 6865 6967 6874  meta_data[height
-00017d50: 5f69 6478 5d5b 2268 6569 6768 7422 5d29  _idx]["height"])
-00017d60: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00017d70: 2020 2063 6865 636b 5f69 6e74 280a 2020     check_int(.  
-00017d80: 2020 2020 2020 2020 2020 6e61 6d65 3d66            name=f
-00017d90: 227b 686f 7269 7a6f 6e74 616c 5f76 6964  "{horizontal_vid
-00017da0: 656f 5f63 6f6e 6361 7465 6e61 746f 722e  eo_concatenator.
-00017db0: 5f5f 6e61 6d65 5f5f 7d20 6865 6967 6874  __name__} height
-00017dc0: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
-00017dd0: 616c 7565 3d68 6569 6768 745f 7078 2c0a  alue=height_px,.
-00017de0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-00017df0: 7661 6c75 653d 312c 0a20 2020 2020 2020  value=1,.       
-00017e00: 2029 0a20 2020 2020 2020 2068 6569 6768   ).        heigh
-00017e10: 7420 3d20 696e 7428 6865 6967 6874 5f70  t = int(height_p
-00017e20: 7829 0a20 2020 2076 6964 656f 5f70 6174  x).    video_pat
-00017e30: 685f 7374 7220 3d20 2220 222e 6a6f 696e  h_str = " ".join
-00017e40: 285b 6627 2d69 2022 7b70 6174 687d 2227  ([f'-i "{path}"'
-00017e50: 2066 6f72 2070 6174 6820 696e 2076 6964   for path in vid
-00017e60: 656f 5f70 6174 6873 5d29 0a20 2020 2063  eo_paths]).    c
-00017e70: 6f64 6563 203d 2022 6832 3634 5f6e 7665  odec = "h264_nve
-00017e80: 6e63 2220 6966 2067 7075 2065 6c73 6520  nc" if gpu else 
-00017e90: 226c 6962 7670 782d 7670 3922 0a20 2020  "libvpx-vp9".   
-00017ea0: 2066 696c 7465 725f 636f 6d70 6c65 7820   filter_complex 
-00017eb0: 3d20 223b 222e 6a6f 696e 280a 2020 2020  = ";".join(.    
-00017ec0: 2020 2020 5b66 225b 7b69 6478 7d3a 765d      [f"[{idx}:v]
-00017ed0: 7363 616c 653d 2d31 3a7b 6865 6967 6874  scale=-1:{height
-00017ee0: 7d5b 767b 6964 787d 5d22 2066 6f72 2069  }[v{idx}]" for i
-00017ef0: 6478 2069 6e20 7261 6e67 6528 6c65 6e28  dx in range(len(
-00017f00: 7669 6465 6f5f 7061 7468 7329 295d 0a20  video_paths))]. 
-00017f10: 2020 2029 0a20 2020 2066 696c 7465 725f     ).    filter_
-00017f20: 636f 6d70 6c65 7820 2b3d 2066 223b 7b27  complex += f";{'
-00017f30: 272e 6a6f 696e 285b 6627 5b76 7b69 6478  '.join([f'[v{idx
-00017f40: 7d5d 2720 666f 7220 6964 7820 696e 2072  }]' for idx in r
-00017f50: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
-00017f60: 6174 6873 2929 5d29 7d68 7374 6163 6b3d  aths))])}hstack=
-00017f70: 696e 7075 7473 3d7b 6c65 6e28 7669 6465  inputs={len(vide
-00017f80: 6f5f 7061 7468 7329 7d5b 765d 220a 2020  o_paths)}[v]".  
-00017f90: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00017fa0: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
-00017fb0: 2020 2020 2020 2020 2066 2243 6f6e 6361           f"Conca
-00017fc0: 7465 6e61 7469 6e67 207b 6c65 6e28 7669  tenating {len(vi
-00017fd0: 6465 6f5f 7061 7468 7329 7d20 7669 6465  deo_paths)} vide
-00017fe0: 6f73 2068 6f72 697a 6f6e 7461 6c6c 7920  os horizontally 
-00017ff0: 7769 7468 2061 207b 6865 6967 6874 7d20  with a {height} 
-00018000: 7069 7865 6c20 6865 6967 6874 2e2e 2e20  pixel height... 
-00018010: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-00018020: 636d 6420 3d20 6627 6666 6d70 6567 207b  cmd = f'ffmpeg {
-00018030: 7669 6465 6f5f 7061 7468 5f73 7472 7d20  video_path_str} 
-00018040: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
-00018050: 227b 6669 6c74 6572 5f63 6f6d 706c 6578  "{filter_complex
-00018060: 7d22 202d 6d61 7020 225b 765d 2220 2d63  }" -map "[v]" -c
-00018070: 3a76 207b 636f 6465 637d 202d 6c6f 676c  :v {codec} -logl
-00018080: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
-00018090: 7320 227b 7361 7665 5f70 6174 687d 2220  s "{save_path}" 
-000180a0: 2d79 270a 2020 2020 7375 6270 726f 6365  -y'.    subproce
-000180b0: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
-000180c0: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
-000180d0: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
-000180e0: 0a20 2020 2074 696d 6572 2e73 746f 705f  .    timer.stop_
-000180f0: 7469 6d65 7228 290a 2020 2020 6966 2076  timer().    if v
-00018100: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00018110: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00018120: 2020 2066 2248 6f72 697a 6f6e 7461 6c20     f"Horizontal 
-00018130: 636f 6e63 6174 656e 6174 696f 6e20 636f  concatenation co
-00018140: 6d70 6c65 7465 2c20 7361 7665 6420 6174  mplete, saved at
-00018150: 207b 7361 7665 5f70 6174 687d 2028 656c   {save_path} (el
-00018160: 6170 7365 6420 7469 6d65 3a20 7b74 696d  apsed time: {tim
-00018170: 6572 2e65 6c61 7073 6564 5f74 696d 655f  er.elapsed_time_
-00018180: 7374 727d 732e 2922 0a20 2020 2020 2020  str}s.)".       
-00018190: 2029 0a0a 0a64 6566 2076 6572 7469 6361   )...def vertica
-000181a0: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-000181b0: 6174 6f72 280a 2020 2020 7669 6465 6f5f  ator(.    video_
-000181c0: 7061 7468 733a 204c 6973 745b 556e 696f  paths: List[Unio
-000181d0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-000181e0: 6b65 5d5d 2c0a 2020 2020 7361 7665 5f70  ke]],.    save_p
-000181f0: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00018200: 6f73 2e50 6174 684c 696b 655d 2c0a 2020  os.PathLike],.  
-00018210: 2020 7769 6474 685f 7078 3a20 4f70 7469    width_px: Opti
-00018220: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00018230: 2c0a 2020 2020 7769 6474 685f 6964 783a  ,.    width_idx:
-00018240: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00018250: 204e 6f6e 652c 0a20 2020 2067 7075 3a20   None,.    gpu: 
-00018260: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00018270: 2046 616c 7365 2c0a 2020 2020 7665 7262   False,.    verb
-00018280: 6f73 653a 204f 7074 696f 6e61 6c5b 626f  ose: Optional[bo
-00018290: 6f6c 5d20 3d20 5472 7565 2c0a 2920 2d3e  ol] = True,.) ->
-000182a0: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-000182b0: 2020 2043 6f6e 6361 7465 6e61 7465 7320     Concatenates 
-000182c0: 6d75 6c74 6970 6c65 2076 6964 656f 7320  multiple videos 
-000182d0: 7665 7274 6963 616c 6c79 2e0a 0a20 2020  vertically...   
-000182e0: 202e 2e20 696d 6167 653a 3a20 5f73 7461   .. image:: _sta
-000182f0: 7469 632f 696d 672f 7665 7274 6963 616c  tic/img/vertical
-00018300: 5f76 6964 656f 5f63 6f6e 6361 7465 6e61  _video_concatena
-00018310: 746f 722e 706e 670a 2020 2020 2020 203a  tor.png.       :
-00018320: 7769 6474 683a 2033 3030 0a20 2020 2020  width: 300.     
-00018330: 2020 3a61 6c69 676e 3a20 6365 6e74 6572    :align: center
-00018340: 0a0a 2020 2020 3a70 6172 616d 204c 6973  ..    :param Lis
-00018350: 745b 556e 696f 6e5b 7374 722c 206f 732e  t[Union[str, os.
-00018360: 5061 7468 4c69 6b65 5d5d 2076 6964 656f  PathLike]] video
-00018370: 5f70 6174 6873 3a20 4c69 7374 206f 6620  _paths: List of 
-00018380: 696e 7075 7420 7669 6465 6f20 6669 6c65  input video file
-00018390: 2070 6174 6873 2e0a 2020 2020 3a70 6172   paths..    :par
-000183a0: 616d 2055 6e69 6f6e 5b73 7472 2c20 6f73  am Union[str, os
-000183b0: 2e50 6174 684c 696b 655d 2073 6176 655f  .PathLike] save_
-000183c0: 7061 7468 3a20 4669 6c65 2070 6174 6820  path: File path 
-000183d0: 746f 2073 6176 6520 7468 6520 636f 6e63  to save the conc
-000183e0: 6174 656e 6174 6564 2076 6964 656f 2e0a  atenated video..
-000183f0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-00018400: 6e61 6c5b 696e 745d 2077 6964 7468 5f70  nal[int] width_p
-00018410: 783a 2057 6964 7468 206f 6620 7468 6520  x: Width of the 
-00018420: 6f75 7470 7574 2076 6964 656f 2069 6e20  output video in 
-00018430: 7069 7865 6c73 2e0a 2020 2020 3a70 6172  pixels..    :par
-00018440: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
-00018450: 2077 6964 7468 5f69 6478 3a20 496e 6465   width_idx: Inde
-00018460: 7820 6f66 2074 6865 2076 6964 656f 2074  x of the video t
-00018470: 6f20 7573 6520 666f 7220 6465 7465 726d  o use for determ
-00018480: 696e 696e 6720 7769 6474 682e 0a20 2020  ining width..   
-00018490: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-000184a0: 5b62 6f6f 6c5d 2067 7075 3a20 5768 6574  [bool] gpu: Whet
-000184b0: 6865 7220 746f 2075 7365 2047 5055 2d61  her to use GPU-a
-000184c0: 6363 656c 6572 6174 6564 2063 6f64 6563  ccelerated codec
-000184d0: 2028 6465 6661 756c 743a 2046 616c 7365   (default: False
-000184e0: 292e 0a20 2020 203a 7061 7261 6d20 4f70  )..    :param Op
-000184f0: 7469 6f6e 616c 5b62 6f6f 6c5d 2076 6572  tional[bool] ver
-00018500: 626f 7365 3a57 6865 7468 6572 2074 6f20  bose:Whether to 
-00018510: 7072 696e 7420 7072 6f67 7265 7373 206d  print progress m
-00018520: 6573 7361 6765 7320 2864 6566 6175 6c74  essages (default
-00018530: 3a20 5472 7565 292e 0a20 2020 203a 7261  : True)..    :ra
-00018540: 6973 6573 2046 464d 5045 4743 6f64 6563  ises FFMPEGCodec
-00018550: 4750 5545 7272 6f72 3a20 4966 2047 5055  GPUError: If GPU
-00018560: 2069 7320 7265 7175 6573 7465 6420 6275   is requested bu
-00018570: 7420 6e6f 7420 6176 6169 6c61 626c 652e  t not available.
-00018580: 0a20 2020 203a 7261 6973 6573 2049 6e76  .    :raises Inv
-00018590: 616c 6964 496e 7075 7445 7272 6f72 3a20  alidInputError: 
-000185a0: 4966 2062 6f74 6820 6f72 206e 6569 7468  If both or neith
-000185b0: 6572 2077 6964 7468 5f70 7820 616e 6420  er width_px and 
-000185c0: 7769 6474 685f 6964 7820 6172 6520 7072  width_idx are pr
-000185d0: 6f76 6964 6564 2e0a 0a20 2020 203a 6578  ovided...    :ex
-000185e0: 616d 706c 653a 0a20 2020 203e 3e3e 2076  ample:.    >>> v
-000185f0: 6964 656f 5f70 6174 6873 203d 205b 272f  ideo_paths = ['/
-00018600: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-00018610: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-00018620: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
-00018630: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
-00018640: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
-00018650: 742f 3038 3130 3230 3231 5f44 4f54 5f52  t/08102021_DOT_R
-00018660: 6174 375f 3828 3229 2e6d 7034 272c 0a20  at7_8(2).mp4',. 
-00018670: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00018680: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
-00018690: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-000186a0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-000186b0: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
-000186c0: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-000186d0: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
-000186e0: 3231 5f44 4f54 5f52 6174 3131 5f31 322e  21_DOT_Rat11_12.
-000186f0: 6d70 3427 2c0a 2020 2020 3e3e 3e20 2020  mp4',.    >>>   
-00018700: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
-00018710: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-00018720: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-00018730: 6f75 626c 6573 686f 6f74 696e 672f 5241  oubleshooting/RA
-00018740: 545f 4e4f 522f 7072 6f6a 6563 745f 666f  T_NOR/project_fo
-00018750: 6c64 6572 2f76 6964 656f 732f 7465 7374  lder/videos/test
-00018760: 2f30 3831 3032 3032 315f 444f 545f 5261  /08102021_DOT_Ra
-00018770: 7431 315f 3132 5f31 2e6d 7034 275d 0a20  t11_12_1.mp4']. 
-00018780: 2020 203e 3e3e 205f 203d 2076 6572 7469     >>> _ = verti
-00018790: 6361 6c5f 7669 6465 6f5f 636f 6e63 6174  cal_video_concat
-000187a0: 656e 6174 6f72 2876 6964 656f 5f70 6174  enator(video_pat
-000187b0: 6873 3d76 6964 656f 5f70 6174 6873 2c20  hs=video_paths, 
-000187c0: 7769 6474 685f 6964 783d 312c 2073 6176  width_idx=1, sav
-000187d0: 655f 7061 7468 3d27 2f55 7365 7273 2f73  e_path='/Users/s
-000187e0: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-000187f0: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-00018800: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
-00018810: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-00018820: 6964 656f 732f 7465 7374 2f6e 6577 2f30  ideos/test/new/0
-00018830: 3831 3032 3032 315f 444f 545f 5261 7437  8102021_DOT_Rat7
-00018840: 5f38 2832 295f 2e6d 7034 272c 2067 7075  _8(2)_.mp4', gpu
-00018850: 3d46 616c 7365 290a 2020 2020 2222 220a  =False).    """.
-00018860: 0a20 2020 2063 6865 636b 5f66 666d 7065  .    check_ffmpe
-00018870: 675f 6176 6169 6c61 626c 6528 290a 2020  g_available().  
-00018880: 2020 6966 2067 7075 2061 6e64 206e 6f74    if gpu and not
-00018890: 2063 6865 636b 5f6e 7669 6465 615f 6770   check_nvidea_gp
-000188a0: 755f 6176 6169 6c61 626c 6528 293a 0a20  u_available():. 
-000188b0: 2020 2020 2020 2072 6169 7365 2046 464d         raise FFM
-000188c0: 5045 4743 6f64 6563 4750 5545 7272 6f72  PEGCodecGPUError
-000188d0: 280a 2020 2020 2020 2020 2020 2020 6d73  (.            ms
-000188e0: 673d 224e 5649 4449 4120 4750 5520 6e6f  g="NVIDIA GPU no
-000188f0: 7420 6176 6169 6c61 626c 6522 2c20 736f  t available", so
-00018900: 7572 6365 3d76 6572 7469 6361 6c5f 7669  urce=vertical_vi
-00018910: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
-00018920: 2e5f 5f6e 616d 655f 5f0a 2020 2020 2020  .__name__.      
-00018930: 2020 290a 2020 2020 7669 6465 6f5f 6d65    ).    video_me
-00018940: 7461 5f64 6174 6120 3d20 5b0a 2020 2020  ta_data = [.    
-00018950: 2020 2020 6765 745f 7669 6465 6f5f 6d65      get_video_me
-00018960: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
-00018970: 7468 3d76 6964 656f 5f70 6174 6829 2066  th=video_path) f
-00018980: 6f72 2076 6964 656f 5f70 6174 6820 696e  or video_path in
-00018990: 2076 6964 656f 5f70 6174 6873 0a20 2020   video_paths.   
-000189a0: 205d 0a20 2020 2074 696d 6572 203d 2053   ].    timer = S
-000189b0: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
-000189c0: 5472 7565 290a 2020 2020 6368 6563 6b5f  True).    check_
-000189d0: 7661 6c69 645f 6c73 7428 0a20 2020 2020  valid_lst(.     
-000189e0: 2020 2064 6174 613d 7669 6465 6f5f 7061     data=video_pa
-000189f0: 7468 732c 2073 6f75 7263 653d 7665 7274  ths, source=vert
-00018a00: 6963 616c 5f76 6964 656f 5f63 6f6e 6361  ical_video_conca
-00018a10: 7465 6e61 746f 722e 5f5f 6e61 6d65 5f5f  tenator.__name__
-00018a20: 2c20 6d69 6e5f 6c65 6e3d 320a 2020 2020  , min_len=2.    
-00018a30: 290a 2020 2020 6368 6563 6b5f 6966 5f64  ).    check_if_d
-00018a40: 6972 5f65 7869 7374 7328 0a20 2020 2020  ir_exists(.     
-00018a50: 2020 2069 6e5f 6469 723d 6f73 2e70 6174     in_dir=os.pat
-00018a60: 682e 6469 726e 616d 6528 7361 7665 5f70  h.dirname(save_p
-00018a70: 6174 6829 2c20 736f 7572 6365 3d76 6572  ath), source=ver
-00018a80: 7469 6361 6c5f 7669 6465 6f5f 636f 6e63  tical_video_conc
-00018a90: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
-00018aa0: 5f0a 2020 2020 290a 2020 2020 6966 2028  _.    ).    if (
-00018ab0: 2877 6964 7468 5f70 7820 6973 204e 6f6e  (width_px is Non
-00018ac0: 6529 2061 6e64 2028 7769 6474 685f 6964  e) and (width_id
-00018ad0: 7820 6973 204e 6f6e 6529 2920 6f72 2028  x is None)) or (
-00018ae0: 0a20 2020 2020 2020 2028 7769 6474 685f  .        (width_
-00018af0: 7078 2069 7320 6e6f 7420 4e6f 6e65 2920  px is not None) 
-00018b00: 616e 6420 2877 6964 7468 5f69 6478 2069  and (width_idx i
-00018b10: 7320 6e6f 7420 4e6f 6e65 290a 2020 2020  s not None).    
-00018b20: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00018b30: 2049 6e76 616c 6964 496e 7075 7445 7272   InvalidInputErr
-00018b40: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00018b50: 6d73 673d 2250 726f 7669 6465 2061 2077  msg="Provide a w
-00018b60: 6964 7468 5f70 7820 4f52 2077 6964 7468  idth_px OR width
-00018b70: 5f69 6478 222c 0a20 2020 2020 2020 2020  _idx",.         
-00018b80: 2020 2073 6f75 7263 653d 7665 7274 6963     source=vertic
-00018b90: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
-00018ba0: 6e61 746f 722e 5f5f 6e61 6d65 5f5f 2c0a  nator.__name__,.
-00018bb0: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
-00018bc0: 2077 6964 7468 5f69 6478 2069 7320 6e6f   width_idx is no
-00018bd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00018be0: 6368 6563 6b5f 696e 7428 0a20 2020 2020  check_int(.     
-00018bf0: 2020 2020 2020 206e 616d 653d 6622 7b76         name=f"{v
-00018c00: 6572 7469 6361 6c5f 7669 6465 6f5f 636f  ertical_video_co
-00018c10: 6e63 6174 656e 6174 6f72 2e5f 5f6e 616d  ncatenator.__nam
-00018c20: 655f 5f7d 2077 6964 7468 2069 6e64 6578  e__} width index
-00018c30: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
-00018c40: 616c 7565 3d77 6964 7468 5f69 6478 2c0a  alue=width_idx,.
-00018c50: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-00018c60: 7661 6c75 653d 302c 0a20 2020 2020 2020  value=0,.       
-00018c70: 2020 2020 206d 6178 5f76 616c 7565 3d6c       max_value=l
-00018c80: 656e 2876 6964 656f 5f70 6174 6873 2920  en(video_paths) 
-00018c90: 2d20 312c 0a20 2020 2020 2020 2029 0a20  - 1,.        ). 
-00018ca0: 2020 2020 2020 2077 6964 7468 203d 2069         width = i
-00018cb0: 6e74 2876 6964 656f 5f6d 6574 615f 6461  nt(video_meta_da
-00018cc0: 7461 5b77 6964 7468 5f69 6478 5d5b 2277  ta[width_idx]["w
-00018cd0: 6964 7468 225d 290a 2020 2020 656c 7365  idth"]).    else
-00018ce0: 3a0a 2020 2020 2020 2020 6368 6563 6b5f  :.        check_
-00018cf0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-00018d00: 206e 616d 653d 6622 7b76 6572 7469 6361   name=f"{vertica
-00018d10: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-00018d20: 6174 6f72 2e5f 5f6e 616d 655f 5f7d 2077  ator.__name__} w
-00018d30: 6964 7468 222c 0a20 2020 2020 2020 2020  idth",.         
-00018d40: 2020 2076 616c 7565 3d77 6964 7468 5f70     value=width_p
-00018d50: 782c 0a20 2020 2020 2020 2020 2020 206d  x,.            m
-00018d60: 696e 5f76 616c 7565 3d31 2c0a 2020 2020  in_value=1,.    
-00018d70: 2020 2020 290a 2020 2020 2020 2020 7769      ).        wi
-00018d80: 6474 6820 3d20 696e 7428 7769 6474 685f  dth = int(width_
-00018d90: 7078 290a 2020 2020 7669 6465 6f5f 7061  px).    video_pa
-00018da0: 7468 5f73 7472 203d 2022 2022 2e6a 6f69  th_str = " ".joi
-00018db0: 6e28 5b66 272d 6920 227b 7061 7468 7d22  n([f'-i "{path}"
-00018dc0: 2720 666f 7220 7061 7468 2069 6e20 7669  ' for path in vi
-00018dd0: 6465 6f5f 7061 7468 735d 290a 2020 2020  deo_paths]).    
-00018de0: 636f 6465 6320 3d20 2268 3236 345f 6e76  codec = "h264_nv
-00018df0: 656e 6322 2069 6620 6770 7520 656c 7365  enc" if gpu else
-00018e00: 2022 6c69 6276 7078 2d76 7039 220a 2020   "libvpx-vp9".  
-00018e10: 2020 6669 6c74 6572 5f63 6f6d 706c 6578    filter_complex
-00018e20: 203d 2022 3b22 2e6a 6f69 6e28 0a20 2020   = ";".join(.   
-00018e30: 2020 2020 205b 6622 5b7b 6964 787d 3a76       [f"[{idx}:v
-00018e40: 5d73 6361 6c65 3d7b 7769 6474 687d 3a2d  ]scale={width}:-
-00018e50: 315b 767b 6964 787d 5d22 2066 6f72 2069  1[v{idx}]" for i
-00018e60: 6478 2069 6e20 7261 6e67 6528 6c65 6e28  dx in range(len(
-00018e70: 7669 6465 6f5f 7061 7468 7329 295d 0a20  video_paths))]. 
-00018e80: 2020 2029 0a20 2020 2066 696c 7465 725f     ).    filter_
-00018e90: 636f 6d70 6c65 7820 2b3d 2066 223b 7b27  complex += f";{'
-00018ea0: 272e 6a6f 696e 285b 6627 5b76 7b69 6478  '.join([f'[v{idx
-00018eb0: 7d5d 2720 666f 7220 6964 7820 696e 2072  }]' for idx in r
-00018ec0: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
-00018ed0: 6174 6873 2929 5d29 7d22 0a20 2020 2066  aths))])}".    f
-00018ee0: 696c 7465 725f 636f 6d70 6c65 7820 2b3d  ilter_complex +=
-00018ef0: 2066 2276 7374 6163 6b3d 696e 7075 7473   f"vstack=inputs
-00018f00: 3d7b 6c65 6e28 7669 6465 6f5f 7061 7468  ={len(video_path
-00018f10: 7329 7d5b 765d 220a 2020 2020 6966 2076  s)}[v]".    if v
-00018f20: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00018f30: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00018f40: 2020 2066 2243 6f6e 6361 7465 6e61 7469     f"Concatenati
-00018f50: 6e67 207b 6c65 6e28 7669 6465 6f5f 7061  ng {len(video_pa
-00018f60: 7468 7329 7d20 7669 6465 6f73 2076 6572  ths)} videos ver
-00018f70: 7469 6361 6c6c 7920 7769 7468 2061 207b  tically with a {
-00018f80: 7769 6474 687d 2070 6978 656c 2077 6964  width} pixel wid
-00018f90: 7468 2e2e 2e22 0a20 2020 2020 2020 2029  th...".        )
-00018fa0: 0a20 2020 2063 6d64 203d 2066 2766 666d  .    cmd = f'ffm
-00018fb0: 7065 6720 7b76 6964 656f 5f70 6174 685f  peg {video_path_
-00018fc0: 7374 727d 202d 6669 6c74 6572 5f63 6f6d  str} -filter_com
-00018fd0: 706c 6578 2022 7b66 696c 7465 725f 636f  plex "{filter_co
-00018fe0: 6d70 6c65 787d 2220 2d6d 6170 2022 5b76  mplex}" -map "[v
-00018ff0: 5d22 202d 633a 7620 7b63 6f64 6563 7d20  ]" -c:v {codec} 
-00019000: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
-00019010: 2d73 7461 7473 2022 7b73 6176 655f 7061  -stats "{save_pa
-00019020: 7468 7d22 202d 7927 0a20 2020 2073 7562  th}" -y'.    sub
-00019030: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
-00019040: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
-00019050: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
-00019060: 5049 5045 290a 2020 2020 7469 6d65 722e  PIPE).    timer.
-00019070: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
-00019080: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-00019090: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
-000190a0: 2020 2020 2020 2020 6622 5665 7274 6963          f"Vertic
-000190b0: 616c 2063 6f6e 6361 7465 6e61 7469 6f6e  al concatenation
-000190c0: 2063 6f6d 706c 6574 652e 2053 6176 6564   complete. Saved
-000190d0: 2061 7420 7b73 6176 655f 7061 7468 7d20   at {save_path} 
-000190e0: 2845 6c61 7073 6564 2074 696d 653a 207b  (Elapsed time: {
-000190f0: 7469 6d65 722e 656c 6170 7365 645f 7469  timer.elapsed_ti
-00019100: 6d65 5f73 7472 7d73 2e29 220a 2020 2020  me_str}s.)".    
-00019110: 2020 2020 290a 0a0a 6465 6620 6d6f 7361      )...def mosa
-00019120: 6963 5f63 6f6e 6361 7465 6e61 746f 7228  ic_concatenator(
-00019130: 0a20 2020 2076 6964 656f 5f70 6174 6873  .    video_paths
-00019140: 3a20 4c69 7374 5b55 6e69 6f6e 5b73 7472  : List[Union[str
-00019150: 2c20 6f73 2e50 6174 684c 696b 655d 5d2c  , os.PathLike]],
-00019160: 0a20 2020 2073 6176 655f 7061 7468 3a20  .    save_path: 
-00019170: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-00019180: 7468 4c69 6b65 5d2c 0a20 2020 2077 6964  thLike],.    wid
-00019190: 7468 5f69 6478 3a20 4f70 7469 6f6e 616c  th_idx: Optional
-000191a0: 5b55 6e69 6f6e 5b69 6e74 2c20 7374 725d  [Union[int, str]
-000191b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7769  ] = None,.    wi
-000191c0: 6474 685f 7078 3a20 4f70 7469 6f6e 616c  dth_px: Optional
-000191d0: 5b55 6e69 6f6e 5b69 6e74 2c20 7374 725d  [Union[int, str]
-000191e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6865  ] = None,.    he
-000191f0: 6967 6874 5f69 6478 3a20 4f70 7469 6f6e  ight_idx: Option
-00019200: 616c 5b55 6e69 6f6e 5b69 6e74 2c20 7374  al[Union[int, st
-00019210: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-00019220: 6865 6967 6874 5f70 783a 204f 7074 696f  height_px: Optio
-00019230: 6e61 6c5b 556e 696f 6e5b 696e 742c 2073  nal[Union[int, s
-00019240: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-00019250: 2067 7075 3a20 4f70 7469 6f6e 616c 5b62   gpu: Optional[b
-00019260: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-00019270: 2020 7665 7262 6f73 653a 204f 7074 696f    verbose: Optio
-00019280: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-00019290: 2c0a 2020 2020 756e 6576 656e 5f66 696c  ,.    uneven_fil
-000192a0: 6c5f 636f 6c6f 723a 204f 7074 696f 6e61  l_color: Optiona
-000192b0: 6c5b 7374 725d 203d 2022 626c 6163 6b22  l[str] = "black"
-000192c0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-000192d0: 2022 2222 0a20 2020 2043 6f6e 6361 7465   """.    Concate
-000192e0: 6e61 7465 7320 6d75 6c74 6970 6c65 2076  nates multiple v
-000192f0: 6964 656f 7320 696e 746f 2061 206d 6f73  ideos into a mos
-00019300: 6169 6320 6c61 796f 7574 2e0a 0a20 2020  aic layout...   
-00019310: 202e 2e20 696d 6167 653a 3a20 5f73 7461   .. image:: _sta
-00019320: 7469 632f 696d 672f 6d6f 7361 6963 5f63  tic/img/mosaic_c
-00019330: 6f6e 6361 7465 6e61 746f 722e 706e 670a  oncatenator.png.
-00019340: 2020 2020 2020 203a 7769 6474 683a 2036         :width: 6
-00019350: 3030 0a20 2020 2020 2020 3a61 6c69 676e  00.       :align
-00019360: 3a20 6365 6e74 6572 0a0a 2020 2020 2e2e  : center..    ..
-00019370: 206e 6f74 653a 3a0a 2020 2020 2020 2069   note::.       i
-00019380: 6620 616e 2075 6e65 7665 6e20 6e75 6d62  f an uneven numb
-00019390: 6572 206f 6620 7669 6465 6f73 2c20 7468  er of videos, th
-000193a0: 6520 6c61 7374 2069 6e64 6578 2077 696c  e last index wil
-000193b0: 6c20 6265 2066 696c 6c65 6420 6279 2060  l be filled by `
-000193c0: 6075 6e65 7665 6e5f 6669 6c6c 5f63 6f6c  `uneven_fill_col
-000193d0: 6f72 6060 2e0a 0a20 2020 203a 7061 7261  or``...    :para
-000193e0: 6d20 4c69 7374 5b55 6e69 6f6e 5b73 7472  m List[Union[str
-000193f0: 2c20 6f73 2e50 6174 684c 696b 655d 5d20  , os.PathLike]] 
-00019400: 7669 6465 6f5f 7061 7468 733a 204c 6973  video_paths: Lis
-00019410: 7420 6f66 2069 6e70 7574 2076 6964 656f  t of input video
-00019420: 2066 696c 6520 7061 7468 732e 0a20 2020   file paths..   
-00019430: 203a 7061 7261 6d20 556e 696f 6e5b 7374   :param Union[st
-00019440: 722c 206f 732e 5061 7468 4c69 6b65 5d20  r, os.PathLike] 
-00019450: 7361 7665 5f70 6174 683a 2046 696c 6520  save_path: File 
-00019460: 7061 7468 2074 6f20 7361 7665 2074 6865  path to save the
-00019470: 2063 6f6e 6361 7465 6e61 7465 6420 7669   concatenated vi
-00019480: 6465 6f2e 0a20 2020 203a 7061 7261 6d20  deo..    :param 
-00019490: 4f70 7469 6f6e 616c 5b69 6e74 5d20 7769  Optional[int] wi
-000194a0: 6474 685f 7078 3a20 5769 6474 6820 6f66  dth_px: Width of
-000194b0: 2074 6865 206f 7574 7075 7420 7669 6465   the output vide
-000194c0: 6f20 696e 2070 6978 656c 732e 0a20 2020  o in pixels..   
-000194d0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-000194e0: 5b69 6e74 5d20 7769 6474 685f 6964 783a  [int] width_idx:
-000194f0: 2049 6e64 6578 206f 6620 7468 6520 7669   Index of the vi
-00019500: 6465 6f20 746f 2075 7365 2066 6f72 2064  deo to use for d
-00019510: 6574 6572 6d69 6e69 6e67 2077 6964 7468  etermining width
-00019520: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00019530: 696f 6e61 6c5b 696e 745d 2068 6569 6768  ional[int] heigh
-00019540: 745f 7078 3a20 4865 6967 6874 206f 6620  t_px: Height of 
-00019550: 7468 6520 6f75 7470 7574 2076 6964 656f  the output video
-00019560: 2070 616e 656c 7320 696e 2070 6978 656c   panels in pixel
-00019570: 732e 0a20 2020 203a 7061 7261 6d20 4f70  s..    :param Op
-00019580: 7469 6f6e 616c 5b69 6e74 5d20 6865 6967  tional[int] heig
-00019590: 6874 5f69 6478 3a20 4865 6967 6874 206f  ht_idx: Height o
-000195a0: 6620 7468 6520 7669 6465 6f20 746f 2075  f the video to u
-000195b0: 7365 2066 6f72 2064 6574 6572 6d69 6e69  se for determini
-000195c0: 6e67 2077 6964 7468 2e0a 2020 2020 3a70  ng width..    :p
-000195d0: 6172 616d 204f 7074 696f 6e61 6c5b 626f  aram Optional[bo
-000195e0: 6f6c 5d20 6770 753a 2057 6865 7468 6572  ol] gpu: Whether
-000195f0: 2074 6f20 7573 6520 4750 552d 6163 6365   to use GPU-acce
-00019600: 6c65 7261 7465 6420 636f 6465 6320 2864  lerated codec (d
-00019610: 6566 6175 6c74 3a20 4661 6c73 6529 2e0a  efault: False)..
-00019620: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-00019630: 6e61 6c5b 626f 6f6c 5d20 7665 7262 6f73  nal[bool] verbos
-00019640: 653a 2057 6865 7468 6572 2074 6f20 7072  e: Whether to pr
-00019650: 696e 7420 7072 6f67 7265 7373 206d 6573  int progress mes
-00019660: 7361 6765 7320 2864 6566 6175 6c74 3a20  sages (default: 
-00019670: 5472 7565 292e 0a0a 2020 2020 3a65 7861  True)...    :exa
-00019680: 6d70 6c65 3a0a 2020 2020 3e3e 3e20 7669  mple:.    >>> vi
-00019690: 6465 6f5f 7061 7468 7320 3d20 5b27 2f55  deo_paths = ['/U
-000196a0: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-000196b0: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-000196c0: 6f75 626c 6573 686f 6f74 696e 672f 5241  oubleshooting/RA
-000196d0: 545f 4e4f 522f 7072 6f6a 6563 745f 666f  T_NOR/project_fo
-000196e0: 6c64 6572 2f76 6964 656f 732f 7465 7374  lder/videos/test
-000196f0: 2f30 3831 3032 3032 315f 444f 545f 5261  /08102021_DOT_Ra
-00019700: 7437 5f38 2832 292e 6d70 3427 2c20 272f  t7_8(2).mp4', '/
-00019710: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-00019720: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-00019730: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
-00019740: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
-00019750: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
-00019760: 742f 3038 3130 3230 3231 5f44 4f54 5f52  t/08102021_DOT_R
-00019770: 6174 3131 5f31 322e 6d70 3427 2c20 272f  at11_12.mp4', '/
-00019780: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-00019790: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-000197a0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
-000197b0: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
-000197c0: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
-000197d0: 742f 6e65 772f 3230 3232 2d30 362d 3231  t/new/2022-06-21
-000197e0: 5f4e 4f42 5f49 4f54 5f32 332e 6d70 3427  _NOB_IOT_23.mp4'
-000197f0: 5d0a 2020 2020 3e3e 3e20 7361 7665 5f70  ].    >>> save_p
-00019800: 6174 6820 3d20 272f 5573 6572 732f 7369  ath = '/Users/si
-00019810: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-00019820: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-00019830: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
-00019840: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-00019850: 6465 6f73 2f74 6573 742f 6e65 772f 626c  deos/test/new/bl
-00019860: 616e 6b5f 7465 7374 2e6d 7034 270a 2020  ank_test.mp4'.  
-00019870: 2020 3e3e 3e20 6d6f 7361 6963 5f63 6f6e    >>> mosaic_con
-00019880: 6361 7465 6e61 746f 7228 7669 6465 6f5f  catenator(video_
-00019890: 7061 7468 733d 7669 6465 6f5f 7061 7468  paths=video_path
-000198a0: 732c 2073 6176 655f 7061 7468 3d73 6176  s, save_path=sav
-000198b0: 655f 7061 7468 2c20 7769 6474 685f 6964  e_path, width_id
-000198c0: 783d 312c 2068 6569 6768 745f 6964 783d  x=1, height_idx=
-000198d0: 312c 2067 7075 3d46 616c 7365 290a 2020  1, gpu=False).  
-000198e0: 2020 2222 220a 0a20 2020 2063 6865 636b    """..    check
-000198f0: 5f66 666d 7065 675f 6176 6169 6c61 626c  _ffmpeg_availabl
-00019900: 6528 290a 2020 2020 6966 2067 7075 2061  e().    if gpu a
-00019910: 6e64 206e 6f74 2063 6865 636b 5f6e 7669  nd not check_nvi
-00019920: 6465 615f 6770 755f 6176 6169 6c61 626c  dea_gpu_availabl
-00019930: 6528 293a 0a20 2020 2020 2020 2072 6169  e():.        rai
-00019940: 7365 2046 464d 5045 4743 6f64 6563 4750  se FFMPEGCodecGP
-00019950: 5545 7272 6f72 280a 2020 2020 2020 2020  UError(.        
-00019960: 2020 2020 6d73 673d 224e 5649 4449 4120      msg="NVIDIA 
-00019970: 4750 5520 6e6f 7420 6176 6169 6c61 626c  GPU not availabl
-00019980: 6522 2c20 736f 7572 6365 3d6d 6f73 6169  e", source=mosai
-00019990: 635f 636f 6e63 6174 656e 6174 6f72 2e5f  c_concatenator._
-000199a0: 5f6e 616d 655f 5f0a 2020 2020 2020 2020  _name__.        
-000199b0: 290a 2020 2020 7469 6d65 7220 3d20 5369  ).    timer = Si
-000199c0: 6d62 6154 696d 6572 2873 7461 7274 3d54  mbaTimer(start=T
-000199d0: 7275 6529 0a20 2020 2064 7420 3d20 6461  rue).    dt = da
-000199e0: 7465 7469 6d65 2e6e 6f77 2829 2e73 7472  tetime.now().str
-000199f0: 6674 696d 6528 2225 5925 6d25 6425 4825  ftime("%Y%m%d%H%
-00019a00: 4d25 5322 290a 2020 2020 6368 6563 6b5f  M%S").    check_
-00019a10: 7661 6c69 645f 6c73 7428 0a20 2020 2020  valid_lst(.     
-00019a20: 2020 2064 6174 613d 7669 6465 6f5f 7061     data=video_pa
-00019a30: 7468 732c 0a20 2020 2020 2020 2073 6f75  ths,.        sou
-00019a40: 7263 653d 6622 7b6d 6f73 6169 635f 636f  rce=f"{mosaic_co
-00019a50: 6e63 6174 656e 6174 6f72 2e5f 5f6e 616d  ncatenator.__nam
-00019a60: 655f 5f7d 2076 6964 656f 5f70 6174 6873  e__} video_paths
-00019a70: 222c 0a20 2020 2020 2020 206d 696e 5f6c  ",.        min_l
-00019a80: 656e 3d33 2c0a 2020 2020 290a 2020 2020  en=3,.    ).    
-00019a90: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
-00019aa0: 3d20 5b0a 2020 2020 2020 2020 6765 745f  = [.        get_
-00019ab0: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
-00019ac0: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
-00019ad0: 5f70 6174 6829 2066 6f72 2076 6964 656f  _path) for video
-00019ae0: 5f70 6174 6820 696e 2076 6964 656f 5f70  _path in video_p
-00019af0: 6174 6873 0a20 2020 205d 0a20 2020 206d  aths.    ].    m
-00019b00: 6178 5f76 6964 656f 5f6c 656e 6774 6820  ax_video_length 
-00019b10: 3d20 6d61 7828 5b78 5b22 7669 6465 6f5f  = max([x["video_
-00019b20: 6c65 6e67 7468 5f73 225d 2066 6f72 2078  length_s"] for x
-00019b30: 2069 6e20 7669 6465 6f5f 6d65 7461 5f64   in video_meta_d
-00019b40: 6174 615d 290a 2020 2020 6966 2028 2877  ata]).    if ((w
-00019b50: 6964 7468 5f70 7820 6973 204e 6f6e 6529  idth_px is None)
-00019b60: 2061 6e64 2028 7769 6474 685f 6964 7820   and (width_idx 
-00019b70: 6973 204e 6f6e 6529 2920 6f72 2028 0a20  is None)) or (. 
-00019b80: 2020 2020 2020 2028 7769 6474 685f 7078         (width_px
-00019b90: 2069 7320 6e6f 7420 4e6f 6e65 2920 616e   is not None) an
-00019ba0: 6420 2877 6964 7468 5f69 6478 2069 7320  d (width_idx is 
-00019bb0: 6e6f 7420 4e6f 6e65 290a 2020 2020 293a  not None).    ):
-00019bc0: 0a20 2020 2020 2020 2072 6169 7365 2049  .        raise I
-00019bd0: 6e76 616c 6964 496e 7075 7445 7272 6f72  nvalidInputError
-00019be0: 280a 2020 2020 2020 2020 2020 2020 6d73  (.            ms
-00019bf0: 673d 2250 726f 7669 6465 2061 2077 6964  g="Provide a wid
-00019c00: 7468 5f70 7820 4f52 2077 6964 7468 5f69  th_px OR width_i
-00019c10: 6478 222c 2073 6f75 7263 653d 6d6f 7361  dx", source=mosa
-00019c20: 6963 5f63 6f6e 6361 7465 6e61 746f 722e  ic_concatenator.
-00019c30: 5f5f 6e61 6d65 5f5f 0a20 2020 2020 2020  __name__.       
-00019c40: 2029 0a20 2020 2069 6620 2828 6865 6967   ).    if ((heig
-00019c50: 6874 5f70 7820 6973 204e 6f6e 6529 2061  ht_px is None) a
-00019c60: 6e64 2028 6865 6967 6874 5f69 6478 2069  nd (height_idx i
-00019c70: 7320 4e6f 6e65 2929 206f 7220 280a 2020  s None)) or (.  
-00019c80: 2020 2020 2020 2868 6569 6768 745f 7078        (height_px
-00019c90: 2069 7320 6e6f 7420 4e6f 6e65 2920 616e   is not None) an
-00019ca0: 6420 2868 6569 6768 745f 6964 7820 6973  d (height_idx is
-00019cb0: 206e 6f74 204e 6f6e 6529 0a20 2020 2029   not None).    )
-00019cc0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00019cd0: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
-00019ce0: 7228 0a20 2020 2020 2020 2020 2020 206d  r(.            m
-00019cf0: 7367 3d22 5072 6f76 6964 6520 6120 6865  sg="Provide a he
-00019d00: 6967 6874 5f70 7820 4f52 2068 6569 6768  ight_px OR heigh
-00019d10: 745f 6964 7822 2c20 736f 7572 6365 3d6d  t_idx", source=m
-00019d20: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
-00019d30: 6f72 2e5f 5f6e 616d 655f 5f0a 2020 2020  or.__name__.    
-00019d40: 2020 2020 290a 2020 2020 6966 2077 6964      ).    if wid
-00019d50: 7468 5f69 6478 2069 7320 6e6f 7420 4e6f  th_idx is not No
-00019d60: 6e65 3a0a 2020 2020 2020 2020 6368 6563  ne:.        chec
-00019d70: 6b5f 696e 7428 0a20 2020 2020 2020 2020  k_int(.         
-00019d80: 2020 206e 616d 653d 6622 7b76 6572 7469     name=f"{verti
-00019d90: 6361 6c5f 7669 6465 6f5f 636f 6e63 6174  cal_video_concat
-00019da0: 656e 6174 6f72 2e5f 5f6e 616d 655f 5f7d  enator.__name__}
-00019db0: 2077 6964 7468 2069 6e64 6578 222c 0a20   width index",. 
-00019dc0: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00019dd0: 3d77 6964 7468 5f69 6478 2c0a 2020 2020  =width_idx,.    
-00019de0: 2020 2020 2020 2020 6d69 6e5f 7661 6c75          min_valu
-00019df0: 653d 312c 0a20 2020 2020 2020 2020 2020  e=1,.           
-00019e00: 206d 6178 5f76 616c 7565 3d6c 656e 2876   max_value=len(v
-00019e10: 6964 656f 5f70 6174 6873 2920 2d20 312c  ideo_paths) - 1,
-00019e20: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00019e30: 2020 2077 6964 7468 203d 2069 6e74 2876     width = int(v
-00019e40: 6964 656f 5f6d 6574 615f 6461 7461 5b77  ideo_meta_data[w
-00019e50: 6964 7468 5f69 6478 5d5b 2277 6964 7468  idth_idx]["width
-00019e60: 225d 290a 2020 2020 656c 7365 3a0a 2020  "]).    else:.  
-00019e70: 2020 2020 2020 7769 6474 6820 3d20 7769        width = wi
-00019e80: 6474 685f 7078 0a20 2020 2069 6620 6865  dth_px.    if he
-00019e90: 6967 6874 5f69 6478 2069 7320 6e6f 7420  ight_idx is not 
-00019ea0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
-00019eb0: 6563 6b5f 696e 7428 0a20 2020 2020 2020  eck_int(.       
-00019ec0: 2020 2020 206e 616d 653d 6622 7b76 6572       name=f"{ver
-00019ed0: 7469 6361 6c5f 7669 6465 6f5f 636f 6e63  tical_video_conc
-00019ee0: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
-00019ef0: 5f7d 2068 6569 6768 7420 696e 6465 7822  _} height index"
-00019f00: 2c0a 2020 2020 2020 2020 2020 2020 7661  ,.            va
-00019f10: 6c75 653d 7769 6474 685f 6964 782c 0a20  lue=width_idx,. 
-00019f20: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
-00019f30: 616c 7565 3d31 2c0a 2020 2020 2020 2020  alue=1,.        
-00019f40: 2020 2020 6d61 785f 7661 6c75 653d 6c65      max_value=le
-00019f50: 6e28 7669 6465 6f5f 7061 7468 7329 202d  n(video_paths) -
-00019f60: 2031 2c0a 2020 2020 2020 2020 290a 2020   1,.        ).  
-00019f70: 2020 2020 2020 6865 6967 6874 203d 2069        height = i
-00019f80: 6e74 2876 6964 656f 5f6d 6574 615f 6461  nt(video_meta_da
-00019f90: 7461 5b77 6964 7468 5f69 6478 5d5b 2268  ta[width_idx]["h
-00019fa0: 6569 6768 7422 5d29 0a20 2020 2065 6c73  eight"]).    els
-00019fb0: 653a 0a20 2020 2020 2020 2068 6569 6768  e:.        heigh
-00019fc0: 7420 3d20 6865 6967 6874 5f70 780a 2020  t = height_px.  
-00019fd0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00019fe0: 2020 2020 2020 7072 696e 7428 6622 4372        print(f"Cr
-00019ff0: 6561 7469 6e67 206d 6f73 6169 6320 7669  eating mosaic vi
-0001a000: 6465 6f20 2e2e 2e22 290a 2020 2020 7465  deo ...").    te
-0001a010: 6d70 5f64 6972 203d 206f 732e 7061 7468  mp_dir = os.path
-0001a020: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
-0001a030: 726e 616d 6528 7669 6465 6f5f 7061 7468  rname(video_path
-0001a040: 735b 305d 292c 2066 2274 656d 705f 7b64  s[0]), f"temp_{d
-0001a050: 747d 2229 0a20 2020 206f 732e 6d61 6b65  t}").    os.make
-0001a060: 6469 7273 2874 656d 705f 6469 7229 0a20  dirs(temp_dir). 
-0001a070: 2020 2069 6620 6e6f 7420 286c 656e 2876     if not (len(v
-0001a080: 6964 656f 5f70 6174 6873 2920 2520 3229  ideo_paths) % 2)
-0001a090: 203d 3d20 303a 0a20 2020 2020 2020 2062   == 0:.        b
-0001a0a0: 6c61 6e6b 5f70 6174 6820 3d20 6f73 2e70  lank_path = os.p
-0001a0b0: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
-0001a0c0: 722c 2066 227b 6474 7d2e 6d70 3422 290a  r, f"{dt}.mp4").
-0001a0d0: 2020 2020 2020 2020 6372 6561 7465 5f62          create_b
-0001a0e0: 6c61 6e6b 5f76 6964 656f 280a 2020 2020  lank_video(.    
-0001a0f0: 2020 2020 2020 2020 7061 7468 3d62 6c61          path=bla
-0001a100: 6e6b 5f70 6174 682c 0a20 2020 2020 2020  nk_path,.       
-0001a110: 2020 2020 206c 656e 6774 683d 6d61 785f       length=max_
-0001a120: 7669 6465 6f5f 6c65 6e67 7468 2c0a 2020  video_length,.  
-0001a130: 2020 2020 2020 2020 2020 7769 6474 683d            width=
-0001a140: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
-0001a150: 2020 2068 6569 6768 743d 6865 6967 6874     height=height
-0001a160: 2c0a 2020 2020 2020 2020 2020 2020 6770  ,.            gp
-0001a170: 753d 6770 752c 0a20 2020 2020 2020 2020  u=gpu,.         
-0001a180: 2020 2076 6572 626f 7365 3d76 6572 626f     verbose=verbo
-0001a190: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0001a1a0: 636f 6c6f 723d 756e 6576 656e 5f66 696c  color=uneven_fil
-0001a1b0: 6c5f 636f 6c6f 722c 0a20 2020 2020 2020  l_color,.       
-0001a1c0: 2029 0a20 2020 2020 2020 2076 6964 656f   ).        video
-0001a1d0: 5f70 6174 6873 2e61 7070 656e 6428 626c  _paths.append(bl
-0001a1e0: 616e 6b5f 7061 7468 290a 2020 2020 7570  ank_path).    up
-0001a1f0: 7065 725f 7669 6465 6f73 2c20 6c6f 7765  per_videos, lowe
-0001a200: 725f 7669 6465 6f73 203d 2028 0a20 2020  r_videos = (.   
-0001a210: 2020 2020 2076 6964 656f 5f70 6174 6873       video_paths
-0001a220: 5b3a 206c 656e 2876 6964 656f 5f70 6174  [: len(video_pat
-0001a230: 6873 2920 2f2f 2032 5d2c 0a20 2020 2020  hs) // 2],.     
-0001a240: 2020 2076 6964 656f 5f70 6174 6873 5b6c     video_paths[l
-0001a250: 656e 2876 6964 656f 5f70 6174 6873 2920  en(video_paths) 
-0001a260: 2f2f 2032 203a 5d2c 0a20 2020 2029 0a20  // 2 :],.    ). 
-0001a270: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
-0001a280: 2020 2020 2020 2070 7269 6e74 2822 4372         print("Cr
-0001a290: 6561 7469 6e67 2075 7070 6572 206d 6f73  eating upper mos
-0001a2a0: 6169 632e 2e2e 2028 5374 6570 2031 2f33  aic... (Step 1/3
-0001a2b0: 2922 290a 2020 2020 6966 206c 656e 2875  )").    if len(u
-0001a2c0: 7070 6572 5f76 6964 656f 7329 203e 2031  pper_videos) > 1
-0001a2d0: 3a0a 2020 2020 2020 2020 7570 7065 725f  :.        upper_
-0001a2e0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-0001a2f0: 6f69 6e28 7465 6d70 5f64 6972 2c20 2275  oin(temp_dir, "u
-0001a300: 7070 6572 2e6d 7034 2229 0a20 2020 2020  pper.mp4").     
-0001a310: 2020 2068 6f72 697a 6f6e 7461 6c5f 7669     horizontal_vi
-0001a320: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
-0001a330: 280a 2020 2020 2020 2020 2020 2020 7669  (.            vi
-0001a340: 6465 6f5f 7061 7468 733d 7570 7065 725f  deo_paths=upper_
-0001a350: 7669 6465 6f73 2c0a 2020 2020 2020 2020  videos,.        
-0001a360: 2020 2020 7361 7665 5f70 6174 683d 7570      save_path=up
-0001a370: 7065 725f 7061 7468 2c0a 2020 2020 2020  per_path,.      
-0001a380: 2020 2020 2020 6770 753d 6770 752c 0a20        gpu=gpu,. 
-0001a390: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-0001a3a0: 745f 7078 3d68 6569 6768 742c 0a20 2020  t_px=height,.   
-0001a3b0: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
-0001a3c0: 3d76 6572 626f 7365 2c0a 2020 2020 2020  =verbose,.      
-0001a3d0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-0001a3e0: 2020 2020 2020 7570 7065 725f 7061 7468        upper_path
-0001a3f0: 203d 2075 7070 6572 5f76 6964 656f 735b   = upper_videos[
-0001a400: 305d 0a20 2020 2069 6620 7665 7262 6f73  0].    if verbos
-0001a410: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-0001a420: 2822 4372 6561 7469 6e67 206c 6f77 6572  ("Creating lower
-0001a430: 206d 6f73 6169 632e 2e2e 2028 5374 6570   mosaic... (Step
-0001a440: 2032 2f33 2922 290a 2020 2020 6966 206c   2/3)").    if l
-0001a450: 656e 286c 6f77 6572 5f76 6964 656f 7329  en(lower_videos)
-0001a460: 203e 2031 3a0a 2020 2020 2020 2020 6c6f   > 1:.        lo
-0001a470: 7765 725f 7061 7468 203d 206f 732e 7061  wer_path = os.pa
-0001a480: 7468 2e6a 6f69 6e28 7465 6d70 5f64 6972  th.join(temp_dir
-0001a490: 2c20 226c 6f77 6572 2e6d 7034 2229 0a20  , "lower.mp4"). 
-0001a4a0: 2020 2020 2020 2068 6f72 697a 6f6e 7461         horizonta
-0001a4b0: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-0001a4c0: 6174 6f72 280a 2020 2020 2020 2020 2020  ator(.          
-0001a4d0: 2020 7669 6465 6f5f 7061 7468 733d 6c6f    video_paths=lo
-0001a4e0: 7765 725f 7669 6465 6f73 2c0a 2020 2020  wer_videos,.    
-0001a4f0: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
-0001a500: 683d 6c6f 7765 725f 7061 7468 2c0a 2020  h=lower_path,.  
-0001a510: 2020 2020 2020 2020 2020 6770 753d 6770            gpu=gp
-0001a520: 752c 0a20 2020 2020 2020 2020 2020 2068  u,.            h
-0001a530: 6569 6768 745f 7078 3d68 6569 6768 742c  eight_px=height,
-0001a540: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-0001a550: 626f 7365 3d76 6572 626f 7365 2c0a 2020  bose=verbose,.  
-0001a560: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
-0001a570: 3a0a 2020 2020 2020 2020 6c6f 7765 725f  :.        lower_
-0001a580: 7061 7468 203d 206c 6f77 6572 5f76 6964  path = lower_vid
-0001a590: 656f 735b 305d 0a20 2020 2070 616e 656c  eos[0].    panel
-0001a5a0: 735f 6d65 7461 203d 205b 0a20 2020 2020  s_meta = [.     
-0001a5b0: 2020 2067 6574 5f76 6964 656f 5f6d 6574     get_video_met
-0001a5c0: 615f 6461 7461 2876 6964 656f 5f70 6174  a_data(video_pat
-0001a5d0: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-0001a5e0: 2020 2020 2020 666f 7220 7669 6465 6f5f        for video_
-0001a5f0: 7061 7468 2069 6e20 5b6c 6f77 6572 5f70  path in [lower_p
-0001a600: 6174 682c 2075 7070 6572 5f70 6174 685d  ath, upper_path]
-0001a610: 0a20 2020 205d 0a20 2020 2069 6620 7665  .    ].    if ve
-0001a620: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-0001a630: 7269 6e74 2822 4a6f 696e 696e 6720 7570  rint("Joining up
-0001a640: 7065 7220 616e 6420 6c6f 7765 7220 6d6f  per and lower mo
-0001a650: 7361 6963 2e2e 2e20 2853 7465 7020 322f  saic... (Step 2/
-0001a660: 3329 2229 0a20 2020 2076 6572 7469 6361  3)").    vertica
-0001a670: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-0001a680: 6174 6f72 280a 2020 2020 2020 2020 7669  ator(.        vi
-0001a690: 6465 6f5f 7061 7468 733d 5b75 7070 6572  deo_paths=[upper
-0001a6a0: 5f70 6174 682c 206c 6f77 6572 5f70 6174  _path, lower_pat
-0001a6b0: 685d 2c0a 2020 2020 2020 2020 7361 7665  h],.        save
-0001a6c0: 5f70 6174 683d 7361 7665 5f70 6174 682c  _path=save_path,
-0001a6d0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-0001a6e0: 3d76 6572 626f 7365 2c0a 2020 2020 2020  =verbose,.      
-0001a6f0: 2020 6770 753d 6770 752c 0a20 2020 2020    gpu=gpu,.     
-0001a700: 2020 2077 6964 7468 5f70 783d 6d61 7828     width_px=max(
-0001a710: 5b78 5b22 7769 6474 6822 5d20 666f 7220  [x["width"] for 
-0001a720: 7820 696e 2070 616e 656c 735f 6d65 7461  x in panels_meta
-0001a730: 5d29 2c0a 2020 2020 290a 2020 2020 7469  ]),.    ).    ti
-0001a740: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
-0001a750: 0a20 2020 2073 6875 7469 6c2e 726d 7472  .    shutil.rmtr
-0001a760: 6565 2874 656d 705f 6469 7229 0a20 2020  ee(temp_dir).   
-0001a770: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-0001a780: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
-0001a790: 2020 2020 2020 2020 6622 4d6f 7361 6963          f"Mosaic
-0001a7a0: 2063 6f6e 6361 7465 6e61 7469 6f6e 2063   concatenation c
-0001a7b0: 6f6d 706c 6574 652e 2053 6176 6564 2061  omplete. Saved a
-0001a7c0: 7420 7b73 6176 655f 7061 7468 7d20 2845  t {save_path} (E
-0001a7d0: 6c61 7073 6564 2074 696d 653a 207b 7469  lapsed time: {ti
-0001a7e0: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
-0001a7f0: 5f73 7472 7d73 2e29 220a 2020 2020 2020  _str}s.)".      
-0001a800: 2020 290a 0a0a 6465 6620 6d69 7865 645f    )...def mixed_
-0001a810: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
-0001a820: 746f 7228 0a20 2020 2076 6964 656f 5f70  tor(.    video_p
-0001a830: 6174 6873 3a20 4c69 7374 5b55 6e69 6f6e  aths: List[Union
-0001a840: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-0001a850: 655d 5d2c 0a20 2020 2073 6176 655f 7061  e]],.    save_pa
-0001a860: 7468 3a20 556e 696f 6e5b 7374 722c 206f  th: Union[str, o
-0001a870: 732e 5061 7468 4c69 6b65 5d2c 0a20 2020  s.PathLike],.   
-0001a880: 2067 7075 3a20 4f70 7469 6f6e 616c 5b62   gpu: Optional[b
-0001a890: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-0001a8a0: 2020 7665 7262 6f73 653a 204f 7074 696f    verbose: Optio
-0001a8b0: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-0001a8c0: 2c0a 2020 2020 756e 6576 656e 5f66 696c  ,.    uneven_fil
-0001a8d0: 6c5f 636f 6c6f 723a 204f 7074 696f 6e61  l_color: Optiona
-0001a8e0: 6c5b 7374 725d 203d 2022 626c 6163 6b22  l[str] = "black"
-0001a8f0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-0001a900: 2022 2222 0a20 2020 2043 7265 6174 6520   """.    Create 
-0001a910: 6120 6d69 7865 6420 6d6f 7361 6963 2076  a mixed mosaic v
-0001a920: 6964 656f 2062 7920 636f 6e63 6174 656e  ideo by concaten
-0001a930: 6174 696e 6720 6d75 6c74 6970 6c65 2069  ating multiple i
-0001a940: 6e70 7574 2076 6964 656f 7320 696e 2061  nput videos in a
-0001a950: 206d 6f73 6169 6320 6c61 796f 7574 206f   mosaic layout o
-0001a960: 6620 7661 7269 6f75 7320 7369 7a65 732e  f various sizes.
-0001a970: 0a0a 2020 2020 2e2e 2069 6d61 6765 3a3a  ..    .. image::
-0001a980: 205f 7374 6174 6963 2f69 6d67 2f6d 6978   _static/img/mix
-0001a990: 6564 5f6d 6f73 6169 635f 636f 6e63 6174  ed_mosaic_concat
-0001a9a0: 656e 6174 6f72 2e70 6e67 0a20 2020 2020  enator.png.     
-0001a9b0: 2020 3a77 6964 7468 3a20 3630 300a 2020    :width: 600.  
-0001a9c0: 2020 2020 203a 616c 6967 6e3a 2063 656e       :align: cen
-0001a9d0: 7465 720a 0a20 2020 202e 2e20 6e6f 7465  ter..    .. note
-0001a9e0: 3a3a 0a20 2020 2020 2020 5468 6520 7265  ::.       The re
-0001a9f0: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
-0001aa00: 6f75 7470 7574 2076 6964 656f 2069 7320  output video is 
-0001aa10: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
-0001aa20: 6520 7265 736f 6c75 7469 6f6e 206f 6620  e resolution of 
-0001aa30: 7468 6520 7669 6465 6f20 7061 7468 2061  the video path a
-0001aa40: 7420 7468 6520 6669 7273 7420 696e 6465  t the first inde
-0001aa50: 782e 0a0a 2020 2020 2020 2049 6620 616e  x...       If an
-0001aa60: 2075 6e65 7665 6e20 6e75 6d62 6572 206f   uneven number o
-0001aa70: 6620 7269 6768 742d 7061 6e65 6c20 7669  f right-panel vi
-0001aa80: 6465 6f73 2028 2069 6620 6e6f 7420 286c  deos ( if not (l
-0001aa90: 656e 2876 6964 656f 5f70 6174 6873 292d  en(video_paths)-
-0001aaa0: 3129 2025 2032 2920 3d3d 2030 292c 2074  1) % 2) == 0), t
-0001aab0: 6865 6e20 7468 6520 6c61 7374 2069 6e64  hen the last ind
-0001aac0: 6578 2077 696c 6c20 6265 2066 696c 6c65  ex will be fille
-0001aad0: 6420 6279 2060 6075 6e65 7665 6e5f 6669  d by ``uneven_fi
-0001aae0: 6c6c 5f63 6f6c 6f72 6060 2e0a 0a20 2020  ll_color``...   
-0001aaf0: 203a 7061 7261 6d20 4c69 7374 5b55 6e69   :param List[Uni
-0001ab00: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-0001ab10: 696b 655d 5d20 7669 6465 6f5f 7061 7468  ike]] video_path
-0001ab20: 733a 204c 6973 7420 6f66 2069 6e70 7574  s: List of input
-0001ab30: 2076 6964 656f 2066 696c 6520 7061 7468   video file path
-0001ab40: 732e 0a20 2020 203a 7061 7261 6d20 556e  s..    :param Un
-0001ab50: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-0001ab60: 4c69 6b65 5d20 7361 7665 5f70 6174 683a  Like] save_path:
-0001ab70: 2046 696c 6520 7061 7468 2074 6f20 7361   File path to sa
-0001ab80: 7665 2074 6865 2063 6f6e 6361 7465 6e61  ve the concatena
-0001ab90: 7465 6420 7669 6465 6f2e 0a20 2020 203a  ted video..    :
-0001aba0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b62  param Optional[b
-0001abb0: 6f6f 6c5d 2067 7075 3a20 5768 6574 6865  ool] gpu: Whethe
-0001abc0: 7220 746f 2075 7365 2047 5055 2d61 6363  r to use GPU-acc
-0001abd0: 656c 6572 6174 6564 2063 6f64 6563 2028  elerated codec (
-0001abe0: 6465 6661 756c 743a 2046 616c 7365 292e  default: False).
-0001abf0: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-0001ac00: 6f6e 616c 5b62 6f6f 6c5d 2076 6572 626f  onal[bool] verbo
-0001ac10: 7365 3a20 5768 6574 6865 7220 746f 2070  se: Whether to p
-0001ac20: 7269 6e74 2070 726f 6772 6573 7320 6d65  rint progress me
-0001ac30: 7373 6167 6573 2028 6465 6661 756c 743a  ssages (default:
-0001ac40: 2054 7275 6529 2e0a 0a20 2020 203a 6578   True)...    :ex
-0001ac50: 616d 706c 653a 0a20 2020 203e 3e3e 2076  ample:.    >>> v
-0001ac60: 6964 656f 5f70 6174 6873 203d 205b 2776  ideo_paths = ['v
-0001ac70: 6964 656f 312e 6d70 3427 2c20 2776 6964  ideo1.mp4', 'vid
-0001ac80: 656f 322e 6d70 3427 2c20 2776 6964 656f  eo2.mp4', 'video
-0001ac90: 332e 6d70 3427 5d0a 2020 2020 3e3e 3e20  3.mp4'].    >>> 
-0001aca0: 7361 7665 5f70 6174 6820 3d20 272f 5573  save_path = '/Us
-0001acb0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0001acc0: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0001acd0: 7562 6c65 7368 6f6f 7469 6e67 2f52 4154  ubleshooting/RAT
-0001ace0: 5f4e 4f52 2f70 726f 6a65 6374 5f66 6f6c  _NOR/project_fol
-0001acf0: 6465 722f 7669 6465 6f73 2f74 6573 742f  der/videos/test/
-0001ad00: 6e65 772f 626c 616e 6b5f 7465 7374 2e6d  new/blank_test.m
-0001ad10: 7034 270a 2020 2020 3e3e 3e20 6d69 7865  p4'.    >>> mixe
-0001ad20: 645f 6d6f 7361 6963 5f63 6f6e 6361 7465  d_mosaic_concate
-0001ad30: 6e61 746f 7228 7669 6465 6f5f 7061 7468  nator(video_path
-0001ad40: 733d 7669 6465 6f5f 7061 7468 732c 2073  s=video_paths, s
-0001ad50: 6176 655f 7061 7468 3d73 6176 655f 7061  ave_path=save_pa
-0001ad60: 7468 2c20 6770 753d 4661 6c73 652c 2076  th, gpu=False, v
-0001ad70: 6572 626f 7365 3d54 7275 6529 0a20 2020  erbose=True).   
-0001ad80: 2022 2222 0a0a 2020 2020 6368 6563 6b5f   """..    check_
-0001ad90: 6666 6d70 6567 5f61 7661 696c 6162 6c65  ffmpeg_available
-0001ada0: 2829 0a20 2020 2069 6620 6770 7520 616e  ().    if gpu an
-0001adb0: 6420 6e6f 7420 6368 6563 6b5f 6e76 6964  d not check_nvid
-0001adc0: 6561 5f67 7075 5f61 7661 696c 6162 6c65  ea_gpu_available
-0001add0: 2829 3a0a 2020 2020 2020 2020 7261 6973  ():.        rais
-0001ade0: 6520 4646 4d50 4547 436f 6465 6347 5055  e FFMPEGCodecGPU
-0001adf0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0001ae00: 2020 206d 7367 3d22 4e56 4944 4941 2047     msg="NVIDIA G
-0001ae10: 5055 206e 6f74 2061 7661 696c 6162 6c65  PU not available
-0001ae20: 222c 2073 6f75 7263 653d 6d69 7865 645f  ", source=mixed_
-0001ae30: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
-0001ae40: 746f 722e 5f5f 6e61 6d65 5f5f 0a20 2020  tor.__name__.   
-0001ae50: 2020 2020 2029 0a20 2020 2074 696d 6572       ).    timer
-0001ae60: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
-0001ae70: 6172 743d 5472 7565 290a 2020 2020 6368  art=True).    ch
-0001ae80: 6563 6b5f 7661 6c69 645f 6c73 7428 0a20  eck_valid_lst(. 
-0001ae90: 2020 2020 2020 2064 6174 613d 7669 6465         data=vide
-0001aea0: 6f5f 7061 7468 732c 2073 6f75 7263 653d  o_paths, source=
-0001aeb0: 6d69 7865 645f 6d6f 7361 6963 5f63 6f6e  mixed_mosaic_con
-0001aec0: 6361 7465 6e61 746f 722e 5f5f 6e61 6d65  catenator.__name
-0001aed0: 5f5f 2c20 6d69 6e5f 6c65 6e3d 320a 2020  __, min_len=2.  
-0001aee0: 2020 290a 2020 2020 6474 203d 2064 6174    ).    dt = dat
-0001aef0: 6574 696d 652e 6e6f 7728 292e 7374 7266  etime.now().strf
-0001af00: 7469 6d65 2822 2559 256d 2564 2548 254d  time("%Y%m%d%H%M
-0001af10: 2553 2229 0a20 2020 2076 6964 656f 5f6d  %S").    video_m
-0001af20: 6574 615f 6461 7461 203d 205b 0a20 2020  eta_data = [.   
-0001af30: 2020 2020 2067 6574 5f76 6964 656f 5f6d       get_video_m
-0001af40: 6574 615f 6461 7461 2876 6964 656f 5f70  eta_data(video_p
-0001af50: 6174 683d 7669 6465 6f5f 7061 7468 2920  ath=video_path) 
-0001af60: 666f 7220 7669 6465 6f5f 7061 7468 2069  for video_path i
-0001af70: 6e20 7669 6465 6f5f 7061 7468 730a 2020  n video_paths.  
-0001af80: 2020 5d0a 2020 2020 6d61 785f 7669 6465    ].    max_vide
-0001af90: 6f5f 6c65 6e67 7468 203d 206d 6178 285b  o_length = max([
-0001afa0: 785b 2276 6964 656f 5f6c 656e 6774 685f  x["video_length_
-0001afb0: 7322 5d20 666f 7220 7820 696e 2076 6964  s"] for x in vid
-0001afc0: 656f 5f6d 6574 615f 6461 7461 5d29 0a20  eo_meta_data]). 
-0001afd0: 2020 2063 6865 636b 5f69 665f 6469 725f     check_if_dir_
-0001afe0: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
-0001aff0: 696e 5f64 6972 3d6f 732e 7061 7468 2e64  in_dir=os.path.d
-0001b000: 6972 6e61 6d65 2873 6176 655f 7061 7468  irname(save_path
-0001b010: 292c 2073 6f75 7263 653d 6d69 7865 645f  ), source=mixed_
-0001b020: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
-0001b030: 746f 722e 5f5f 6e61 6d65 5f5f 0a20 2020  tor.__name__.   
-0001b040: 2029 0a20 2020 206c 6172 6765 5f6d 6f73   ).    large_mos
-0001b050: 6169 635f 7061 7468 2c20 7669 6465 6f5f  aic_path, video_
-0001b060: 7061 7468 7320 3d20 7669 6465 6f5f 7061  paths = video_pa
-0001b070: 7468 735b 305d 2c20 7669 6465 6f5f 7061  ths[0], video_pa
-0001b080: 7468 735b 313a 5d0a 2020 2020 6d6f 7361  ths[1:].    mosa
-0001b090: 6963 5f68 6569 6768 7420 3d20 696e 7428  ic_height = int(
-0001b0a0: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
-0001b0b0: 305d 5b22 6865 6967 6874 225d 202f 2032  0]["height"] / 2
-0001b0c0: 290a 2020 2020 6966 2076 6572 626f 7365  ).    if verbose
-0001b0d0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-0001b0e0: 2243 7265 6174 696e 6720 6d69 7865 6420  "Creating mixed 
-0001b0f0: 6d6f 7361 6963 2076 6964 656f 2e2e 2e20  mosaic video... 
-0001b100: 2229 0a20 2020 2074 656d 705f 6469 7220  ").    temp_dir 
-0001b110: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-0001b120: 732e 7061 7468 2e64 6972 6e61 6d65 286c  s.path.dirname(l
-0001b130: 6172 6765 5f6d 6f73 6169 635f 7061 7468  arge_mosaic_path
-0001b140: 292c 2066 2274 656d 705f 7b64 747d 2229  ), f"temp_{dt}")
-0001b150: 0a20 2020 206f 732e 6d61 6b65 6469 7273  .    os.makedirs
-0001b160: 2874 656d 705f 6469 7229 0a20 2020 2069  (temp_dir).    i
-0001b170: 6620 6e6f 7420 286c 656e 2876 6964 656f  f not (len(video
-0001b180: 5f70 6174 6873 2920 2520 3229 203d 3d20  _paths) % 2) == 
-0001b190: 303a 0a20 2020 2020 2020 2062 6c61 6e6b  0:.        blank
-0001b1a0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0001b1b0: 6a6f 696e 2874 656d 705f 6469 722c 2066  join(temp_dir, f
-0001b1c0: 227b 6474 7d2e 6d70 3422 290a 2020 2020  "{dt}.mp4").    
-0001b1d0: 2020 2020 6372 6561 7465 5f62 6c61 6e6b      create_blank
-0001b1e0: 5f76 6964 656f 280a 2020 2020 2020 2020  _video(.        
-0001b1f0: 2020 2020 7061 7468 3d62 6c61 6e6b 5f70      path=blank_p
-0001b200: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0001b210: 206c 656e 6774 683d 6d61 785f 7669 6465   length=max_vide
-0001b220: 6f5f 6c65 6e67 7468 2c0a 2020 2020 2020  o_length,.      
-0001b230: 2020 2020 2020 7769 6474 683d 6765 745f        width=get_
-0001b240: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
-0001b250: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
-0001b260: 5f70 6174 6873 5b2d 315d 295b 2277 6964  _paths[-1])["wid
-0001b270: 7468 225d 2c0a 2020 2020 2020 2020 2020  th"],.          
-0001b280: 2020 6865 6967 6874 3d67 6574 5f76 6964    height=get_vid
-0001b290: 656f 5f6d 6574 615f 6461 7461 2876 6964  eo_meta_data(vid
-0001b2a0: 656f 5f70 6174 683d 7669 6465 6f5f 7061  eo_path=video_pa
-0001b2b0: 7468 735b 2d31 5d29 5b22 6865 6967 6874  ths[-1])["height
-0001b2c0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0001b2d0: 6770 753d 6770 752c 0a20 2020 2020 2020  gpu=gpu,.       
-0001b2e0: 2020 2020 2076 6572 626f 7365 3d54 7275       verbose=Tru
-0001b2f0: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
-0001b300: 6f6c 6f72 3d75 6e65 7665 6e5f 6669 6c6c  olor=uneven_fill
-0001b310: 5f63 6f6c 6f72 2c0a 2020 2020 2020 2020  _color,.        
-0001b320: 290a 2020 2020 2020 2020 7669 6465 6f5f  ).        video_
-0001b330: 7061 7468 732e 6170 7065 6e64 2862 6c61  paths.append(bla
-0001b340: 6e6b 5f70 6174 6829 0a20 2020 2075 7070  nk_path).    upp
-0001b350: 6572 5f76 6964 656f 732c 206c 6f77 6572  er_videos, lower
-0001b360: 5f76 6964 656f 7320 3d20 280a 2020 2020  _videos = (.    
-0001b370: 2020 2020 7669 6465 6f5f 7061 7468 735b      video_paths[
-0001b380: 3a20 6c65 6e28 7669 6465 6f5f 7061 7468  : len(video_path
-0001b390: 7329 202f 2f20 325d 2c0a 2020 2020 2020  s) // 2],.      
-0001b3a0: 2020 7669 6465 6f5f 7061 7468 735b 6c65    video_paths[le
-0001b3b0: 6e28 7669 6465 6f5f 7061 7468 7329 202f  n(video_paths) /
-0001b3c0: 2f20 3220 3a5d 2c0a 2020 2020 290a 2020  / 2 :],.    ).  
-0001b3d0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-0001b3e0: 2020 2020 2020 7072 696e 7428 2243 7265        print("Cre
-0001b3f0: 6174 696e 6720 7570 7065 7220 7269 6768  ating upper righ
-0001b400: 7420 6d6f 7361 6963 202e 2e2e 2028 5374  t mosaic ... (St
-0001b410: 6570 2031 2f34 2922 290a 2020 2020 6966  ep 1/4)").    if
-0001b420: 206c 656e 2875 7070 6572 5f76 6964 656f   len(upper_video
-0001b430: 7329 203e 2031 3a0a 2020 2020 2020 2020  s) > 1:.        
-0001b440: 7570 7065 725f 7061 7468 203d 206f 732e  upper_path = os.
-0001b450: 7061 7468 2e6a 6f69 6e28 7465 6d70 5f64  path.join(temp_d
-0001b460: 6972 2c20 2275 7070 6572 2e6d 7034 2229  ir, "upper.mp4")
-0001b470: 0a20 2020 2020 2020 2068 6f72 697a 6f6e  .        horizon
-0001b480: 7461 6c5f 7669 6465 6f5f 636f 6e63 6174  tal_video_concat
-0001b490: 656e 6174 6f72 280a 2020 2020 2020 2020  enator(.        
-0001b4a0: 2020 2020 7669 6465 6f5f 7061 7468 733d      video_paths=
-0001b4b0: 7570 7065 725f 7669 6465 6f73 2c0a 2020  upper_videos,.  
-0001b4c0: 2020 2020 2020 2020 2020 7361 7665 5f70            save_p
-0001b4d0: 6174 683d 7570 7065 725f 7061 7468 2c0a  ath=upper_path,.
-0001b4e0: 2020 2020 2020 2020 2020 2020 6770 753d              gpu=
-0001b4f0: 6770 752c 0a20 2020 2020 2020 2020 2020  gpu,.           
-0001b500: 2068 6569 6768 745f 7078 3d6d 6f73 6169   height_px=mosai
-0001b510: 635f 6865 6967 6874 2c0a 2020 2020 2020  c_height,.      
-0001b520: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
-0001b530: 7262 6f73 652c 0a20 2020 2020 2020 2029  rbose,.        )
-0001b540: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0001b550: 2020 2075 7070 6572 5f70 6174 6820 3d20     upper_path = 
-0001b560: 7570 7065 725f 7669 6465 6f73 5b30 5d0a  upper_videos[0].
-0001b570: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-0001b580: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
-0001b590: 7265 6174 696e 6720 6c6f 7765 7220 7269  reating lower ri
-0001b5a0: 6768 7420 6d6f 7361 6963 202e 2e2e 2028  ght mosaic ... (
-0001b5b0: 5374 6570 2032 2f34 2922 290a 2020 2020  Step 2/4)").    
-0001b5c0: 6966 206c 656e 286c 6f77 6572 5f76 6964  if len(lower_vid
-0001b5d0: 656f 7329 203e 2031 3a0a 2020 2020 2020  eos) > 1:.      
-0001b5e0: 2020 6c6f 7765 725f 7061 7468 203d 206f    lower_path = o
-0001b5f0: 732e 7061 7468 2e6a 6f69 6e28 7465 6d70  s.path.join(temp
-0001b600: 5f64 6972 2c20 226c 6f77 6572 2e6d 7034  _dir, "lower.mp4
-0001b610: 2229 0a20 2020 2020 2020 2068 6f72 697a  ").        horiz
-0001b620: 6f6e 7461 6c5f 7669 6465 6f5f 636f 6e63  ontal_video_conc
-0001b630: 6174 656e 6174 6f72 280a 2020 2020 2020  atenator(.      
-0001b640: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
-0001b650: 733d 6c6f 7765 725f 7669 6465 6f73 2c0a  s=lower_videos,.
-0001b660: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001b670: 5f70 6174 683d 6c6f 7765 725f 7061 7468  _path=lower_path
-0001b680: 2c0a 2020 2020 2020 2020 2020 2020 6770  ,.            gp
-0001b690: 753d 6770 752c 0a20 2020 2020 2020 2020  u=gpu,.         
-0001b6a0: 2020 2076 6572 626f 7365 3d76 6572 626f     verbose=verbo
-0001b6b0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0001b6c0: 6865 6967 6874 5f70 783d 6d6f 7361 6963  height_px=mosaic
-0001b6d0: 5f68 6569 6768 742c 0a20 2020 2020 2020  _height,.       
-0001b6e0: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-0001b6f0: 2020 2020 206c 6f77 6572 5f70 6174 6820       lower_path 
-0001b700: 3d20 6c6f 7765 725f 7669 6465 6f73 5b30  = lower_videos[0
-0001b710: 5d0a 2020 2020 7061 6e65 6c73 5f6d 6574  ].    panels_met
-0001b720: 6120 3d20 5b0a 2020 2020 2020 2020 6765  a = [.        ge
-0001b730: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
-0001b740: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
-0001b750: 656f 5f70 6174 6829 0a20 2020 2020 2020  eo_path).       
-0001b760: 2066 6f72 2076 6964 656f 5f70 6174 6820   for video_path 
-0001b770: 696e 205b 6c6f 7765 725f 7061 7468 2c20  in [lower_path, 
-0001b780: 7570 7065 725f 7061 7468 5d0a 2020 2020  upper_path].    
-0001b790: 5d0a 2020 2020 6d6f 7361 6963 5f70 6174  ].    mosaic_pat
-0001b7a0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-0001b7b0: 2874 656d 705f 6469 722c 2022 6d6f 7361  (temp_dir, "mosa
-0001b7c0: 6963 2e6d 7034 2229 0a20 2020 2069 6620  ic.mp4").    if 
-0001b7d0: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-0001b7e0: 2070 7269 6e74 2822 4a6f 696e 696e 6720   print("Joining 
-0001b7f0: 7570 7065 7220 616e 6420 6c6f 7765 7220  upper and lower 
-0001b800: 7269 6768 7420 6d6f 7361 6963 2e2e 2e20  right mosaic... 
-0001b810: 2853 7465 7020 332f 3429 2229 0a20 2020  (Step 3/4)").   
-0001b820: 2076 6572 7469 6361 6c5f 7669 6465 6f5f   vertical_video_
-0001b830: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
-0001b840: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
-0001b850: 733d 5b75 7070 6572 5f70 6174 682c 206c  s=[upper_path, l
-0001b860: 6f77 6572 5f70 6174 685d 2c0a 2020 2020  ower_path],.    
-0001b870: 2020 2020 7769 6474 685f 7078 3d6d 6178      width_px=max
-0001b880: 285b 785b 2277 6964 7468 225d 2066 6f72  ([x["width"] for
-0001b890: 2078 2069 6e20 7061 6e65 6c73 5f6d 6574   x in panels_met
-0001b8a0: 615d 292c 0a20 2020 2020 2020 2073 6176  a]),.        sav
-0001b8b0: 655f 7061 7468 3d6d 6f73 6169 635f 7061  e_path=mosaic_pa
-0001b8c0: 7468 2c0a 2020 2020 2020 2020 6770 753d  th,.        gpu=
-0001b8d0: 6770 752c 0a20 2020 2020 2020 2076 6572  gpu,.        ver
-0001b8e0: 626f 7365 3d76 6572 626f 7365 2c0a 2020  bose=verbose,.  
-0001b8f0: 2020 290a 2020 2020 6966 2076 6572 626f    ).    if verbo
-0001b900: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-0001b910: 7428 224a 6f69 6e69 6e67 206c 6566 7420  t("Joining left 
-0001b920: 616e 6420 7269 6768 7420 6d6f 7361 6963  and right mosaic
-0001b930: 2e2e 2e20 2853 7465 7020 342f 3429 2229  ... (Step 4/4)")
-0001b940: 0a20 2020 2068 6f72 697a 6f6e 7461 6c5f  .    horizontal_
-0001b950: 7669 6465 6f5f 636f 6e63 6174 656e 6174  video_concatenat
-0001b960: 6f72 280a 2020 2020 2020 2020 7669 6465  or(.        vide
-0001b970: 6f5f 7061 7468 733d 5b6c 6172 6765 5f6d  o_paths=[large_m
-0001b980: 6f73 6169 635f 7061 7468 2c20 6d6f 7361  osaic_path, mosa
-0001b990: 6963 5f70 6174 685d 2c0a 2020 2020 2020  ic_path],.      
-0001b9a0: 2020 6865 6967 6874 5f69 6478 3d30 2c0a    height_idx=0,.
-0001b9b0: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
-0001b9c0: 683d 7361 7665 5f70 6174 682c 0a20 2020  h=save_path,.   
-0001b9d0: 2020 2020 2067 7075 3d67 7075 2c0a 2020       gpu=gpu,.  
-0001b9e0: 2020 290a 2020 2020 7469 6d65 722e 7374    ).    timer.st
-0001b9f0: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
-0001ba00: 6875 7469 6c2e 726d 7472 6565 2874 656d  hutil.rmtree(tem
-0001ba10: 705f 6469 7229 0a20 2020 2069 6620 7665  p_dir).    if ve
-0001ba20: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-0001ba30: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
-0001ba40: 2020 6622 4d69 7865 6420 6d6f 7361 6963    f"Mixed mosaic
-0001ba50: 2063 6f6e 6361 7465 6e61 7469 6f6e 2063   concatenation c
-0001ba60: 6f6d 706c 6574 652e 2053 6176 6564 2061  omplete. Saved a
-0001ba70: 7420 7b73 6176 655f 7061 7468 7d20 2845  t {save_path} (E
-0001ba80: 6c61 7073 6564 2074 696d 653a 207b 7469  lapsed time: {ti
-0001ba90: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
-0001baa0: 5f73 7472 7d73 2e29 220a 2020 2020 2020  _str}s.)".      
-0001bab0: 2020 290a 0a0a 6465 6620 636c 6970 5f76    )...def clip_v
-0001bac0: 6964 656f 735f 6279 5f66 7261 6d65 5f69  ideos_by_frame_i
-0001bad0: 6473 280a 2020 2020 6669 6c65 5f70 6174  ds(.    file_pat
-0001bae0: 6873 3a20 4c69 7374 5b55 6e69 6f6e 5b73  hs: List[Union[s
-0001baf0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0001bb00: 5d2c 0a20 2020 2066 726d 5f69 6473 3a20  ],.    frm_ids: 
-0001bb10: 4c69 7374 5b4c 6973 745b 696e 745d 5d2c  List[List[int]],
-0001bb20: 0a20 2020 2073 6176 655f 6469 723a 204f  .    save_dir: O
-0001bb30: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-0001bb40: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
-0001bb50: 203d 204e 6f6e 652c 0a29 3a0a 2020 2020   = None,.):.    
-0001bb60: 2222 220a 2020 2020 436c 6970 2076 6964  """.    Clip vid
-0001bb70: 656f 7320 7370 6563 6966 6965 6420 6279  eos specified by
-0001bb80: 2066 7261 6d65 2049 4473 2028 6e75 6d62   frame IDs (numb
-0001bb90: 6572 7329 2e0a 0a20 2020 203a 7061 7261  ers)...    :para
-0001bba0: 6d20 4c69 7374 5b55 6e69 6f6e 5b73 7472  m List[Union[str
-0001bbb0: 2c20 6f73 2e50 6174 684c 696b 655d 5d20  , os.PathLike]] 
-0001bbc0: 6669 6c65 5f70 6174 6873 3a20 4c69 7374  file_paths: List
-0001bbd0: 206f 6620 7061 7468 7320 746f 2069 6e70   of paths to inp
-0001bbe0: 7574 2076 6964 656f 2066 696c 6573 2e0a  ut video files..
-0001bbf0: 2020 2020 3a70 6172 616d 204c 6973 745b      :param List[
-0001bc00: 4c69 7374 5b69 6e74 5d5d 2066 726d 5f69  List[int]] frm_i
-0001bc10: 6473 3a20 4c69 7374 206f 6620 6c69 7374  ds: List of list
-0001bc20: 7320 636f 6e74 6169 6e69 6e67 2073 7461  s containing sta
-0001bc30: 7274 2061 6e64 2065 6e64 2066 7261 6d65  rt and end frame
-0001bc40: 2049 4473 2066 6f72 2065 6163 6820 7669   IDs for each vi
-0001bc50: 6465 6f2e 0a20 2020 203a 7061 7261 6d20  deo..    :param 
-0001bc60: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
-0001bc70: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0001bc80: 5d20 7361 7665 5f64 6972 3a20 2044 6972  ] save_dir:  Dir
-0001bc90: 6563 746f 7279 2074 6f20 7361 7665 2074  ectory to save t
-0001bca0: 6865 2063 6c69 7070 6564 2076 6964 656f  he clipped video
-0001bcb0: 732e 2049 6620 4e6f 6e65 2c20 7669 6465  s. If None, vide
-0001bcc0: 6f73 2077 696c 6c20 6265 2073 6176 6564  os will be saved
-0001bcd0: 2069 6e20 7468 6520 7361 6d65 2064 6972   in the same dir
-0001bce0: 6563 746f 7279 2061 7320 7468 6520 696e  ectory as the in
-0001bcf0: 7075 7420 7669 6465 6f73 2077 6974 6820  put videos with 
-0001bd00: 6672 616d 6520 6e75 6d62 6572 7320 6173  frame numbers as
-0001bd10: 2073 7566 6669 782e 0a20 2020 203a 7265   suffix..    :re
-0001bd20: 7475 726e 3a20 4e6f 6e65 2e0a 0a20 2020  turn: None...   
-0001bd30: 203a 6578 616d 706c 653a 0a20 2020 203e   :example:.    >
-0001bd40: 3e3e 2066 696c 655f 7061 7468 7320 3d20  >> file_paths = 
-0001bd50: 5b27 2f55 7365 7273 2f73 696d 6f6e 2f44  ['/Users/simon/D
-0001bd60: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0001bd70: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0001bd80: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0001bd90: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
-0001bda0: 6d65 732f 6f75 7470 7574 2f70 6174 685f  mes/output/path_
-0001bdb0: 706c 6f74 732f 5472 6961 6c20 2020 2031  plots/Trial    1
-0001bdc0: 302e 6d70 3427 2c20 272f 5573 6572 732f  0.mp4', '/Users/
-0001bdd0: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-0001bde0: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-0001bdf0: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
-0001be00: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
-0001be10: 6465 722f 6672 616d 6573 2f6f 7574 7075  der/frames/outpu
-0001be20: 742f 7061 7468 5f70 6c6f 7473 2f54 7269  t/path_plots/Tri
-0001be30: 616c 2020 2020 3130 5f31 2e6d 7034 275d  al    10_1.mp4']
-0001be40: 0a20 2020 203e 3e3e 2066 726d 5f69 6473  .    >>> frm_ids
-0001be50: 203d 205b 5b30 2c20 3230 5d2c 205b 3230   = [[0, 20], [20
-0001be60: 2c20 3430 5d5d 0a20 2020 203e 3e3e 2063  , 40]].    >>> c
-0001be70: 6c69 705f 7669 6465 6f73 5f62 795f 6672  lip_videos_by_fr
-0001be80: 616d 655f 6964 7328 6669 6c65 5f70 6174  ame_ids(file_pat
-0001be90: 6873 3d66 696c 655f 7061 7468 732c 2066  hs=file_paths, f
-0001bea0: 726d 5f69 6473 3d66 726d 5f69 6473 2c20  rm_ids=frm_ids, 
-0001beb0: 7361 7665 5f64 6972 3d27 2f55 7365 7273  save_dir='/Users
-0001bec0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-0001bed0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-0001bee0: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-0001bef0: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-0001bf00: 6c64 6572 2f66 7261 6d65 732f 6f75 7470  lder/frames/outp
-0001bf10: 7574 2f70 6174 685f 706c 6f74 732f 7472  ut/path_plots/tr
-0001bf20: 6961 6c5f 636e 7427 290a 2020 2020 2222  ial_cnt').    ""
-0001bf30: 220a 0a20 2020 2074 696d 6572 203d 2053  "..    timer = S
-0001bf40: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
-0001bf50: 5472 7565 290a 2020 2020 6368 6563 6b5f  True).    check_
-0001bf60: 7661 6c69 645f 6c73 7428 0a20 2020 2020  valid_lst(.     
-0001bf70: 2020 2064 6174 613d 6669 6c65 5f70 6174     data=file_pat
-0001bf80: 6873 2c0a 2020 2020 2020 2020 736f 7572  hs,.        sour
-0001bf90: 6365 3d63 6c69 705f 7669 6465 6f73 5f62  ce=clip_videos_b
-0001bfa0: 795f 6672 616d 655f 6964 732e 5f5f 6e61  y_frame_ids.__na
-0001bfb0: 6d65 5f5f 2c0a 2020 2020 2020 2020 7661  me__,.        va
-0001bfc0: 6c69 645f 6474 7970 6573 3d28 7374 722c  lid_dtypes=(str,
-0001bfd0: 292c 0a20 2020 2020 2020 206d 696e 5f6c  ),.        min_l
-0001bfe0: 656e 3d31 2c0a 2020 2020 290a 2020 2020  en=1,.    ).    
-0001bff0: 6368 6563 6b5f 7661 6c69 645f 6c73 7428  check_valid_lst(
-0001c000: 0a20 2020 2020 2020 2064 6174 613d 6672  .        data=fr
-0001c010: 6d5f 6964 732c 0a20 2020 2020 2020 2073  m_ids,.        s
-0001c020: 6f75 7263 653d 636c 6970 5f76 6964 656f  ource=clip_video
-0001c030: 735f 6279 5f66 7261 6d65 5f69 6473 2e5f  s_by_frame_ids._
-0001c040: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
-0001c050: 2076 616c 6964 5f64 7479 7065 733d 286c   valid_dtypes=(l
-0001c060: 6973 742c 292c 0a20 2020 2020 2020 2065  ist,),.        e
-0001c070: 7861 6374 5f6c 656e 3d6c 656e 2866 696c  xact_len=len(fil
-0001c080: 655f 7061 7468 7329 2c0a 2020 2020 290a  e_paths),.    ).
-0001c090: 2020 2020 666f 7220 636e 742c 2069 2069      for cnt, i i
-0001c0a0: 6e20 656e 756d 6572 6174 6528 6672 6d5f  n enumerate(frm_
-0001c0b0: 6964 7329 3a0a 2020 2020 2020 2020 6368  ids):.        ch
-0001c0c0: 6563 6b5f 7661 6c69 645f 6c73 7428 0a20  eck_valid_lst(. 
-0001c0d0: 2020 2020 2020 2020 2020 2064 6174 613d             data=
-0001c0e0: 692c 0a20 2020 2020 2020 2020 2020 2073  i,.            s
-0001c0f0: 6f75 7263 653d 6622 636c 6970 5f76 6964  ource=f"clip_vid
-0001c100: 656f 735f 6279 5f66 7261 6d65 5f63 6f75  eos_by_frame_cou
-0001c110: 6e74 2e5f 5f6e 616d 655f 2066 726d 5f69  nt.__name_ frm_i
-0001c120: 6473 207b 636e 747d 222c 0a20 2020 2020  ds {cnt}",.     
-0001c130: 2020 2020 2020 2076 616c 6964 5f64 7479         valid_dty
-0001c140: 7065 733d 2869 6e74 2c29 2c0a 2020 2020  pes=(int,),.    
-0001c150: 2020 2020 2020 2020 6578 6163 745f 6c65          exact_le
-0001c160: 6e3d 322c 0a20 2020 2020 2020 2029 0a20  n=2,.        ). 
-0001c170: 2020 2020 2020 2069 6620 695b 305d 203e         if i[0] >
-0001c180: 3d20 695b 315d 3a0a 2020 2020 2020 2020  = i[1]:.        
-0001c190: 2020 2020 7261 6973 6520 4672 616d 6552      raise FrameR
-0001c1a0: 616e 6765 4572 726f 7228 0a20 2020 2020  angeError(.     
-0001c1b0: 2020 2020 2020 2020 2020 206d 7367 3d66             msg=f
-0001c1c0: 2253 7461 7274 2066 7261 6d65 2066 6f72  "Start frame for
-0001c1d0: 2076 6964 656f 207b 697d 2069 7320 6166   video {i} is af
-0001c1e0: 7465 7220 6f72 2074 6865 2073 616d 6520  ter or the same 
-0001c1f0: 6173 2074 6865 2065 6e64 2066 7261 6d65  as the end frame
-0001c200: 2028 7b69 5b30 5d7d 2c20 7b69 5b31 5d7d   ({i[0]}, {i[1]}
-0001c210: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-0001c220: 2020 2020 736f 7572 6365 3d63 6c69 705f      source=clip_
-0001c230: 7669 6465 6f73 5f62 795f 6672 616d 655f  videos_by_frame_
-0001c240: 6964 732e 5f5f 6e61 6d65 5f5f 2c0a 2020  ids.__name__,.  
-0001c250: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001c260: 2020 2020 6966 2028 695b 305d 203c 2030      if (i[0] < 0
-0001c270: 2920 6f72 2028 695b 315d 203c 2031 293a  ) or (i[1] < 1):
-0001c280: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001c290: 7365 2046 7261 6d65 5261 6e67 6545 7272  se FrameRangeErr
-0001c2a0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0001c2b0: 2020 2020 6d73 673d 6622 5374 6172 7420      msg=f"Start 
-0001c2c0: 6672 616d 6520 6861 7320 746f 2062 6520  frame has to be 
-0001c2d0: 6174 206c 6561 7374 2030 2061 6e64 2065  at least 0 and e
-0001c2e0: 6e64 2066 7261 6d65 2068 6173 2074 6f20  nd frame has to 
-0001c2f0: 6265 2061 7420 6c65 6173 7420 3122 2c0a  be at least 1",.
-0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c310: 736f 7572 6365 3d63 6c69 705f 7669 6465  source=clip_vide
-0001c320: 6f73 5f62 795f 6672 616d 655f 6964 732e  os_by_frame_ids.
-0001c330: 5f5f 6e61 6d65 5f5f 2c0a 2020 2020 2020  __name__,.      
-0001c340: 2020 2020 2020 290a 2020 2020 7669 6465        ).    vide
-0001c350: 6f5f 6d65 7461 5f64 6174 6120 3d20 5b67  o_meta_data = [g
-0001c360: 6574 5f76 6964 656f 5f6d 6574 615f 6461  et_video_meta_da
-0001c370: 7461 2876 6964 656f 5f70 6174 683d 7829  ta(video_path=x)
-0001c380: 2066 6f72 2078 2069 6e20 6669 6c65 5f70   for x in file_p
-0001c390: 6174 6873 5d0a 2020 2020 666f 7220 6920  aths].    for i 
-0001c3a0: 696e 2072 616e 6765 286c 656e 2876 6964  in range(len(vid
-0001c3b0: 656f 5f6d 6574 615f 6461 7461 2929 3a0a  eo_meta_data)):.
-0001c3c0: 2020 2020 2020 2020 6966 2028 6672 6d5f          if (frm_
-0001c3d0: 6964 735b 695d 5b30 5d20 3e20 7669 6465  ids[i][0] > vide
-0001c3e0: 6f5f 6d65 7461 5f64 6174 615b 695d 5b22  o_meta_data[i]["
-0001c3f0: 6672 616d 655f 636f 756e 7422 5d29 206f  frame_count"]) o
-0001c400: 7220 280a 2020 2020 2020 2020 2020 2020  r (.            
-0001c410: 6672 6d5f 6964 735b 695d 5b31 5d20 3e20  frm_ids[i][1] > 
-0001c420: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
-0001c430: 695d 5b22 6672 616d 655f 636f 756e 7422  i]["frame_count"
-0001c440: 5d0a 2020 2020 2020 2020 293a 0a20 2020  ].        ):.   
-0001c450: 2020 2020 2020 2020 2072 6169 7365 2046           raise F
-0001c460: 7261 6d65 5261 6e67 6545 7272 6f72 280a  rameRangeError(.
-0001c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c480: 6d73 673d 6627 5669 6465 6f20 7b69 2b31  msg=f'Video {i+1
-0001c490: 7d20 6861 7320 7b76 6964 656f 5f6d 6574  } has {video_met
-0001c4a0: 615f 6461 7461 5b69 5d5b 2266 7261 6d65  a_data[i]["frame
-0001c4b0: 5f63 6f75 6e74 225d 7d20 6672 616d 6573  _count"]} frames
-0001c4c0: 2c20 6361 6e6e 6f74 2075 7365 2073 7461  , cannot use sta
-0001c4d0: 7274 2061 6e64 2065 6e64 2066 7261 6d65  rt and end frame
-0001c4e0: 207b 6672 6d5f 6964 735b 695d 7d27 2c0a   {frm_ids[i]}',.
-0001c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c500: 736f 7572 6365 3d63 6c69 705f 7669 6465  source=clip_vide
-0001c510: 6f73 5f62 795f 6672 616d 655f 6964 732e  os_by_frame_ids.
-0001c520: 5f5f 6e61 6d65 5f5f 2c0a 2020 2020 2020  __name__,.      
-0001c530: 2020 2020 2020 290a 2020 2020 6966 2073        ).    if s
-0001c540: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
-0001c550: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
-0001c560: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
-0001c570: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-0001c580: 5f64 6972 3d73 6176 655f 6469 722c 0a20  _dir=save_dir,. 
-0001c590: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0001c5a0: 653d 636c 6970 5f76 6964 656f 735f 6279  e=clip_videos_by
-0001c5b0: 5f66 7261 6d65 5f69 6473 2e5f 5f6e 616d  _frame_ids.__nam
-0001c5c0: 655f 5f2c 0a20 2020 2020 2020 2020 2020  e__,.           
-0001c5d0: 2063 7265 6174 655f 6966 5f6e 6f74 5f65   create_if_not_e
-0001c5e0: 7869 7374 3d54 7275 652c 0a20 2020 2020  xist=True,.     
-0001c5f0: 2020 2029 0a20 2020 2066 6f72 2063 6e74     ).    for cnt
-0001c600: 2c20 6669 6c65 5f70 6174 6820 696e 2065  , file_path in e
-0001c610: 6e75 6d65 7261 7465 2866 696c 655f 7061  numerate(file_pa
-0001c620: 7468 7329 3a0a 2020 2020 2020 2020 7669  ths):.        vi
-0001c630: 6465 6f5f 7469 6d65 7220 3d20 5369 6d62  deo_timer = Simb
-0001c640: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
-0001c650: 6529 0a20 2020 2020 2020 2064 6972 2c20  e).        dir, 
-0001c660: 7669 6465 6f5f 6e61 6d65 2c20 6578 7420  video_name, ext 
-0001c670: 3d20 6765 745f 666e 5f65 7874 2866 696c  = get_fn_ext(fil
-0001c680: 6570 6174 683d 6669 6c65 5f70 6174 6829  epath=file_path)
-0001c690: 0a20 2020 2020 2020 2073 5f66 2c20 655f  .        s_f, e_
-0001c6a0: 6620 3d20 6672 6d5f 6964 735b 636e 745d  f = frm_ids[cnt]
-0001c6b0: 5b30 5d2c 2066 726d 5f69 6473 5b63 6e74  [0], frm_ids[cnt
-0001c6c0: 5d5b 315d 0a20 2020 2020 2020 2070 7269  ][1].        pri
-0001c6d0: 6e74 2866 2254 7269 6d6d 696e 6720 7b76  nt(f"Trimming {v
-0001c6e0: 6964 656f 5f6e 616d 657d 2066 726f 6d20  ideo_name} from 
-0001c6f0: 6672 616d 6520 7b73 5f66 7d20 746f 2066  frame {s_f} to f
-0001c700: 7261 6d65 207b 655f 667d 2e2e 2e22 290a  rame {e_f}...").
-0001c710: 2020 2020 2020 2020 6966 2073 6176 655f          if save_
-0001c720: 6469 7220 6973 206e 6f74 204e 6f6e 653a  dir is not None:
-0001c730: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-0001c740: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0001c750: 6a6f 696e 2873 6176 655f 6469 722c 206f  join(save_dir, o
-0001c760: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0001c770: 6669 6c65 5f70 6174 6829 290a 2020 2020  file_path)).    
-0001c780: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001c790: 2020 2020 2020 6f75 745f 7061 7468 203d        out_path =
-0001c7a0: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
-0001c7b0: 722c 2066 227b 7669 6465 6f5f 6e61 6d65  r, f"{video_name
-0001c7c0: 7d5f 7b73 5f66 7d5f 7b65 5f66 7d7b 6578  }_{s_f}_{e_f}{ex
-0001c7d0: 747d 2229 0a20 2020 2020 2020 2063 6d64  t}").        cmd
-0001c7e0: 203d 2066 2766 666d 7065 6720 2d69 2022   = f'ffmpeg -i "
-0001c7f0: 7b66 696c 655f 7061 7468 7d22 202d 7666  {file_path}" -vf
-0001c800: 2022 7472 696d 3d7b 735f 667d 3a7b 655f   "trim={s_f}:{e_
-0001c810: 667d 2c73 6574 7074 733d 5054 532d 5354  f},setpts=PTS-ST
-0001c820: 4152 5450 5453 2220 2d63 3a76 206c 6962  ARTPTS" -c:v lib
-0001c830: 7832 3634 202d 633a 6120 6161 6320 2d6c  x264 -c:a aac -l
-0001c840: 6f67 6c65 7665 6c20 6572 726f 7220 2d73  oglevel error -s
-0001c850: 7461 7473 2022 7b6f 7574 5f70 6174 687d  tats "{out_path}
-0001c860: 2220 2d79 270a 2020 2020 2020 2020 7375  " -y'.        su
-0001c870: 6270 726f 6365 7373 2e63 616c 6c28 636d  bprocess.call(cm
-0001c880: 642c 2073 6865 6c6c 3d54 7275 652c 2073  d, shell=True, s
-0001c890: 7464 6f75 743d 7375 6270 726f 6365 7373  tdout=subprocess
-0001c8a0: 2e50 4950 4529 0a20 2020 2020 2020 2076  .PIPE).        v
-0001c8b0: 6964 656f 5f74 696d 6572 2e73 746f 705f  ideo_timer.stop_
-0001c8c0: 7469 6d65 7228 290a 2020 2020 2020 2020  timer().        
-0001c8d0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0001c8e0: 2020 2066 2256 6964 656f 207b 7669 6465     f"Video {vide
-0001c8f0: 6f5f 6e61 6d65 7d20 636f 6d70 6c65 7465  o_name} complete
-0001c900: 2028 656c 6170 7365 6420 7469 6d65 207b   (elapsed time {
-0001c910: 7669 6465 6f5f 7469 6d65 722e 656c 6170  video_timer.elap
-0001c920: 7365 645f 7469 6d65 5f73 7472 7d73 2922  sed_time_str}s)"
-0001c930: 0a20 2020 2020 2020 2029 0a20 2020 2074  .        ).    t
-0001c940: 696d 6572 2e73 746f 705f 7469 6d65 7228  imer.stop_timer(
-0001c950: 290a 2020 2020 6966 2073 6176 655f 6469  ).    if save_di
-0001c960: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-0001c970: 2020 2073 7464 6f75 745f 7375 6363 6573     stdout_succes
-0001c980: 7328 0a20 2020 2020 2020 2020 2020 206d  s(.            m
-0001c990: 7367 3d66 227b 6c65 6e28 6669 6c65 5f70  sg=f"{len(file_p
-0001c9a0: 6174 6873 297d 2076 6964 656f 2873 2920  aths)} video(s) 
-0001c9b0: 636c 6970 7065 6420 6279 2066 7261 6d65  clipped by frame
-0001c9c0: 222c 0a20 2020 2020 2020 2020 2020 2065  ",.            e
-0001c9d0: 6c61 7073 6564 5f74 696d 653d 7469 6d65  lapsed_time=time
-0001c9e0: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
-0001c9f0: 7472 2c0a 2020 2020 2020 2020 290a 2020  tr,.        ).  
-0001ca00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001ca10: 7374 646f 7574 5f73 7563 6365 7373 280a  stdout_success(.
-0001ca20: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-0001ca30: 6622 7b6c 656e 2866 696c 655f 7061 7468  f"{len(file_path
-0001ca40: 7329 7d20 7669 6465 6f28 7329 2063 6c69  s)} video(s) cli
-0001ca50: 7070 6564 2062 7920 6672 616d 6520 616e  pped by frame an
-0001ca60: 6420 7361 7665 6420 696e 207b 7361 7665  d saved in {save
-0001ca70: 5f64 6972 7d22 2c0a 2020 2020 2020 2020  _dir}",.        
-0001ca80: 2020 2020 656c 6170 7365 645f 7469 6d65      elapsed_time
-0001ca90: 3d74 696d 6572 2e65 6c61 7073 6564 5f74  =timer.elapsed_t
-0001caa0: 696d 655f 7374 722c 0a20 2020 2020 2020  ime_str,.       
-0001cab0: 2029 0a0a 0a23 2076 6964 656f 5f70 6174   )...# video_pat
-0001cac0: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
-0001cad0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-0001cae0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-0001caf0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
-0001cb00: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
-0001cb10: 722f 6d65 7267 652f 5472 6961 6c20 2020  r/merge/Trial   
-0001cb20: 2031 305f 636c 6970 7065 645f 6761 6e74   10_clipped_gant
-0001cb30: 742e 6d70 3427 2c0a 2320 2020 2020 2020  t.mp4',.#       
-0001cb40: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
-0001cb50: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-0001cb60: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-0001cb70: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-0001cb80: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-0001cb90: 6c64 6572 2f6d 6572 6765 2f54 7269 616c  lder/merge/Trial
-0001cba0: 2020 2020 3130 5f63 6c69 7070 6564 2e6d      10_clipped.m
-0001cbb0: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
-0001cbc0: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
-0001cbd0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-0001cbe0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-0001cbf0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
-0001cc00: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
-0001cc10: 722f 6d65 7267 652f 5472 6961 6c20 2020  r/merge/Trial   
-0001cc20: 2031 305f 636c 6970 7065 645f 6c69 6e65   10_clipped_line
-0001cc30: 2e6d 7034 272c 0a23 2020 2020 2020 2020  .mp4',.#        
-0001cc40: 2020 2020 2020 2020 272f 5573 6572 732f          '/Users/
-0001cc50: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-0001cc60: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-0001cc70: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
-0001cc80: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
-0001cc90: 6465 722f 6d65 7267 652f 5472 6961 6c20  der/merge/Trial 
-0001cca0: 2020 2020 335f 636c 6970 7065 642e 6d70      3_clipped.mp
-0001ccb0: 3427 5d0a 230a 2320 7669 6465 6f5f 7061  4'].#.# video_pa
-0001ccc0: 7468 7320 3d20 5b27 2f55 7365 7273 2f73  ths = ['/Users/s
-0001ccd0: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-0001cce0: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-0001ccf0: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
-0001cd00: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
-0001cd10: 6572 2f76 6964 656f 732f 5472 6961 6c20  er/videos/Trial 
-0001cd20: 2020 2031 302e 6d70 3427 2c0a 2320 2020     10.mp4',.#   
-0001cd30: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
-0001cd40: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-0001cd50: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-0001cd60: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
-0001cd70: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
-0001cd80: 745f 666f 6c64 6572 2f6d 6572 6765 2f54  t_folder/merge/T
-0001cd90: 7269 616c 2020 2020 3130 5f63 6c69 7070  rial    10_clipp
-0001cda0: 6564 5f67 616e 7474 2e6d 7034 272c 0a23  ed_gantt.mp4',.#
-0001cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cdc0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
-0001cdd0: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
-0001cde0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
-0001cdf0: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
-0001ce00: 6a65 6374 5f66 6f6c 6465 722f 6d65 7267  ject_folder/merg
-0001ce10: 652f 5472 6961 6c20 2020 2031 305f 636c  e/Trial    10_cl
-0001ce20: 6970 7065 645f 6c69 6e65 2e6d 7034 272c  ipped_line.mp4',
-0001ce30: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-0001ce40: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
-0001ce50: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0001ce60: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0001ce70: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
-0001ce80: 726f 6a65 6374 5f66 6f6c 6465 722f 6d65  roject_folder/me
-0001ce90: 7267 652f 5472 6961 6c20 2020 2020 335f  rge/Trial     3_
-0001cea0: 636c 6970 7065 642e 6d70 3427 5d0a 230a  clipped.mp4'].#.
-0001ceb0: 2320 7361 7665 5f70 6174 6820 3d20 272f  # save_path = '/
-0001cec0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-0001ced0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-0001cee0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
-0001cef0: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
-0001cf00: 6374 5f66 6f6c 6465 722f 6d65 7267 652f  ct_folder/merge/
-0001cf10: 6f75 742e 6d70 3427 0a0a 230a 2320 7669  out.mp4'..#.# vi
-0001cf20: 6465 6f5f 7061 7468 7320 3d20 5b27 2f55  deo_paths = ['/U
-0001cf30: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-0001cf40: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-0001cf50: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
-0001cf60: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
-0001cf70: 745f 666f 6c64 6572 2f66 7261 6d65 732f  t_folder/frames/
-0001cf80: 6f75 7470 7574 2f67 616e 7474 5f70 6c6f  output/gantt_plo
-0001cf90: 7473 2f54 7269 616c 2020 2020 3130 2e6d  ts/Trial    10.m
-0001cfa0: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
-0001cfb0: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
-0001cfc0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-0001cfd0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-0001cfe0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
-0001cff0: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
-0001d000: 722f 7669 6465 6f73 2f54 7269 616c 2020  r/videos/Trial  
-0001d010: 2020 3130 2e6d 7034 272c 0a23 2020 2020    10.mp4',.#    
-0001d020: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
-0001d030: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0001d040: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0001d050: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
-0001d060: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
-0001d070: 5f66 6f6c 6465 722f 6672 616d 6573 2f6f  _folder/frames/o
-0001d080: 7574 7075 742f 6c69 6e65 5f70 6c6f 742f  utput/line_plot/
-0001d090: 5472 6961 6c20 2020 2031 302e 6d70 3427  Trial    10.mp4'
-0001d0a0: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
-0001d0b0: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
-0001d0c0: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-0001d0d0: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-0001d0e0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
-0001d0f0: 7072 6f6a 6563 745f 666f 6c64 6572 2f66  project_folder/f
-0001d100: 7261 6d65 732f 6f75 7470 7574 2f6c 696e  rames/output/lin
-0001d110: 655f 706c 6f74 2f54 7269 616c 2020 2020  e_plot/Trial    
-0001d120: 2033 2e6d 7034 275d 0a23 2073 6176 655f   3.mp4'].# save_
-0001d130: 7061 7468 203d 2027 2f55 7365 7273 2f73  path = '/Users/s
-0001d140: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-0001d150: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-0001d160: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
-0001d170: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-0001d180: 6964 656f 732f 7465 7374 2f6e 6577 2f62  ideos/test/new/b
-0001d190: 6c61 6e6b 5f74 6573 742e 6d70 3427 0a0a  lank_test.mp4'..
-0001d1a0: 2320 7669 6465 6f5f 7061 7468 7320 3d20  # video_paths = 
-0001d1b0: 5b27 2f55 7365 7273 2f73 696d 6f6e 2f44  ['/Users/simon/D
-0001d1c0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0001d1d0: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0001d1e0: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0001d1f0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-0001d200: 656f 732f 5472 6961 6c20 2020 2031 302e  eos/Trial    10.
-0001d210: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
-0001d220: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
-0001d230: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-0001d240: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-0001d250: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
-0001d260: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
-0001d270: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
-0001d280: 2f6c 696e 655f 706c 6f74 2f54 7269 616c  /line_plot/Trial
-0001d290: 2020 2020 3130 2e6d 7034 272c 0a23 2020      10.mp4',.#  
-0001d2a0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-0001d2b0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-0001d2c0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-0001d2d0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
-0001d2e0: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
-0001d2f0: 6374 5f66 6f6c 6465 722f 6672 616d 6573  ct_folder/frames
-0001d300: 2f6f 7574 7075 742f 6c69 6e65 5f70 6c6f  /output/line_plo
-0001d310: 742f 5472 6961 6c20 2020 2020 332e 6d70  t/Trial     3.mp
-0001d320: 3427 5d0a 0a23 206d 6978 6564 5f6d 6f73  4']..# mixed_mos
-0001d330: 6169 635f 636f 6e63 6174 656e 6174 6f72  aic_concatenator
-0001d340: 2876 6964 656f 5f70 6174 6873 3d76 6964  (video_paths=vid
-0001d350: 656f 5f70 6174 6873 2c20 7361 7665 5f70  eo_paths, save_p
-0001d360: 6174 683d 7361 7665 5f70 6174 682c 2067  ath=save_path, g
-0001d370: 7075 3d46 616c 7365 2c20 7665 7262 6f73  pu=False, verbos
-0001d380: 653d 5472 7565 290a                      e=True).
+0000fe30: 2073 656c 662e 7361 7665 5f64 6972 2c20   self.save_dir, 
+0000fe40: 6622 7b6e 616d 657d 5f72 6f74 6174 6564  f"{name}_rotated
+0000fe50: 5f7b 7365 6c66 2e64 6174 6574 696d 657d  _{self.datetime}
+0000fe60: 2e6d 7034 220a 2020 2020 2020 2020 2020  .mp4".          
+0000fe70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000fe80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fe90: 6770 753a 0a20 2020 2020 2020 2020 2020  gpu:.           
+0000fea0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+0000feb0: 2766 666d 7065 6720 2d68 7761 6363 656c  'ffmpeg -hwaccel
+0000fec0: 2061 7574 6f20 2d69 2022 7b76 6964 656f   auto -i "{video
+0000fed0: 5f70 6174 687d 2220 2d76 6620 2268 7775  _path}" -vf "hwu
+0000fee0: 706c 6f61 645f 6375 6461 2c72 6f74 6174  pload_cuda,rotat
+0000fef0: 653d 7b72 6f74 6174 696f 6e7d 2a28 5049  e={rotation}*(PI
+0000ff00: 2f31 3830 292c 666f 726d 6174 3d6e 7631  /180),format=nv1
+0000ff10: 327c 6375 6461 2220 2d63 3a76 2068 3236  2|cuda" -c:v h26
+0000ff20: 345f 6e76 656e 6320 227b 7361 7665 5f70  4_nvenc "{save_p
+0000ff30: 6174 687d 2220 2d79 270a 2020 2020 2020  ath}" -y'.      
+0000ff40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff60: 2020 2020 636d 6420 3d20 6627 6666 6d70      cmd = f'ffmp
+0000ff70: 6567 202d 6920 227b 7669 6465 6f5f 7061  eg -i "{video_pa
+0000ff80: 7468 7d22 202d 7666 2022 726f 7461 7465  th}" -vf "rotate
+0000ff90: 3d7b 726f 7461 7469 6f6e 7d2a 2850 492f  ={rotation}*(PI/
+0000ffa0: 3138 3029 2220 227b 7361 7665 5f70 6174  180)" "{save_pat
+0000ffb0: 687d 2220 2d79 270a 2020 2020 2020 2020  h}" -y'.        
+0000ffc0: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+0000ffd0: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
+0000ffe0: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
+0000fff0: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
+00010000: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00010010: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
+00010020: 6964 656f 5f63 6e74 2c20 2876 6964 656f  ideo_cnt, (video
+00010030: 5f70 6174 682c 2072 6f74 6174 696f 6e29  _path, rotation)
+00010040: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
+00010050: 6c66 2e72 6573 756c 7473 2e69 7465 6d73  lf.results.items
+00010060: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+00010070: 2020 2020 2063 6170 203d 2063 7632 2e56       cap = cv2.V
+00010080: 6964 656f 4361 7074 7572 6528 7669 6465  ideoCapture(vide
+00010090: 6f5f 7061 7468 290a 2020 2020 2020 2020  o_path).        
+000100a0: 2020 2020 2020 2020 5f2c 206e 616d 652c          _, name,
+000100b0: 205f 203d 2067 6574 5f66 6e5f 6578 7428   _ = get_fn_ext(
+000100c0: 6669 6c65 7061 7468 3d76 6964 656f 5f70  filepath=video_p
+000100d0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+000100e0: 2020 2020 2072 6f74 6174 696f 6e5f 6d61       rotation_ma
+000100f0: 7472 6978 203d 2063 7632 2e67 6574 526f  trix = cv2.getRo
+00010100: 7461 7469 6f6e 4d61 7472 6978 3244 280a  tationMatrix2D(.
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00010130: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010140: 6c66 2e76 6964 656f 5f6d 6574 615f 6461  lf.video_meta_da
+00010150: 7461 5b22 7769 6474 6822 5d20 2f20 322c  ta["width"] / 2,
+00010160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010170: 2020 2020 2020 2020 2073 656c 662e 7669           self.vi
+00010180: 6465 6f5f 6d65 7461 5f64 6174 615b 2268  deo_meta_data["h
+00010190: 6569 6768 7422 5d20 2f20 322c 0a20 2020  eight"] / 2,.   
+000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101b0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000101c0: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+000101d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000101e0: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+000101f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010200: 2020 2020 2020 2020 2020 2073 6176 655f             save_
+00010210: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00010220: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+00010230: 2020 2020 2020 2020 2073 656c 662e 7361           self.sa
+00010240: 7665 5f64 6972 2c20 6622 7b6e 616d 657d  ve_dir, f"{name}
+00010250: 5f72 6f74 6174 6564 5f7b 7365 6c66 2e64  _rotated_{self.d
+00010260: 6174 6574 696d 657d 2e6d 7034 220a 2020  atetime}.mp4".  
+00010270: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010290: 7669 6465 6f5f 6d65 7461 203d 2067 6574  video_meta = get
+000102a0: 5f76 6964 656f 5f6d 6574 615f 6461 7461  _video_meta_data
+000102b0: 2876 6964 656f 5f70 6174 683d 7669 6465  (video_path=vide
+000102c0: 6f5f 7061 7468 290a 2020 2020 2020 2020  o_path).        
+000102d0: 2020 2020 2020 2020 666f 7572 6363 203d          fourcc =
+000102e0: 2063 7632 2e56 6964 656f 5772 6974 6572   cv2.VideoWriter
+000102f0: 5f66 6f75 7263 6328 2a46 6f72 6d61 7473  _fourcc(*Formats
+00010300: 2e4d 5034 5f43 4f44 4543 2e76 616c 7565  .MP4_CODEC.value
+00010310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010320: 2020 7772 6974 6572 203d 2063 7632 2e56    writer = cv2.V
+00010330: 6964 656f 5772 6974 6572 280a 2020 2020  ideoWriter(.    
+00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010350: 7361 7665 5f70 6174 682c 0a20 2020 2020  save_path,.     
+00010360: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010370: 6f75 7263 632c 0a20 2020 2020 2020 2020  ourcc,.         
+00010380: 2020 2020 2020 2020 2020 2076 6964 656f             video
+00010390: 5f6d 6574 615b 2266 7073 225d 2c0a 2020  _meta["fps"],.  
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2020 2876 6964 656f 5f6d 6574 615b 2277    (video_meta["w
+000103c0: 6964 7468 225d 2c20 7669 6465 6f5f 6d65  idth"], video_me
+000103d0: 7461 5b22 6865 6967 6874 225d 292c 0a20  ta["height"]),. 
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000103f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010400: 2069 6d67 5f63 6e74 203d 2030 0a20 2020   img_cnt = 0.   
+00010410: 2020 2020 2020 2020 2020 2020 2077 6869               whi
+00010420: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+00010430: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010440: 2c20 696d 6720 3d20 6361 702e 7265 6164  , img = cap.read
+00010450: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010460: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
+00010470: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00010480: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00010490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000104a0: 2020 2020 2069 6d67 203d 2063 7632 2e77       img = cv2.w
+000104b0: 6172 7041 6666 696e 6528 0a20 2020 2020  arpAffine(.     
+000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104d0: 2020 2069 6d67 2c0a 2020 2020 2020 2020     img,.        
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104f0: 726f 7461 7469 6f6e 5f6d 6174 7269 782c  rotation_matrix,
+00010500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010510: 2020 2020 2020 2020 2028 7365 6c66 2e76           (self.v
+00010520: 6964 656f 5f6d 6574 615f 6461 7461 5b22  ideo_meta_data["
+00010530: 7769 6474 6822 5d2c 2073 656c 662e 7669  width"], self.vi
+00010540: 6465 6f5f 6d65 7461 5f64 6174 615b 2268  deo_meta_data["h
+00010550: 6569 6768 7422 5d29 2c0a 2020 2020 2020  eight"]),.      
+00010560: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010580: 2020 2020 7772 6974 6572 2e77 7269 7465      writer.write
+00010590: 2869 6d67 290a 2020 2020 2020 2020 2020  (img).          
+000105a0: 2020 2020 2020 2020 2020 696d 675f 636e            img_cn
+000105b0: 7420 2b3d 2031 0a20 2020 2020 2020 2020  t += 1.         
+000105c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000105d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000105e0: 2020 2020 2020 2020 2020 6627 526f 7461            f'Rota
+000105f0: 7469 6e67 2066 7261 6d65 207b 696d 675f  ting frame {img_
+00010600: 636e 747d 2f7b 7669 6465 6f5f 6d65 7461  cnt}/{video_meta
+00010610: 5b22 6672 616d 655f 636f 756e 7422 5d7d  ["frame_count"]}
+00010620: 2028 5669 6465 6f20 7b76 6964 656f 5f63   (Video {video_c
+00010630: 6e74 202b 2031 7d2f 7b6c 656e 2873 656c  nt + 1}/{len(sel
+00010640: 662e 7265 7375 6c74 732e 6b65 7973 2829  f.results.keys()
+00010650: 297d 2920 270a 2020 2020 2020 2020 2020  )}) '.          
+00010660: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00010670: 2020 2020 2020 2020 2020 2020 6361 702e              cap.
+00010680: 7265 6c65 6173 6528 290a 2020 2020 2020  release().      
+00010690: 2020 2020 2020 2020 2020 7772 6974 6572            writer
+000106a0: 2e72 656c 6561 7365 2829 0a20 2020 2020  .release().     
+000106b0: 2020 2073 7464 6f75 745f 7375 6363 6573     stdout_succes
+000106c0: 7328 0a20 2020 2020 2020 2020 2020 206d  s(.            m
+000106d0: 7367 3d66 2241 6c6c 2076 6964 656f 7320  sg=f"All videos 
+000106e0: 726f 7461 7465 6420 616e 6420 7361 7665  rotated and save
+000106f0: 6420 696e 207b 7365 6c66 2e73 6176 655f  d in {self.save_
+00010700: 6469 727d 222c 0a20 2020 2020 2020 2020  dir}",.         
+00010710: 2020 2065 6c61 7073 6564 5f74 696d 653d     elapsed_time=
+00010720: 7374 7228 726f 756e 6428 2874 696d 652e  str(round((time.
+00010730: 7469 6d65 2829 202d 2073 7461 7274 292c  time() - start),
+00010740: 2032 2929 2c0a 2020 2020 2020 2020 2020   2)),.          
+00010750: 2020 736f 7572 6365 3d73 656c 662e 5f5f    source=self.__
+00010760: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00010770: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00010780: 2064 6566 205f 5f73 6176 6528 7365 6c66   def __save(self
+00010790: 293a 0a20 2020 2020 2020 2070 726f 6365  ):.        proce
+000107a0: 7373 203d 204e 6f6e 650a 2020 2020 2020  ss = None.      
+000107b0: 2020 7365 6c66 2e72 6573 756c 7473 5b73    self.results[s
+000107c0: 656c 662e 6669 6c65 5f70 6174 685d 203d  elf.file_path] =
+000107d0: 2073 656c 662e 6469 665f 616e 676c 650a   self.dif_angle.
+000107e0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+000107f0: 656c 662e 7265 7375 6c74 732e 6b65 7973  elf.results.keys
+00010800: 2829 2920 3d3d 206c 656e 2873 656c 662e  ()) == len(self.
+00010810: 7669 6465 6f5f 7061 7468 7329 3a0a 2020  video_paths):.  
+00010820: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+00010830: 7320 3d20 6d75 6c74 6970 726f 6365 7373  s = multiprocess
+00010840: 696e 672e 5072 6f63 6573 7328 7461 7267  ing.Process(targ
+00010850: 6574 3d73 656c 662e 5f5f 7275 6e5f 726f  et=self.__run_ro
+00010860: 7461 7469 6f6e 2829 290a 2020 2020 2020  tation()).      
+00010870: 2020 2020 2020 7072 6f63 6573 732e 7374        process.st
+00010880: 6172 7428 290a 2020 2020 2020 2020 656c  art().        el
+00010890: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000108a0: 7365 6c66 2e5f 5f72 756e 5f69 6e74 6572  self.__run_inter
+000108b0: 6661 6365 280a 2020 2020 2020 2020 2020  face(.          
+000108c0: 2020 2020 2020 6669 6c65 5f70 6174 683d        file_path=
+000108d0: 7365 6c66 2e76 6964 656f 5f70 6174 6873  self.video_paths
+000108e0: 5b6c 656e 2873 656c 662e 7265 7375 6c74  [len(self.result
+000108f0: 732e 6b65 7973 2829 2920 2d20 315d 0a20  s.keys()) - 1]. 
+00010900: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010910: 2020 2020 2069 6620 7072 6f63 6573 7320       if process 
+00010920: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010930: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00010940: 2e6a 6f69 6e28 290a 0a20 2020 2064 6566  .join()..    def
+00010950: 205f 5f62 696e 645f 6b65 7973 2873 656c   __bind_keys(sel
+00010960: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00010970: 2e6d 6169 6e5f 6672 6d2e 6269 6e64 280a  .main_frm.bind(.
+00010980: 2020 2020 2020 2020 2020 2020 223c 4c65              "<Le
+00010990: 6674 3e22 2c20 6c61 6d62 6461 2078 3a20  ft>", lambda x: 
+000109a0: 7365 6c66 2e5f 5f72 6f74 6174 6528 7661  self.__rotate(va
+000109b0: 6c75 653d 312c 2069 6d67 3d73 656c 662e  lue=1, img=self.
+000109c0: 5f6f 7269 675f 696d 6729 0a20 2020 2020  _orig_img).     
+000109d0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+000109e0: 662e 6d61 696e 5f66 726d 2e62 696e 6428  f.main_frm.bind(
+000109f0: 0a20 2020 2020 2020 2020 2020 2022 3c52  .            "<R
+00010a00: 6967 6874 3e22 2c20 6c61 6d62 6461 2078  ight>", lambda x
+00010a10: 3a20 7365 6c66 2e5f 5f72 6f74 6174 6528  : self.__rotate(
+00010a20: 7661 6c75 653d 2d31 2c20 696d 673d 7365  value=-1, img=se
+00010a30: 6c66 2e5f 6f72 6967 5f69 6d67 290a 2020  lf._orig_img).  
+00010a40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010a50: 7365 6c66 2e6d 6169 6e5f 6672 6d2e 6269  self.main_frm.bi
+00010a60: 6e64 2822 3c45 7363 6170 653e 222c 206c  nd("<Escape>", l
+00010a70: 616d 6264 6120 783a 2073 656c 662e 5f5f  ambda x: self.__
+00010a80: 7361 7665 2829 290a 0a20 2020 2064 6566  save())..    def
+00010a90: 205f 5f72 756e 5f69 6e74 6572 6661 6365   __run_interface
+00010aa0: 2873 656c 662c 2066 696c 655f 7061 7468  (self, file_path
+00010ab0: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+00010ac0: 7365 6c66 2e64 6966 5f61 6e67 6c65 203d  self.dif_angle =
+00010ad0: 2030 0a20 2020 2020 2020 2070 7269 6e74   0.        print
+00010ae0: 2866 696c 655f 7061 7468 290a 2020 2020  (file_path).    
+00010af0: 2020 2020 7365 6c66 2e76 6964 656f 5f6d      self.video_m
+00010b00: 6574 615f 6461 7461 203d 2067 6574 5f76  eta_data = get_v
+00010b10: 6964 656f 5f6d 6574 615f 6461 7461 2876  ideo_meta_data(v
+00010b20: 6964 656f 5f70 6174 683d 6669 6c65 5f70  ideo_path=file_p
+00010b30: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
+00010b40: 662e 6669 6c65 5f70 6174 6820 3d20 6669  f.file_path = fi
+00010b50: 6c65 5f70 6174 680a 2020 2020 2020 2020  le_path.        
+00010b60: 5f2c 2073 656c 662e 7669 6465 6f5f 6e61  _, self.video_na
+00010b70: 6d65 2c20 5f20 3d20 6765 745f 666e 5f65  me, _ = get_fn_e
+00010b80: 7874 2866 696c 6570 6174 683d 6669 6c65  xt(filepath=file
+00010b90: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
+00010ba0: 656c 662e 6d61 696e 5f66 726d 203d 2054  elf.main_frm = T
+00010bb0: 6f70 6c65 7665 6c28 290a 2020 2020 2020  oplevel().      
+00010bc0: 2020 7365 6c66 2e6d 6169 6e5f 6672 6d2e    self.main_frm.
+00010bd0: 7469 746c 6528 6622 524f 5441 5445 2056  title(f"ROTATE V
+00010be0: 4944 454f 207b 7365 6c66 2e76 6964 656f  IDEO {self.video
+00010bf0: 5f6e 616d 657d 2229 0a20 2020 2020 2020  _name}").       
+00010c00: 2073 656c 662e 7669 6465 6f5f 6672 6d20   self.video_frm 
+00010c10: 3d20 4672 616d 6528 7365 6c66 2e6d 6169  = Frame(self.mai
+00010c20: 6e5f 6672 6d29 0a20 2020 2020 2020 2073  n_frm).        s
+00010c30: 656c 662e 7669 6465 6f5f 6672 6d2e 6772  elf.video_frm.gr
+00010c40: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
+00010c50: 3d30 290a 2020 2020 2020 2020 7365 6c66  =0).        self
+00010c60: 2e69 6e73 7472 7563 7469 6f6e 5f66 726d  .instruction_frm
+00010c70: 203d 2046 7261 6d65 2873 656c 662e 6d61   = Frame(self.ma
+00010c80: 696e 5f66 726d 2c20 7769 6474 683d 3130  in_frm, width=10
+00010c90: 302c 2068 6569 6768 743d 3130 3029 0a20  0, height=100). 
+00010ca0: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00010cb0: 7275 6374 696f 6e5f 6672 6d2e 6772 6964  ruction_frm.grid
+00010cc0: 2872 6f77 3d30 2c20 636f 6c75 6d6e 3d32  (row=0, column=2
+00010cd0: 2c20 7374 6963 6b79 3d4e 5729 0a20 2020  , sticky=NW).   
+00010ce0: 2020 2020 2073 656c 662e 6b65 795f 6c62       self.key_lb
+00010cf0: 6c73 203d 204c 6162 656c 280a 2020 2020  ls = Label(.    
+00010d00: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
+00010d10: 7472 7563 7469 6f6e 5f66 726d 2c0a 2020  truction_frm,.  
+00010d20: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
+00010d30: 5c6e 5c6e 204e 6176 6967 6174 696f 6e3a  \n\n Navigation:
+00010d40: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+00010d50: 5c6e 204c 6566 7420 6172 726f 7720 3d20  \n Left arrow = 
+00010d60: 31c2 b020 6c65 6674 220a 2020 2020 2020  1.. left".      
+00010d70: 2020 2020 2020 225c 6e20 5269 6768 7420        "\n Right 
+00010d80: 6172 726f 7720 3d20 31c2 b020 7269 6768  arrow = 1.. righ
+00010d90: 7422 0a20 2020 2020 2020 2020 2020 2022  t".            "
+00010da0: 5c6e 2045 7363 203d 2053 6176 6522 2c0a  \n Esc = Save",.
+00010db0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010dc0: 2020 2073 656c 662e 6b65 795f 6c62 6c73     self.key_lbls
+00010dd0: 2e67 7269 6428 7374 6963 6b79 3d4e 5729  .grid(sticky=NW)
+00010de0: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
+00010df0: 7020 3d20 6376 322e 5669 6465 6f43 6170  p = cv2.VideoCap
+00010e00: 7475 7265 2866 696c 655f 7061 7468 290a  ture(file_path).
+00010e10: 2020 2020 2020 2020 5f2c 2073 656c 662e          _, self.
+00010e20: 696d 6720 3d20 7365 6c66 2e63 6170 2e72  img = self.cap.r
+00010e30: 6561 6428 290a 2020 2020 2020 2020 7365  ead().        se
+00010e40: 6c66 2e5f 6f72 6967 5f69 6d67 203d 2063  lf._orig_img = c
+00010e50: 7632 2e63 7674 436f 6c6f 7228 7365 6c66  v2.cvtColor(self
+00010e60: 2e69 6d67 2c20 6376 322e 434f 4c4f 525f  .img, cv2.COLOR_
+00010e70: 5247 4232 4247 5229 0a20 2020 2020 2020  RGB2BGR).       
+00010e80: 2073 656c 662e 5f5f 696e 7365 7274 5f69   self.__insert_i
+00010e90: 6d67 2869 6d67 3d73 656c 662e 5f6f 7269  mg(img=self._ori
+00010ea0: 675f 696d 6729 0a20 2020 2020 2020 2073  g_img).        s
+00010eb0: 656c 662e 5f5f 6269 6e64 5f6b 6579 7328  elf.__bind_keys(
+00010ec0: 290a 0a20 2020 2064 6566 2072 756e 2873  )..    def run(s
+00010ed0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00010ee0: 6c66 2e72 6573 756c 7473 203d 207b 7d0a  lf.results = {}.
+00010ef0: 2020 2020 2020 2020 666f 7220 7669 6465          for vide
+00010f00: 6f5f 7061 7468 2069 6e20 7365 6c66 2e76  o_path in self.v
+00010f10: 6964 656f 5f70 6174 6873 3a0a 2020 2020  ideo_paths:.    
+00010f20: 2020 2020 2020 2020 7365 6c66 2e5f 5f72          self.__r
+00010f30: 756e 5f69 6e74 6572 6661 6365 2876 6964  un_interface(vid
+00010f40: 656f 5f70 6174 6829 0a20 2020 2020 2020  eo_path).       
+00010f50: 2073 656c 662e 6d61 696e 5f66 726d 2e6d   self.main_frm.m
+00010f60: 6169 6e6c 6f6f 7028 290a 0a0a 6465 6620  ainloop()...def 
+00010f70: 6578 7472 6163 745f 6672 616d 6573 5f66  extract_frames_f
+00010f80: 726f 6d5f 616c 6c5f 7669 6465 6f73 5f69  rom_all_videos_i
+00010f90: 6e5f 6469 7265 6374 6f72 7928 0a20 2020  n_directory(.   
+00010fa0: 2063 6f6e 6669 675f 7061 7468 3a20 556e   config_path: Un
+00010fb0: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00010fc0: 4c69 6b65 5d2c 2064 6972 6563 746f 7279  Like], directory
+00010fd0: 3a20 556e 696f 6e5b 7374 722c 206f 732e  : Union[str, os.
+00010fe0: 5061 7468 4c69 6b65 5d0a 2920 2d3e 204e  PathLike].) -> N
+00010ff0: 6f6e 653a 0a20 2020 2022 2222 0a20 2020  one:.    """.   
+00011000: 2045 7874 7261 6374 2061 6c6c 2066 7261   Extract all fra
+00011010: 6d65 7320 6672 6f6d 2061 6c6c 2076 6964  mes from all vid
+00011020: 656f 7320 696e 2061 2064 6972 6563 746f  eos in a directo
+00011030: 7279 2e20 5468 6520 7265 7375 6c74 7320  ry. The results 
+00011040: 6172 6520 7361 7665 6420 696e 2074 6865  are saved in the
+00011050: 2070 726f 6a65 6374 5f66 6f6c 6465 722f   project_folder/
+00011060: 6672 616d 6573 2f69 6e70 7574 2064 6972  frames/input dir
+00011070: 6563 746f 7279 206f 6620 7468 6520 5369  ectory of the Si
+00011080: 6d42 4120 7072 6f6a 6563 740a 0a20 2020  mBA project..   
+00011090: 203a 7061 7261 6d65 7465 7220 7374 7220   :parameter str 
+000110a0: 636f 6e66 6967 5f70 6174 683a 2070 6174  config_path: pat
+000110b0: 6820 746f 2053 696d 4241 2070 726f 6a65  h to SimBA proje
+000110c0: 6374 2063 6f6e 6669 6720 6669 6c65 2069  ct config file i
+000110d0: 6e20 436f 6e66 6967 7061 7273 6572 2066  n Configparser f
+000110e0: 6f72 6d61 742e 0a20 2020 203a 7061 7261  ormat..    :para
+000110f0: 6d65 7465 7220 7374 7220 6469 7265 6374  meter str direct
+00011100: 6f72 793a 2070 6174 6820 746f 2066 696c  ory: path to fil
+00011110: 6520 6f72 2066 6f6c 6465 7220 636f 6e74  e or folder cont
+00011120: 6169 6e69 6e67 2076 6964 656f 7320 696e  aining videos in
+00011130: 206d 7034 2061 6e64 2f6f 7220 6176 6920   mp4 and/or avi 
+00011140: 666f 726d 6174 2e0a 0a20 2020 203a 6578  format...    :ex
+00011150: 616d 706c 653a 0a20 2020 203e 3e3e 2065  ample:.    >>> e
+00011160: 7874 7261 6374 5f66 7261 6d65 735f 6672  xtract_frames_fr
+00011170: 6f6d 5f61 6c6c 5f76 6964 656f 735f 696e  om_all_videos_in
+00011180: 5f64 6972 6563 746f 7279 2863 6f6e 6669  _directory(confi
+00011190: 675f 7061 7468 3d27 7072 6f6a 6563 745f  g_path='project_
+000111a0: 666f 6c64 6572 2f70 726f 6a65 6374 5f63  folder/project_c
+000111b0: 6f6e 6669 672e 696e 6927 2c20 736f 7572  onfig.ini', sour
+000111c0: 6365 3d27 2f74 6573 7473 2f74 6573 745f  ce='/tests/test_
+000111d0: 6461 7461 2f76 6964 656f 5f74 6573 7473  data/video_tests
+000111e0: 2729 0a20 2020 2022 2222 0a0a 2020 2020  ').    """..    
+000111f0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+00011200: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+00011210: 2020 2076 6964 656f 5f70 6174 6873 2c20     video_paths, 
+00011220: 7669 6465 6f5f 7479 7065 7320 3d20 5b5d  video_types = []
+00011230: 2c20 5b22 2e61 7669 222c 2022 2e6d 7034  , [".avi", ".mp4
+00011240: 225d 0a20 2020 2066 696c 6573 5f69 6e5f  "].    files_in_
+00011250: 666f 6c64 6572 203d 2067 6c6f 622e 676c  folder = glob.gl
+00011260: 6f62 2864 6972 6563 746f 7279 202b 2022  ob(directory + "
+00011270: 2f2a 2229 0a20 2020 2066 6f72 2066 696c  /*").    for fil
+00011280: 655f 7061 7468 2069 6e20 6669 6c65 735f  e_path in files_
+00011290: 696e 5f66 6f6c 6465 723a 0a20 2020 2020  in_folder:.     
+000112a0: 2020 205f 2c20 5f2c 2065 7874 203d 2067     _, _, ext = g
+000112b0: 6574 5f66 6e5f 6578 7428 6669 6c65 7061  et_fn_ext(filepa
+000112c0: 7468 3d66 696c 655f 7061 7468 290a 2020  th=file_path).  
+000112d0: 2020 2020 2020 6966 2065 7874 2e6c 6f77        if ext.low
+000112e0: 6572 2829 2069 6e20 7669 6465 6f5f 7479  er() in video_ty
+000112f0: 7065 733a 0a20 2020 2020 2020 2020 2020  pes:.           
+00011300: 2076 6964 656f 5f70 6174 6873 2e61 7070   video_paths.app
+00011310: 656e 6428 6669 6c65 5f70 6174 6829 0a20  end(file_path). 
+00011320: 2020 2069 6620 6c65 6e28 7669 6465 6f5f     if len(video_
+00011330: 7061 7468 7329 203d 3d20 303a 0a20 2020  paths) == 0:.   
+00011340: 2020 2020 2072 6169 7365 204e 6f46 696c       raise NoFil
+00011350: 6573 466f 756e 6445 7272 6f72 280a 2020  esFoundError(.  
+00011360: 2020 2020 2020 2020 2020 6d73 673d 6622            msg=f"
+00011370: 5349 4d42 4120 4552 524f 523a 2030 2076  SIMBA ERROR: 0 v
+00011380: 6964 656f 2066 696c 6573 2069 6e20 6d70  ideo files in mp
+00011390: 3420 6f72 2061 7669 2066 6f72 6d61 7420  4 or avi format 
+000113a0: 666f 756e 6420 696e 207b 6469 7265 6374  found in {direct
+000113b0: 6f72 797d 222c 0a20 2020 2020 2020 2020  ory}",.         
+000113c0: 2020 2073 6f75 7263 653d 6578 7472 6163     source=extrac
+000113d0: 745f 6672 616d 6573 5f66 726f 6d5f 616c  t_frames_from_al
+000113e0: 6c5f 7669 6465 6f73 5f69 6e5f 6469 7265  l_videos_in_dire
+000113f0: 6374 6f72 792e 5f5f 6e61 6d65 5f5f 2c0a  ctory.__name__,.
+00011400: 2020 2020 2020 2020 290a 2020 2020 636f          ).    co
+00011410: 6e66 6967 203d 2072 6561 645f 636f 6e66  nfig = read_conf
+00011420: 6967 5f66 696c 6528 636f 6e66 6967 5f70  ig_file(config_p
+00011430: 6174 6829 0a20 2020 2070 726f 6a65 6374  ath).    project
+00011440: 5f70 6174 6820 3d20 7265 6164 5f63 6f6e  _path = read_con
+00011450: 6669 675f 656e 7472 7928 0a20 2020 2020  fig_entry(.     
+00011460: 2020 2063 6f6e 6669 672c 2022 4765 6e65     config, "Gene
+00011470: 7261 6c20 7365 7474 696e 6773 222c 2022  ral settings", "
+00011480: 7072 6f6a 6563 745f 7061 7468 222c 2064  project_path", d
+00011490: 6174 615f 7479 7065 3d22 666f 6c64 6572  ata_type="folder
+000114a0: 5f70 6174 6822 0a20 2020 2029 0a0a 2020  _path".    )..  
+000114b0: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+000114c0: 2022 4578 7472 6163 7469 6e67 2066 7261   "Extracting fra
+000114d0: 6d65 7320 666f 7220 7b7d 2076 6964 656f  mes for {} video
+000114e0: 7320 696e 746f 2070 726f 6a65 6374 5f66  s into project_f
+000114f0: 6f6c 6465 722f 6672 616d 6573 2f69 6e70  older/frames/inp
+00011500: 7574 2064 6972 6563 746f 7279 2e2e 2e22  ut directory..."
+00011510: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00011520: 2020 2020 206c 656e 2876 6964 656f 5f70       len(video_p
+00011530: 6174 6873 290a 2020 2020 2020 2020 290a  aths).        ).
+00011540: 2020 2020 290a 2020 2020 666f 7220 7669      ).    for vi
+00011550: 6465 6f5f 7061 7468 2069 6e20 7669 6465  deo_path in vide
+00011560: 6f5f 7061 7468 733a 0a20 2020 2020 2020  o_paths:.       
+00011570: 2064 6972 5f6e 616d 652c 2076 6964 656f   dir_name, video
+00011580: 5f6e 616d 652c 2065 7874 203d 2067 6574  _name, ext = get
+00011590: 5f66 6e5f 6578 7428 7669 6465 6f5f 7061  _fn_ext(video_pa
+000115a0: 7468 290a 2020 2020 2020 2020 7361 7665  th).        save
+000115b0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+000115c0: 6a6f 696e 2870 726f 6a65 6374 5f70 6174  join(project_pat
+000115d0: 682c 2022 6672 616d 6573 222c 2022 696e  h, "frames", "in
+000115e0: 7075 7422 2c20 7669 6465 6f5f 6e61 6d65  put", video_name
+000115f0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00011600: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+00011610: 7361 7665 5f70 6174 6829 3a0a 2020 2020  save_path):.    
+00011620: 2020 2020 2020 2020 6f73 2e6d 616b 6564          os.maked
+00011630: 6972 7328 7361 7665 5f70 6174 6829 0a20  irs(save_path). 
+00011640: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011650: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 6622 4672 616d 6573 2066 6f72 2076 6964  f"Frames for vid
+00011680: 656f 207b 7669 6465 6f5f 6e61 6d65 7d20  eo {video_name} 
+00011690: 616c 7265 6164 7920 6578 7472 6163 7465  already extracte
+000116a0: 642e 2053 696d 4241 2069 7320 6f76 6572  d. SimBA is over
+000116b0: 7772 6974 696e 6720 7072 696f 7220 6672  writing prior fr
+000116c0: 616d 6573 2e2e 2e22 0a20 2020 2020 2020  ames...".       
+000116d0: 2020 2020 2029 0a20 2020 2020 2020 2076       ).        v
+000116e0: 6964 656f 5f74 6f5f 6672 616d 6573 2876  ideo_to_frames(v
+000116f0: 6964 656f 5f70 6174 682c 2073 6176 655f  ideo_path, save_
+00011700: 7061 7468 2c20 6f76 6572 7772 6974 653d  path, overwrite=
+00011710: 5472 7565 2c20 6576 6572 793d 312c 2063  True, every=1, c
+00011720: 6875 6e6b 5f73 697a 653d 3130 3030 290a  hunk_size=1000).
+00011730: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
+00011740: 696d 6572 2829 0a20 2020 2073 7464 6f75  imer().    stdou
+00011750: 745f 7375 6363 6573 7328 0a20 2020 2020  t_success(.     
+00011760: 2020 2066 2246 7261 6d65 7320 6372 6561     f"Frames crea
+00011770: 7465 6420 666f 7220 7b73 7472 286c 656e  ted for {str(len
+00011780: 2876 6964 656f 5f70 6174 6873 2929 7d20  (video_paths))} 
+00011790: 7669 6465 6f73 222c 0a20 2020 2020 2020  videos",.       
+000117a0: 2065 6c61 7073 6564 5f74 696d 653d 7469   elapsed_time=ti
+000117b0: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
+000117c0: 5f73 7472 2c0a 2020 2020 2020 2020 736f  _str,.        so
+000117d0: 7572 6365 3d65 7874 7261 6374 5f66 7261  urce=extract_fra
+000117e0: 6d65 735f 6672 6f6d 5f61 6c6c 5f76 6964  mes_from_all_vid
+000117f0: 656f 735f 696e 5f64 6972 6563 746f 7279  eos_in_directory
+00011800: 2e5f 5f6e 616d 655f 5f2c 0a20 2020 2029  .__name__,.    )
+00011810: 0a0a 0a64 6566 2063 6f70 795f 696d 675f  ...def copy_img_
+00011820: 666f 6c64 6572 280a 2020 2020 636f 6e66  folder(.    conf
+00011830: 6967 5f70 6174 683a 2055 6e69 6f6e 5b73  ig_path: Union[s
+00011840: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+00011850: 2c20 736f 7572 6365 3a20 556e 696f 6e5b  , source: Union[
+00011860: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+00011870: 5d0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ].) -> None:.   
+00011880: 2022 2222 0a20 2020 2043 6f70 7920 6469   """.    Copy di
+00011890: 7265 6374 6f72 7920 6f66 2070 6e67 2066  rectory of png f
+000118a0: 696c 6573 2074 6f20 7468 6520 5369 6d42  iles to the SimB
+000118b0: 4120 7072 6f6a 6563 742e 2054 6865 2064  A project. The d
+000118c0: 6972 6563 746f 7279 2069 7320 7374 6f72  irectory is stor
+000118d0: 6564 2069 6e20 7468 6520 7072 6f6a 6563  ed in the projec
+000118e0: 745f 666f 6c64 6572 2f66 7261 6d65 732f  t_folder/frames/
+000118f0: 696e 7075 7420 666f 6c64 6572 206f 6620  input folder of 
+00011900: 7468 6520 5369 6d42 4120 7072 6f6a 6563  the SimBA projec
+00011910: 740a 0a20 2020 203a 7061 7261 6d65 7465  t..    :paramete
+00011920: 7220 7374 7220 636f 6e66 6967 5f70 6174  r str config_pat
+00011930: 683a 2070 6174 6820 746f 2053 696d 4241  h: path to SimBA
+00011940: 2070 726f 6a65 6374 2063 6f6e 6669 6720   project config 
+00011950: 6669 6c65 2069 6e20 436f 6e66 6967 7061  file in Configpa
+00011960: 7273 6572 2066 6f72 6d61 742e 0a20 2020  rser format..   
+00011970: 203a 7061 7261 6d65 7465 7220 7374 7220   :parameter str 
+00011980: 736f 7572 6365 3a20 7061 7468 2074 6f20  source: path to 
+00011990: 696d 6167 6520 666f 6c64 6572 206f 7574  image folder out
+000119a0: 7369 6465 2053 696d 4241 2070 726f 6a65  side SimBA proje
+000119b0: 6374 2e0a 0a20 2020 203a 6578 616d 706c  ct...    :exampl
+000119c0: 653a 0a20 2020 203e 3e3e 2063 6f70 795f  e:.    >>> copy_
+000119d0: 696d 675f 666f 6c64 6572 2863 6f6e 6669  img_folder(confi
+000119e0: 675f 7061 7468 3d27 4d79 5369 6d42 4170  g_path='MySimBAp
+000119f0: 726f 6a65 6374 436f 6e66 6967 272c 2073  rojectConfig', s
+00011a00: 6f75 7263 653d 272f 4469 7265 6374 6f72  ource='/Director
+00011a10: 7957 6974 6856 6964 656f 732f 2729 0a0a  yWithVideos/')..
+00011a20: 2020 2020 2222 220a 2020 2020 7469 6d65      """.    time
+00011a30: 7220 3d20 5369 6d62 6154 696d 6572 2873  r = SimbaTimer(s
+00011a40: 7461 7274 3d54 7275 6529 0a20 2020 2069  tart=True).    i
+00011a50: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+00011a60: 6469 7228 736f 7572 6365 293a 0a20 2020  dir(source):.   
+00011a70: 2020 2020 2072 6169 7365 204e 6f74 4469       raise NotDi
+00011a80: 7265 6374 6f72 7945 7272 6f72 280a 2020  rectoryError(.  
+00011a90: 2020 2020 2020 2020 2020 6d73 673d 6622            msg=f"
+00011aa0: 5349 4d42 4120 4552 524f 523a 2073 6f75  SIMBA ERROR: sou
+00011ab0: 7263 6520 7b73 6f75 7263 657d 2069 7320  rce {source} is 
+00011ac0: 6e6f 7420 6120 6469 7265 6374 6f72 792e  not a directory.
+00011ad0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+00011ae0: 6f75 7263 653d 636f 7079 5f69 6d67 5f66  ource=copy_img_f
+00011af0: 6f6c 6465 722e 5f5f 6e61 6d65 5f5f 2c0a  older.__name__,.
+00011b00: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
+00011b10: 206c 656e 2867 6c6f 622e 676c 6f62 2873   len(glob.glob(s
+00011b20: 6f75 7263 6520 2b20 222f 2a2e 706e 6722  ource + "/*.png"
+00011b30: 2929 203d 3d20 303a 0a20 2020 2020 2020  )) == 0:.       
+00011b40: 2072 6169 7365 204e 6f46 696c 6573 466f   raise NoFilesFo
+00011b50: 756e 6445 7272 6f72 280a 2020 2020 2020  undError(.      
+00011b60: 2020 2020 2020 6d73 673d 6622 5349 4d42        msg=f"SIMB
+00011b70: 4120 4552 524f 523a 2073 6f75 7263 6520  A ERROR: source 
+00011b80: 7b73 6f75 7263 657d 2064 6f65 7320 6e6f  {source} does no
+00011b90: 7420 636f 6e74 6169 6e20 616e 7920 2e70  t contain any .p
+00011ba0: 6e67 2066 696c 6573 2e22 2c0a 2020 2020  ng files.",.    
+00011bb0: 2020 2020 2020 2020 736f 7572 6365 3d63          source=c
+00011bc0: 6f70 795f 696d 675f 666f 6c64 6572 2e5f  opy_img_folder._
+00011bd0: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
+00011be0: 2029 0a20 2020 2069 6e70 7574 5f62 6173   ).    input_bas
+00011bf0: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
+00011c00: 6261 7365 6e61 6d65 2873 6f75 7263 6529  basename(source)
+00011c10: 0a20 2020 2063 6f6e 6669 6720 3d20 7265  .    config = re
+00011c20: 6164 5f63 6f6e 6669 675f 6669 6c65 2863  ad_config_file(c
+00011c30: 6f6e 6669 675f 7061 7468 290a 2020 2020  onfig_path).    
+00011c40: 7072 6f6a 6563 745f 7061 7468 203d 2072  project_path = r
+00011c50: 6561 645f 636f 6e66 6967 5f65 6e74 7279  ead_config_entry
+00011c60: 280a 2020 2020 2020 2020 636f 6e66 6967  (.        config
+00011c70: 2c0a 2020 2020 2020 2020 436f 6e66 6967  ,.        Config
+00011c80: 4b65 792e 4745 4e45 5241 4c5f 5345 5454  Key.GENERAL_SETT
+00011c90: 494e 4753 2e76 616c 7565 2c0a 2020 2020  INGS.value,.    
+00011ca0: 2020 2020 436f 6e66 6967 4b65 792e 5052      ConfigKey.PR
+00011cb0: 4f4a 4543 545f 5041 5448 2e76 616c 7565  OJECT_PATH.value
+00011cc0: 2c0a 2020 2020 2020 2020 6461 7461 5f74  ,.        data_t
+00011cd0: 7970 653d 2266 6f6c 6465 725f 7061 7468  ype="folder_path
+00011ce0: 222c 0a20 2020 2029 0a20 2020 2069 6e70  ",.    ).    inp
+00011cf0: 7574 5f66 7261 6d65 735f 6469 7220 3d20  ut_frames_dir = 
+00011d00: 6f73 2e70 6174 682e 6a6f 696e 2870 726f  os.path.join(pro
+00011d10: 6a65 6374 5f70 6174 682c 2050 6174 6873  ject_path, Paths
+00011d20: 2e49 4e50 5554 5f46 5241 4d45 535f 4449  .INPUT_FRAMES_DI
+00011d30: 522e 7661 6c75 6529 0a20 2020 2064 6573  R.value).    des
+00011d40: 7469 6e61 7469 6f6e 203d 206f 732e 7061  tination = os.pa
+00011d50: 7468 2e6a 6f69 6e28 696e 7075 745f 6672  th.join(input_fr
+00011d60: 616d 6573 5f64 6972 2c20 696e 7075 745f  ames_dir, input_
+00011d70: 6261 7365 6e61 6d65 290a 2020 2020 6966  basename).    if
+00011d80: 206f 732e 7061 7468 2e69 7364 6972 2864   os.path.isdir(d
+00011d90: 6573 7469 6e61 7469 6f6e 293a 0a20 2020  estination):.   
+00011da0: 2020 2020 2072 6169 7365 2044 6972 6563       raise Direc
+00011db0: 746f 7279 4578 6973 7445 7272 6f72 280a  toryExistError(.
+00011dc0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00011dd0: 6622 5349 4d42 4120 4552 524f 523a 207b  f"SIMBA ERROR: {
+00011de0: 6465 7374 696e 6174 696f 6e7d 2061 6c72  destination} alr
+00011df0: 6561 6479 2065 7869 7374 2069 6e20 5369  eady exist in Si
+00011e00: 6d42 4120 7072 6f6a 6563 742e 222c 0a20  mBA project.",. 
+00011e10: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+00011e20: 653d 636f 7079 5f69 6d67 5f66 6f6c 6465  e=copy_img_folde
+00011e30: 722e 5f5f 6e61 6d65 5f5f 2c0a 2020 2020  r.__name__,.    
+00011e40: 2020 2020 290a 2020 2020 7072 696e 7428      ).    print(
+00011e50: 6622 496d 706f 7274 696e 6720 696d 6167  f"Importing imag
+00011e60: 6520 6669 6c65 7320 666f 7220 7b69 6e70  e files for {inp
+00011e70: 7574 5f62 6173 656e 616d 657d 2e2e 2e22  ut_basename}..."
+00011e80: 290a 2020 2020 7368 7574 696c 2e63 6f70  ).    shutil.cop
+00011e90: 7974 7265 6528 736f 7572 6365 2c20 6465  ytree(source, de
+00011ea0: 7374 696e 6174 696f 6e29 0a20 2020 2074  stination).    t
+00011eb0: 696d 6572 2e73 746f 705f 7469 6d65 7228  imer.stop_timer(
+00011ec0: 290a 2020 2020 7374 646f 7574 5f73 7563  ).    stdout_suc
+00011ed0: 6365 7373 280a 2020 2020 2020 2020 6d73  cess(.        ms
+00011ee0: 673d 6622 7b64 6573 7469 6e61 7469 6f6e  g=f"{destination
+00011ef0: 7d20 696d 706f 7274 6564 2074 6f20 5369  } imported to Si
+00011f00: 6d42 4120 7072 6f6a 6563 7422 2c0a 2020  mBA project",.  
+00011f10: 2020 2020 2020 656c 6170 7365 645f 7469        elapsed_ti
+00011f20: 6d65 3d74 696d 6572 2e65 6c61 7073 6564  me=timer.elapsed
+00011f30: 5f74 696d 655f 7374 722c 0a20 2020 2020  _time_str,.     
+00011f40: 2020 2073 6f75 7263 653d 636f 7079 5f69     source=copy_i
+00011f50: 6d67 5f66 6f6c 6465 722e 5f5f 6e61 6d65  mg_folder.__name
+00011f60: 5f5f 2c0a 2020 2020 290a 0a0a 6465 6620  __,.    )...def 
+00011f70: 6170 7065 6e64 5f61 7564 696f 280a 2020  append_audio(.  
+00011f80: 2020 7669 6465 6f5f 7061 7468 3a20 556e    video_path: Un
+00011f90: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00011fa0: 4c69 6b65 5d2c 0a20 2020 2061 7564 696f  Like],.    audio
+00011fb0: 5f70 6174 683a 2055 6e69 6f6e 5b73 7472  _path: Union[str
+00011fc0: 2c20 6f73 2e50 6174 684c 696b 655d 2c0a  , os.PathLike],.
+00011fd0: 2020 2020 6175 6469 6f5f 7372 635f 7479      audio_src_ty
+00011fe0: 7065 3a20 4c69 7465 7261 6c5b 2276 6964  pe: Literal["vid
+00011ff0: 656f 222c 2022 6175 6469 6f22 5d20 3d20  eo", "audio"] = 
+00012000: 2276 6964 656f 222c 0a29 202d 3e20 4e6f  "video",.) -> No
+00012010: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
+00012020: 4170 7065 6e64 2061 7564 696f 2074 7261  Append audio tra
+00012030: 636b 2066 726f 6d20 6f6e 6520 7669 6465  ck from one vide
+00012040: 6f20 746f 2061 6e6f 7468 6572 2076 6964  o to another vid
+00012050: 656f 2077 6974 686f 7574 2061 6e20 6175  eo without an au
+00012060: 6469 6f20 7472 6163 6b2e 0a0a 2020 2020  dio track...    
+00012070: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
+00012080: 2c20 6f73 2e50 6174 684c 696b 655d 2076  , os.PathLike] v
+00012090: 6964 656f 5f6f 6e65 5f70 6174 683a 2050  ideo_one_path: P
+000120a0: 6174 6820 746f 2076 6964 656f 2066 696c  ath to video fil
+000120b0: 6520 7769 7468 6f75 7420 6175 6469 6f20  e without audio 
+000120c0: 7472 6163 6b2e 0a20 2020 203a 7061 7261  track..    :para
+000120d0: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
+000120e0: 5061 7468 4c69 6b65 5d20 6175 6469 6f5f  PathLike] audio_
+000120f0: 7061 7468 3a20 5061 7468 2074 6f20 6669  path: Path to fi
+00012100: 6c65 2028 652e 672e 2c20 7669 6465 6f29  le (e.g., video)
+00012110: 2077 6974 6820 6175 6469 6f20 7472 6163   with audio trac
+00012120: 6b2e 0a20 2020 203a 7061 7261 6d20 4c69  k..    :param Li
+00012130: 7465 7261 6c5b 2776 6964 656f 272c 2027  teral['video', '
+00012140: 6175 6469 6f27 5d20 6175 6469 6f5f 7372  audio'] audio_sr
+00012150: 635f 7479 7065 3a20 5479 7065 206f 6620  c_type: Type of 
+00012160: 6175 6469 6f20 736f 7572 6365 206f 6620  audio source of 
+00012170: 2276 6964 656f 5f74 776f 5f70 6174 6822  "video_two_path"
+00012180: 2028 652e 672e 2c20 7669 6465 6f20 6f72   (e.g., video or
+00012190: 2061 7564 696f 2066 696c 6529 2e0a 0a20   audio file)... 
+000121a0: 2020 203a 6578 616d 706c 653a 0a20 2020     :example:.   
+000121b0: 203e 3e3e 2061 7070 656e 645f 6175 6469   >>> append_audi
+000121c0: 6f28 7669 6465 6f5f 7061 7468 3d27 2f55  o(video_path='/U
+000121d0: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+000121e0: 6f70 2f65 6e76 732f 7472 6f75 626c 6573  op/envs/troubles
+000121f0: 686f 6f74 696e 672f 7477 6f5f 626c 6163  hooting/two_blac
+00012200: 6b5f 616e 696d 616c 735f 3134 6270 2f70  k_animals_14bp/p
+00012210: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+00012220: 6465 6f73 2f6d 6572 6765 645f 7669 6465  deos/merged_vide
+00012230: 6f5f 3230 3233 3034 3235 3230 3136 3337  o_20230425201637
+00012240: 2e6d 7034 272c 0a20 2020 203e 3e3e 2061  .mp4',.    >>> a
+00012250: 7564 696f 5f70 6174 683d 222f 5573 6572  udio_path="/User
+00012260: 732f 7369 6d6f 6e2f 446f 6375 6d65 6e74  s/simon/Document
+00012270: 732f 5a6f 6f6d 2f64 6464 2f76 6964 656f  s/Zoom/ddd/video
+00012280: 3131 3830 3733 3232 3333 2e6d 7034 2229  1180732233.mp4")
+00012290: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
+000122a0: 206e 6f74 2063 6865 636b 5f66 666d 7065   not check_ffmpe
+000122b0: 675f 6176 6169 6c61 626c 6528 293a 0a20  g_available():. 
+000122c0: 2020 2020 2020 2072 6169 7365 2046 464d         raise FFM
+000122d0: 5045 474e 6f74 466f 756e 6445 7272 6f72  PEGNotFoundError
+000122e0: 280a 2020 2020 2020 2020 2020 2020 6d73  (.            ms
+000122f0: 673d 2246 464d 7065 6720 6e6f 7420 666f  g="FFMpeg not fo
+00012300: 756e 6420 6f6e 2063 6f6d 7075 7465 722e  und on computer.
+00012310: 2053 6565 2053 696d 4241 2064 6f63 7320   See SimBA docs 
+00012320: 666f 7220 696e 7374 616c 6c20 696e 7374  for install inst
+00012330: 7275 6374 696f 6e73 2e22 2c0a 2020 2020  ructions.",.    
+00012340: 2020 2020 2020 2020 736f 7572 6365 3d61          source=a
+00012350: 7070 656e 645f 6175 6469 6f2e 5f5f 6e61  ppend_audio.__na
+00012360: 6d65 5f5f 2c0a 2020 2020 2020 2020 290a  me__,.        ).
+00012370: 2020 2020 6368 6563 6b5f 6669 6c65 5f65      check_file_e
+00012380: 7869 7374 5f61 6e64 5f72 6561 6461 626c  xist_and_readabl
+00012390: 6528 6669 6c65 5f70 6174 683d 7669 6465  e(file_path=vide
+000123a0: 6f5f 7061 7468 290a 2020 2020 6368 6563  o_path).    chec
+000123b0: 6b5f 6669 6c65 5f65 7869 7374 5f61 6e64  k_file_exist_and
+000123c0: 5f72 6561 6461 626c 6528 6669 6c65 5f70  _readable(file_p
+000123d0: 6174 683d 6175 6469 6f5f 7061 7468 290a  ath=audio_path).
+000123e0: 2020 2020 7669 6465 6f5f 6d65 7461 5f64      video_meta_d
+000123f0: 6174 6120 3d20 6765 745f 7669 6465 6f5f  ata = get_video_
+00012400: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
+00012410: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
+00012420: 0a20 2020 2061 7564 696f 5f73 7263 5f6d  .    audio_src_m
+00012430: 6574 615f 6461 7461 203d 2067 6574 5f76  eta_data = get_v
+00012440: 6964 656f 5f6d 6574 615f 6461 7461 2876  ideo_meta_data(v
+00012450: 6964 656f 5f70 6174 683d 6175 6469 6f5f  ideo_path=audio_
+00012460: 7061 7468 290a 2020 2020 7361 7665 5f70  path).    save_p
+00012470: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00012480: 696e 280a 2020 2020 2020 2020 6f73 2e70  in(.        os.p
+00012490: 6174 682e 6469 726e 616d 6528 7669 6465  ath.dirname(vide
+000124a0: 6f5f 7061 7468 292c 2067 6574 5f66 6e5f  o_path), get_fn_
+000124b0: 6578 7428 6669 6c65 7061 7468 3d76 6964  ext(filepath=vid
+000124c0: 656f 5f70 6174 6829 5b31 5d20 2b20 225f  eo_path)[1] + "_
+000124d0: 775f 6175 6469 6f2e 6d70 3422 0a20 2020  w_audio.mp4".   
+000124e0: 2029 0a20 2020 2063 6d64 203d 205b 0a20   ).    cmd = [. 
+000124f0: 2020 2020 2020 2022 6666 7072 6f62 6522         "ffprobe"
+00012500: 2c0a 2020 2020 2020 2020 222d 7622 2c0a  ,.        "-v",.
+00012510: 2020 2020 2020 2020 2265 7272 6f72 222c          "error",
+00012520: 0a20 2020 2020 2020 2022 2d73 656c 6563  .        "-selec
+00012530: 745f 7374 7265 616d 7322 2c0a 2020 2020  t_streams",.    
+00012540: 2020 2020 2261 3a30 222c 0a20 2020 2020      "a:0",.     
+00012550: 2020 2022 2d73 686f 775f 656e 7472 6965     "-show_entrie
+00012560: 7322 2c0a 2020 2020 2020 2020 2273 7472  s",.        "str
+00012570: 6561 6d3d 636f 6465 635f 6e61 6d65 222c  eam=codec_name",
+00012580: 0a20 2020 2020 2020 2022 2d6f 6622 2c0a  .        "-of",.
+00012590: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+000125a0: 3d6e 6f70 7269 6e74 5f77 7261 7070 6572  =noprint_wrapper
+000125b0: 733d 313a 6e6f 6b65 793d 3122 2c0a 2020  s=1:nokey=1",.  
+000125c0: 2020 2020 2020 6175 6469 6f5f 7061 7468        audio_path
+000125d0: 2c0a 2020 2020 5d0a 2020 2020 7472 793a  ,.    ].    try:
+000125e0: 0a20 2020 2020 2020 2074 7261 636b 5f74  .        track_t
+000125f0: 7970 6520 3d20 280a 2020 2020 2020 2020  ype = (.        
+00012600: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+00012610: 6865 636b 5f6f 7574 7075 7428 636d 642c  heck_output(cmd,
+00012620: 2073 7464 6572 723d 7375 6270 726f 6365   stderr=subproce
+00012630: 7373 2e53 5444 4f55 5429 0a20 2020 2020  ss.STDOUT).     
+00012640: 2020 2020 2020 202e 6465 636f 6465 2822         .decode("
+00012650: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
+00012660: 2020 2020 2e73 7472 6970 2829 0a20 2020      .strip().   
+00012670: 2020 2020 2029 0a20 2020 2065 7863 6570       ).    excep
+00012680: 7420 7375 6270 726f 6365 7373 2e43 616c  t subprocess.Cal
+00012690: 6c65 6450 726f 6365 7373 4572 726f 723a  ledProcessError:
+000126a0: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
+000126b0: 6f44 6174 6145 7272 6f72 280a 2020 2020  oDataError(.    
+000126c0: 2020 2020 2020 2020 6d73 673d 6622 4e6f          msg=f"No
+000126d0: 2061 7564 696f 2074 7261 636b 2066 6f75   audio track fou
+000126e0: 6e64 2069 6e20 6669 6c65 207b 6175 6469  nd in file {audi
+000126f0: 6f5f 7061 7468 7d22 2c0a 2020 2020 2020  o_path}",.      
+00012700: 2020 2020 2020 736f 7572 6365 3d61 7070        source=app
+00012710: 656e 645f 6175 6469 6f2e 5f5f 6e61 6d65  end_audio.__name
+00012720: 5f5f 2c0a 2020 2020 2020 2020 290a 0a20  __,.        ).. 
+00012730: 2020 2069 6620 7669 6465 6f5f 6d65 7461     if video_meta
+00012740: 5f64 6174 615b 2266 7261 6d65 5f63 6f75  _data["frame_cou
+00012750: 6e74 225d 2021 3d20 6175 6469 6f5f 7372  nt"] != audio_sr
+00012760: 635f 6d65 7461 5f64 6174 615b 2266 7261  c_meta_data["fra
+00012770: 6d65 5f63 6f75 6e74 225d 3a0a 2020 2020  me_count"]:.    
+00012780: 2020 2020 496e 5661 6c69 6455 7365 7249      InValidUserI
+00012790: 6e70 7574 5761 726e 696e 6728 0a20 2020  nputWarning(.   
+000127a0: 2020 2020 2020 2020 206d 7367 3d66 2754           msg=f'T
+000127b0: 6865 2076 6964 656f 2028 7b76 6964 656f  he video ({video
+000127c0: 5f6d 6574 615f 6461 7461 5b22 6672 616d  _meta_data["fram
+000127d0: 655f 636f 756e 7422 5d7d 2920 616e 6420  e_count"]}) and 
+000127e0: 6175 6469 6f20 736f 7572 6365 2028 7b61  audio source ({a
+000127f0: 7564 696f 5f73 7263 5f6d 6574 615f 6461  udio_src_meta_da
+00012800: 7461 5b22 6672 616d 655f 636f 756e 7422  ta["frame_count"
+00012810: 5d7d 2920 646f 6573 206e 6f74 2068 6176  ]}) does not hav
+00012820: 6520 616e 2065 7175 616c 206e 756d 6265  e an equal numbe
+00012830: 7220 6f66 2066 7261 6d65 732e 272c 0a20  r of frames.',. 
+00012840: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+00012850: 653d 6170 7065 6e64 5f61 7564 696f 2e5f  e=append_audio._
+00012860: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
+00012870: 2029 0a0a 2020 2020 636d 6420 3d20 6627   )..    cmd = f'
+00012880: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
+00012890: 6f5f 7061 7468 7d22 202d 6920 227b 6175  o_path}" -i "{au
+000128a0: 6469 6f5f 7061 7468 7d22 202d 633a 7620  dio_path}" -c:v 
+000128b0: 636f 7079 202d 6d61 7020 303a 763a 3020  copy -map 0:v:0 
+000128c0: 2d6d 6170 2031 3a61 3a30 2022 7b73 6176  -map 1:a:0 "{sav
+000128d0: 655f 7061 7468 7d22 202d 7927 0a0a 2020  e_path}" -y'..  
+000128e0: 2020 7472 793a 0a20 2020 2020 2020 2073    try:.        s
+000128f0: 7562 7072 6f63 6573 732e 7275 6e28 636d  ubprocess.run(cm
+00012900: 642c 2073 6865 6c6c 3d54 7275 652c 2063  d, shell=True, c
+00012910: 6865 636b 3d54 7275 6529 0a20 2020 2065  heck=True).    e
+00012920: 7863 6570 7420 7375 6270 726f 6365 7373  xcept subprocess
+00012930: 2e43 616c 6c65 6450 726f 6365 7373 4572  .CalledProcessEr
+00012940: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
+00012950: 2020 7072 696e 7428 2245 7272 6f72 3a22    print("Error:"
+00012960: 2c20 6529 0a0a 2020 2020 7374 646f 7574  , e)..    stdout
+00012970: 5f73 7563 6365 7373 280a 2020 2020 2020  _success(.      
+00012980: 2020 6d73 673d 6622 4175 6469 6f20 6d65    msg=f"Audio me
+00012990: 7267 6564 2073 7563 6365 7373 6675 6c6c  rged successfull
+000129a0: 792c 2066 696c 6520 7361 7665 6420 6174  y, file saved at
+000129b0: 207b 7361 7665 5f70 6174 687d 2122 2c0a   {save_path}!",.
+000129c0: 2020 2020 2020 2020 736f 7572 6365 3d61          source=a
+000129d0: 7070 656e 645f 6175 6469 6f2e 5f5f 6e61  ppend_audio.__na
+000129e0: 6d65 5f5f 2c0a 2020 2020 290a 0a0a 6465  me__,.    )...de
+000129f0: 6620 6372 6f70 5f73 696e 676c 655f 7669  f crop_single_vi
+00012a00: 6465 6f5f 6369 7263 6c65 2866 696c 655f  deo_circle(file_
+00012a10: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00012a20: 206f 732e 5061 7468 4c69 6b65 5d29 202d   os.PathLike]) -
+00012a30: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
+00012a40: 2020 2020 4372 6f70 2061 2076 6964 656f      Crop a video
+00012a50: 2062 6173 6564 206f 6e20 6369 7263 756c   based on circul
+00012a60: 6172 2072 6567 696f 6e73 206f 6620 696e  ar regions of in
+00012a70: 7465 7265 7374 2028 524f 4973 2920 7365  terest (ROIs) se
+00012a80: 6c65 6374 6564 2062 7920 7468 6520 7573  lected by the us
+00012a90: 6572 2e0a 0a20 2020 203a 7061 7261 6d20  er...    :param 
+00012aa0: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00012ab0: 6174 684c 696b 655d 2066 696c 655f 7061  athLike] file_pa
+00012ac0: 7468 3a20 5468 6520 7061 7468 2074 6f20  th: The path to 
+00012ad0: 7468 6520 696e 7075 7420 7669 6465 6f20  the input video 
+00012ae0: 6669 6c65 2e0a 0a20 2020 202e 2e20 6e6f  file...    .. no
+00012af0: 7465 3a3a 0a20 2020 2020 2020 5468 6973  te::.       This
+00012b00: 2066 756e 6374 696f 6e20 6372 6f70 7320   function crops 
+00012b10: 7468 6520 696e 7075 7420 7669 6465 6f20  the input video 
+00012b20: 6261 7365 6420 6f6e 2063 6972 6375 6c61  based on circula
+00012b30: 7220 7265 6769 6f6e 7320 6f66 2069 6e74  r regions of int
+00012b40: 6572 6573 7420 2852 4f49 7329 2073 656c  erest (ROIs) sel
+00012b50: 6563 7465 6420 6279 2074 6865 2075 7365  ected by the use
+00012b60: 722e 0a20 2020 2020 2020 5468 6520 7573  r..       The us
+00012b70: 6572 2069 7320 7072 6f6d 7074 6564 2074  er is prompted t
+00012b80: 6f20 7365 6c65 6374 2061 2063 6972 6375  o select a circu
+00012b90: 6c61 7220 524f 4920 6f6e 2074 6865 2076  lar ROI on the v
+00012ba0: 6964 656f 2066 7261 6d65 2c20 616e 6420  ideo frame, and 
+00012bb0: 7468 6520 6675 6e63 7469 6f6e 2074 6865  the function the
+00012bc0: 6e20 6372 6f70 7320 7468 6520 7669 6465  n crops the vide
+00012bd0: 6f0a 2020 2020 2020 2062 6173 6564 206f  o.       based o
+00012be0: 6e20 7468 6520 7365 6c65 6374 6564 2052  n the selected R
+00012bf0: 4f49 2e20 5468 6520 6372 6f70 7065 6420  OI. The cropped 
+00012c00: 7669 6465 6f20 6973 2073 6176 6564 2077  video is saved w
+00012c10: 6974 6820 225f 6369 7263 6c65 5f63 726f  ith "_circle_cro
+00012c20: 7070 6564 2220 7375 6666 6978 2069 6e20  pped" suffix in 
+00012c30: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
+00012c40: 7279 0a20 2020 2020 2020 6173 2074 6865  ry.       as the
+00012c50: 2069 6e70 7574 2076 6964 656f 2066 696c   input video fil
+00012c60: 652e 0a0a 2020 2020 3a65 7861 6d70 6c65  e...    :example
+00012c70: 3a0a 2020 2020 3e3e 3e20 6372 6f70 5f73  :.    >>> crop_s
+00012c80: 696e 676c 655f 7669 6465 6f5f 6369 7263  ingle_video_circ
+00012c90: 6c65 2866 696c 655f 7061 7468 3d27 2f55  le(file_path='/U
+00012ca0: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+00012cb0: 6f70 2f41 4747 5245 5353 4956 4954 595f  op/AGGRESSIVITY_
+00012cc0: 345f 3131 5f32 315f 5472 6961 6c5f 325f  4_11_21_Trial_2_
+00012cd0: 6361 6d65 7261 315f 726f 7461 7465 645f  camera1_rotated_
+00012ce0: 3230 3234 3032 3131 3134 3333 3535 2e6d  20240211143355.m
+00012cf0: 7034 2729 0a20 2020 2022 2222 0a0a 2020  p4').    """..  
+00012d00: 2020 6469 722c 2076 6964 656f 5f6e 616d    dir, video_nam
+00012d10: 652c 205f 203d 2067 6574 5f66 6e5f 6578  e, _ = get_fn_ex
+00012d20: 7428 6669 6c65 7061 7468 3d66 696c 655f  t(filepath=file_
+00012d30: 7061 7468 290a 2020 2020 7361 7665 5f70  path).    save_p
+00012d40: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00012d50: 696e 2864 6972 2c20 6622 7b76 6964 656f  in(dir, f"{video
+00012d60: 5f6e 616d 657d 5f63 6972 636c 655f 6372  _name}_circle_cr
+00012d70: 6f70 7065 642e 6d70 3422 290a 2020 2020  opped.mp4").    
+00012d80: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
+00012d90: 3d20 6765 745f 7669 6465 6f5f 6d65 7461  = get_video_meta
+00012da0: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
+00012db0: 3d66 696c 655f 7061 7468 290a 2020 2020  =file_path).    
+00012dc0: 6368 6563 6b5f 6669 6c65 5f65 7869 7374  check_file_exist
+00012dd0: 5f61 6e64 5f72 6561 6461 626c 6528 6669  _and_readable(fi
+00012de0: 6c65 5f70 6174 683d 6669 6c65 5f70 6174  le_path=file_pat
+00012df0: 6829 0a20 2020 2063 6972 636c 655f 7365  h).    circle_se
+00012e00: 6c65 6374 6f72 203d 2052 4f49 5365 6c65  lector = ROISele
+00012e10: 6374 6f72 4369 7263 6c65 2870 6174 683d  ctorCircle(path=
+00012e20: 6669 6c65 5f70 6174 6829 0a20 2020 2063  file_path).    c
+00012e30: 6972 636c 655f 7365 6c65 6374 6f72 2e72  ircle_selector.r
+00012e40: 756e 2829 0a20 2020 2074 696d 6572 203d  un().    timer =
+00012e50: 2053 696d 6261 5469 6d65 7228 7374 6172   SimbaTimer(star
+00012e60: 743d 5472 7565 290a 2020 2020 7220 3d20  t=True).    r = 
+00012e70: 6369 7263 6c65 5f73 656c 6563 746f 722e  circle_selector.
+00012e80: 6369 7263 6c65 5f72 6164 6975 730a 2020  circle_radius.  
+00012e90: 2020 782c 2079 203d 2063 6972 636c 655f    x, y = circle_
+00012ea0: 7365 6c65 6374 6f72 2e63 6972 636c 655f  selector.circle_
+00012eb0: 6365 6e74 6572 5b30 5d2c 2063 6972 636c  center[0], circl
+00012ec0: 655f 7365 6c65 6374 6f72 2e63 6972 636c  e_selector.circl
+00012ed0: 655f 6365 6e74 6572 5b31 5d0a 2020 2020  e_center[1].    
+00012ee0: 706f 6c79 676f 6e20 3d20 506f 6c79 676f  polygon = Polygo
+00012ef0: 6e28 0a20 2020 2020 2020 205b 0a20 2020  n(.        [.   
+00012f00: 2020 2020 2020 2020 2028 7820 2b20 7220           (x + r 
+00012f10: 2a20 6e70 2e63 6f73 2861 6e67 6c65 292c  * np.cos(angle),
+00012f20: 2079 202b 2072 202a 206e 702e 7369 6e28   y + r * np.sin(
+00012f30: 616e 676c 6529 290a 2020 2020 2020 2020  angle)).        
+00012f40: 2020 2020 666f 7220 616e 676c 6520 696e      for angle in
+00012f50: 206e 702e 6c69 6e73 7061 6365 2830 2c20   np.linspace(0, 
+00012f60: 3220 2a20 6e70 2e70 692c 2031 3030 290a  2 * np.pi, 100).
+00012f70: 2020 2020 2020 2020 5d0a 2020 2020 290a          ].    ).
+00012f80: 2020 2020 706f 6c79 676f 6e73 203d 205b      polygons = [
+00012f90: 706f 6c79 676f 6e20 666f 7220 7820 696e  polygon for x in
+00012fa0: 2072 616e 6765 2876 6964 656f 5f6d 6574   range(video_met
+00012fb0: 615f 6461 7461 5b22 6672 616d 655f 636f  a_data["frame_co
+00012fc0: 756e 7422 5d29 5d0a 2020 2020 6966 2028  unt"])].    if (
+00012fd0: 706c 6174 666f 726d 2e73 7973 7465 6d28  platform.system(
+00012fe0: 2920 3d3d 2022 4461 7277 696e 2229 2061  ) == "Darwin") a
+00012ff0: 6e64 2028 6d75 6c74 6970 726f 6365 7373  nd (multiprocess
+00013000: 696e 672e 6765 745f 7374 6172 745f 6d65  ing.get_start_me
+00013010: 7468 6f64 2829 2069 7320 4e6f 6e65 293a  thod() is None):
+00013020: 0a20 2020 2020 2020 206d 756c 7469 7072  .        multipr
+00013030: 6f63 6573 7369 6e67 2e73 6574 5f73 7461  ocessing.set_sta
+00013040: 7274 5f6d 6574 686f 6428 2273 7061 776e  rt_method("spawn
+00013050: 222c 2066 6f72 6365 3d54 7275 6529 0a20  ", force=True). 
+00013060: 2020 2070 6f6c 7967 6f6e 7320 3d20 496d     polygons = Im
+00013070: 6167 654d 6978 696e 2829 2e73 6c69 6365  ageMixin().slice
+00013080: 5f73 6861 7065 735f 696e 5f69 6d67 7328  _shapes_in_imgs(
+00013090: 0a20 2020 2020 2020 2069 6d67 733d 6669  .        imgs=fi
+000130a0: 6c65 5f70 6174 682c 2073 6861 7065 733d  le_path, shapes=
+000130b0: 706f 6c79 676f 6e73 2c20 7665 7262 6f73  polygons, verbos
+000130c0: 653d 4661 6c73 650a 2020 2020 290a 2020  e=False.    ).  
+000130d0: 2020 7469 6d65 2e73 6c65 6570 2833 290a    time.sleep(3).
+000130e0: 2020 2020 5f20 3d20 496d 6167 654d 6978      _ = ImageMix
+000130f0: 696e 2e69 6d67 5f73 7461 636b 5f74 6f5f  in.img_stack_to_
+00013100: 7669 6465 6f28 0a20 2020 2020 2020 2069  video(.        i
+00013110: 6d67 733d 706f 6c79 676f 6e73 2c20 7361  mgs=polygons, sa
+00013120: 7665 5f70 6174 683d 7361 7665 5f70 6174  ve_path=save_pat
+00013130: 682c 2066 7073 3d76 6964 656f 5f6d 6574  h, fps=video_met
+00013140: 615f 6461 7461 5b22 6670 7322 5d0a 2020  a_data["fps"].  
+00013150: 2020 290a 2020 2020 7469 6d65 722e 7374    ).    timer.st
+00013160: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
+00013170: 7464 6f75 745f 7375 6363 6573 7328 0a20  tdout_success(. 
+00013180: 2020 2020 2020 206d 7367 3d66 2243 6972         msg=f"Cir
+00013190: 636c 652d 6261 7365 6420 6372 6f70 7065  cle-based croppe
+000131a0: 6420 7361 7665 6420 6174 2074 6f20 7b73  d saved at to {s
+000131b0: 6176 655f 7061 7468 7d22 2c0a 2020 2020  ave_path}",.    
+000131c0: 2020 2020 656c 6170 7365 645f 7469 6d65      elapsed_time
+000131d0: 3d74 696d 6572 2e65 6c61 7073 6564 5f74  =timer.elapsed_t
+000131e0: 696d 655f 7374 722c 0a20 2020 2029 0a0a  ime_str,.    )..
+000131f0: 0a64 6566 2063 726f 705f 6d75 6c74 6970  .def crop_multip
+00013200: 6c65 5f76 6964 656f 735f 6369 7263 6c65  le_videos_circle
+00013210: 7328 0a20 2020 2069 6e5f 6469 723a 2055  s(.    in_dir: U
+00013220: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00013230: 684c 696b 655d 2c20 6f75 745f 6469 723a  hLike], out_dir:
+00013240: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00013250: 6174 684c 696b 655d 0a29 202d 3e20 4e6f  athLike].) -> No
+00013260: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
+00013270: 4372 6f70 206d 756c 7469 706c 6520 7669  Crop multiple vi
+00013280: 6465 6f73 2062 6173 6564 206f 6e20 6369  deos based on ci
+00013290: 7263 756c 6172 2072 6567 696f 6e73 206f  rcular regions o
+000132a0: 6620 696e 7465 7265 7374 2028 524f 4973  f interest (ROIs
+000132b0: 2920 7365 6c65 6374 6564 2062 7920 7468  ) selected by th
+000132c0: 6520 7573 6572 2e0a 0a20 2020 203a 7061  e user...    :pa
+000132d0: 7261 6d20 2055 6e69 6f6e 5b73 7472 2c20  ram  Union[str, 
+000132e0: 6f73 2e50 6174 684c 696b 655d 2069 6e5f  os.PathLike] in_
+000132f0: 6469 723a 2054 6865 2064 6972 6563 746f  dir: The directo
+00013300: 7279 2063 6f6e 7461 696e 696e 6720 696e  ry containing in
+00013310: 7075 7420 7669 6465 6f20 6669 6c65 732e  put video files.
+00013320: 0a20 2020 203a 7061 7261 6d20 2055 6e69  .    :param  Uni
+00013330: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00013340: 696b 655d 206f 7574 5f64 6972 3a20 5468  ike] out_dir: Th
+00013350: 6520 6469 7265 6374 6f72 7920 746f 2073  e directory to s
+00013360: 6176 6520 7468 6520 6372 6f70 7065 6420  ave the cropped 
+00013370: 7669 6465 6f20 6669 6c65 732e 0a0a 2020  video files...  
+00013380: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+00013390: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000133a0: 2063 726f 7073 206d 756c 7469 706c 6520   crops multiple 
+000133b0: 7669 6465 6f73 2062 6173 6564 206f 6e20  videos based on 
+000133c0: 6369 7263 756c 6172 2052 4f49 7320 7365  circular ROIs se
+000133d0: 6c65 6374 6564 2062 7920 7468 6520 7573  lected by the us
+000133e0: 6572 2e0a 2020 2020 2020 2054 6865 2075  er..       The u
+000133f0: 7365 7220 6973 2061 736b 6564 2074 6f20  ser is asked to 
+00013400: 6465 6669 6e65 2061 2063 6972 636c 6520  define a circle 
+00013410: 6d61 6e75 616c 6c79 2069 6e20 6f6e 6520  manually in one 
+00013420: 7669 6465 6f20 7769 7468 696e 2074 6865  video within the
+00013430: 2069 6e70 7574 2064 6972 6563 746f 7279   input directory
+00013440: 2e0a 2020 2020 2020 2054 6865 2066 756e  ..       The fun
+00013450: 6374 696f 6e20 7468 656e 2063 726f 7073  ction then crops
+00013460: 2061 6c6c 2074 6865 2076 6964 656f 2069   all the video i
+00013470: 6e20 7468 6520 696e 7075 7420 6469 7265  n the input dire
+00013480: 6374 6f72 7920 6163 636f 7264 696e 6720  ctory according 
+00013490: 746f 2074 6865 2073 6861 7065 2064 6566  to the shape def
+000134a0: 696e 6564 0a20 2020 2020 2020 7573 696e  ined.       usin
+000134b0: 6720 7468 6520 6669 7273 7420 7669 6465  g the first vide
+000134c0: 6f20 616e 6420 7361 7665 7320 7468 6520  o and saves the 
+000134d0: 7669 6465 6f73 2069 6e20 7468 6520 6060  videos in the ``
+000134e0: 6f75 745f 6469 7260 6020 7769 7468 2074  out_dir`` with t
+000134f0: 6865 2073 616d 6520 6669 6c65 6e61 6d65  he same filename
+00013500: 7320 6173 2074 6865 206f 7269 6769 6e61  s as the origina
+00013510: 6c20 7669 6465 6f73 2e2e 0a0a 2020 2020  l videos....    
+00013520: 3a65 7861 6d70 6c65 3a0a 2020 2020 3e3e  :example:.    >>
+00013530: 3e20 6372 6f70 5f6d 756c 7469 706c 655f  > crop_multiple_
+00013540: 7669 6465 6f73 5f63 6972 636c 6573 2869  videos_circles(i
+00013550: 6e5f 6469 723d 272f 5573 6572 732f 7369  n_dir='/Users/si
+00013560: 6d6f 6e2f 4465 736b 746f 702f 6564 6974  mon/Desktop/edit
+00013570: 6564 2f74 6573 7473 272c 206f 7574 5f64  ed/tests', out_d
+00013580: 6972 3d27 2f55 7365 7273 2f73 696d 6f6e  ir='/Users/simon
+00013590: 2f44 6573 6b74 6f70 2729 0a20 2020 2022  /Desktop').    "
+000135a0: 2222 0a0a 2020 2020 6368 6563 6b5f 6966  ""..    check_if
+000135b0: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
+000135c0: 6972 3d69 6e5f 6469 7229 0a20 2020 2063  ir=in_dir).    c
+000135d0: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
+000135e0: 7473 2869 6e5f 6469 723d 6f75 745f 6469  ts(in_dir=out_di
+000135f0: 7229 0a20 2020 2076 6964 656f 5f66 696c  r).    video_fil
+00013600: 6573 203d 2066 696e 645f 616c 6c5f 7669  es = find_all_vi
+00013610: 6465 6f73 5f69 6e5f 6469 7265 6374 6f72  deos_in_director
+00013620: 7928 6469 7265 6374 6f72 793d 696e 5f64  y(directory=in_d
+00013630: 6972 290a 2020 2020 6369 7263 6c65 5f73  ir).    circle_s
+00013640: 656c 6563 746f 7220 3d20 524f 4953 656c  elector = ROISel
+00013650: 6563 746f 7243 6972 636c 6528 7061 7468  ectorCircle(path
+00013660: 3d6f 732e 7061 7468 2e6a 6f69 6e28 696e  =os.path.join(in
+00013670: 5f64 6972 2c20 7669 6465 6f5f 6669 6c65  _dir, video_file
+00013680: 735b 305d 2929 0a20 2020 2063 6972 636c  s[0])).    circl
+00013690: 655f 7365 6c65 6374 6f72 2e72 756e 2829  e_selector.run()
+000136a0: 0a20 2020 2072 203d 2063 6972 636c 655f  .    r = circle_
+000136b0: 7365 6c65 6374 6f72 2e63 6972 636c 655f  selector.circle_
+000136c0: 7261 6469 7573 0a20 2020 2078 2c20 7920  radius.    x, y 
+000136d0: 3d20 6369 7263 6c65 5f73 656c 6563 746f  = circle_selecto
+000136e0: 722e 6369 7263 6c65 5f63 656e 7465 725b  r.circle_center[
+000136f0: 305d 2c20 6369 7263 6c65 5f73 656c 6563  0], circle_selec
+00013700: 746f 722e 6369 7263 6c65 5f63 656e 7465  tor.circle_cente
+00013710: 725b 315d 0a20 2020 2070 6f6c 7967 6f6e  r[1].    polygon
+00013720: 203d 2050 6f6c 7967 6f6e 280a 2020 2020   = Polygon(.    
+00013730: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00013740: 2020 2878 202b 2072 202a 206e 702e 636f    (x + r * np.co
+00013750: 7328 616e 676c 6529 2c20 7920 2b20 7220  s(angle), y + r 
+00013760: 2a20 6e70 2e73 696e 2861 6e67 6c65 2929  * np.sin(angle))
+00013770: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013780: 2061 6e67 6c65 2069 6e20 6e70 2e6c 696e   angle in np.lin
+00013790: 7370 6163 6528 302c 2032 202a 206e 702e  space(0, 2 * np.
+000137a0: 7069 2c20 3130 3029 0a20 2020 2020 2020  pi, 100).       
+000137b0: 205d 0a20 2020 2029 0a20 2020 2074 696d   ].    ).    tim
+000137c0: 6572 203d 2053 696d 6261 5469 6d65 7228  er = SimbaTimer(
+000137d0: 7374 6172 743d 5472 7565 290a 2020 2020  start=True).    
+000137e0: 6966 2028 706c 6174 666f 726d 2e73 7973  if (platform.sys
+000137f0: 7465 6d28 2920 3d3d 2022 4461 7277 696e  tem() == "Darwin
+00013800: 2229 2061 6e64 2028 6d75 6c74 6970 726f  ") and (multipro
+00013810: 6365 7373 696e 672e 6765 745f 7374 6172  cessing.get_star
+00013820: 745f 6d65 7468 6f64 2829 2069 7320 4e6f  t_method() is No
+00013830: 6e65 293a 0a20 2020 2020 2020 206d 756c  ne):.        mul
+00013840: 7469 7072 6f63 6573 7369 6e67 2e73 6574  tiprocessing.set
+00013850: 5f73 7461 7274 5f6d 6574 686f 6428 2273  _start_method("s
+00013860: 7061 776e 222c 2066 6f72 6365 3d46 616c  pawn", force=Fal
+00013870: 7365 290a 2020 2020 666f 7220 7669 6465  se).    for vide
+00013880: 6f5f 636e 742c 2076 6964 656f 5f70 6174  o_cnt, video_pat
+00013890: 6820 696e 2065 6e75 6d65 7261 7465 2876  h in enumerate(v
+000138a0: 6964 656f 5f66 696c 6573 293a 0a20 2020  ideo_files):.   
+000138b0: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
+000138c0: 2020 2020 2020 2020 6622 4369 7263 6c65          f"Circle
+000138d0: 2063 726f 7070 696e 6720 7669 6465 6f20   cropping video 
+000138e0: 7b76 6964 656f 5f70 6174 687d 2028 7b76  {video_path} ({v
+000138f0: 6964 656f 5f63 6e74 2b31 7d2f 7b6c 656e  ideo_cnt+1}/{len
+00013900: 2876 6964 656f 5f66 696c 6573 297d 292e  (video_files)}).
+00013910: 2e2e 220a 2020 2020 2020 2020 290a 2020  ..".        ).  
+00013920: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
+00013930: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00013940: 696e 5f64 6972 2c20 7669 6465 6f5f 7061  in_dir, video_pa
+00013950: 7468 290a 2020 2020 2020 2020 5f2c 2076  th).        _, v
+00013960: 6964 656f 5f6e 616d 652c 205f 203d 2067  ideo_name, _ = g
+00013970: 6574 5f66 6e5f 6578 7428 6669 6c65 7061  et_fn_ext(filepa
+00013980: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+00013990: 2020 2020 2020 2073 6176 655f 7061 7468         save_path
+000139a0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000139b0: 6f75 745f 6469 722c 2066 227b 7669 6465  out_dir, f"{vide
+000139c0: 6f5f 6e61 6d65 7d2e 6d70 3422 290a 2020  o_name}.mp4").  
+000139d0: 2020 2020 2020 7669 6465 6f5f 6d65 7461        video_meta
+000139e0: 5f64 6174 6120 3d20 6765 745f 7669 6465  _data = get_vide
+000139f0: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
+00013a00: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
+00013a10: 6829 0a20 2020 2020 2020 2070 6f6c 7967  h).        polyg
+00013a20: 6f6e 7320 3d20 5b70 6f6c 7967 6f6e 2066  ons = [polygon f
+00013a30: 6f72 2078 2069 6e20 7261 6e67 6528 7669  or x in range(vi
+00013a40: 6465 6f5f 6d65 7461 5f64 6174 615b 2266  deo_meta_data["f
+00013a50: 7261 6d65 5f63 6f75 6e74 225d 295d 0a20  rame_count"])]. 
+00013a60: 2020 2020 2020 2070 6f6c 7967 6f6e 7320         polygons 
+00013a70: 3d20 496d 6167 654d 6978 696e 2829 2e73  = ImageMixin().s
+00013a80: 6c69 6365 5f73 6861 7065 735f 696e 5f69  lice_shapes_in_i
+00013a90: 6d67 7328 0a20 2020 2020 2020 2020 2020  mgs(.           
+00013aa0: 2069 6d67 733d 7669 6465 6f5f 7061 7468   imgs=video_path
+00013ab0: 2c20 7368 6170 6573 3d70 6f6c 7967 6f6e  , shapes=polygon
+00013ac0: 732c 2076 6572 626f 7365 3d46 616c 7365  s, verbose=False
+00013ad0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00013ae0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+00013af0: 0a20 2020 2020 2020 205f 203d 2049 6d61  .        _ = Ima
+00013b00: 6765 4d69 7869 6e2e 696d 675f 7374 6163  geMixin.img_stac
+00013b10: 6b5f 746f 5f76 6964 656f 280a 2020 2020  k_to_video(.    
+00013b20: 2020 2020 2020 2020 696d 6773 3d70 6f6c          imgs=pol
+00013b30: 7967 6f6e 732c 2073 6176 655f 7061 7468  ygons, save_path
+00013b40: 3d73 6176 655f 7061 7468 2c20 6670 733d  =save_path, fps=
+00013b50: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+00013b60: 2266 7073 225d 0a20 2020 2020 2020 2029  "fps"].        )
+00013b70: 0a20 2020 2074 696d 6572 2e73 746f 705f  .    timer.stop_
+00013b80: 7469 6d65 7228 290a 2020 2020 7374 646f  timer().    stdo
+00013b90: 7574 5f73 7563 6365 7373 280a 2020 2020  ut_success(.    
+00013ba0: 2020 2020 6d73 673d 6622 4369 7263 6c65      msg=f"Circle
+00013bb0: 2d62 6173 6564 2063 726f 7070 6564 207b  -based cropped {
+00013bc0: 6c65 6e28 7669 6465 6f5f 6669 6c65 7329  len(video_files)
+00013bd0: 7d20 6669 6c65 7320 746f 2064 6972 6563  } files to direc
+00013be0: 746f 7279 207b 6f75 745f 6469 727d 222c  tory {out_dir}",
+00013bf0: 0a20 2020 2020 2020 2065 6c61 7073 6564  .        elapsed
+00013c00: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
+00013c10: 7365 645f 7469 6d65 5f73 7472 2c0a 2020  sed_time_str,.  
+00013c20: 2020 290a 0a0a 6465 6620 6372 6f70 5f73    )...def crop_s
+00013c30: 696e 676c 655f 7669 6465 6f5f 706f 6c79  ingle_video_poly
+00013c40: 676f 6e28 6669 6c65 5f70 6174 683a 2055  gon(file_path: U
+00013c50: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00013c60: 684c 696b 655d 2920 2d3e 204e 6f6e 653a  hLike]) -> None:
+00013c70: 0a20 2020 2022 2222 0a20 2020 2043 726f  .    """.    Cro
+00013c80: 7020 6120 7669 6465 6f20 6261 7365 6420  p a video based 
+00013c90: 6f6e 2070 6f6c 7967 6f6e 616c 2072 6567  on polygonal reg
+00013ca0: 696f 6e73 206f 6620 696e 7465 7265 7374  ions of interest
+00013cb0: 2028 524f 4973 2920 7365 6c65 6374 6564   (ROIs) selected
+00013cc0: 2062 7920 7468 6520 7573 6572 2e0a 0a20   by the user... 
+00013cd0: 2020 203a 7061 7261 6d20 2055 6e69 6f6e     :param  Union
+00013ce0: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+00013cf0: 655d 2066 696c 655f 7061 7468 3a20 5468  e] file_path: Th
+00013d00: 6520 7061 7468 2074 6f20 7468 6520 696e  e path to the in
+00013d10: 7075 7420 7669 6465 6f20 6669 6c65 2e0a  put video file..
+00013d20: 0a20 2020 202e 2e20 6e6f 7465 3a3a 0a20  .    .. note::. 
+00013d30: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+00013d40: 696f 6e20 6372 6f70 7320 7468 6520 696e  ion crops the in
+00013d50: 7075 7420 7669 6465 6f20 6261 7365 6420  put video based 
+00013d60: 6f6e 2070 6f6c 7967 6f6e 616c 2072 6567  on polygonal reg
+00013d70: 696f 6e73 206f 6620 696e 7465 7265 7374  ions of interest
+00013d80: 2028 524f 4973 2920 7365 6c65 6374 6564   (ROIs) selected
+00013d90: 2062 7920 7468 6520 7573 6572 2e0a 2020   by the user..  
+00013da0: 2020 2020 2054 6865 2075 7365 7220 6973       The user is
+00013db0: 2070 726f 6d70 7465 6420 746f 2073 656c   prompted to sel
+00013dc0: 6563 7420 6120 706f 6c79 676f 6e61 6c20  ect a polygonal 
+00013dd0: 524f 4920 6f6e 2074 6865 2076 6964 656f  ROI on the video
+00013de0: 2066 7261 6d65 2c20 616e 6420 7468 6520   frame, and the 
+00013df0: 6675 6e63 7469 6f6e 2074 6865 6e20 6372  function then cr
+00013e00: 6f70 7320 7468 6520 7669 6465 6f0a 2020  ops the video.  
+00013e10: 2020 2020 2062 6173 6564 206f 6e20 7468       based on th
+00013e20: 6520 7365 6c65 6374 6564 2052 4f49 2e20  e selected ROI. 
+00013e30: 5468 6520 6372 6f70 7065 6420 7669 6465  The cropped vide
+00013e40: 6f20 6973 2073 6176 6564 2077 6974 6820  o is saved with 
+00013e50: 225f 706f 6c79 676f 6e5f 6372 6f70 7065  "_polygon_croppe
+00013e60: 6422 2073 7566 6669 7820 696e 2074 6865  d" suffix in the
+00013e70: 2073 616d 6520 6469 7265 6374 6f72 790a   same directory.
+00013e80: 2020 2020 2020 2061 7320 7468 6520 696e         as the in
+00013e90: 7075 7420 7669 6465 6f20 6669 6c65 2e0a  put video file..
+00013ea0: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+00013eb0: 2020 203e 3e3e 2063 726f 705f 7369 6e67     >>> crop_sing
+00013ec0: 6c65 5f76 6964 656f 5f70 6f6c 7967 6f6e  le_video_polygon
+00013ed0: 2866 696c 655f 7061 7468 3d27 2f55 7365  (file_path='/Use
+00013ee0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+00013ef0: 2f41 4747 5245 5353 4956 4954 595f 345f  /AGGRESSIVITY_4_
+00013f00: 3131 5f32 315f 5472 6961 6c5f 325f 6361  11_21_Trial_2_ca
+00013f10: 6d65 7261 315f 726f 7461 7465 645f 3230  mera1_rotated_20
+00013f20: 3234 3032 3131 3134 3333 3535 2e6d 7034  240211143355.mp4
+00013f30: 2729 0a20 2020 2022 2222 0a0a 2020 2020  ').    """..    
+00013f40: 6469 722c 2076 6964 656f 5f6e 616d 652c  dir, video_name,
+00013f50: 205f 203d 2067 6574 5f66 6e5f 6578 7428   _ = get_fn_ext(
+00013f60: 6669 6c65 7061 7468 3d66 696c 655f 7061  filepath=file_pa
+00013f70: 7468 290a 2020 2020 7361 7665 5f70 6174  th).    save_pat
+00013f80: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+00013f90: 2864 6972 2c20 6622 7b76 6964 656f 5f6e  (dir, f"{video_n
+00013fa0: 616d 657d 5f70 6f6c 7967 6f6e 5f63 726f  ame}_polygon_cro
+00013fb0: 7070 6564 2e6d 7034 2229 0a20 2020 2076  pped.mp4").    v
+00013fc0: 6964 656f 5f6d 6574 615f 6461 7461 203d  ideo_meta_data =
+00013fd0: 2067 6574 5f76 6964 656f 5f6d 6574 615f   get_video_meta_
+00013fe0: 6461 7461 2876 6964 656f 5f70 6174 683d  data(video_path=
+00013ff0: 6669 6c65 5f70 6174 6829 0a20 2020 2063  file_path).    c
+00014000: 6865 636b 5f66 696c 655f 6578 6973 745f  heck_file_exist_
+00014010: 616e 645f 7265 6164 6162 6c65 2866 696c  and_readable(fil
+00014020: 655f 7061 7468 3d66 696c 655f 7061 7468  e_path=file_path
+00014030: 290a 2020 2020 706f 6c79 676f 6e5f 7365  ).    polygon_se
+00014040: 6c65 6374 6f72 203d 2052 4f49 5365 6c65  lector = ROISele
+00014050: 6374 6f72 506f 6c79 676f 6e28 7061 7468  ctorPolygon(path
+00014060: 3d66 696c 655f 7061 7468 290a 2020 2020  =file_path).    
+00014070: 706f 6c79 676f 6e5f 7365 6c65 6374 6f72  polygon_selector
+00014080: 2e72 756e 2829 0a20 2020 2074 696d 6572  .run().    timer
+00014090: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
+000140a0: 6172 743d 5472 7565 290a 2020 2020 7665  art=True).    ve
+000140b0: 7274 6963 6573 203d 2070 6f6c 7967 6f6e  rtices = polygon
+000140c0: 5f73 656c 6563 746f 722e 706f 6c79 676f  _selector.polygo
+000140d0: 6e5f 7665 7274 6963 6573 0a20 2020 2070  n_vertices.    p
+000140e0: 6f6c 7967 6f6e 203d 2050 6f6c 7967 6f6e  olygon = Polygon
+000140f0: 2876 6572 7469 6365 7329 0a20 2020 2070  (vertices).    p
+00014100: 6f6c 7967 6f6e 7320 3d20 5b70 6f6c 7967  olygons = [polyg
+00014110: 6f6e 2066 6f72 2078 2069 6e20 7261 6e67  on for x in rang
+00014120: 6528 7669 6465 6f5f 6d65 7461 5f64 6174  e(video_meta_dat
+00014130: 615b 2266 7261 6d65 5f63 6f75 6e74 225d  a["frame_count"]
+00014140: 295d 0a20 2020 2069 6620 2870 6c61 7466  )].    if (platf
+00014150: 6f72 6d2e 7379 7374 656d 2829 203d 3d20  orm.system() == 
+00014160: 2244 6172 7769 6e22 2920 616e 6420 286d  "Darwin") and (m
+00014170: 756c 7469 7072 6f63 6573 7369 6e67 2e67  ultiprocessing.g
+00014180: 6574 5f73 7461 7274 5f6d 6574 686f 6428  et_start_method(
+00014190: 2920 6973 204e 6f6e 6529 3a0a 2020 2020  ) is None):.    
+000141a0: 2020 2020 6d75 6c74 6970 726f 6365 7373      multiprocess
+000141b0: 696e 672e 7365 745f 7374 6172 745f 6d65  ing.set_start_me
+000141c0: 7468 6f64 2822 7370 6177 6e22 2c20 666f  thod("spawn", fo
+000141d0: 7263 653d 4661 6c73 6529 0a20 2020 2070  rce=False).    p
+000141e0: 6f6c 7967 6f6e 7320 3d20 496d 6167 654d  olygons = ImageM
+000141f0: 6978 696e 2829 2e73 6c69 6365 5f73 6861  ixin().slice_sha
+00014200: 7065 735f 696e 5f69 6d67 7328 0a20 2020  pes_in_imgs(.   
+00014210: 2020 2020 2069 6d67 733d 6669 6c65 5f70       imgs=file_p
+00014220: 6174 682c 2073 6861 7065 733d 706f 6c79  ath, shapes=poly
+00014230: 676f 6e73 2c20 7665 7262 6f73 653d 5472  gons, verbose=Tr
+00014240: 7565 0a20 2020 2029 0a20 2020 205f 203d  ue.    ).    _ =
+00014250: 2049 6d61 6765 4d69 7869 6e2e 696d 675f   ImageMixin.img_
+00014260: 7374 6163 6b5f 746f 5f76 6964 656f 280a  stack_to_video(.
+00014270: 2020 2020 2020 2020 696d 6773 3d70 6f6c          imgs=pol
+00014280: 7967 6f6e 732c 2073 6176 655f 7061 7468  ygons, save_path
+00014290: 3d73 6176 655f 7061 7468 2c20 6670 733d  =save_path, fps=
+000142a0: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+000142b0: 2266 7073 225d 0a20 2020 2029 0a20 2020  "fps"].    ).   
+000142c0: 2074 696d 6572 2e73 746f 705f 7469 6d65   timer.stop_time
+000142d0: 7228 290a 2020 2020 7374 646f 7574 5f73  r().    stdout_s
+000142e0: 7563 6365 7373 280a 2020 2020 2020 2020  uccess(.        
+000142f0: 6d73 673d 6622 506f 6c79 676f 6e2d 6261  msg=f"Polygon-ba
+00014300: 7365 6420 6372 6f70 7065 6420 7361 7665  sed cropped save
+00014310: 6420 6174 2074 6f20 7b73 6176 655f 7061  d at to {save_pa
+00014320: 7468 7d22 2c0a 2020 2020 2020 2020 656c  th}",.        el
+00014330: 6170 7365 645f 7469 6d65 3d74 696d 6572  apsed_time=timer
+00014340: 2e65 6c61 7073 6564 5f74 696d 655f 7374  .elapsed_time_st
+00014350: 722c 0a20 2020 2029 0a0a 0a64 6566 2063  r,.    )...def c
+00014360: 726f 705f 6d75 6c74 6970 6c65 5f76 6964  rop_multiple_vid
+00014370: 656f 735f 706f 6c79 676f 6e73 280a 2020  eos_polygons(.  
+00014380: 2020 696e 5f64 6972 3a20 556e 696f 6e5b    in_dir: Union[
+00014390: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+000143a0: 5d2c 206f 7574 5f64 6972 3a20 556e 696f  ], out_dir: Unio
+000143b0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+000143c0: 6b65 5d0a 2920 2d3e 204e 6f6e 653a 0a20  ke].) -> None:. 
+000143d0: 2020 2022 2222 0a20 2020 2043 726f 7020     """.    Crop 
+000143e0: 6d75 6c74 6970 6c65 2076 6964 656f 7320  multiple videos 
+000143f0: 6261 7365 6420 6f6e 2070 6f6c 7967 6f6e  based on polygon
+00014400: 616c 2072 6567 696f 6e73 206f 6620 696e  al regions of in
+00014410: 7465 7265 7374 2028 524f 4973 2920 7365  terest (ROIs) se
+00014420: 6c65 6374 6564 2062 7920 7468 6520 7573  lected by the us
+00014430: 6572 2e0a 0a20 2020 203a 7061 7261 6d20  er...    :param 
+00014440: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00014450: 6174 684c 696b 655d 2069 6e5f 6469 723a  athLike] in_dir:
+00014460: 2054 6865 2064 6972 6563 746f 7279 2063   The directory c
+00014470: 6f6e 7461 696e 696e 6720 696e 7075 7420  ontaining input 
+00014480: 7669 6465 6f20 6669 6c65 732e 0a20 2020  video files..   
+00014490: 203a 7061 7261 6d20 2055 6e69 6f6e 5b73   :param  Union[s
+000144a0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+000144b0: 206f 7574 5f64 6972 3a20 5468 6520 6469   out_dir: The di
+000144c0: 7265 6374 6f72 7920 746f 2073 6176 6520  rectory to save 
+000144d0: 7468 6520 6372 6f70 7065 6420 7669 6465  the cropped vide
+000144e0: 6f20 6669 6c65 732e 0a0a 2020 2020 2e2e  o files...    ..
+000144f0: 206e 6f74 653a 3a0a 2020 2020 2020 2054   note::.       T
+00014500: 6869 7320 6675 6e63 7469 6f6e 2063 726f  his function cro
+00014510: 7073 206d 756c 7469 706c 6520 7669 6465  ps multiple vide
+00014520: 6f73 2062 6173 6564 206f 6e20 706f 6c79  os based on poly
+00014530: 676f 6e61 6c20 524f 4973 2073 656c 6563  gonal ROIs selec
+00014540: 7465 6420 6279 2074 6865 2075 7365 722e  ted by the user.
+00014550: 0a20 2020 2020 2020 5468 6520 7573 6572  .       The user
+00014560: 2069 7320 6173 6b65 6420 746f 2064 6566   is asked to def
+00014570: 696e 6520 6120 706f 6c79 676f 6e20 6d61  ine a polygon ma
+00014580: 6e75 616c 6c79 2069 6e20 6f6e 6520 7669  nually in one vi
+00014590: 6465 6f20 7769 7468 696e 2074 6865 2069  deo within the i
+000145a0: 6e70 7574 2064 6972 6563 746f 7279 2e0a  nput directory..
+000145b0: 2020 2020 2020 2054 6865 2066 756e 6374         The funct
+000145c0: 696f 6e20 7468 656e 2063 726f 7073 2061  ion then crops a
+000145d0: 6c6c 2074 6865 2076 6964 656f 2069 6e20  ll the video in 
+000145e0: 7468 6520 696e 7075 7420 6469 7265 6374  the input direct
+000145f0: 6f72 7920 6163 636f 7264 696e 6720 746f  ory according to
+00014600: 2074 6865 2073 6861 7065 2064 6566 696e   the shape defin
+00014610: 6564 0a20 2020 2020 2020 7573 696e 6720  ed.       using 
+00014620: 7468 6520 6669 7273 7420 7669 6465 6f20  the first video 
+00014630: 616e 6420 7361 7665 7320 7468 6520 7669  and saves the vi
+00014640: 6465 6f73 2069 6e20 7468 6520 6060 6f75  deos in the ``ou
+00014650: 745f 6469 7260 6020 7769 7468 2074 6865  t_dir`` with the
+00014660: 2073 616d 6520 6669 6c65 6e61 6d65 7320   same filenames 
+00014670: 6173 2074 6865 206f 7269 6769 6e61 6c20  as the original 
+00014680: 7669 6465 6f73 2e2e 0a0a 2020 2020 3a65  videos....    :e
+00014690: 7861 6d70 6c65 3a0a 2020 2020 3e3e 3e20  xample:.    >>> 
+000146a0: 6372 6f70 5f6d 756c 7469 706c 655f 7669  crop_multiple_vi
+000146b0: 6465 6f73 5f70 6f6c 7967 6f6e 7328 696e  deos_polygons(in
+000146c0: 5f64 6972 3d27 2f55 7365 7273 2f73 696d  _dir='/Users/sim
+000146d0: 6f6e 2f44 6573 6b74 6f70 2f65 6469 7465  on/Desktop/edite
+000146e0: 642f 7465 7374 7327 2c20 6f75 745f 6469  d/tests', out_di
+000146f0: 723d 272f 5573 6572 732f 7369 6d6f 6e2f  r='/Users/simon/
+00014700: 4465 736b 746f 7027 290a 2020 2020 2222  Desktop').    ""
+00014710: 220a 0a20 2020 2063 6865 636b 5f69 665f  "..    check_if_
+00014720: 6469 725f 6578 6973 7473 2869 6e5f 6469  dir_exists(in_di
+00014730: 723d 696e 5f64 6972 290a 2020 2020 6368  r=in_dir).    ch
+00014740: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
+00014750: 7328 696e 5f64 6972 3d6f 7574 5f64 6972  s(in_dir=out_dir
+00014760: 290a 2020 2020 7669 6465 6f5f 6669 6c65  ).    video_file
+00014770: 7320 3d20 6669 6e64 5f61 6c6c 5f76 6964  s = find_all_vid
+00014780: 656f 735f 696e 5f64 6972 6563 746f 7279  eos_in_directory
+00014790: 2864 6972 6563 746f 7279 3d69 6e5f 6469  (directory=in_di
+000147a0: 7229 0a20 2020 2070 6f6c 7967 6f6e 5f73  r).    polygon_s
+000147b0: 656c 6563 746f 7220 3d20 524f 4953 656c  elector = ROISel
+000147c0: 6563 746f 7250 6f6c 7967 6f6e 2870 6174  ectorPolygon(pat
+000147d0: 683d 6f73 2e70 6174 682e 6a6f 696e 2869  h=os.path.join(i
+000147e0: 6e5f 6469 722c 2076 6964 656f 5f66 696c  n_dir, video_fil
+000147f0: 6573 5b30 5d29 290a 2020 2020 706f 6c79  es[0])).    poly
+00014800: 676f 6e5f 7365 6c65 6374 6f72 2e72 756e  gon_selector.run
+00014810: 2829 0a20 2020 2076 6572 7469 6365 7320  ().    vertices 
+00014820: 3d20 706f 6c79 676f 6e5f 7365 6c65 6374  = polygon_select
+00014830: 6f72 2e70 6f6c 7967 6f6e 5f76 6572 7469  or.polygon_verti
+00014840: 6365 730a 2020 2020 706f 6c79 676f 6e20  ces.    polygon 
+00014850: 3d20 506f 6c79 676f 6e28 7665 7274 6963  = Polygon(vertic
+00014860: 6573 290a 2020 2020 7469 6d65 7220 3d20  es).    timer = 
+00014870: 5369 6d62 6154 696d 6572 2873 7461 7274  SimbaTimer(start
+00014880: 3d54 7275 6529 0a20 2020 2066 6f72 2076  =True).    for v
+00014890: 6964 656f 5f63 6e74 2c20 7669 6465 6f5f  ideo_cnt, video_
+000148a0: 7061 7468 2069 6e20 656e 756d 6572 6174  path in enumerat
+000148b0: 6528 7669 6465 6f5f 6669 6c65 7329 3a0a  e(video_files):.
+000148c0: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+000148d0: 2020 2020 2020 2020 2020 2066 2250 6f6c             f"Pol
+000148e0: 7967 6f6e 2063 726f 7070 696e 6720 7669  ygon cropping vi
+000148f0: 6465 6f20 7b76 6964 656f 5f70 6174 687d  deo {video_path}
+00014900: 2028 7b76 6964 656f 5f63 6e74 2b31 7d2f   ({video_cnt+1}/
+00014910: 7b6c 656e 2876 6964 656f 5f66 696c 6573  {len(video_files
+00014920: 297d 292e 2e2e 220a 2020 2020 2020 2020  )})...".        
+00014930: 290a 2020 2020 2020 2020 7669 6465 6f5f  ).        video_
+00014940: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00014950: 6f69 6e28 696e 5f64 6972 2c20 7669 6465  oin(in_dir, vide
+00014960: 6f5f 7061 7468 290a 2020 2020 2020 2020  o_path).        
+00014970: 5f2c 2076 6964 656f 5f6e 616d 652c 205f  _, video_name, _
+00014980: 203d 2067 6574 5f66 6e5f 6578 7428 6669   = get_fn_ext(fi
+00014990: 6c65 7061 7468 3d76 6964 656f 5f70 6174  lepath=video_pat
+000149a0: 6829 0a20 2020 2020 2020 2073 6176 655f  h).        save_
+000149b0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+000149c0: 6f69 6e28 6f75 745f 6469 722c 2066 227b  oin(out_dir, f"{
+000149d0: 7669 6465 6f5f 6e61 6d65 7d2e 6d70 3422  video_name}.mp4"
+000149e0: 290a 2020 2020 2020 2020 7669 6465 6f5f  ).        video_
+000149f0: 6d65 7461 5f64 6174 6120 3d20 6765 745f  meta_data = get_
+00014a00: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
+00014a10: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
+00014a20: 5f70 6174 6829 0a20 2020 2020 2020 2070  _path).        p
+00014a30: 6f6c 7967 6f6e 7320 3d20 5b70 6f6c 7967  olygons = [polyg
+00014a40: 6f6e 2066 6f72 2078 2069 6e20 7261 6e67  on for x in rang
+00014a50: 6528 7669 6465 6f5f 6d65 7461 5f64 6174  e(video_meta_dat
+00014a60: 615b 2266 7261 6d65 5f63 6f75 6e74 225d  a["frame_count"]
+00014a70: 295d 0a20 2020 2020 2020 2070 6f6c 7967  )].        polyg
+00014a80: 6f6e 7320 3d20 496d 6167 654d 6978 696e  ons = ImageMixin
+00014a90: 2829 2e73 6c69 6365 5f73 6861 7065 735f  ().slice_shapes_
+00014aa0: 696e 5f69 6d67 7328 0a20 2020 2020 2020  in_imgs(.       
+00014ab0: 2020 2020 2069 6d67 733d 7669 6465 6f5f       imgs=video_
+00014ac0: 7061 7468 2c20 7368 6170 6573 3d70 6f6c  path, shapes=pol
+00014ad0: 7967 6f6e 732c 2076 6572 626f 7365 3d46  ygons, verbose=F
+00014ae0: 616c 7365 0a20 2020 2020 2020 2029 0a20  alse.        ). 
+00014af0: 2020 2020 2020 205f 203d 2049 6d61 6765         _ = Image
+00014b00: 4d69 7869 6e2e 696d 675f 7374 6163 6b5f  Mixin.img_stack_
+00014b10: 746f 5f76 6964 656f 280a 2020 2020 2020  to_video(.      
+00014b20: 2020 2020 2020 696d 6773 3d70 6f6c 7967        imgs=polyg
+00014b30: 6f6e 732c 2073 6176 655f 7061 7468 3d73  ons, save_path=s
+00014b40: 6176 655f 7061 7468 2c20 6670 733d 7669  ave_path, fps=vi
+00014b50: 6465 6f5f 6d65 7461 5f64 6174 615b 2266  deo_meta_data["f
+00014b60: 7073 225d 0a20 2020 2020 2020 2029 0a20  ps"].        ). 
+00014b70: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
+00014b80: 6d65 7228 290a 2020 2020 7374 646f 7574  mer().    stdout
+00014b90: 5f73 7563 6365 7373 280a 2020 2020 2020  _success(.      
+00014ba0: 2020 6d73 673d 6622 506f 6c79 676f 6e2d    msg=f"Polygon-
+00014bb0: 6261 7365 6420 6372 6f70 7065 6420 7b6c  based cropped {l
+00014bc0: 656e 2876 6964 656f 5f66 696c 6573 297d  en(video_files)}
+00014bd0: 2066 696c 6573 2074 6f20 6469 7265 6374   files to direct
+00014be0: 6f72 7920 7b6f 7574 5f64 6972 7d22 2c0a  ory {out_dir}",.
+00014bf0: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
+00014c00: 7469 6d65 3d74 696d 6572 2e65 6c61 7073  time=timer.elaps
+00014c10: 6564 5f74 696d 655f 7374 722c 0a20 2020  ed_time_str,.   
+00014c20: 2029 0a0a 0a64 6566 2072 6573 697a 655f   )...def resize_
+00014c30: 7669 6465 6f73 5f62 795f 6865 6967 6874  videos_by_height
+00014c40: 280a 2020 2020 7669 6465 6f5f 7061 7468  (.    video_path
+00014c50: 733a 204c 6973 745b 556e 696f 6e5b 7374  s: List[Union[st
+00014c60: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
+00014c70: 2c0a 2020 2020 6865 6967 6874 3a20 556e  ,.    height: Un
+00014c80: 696f 6e5b 696e 742c 2073 7472 5d2c 0a20  ion[int, str],. 
+00014c90: 2020 206f 7665 7277 7269 7465 3a20 4f70     overwrite: Op
+00014ca0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
+00014cb0: 616c 7365 2c0a 2020 2020 7361 7665 5f64  alse,.    save_d
+00014cc0: 6972 3a20 4f70 7469 6f6e 616c 5b55 6e69  ir: Optional[Uni
+00014cd0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00014ce0: 696b 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ike]] = None,.  
+00014cf0: 2020 6770 753a 204f 7074 696f 6e61 6c5b    gpu: Optional[
+00014d00: 626f 6f6c 5d20 3d20 4661 6c73 652c 0a20  bool] = False,. 
+00014d10: 2020 2076 6572 626f 7365 3a20 4f70 7469     verbose: Opti
+00014d20: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
+00014d30: 652c 0a29 202d 3e20 556e 696f 6e5b 4e6f  e,.) -> Union[No
+00014d40: 6e65 2c20 4c69 7374 5b55 6e69 6f6e 5b4e  ne, List[Union[N
+00014d50: 6f6e 652c 2073 7472 2c20 6f73 2e50 6174  one, str, os.Pat
+00014d60: 684c 696b 655d 5d5d 3a0a 2020 2020 2222  hLike]]]:.    ""
+00014d70: 220a 2020 2020 5265 2d73 697a 6520 6120  ".    Re-size a 
+00014d80: 6c69 7374 206f 6620 7669 6465 6f73 2074  list of videos t
+00014d90: 6f20 6120 7370 6563 6966 6965 6420 6865  o a specified he
+00014da0: 6967 6874 2077 6869 6c65 2072 6574 6169  ight while retai
+00014db0: 6e69 6e67 2074 6865 6972 2061 7370 6563  ning their aspec
+00014dc0: 7420 7261 7469 6f73 2e0a 0a20 2020 203a  t ratios...    :
+00014dd0: 7061 7261 6d20 4c69 7374 5b55 6e69 6f6e  param List[Union
+00014de0: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+00014df0: 655d 5d20 7669 6465 6f5f 7061 7468 733a  e]] video_paths:
+00014e00: 204c 6973 7420 6f66 2070 6174 6820 746f   List of path to
+00014e10: 2076 6964 656f 732e 0a20 2020 203a 7061   videos..    :pa
+00014e20: 7261 6d20 556e 696f 6e5b 696e 742c 2073  ram Union[int, s
+00014e30: 7472 5d20 6865 6967 6874 3a20 5468 6520  tr] height: The 
+00014e40: 6865 6967 6874 206f 6620 7468 6520 6f75  height of the ou
+00014e50: 7470 7574 2076 6964 656f 732e 2049 6620  tput videos. If 
+00014e60: 696e 742c 2074 6865 6e20 7468 6520 6865  int, then the he
+00014e70: 6967 6874 2069 6e20 7069 7865 6c73 2e20  ight in pixels. 
+00014e80: 4966 2073 7472 2c20 7468 656e 2074 6865  If str, then the
+00014e90: 2069 6e64 6578 2069 6e20 6060 7669 6465   index in ``vide
+00014ea0: 6f5f 7061 7468 7360 6020 6672 6f6d 2077  o_paths`` from w
+00014eb0: 6869 6368 2074 6f20 6772 6162 2074 6865  hich to grab the
+00014ec0: 2068 6569 6768 742e 0a20 2020 203a 7061   height..    :pa
+00014ed0: 7261 6d20 4f70 7469 6f6e 616c 5b62 6f6f  ram Optional[boo
+00014ee0: 6c5d 206f 7665 7277 7269 7465 3a20 4966  l] overwrite: If
+00014ef0: 2054 7275 652c 2074 6865 6e20 6f76 6572   True, then over
+00014f00: 7772 6974 6573 2074 6865 206f 7269 6769  writes the origi
+00014f10: 6e61 6c20 7669 6465 6f73 2e20 4465 6661  nal videos. Defa
+00014f20: 756c 7420 4661 6c73 652e 0a20 2020 203a  ult False..    :
+00014f30: 7061 7261 6d20 4f70 7469 6f6e 616c 5b55  param Optional[U
+00014f40: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00014f50: 684c 696b 655d 5d20 7361 7665 5f64 6972  hLike]] save_dir
+00014f60: 3a20 4966 206e 6f74 204e 6f6e 652c 2074  : If not None, t
+00014f70: 6865 6e20 7468 6520 6469 7265 6374 6f72  hen the director
+00014f80: 7920 7768 6572 6520 746f 2073 746f 7265  y where to store
+00014f90: 2074 6865 2072 652d 7369 7a65 6420 7669   the re-sized vi
+00014fa0: 6465 6f73 2e0a 2020 2020 3a70 6172 616d  deos..    :param
+00014fb0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00014fc0: 6770 753a 2049 6620 5472 7565 2c20 7468  gpu: If True, th
+00014fd0: 656e 2075 7365 2046 466d 7065 6720 4750  en use FFmpeg GP
+00014fe0: 5520 636f 6465 6373 2e20 4465 6661 756c  U codecs. Defaul
+00014ff0: 7420 4661 6c73 652e 0a20 2020 203a 7061  t False..    :pa
+00015000: 7261 6d20 4f70 7469 6f6e 616c 5b62 6f6f  ram Optional[boo
+00015010: 6c5d 2076 6572 626f 7365 3a20 4966 2054  l] verbose: If T
+00015020: 7275 652c 2070 7269 6e74 7320 7072 6f67  rue, prints prog
+00015030: 7265 7373 2e20 4465 6661 756c 7420 5472  ress. Default Tr
+00015040: 7565 2e0a 2020 2020 3a72 6574 7572 6e20  ue..    :return 
+00015050: 556e 696f 6e5b 4e6f 6e65 2c20 4c69 7374  Union[None, List
+00015060: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
+00015070: 6174 684c 696b 655d 5d5d 3a20 4966 2073  athLike]]]: If s
+00015080: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
+00015090: 6f6e 652c 2072 6574 7572 6e73 2074 6865  one, returns the
+000150a0: 2070 6174 6873 206f 6620 7468 6520 7265   paths of the re
+000150b0: 2d73 697a 6564 2076 6964 656f 732e 2045  -sized videos. E
+000150c0: 6c73 6520 7265 7475 726e 7320 656d 7074  lse returns empt
+000150d0: 7920 6c69 7374 2e0a 0a20 2020 203a 6578  y list...    :ex
+000150e0: 616d 706c 653a 0a20 2020 203e 3e3e 2076  ample:.    >>> v
+000150f0: 6964 656f 5f70 6174 6873 3d20 5b27 2f55  ideo_paths= ['/U
+00015100: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+00015110: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
+00015120: 6f75 626c 6573 686f 6f74 696e 672f 5241  oubleshooting/RA
+00015130: 545f 4e4f 522f 7072 6f6a 6563 745f 666f  T_NOR/project_fo
+00015140: 6c64 6572 2f76 6964 656f 732f 7465 7374  lder/videos/test
+00015150: 2f30 3831 3032 3032 315f 444f 545f 5261  /08102021_DOT_Ra
+00015160: 7437 5f38 2832 292e 6d70 3427 2c20 272f  t7_8(2).mp4', '/
+00015170: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+00015180: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+00015190: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
+000151a0: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
+000151b0: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
+000151c0: 742f 3038 3130 3230 3231 5f44 4f54 5f52  t/08102021_DOT_R
+000151d0: 6174 3131 5f31 322e 6d70 3427 5d0a 2020  at11_12.mp4'].  
+000151e0: 2020 3e3e 3e20 5f20 3d20 7265 7369 7a65    >>> _ = resize
+000151f0: 5f76 6964 656f 735f 6279 5f68 6569 6768  _videos_by_heigh
+00015200: 7428 7669 6465 6f5f 7061 7468 733d 7669  t(video_paths=vi
+00015210: 6465 6f5f 7061 7468 732c 2068 6569 6768  deo_paths, heigh
+00015220: 743d 3330 302c 206f 7665 7277 7269 7465  t=300, overwrite
+00015230: 3d46 616c 7365 2c20 7361 7665 5f64 6972  =False, save_dir
+00015240: 3d27 2f55 7365 7273 2f73 696d 6f6e 2f44  ='/Users/simon/D
+00015250: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+00015260: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+00015270: 672f 5241 545f 4e4f 522f 7072 6f6a 6563  g/RAT_NOR/projec
+00015280: 745f 666f 6c64 6572 2f76 6964 656f 732f  t_folder/videos/
+00015290: 7465 7374 2f6e 6577 2729 0a20 2020 2022  test/new').    "
+000152a0: 2222 0a20 2020 2074 696d 6572 203d 2053  "".    timer = S
+000152b0: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
+000152c0: 5472 7565 290a 2020 2020 6966 2028 6e6f  True).    if (no
+000152d0: 7420 6f76 6572 7772 6974 6529 2061 6e64  t overwrite) and
+000152e0: 2028 7361 7665 5f64 6972 2069 7320 4e6f   (save_dir is No
+000152f0: 6e65 293a 0a20 2020 2020 2020 2072 6169  ne):.        rai
+00015300: 7365 2049 6e76 616c 6964 496e 7075 7445  se InvalidInputE
+00015310: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00015320: 2020 6d73 673d 2250 6173 7320 6120 7361    msg="Pass a sa
+00015330: 7665 5f64 6972 204f 5220 7365 7420 6f76  ve_dir OR set ov
+00015340: 6572 7772 6974 6520 746f 2054 7275 6522  erwrite to True"
+00015350: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
+00015360: 7572 6365 3d72 6573 697a 655f 7669 6465  urce=resize_vide
+00015370: 6f73 5f62 795f 6865 6967 6874 2e5f 5f6e  os_by_height.__n
+00015380: 616d 655f 5f2c 0a20 2020 2020 2020 2029  ame__,.        )
+00015390: 0a20 2020 2065 6c69 6620 286f 7665 7277  .    elif (overw
+000153a0: 7269 7465 2920 616e 6420 2873 6176 655f  rite) and (save_
+000153b0: 6469 7220 6973 206e 6f74 204e 6f6e 6529  dir is not None)
+000153c0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+000153d0: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
+000153e0: 7228 0a20 2020 2020 2020 2020 2020 206d  r(.            m
+000153f0: 7367 3d22 5061 7373 2045 4954 4845 5220  sg="Pass EITHER 
+00015400: 6f76 6572 7772 6974 6520 6173 2054 7275  overwrite as Tru
+00015410: 6520 4f52 2070 6173 7320 6120 7361 7665  e OR pass a save
+00015420: 5f64 6972 222c 0a20 2020 2020 2020 2020  _dir",.         
+00015430: 2020 2073 6f75 7263 653d 7265 7369 7a65     source=resize
+00015440: 5f76 6964 656f 735f 6279 5f68 6569 6768  _videos_by_heigh
+00015450: 742e 5f5f 6e61 6d65 5f5f 2c0a 2020 2020  t.__name__,.    
+00015460: 2020 2020 290a 2020 2020 6966 2073 6176      ).    if sav
+00015470: 655f 6469 7220 6973 206e 6f74 204e 6f6e  e_dir is not Non
+00015480: 653a 0a20 2020 2020 2020 2069 6620 6e6f  e:.        if no
+00015490: 7420 6f73 2e70 6174 682e 6973 6469 7228  t os.path.isdir(
+000154a0: 7361 7665 5f64 6972 293a 0a20 2020 2020  save_dir):.     
+000154b0: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
+000154c0: 7273 2873 6176 655f 6469 7229 0a20 2020  rs(save_dir).   
+000154d0: 2063 6865 636b 5f76 616c 6964 5f6c 7374   check_valid_lst
+000154e0: 280a 2020 2020 2020 2020 6461 7461 3d76  (.        data=v
+000154f0: 6964 656f 5f70 6174 6873 2c20 736f 7572  ideo_paths, sour
+00015500: 6365 3d72 6573 697a 655f 7669 6465 6f73  ce=resize_videos
+00015510: 5f62 795f 6865 6967 6874 2e5f 5f6e 616d  _by_height.__nam
+00015520: 655f 5f2c 206d 696e 5f6c 656e 3d31 0a20  e__, min_len=1. 
+00015530: 2020 2029 0a20 2020 205f 203d 205b 6368     ).    _ = [ch
+00015540: 6563 6b5f 6669 6c65 5f65 7869 7374 5f61  eck_file_exist_a
+00015550: 6e64 5f72 6561 6461 626c 6528 7829 2066  nd_readable(x) f
+00015560: 6f72 2078 2069 6e20 7669 6465 6f5f 7061  or x in video_pa
+00015570: 7468 735d 0a20 2020 206e 6577 5f76 6964  ths].    new_vid
+00015580: 656f 5f70 6174 6873 203d 205b 5d0a 2020  eo_paths = [].  
+00015590: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000155a0: 6865 6967 6874 2c20 7374 7229 3a0a 2020  height, str):.  
+000155b0: 2020 2020 2020 6368 6563 6b5f 696e 7428        check_int(
+000155c0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+000155d0: 653d 6622 7b72 6573 697a 655f 7669 6465  e=f"{resize_vide
+000155e0: 6f73 5f62 795f 6865 6967 6874 2e5f 5f6e  os_by_height.__n
+000155f0: 616d 655f 5f7d 2068 6569 6768 7422 2c0a  ame__} height",.
+00015600: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00015610: 653d 6865 6967 6874 2c0a 2020 2020 2020  e=height,.      
+00015620: 2020 2020 2020 6d69 6e5f 7661 6c75 653d        min_value=
+00015630: 302c 0a20 2020 2020 2020 2020 2020 206d  0,.            m
+00015640: 6178 5f76 616c 7565 3d6c 656e 2876 6964  ax_value=len(vid
+00015650: 656f 5f70 6174 6873 292c 0a20 2020 2020  eo_paths),.     
+00015660: 2020 2029 0a20 2020 2020 2020 2076 6964     ).        vid
+00015670: 656f 5f68 6569 6768 7473 203d 205b 5d0a  eo_heights = [].
+00015680: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00015690: 2076 6964 656f 5f70 6174 6873 3a0a 2020   video_paths:.  
+000156a0: 2020 2020 2020 2020 2020 7669 6465 6f5f            video_
+000156b0: 6865 6967 6874 732e 6170 7065 6e64 2867  heights.append(g
+000156c0: 6574 5f76 6964 656f 5f6d 6574 615f 6461  et_video_meta_da
+000156d0: 7461 2876 6964 656f 5f70 6174 683d 6929  ta(video_path=i)
+000156e0: 5b22 6865 6967 6874 225d 290a 2020 2020  ["height"]).    
+000156f0: 2020 2020 6865 6967 6874 203d 2076 6964      height = vid
+00015700: 656f 5f68 6569 6768 7473 5b69 6e74 2868  eo_heights[int(h
+00015710: 6569 6768 7429 5d0a 2020 2020 666f 7220  eight)].    for 
+00015720: 636e 742c 2076 6964 656f 5f70 6174 6820  cnt, video_path 
+00015730: 696e 2065 6e75 6d65 7261 7465 2876 6964  in enumerate(vid
+00015740: 656f 5f70 6174 6873 293a 0a20 2020 2020  eo_paths):.     
+00015750: 2020 2064 6972 5f6e 616d 652c 2076 6964     dir_name, vid
+00015760: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
+00015770: 6574 5f66 6e5f 6578 7428 7669 6465 6f5f  et_fn_ext(video_
+00015780: 7061 7468 290a 2020 2020 2020 2020 6966  path).        if
+00015790: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+000157a0: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
+000157b0: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
+000157c0: 6573 697a 696e 6720 6865 6967 6874 2076  esizing height v
+000157d0: 6964 656f 207b 7669 6465 6f5f 6e61 6d65  ideo {video_name
+000157e0: 7d20 2856 6964 656f 207b 636e 742b 317d  } (Video {cnt+1}
+000157f0: 2f7b 6c65 6e28 7669 6465 6f5f 7061 7468  /{len(video_path
+00015800: 7329 7d29 2e2e 2e22 0a20 2020 2020 2020  s)})...".       
+00015810: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00015820: 6620 6f76 6572 7772 6974 653a 0a20 2020  f overwrite:.   
+00015830: 2020 2020 2020 2020 2064 7420 3d20 6461           dt = da
+00015840: 7465 7469 6d65 2e6e 6f77 2829 2e73 7472  tetime.now().str
+00015850: 6674 696d 6528 2225 5925 6d25 6425 4825  ftime("%Y%m%d%H%
+00015860: 4d25 5322 290a 2020 2020 2020 2020 2020  M%S").          
+00015870: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
+00015880: 2e70 6174 682e 6a6f 696e 2864 6972 5f6e  .path.join(dir_n
+00015890: 616d 652c 2066 227b 7669 6465 6f5f 6e61  ame, f"{video_na
+000158a0: 6d65 7d5f 7b64 747d 2e6d 7034 2229 0a20  me}_{dt}.mp4"). 
+000158b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000158c0: 2020 2020 2020 2020 2073 6176 655f 7061           save_pa
+000158d0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+000158e0: 6e28 7361 7665 5f64 6972 2c20 6622 7b76  n(save_dir, f"{v
+000158f0: 6964 656f 5f6e 616d 657d 2e6d 7034 2229  ideo_name}.mp4")
+00015900: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+00015910: 5f76 6964 656f 5f70 6174 6873 2e61 7070  _video_paths.app
+00015920: 656e 6428 7361 7665 5f70 6174 6829 0a20  end(save_path). 
+00015930: 2020 2020 2020 2069 6620 6770 753a 0a20         if gpu:. 
+00015940: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00015950: 2066 2766 666d 7065 6720 2d79 202d 6877   f'ffmpeg -y -hw
+00015960: 6163 6365 6c20 6175 746f 202d 633a 7620  accel auto -c:v 
+00015970: 6832 3634 5f63 7576 6964 202d 6920 227b  h264_cuvid -i "{
+00015980: 7669 6465 6f5f 7061 7468 7d22 202d 7666  video_path}" -vf
+00015990: 2073 6361 6c65 5f6e 7070 3d2d 323a 7b68   scale_npp=-2:{h
+000159a0: 6569 6768 747d 202d 633a 7620 6832 3634  eight} -c:v h264
+000159b0: 5f6e 7665 6e63 2022 7b73 6176 655f 7061  _nvenc "{save_pa
+000159c0: 7468 7d22 202d 6869 6465 5f62 616e 6e65  th}" -hide_banne
+000159d0: 7220 2d6c 6f67 6c65 7665 6c20 6572 726f  r -loglevel erro
+000159e0: 7220 2d79 270a 2020 2020 2020 2020 656c  r -y'.        el
+000159f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015a00: 636d 6420 3d20 6627 6666 6d70 6567 202d  cmd = f'ffmpeg -
+00015a10: 7920 2d69 2022 7b76 6964 656f 5f70 6174  y -i "{video_pat
+00015a20: 687d 2220 2d76 6620 7363 616c 653d 2d32  h}" -vf scale=-2
+00015a30: 3a7b 6865 6967 6874 7d20 227b 7361 7665  :{height} "{save
+00015a40: 5f70 6174 687d 2220 2d68 6964 655f 6261  _path}" -hide_ba
+00015a50: 6e6e 6572 202d 6c6f 676c 6576 656c 2065  nner -loglevel e
+00015a60: 7272 6f72 202d 7927 0a20 2020 2020 2020  rror -y'.       
+00015a70: 2073 7562 7072 6f63 6573 732e 6361 6c6c   subprocess.call
+00015a80: 2863 6d64 2c20 7368 656c 6c3d 5472 7565  (cmd, shell=True
+00015a90: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
+00015aa0: 6573 732e 5049 5045 290a 2020 2020 2020  ess.PIPE).      
+00015ab0: 2020 6966 206f 7665 7277 7269 7465 3a0a    if overwrite:.
+00015ac0: 2020 2020 2020 2020 2020 2020 7368 7574              shut
+00015ad0: 696c 2e63 6f70 7928 7361 7665 5f70 6174  il.copy(save_pat
+00015ae0: 682c 2076 6964 656f 5f70 6174 6829 0a20  h, video_path). 
+00015af0: 2020 2020 2020 2020 2020 206f 732e 7265             os.re
+00015b00: 6d6f 7665 2873 6176 655f 7061 7468 290a  move(save_path).
+00015b10: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
+00015b20: 696d 6572 2829 0a20 2020 2069 6620 7665  imer().    if ve
+00015b30: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+00015b40: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+00015b50: 2020 6622 5265 7369 7a65 6420 6865 6967    f"Resized heig
+00015b60: 6874 207b 6c65 6e28 7669 6465 6f5f 7061  ht {len(video_pa
+00015b70: 7468 7329 7d20 7669 6465 6f28 7329 2e20  ths)} video(s). 
+00015b80: 456c 6170 7365 6420 7469 6d65 3a20 7b74  Elapsed time: {t
+00015b90: 696d 6572 2e65 6c61 7073 6564 5f74 696d  imer.elapsed_tim
+00015ba0: 655f 7374 727d 732e 220a 2020 2020 2020  e_str}s.".      
+00015bb0: 2020 290a 2020 2020 7265 7475 726e 206e    ).    return n
+00015bc0: 6577 5f76 6964 656f 5f70 6174 6873 0a0a  ew_video_paths..
+00015bd0: 0a64 6566 2072 6573 697a 655f 7669 6465  .def resize_vide
+00015be0: 6f73 5f62 795f 7769 6474 6828 0a20 2020  os_by_width(.   
+00015bf0: 2076 6964 656f 5f70 6174 6873 3a20 4c69   video_paths: Li
+00015c00: 7374 5b55 6e69 6f6e 5b73 7472 2c20 6f73  st[Union[str, os
+00015c10: 2e50 6174 684c 696b 655d 5d2c 0a20 2020  .PathLike]],.   
+00015c20: 2077 6964 7468 3a20 556e 696f 6e5b 696e   width: Union[in
+00015c30: 742c 2073 7472 5d2c 0a20 2020 206f 7665  t, str],.    ove
+00015c40: 7277 7269 7465 3a20 4f70 7469 6f6e 616c  rwrite: Optional
+00015c50: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+00015c60: 2020 2020 7361 7665 5f64 6972 3a20 4f70      save_dir: Op
+00015c70: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+00015c80: 2c20 6f73 2e50 6174 684c 696b 655d 5d20  , os.PathLike]] 
+00015c90: 3d20 4e6f 6e65 2c0a 2020 2020 6770 753a  = None,.    gpu:
+00015ca0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00015cb0: 3d20 4661 6c73 652c 0a20 2020 2076 6572  = False,.    ver
+00015cc0: 626f 7365 3a20 4f70 7469 6f6e 616c 5b62  bose: Optional[b
+00015cd0: 6f6f 6c5d 203d 2054 7275 652c 0a29 202d  ool] = True,.) -
+00015ce0: 3e20 556e 696f 6e5b 4e6f 6e65 2c20 4c69  > Union[None, Li
+00015cf0: 7374 5b55 6e69 6f6e 5b4e 6f6e 652c 2073  st[Union[None, s
+00015d00: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+00015d10: 5d5d 3a0a 2020 2020 2222 220a 2020 2020  ]]:.    """.    
+00015d20: 5265 2d73 697a 6520 6120 6c69 7374 206f  Re-size a list o
+00015d30: 6620 7669 6465 6f73 2074 6f20 6120 7370  f videos to a sp
+00015d40: 6563 6966 6965 6420 7769 6474 6820 7768  ecified width wh
+00015d50: 696c 6520 7265 7461 696e 696e 6720 7468  ile retaining th
+00015d60: 6569 7220 6173 7065 6374 2072 6174 696f  eir aspect ratio
+00015d70: 732e 0a0a 2020 2020 3a70 6172 616d 204c  s...    :param L
+00015d80: 6973 745b 556e 696f 6e5b 7374 722c 206f  ist[Union[str, o
+00015d90: 732e 5061 7468 4c69 6b65 5d5d 2076 6964  s.PathLike]] vid
+00015da0: 656f 5f70 6174 6873 3a20 4c69 7374 206f  eo_paths: List o
+00015db0: 6620 7061 7468 2074 6f20 7669 6465 6f73  f path to videos
+00015dc0: 2e0a 2020 2020 3a70 6172 616d 2055 6e69  ..    :param Uni
+00015dd0: 6f6e 5b69 6e74 2c20 7374 725d 2077 6964  on[int, str] wid
+00015de0: 7468 3a20 5468 6520 7769 6474 6820 6f66  th: The width of
+00015df0: 2074 6865 206f 7574 7075 7420 7669 6465   the output vide
+00015e00: 6f73 2e20 4966 2069 6e74 2c20 7468 656e  os. If int, then
+00015e10: 2074 6865 2077 6964 7468 2069 6e20 7069   the width in pi
+00015e20: 7865 6c73 2e20 4966 2073 7472 2c20 7468  xels. If str, th
+00015e30: 656e 2074 6865 2069 6e64 6578 2069 6e20  en the index in 
+00015e40: 6060 7669 6465 6f5f 7061 7468 7360 6020  ``video_paths`` 
+00015e50: 6672 6f6d 2077 6869 6368 2074 6f20 6772  from which to gr
+00015e60: 6162 2074 6865 2077 6964 7468 2e0a 2020  ab the width..  
+00015e70: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+00015e80: 6c5b 626f 6f6c 5d20 6f76 6572 7772 6974  l[bool] overwrit
+00015e90: 653a 2049 6620 5472 7565 2c20 7468 656e  e: If True, then
+00015ea0: 206f 7665 7277 7269 7465 7320 7468 6520   overwrites the 
+00015eb0: 6f72 6967 696e 616c 2076 6964 656f 732e  original videos.
+00015ec0: 2044 6566 6175 6c74 2046 616c 7365 2e0a   Default False..
+00015ed0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00015ee0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+00015ef0: 732e 5061 7468 4c69 6b65 5d5d 2073 6176  s.PathLike]] sav
+00015f00: 655f 6469 723a 2049 6620 6e6f 7420 4e6f  e_dir: If not No
+00015f10: 6e65 2c20 7468 656e 2074 6865 2064 6972  ne, then the dir
+00015f20: 6563 746f 7279 2077 6865 7265 2074 6f20  ectory where to 
+00015f30: 7374 6f72 6520 7468 6520 7265 2d73 697a  store the re-siz
+00015f40: 6564 2076 6964 656f 732e 0a20 2020 203a  ed videos..    :
+00015f50: 7061 7261 6d20 4f70 7469 6f6e 616c 5b62  param Optional[b
+00015f60: 6f6f 6c5d 2067 7075 3a20 4966 2054 7275  ool] gpu: If Tru
+00015f70: 652c 2074 6865 6e20 7573 6520 4646 6d70  e, then use FFmp
+00015f80: 6567 2047 5055 2063 6f64 6563 732e 2044  eg GPU codecs. D
+00015f90: 6566 6175 6c74 2046 616c 7365 2e0a 2020  efault False..  
+00015fa0: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+00015fb0: 6c5b 626f 6f6c 5d20 7665 7262 6f73 653a  l[bool] verbose:
+00015fc0: 2049 6620 5472 7565 2c20 7072 696e 7473   If True, prints
+00015fd0: 2070 726f 6772 6573 732e 2044 6566 6175   progress. Defau
+00015fe0: 6c74 2054 7275 652e 0a20 2020 203a 7265  lt True..    :re
+00015ff0: 7475 726e 2055 6e69 6f6e 5b4e 6f6e 652c  turn Union[None,
+00016000: 204c 6973 745b 556e 696f 6e5b 7374 722c   List[Union[str,
+00016010: 206f 732e 5061 7468 4c69 6b65 5d5d 5d3a   os.PathLike]]]:
+00016020: 2049 6620 7361 7665 5f64 6972 2069 7320   If save_dir is 
+00016030: 6e6f 7420 4e6f 6e65 2c20 7265 7475 726e  not None, return
+00016040: 7320 7468 6520 7061 7468 7320 6f66 2074  s the paths of t
+00016050: 6865 2072 652d 7369 7a65 6420 7669 6465  he re-sized vide
+00016060: 6f73 2e20 456c 7365 2072 6574 7572 6e73  os. Else returns
+00016070: 2065 6d70 7479 206c 6973 742e 0a0a 2020   empty list...  
+00016080: 2020 3a65 7861 6d70 6c65 3a0a 2020 2020    :example:.    
+00016090: 3e3e 3e20 7669 6465 6f5f 7061 7468 733d  >>> video_paths=
+000160a0: 205b 272f 5573 6572 732f 7369 6d6f 6e2f   ['/Users/simon/
+000160b0: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+000160c0: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+000160d0: 6e67 2f52 4154 5f4e 4f52 2f70 726f 6a65  ng/RAT_NOR/proje
+000160e0: 6374 5f66 6f6c 6465 722f 7669 6465 6f73  ct_folder/videos
+000160f0: 2f74 6573 742f 3038 3130 3230 3231 5f44  /test/08102021_D
+00016100: 4f54 5f52 6174 375f 3828 3229 2e6d 7034  OT_Rat7_8(2).mp4
+00016110: 272c 2027 2f55 7365 7273 2f73 696d 6f6e  ', '/Users/simon
+00016120: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
+00016130: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
+00016140: 696e 672f 5241 545f 4e4f 522f 7072 6f6a  ing/RAT_NOR/proj
+00016150: 6563 745f 666f 6c64 6572 2f76 6964 656f  ect_folder/video
+00016160: 732f 7465 7374 2f30 3831 3032 3032 315f  s/test/08102021_
+00016170: 444f 545f 5261 7431 315f 3132 2e6d 7034  DOT_Rat11_12.mp4
+00016180: 275d 0a20 2020 203e 3e3e 205f 203d 2072  '].    >>> _ = r
+00016190: 6573 697a 655f 7669 6465 6f73 5f62 795f  esize_videos_by_
+000161a0: 7769 6474 6828 7669 6465 6f5f 7061 7468  width(video_path
+000161b0: 733d 7669 6465 6f5f 7061 7468 732c 2077  s=video_paths, w
+000161c0: 6964 7468 3d33 3030 2c20 6f76 6572 7772  idth=300, overwr
+000161d0: 6974 653d 4661 6c73 652c 2073 6176 655f  ite=False, save_
+000161e0: 6469 723d 272f 5573 6572 732f 7369 6d6f  dir='/Users/simo
+000161f0: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+00016200: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+00016210: 7469 6e67 2f52 4154 5f4e 4f52 2f70 726f  ting/RAT_NOR/pro
+00016220: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+00016230: 6f73 2f74 6573 742f 6e65 7727 290a 2020  os/test/new').  
+00016240: 2020 2222 220a 0a20 2020 2074 696d 6572    """..    timer
+00016250: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
+00016260: 6172 743d 5472 7565 290a 2020 2020 6966  art=True).    if
+00016270: 2028 6e6f 7420 6f76 6572 7772 6974 6529   (not overwrite)
+00016280: 2061 6e64 2028 7361 7665 5f64 6972 2069   and (save_dir i
+00016290: 7320 4e6f 6e65 293a 0a20 2020 2020 2020  s None):.       
+000162a0: 2072 6169 7365 2049 6e76 616c 6964 496e   raise InvalidIn
+000162b0: 7075 7445 7272 6f72 280a 2020 2020 2020  putError(.      
+000162c0: 2020 2020 2020 6d73 673d 2250 726f 7669        msg="Provi
+000162d0: 6465 2061 2073 6176 655f 6469 7220 6f72  de a save_dir or
+000162e0: 2073 6574 206f 7665 7277 7269 7465 2074   set overwrite t
+000162f0: 6f20 5472 7565 222c 0a20 2020 2020 2020  o True",.       
+00016300: 2020 2020 2073 6f75 7263 653d 7265 7369       source=resi
+00016310: 7a65 5f76 6964 656f 735f 6279 5f77 6964  ze_videos_by_wid
+00016320: 7468 2e5f 5f6e 616d 655f 5f2c 0a20 2020  th.__name__,.   
+00016330: 2020 2020 2029 0a20 2020 2065 6c69 6620       ).    elif 
+00016340: 286f 7665 7277 7269 7465 2920 616e 6420  (overwrite) and 
+00016350: 2873 6176 655f 6469 7220 6973 206e 6f74  (save_dir is not
+00016360: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00016370: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
+00016380: 7574 4572 726f 7228 0a20 2020 2020 2020  utError(.       
+00016390: 2020 2020 206d 7367 3d22 5365 7420 4549       msg="Set EI
+000163a0: 5448 4552 206f 7665 7277 7269 7465 2074  THER overwrite t
+000163b0: 6f20 5472 7565 204f 5220 5072 6f76 6964  o True OR Provid
+000163c0: 6520 6120 7361 7665 5f64 6972 222c 0a20  e a save_dir",. 
+000163d0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000163e0: 653d 7265 7369 7a65 5f76 6964 656f 735f  e=resize_videos_
+000163f0: 6279 5f77 6964 7468 2e5f 5f6e 616d 655f  by_width.__name_
+00016400: 5f2c 0a20 2020 2020 2020 2029 0a20 2020  _,.        ).   
+00016410: 2069 6620 7361 7665 5f64 6972 2069 7320   if save_dir is 
+00016420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016430: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+00016440: 2e69 7364 6972 2873 6176 655f 6469 7229  .isdir(save_dir)
+00016450: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
+00016460: 2e6d 616b 6564 6972 7328 7361 7665 5f64  .makedirs(save_d
+00016470: 6972 290a 2020 2020 6368 6563 6b5f 7661  ir).    check_va
+00016480: 6c69 645f 6c73 7428 6461 7461 3d76 6964  lid_lst(data=vid
+00016490: 656f 5f70 6174 6873 2c20 736f 7572 6365  eo_paths, source
+000164a0: 3d72 6573 697a 655f 7669 6465 6f73 5f62  =resize_videos_b
+000164b0: 795f 7769 6474 682e 5f5f 6e61 6d65 5f5f  y_width.__name__
+000164c0: 2c20 6d69 6e5f 6c65 6e3d 3129 0a20 2020  , min_len=1).   
+000164d0: 205f 203d 205b 6368 6563 6b5f 6669 6c65   _ = [check_file
+000164e0: 5f65 7869 7374 5f61 6e64 5f72 6561 6461  _exist_and_reada
+000164f0: 626c 6528 7829 2066 6f72 2078 2069 6e20  ble(x) for x in 
+00016500: 7669 6465 6f5f 7061 7468 735d 0a20 2020  video_paths].   
+00016510: 206e 6577 5f76 6964 656f 5f70 6174 6873   new_video_paths
+00016520: 203d 205b 5d0a 2020 2020 6966 2069 7369   = [].    if isi
+00016530: 6e73 7461 6e63 6528 7769 6474 682c 2073  nstance(width, s
+00016540: 7472 293a 0a20 2020 2020 2020 2063 6865  tr):.        che
+00016550: 636b 5f69 6e74 280a 2020 2020 2020 2020  ck_int(.        
+00016560: 2020 2020 6e61 6d65 3d66 227b 7265 7369      name=f"{resi
+00016570: 7a65 5f76 6964 656f 735f 6279 5f77 6964  ze_videos_by_wid
+00016580: 7468 2e5f 5f6e 616d 655f 5f7d 2068 6569  th.__name__} hei
+00016590: 6768 7422 2c0a 2020 2020 2020 2020 2020  ght",.          
+000165a0: 2020 7661 6c75 653d 7769 6474 682c 0a20    value=width,. 
+000165b0: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
+000165c0: 616c 7565 3d30 2c0a 2020 2020 2020 2020  alue=0,.        
+000165d0: 2020 2020 6d61 785f 7661 6c75 653d 6c65      max_value=le
+000165e0: 6e28 7669 6465 6f5f 7061 7468 7329 2c0a  n(video_paths),.
+000165f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00016600: 2020 7669 6465 6f5f 7769 6474 6873 203d    video_widths =
+00016610: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+00016620: 6920 696e 2076 6964 656f 5f70 6174 6873  i in video_paths
+00016630: 3a0a 2020 2020 2020 2020 2020 2020 7669  :.            vi
+00016640: 6465 6f5f 7769 6474 6873 2e61 7070 656e  deo_widths.appen
+00016650: 6428 6765 745f 7669 6465 6f5f 6d65 7461  d(get_video_meta
+00016660: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
+00016670: 3d69 295b 2277 6964 7468 225d 290a 2020  =i)["width"]).  
+00016680: 2020 2020 2020 7769 6474 6820 3d20 7669        width = vi
+00016690: 6465 6f5f 7769 6474 6873 5b69 6e74 2877  deo_widths[int(w
+000166a0: 6964 7468 295d 0a20 2020 2066 6f72 2063  idth)].    for c
+000166b0: 6e74 2c20 7669 6465 6f5f 7061 7468 2069  nt, video_path i
+000166c0: 6e20 656e 756d 6572 6174 6528 7669 6465  n enumerate(vide
+000166d0: 6f5f 7061 7468 7329 3a0a 2020 2020 2020  o_paths):.      
+000166e0: 2020 6469 725f 6e61 6d65 2c20 7669 6465    dir_name, vide
+000166f0: 6f5f 6e61 6d65 2c20 6578 7420 3d20 6765  o_name, ext = ge
+00016700: 745f 666e 5f65 7874 2876 6964 656f 5f70  t_fn_ext(video_p
+00016710: 6174 6829 0a20 2020 2020 2020 2069 6620  ath).        if 
+00016720: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00016730: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
+00016740: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
+00016750: 7369 7a69 6e67 2077 6964 7468 2076 6964  sizing width vid
+00016760: 656f 207b 7669 6465 6f5f 6e61 6d65 7d20  eo {video_name} 
+00016770: 2856 6964 656f 207b 636e 742b 317d 2f7b  (Video {cnt+1}/{
+00016780: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
+00016790: 7d29 2e2e 2e22 0a20 2020 2020 2020 2020  })...".         
+000167a0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+000167b0: 6f76 6572 7772 6974 653a 0a20 2020 2020  overwrite:.     
+000167c0: 2020 2020 2020 2064 7420 3d20 6461 7465         dt = date
+000167d0: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
+000167e0: 696d 6528 2225 5925 6d25 6425 4825 4d25  ime("%Y%m%d%H%M%
+000167f0: 5322 290a 2020 2020 2020 2020 2020 2020  S").            
+00016800: 7361 7665 5f70 6174 6820 3d20 6f73 2e70  save_path = os.p
+00016810: 6174 682e 6a6f 696e 2864 6972 5f6e 616d  ath.join(dir_nam
+00016820: 652c 2066 227b 7669 6465 6f5f 6e61 6d65  e, f"{video_name
+00016830: 7d5f 7b64 747d 2e6d 7034 2229 0a20 2020  }_{dt}.mp4").   
+00016840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016850: 2020 2020 2020 2073 6176 655f 7061 7468         save_path
+00016860: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00016870: 7361 7665 5f64 6972 2c20 6622 7b76 6964  save_dir, f"{vid
+00016880: 656f 5f6e 616d 657d 2e6d 7034 2229 0a20  eo_name}.mp4"). 
+00016890: 2020 2020 2020 2020 2020 206e 6577 5f76             new_v
+000168a0: 6964 656f 5f70 6174 6873 2e61 7070 656e  ideo_paths.appen
+000168b0: 6428 7361 7665 5f70 6174 6829 0a20 2020  d(save_path).   
+000168c0: 2020 2020 2069 6620 6770 753a 0a20 2020       if gpu:.   
+000168d0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+000168e0: 2766 666d 7065 6720 2d79 202d 6877 6163  'ffmpeg -y -hwac
+000168f0: 6365 6c20 6175 746f 202d 6920 227b 7669  cel auto -i "{vi
+00016900: 6465 6f5f 7061 7468 7d22 202d 7666 2073  deo_path}" -vf s
+00016910: 6361 6c65 5f6e 7070 3d7b 7769 6474 687d  cale_npp={width}
+00016920: 3a2d 3220 2d63 3a76 2068 3236 345f 6e76  :-2 -c:v h264_nv
+00016930: 656e 6320 227b 7361 7665 5f70 6174 687d  enc "{save_path}
+00016940: 2220 2d68 6964 655f 6261 6e6e 6572 202d  " -hide_banner -
+00016950: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
+00016960: 7927 0a20 2020 2020 2020 2065 6c73 653a  y'.        else:
+00016970: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00016980: 203d 2066 2766 666d 7065 6720 2d79 202d   = f'ffmpeg -y -
+00016990: 6920 227b 7669 6465 6f5f 7061 7468 7d22  i "{video_path}"
+000169a0: 202d 7666 2073 6361 6c65 3d7b 7769 6474   -vf scale={widt
+000169b0: 687d 3a2d 3220 227b 7361 7665 5f70 6174  h}:-2 "{save_pat
+000169c0: 687d 2220 2d68 6964 655f 6261 6e6e 6572  h}" -hide_banner
+000169d0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
+000169e0: 202d 7927 0a20 2020 2020 2020 2073 7562   -y'.        sub
+000169f0: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
+00016a00: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
+00016a10: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
+00016a20: 5049 5045 290a 2020 2020 2020 2020 6966  PIPE).        if
+00016a30: 206f 7665 7277 7269 7465 3a0a 2020 2020   overwrite:.    
+00016a40: 2020 2020 2020 2020 7368 7574 696c 2e63          shutil.c
+00016a50: 6f70 7928 7361 7665 5f70 6174 682c 2076  opy(save_path, v
+00016a60: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
+00016a70: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
+00016a80: 2873 6176 655f 7061 7468 290a 2020 2020  (save_path).    
+00016a90: 7469 6d65 722e 7374 6f70 5f74 696d 6572  timer.stop_timer
+00016aa0: 2829 0a20 2020 2069 6620 7665 7262 6f73  ().    if verbos
+00016ab0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
+00016ac0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00016ad0: 5265 7369 7a65 6420 7769 6474 6820 7b6c  Resized width {l
+00016ae0: 656e 2876 6964 656f 5f70 6174 6873 297d  en(video_paths)}
+00016af0: 2076 6964 656f 2873 292e 2045 6c61 7073   video(s). Elaps
+00016b00: 6564 2074 696d 653a 207b 7469 6d65 722e  ed time: {timer.
+00016b10: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
+00016b20: 7d73 2e22 0a20 2020 2020 2020 2029 0a20  }s.".        ). 
+00016b30: 2020 2072 6574 7572 6e20 6e65 775f 7669     return new_vi
+00016b40: 6465 6f5f 7061 7468 730a 0a0a 6465 6620  deo_paths...def 
+00016b50: 6372 6561 7465 5f62 6c61 6e6b 5f76 6964  create_blank_vid
+00016b60: 656f 280a 2020 2020 7061 7468 3a20 556e  eo(.    path: Un
+00016b70: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00016b80: 4c69 6b65 5d2c 0a20 2020 206c 656e 6774  Like],.    lengt
+00016b90: 683a 2069 6e74 2c0a 2020 2020 7769 6474  h: int,.    widt
+00016ba0: 683a 2069 6e74 2c0a 2020 2020 6865 6967  h: int,.    heig
+00016bb0: 6874 3a20 696e 742c 0a20 2020 2063 6f6c  ht: int,.    col
+00016bc0: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
+00016bd0: 5d20 3d20 2262 6c61 636b 222c 0a20 2020  ] = "black",.   
+00016be0: 2067 7075 3a20 4f70 7469 6f6e 616c 5b62   gpu: Optional[b
+00016bf0: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
+00016c00: 2020 7665 7262 6f73 653a 204f 7074 696f    verbose: Optio
+00016c10: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+00016c20: 652c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  e,.) -> None:.  
+00016c30: 2020 2222 220a 2020 2020 4372 6561 7465    """.    Create
+00016c40: 2061 2022 626c 616e 6b22 2075 6e69 2d63   a "blank" uni-c
+00016c50: 6f6c 6f72 6564 2076 6964 656f 206f 6620  olored video of 
+00016c60: 7370 6563 6966 6965 6420 7369 7a65 2061  specified size a
+00016c70: 6e64 206c 656e 6774 682e 0a0a 2020 2020  nd length...    
+00016c80: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
+00016c90: 2c20 6f73 2e50 6174 684c 696b 655d 2070  , os.PathLike] p
+00016ca0: 6174 683a 204c 6f63 6174 696f 6e20 7768  ath: Location wh
+00016cb0: 6572 6520 746f 2073 746f 7265 2074 6865  ere to store the
+00016cc0: 2062 6c61 6e6b 2076 6964 656f 2e0a 2020   blank video..  
+00016cd0: 2020 3a70 6172 616d 2069 6e74 206c 656e    :param int len
+00016ce0: 6774 683a 204c 656e 6774 6820 6f66 2074  gth: Length of t
+00016cf0: 6865 2062 6c61 6e6b 2076 6964 656f 2069  he blank video i
+00016d00: 6e20 7365 636f 6e64 732e 0a20 2020 203a  n seconds..    :
+00016d10: 7061 7261 6d20 696e 7420 7769 6474 683a  param int width:
+00016d20: 2057 6964 7468 206f 6620 7468 6520 626c   Width of the bl
+00016d30: 616e 6b20 7669 6465 6f20 696e 2070 6978  ank video in pix
+00016d40: 656c 732e 0a20 2020 203a 7061 7261 6d20  els..    :param 
+00016d50: 696e 7420 6865 6967 6874 3a20 4865 6967  int height: Heig
+00016d60: 6874 206f 6620 7468 6520 626c 616e 6b20  ht of the blank 
+00016d70: 7669 6465 6f20 696e 2070 6978 656c 732e  video in pixels.
+00016d80: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00016d90: 6f6e 616c 5b73 7472 5d20 636f 6c6f 723a  onal[str] color:
+00016da0: 2043 6f6c 6f72 206f 6620 7468 6520 626c   Color of the bl
+00016db0: 616e 6b20 7669 6465 6f2e 2044 6566 6175  ank video. Defau
+00016dc0: 6c74 2062 6c61 636b 2e0a 2020 2020 3a70  lt black..    :p
+00016dd0: 6172 616d 204f 7074 696f 6e61 6c5b 626f  aram Optional[bo
+00016de0: 6f6c 5d20 6770 753a 2049 6620 5472 7565  ol] gpu: If True
+00016df0: 2c20 7468 656e 2075 7365 2046 466d 7065  , then use FFmpe
+00016e00: 6720 4750 5520 636f 6465 6373 2e20 4465  g GPU codecs. De
+00016e10: 6661 756c 7420 4661 6c73 652e 0a20 2020  fault False..   
+00016e20: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00016e30: 5b62 6f6f 6c5d 2076 6572 626f 7365 3a20  [bool] verbose: 
+00016e40: 4966 2054 7275 652c 2070 7269 6e74 7320  If True, prints 
+00016e50: 7072 6f67 7265 7373 2e20 4465 6661 756c  progress. Defaul
+00016e60: 7420 5472 7565 2e0a 2020 2020 3a72 6574  t True..    :ret
+00016e70: 7572 6e3a 204e 6f6e 652e 0a0a 2020 2020  urn: None...    
+00016e80: 3a65 7861 6d70 6c65 3a0a 2020 2020 3e3e  :example:.    >>
+00016e90: 3e20 5f20 3d20 6372 6561 7465 5f62 6c61  > _ = create_bla
+00016ea0: 6e6b 5f76 6964 656f 2870 6174 683d 272f  nk_video(path='/
+00016eb0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+00016ec0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+00016ed0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
+00016ee0: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
+00016ef0: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
+00016f00: 742f 6e65 772f 626c 616e 6b5f 7465 7374  t/new/blank_test
+00016f10: 2e6d 7034 272c 206c 656e 6774 683d 352c  .mp4', length=5,
+00016f20: 2077 6964 7468 3d33 3030 2c20 6865 6967   width=300, heig
+00016f30: 6874 3d34 3030 2c20 6770 753d 4661 6c73  ht=400, gpu=Fals
+00016f40: 652c 2076 6572 626f 7365 3d54 7275 652c  e, verbose=True,
+00016f50: 2063 6f6c 6f72 3d27 6f72 616e 6765 2729   color='orange')
+00016f60: 0a20 2020 2022 2222 0a0a 2020 2020 6368  .    """..    ch
+00016f70: 6563 6b5f 696e 7428 6e61 6d65 3d66 227b  eck_int(name=f"{
+00016f80: 6372 6561 7465 5f62 6c61 6e6b 5f76 6964  create_blank_vid
+00016f90: 656f 2e5f 5f6e 616d 655f 5f7d 206c 656e  eo.__name__} len
+00016fa0: 6774 6822 2c20 7661 6c75 653d 6c65 6e67  gth", value=leng
+00016fb0: 7468 2c20 6d69 6e5f 7661 6c75 653d 3129  th, min_value=1)
+00016fc0: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
+00016fd0: 616d 653d 6622 7b63 7265 6174 655f 626c  ame=f"{create_bl
+00016fe0: 616e 6b5f 7669 6465 6f2e 5f5f 6e61 6d65  ank_video.__name
+00016ff0: 5f5f 7d20 7769 6474 6822 2c20 7661 6c75  __} width", valu
+00017000: 653d 7769 6474 682c 206d 696e 5f76 616c  e=width, min_val
+00017010: 7565 3d31 290a 2020 2020 6368 6563 6b5f  ue=1).    check_
+00017020: 696e 7428 6e61 6d65 3d66 227b 6372 6561  int(name=f"{crea
+00017030: 7465 5f62 6c61 6e6b 5f76 6964 656f 2e5f  te_blank_video._
+00017040: 5f6e 616d 655f 5f7d 2068 6569 6768 7422  _name__} height"
+00017050: 2c20 7661 6c75 653d 6865 6967 6874 2c20  , value=height, 
+00017060: 6d69 6e5f 7661 6c75 653d 3129 0a20 2020  min_value=1).   
+00017070: 2063 6865 636b 5f69 665f 6469 725f 6578   check_if_dir_ex
+00017080: 6973 7473 280a 2020 2020 2020 2020 696e  ists(.        in
+00017090: 5f64 6972 3d6f 732e 7061 7468 2e64 6972  _dir=os.path.dir
+000170a0: 6e61 6d65 2870 6174 6829 2c0a 2020 2020  name(path),.    
+000170b0: 2020 2020 736f 7572 6365 3d63 7265 6174      source=creat
+000170c0: 655f 626c 616e 6b5f 7669 6465 6f2e 5f5f  e_blank_video.__
+000170d0: 6e61 6d65 5f5f 2c0a 2020 2020 2020 2020  name__,.        
+000170e0: 6372 6561 7465 5f69 665f 6e6f 745f 6578  create_if_not_ex
+000170f0: 6973 743d 5472 7565 2c0a 2020 2020 290a  ist=True,.    ).
+00017100: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
+00017110: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
+00017120: 6529 0a20 2020 2069 6620 7665 7262 6f73  e).    if verbos
+00017130: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
+00017140: 2822 4372 6561 7469 6e67 2062 6c61 6e6b  ("Creating blank
+00017150: 2076 6964 656f 2e2e 2e22 290a 2020 2020   video...").    
+00017160: 6966 2067 7075 3a0a 2020 2020 2020 2020  if gpu:.        
+00017170: 636d 6420 3d20 6627 6666 6d70 6567 202d  cmd = f'ffmpeg -
+00017180: 7920 2d74 207b 6c65 6e67 7468 7d20 2d66  y -t {length} -f
+00017190: 206c 6176 6669 202d 6920 636f 6c6f 723d   lavfi -i color=
+000171a0: 633d 7b63 6f6c 6f72 7d3a 733d 7b77 6964  c={color}:s={wid
+000171b0: 7468 7d78 7b68 6569 6768 747d 202d 633a  th}x{height} -c:
+000171c0: 7620 6832 3634 5f6e 7665 6e63 202d 7072  v h264_nvenc -pr
+000171d0: 6573 6574 2073 6c6f 7720 2d74 756e 6520  eset slow -tune 
+000171e0: 7374 696c 6c69 6d61 6765 202d 7069 785f  stillimage -pix_
+000171f0: 666d 7420 7975 7634 3230 7020 227b 7061  fmt yuv420p "{pa
+00017200: 7468 7d22 202d 6869 6465 5f62 616e 6e65  th}" -hide_banne
+00017210: 7220 2d6c 6f67 6c65 7665 6c20 6572 726f  r -loglevel erro
+00017220: 7220 2d79 270a 2020 2020 656c 7365 3a0a  r -y'.    else:.
+00017230: 2020 2020 2020 2020 636d 6420 3d20 6627          cmd = f'
+00017240: 6666 6d70 6567 202d 7920 2d74 207b 6c65  ffmpeg -y -t {le
+00017250: 6e67 7468 7d20 2d66 206c 6176 6669 202d  ngth} -f lavfi -
+00017260: 6920 636f 6c6f 723d 633d 7b63 6f6c 6f72  i color=c={color
+00017270: 7d3a 733d 7b77 6964 7468 7d78 7b68 6569  }:s={width}x{hei
+00017280: 6768 747d 202d 633a 7620 6c69 6278 3236  ght} -c:v libx26
+00017290: 3420 2d74 756e 6520 7374 696c 6c69 6d61  4 -tune stillima
+000172a0: 6765 202d 7069 785f 666d 7420 7975 7634  ge -pix_fmt yuv4
+000172b0: 3230 7020 227b 7061 7468 7d22 202d 6869  20p "{path}" -hi
+000172c0: 6465 5f62 616e 6e65 7220 2d6c 6f67 6c65  de_banner -logle
+000172d0: 7665 6c20 6572 726f 7220 2d79 270a 2020  vel error -y'.  
+000172e0: 2020 7375 6270 726f 6365 7373 2e63 616c    subprocess.cal
+000172f0: 6c28 636d 642c 2073 6865 6c6c 3d54 7275  l(cmd, shell=Tru
+00017300: 652c 2073 7464 6f75 743d 7375 6270 726f  e, stdout=subpro
+00017310: 6365 7373 2e50 4950 4529 0a20 2020 2074  cess.PIPE).    t
+00017320: 696d 6572 2e73 746f 705f 7469 6d65 7228  imer.stop_timer(
+00017330: 290a 2020 2020 6966 2076 6572 626f 7365  ).    if verbose
+00017340: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00017350: 0a20 2020 2020 2020 2020 2020 2066 2242  .            f"B
+00017360: 6c61 6e6b 2076 6964 656f 2063 6f6d 706c  lank video compl
+00017370: 6574 652e 2053 6176 6564 2061 7420 7b70  ete. Saved at {p
+00017380: 6174 687d 2e20 456c 6170 7365 6420 7469  ath}. Elapsed ti
+00017390: 6d65 3a20 7b74 696d 6572 2e65 6c61 7073  me: {timer.elaps
+000173a0: 6564 5f74 696d 655f 7374 727d 732e 220a  ed_time_str}s.".
+000173b0: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
+000173c0: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
+000173d0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
+000173e0: 2020 2076 6964 656f 5f70 6174 6873 3a20     video_paths: 
+000173f0: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
+00017400: 6f73 2e50 6174 684c 696b 655d 5d2c 0a20  os.PathLike]],. 
+00017410: 2020 2073 6176 655f 7061 7468 3a20 556e     save_path: Un
+00017420: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00017430: 4c69 6b65 5d2c 0a20 2020 2068 6569 6768  Like],.    heigh
+00017440: 745f 7078 3a20 4f70 7469 6f6e 616c 5b55  t_px: Optional[U
+00017450: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d20  nion[int, str]] 
+00017460: 3d20 4e6f 6e65 2c0a 2020 2020 6865 6967  = None,.    heig
+00017470: 6874 5f69 6478 3a20 4f70 7469 6f6e 616c  ht_idx: Optional
+00017480: 5b55 6e69 6f6e 5b69 6e74 2c20 7374 725d  [Union[int, str]
+00017490: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6770  ] = None,.    gp
+000174a0: 753a 204f 7074 696f 6e61 6c5b 626f 6f6c  u: Optional[bool
+000174b0: 5d20 3d20 4661 6c73 652c 0a20 2020 2076  ] = False,.    v
+000174c0: 6572 626f 7365 3a20 4f70 7469 6f6e 616c  erbose: Optional
+000174d0: 5b62 6f6f 6c5d 203d 2054 7275 652c 0a29  [bool] = True,.)
+000174e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+000174f0: 220a 2020 2020 436f 6e63 6174 656e 6174  ".    Concatenat
+00017500: 6573 206d 756c 7469 706c 6520 7669 6465  es multiple vide
+00017510: 6f73 2068 6f72 697a 6f6e 7461 6c6c 792e  os horizontally.
+00017520: 0a0a 2020 2020 2e2e 2069 6d61 6765 3a3a  ..    .. image::
+00017530: 205f 7374 6174 6963 2f69 6d67 2f68 6f72   _static/img/hor
+00017540: 697a 6f6e 7461 6c5f 7669 6465 6f5f 636f  izontal_video_co
+00017550: 6e63 6174 656e 6174 6f72 2e67 6966 0a20  ncatenator.gif. 
+00017560: 2020 2020 2020 3a77 6964 7468 3a20 3630        :width: 60
+00017570: 300a 2020 2020 2020 203a 616c 6967 6e3a  0.       :align:
+00017580: 2063 656e 7465 720a 0a20 2020 203a 7061   center..    :pa
+00017590: 7261 6d20 4c69 7374 5b55 6e69 6f6e 5b73  ram List[Union[s
+000175a0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+000175b0: 5d20 7669 6465 6f5f 7061 7468 733a 204c  ] video_paths: L
+000175c0: 6973 7420 6f66 2069 6e70 7574 2076 6964  ist of input vid
+000175d0: 656f 2066 696c 6520 7061 7468 732e 0a20  eo file paths.. 
+000175e0: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
+000175f0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+00017600: 5d20 7361 7665 5f70 6174 683a 2046 696c  ] save_path: Fil
+00017610: 6520 7061 7468 2074 6f20 7361 7665 2074  e path to save t
+00017620: 6865 2063 6f6e 6361 7465 6e61 7465 6420  he concatenated 
+00017630: 7669 6465 6f2e 0a20 2020 203a 7061 7261  video..    :para
+00017640: 6d20 4f70 7469 6f6e 616c 5b69 6e74 5d20  m Optional[int] 
+00017650: 6865 6967 6874 5f70 783a 2048 6569 6768  height_px: Heigh
+00017660: 7420 6f66 2074 6865 206f 7574 7075 7420  t of the output 
+00017670: 7669 6465 6f20 696e 2070 6978 656c 732e  video in pixels.
+00017680: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00017690: 6f6e 616c 5b69 6e74 5d20 6865 6967 6874  onal[int] height
+000176a0: 5f69 6478 3a20 496e 6465 7820 6f66 2074  _idx: Index of t
+000176b0: 6865 2076 6964 656f 2074 6f20 7573 6520  he video to use 
+000176c0: 666f 7220 6465 7465 726d 696e 696e 6720  for determining 
+000176d0: 4865 6967 6874 2e0a 2020 2020 3a70 6172  Height..    :par
+000176e0: 616d 204f 7074 696f 6e61 6c5b 626f 6f6c  am Optional[bool
+000176f0: 5d20 6770 753a 2057 6865 7468 6572 2074  ] gpu: Whether t
+00017700: 6f20 7573 6520 4750 552d 6163 6365 6c65  o use GPU-accele
+00017710: 7261 7465 6420 636f 6465 6320 2864 6566  rated codec (def
+00017720: 6175 6c74 3a20 4661 6c73 6529 2e0a 2020  ault: False)..  
+00017730: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+00017740: 6c5b 626f 6f6c 5d20 7665 7262 6f73 653a  l[bool] verbose:
+00017750: 5768 6574 6865 7220 746f 2070 7269 6e74  Whether to print
+00017760: 2070 726f 6772 6573 7320 6d65 7373 6167   progress messag
+00017770: 6573 2028 6465 6661 756c 743a 2054 7275  es (default: Tru
+00017780: 6529 2e0a 0a20 2020 203a 6578 616d 706c  e)...    :exampl
+00017790: 653a 0a20 2020 203e 3e3e 2076 6964 656f  e:.    >>> video
+000177a0: 5f70 6174 6873 203d 205b 2776 6964 656f  _paths = ['video
+000177b0: 312e 6d70 3427 2c20 2776 6964 656f 322e  1.mp4', 'video2.
+000177c0: 6d70 3427 5d0a 2020 2020 3e3e 3e20 7820  mp4'].    >>> x 
+000177d0: 3d20 686f 7269 7a6f 6e74 616c 5f76 6964  = horizontal_vid
+000177e0: 656f 5f63 6f6e 6361 7465 6e61 746f 7228  eo_concatenator(
+000177f0: 7669 6465 6f5f 7061 7468 733d 7669 6465  video_paths=vide
+00017800: 6f5f 7061 7468 732c 2068 6569 6768 745f  o_paths, height_
+00017810: 7078 3d35 302c 2073 6176 655f 7061 7468  px=50, save_path
+00017820: 3d27 2f55 7365 7273 2f73 696d 6f6e 2f44  ='/Users/simon/D
+00017830: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+00017840: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+00017850: 672f 5241 545f 4e4f 522f 7072 6f6a 6563  g/RAT_NOR/projec
+00017860: 745f 666f 6c64 6572 2f76 6964 656f 732f  t_folder/videos/
+00017870: 7465 7374 2f6e 6577 2f30 3831 3032 3032  test/new/0810202
+00017880: 315f 444f 545f 5261 7437 5f38 2832 295f  1_DOT_Rat7_8(2)_
+00017890: 2e6d 7034 272c 2067 7075 3d46 616c 7365  .mp4', gpu=False
+000178a0: 290a 2020 2020 2222 220a 2020 2020 6368  ).    """.    ch
+000178b0: 6563 6b5f 6666 6d70 6567 5f61 7661 696c  eck_ffmpeg_avail
+000178c0: 6162 6c65 2829 0a20 2020 2069 6620 6770  able().    if gp
+000178d0: 7520 616e 6420 6e6f 7420 6368 6563 6b5f  u and not check_
+000178e0: 6e76 6964 6561 5f67 7075 5f61 7661 696c  nvidea_gpu_avail
+000178f0: 6162 6c65 2829 3a0a 2020 2020 2020 2020  able():.        
+00017900: 7261 6973 6520 4646 4d50 4547 436f 6465  raise FFMPEGCode
+00017910: 6347 5055 4572 726f 7228 0a20 2020 2020  cGPUError(.     
+00017920: 2020 2020 2020 206d 7367 3d22 4e56 4944         msg="NVID
+00017930: 4541 2047 5055 206e 6f74 2061 7661 696c  EA GPU not avail
+00017940: 6162 6c65 2028 6173 2065 7661 6c75 6174  able (as evaluat
+00017950: 6564 2062 7920 6e76 6964 6561 2d73 6d69  ed by nvidea-smi
+00017960: 2072 6574 7572 6e69 6e67 204e 6f6e 6529   returning None)
+00017970: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+00017980: 6f75 7263 653d 686f 7269 7a6f 6e74 616c  ource=horizontal
+00017990: 5f76 6964 656f 5f63 6f6e 6361 7465 6e61  _video_concatena
+000179a0: 746f 722e 5f5f 6e61 6d65 5f5f 2c0a 2020  tor.__name__,.  
+000179b0: 2020 2020 2020 290a 2020 2020 7469 6d65        ).    time
+000179c0: 7220 3d20 5369 6d62 6154 696d 6572 2873  r = SimbaTimer(s
+000179d0: 7461 7274 3d54 7275 6529 0a20 2020 2063  tart=True).    c
+000179e0: 6865 636b 5f76 616c 6964 5f6c 7374 280a  heck_valid_lst(.
+000179f0: 2020 2020 2020 2020 6461 7461 3d76 6964          data=vid
+00017a00: 656f 5f70 6174 6873 2c20 736f 7572 6365  eo_paths, source
+00017a10: 3d68 6f72 697a 6f6e 7461 6c5f 7669 6465  =horizontal_vide
+00017a20: 6f5f 636f 6e63 6174 656e 6174 6f72 2e5f  o_concatenator._
+00017a30: 5f6e 616d 655f 5f2c 206d 696e 5f6c 656e  _name__, min_len
+00017a40: 3d32 0a20 2020 2029 0a20 2020 2063 6865  =2.    ).    che
+00017a50: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
+00017a60: 280a 2020 2020 2020 2020 696e 5f64 6972  (.        in_dir
+00017a70: 3d6f 732e 7061 7468 2e64 6972 6e61 6d65  =os.path.dirname
+00017a80: 2873 6176 655f 7061 7468 292c 2073 6f75  (save_path), sou
+00017a90: 7263 653d 686f 7269 7a6f 6e74 616c 5f76  rce=horizontal_v
+00017aa0: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
+00017ab0: 722e 5f5f 6e61 6d65 5f5f 0a20 2020 2029  r.__name__.    )
+00017ac0: 0a20 2020 2076 6964 656f 5f6d 6574 615f  .    video_meta_
+00017ad0: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
+00017ae0: 2067 6574 5f76 6964 656f 5f6d 6574 615f   get_video_meta_
+00017af0: 6461 7461 2876 6964 656f 5f70 6174 683d  data(video_path=
+00017b00: 7669 6465 6f5f 7061 7468 2920 666f 7220  video_path) for 
+00017b10: 7669 6465 6f5f 7061 7468 2069 6e20 7669  video_path in vi
+00017b20: 6465 6f5f 7061 7468 730a 2020 2020 5d0a  deo_paths.    ].
+00017b30: 2020 2020 6966 2028 2868 6569 6768 745f      if ((height_
+00017b40: 7078 2069 7320 4e6f 6e65 2920 616e 6420  px is None) and 
+00017b50: 2868 6569 6768 745f 6964 7820 6973 204e  (height_idx is N
+00017b60: 6f6e 6529 2920 6f72 2028 0a20 2020 2020  one)) or (.     
+00017b70: 2020 2028 6865 6967 6874 5f70 7820 6973     (height_px is
+00017b80: 206e 6f74 204e 6f6e 6529 2061 6e64 2028   not None) and (
+00017b90: 6865 6967 6874 5f69 6478 2069 7320 6e6f  height_idx is no
+00017ba0: 7420 4e6f 6e65 290a 2020 2020 293a 0a20  t None).    ):. 
+00017bb0: 2020 2020 2020 2072 6169 7365 2049 6e76         raise Inv
+00017bc0: 616c 6964 496e 7075 7445 7272 6f72 280a  alidInputError(.
+00017bd0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00017be0: 2250 726f 7669 6465 2061 2068 6569 6768  "Provide a heigh
+00017bf0: 745f 7078 204f 5220 6865 6967 6874 5f69  t_px OR height_i
+00017c00: 6478 222c 0a20 2020 2020 2020 2020 2020  dx",.           
+00017c10: 2073 6f75 7263 653d 686f 7269 7a6f 6e74   source=horizont
+00017c20: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
+00017c30: 6e61 746f 722e 5f5f 6e61 6d65 5f5f 2c0a  nator.__name__,.
+00017c40: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
+00017c50: 2068 6569 6768 745f 6964 7820 6973 206e   height_idx is n
+00017c60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017c70: 2063 6865 636b 5f69 6e74 280a 2020 2020   check_int(.    
+00017c80: 2020 2020 2020 2020 6e61 6d65 3d66 227b          name=f"{
+00017c90: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
+00017ca0: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
+00017cb0: 6e61 6d65 5f5f 7d20 6865 6967 6874 222c  name__} height",
+00017cc0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00017cd0: 7565 3d68 6569 6768 745f 6964 782c 0a20  ue=height_idx,. 
+00017ce0: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
+00017cf0: 616c 7565 3d30 2c0a 2020 2020 2020 2020  alue=0,.        
+00017d00: 2020 2020 6d61 785f 7661 6c75 653d 6c65      max_value=le
+00017d10: 6e28 7669 6465 6f5f 7061 7468 7329 202d  n(video_paths) -
+00017d20: 2031 2c0a 2020 2020 2020 2020 290a 2020   1,.        ).  
+00017d30: 2020 2020 2020 6865 6967 6874 203d 2069        height = i
+00017d40: 6e74 2876 6964 656f 5f6d 6574 615f 6461  nt(video_meta_da
+00017d50: 7461 5b68 6569 6768 745f 6964 785d 5b22  ta[height_idx]["
+00017d60: 6865 6967 6874 225d 290a 2020 2020 656c  height"]).    el
+00017d70: 7365 3a0a 2020 2020 2020 2020 6368 6563  se:.        chec
+00017d80: 6b5f 696e 7428 0a20 2020 2020 2020 2020  k_int(.         
+00017d90: 2020 206e 616d 653d 6622 7b68 6f72 697a     name=f"{horiz
+00017da0: 6f6e 7461 6c5f 7669 6465 6f5f 636f 6e63  ontal_video_conc
+00017db0: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
+00017dc0: 5f7d 2068 6569 6768 7422 2c0a 2020 2020  _} height",.    
+00017dd0: 2020 2020 2020 2020 7661 6c75 653d 6865          value=he
+00017de0: 6967 6874 5f70 782c 0a20 2020 2020 2020  ight_px,.       
+00017df0: 2020 2020 206d 696e 5f76 616c 7565 3d31       min_value=1
+00017e00: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00017e10: 2020 2020 6865 6967 6874 203d 2069 6e74      height = int
+00017e20: 2868 6569 6768 745f 7078 290a 2020 2020  (height_px).    
+00017e30: 7669 6465 6f5f 7061 7468 5f73 7472 203d  video_path_str =
+00017e40: 2022 2022 2e6a 6f69 6e28 5b66 272d 6920   " ".join([f'-i 
+00017e50: 227b 7061 7468 7d22 2720 666f 7220 7061  "{path}"' for pa
+00017e60: 7468 2069 6e20 7669 6465 6f5f 7061 7468  th in video_path
+00017e70: 735d 290a 2020 2020 636f 6465 6320 3d20  s]).    codec = 
+00017e80: 2268 3236 345f 6e76 656e 6322 2069 6620  "h264_nvenc" if 
+00017e90: 6770 7520 656c 7365 2022 6c69 6276 7078  gpu else "libvpx
+00017ea0: 2d76 7039 220a 2020 2020 6669 6c74 6572  -vp9".    filter
+00017eb0: 5f63 6f6d 706c 6578 203d 2022 3b22 2e6a  _complex = ";".j
+00017ec0: 6f69 6e28 0a20 2020 2020 2020 205b 6622  oin(.        [f"
+00017ed0: 5b7b 6964 787d 3a76 5d73 6361 6c65 3d2d  [{idx}:v]scale=-
+00017ee0: 313a 7b68 6569 6768 747d 5b76 7b69 6478  1:{height}[v{idx
+00017ef0: 7d5d 2220 666f 7220 6964 7820 696e 2072  }]" for idx in r
+00017f00: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
+00017f10: 6174 6873 2929 5d0a 2020 2020 290a 2020  aths))].    ).  
+00017f20: 2020 6669 6c74 6572 5f63 6f6d 706c 6578    filter_complex
+00017f30: 202b 3d20 6622 3b7b 2727 2e6a 6f69 6e28   += f";{''.join(
+00017f40: 5b66 275b 767b 6964 787d 5d27 2066 6f72  [f'[v{idx}]' for
+00017f50: 2069 6478 2069 6e20 7261 6e67 6528 6c65   idx in range(le
+00017f60: 6e28 7669 6465 6f5f 7061 7468 7329 295d  n(video_paths))]
+00017f70: 297d 6873 7461 636b 3d69 6e70 7574 733d  )}hstack=inputs=
+00017f80: 7b6c 656e 2876 6964 656f 5f70 6174 6873  {len(video_paths
+00017f90: 297d 5b76 5d22 0a20 2020 2069 6620 7665  )}[v]".    if ve
+00017fa0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+00017fb0: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+00017fc0: 2020 6622 436f 6e63 6174 656e 6174 696e    f"Concatenatin
+00017fd0: 6720 7b6c 656e 2876 6964 656f 5f70 6174  g {len(video_pat
+00017fe0: 6873 297d 2076 6964 656f 7320 686f 7269  hs)} videos hori
+00017ff0: 7a6f 6e74 616c 6c79 2077 6974 6820 6120  zontally with a 
+00018000: 7b68 6569 6768 747d 2070 6978 656c 2068  {height} pixel h
+00018010: 6569 6768 742e 2e2e 2022 0a20 2020 2020  eight... ".     
+00018020: 2020 2029 0a20 2020 2063 6d64 203d 2066     ).    cmd = f
+00018030: 2766 666d 7065 6720 7b76 6964 656f 5f70  'ffmpeg {video_p
+00018040: 6174 685f 7374 727d 202d 6669 6c74 6572  ath_str} -filter
+00018050: 5f63 6f6d 706c 6578 2022 7b66 696c 7465  _complex "{filte
+00018060: 725f 636f 6d70 6c65 787d 2220 2d6d 6170  r_complex}" -map
+00018070: 2022 5b76 5d22 202d 633a 7620 7b63 6f64   "[v]" -c:v {cod
+00018080: 6563 7d20 2d6c 6f67 6c65 7665 6c20 6572  ec} -loglevel er
+00018090: 726f 7220 2d73 7461 7473 2022 7b73 6176  ror -stats "{sav
+000180a0: 655f 7061 7468 7d22 202d 7927 0a20 2020  e_path}" -y'.   
+000180b0: 2073 7562 7072 6f63 6573 732e 6361 6c6c   subprocess.call
+000180c0: 2863 6d64 2c20 7368 656c 6c3d 5472 7565  (cmd, shell=True
+000180d0: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
+000180e0: 6573 732e 5049 5045 290a 2020 2020 7469  ess.PIPE).    ti
+000180f0: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
+00018100: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+00018110: 0a20 2020 2020 2020 2070 7269 6e74 280a  .        print(.
+00018120: 2020 2020 2020 2020 2020 2020 6622 486f              f"Ho
+00018130: 7269 7a6f 6e74 616c 2063 6f6e 6361 7465  rizontal concate
+00018140: 6e61 7469 6f6e 2063 6f6d 706c 6574 652c  nation complete,
+00018150: 2073 6176 6564 2061 7420 7b73 6176 655f   saved at {save_
+00018160: 7061 7468 7d20 2865 6c61 7073 6564 2074  path} (elapsed t
+00018170: 696d 653a 207b 7469 6d65 722e 656c 6170  ime: {timer.elap
+00018180: 7365 645f 7469 6d65 5f73 7472 7d73 2e29  sed_time_str}s.)
+00018190: 220a 2020 2020 2020 2020 290a 0a0a 6465  ".        )...de
+000181a0: 6620 7665 7274 6963 616c 5f76 6964 656f  f vertical_video
+000181b0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
+000181c0: 2020 2076 6964 656f 5f70 6174 6873 3a20     video_paths: 
+000181d0: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
+000181e0: 6f73 2e50 6174 684c 696b 655d 5d2c 0a20  os.PathLike]],. 
+000181f0: 2020 2073 6176 655f 7061 7468 3a20 556e     save_path: Un
+00018200: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00018210: 4c69 6b65 5d2c 0a20 2020 2077 6964 7468  Like],.    width
+00018220: 5f70 783a 204f 7074 696f 6e61 6c5b 696e  _px: Optional[in
+00018230: 745d 203d 204e 6f6e 652c 0a20 2020 2077  t] = None,.    w
+00018240: 6964 7468 5f69 6478 3a20 4f70 7469 6f6e  idth_idx: Option
+00018250: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+00018260: 2020 2020 6770 753a 204f 7074 696f 6e61      gpu: Optiona
+00018270: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
+00018280: 0a20 2020 2076 6572 626f 7365 3a20 4f70  .    verbose: Op
+00018290: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
+000182a0: 7275 652c 0a29 202d 3e20 4e6f 6e65 3a0a  rue,.) -> None:.
+000182b0: 2020 2020 2222 220a 2020 2020 436f 6e63      """.    Conc
+000182c0: 6174 656e 6174 6573 206d 756c 7469 706c  atenates multipl
+000182d0: 6520 7669 6465 6f73 2076 6572 7469 6361  e videos vertica
+000182e0: 6c6c 792e 0a0a 2020 2020 2e2e 2069 6d61  lly...    .. ima
+000182f0: 6765 3a3a 205f 7374 6174 6963 2f69 6d67  ge:: _static/img
+00018300: 2f76 6572 7469 6361 6c5f 7669 6465 6f5f  /vertical_video_
+00018310: 636f 6e63 6174 656e 6174 6f72 2e70 6e67  concatenator.png
+00018320: 0a20 2020 2020 2020 3a77 6964 7468 3a20  .       :width: 
+00018330: 3330 300a 2020 2020 2020 203a 616c 6967  300.       :alig
+00018340: 6e3a 2063 656e 7465 720a 0a20 2020 203a  n: center..    :
+00018350: 7061 7261 6d20 4c69 7374 5b55 6e69 6f6e  param List[Union
+00018360: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+00018370: 655d 5d20 7669 6465 6f5f 7061 7468 733a  e]] video_paths:
+00018380: 204c 6973 7420 6f66 2069 6e70 7574 2076   List of input v
+00018390: 6964 656f 2066 696c 6520 7061 7468 732e  ideo file paths.
+000183a0: 0a20 2020 203a 7061 7261 6d20 556e 696f  .    :param Unio
+000183b0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+000183c0: 6b65 5d20 7361 7665 5f70 6174 683a 2046  ke] save_path: F
+000183d0: 696c 6520 7061 7468 2074 6f20 7361 7665  ile path to save
+000183e0: 2074 6865 2063 6f6e 6361 7465 6e61 7465   the concatenate
+000183f0: 6420 7669 6465 6f2e 0a20 2020 203a 7061  d video..    :pa
+00018400: 7261 6d20 4f70 7469 6f6e 616c 5b69 6e74  ram Optional[int
+00018410: 5d20 7769 6474 685f 7078 3a20 5769 6474  ] width_px: Widt
+00018420: 6820 6f66 2074 6865 206f 7574 7075 7420  h of the output 
+00018430: 7669 6465 6f20 696e 2070 6978 656c 732e  video in pixels.
+00018440: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00018450: 6f6e 616c 5b69 6e74 5d20 7769 6474 685f  onal[int] width_
+00018460: 6964 783a 2049 6e64 6578 206f 6620 7468  idx: Index of th
+00018470: 6520 7669 6465 6f20 746f 2075 7365 2066  e video to use f
+00018480: 6f72 2064 6574 6572 6d69 6e69 6e67 2077  or determining w
+00018490: 6964 7468 2e0a 2020 2020 3a70 6172 616d  idth..    :param
+000184a0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+000184b0: 6770 753a 2057 6865 7468 6572 2074 6f20  gpu: Whether to 
+000184c0: 7573 6520 4750 552d 6163 6365 6c65 7261  use GPU-accelera
+000184d0: 7465 6420 636f 6465 6320 2864 6566 6175  ted codec (defau
+000184e0: 6c74 3a20 4661 6c73 6529 2e0a 2020 2020  lt: False)..    
+000184f0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+00018500: 626f 6f6c 5d20 7665 7262 6f73 653a 5768  bool] verbose:Wh
+00018510: 6574 6865 7220 746f 2070 7269 6e74 2070  ether to print p
+00018520: 726f 6772 6573 7320 6d65 7373 6167 6573  rogress messages
+00018530: 2028 6465 6661 756c 743a 2054 7275 6529   (default: True)
+00018540: 2e0a 2020 2020 3a72 6169 7365 7320 4646  ..    :raises FF
+00018550: 4d50 4547 436f 6465 6347 5055 4572 726f  MPEGCodecGPUErro
+00018560: 723a 2049 6620 4750 5520 6973 2072 6571  r: If GPU is req
+00018570: 7565 7374 6564 2062 7574 206e 6f74 2061  uested but not a
+00018580: 7661 696c 6162 6c65 2e0a 2020 2020 3a72  vailable..    :r
+00018590: 6169 7365 7320 496e 7661 6c69 6449 6e70  aises InvalidInp
+000185a0: 7574 4572 726f 723a 2049 6620 626f 7468  utError: If both
+000185b0: 206f 7220 6e65 6974 6865 7220 7769 6474   or neither widt
+000185c0: 685f 7078 2061 6e64 2077 6964 7468 5f69  h_px and width_i
+000185d0: 6478 2061 7265 2070 726f 7669 6465 642e  dx are provided.
+000185e0: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
+000185f0: 2020 2020 3e3e 3e20 7669 6465 6f5f 7061      >>> video_pa
+00018600: 7468 7320 3d20 5b27 2f55 7365 7273 2f73  ths = ['/Users/s
+00018610: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00018620: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00018630: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
+00018640: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
+00018650: 6964 656f 732f 7465 7374 2f30 3831 3032  ideos/test/08102
+00018660: 3032 315f 444f 545f 5261 7437 5f38 2832  021_DOT_Rat7_8(2
+00018670: 292e 6d70 3427 2c0a 2020 2020 3e3e 3e20  ).mp4',.    >>> 
+00018680: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00018690: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+000186a0: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+000186b0: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+000186c0: 5241 545f 4e4f 522f 7072 6f6a 6563 745f  RAT_NOR/project_
+000186d0: 666f 6c64 6572 2f76 6964 656f 732f 7465  folder/videos/te
+000186e0: 7374 2f30 3831 3032 3032 315f 444f 545f  st/08102021_DOT_
+000186f0: 5261 7431 315f 3132 2e6d 7034 272c 0a20  Rat11_12.mp4',. 
+00018700: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+00018710: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
+00018720: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00018730: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00018740: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
+00018750: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+00018760: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
+00018770: 3231 5f44 4f54 5f52 6174 3131 5f31 325f  21_DOT_Rat11_12_
+00018780: 312e 6d70 3427 5d0a 2020 2020 3e3e 3e20  1.mp4'].    >>> 
+00018790: 5f20 3d20 7665 7274 6963 616c 5f76 6964  _ = vertical_vid
+000187a0: 656f 5f63 6f6e 6361 7465 6e61 746f 7228  eo_concatenator(
+000187b0: 7669 6465 6f5f 7061 7468 733d 7669 6465  video_paths=vide
+000187c0: 6f5f 7061 7468 732c 2077 6964 7468 5f69  o_paths, width_i
+000187d0: 6478 3d31 2c20 7361 7665 5f70 6174 683d  dx=1, save_path=
+000187e0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+000187f0: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+00018800: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+00018810: 2f52 4154 5f4e 4f52 2f70 726f 6a65 6374  /RAT_NOR/project
+00018820: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
+00018830: 6573 742f 6e65 772f 3038 3130 3230 3231  est/new/08102021
+00018840: 5f44 4f54 5f52 6174 375f 3828 3229 5f2e  _DOT_Rat7_8(2)_.
+00018850: 6d70 3427 2c20 6770 753d 4661 6c73 6529  mp4', gpu=False)
+00018860: 0a20 2020 2022 2222 0a0a 2020 2020 6368  .    """..    ch
+00018870: 6563 6b5f 6666 6d70 6567 5f61 7661 696c  eck_ffmpeg_avail
+00018880: 6162 6c65 2829 0a20 2020 2069 6620 6770  able().    if gp
+00018890: 7520 616e 6420 6e6f 7420 6368 6563 6b5f  u and not check_
+000188a0: 6e76 6964 6561 5f67 7075 5f61 7661 696c  nvidea_gpu_avail
+000188b0: 6162 6c65 2829 3a0a 2020 2020 2020 2020  able():.        
+000188c0: 7261 6973 6520 4646 4d50 4547 436f 6465  raise FFMPEGCode
+000188d0: 6347 5055 4572 726f 7228 0a20 2020 2020  cGPUError(.     
+000188e0: 2020 2020 2020 206d 7367 3d22 4e56 4944         msg="NVID
+000188f0: 4941 2047 5055 206e 6f74 2061 7661 696c  IA GPU not avail
+00018900: 6162 6c65 222c 2073 6f75 7263 653d 7665  able", source=ve
+00018910: 7274 6963 616c 5f76 6964 656f 5f63 6f6e  rtical_video_con
+00018920: 6361 7465 6e61 746f 722e 5f5f 6e61 6d65  catenator.__name
+00018930: 5f5f 0a20 2020 2020 2020 2029 0a20 2020  __.        ).   
+00018940: 2076 6964 656f 5f6d 6574 615f 6461 7461   video_meta_data
+00018950: 203d 205b 0a20 2020 2020 2020 2067 6574   = [.        get
+00018960: 5f76 6964 656f 5f6d 6574 615f 6461 7461  _video_meta_data
+00018970: 2876 6964 656f 5f70 6174 683d 7669 6465  (video_path=vide
+00018980: 6f5f 7061 7468 2920 666f 7220 7669 6465  o_path) for vide
+00018990: 6f5f 7061 7468 2069 6e20 7669 6465 6f5f  o_path in video_
+000189a0: 7061 7468 730a 2020 2020 5d0a 2020 2020  paths.    ].    
+000189b0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+000189c0: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+000189d0: 2020 2063 6865 636b 5f76 616c 6964 5f6c     check_valid_l
+000189e0: 7374 280a 2020 2020 2020 2020 6461 7461  st(.        data
+000189f0: 3d76 6964 656f 5f70 6174 6873 2c20 736f  =video_paths, so
+00018a00: 7572 6365 3d76 6572 7469 6361 6c5f 7669  urce=vertical_vi
+00018a10: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
+00018a20: 2e5f 5f6e 616d 655f 5f2c 206d 696e 5f6c  .__name__, min_l
+00018a30: 656e 3d32 0a20 2020 2029 0a20 2020 2063  en=2.    ).    c
+00018a40: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
+00018a50: 7473 280a 2020 2020 2020 2020 696e 5f64  ts(.        in_d
+00018a60: 6972 3d6f 732e 7061 7468 2e64 6972 6e61  ir=os.path.dirna
+00018a70: 6d65 2873 6176 655f 7061 7468 292c 2073  me(save_path), s
+00018a80: 6f75 7263 653d 7665 7274 6963 616c 5f76  ource=vertical_v
+00018a90: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
+00018aa0: 722e 5f5f 6e61 6d65 5f5f 0a20 2020 2029  r.__name__.    )
+00018ab0: 0a20 2020 2069 6620 2828 7769 6474 685f  .    if ((width_
+00018ac0: 7078 2069 7320 4e6f 6e65 2920 616e 6420  px is None) and 
+00018ad0: 2877 6964 7468 5f69 6478 2069 7320 4e6f  (width_idx is No
+00018ae0: 6e65 2929 206f 7220 280a 2020 2020 2020  ne)) or (.      
+00018af0: 2020 2877 6964 7468 5f70 7820 6973 206e    (width_px is n
+00018b00: 6f74 204e 6f6e 6529 2061 6e64 2028 7769  ot None) and (wi
+00018b10: 6474 685f 6964 7820 6973 206e 6f74 204e  dth_idx is not N
+00018b20: 6f6e 6529 0a20 2020 2029 3a0a 2020 2020  one).    ):.    
+00018b30: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
+00018b40: 6449 6e70 7574 4572 726f 7228 0a20 2020  dInputError(.   
+00018b50: 2020 2020 2020 2020 206d 7367 3d22 5072           msg="Pr
+00018b60: 6f76 6964 6520 6120 7769 6474 685f 7078  ovide a width_px
+00018b70: 204f 5220 7769 6474 685f 6964 7822 2c0a   OR width_idx",.
+00018b80: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00018b90: 6365 3d76 6572 7469 6361 6c5f 7669 6465  ce=vertical_vide
+00018ba0: 6f5f 636f 6e63 6174 656e 6174 6f72 2e5f  o_concatenator._
+00018bb0: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
+00018bc0: 2029 0a20 2020 2069 6620 7769 6474 685f   ).    if width_
+00018bd0: 6964 7820 6973 206e 6f74 204e 6f6e 653a  idx is not None:
+00018be0: 0a20 2020 2020 2020 2063 6865 636b 5f69  .        check_i
+00018bf0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00018c00: 6e61 6d65 3d66 227b 7665 7274 6963 616c  name=f"{vertical
+00018c10: 5f76 6964 656f 5f63 6f6e 6361 7465 6e61  _video_concatena
+00018c20: 746f 722e 5f5f 6e61 6d65 5f5f 7d20 7769  tor.__name__} wi
+00018c30: 6474 6820 696e 6465 7822 2c0a 2020 2020  dth index",.    
+00018c40: 2020 2020 2020 2020 7661 6c75 653d 7769          value=wi
+00018c50: 6474 685f 6964 782c 0a20 2020 2020 2020  dth_idx,.       
+00018c60: 2020 2020 206d 696e 5f76 616c 7565 3d30       min_value=0
+00018c70: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00018c80: 785f 7661 6c75 653d 6c65 6e28 7669 6465  x_value=len(vide
+00018c90: 6f5f 7061 7468 7329 202d 2031 2c0a 2020  o_paths) - 1,.  
+00018ca0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00018cb0: 7769 6474 6820 3d20 696e 7428 7669 6465  width = int(vide
+00018cc0: 6f5f 6d65 7461 5f64 6174 615b 7769 6474  o_meta_data[widt
+00018cd0: 685f 6964 785d 5b22 7769 6474 6822 5d29  h_idx]["width"])
+00018ce0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00018cf0: 2020 2063 6865 636b 5f69 6e74 280a 2020     check_int(.  
+00018d00: 2020 2020 2020 2020 2020 6e61 6d65 3d66            name=f
+00018d10: 227b 7665 7274 6963 616c 5f76 6964 656f  "{vertical_video
+00018d20: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
+00018d30: 6e61 6d65 5f5f 7d20 7769 6474 6822 2c0a  name__} width",.
+00018d40: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00018d50: 653d 7769 6474 685f 7078 2c0a 2020 2020  e=width_px,.    
+00018d60: 2020 2020 2020 2020 6d69 6e5f 7661 6c75          min_valu
+00018d70: 653d 312c 0a20 2020 2020 2020 2029 0a20  e=1,.        ). 
+00018d80: 2020 2020 2020 2077 6964 7468 203d 2069         width = i
+00018d90: 6e74 2877 6964 7468 5f70 7829 0a20 2020  nt(width_px).   
+00018da0: 2076 6964 656f 5f70 6174 685f 7374 7220   video_path_str 
+00018db0: 3d20 2220 222e 6a6f 696e 285b 6627 2d69  = " ".join([f'-i
+00018dc0: 2022 7b70 6174 687d 2227 2066 6f72 2070   "{path}"' for p
+00018dd0: 6174 6820 696e 2076 6964 656f 5f70 6174  ath in video_pat
+00018de0: 6873 5d29 0a20 2020 2063 6f64 6563 203d  hs]).    codec =
+00018df0: 2022 6832 3634 5f6e 7665 6e63 2220 6966   "h264_nvenc" if
+00018e00: 2067 7075 2065 6c73 6520 226c 6962 7670   gpu else "libvp
+00018e10: 782d 7670 3922 0a20 2020 2066 696c 7465  x-vp9".    filte
+00018e20: 725f 636f 6d70 6c65 7820 3d20 223b 222e  r_complex = ";".
+00018e30: 6a6f 696e 280a 2020 2020 2020 2020 5b66  join(.        [f
+00018e40: 225b 7b69 6478 7d3a 765d 7363 616c 653d  "[{idx}:v]scale=
+00018e50: 7b77 6964 7468 7d3a 2d31 5b76 7b69 6478  {width}:-1[v{idx
+00018e60: 7d5d 2220 666f 7220 6964 7820 696e 2072  }]" for idx in r
+00018e70: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
+00018e80: 6174 6873 2929 5d0a 2020 2020 290a 2020  aths))].    ).  
+00018e90: 2020 6669 6c74 6572 5f63 6f6d 706c 6578    filter_complex
+00018ea0: 202b 3d20 6622 3b7b 2727 2e6a 6f69 6e28   += f";{''.join(
+00018eb0: 5b66 275b 767b 6964 787d 5d27 2066 6f72  [f'[v{idx}]' for
+00018ec0: 2069 6478 2069 6e20 7261 6e67 6528 6c65   idx in range(le
+00018ed0: 6e28 7669 6465 6f5f 7061 7468 7329 295d  n(video_paths))]
+00018ee0: 297d 220a 2020 2020 6669 6c74 6572 5f63  )}".    filter_c
+00018ef0: 6f6d 706c 6578 202b 3d20 6622 7673 7461  omplex += f"vsta
+00018f00: 636b 3d69 6e70 7574 733d 7b6c 656e 2876  ck=inputs={len(v
+00018f10: 6964 656f 5f70 6174 6873 297d 5b76 5d22  ideo_paths)}[v]"
+00018f20: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+00018f30: 0a20 2020 2020 2020 2070 7269 6e74 280a  .        print(.
+00018f40: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+00018f50: 6e63 6174 656e 6174 696e 6720 7b6c 656e  ncatenating {len
+00018f60: 2876 6964 656f 5f70 6174 6873 297d 2076  (video_paths)} v
+00018f70: 6964 656f 7320 7665 7274 6963 616c 6c79  ideos vertically
+00018f80: 2077 6974 6820 6120 7b77 6964 7468 7d20   with a {width} 
+00018f90: 7069 7865 6c20 7769 6474 682e 2e2e 220a  pixel width...".
+00018fa0: 2020 2020 2020 2020 290a 2020 2020 636d          ).    cm
+00018fb0: 6420 3d20 6627 6666 6d70 6567 207b 7669  d = f'ffmpeg {vi
+00018fc0: 6465 6f5f 7061 7468 5f73 7472 7d20 2d66  deo_path_str} -f
+00018fd0: 696c 7465 725f 636f 6d70 6c65 7820 227b  ilter_complex "{
+00018fe0: 6669 6c74 6572 5f63 6f6d 706c 6578 7d22  filter_complex}"
+00018ff0: 202d 6d61 7020 225b 765d 2220 2d63 3a76   -map "[v]" -c:v
+00019000: 207b 636f 6465 637d 202d 6c6f 676c 6576   {codec} -loglev
+00019010: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
+00019020: 227b 7361 7665 5f70 6174 687d 2220 2d79  "{save_path}" -y
+00019030: 270a 2020 2020 7375 6270 726f 6365 7373  '.    subprocess
+00019040: 2e63 616c 6c28 636d 642c 2073 6865 6c6c  .call(cmd, shell
+00019050: 3d54 7275 652c 2073 7464 6f75 743d 7375  =True, stdout=su
+00019060: 6270 726f 6365 7373 2e50 4950 4529 0a20  bprocess.PIPE). 
+00019070: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
+00019080: 6d65 7228 290a 2020 2020 6966 2076 6572  mer().    if ver
+00019090: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
+000190a0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+000190b0: 2066 2256 6572 7469 6361 6c20 636f 6e63   f"Vertical conc
+000190c0: 6174 656e 6174 696f 6e20 636f 6d70 6c65  atenation comple
+000190d0: 7465 2e20 5361 7665 6420 6174 207b 7361  te. Saved at {sa
+000190e0: 7665 5f70 6174 687d 2028 456c 6170 7365  ve_path} (Elapse
+000190f0: 6420 7469 6d65 3a20 7b74 696d 6572 2e65  d time: {timer.e
+00019100: 6c61 7073 6564 5f74 696d 655f 7374 727d  lapsed_time_str}
+00019110: 732e 2922 0a20 2020 2020 2020 2029 0a0a  s.)".        )..
+00019120: 0a64 6566 206d 6f73 6169 635f 636f 6e63  .def mosaic_conc
+00019130: 6174 656e 6174 6f72 280a 2020 2020 7669  atenator(.    vi
+00019140: 6465 6f5f 7061 7468 733a 204c 6973 745b  deo_paths: List[
+00019150: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00019160: 7468 4c69 6b65 5d5d 2c0a 2020 2020 7361  thLike]],.    sa
+00019170: 7665 5f70 6174 683a 2055 6e69 6f6e 5b73  ve_path: Union[s
+00019180: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+00019190: 2c0a 2020 2020 7769 6474 685f 6964 783a  ,.    width_idx:
+000191a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+000191b0: 696e 742c 2073 7472 5d5d 203d 204e 6f6e  int, str]] = Non
+000191c0: 652c 0a20 2020 2077 6964 7468 5f70 783a  e,.    width_px:
+000191d0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+000191e0: 696e 742c 2073 7472 5d5d 203d 204e 6f6e  int, str]] = Non
+000191f0: 652c 0a20 2020 2068 6569 6768 745f 6964  e,.    height_id
+00019200: 783a 204f 7074 696f 6e61 6c5b 556e 696f  x: Optional[Unio
+00019210: 6e5b 696e 742c 2073 7472 5d5d 203d 204e  n[int, str]] = N
+00019220: 6f6e 652c 0a20 2020 2068 6569 6768 745f  one,.    height_
+00019230: 7078 3a20 4f70 7469 6f6e 616c 5b55 6e69  px: Optional[Uni
+00019240: 6f6e 5b69 6e74 2c20 7374 725d 5d20 3d20  on[int, str]] = 
+00019250: 4e6f 6e65 2c0a 2020 2020 6770 753a 204f  None,.    gpu: O
+00019260: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00019270: 4661 6c73 652c 0a20 2020 2076 6572 626f  False,.    verbo
+00019280: 7365 3a20 4f70 7469 6f6e 616c 5b62 6f6f  se: Optional[boo
+00019290: 6c5d 203d 2054 7275 652c 0a20 2020 2075  l] = True,.    u
+000192a0: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
+000192b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000192c0: 3d20 2262 6c61 636b 222c 0a29 202d 3e20  = "black",.) -> 
+000192d0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+000192e0: 2020 436f 6e63 6174 656e 6174 6573 206d    Concatenates m
+000192f0: 756c 7469 706c 6520 7669 6465 6f73 2069  ultiple videos i
+00019300: 6e74 6f20 6120 6d6f 7361 6963 206c 6179  nto a mosaic lay
+00019310: 6f75 742e 0a0a 2020 2020 2e2e 2069 6d61  out...    .. ima
+00019320: 6765 3a3a 205f 7374 6174 6963 2f69 6d67  ge:: _static/img
+00019330: 2f6d 6f73 6169 635f 636f 6e63 6174 656e  /mosaic_concaten
+00019340: 6174 6f72 2e70 6e67 0a20 2020 2020 2020  ator.png.       
+00019350: 3a77 6964 7468 3a20 3630 300a 2020 2020  :width: 600.    
+00019360: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
+00019370: 720a 0a20 2020 202e 2e20 6e6f 7465 3a3a  r..    .. note::
+00019380: 0a20 2020 2020 2020 6966 2061 6e20 756e  .       if an un
+00019390: 6576 656e 206e 756d 6265 7220 6f66 2076  even number of v
+000193a0: 6964 656f 732c 2074 6865 206c 6173 7420  ideos, the last 
+000193b0: 696e 6465 7820 7769 6c6c 2062 6520 6669  index will be fi
+000193c0: 6c6c 6564 2062 7920 6060 756e 6576 656e  lled by ``uneven
+000193d0: 5f66 696c 6c5f 636f 6c6f 7260 602e 0a0a  _fill_color``...
+000193e0: 2020 2020 3a70 6172 616d 204c 6973 745b      :param List[
+000193f0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00019400: 7468 4c69 6b65 5d5d 2076 6964 656f 5f70  thLike]] video_p
+00019410: 6174 6873 3a20 4c69 7374 206f 6620 696e  aths: List of in
+00019420: 7075 7420 7669 6465 6f20 6669 6c65 2070  put video file p
+00019430: 6174 6873 2e0a 2020 2020 3a70 6172 616d  aths..    :param
+00019440: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00019450: 6174 684c 696b 655d 2073 6176 655f 7061  athLike] save_pa
+00019460: 7468 3a20 4669 6c65 2070 6174 6820 746f  th: File path to
+00019470: 2073 6176 6520 7468 6520 636f 6e63 6174   save the concat
+00019480: 656e 6174 6564 2076 6964 656f 2e0a 2020  enated video..  
+00019490: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+000194a0: 6c5b 696e 745d 2077 6964 7468 5f70 783a  l[int] width_px:
+000194b0: 2057 6964 7468 206f 6620 7468 6520 6f75   Width of the ou
+000194c0: 7470 7574 2076 6964 656f 2069 6e20 7069  tput video in pi
+000194d0: 7865 6c73 2e0a 2020 2020 3a70 6172 616d  xels..    :param
+000194e0: 204f 7074 696f 6e61 6c5b 696e 745d 2077   Optional[int] w
+000194f0: 6964 7468 5f69 6478 3a20 496e 6465 7820  idth_idx: Index 
+00019500: 6f66 2074 6865 2076 6964 656f 2074 6f20  of the video to 
+00019510: 7573 6520 666f 7220 6465 7465 726d 696e  use for determin
+00019520: 696e 6720 7769 6474 682e 0a20 2020 203a  ing width..    :
+00019530: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
+00019540: 6e74 5d20 6865 6967 6874 5f70 783a 2048  nt] height_px: H
+00019550: 6569 6768 7420 6f66 2074 6865 206f 7574  eight of the out
+00019560: 7075 7420 7669 6465 6f20 7061 6e65 6c73  put video panels
+00019570: 2069 6e20 7069 7865 6c73 2e0a 2020 2020   in pixels..    
+00019580: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+00019590: 696e 745d 2068 6569 6768 745f 6964 783a  int] height_idx:
+000195a0: 2048 6569 6768 7420 6f66 2074 6865 2076   Height of the v
+000195b0: 6964 656f 2074 6f20 7573 6520 666f 7220  ideo to use for 
+000195c0: 6465 7465 726d 696e 696e 6720 7769 6474  determining widt
+000195d0: 682e 0a20 2020 203a 7061 7261 6d20 4f70  h..    :param Op
+000195e0: 7469 6f6e 616c 5b62 6f6f 6c5d 2067 7075  tional[bool] gpu
+000195f0: 3a20 5768 6574 6865 7220 746f 2075 7365  : Whether to use
+00019600: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
+00019610: 2063 6f64 6563 2028 6465 6661 756c 743a   codec (default:
+00019620: 2046 616c 7365 292e 0a20 2020 203a 7061   False)..    :pa
+00019630: 7261 6d20 4f70 7469 6f6e 616c 5b62 6f6f  ram Optional[boo
+00019640: 6c5d 2076 6572 626f 7365 3a20 5768 6574  l] verbose: Whet
+00019650: 6865 7220 746f 2070 7269 6e74 2070 726f  her to print pro
+00019660: 6772 6573 7320 6d65 7373 6167 6573 2028  gress messages (
+00019670: 6465 6661 756c 743a 2054 7275 6529 2e0a  default: True)..
+00019680: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+00019690: 2020 203e 3e3e 2076 6964 656f 5f70 6174     >>> video_pat
+000196a0: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
+000196b0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+000196c0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+000196d0: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
+000196e0: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+000196f0: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
+00019700: 3231 5f44 4f54 5f52 6174 375f 3828 3229  21_DOT_Rat7_8(2)
+00019710: 2e6d 7034 272c 2027 2f55 7365 7273 2f73  .mp4', '/Users/s
+00019720: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00019730: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00019740: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
+00019750: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
+00019760: 6964 656f 732f 7465 7374 2f30 3831 3032  ideos/test/08102
+00019770: 3032 315f 444f 545f 5261 7431 315f 3132  021_DOT_Rat11_12
+00019780: 2e6d 7034 272c 2027 2f55 7365 7273 2f73  .mp4', '/Users/s
+00019790: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+000197a0: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+000197b0: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
+000197c0: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
+000197d0: 6964 656f 732f 7465 7374 2f6e 6577 2f32  ideos/test/new/2
+000197e0: 3032 322d 3036 2d32 315f 4e4f 425f 494f  022-06-21_NOB_IO
+000197f0: 545f 3233 2e6d 7034 275d 0a20 2020 203e  T_23.mp4'].    >
+00019800: 3e3e 2073 6176 655f 7061 7468 203d 2027  >> save_path = '
+00019810: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00019820: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00019830: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00019840: 5241 545f 4e4f 522f 7072 6f6a 6563 745f  RAT_NOR/project_
+00019850: 666f 6c64 6572 2f76 6964 656f 732f 7465  folder/videos/te
+00019860: 7374 2f6e 6577 2f62 6c61 6e6b 5f74 6573  st/new/blank_tes
+00019870: 742e 6d70 3427 0a20 2020 203e 3e3e 206d  t.mp4'.    >>> m
+00019880: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
+00019890: 6f72 2876 6964 656f 5f70 6174 6873 3d76  or(video_paths=v
+000198a0: 6964 656f 5f70 6174 6873 2c20 7361 7665  ideo_paths, save
+000198b0: 5f70 6174 683d 7361 7665 5f70 6174 682c  _path=save_path,
+000198c0: 2077 6964 7468 5f69 6478 3d31 2c20 6865   width_idx=1, he
+000198d0: 6967 6874 5f69 6478 3d31 2c20 6770 753d  ight_idx=1, gpu=
+000198e0: 4661 6c73 6529 0a20 2020 2022 2222 0a0a  False).    """..
+000198f0: 2020 2020 6368 6563 6b5f 6666 6d70 6567      check_ffmpeg
+00019900: 5f61 7661 696c 6162 6c65 2829 0a20 2020  _available().   
+00019910: 2069 6620 6770 7520 616e 6420 6e6f 7420   if gpu and not 
+00019920: 6368 6563 6b5f 6e76 6964 6561 5f67 7075  check_nvidea_gpu
+00019930: 5f61 7661 696c 6162 6c65 2829 3a0a 2020  _available():.  
+00019940: 2020 2020 2020 7261 6973 6520 4646 4d50        raise FFMP
+00019950: 4547 436f 6465 6347 5055 4572 726f 7228  EGCodecGPUError(
+00019960: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+00019970: 3d22 4e56 4944 4941 2047 5055 206e 6f74  ="NVIDIA GPU not
+00019980: 2061 7661 696c 6162 6c65 222c 2073 6f75   available", sou
+00019990: 7263 653d 6d6f 7361 6963 5f63 6f6e 6361  rce=mosaic_conca
+000199a0: 7465 6e61 746f 722e 5f5f 6e61 6d65 5f5f  tenator.__name__
+000199b0: 0a20 2020 2020 2020 2029 0a20 2020 2074  .        ).    t
+000199c0: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
+000199d0: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
+000199e0: 2020 6474 203d 2064 6174 6574 696d 652e    dt = datetime.
+000199f0: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
+00019a00: 2559 256d 2564 2548 254d 2553 2229 0a20  %Y%m%d%H%M%S"). 
+00019a10: 2020 2063 6865 636b 5f76 616c 6964 5f6c     check_valid_l
+00019a20: 7374 280a 2020 2020 2020 2020 6461 7461  st(.        data
+00019a30: 3d76 6964 656f 5f70 6174 6873 2c0a 2020  =video_paths,.  
+00019a40: 2020 2020 2020 736f 7572 6365 3d66 227b        source=f"{
+00019a50: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
+00019a60: 746f 722e 5f5f 6e61 6d65 5f5f 7d20 7669  tor.__name__} vi
+00019a70: 6465 6f5f 7061 7468 7322 2c0a 2020 2020  deo_paths",.    
+00019a80: 2020 2020 6d69 6e5f 6c65 6e3d 332c 0a20      min_len=3,. 
+00019a90: 2020 2029 0a20 2020 2076 6964 656f 5f6d     ).    video_m
+00019aa0: 6574 615f 6461 7461 203d 205b 0a20 2020  eta_data = [.   
+00019ab0: 2020 2020 2067 6574 5f76 6964 656f 5f6d       get_video_m
+00019ac0: 6574 615f 6461 7461 2876 6964 656f 5f70  eta_data(video_p
+00019ad0: 6174 683d 7669 6465 6f5f 7061 7468 2920  ath=video_path) 
+00019ae0: 666f 7220 7669 6465 6f5f 7061 7468 2069  for video_path i
+00019af0: 6e20 7669 6465 6f5f 7061 7468 730a 2020  n video_paths.  
+00019b00: 2020 5d0a 2020 2020 6d61 785f 7669 6465    ].    max_vide
+00019b10: 6f5f 6c65 6e67 7468 203d 206d 6178 285b  o_length = max([
+00019b20: 785b 2276 6964 656f 5f6c 656e 6774 685f  x["video_length_
+00019b30: 7322 5d20 666f 7220 7820 696e 2076 6964  s"] for x in vid
+00019b40: 656f 5f6d 6574 615f 6461 7461 5d29 0a20  eo_meta_data]). 
+00019b50: 2020 2069 6620 2828 7769 6474 685f 7078     if ((width_px
+00019b60: 2069 7320 4e6f 6e65 2920 616e 6420 2877   is None) and (w
+00019b70: 6964 7468 5f69 6478 2069 7320 4e6f 6e65  idth_idx is None
+00019b80: 2929 206f 7220 280a 2020 2020 2020 2020  )) or (.        
+00019b90: 2877 6964 7468 5f70 7820 6973 206e 6f74  (width_px is not
+00019ba0: 204e 6f6e 6529 2061 6e64 2028 7769 6474   None) and (widt
+00019bb0: 685f 6964 7820 6973 206e 6f74 204e 6f6e  h_idx is not Non
+00019bc0: 6529 0a20 2020 2029 3a0a 2020 2020 2020  e).    ):.      
+00019bd0: 2020 7261 6973 6520 496e 7661 6c69 6449    raise InvalidI
+00019be0: 6e70 7574 4572 726f 7228 0a20 2020 2020  nputError(.     
+00019bf0: 2020 2020 2020 206d 7367 3d22 5072 6f76         msg="Prov
+00019c00: 6964 6520 6120 7769 6474 685f 7078 204f  ide a width_px O
+00019c10: 5220 7769 6474 685f 6964 7822 2c20 736f  R width_idx", so
+00019c20: 7572 6365 3d6d 6f73 6169 635f 636f 6e63  urce=mosaic_conc
+00019c30: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
+00019c40: 5f0a 2020 2020 2020 2020 290a 2020 2020  _.        ).    
+00019c50: 6966 2028 2868 6569 6768 745f 7078 2069  if ((height_px i
+00019c60: 7320 4e6f 6e65 2920 616e 6420 2868 6569  s None) and (hei
+00019c70: 6768 745f 6964 7820 6973 204e 6f6e 6529  ght_idx is None)
+00019c80: 2920 6f72 2028 0a20 2020 2020 2020 2028  ) or (.        (
+00019c90: 6865 6967 6874 5f70 7820 6973 206e 6f74  height_px is not
+00019ca0: 204e 6f6e 6529 2061 6e64 2028 6865 6967   None) and (heig
+00019cb0: 6874 5f69 6478 2069 7320 6e6f 7420 4e6f  ht_idx is not No
+00019cc0: 6e65 290a 2020 2020 293a 0a20 2020 2020  ne).    ):.     
+00019cd0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+00019ce0: 496e 7075 7445 7272 6f72 280a 2020 2020  InputError(.    
+00019cf0: 2020 2020 2020 2020 6d73 673d 2250 726f          msg="Pro
+00019d00: 7669 6465 2061 2068 6569 6768 745f 7078  vide a height_px
+00019d10: 204f 5220 6865 6967 6874 5f69 6478 222c   OR height_idx",
+00019d20: 2073 6f75 7263 653d 6d6f 7361 6963 5f63   source=mosaic_c
+00019d30: 6f6e 6361 7465 6e61 746f 722e 5f5f 6e61  oncatenator.__na
+00019d40: 6d65 5f5f 0a20 2020 2020 2020 2029 0a20  me__.        ). 
+00019d50: 2020 2069 6620 7769 6474 685f 6964 7820     if width_idx 
+00019d60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00019d70: 2020 2020 2063 6865 636b 5f69 6e74 280a       check_int(.
+00019d80: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00019d90: 3d66 227b 7665 7274 6963 616c 5f76 6964  =f"{vertical_vid
+00019da0: 656f 5f63 6f6e 6361 7465 6e61 746f 722e  eo_concatenator.
+00019db0: 5f5f 6e61 6d65 5f5f 7d20 7769 6474 6820  __name__} width 
+00019dc0: 696e 6465 7822 2c0a 2020 2020 2020 2020  index",.        
+00019dd0: 2020 2020 7661 6c75 653d 7769 6474 685f      value=width_
+00019de0: 6964 782c 0a20 2020 2020 2020 2020 2020  idx,.           
+00019df0: 206d 696e 5f76 616c 7565 3d31 2c0a 2020   min_value=1,.  
+00019e00: 2020 2020 2020 2020 2020 6d61 785f 7661            max_va
+00019e10: 6c75 653d 6c65 6e28 7669 6465 6f5f 7061  lue=len(video_pa
+00019e20: 7468 7329 202d 2031 2c0a 2020 2020 2020  ths) - 1,.      
+00019e30: 2020 290a 2020 2020 2020 2020 7769 6474    ).        widt
+00019e40: 6820 3d20 696e 7428 7669 6465 6f5f 6d65  h = int(video_me
+00019e50: 7461 5f64 6174 615b 7769 6474 685f 6964  ta_data[width_id
+00019e60: 785d 5b22 7769 6474 6822 5d29 0a20 2020  x]["width"]).   
+00019e70: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+00019e80: 6964 7468 203d 2077 6964 7468 5f70 780a  idth = width_px.
+00019e90: 2020 2020 6966 2068 6569 6768 745f 6964      if height_id
+00019ea0: 7820 6973 206e 6f74 204e 6f6e 653a 0a20  x is not None:. 
+00019eb0: 2020 2020 2020 2063 6865 636b 5f69 6e74         check_int
+00019ec0: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
+00019ed0: 6d65 3d66 227b 7665 7274 6963 616c 5f76  me=f"{vertical_v
+00019ee0: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
+00019ef0: 722e 5f5f 6e61 6d65 5f5f 7d20 6865 6967  r.__name__} heig
+00019f00: 6874 2069 6e64 6578 222c 0a20 2020 2020  ht index",.     
+00019f10: 2020 2020 2020 2076 616c 7565 3d77 6964         value=wid
+00019f20: 7468 5f69 6478 2c0a 2020 2020 2020 2020  th_idx,.        
+00019f30: 2020 2020 6d69 6e5f 7661 6c75 653d 312c      min_value=1,
+00019f40: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00019f50: 5f76 616c 7565 3d6c 656e 2876 6964 656f  _value=len(video
+00019f60: 5f70 6174 6873 2920 2d20 312c 0a20 2020  _paths) - 1,.   
+00019f70: 2020 2020 2029 0a20 2020 2020 2020 2068       ).        h
+00019f80: 6569 6768 7420 3d20 696e 7428 7669 6465  eight = int(vide
+00019f90: 6f5f 6d65 7461 5f64 6174 615b 7769 6474  o_meta_data[widt
+00019fa0: 685f 6964 785d 5b22 6865 6967 6874 225d  h_idx]["height"]
+00019fb0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00019fc0: 2020 2020 6865 6967 6874 203d 2068 6569      height = hei
+00019fd0: 6768 745f 7078 0a20 2020 2069 6620 7665  ght_px.    if ve
+00019fe0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+00019ff0: 7269 6e74 2866 2243 7265 6174 696e 6720  rint(f"Creating 
+0001a000: 6d6f 7361 6963 2076 6964 656f 202e 2e2e  mosaic video ...
+0001a010: 2229 0a20 2020 2074 656d 705f 6469 7220  ").    temp_dir 
+0001a020: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+0001a030: 732e 7061 7468 2e64 6972 6e61 6d65 2876  s.path.dirname(v
+0001a040: 6964 656f 5f70 6174 6873 5b30 5d29 2c20  ideo_paths[0]), 
+0001a050: 6622 7465 6d70 5f7b 6474 7d22 290a 2020  f"temp_{dt}").  
+0001a060: 2020 6f73 2e6d 616b 6564 6972 7328 7465    os.makedirs(te
+0001a070: 6d70 5f64 6972 290a 2020 2020 6966 206e  mp_dir).    if n
+0001a080: 6f74 2028 6c65 6e28 7669 6465 6f5f 7061  ot (len(video_pa
+0001a090: 7468 7329 2025 2032 2920 3d3d 2030 3a0a  ths) % 2) == 0:.
+0001a0a0: 2020 2020 2020 2020 626c 616e 6b5f 7061          blank_pa
+0001a0b0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+0001a0c0: 6e28 7465 6d70 5f64 6972 2c20 6622 7b64  n(temp_dir, f"{d
+0001a0d0: 747d 2e6d 7034 2229 0a20 2020 2020 2020  t}.mp4").       
+0001a0e0: 2063 7265 6174 655f 626c 616e 6b5f 7669   create_blank_vi
+0001a0f0: 6465 6f28 0a20 2020 2020 2020 2020 2020  deo(.           
+0001a100: 2070 6174 683d 626c 616e 6b5f 7061 7468   path=blank_path
+0001a110: 2c0a 2020 2020 2020 2020 2020 2020 6c65  ,.            le
+0001a120: 6e67 7468 3d6d 6178 5f76 6964 656f 5f6c  ngth=max_video_l
+0001a130: 656e 6774 682c 0a20 2020 2020 2020 2020  ength,.         
+0001a140: 2020 2077 6964 7468 3d77 6964 7468 2c0a     width=width,.
+0001a150: 2020 2020 2020 2020 2020 2020 6865 6967              heig
+0001a160: 6874 3d68 6569 6768 742c 0a20 2020 2020  ht=height,.     
+0001a170: 2020 2020 2020 2067 7075 3d67 7075 2c0a         gpu=gpu,.
+0001a180: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+0001a190: 6f73 653d 7665 7262 6f73 652c 0a20 2020  ose=verbose,.   
+0001a1a0: 2020 2020 2020 2020 2063 6f6c 6f72 3d75           color=u
+0001a1b0: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
+0001a1c0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001a1d0: 2020 2020 7669 6465 6f5f 7061 7468 732e      video_paths.
+0001a1e0: 6170 7065 6e64 2862 6c61 6e6b 5f70 6174  append(blank_pat
+0001a1f0: 6829 0a20 2020 2075 7070 6572 5f76 6964  h).    upper_vid
+0001a200: 656f 732c 206c 6f77 6572 5f76 6964 656f  eos, lower_video
+0001a210: 7320 3d20 280a 2020 2020 2020 2020 7669  s = (.        vi
+0001a220: 6465 6f5f 7061 7468 735b 3a20 6c65 6e28  deo_paths[: len(
+0001a230: 7669 6465 6f5f 7061 7468 7329 202f 2f20  video_paths) // 
+0001a240: 325d 2c0a 2020 2020 2020 2020 7669 6465  2],.        vide
+0001a250: 6f5f 7061 7468 735b 6c65 6e28 7669 6465  o_paths[len(vide
+0001a260: 6f5f 7061 7468 7329 202f 2f20 3220 3a5d  o_paths) // 2 :]
+0001a270: 2c0a 2020 2020 290a 2020 2020 6966 2076  ,.    ).    if v
+0001a280: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0001a290: 7072 696e 7428 2243 7265 6174 696e 6720  print("Creating 
+0001a2a0: 7570 7065 7220 6d6f 7361 6963 2e2e 2e20  upper mosaic... 
+0001a2b0: 2853 7465 7020 312f 3329 2229 0a20 2020  (Step 1/3)").   
+0001a2c0: 2069 6620 6c65 6e28 7570 7065 725f 7669   if len(upper_vi
+0001a2d0: 6465 6f73 2920 3e20 313a 0a20 2020 2020  deos) > 1:.     
+0001a2e0: 2020 2075 7070 6572 5f70 6174 6820 3d20     upper_path = 
+0001a2f0: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
+0001a300: 705f 6469 722c 2022 7570 7065 722e 6d70  p_dir, "upper.mp
+0001a310: 3422 290a 2020 2020 2020 2020 686f 7269  4").        hori
+0001a320: 7a6f 6e74 616c 5f76 6964 656f 5f63 6f6e  zontal_video_con
+0001a330: 6361 7465 6e61 746f 7228 0a20 2020 2020  catenator(.     
+0001a340: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
+0001a350: 6873 3d75 7070 6572 5f76 6964 656f 732c  hs=upper_videos,
+0001a360: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+0001a370: 655f 7061 7468 3d75 7070 6572 5f70 6174  e_path=upper_pat
+0001a380: 682c 0a20 2020 2020 2020 2020 2020 2067  h,.            g
+0001a390: 7075 3d67 7075 2c0a 2020 2020 2020 2020  pu=gpu,.        
+0001a3a0: 2020 2020 6865 6967 6874 5f70 783d 6865      height_px=he
+0001a3b0: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
+0001a3c0: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
+0001a3d0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+0001a3e0: 2065 6c73 653a 0a20 2020 2020 2020 2075   else:.        u
+0001a3f0: 7070 6572 5f70 6174 6820 3d20 7570 7065  pper_path = uppe
+0001a400: 725f 7669 6465 6f73 5b30 5d0a 2020 2020  r_videos[0].    
+0001a410: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0001a420: 2020 2020 7072 696e 7428 2243 7265 6174      print("Creat
+0001a430: 696e 6720 6c6f 7765 7220 6d6f 7361 6963  ing lower mosaic
+0001a440: 2e2e 2e20 2853 7465 7020 322f 3329 2229  ... (Step 2/3)")
+0001a450: 0a20 2020 2069 6620 6c65 6e28 6c6f 7765  .    if len(lowe
+0001a460: 725f 7669 6465 6f73 2920 3e20 313a 0a20  r_videos) > 1:. 
+0001a470: 2020 2020 2020 206c 6f77 6572 5f70 6174         lower_pat
+0001a480: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+0001a490: 2874 656d 705f 6469 722c 2022 6c6f 7765  (temp_dir, "lowe
+0001a4a0: 722e 6d70 3422 290a 2020 2020 2020 2020  r.mp4").        
+0001a4b0: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
+0001a4c0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
+0001a4d0: 2020 2020 2020 2020 2020 2076 6964 656f             video
+0001a4e0: 5f70 6174 6873 3d6c 6f77 6572 5f76 6964  _paths=lower_vid
+0001a4f0: 656f 732c 0a20 2020 2020 2020 2020 2020  eos,.           
+0001a500: 2073 6176 655f 7061 7468 3d6c 6f77 6572   save_path=lower
+0001a510: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0001a520: 2020 2067 7075 3d67 7075 2c0a 2020 2020     gpu=gpu,.    
+0001a530: 2020 2020 2020 2020 6865 6967 6874 5f70          height_p
+0001a540: 783d 6865 6967 6874 2c0a 2020 2020 2020  x=height,.      
+0001a550: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
+0001a560: 7262 6f73 652c 0a20 2020 2020 2020 2029  rbose,.        )
+0001a570: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0001a580: 2020 206c 6f77 6572 5f70 6174 6820 3d20     lower_path = 
+0001a590: 6c6f 7765 725f 7669 6465 6f73 5b30 5d0a  lower_videos[0].
+0001a5a0: 2020 2020 7061 6e65 6c73 5f6d 6574 6120      panels_meta 
+0001a5b0: 3d20 5b0a 2020 2020 2020 2020 6765 745f  = [.        get_
+0001a5c0: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
+0001a5d0: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
+0001a5e0: 5f70 6174 6829 0a20 2020 2020 2020 2066  _path).        f
+0001a5f0: 6f72 2076 6964 656f 5f70 6174 6820 696e  or video_path in
+0001a600: 205b 6c6f 7765 725f 7061 7468 2c20 7570   [lower_path, up
+0001a610: 7065 725f 7061 7468 5d0a 2020 2020 5d0a  per_path].    ].
+0001a620: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0001a630: 2020 2020 2020 2020 7072 696e 7428 224a          print("J
+0001a640: 6f69 6e69 6e67 2075 7070 6572 2061 6e64  oining upper and
+0001a650: 206c 6f77 6572 206d 6f73 6169 632e 2e2e   lower mosaic...
+0001a660: 2028 5374 6570 2032 2f33 2922 290a 2020   (Step 2/3)").  
+0001a670: 2020 7665 7274 6963 616c 5f76 6964 656f    vertical_video
+0001a680: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
+0001a690: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
+0001a6a0: 6873 3d5b 7570 7065 725f 7061 7468 2c20  hs=[upper_path, 
+0001a6b0: 6c6f 7765 725f 7061 7468 5d2c 0a20 2020  lower_path],.   
+0001a6c0: 2020 2020 2073 6176 655f 7061 7468 3d73       save_path=s
+0001a6d0: 6176 655f 7061 7468 2c0a 2020 2020 2020  ave_path,.      
+0001a6e0: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
+0001a6f0: 652c 0a20 2020 2020 2020 2067 7075 3d67  e,.        gpu=g
+0001a700: 7075 2c0a 2020 2020 2020 2020 7769 6474  pu,.        widt
+0001a710: 685f 7078 3d6d 6178 285b 785b 2277 6964  h_px=max([x["wid
+0001a720: 7468 225d 2066 6f72 2078 2069 6e20 7061  th"] for x in pa
+0001a730: 6e65 6c73 5f6d 6574 615d 292c 0a20 2020  nels_meta]),.   
+0001a740: 2029 0a20 2020 2074 696d 6572 2e73 746f   ).    timer.sto
+0001a750: 705f 7469 6d65 7228 290a 2020 2020 7368  p_timer().    sh
+0001a760: 7574 696c 2e72 6d74 7265 6528 7465 6d70  util.rmtree(temp
+0001a770: 5f64 6972 290a 2020 2020 6966 2076 6572  _dir).    if ver
+0001a780: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
+0001a790: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0001a7a0: 2066 224d 6f73 6169 6320 636f 6e63 6174   f"Mosaic concat
+0001a7b0: 656e 6174 696f 6e20 636f 6d70 6c65 7465  enation complete
+0001a7c0: 2e20 5361 7665 6420 6174 207b 7361 7665  . Saved at {save
+0001a7d0: 5f70 6174 687d 2028 456c 6170 7365 6420  _path} (Elapsed 
+0001a7e0: 7469 6d65 3a20 7b74 696d 6572 2e65 6c61  time: {timer.ela
+0001a7f0: 7073 6564 5f74 696d 655f 7374 727d 732e  psed_time_str}s.
+0001a800: 2922 0a20 2020 2020 2020 2029 0a0a 0a64  )".        )...d
+0001a810: 6566 206d 6978 6564 5f6d 6f73 6169 635f  ef mixed_mosaic_
+0001a820: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
+0001a830: 2020 7669 6465 6f5f 7061 7468 733a 204c    video_paths: L
+0001a840: 6973 745b 556e 696f 6e5b 7374 722c 206f  ist[Union[str, o
+0001a850: 732e 5061 7468 4c69 6b65 5d5d 2c0a 2020  s.PathLike]],.  
+0001a860: 2020 7361 7665 5f70 6174 683a 2055 6e69    save_path: Uni
+0001a870: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0001a880: 696b 655d 2c0a 2020 2020 6770 753a 204f  ike],.    gpu: O
+0001a890: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001a8a0: 4661 6c73 652c 0a20 2020 2076 6572 626f  False,.    verbo
+0001a8b0: 7365 3a20 4f70 7469 6f6e 616c 5b62 6f6f  se: Optional[boo
+0001a8c0: 6c5d 203d 2054 7275 652c 0a20 2020 2075  l] = True,.    u
+0001a8d0: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
+0001a8e0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0001a8f0: 3d20 2262 6c61 636b 222c 0a29 202d 3e20  = "black",.) -> 
+0001a900: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+0001a910: 2020 4372 6561 7465 2061 206d 6978 6564    Create a mixed
+0001a920: 206d 6f73 6169 6320 7669 6465 6f20 6279   mosaic video by
+0001a930: 2063 6f6e 6361 7465 6e61 7469 6e67 206d   concatenating m
+0001a940: 756c 7469 706c 6520 696e 7075 7420 7669  ultiple input vi
+0001a950: 6465 6f73 2069 6e20 6120 6d6f 7361 6963  deos in a mosaic
+0001a960: 206c 6179 6f75 7420 6f66 2076 6172 696f   layout of vario
+0001a970: 7573 2073 697a 6573 2e0a 0a20 2020 202e  us sizes...    .
+0001a980: 2e20 696d 6167 653a 3a20 5f73 7461 7469  . image:: _stati
+0001a990: 632f 696d 672f 6d69 7865 645f 6d6f 7361  c/img/mixed_mosa
+0001a9a0: 6963 5f63 6f6e 6361 7465 6e61 746f 722e  ic_concatenator.
+0001a9b0: 706e 670a 2020 2020 2020 203a 7769 6474  png.       :widt
+0001a9c0: 683a 2036 3030 0a20 2020 2020 2020 3a61  h: 600.       :a
+0001a9d0: 6c69 676e 3a20 6365 6e74 6572 0a0a 2020  lign: center..  
+0001a9e0: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+0001a9f0: 2020 2054 6865 2072 6573 6f6c 7574 696f     The resolutio
+0001aa00: 6e20 6f66 2074 6865 206f 7574 7075 7420  n of the output 
+0001aa10: 7669 6465 6f20 6973 2064 6574 6572 6d69  video is determi
+0001aa20: 6e65 6420 6279 2074 6865 2072 6573 6f6c  ned by the resol
+0001aa30: 7574 696f 6e20 6f66 2074 6865 2076 6964  ution of the vid
+0001aa40: 656f 2070 6174 6820 6174 2074 6865 2066  eo path at the f
+0001aa50: 6972 7374 2069 6e64 6578 2e0a 0a20 2020  irst index...   
+0001aa60: 2020 2020 4966 2061 6e20 756e 6576 656e      If an uneven
+0001aa70: 206e 756d 6265 7220 6f66 2072 6967 6874   number of right
+0001aa80: 2d70 616e 656c 2076 6964 656f 7320 2820  -panel videos ( 
+0001aa90: 6966 206e 6f74 2028 6c65 6e28 7669 6465  if not (len(vide
+0001aaa0: 6f5f 7061 7468 7329 2d31 2920 2520 3229  o_paths)-1) % 2)
+0001aab0: 203d 3d20 3029 2c20 7468 656e 2074 6865   == 0), then the
+0001aac0: 206c 6173 7420 696e 6465 7820 7769 6c6c   last index will
+0001aad0: 2062 6520 6669 6c6c 6564 2062 7920 6060   be filled by ``
+0001aae0: 756e 6576 656e 5f66 696c 6c5f 636f 6c6f  uneven_fill_colo
+0001aaf0: 7260 602e 0a0a 2020 2020 3a70 6172 616d  r``...    :param
+0001ab00: 204c 6973 745b 556e 696f 6e5b 7374 722c   List[Union[str,
+0001ab10: 206f 732e 5061 7468 4c69 6b65 5d5d 2076   os.PathLike]] v
+0001ab20: 6964 656f 5f70 6174 6873 3a20 4c69 7374  ideo_paths: List
+0001ab30: 206f 6620 696e 7075 7420 7669 6465 6f20   of input video 
+0001ab40: 6669 6c65 2070 6174 6873 2e0a 2020 2020  file paths..    
+0001ab50: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
+0001ab60: 2c20 6f73 2e50 6174 684c 696b 655d 2073  , os.PathLike] s
+0001ab70: 6176 655f 7061 7468 3a20 4669 6c65 2070  ave_path: File p
+0001ab80: 6174 6820 746f 2073 6176 6520 7468 6520  ath to save the 
+0001ab90: 636f 6e63 6174 656e 6174 6564 2076 6964  concatenated vid
+0001aba0: 656f 2e0a 2020 2020 3a70 6172 616d 204f  eo..    :param O
+0001abb0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 6770  ptional[bool] gp
+0001abc0: 753a 2057 6865 7468 6572 2074 6f20 7573  u: Whether to us
+0001abd0: 6520 4750 552d 6163 6365 6c65 7261 7465  e GPU-accelerate
+0001abe0: 6420 636f 6465 6320 2864 6566 6175 6c74  d codec (default
+0001abf0: 3a20 4661 6c73 6529 2e0a 2020 2020 3a70  : False)..    :p
+0001ac00: 6172 616d 204f 7074 696f 6e61 6c5b 626f  aram Optional[bo
+0001ac10: 6f6c 5d20 7665 7262 6f73 653a 2057 6865  ol] verbose: Whe
+0001ac20: 7468 6572 2074 6f20 7072 696e 7420 7072  ther to print pr
+0001ac30: 6f67 7265 7373 206d 6573 7361 6765 7320  ogress messages 
+0001ac40: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
+0001ac50: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
+0001ac60: 2020 2020 3e3e 3e20 7669 6465 6f5f 7061      >>> video_pa
+0001ac70: 7468 7320 3d20 5b27 7669 6465 6f31 2e6d  ths = ['video1.m
+0001ac80: 7034 272c 2027 7669 6465 6f32 2e6d 7034  p4', 'video2.mp4
+0001ac90: 272c 2027 7669 6465 6f33 2e6d 7034 275d  ', 'video3.mp4']
+0001aca0: 0a20 2020 203e 3e3e 2073 6176 655f 7061  .    >>> save_pa
+0001acb0: 7468 203d 2027 2f55 7365 7273 2f73 696d  th = '/Users/sim
+0001acc0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+0001acd0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+0001ace0: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
+0001acf0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+0001ad00: 656f 732f 7465 7374 2f6e 6577 2f62 6c61  eos/test/new/bla
+0001ad10: 6e6b 5f74 6573 742e 6d70 3427 0a20 2020  nk_test.mp4'.   
+0001ad20: 203e 3e3e 206d 6978 6564 5f6d 6f73 6169   >>> mixed_mosai
+0001ad30: 635f 636f 6e63 6174 656e 6174 6f72 2876  c_concatenator(v
+0001ad40: 6964 656f 5f70 6174 6873 3d76 6964 656f  ideo_paths=video
+0001ad50: 5f70 6174 6873 2c20 7361 7665 5f70 6174  _paths, save_pat
+0001ad60: 683d 7361 7665 5f70 6174 682c 2067 7075  h=save_path, gpu
+0001ad70: 3d46 616c 7365 2c20 7665 7262 6f73 653d  =False, verbose=
+0001ad80: 5472 7565 290a 2020 2020 2222 220a 0a20  True).    """.. 
+0001ad90: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
+0001ada0: 6176 6169 6c61 626c 6528 290a 2020 2020  available().    
+0001adb0: 6966 2067 7075 2061 6e64 206e 6f74 2063  if gpu and not c
+0001adc0: 6865 636b 5f6e 7669 6465 615f 6770 755f  heck_nvidea_gpu_
+0001add0: 6176 6169 6c61 626c 6528 293a 0a20 2020  available():.   
+0001ade0: 2020 2020 2072 6169 7365 2046 464d 5045       raise FFMPE
+0001adf0: 4743 6f64 6563 4750 5545 7272 6f72 280a  GCodecGPUError(.
+0001ae00: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+0001ae10: 224e 5649 4449 4120 4750 5520 6e6f 7420  "NVIDIA GPU not 
+0001ae20: 6176 6169 6c61 626c 6522 2c20 736f 7572  available", sour
+0001ae30: 6365 3d6d 6978 6564 5f6d 6f73 6169 635f  ce=mixed_mosaic_
+0001ae40: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
+0001ae50: 616d 655f 5f0a 2020 2020 2020 2020 290a  ame__.        ).
+0001ae60: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
+0001ae70: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
+0001ae80: 6529 0a20 2020 2063 6865 636b 5f76 616c  e).    check_val
+0001ae90: 6964 5f6c 7374 280a 2020 2020 2020 2020  id_lst(.        
+0001aea0: 6461 7461 3d76 6964 656f 5f70 6174 6873  data=video_paths
+0001aeb0: 2c20 736f 7572 6365 3d6d 6978 6564 5f6d  , source=mixed_m
+0001aec0: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
+0001aed0: 6f72 2e5f 5f6e 616d 655f 5f2c 206d 696e  or.__name__, min
+0001aee0: 5f6c 656e 3d32 0a20 2020 2029 0a20 2020  _len=2.    ).   
+0001aef0: 2064 7420 3d20 6461 7465 7469 6d65 2e6e   dt = datetime.n
+0001af00: 6f77 2829 2e73 7472 6674 696d 6528 2225  ow().strftime("%
+0001af10: 5925 6d25 6425 4825 4d25 5322 290a 2020  Y%m%d%H%M%S").  
+0001af20: 2020 7669 6465 6f5f 6d65 7461 5f64 6174    video_meta_dat
+0001af30: 6120 3d20 5b0a 2020 2020 2020 2020 6765  a = [.        ge
+0001af40: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
+0001af50: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
+0001af60: 656f 5f70 6174 6829 2066 6f72 2076 6964  eo_path) for vid
+0001af70: 656f 5f70 6174 6820 696e 2076 6964 656f  eo_path in video
+0001af80: 5f70 6174 6873 0a20 2020 205d 0a20 2020  _paths.    ].   
+0001af90: 206d 6178 5f76 6964 656f 5f6c 656e 6774   max_video_lengt
+0001afa0: 6820 3d20 6d61 7828 5b78 5b22 7669 6465  h = max([x["vide
+0001afb0: 6f5f 6c65 6e67 7468 5f73 225d 2066 6f72  o_length_s"] for
+0001afc0: 2078 2069 6e20 7669 6465 6f5f 6d65 7461   x in video_meta
+0001afd0: 5f64 6174 615d 290a 2020 2020 6368 6563  _data]).    chec
+0001afe0: 6b5f 6966 5f64 6972 5f65 7869 7374 7328  k_if_dir_exists(
+0001aff0: 0a20 2020 2020 2020 2069 6e5f 6469 723d  .        in_dir=
+0001b000: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0001b010: 7361 7665 5f70 6174 6829 2c20 736f 7572  save_path), sour
+0001b020: 6365 3d6d 6978 6564 5f6d 6f73 6169 635f  ce=mixed_mosaic_
+0001b030: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
+0001b040: 616d 655f 5f0a 2020 2020 290a 2020 2020  ame__.    ).    
+0001b050: 6c61 7267 655f 6d6f 7361 6963 5f70 6174  large_mosaic_pat
+0001b060: 682c 2076 6964 656f 5f70 6174 6873 203d  h, video_paths =
+0001b070: 2076 6964 656f 5f70 6174 6873 5b30 5d2c   video_paths[0],
+0001b080: 2076 6964 656f 5f70 6174 6873 5b31 3a5d   video_paths[1:]
+0001b090: 0a20 2020 206d 6f73 6169 635f 6865 6967  .    mosaic_heig
+0001b0a0: 6874 203d 2069 6e74 2876 6964 656f 5f6d  ht = int(video_m
+0001b0b0: 6574 615f 6461 7461 5b30 5d5b 2268 6569  eta_data[0]["hei
+0001b0c0: 6768 7422 5d20 2f20 3229 0a20 2020 2069  ght"] / 2).    i
+0001b0d0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0001b0e0: 2020 2070 7269 6e74 2822 4372 6561 7469     print("Creati
+0001b0f0: 6e67 206d 6978 6564 206d 6f73 6169 6320  ng mixed mosaic 
+0001b100: 7669 6465 6f2e 2e2e 2022 290a 2020 2020  video... ").    
+0001b110: 7465 6d70 5f64 6972 203d 206f 732e 7061  temp_dir = os.pa
+0001b120: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
+0001b130: 6469 726e 616d 6528 6c61 7267 655f 6d6f  dirname(large_mo
+0001b140: 7361 6963 5f70 6174 6829 2c20 6622 7465  saic_path), f"te
+0001b150: 6d70 5f7b 6474 7d22 290a 2020 2020 6f73  mp_{dt}").    os
+0001b160: 2e6d 616b 6564 6972 7328 7465 6d70 5f64  .makedirs(temp_d
+0001b170: 6972 290a 2020 2020 6966 206e 6f74 2028  ir).    if not (
+0001b180: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
+0001b190: 2025 2032 2920 3d3d 2030 3a0a 2020 2020   % 2) == 0:.    
+0001b1a0: 2020 2020 626c 616e 6b5f 7061 7468 203d      blank_path =
+0001b1b0: 206f 732e 7061 7468 2e6a 6f69 6e28 7465   os.path.join(te
+0001b1c0: 6d70 5f64 6972 2c20 6622 7b64 747d 2e6d  mp_dir, f"{dt}.m
+0001b1d0: 7034 2229 0a20 2020 2020 2020 2063 7265  p4").        cre
+0001b1e0: 6174 655f 626c 616e 6b5f 7669 6465 6f28  ate_blank_video(
+0001b1f0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+0001b200: 683d 626c 616e 6b5f 7061 7468 2c0a 2020  h=blank_path,.  
+0001b210: 2020 2020 2020 2020 2020 6c65 6e67 7468            length
+0001b220: 3d6d 6178 5f76 6964 656f 5f6c 656e 6774  =max_video_lengt
+0001b230: 682c 0a20 2020 2020 2020 2020 2020 2077  h,.            w
+0001b240: 6964 7468 3d67 6574 5f76 6964 656f 5f6d  idth=get_video_m
+0001b250: 6574 615f 6461 7461 2876 6964 656f 5f70  eta_data(video_p
+0001b260: 6174 683d 7669 6465 6f5f 7061 7468 735b  ath=video_paths[
+0001b270: 2d31 5d29 5b22 7769 6474 6822 5d2c 0a20  -1])["width"],. 
+0001b280: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0001b290: 743d 6765 745f 7669 6465 6f5f 6d65 7461  t=get_video_meta
+0001b2a0: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
+0001b2b0: 3d76 6964 656f 5f70 6174 6873 5b2d 315d  =video_paths[-1]
+0001b2c0: 295b 2268 6569 6768 7422 5d2c 0a20 2020  )["height"],.   
+0001b2d0: 2020 2020 2020 2020 2067 7075 3d67 7075           gpu=gpu
+0001b2e0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+0001b2f0: 7262 6f73 653d 5472 7565 2c0a 2020 2020  rbose=True,.    
+0001b300: 2020 2020 2020 2020 636f 6c6f 723d 756e          color=un
+0001b310: 6576 656e 5f66 696c 6c5f 636f 6c6f 722c  even_fill_color,
+0001b320: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001b330: 2020 2076 6964 656f 5f70 6174 6873 2e61     video_paths.a
+0001b340: 7070 656e 6428 626c 616e 6b5f 7061 7468  ppend(blank_path
+0001b350: 290a 2020 2020 7570 7065 725f 7669 6465  ).    upper_vide
+0001b360: 6f73 2c20 6c6f 7765 725f 7669 6465 6f73  os, lower_videos
+0001b370: 203d 2028 0a20 2020 2020 2020 2076 6964   = (.        vid
+0001b380: 656f 5f70 6174 6873 5b3a 206c 656e 2876  eo_paths[: len(v
+0001b390: 6964 656f 5f70 6174 6873 2920 2f2f 2032  ideo_paths) // 2
+0001b3a0: 5d2c 0a20 2020 2020 2020 2076 6964 656f  ],.        video
+0001b3b0: 5f70 6174 6873 5b6c 656e 2876 6964 656f  _paths[len(video
+0001b3c0: 5f70 6174 6873 2920 2f2f 2032 203a 5d2c  _paths) // 2 :],
+0001b3d0: 0a20 2020 2029 0a20 2020 2069 6620 7665  .    ).    if ve
+0001b3e0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+0001b3f0: 7269 6e74 2822 4372 6561 7469 6e67 2075  rint("Creating u
+0001b400: 7070 6572 2072 6967 6874 206d 6f73 6169  pper right mosai
+0001b410: 6320 2e2e 2e20 2853 7465 7020 312f 3429  c ... (Step 1/4)
+0001b420: 2229 0a20 2020 2069 6620 6c65 6e28 7570  ").    if len(up
+0001b430: 7065 725f 7669 6465 6f73 2920 3e20 313a  per_videos) > 1:
+0001b440: 0a20 2020 2020 2020 2075 7070 6572 5f70  .        upper_p
+0001b450: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+0001b460: 696e 2874 656d 705f 6469 722c 2022 7570  in(temp_dir, "up
+0001b470: 7065 722e 6d70 3422 290a 2020 2020 2020  per.mp4").      
+0001b480: 2020 686f 7269 7a6f 6e74 616c 5f76 6964    horizontal_vid
+0001b490: 656f 5f63 6f6e 6361 7465 6e61 746f 7228  eo_concatenator(
+0001b4a0: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
+0001b4b0: 656f 5f70 6174 6873 3d75 7070 6572 5f76  eo_paths=upper_v
+0001b4c0: 6964 656f 732c 0a20 2020 2020 2020 2020  ideos,.         
+0001b4d0: 2020 2073 6176 655f 7061 7468 3d75 7070     save_path=upp
+0001b4e0: 6572 5f70 6174 682c 0a20 2020 2020 2020  er_path,.       
+0001b4f0: 2020 2020 2067 7075 3d67 7075 2c0a 2020       gpu=gpu,.  
+0001b500: 2020 2020 2020 2020 2020 6865 6967 6874            height
+0001b510: 5f70 783d 6d6f 7361 6963 5f68 6569 6768  _px=mosaic_heigh
+0001b520: 742c 0a20 2020 2020 2020 2020 2020 2076  t,.            v
+0001b530: 6572 626f 7365 3d76 6572 626f 7365 2c0a  erbose=verbose,.
+0001b540: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
+0001b550: 7365 3a0a 2020 2020 2020 2020 7570 7065  se:.        uppe
+0001b560: 725f 7061 7468 203d 2075 7070 6572 5f76  r_path = upper_v
+0001b570: 6964 656f 735b 305d 0a20 2020 2069 6620  ideos[0].    if 
+0001b580: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+0001b590: 2070 7269 6e74 2822 4372 6561 7469 6e67   print("Creating
+0001b5a0: 206c 6f77 6572 2072 6967 6874 206d 6f73   lower right mos
+0001b5b0: 6169 6320 2e2e 2e20 2853 7465 7020 322f  aic ... (Step 2/
+0001b5c0: 3429 2229 0a20 2020 2069 6620 6c65 6e28  4)").    if len(
+0001b5d0: 6c6f 7765 725f 7669 6465 6f73 2920 3e20  lower_videos) > 
+0001b5e0: 313a 0a20 2020 2020 2020 206c 6f77 6572  1:.        lower
+0001b5f0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+0001b600: 6a6f 696e 2874 656d 705f 6469 722c 2022  join(temp_dir, "
+0001b610: 6c6f 7765 722e 6d70 3422 290a 2020 2020  lower.mp4").    
+0001b620: 2020 2020 686f 7269 7a6f 6e74 616c 5f76      horizontal_v
+0001b630: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
+0001b640: 7228 0a20 2020 2020 2020 2020 2020 2076  r(.            v
+0001b650: 6964 656f 5f70 6174 6873 3d6c 6f77 6572  ideo_paths=lower
+0001b660: 5f76 6964 656f 732c 0a20 2020 2020 2020  _videos,.       
+0001b670: 2020 2020 2073 6176 655f 7061 7468 3d6c       save_path=l
+0001b680: 6f77 6572 5f70 6174 682c 0a20 2020 2020  ower_path,.     
+0001b690: 2020 2020 2020 2067 7075 3d67 7075 2c0a         gpu=gpu,.
+0001b6a0: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+0001b6b0: 6f73 653d 7665 7262 6f73 652c 0a20 2020  ose=verbose,.   
+0001b6c0: 2020 2020 2020 2020 2068 6569 6768 745f           height_
+0001b6d0: 7078 3d6d 6f73 6169 635f 6865 6967 6874  px=mosaic_height
+0001b6e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001b6f0: 656c 7365 3a0a 2020 2020 2020 2020 6c6f  else:.        lo
+0001b700: 7765 725f 7061 7468 203d 206c 6f77 6572  wer_path = lower
+0001b710: 5f76 6964 656f 735b 305d 0a20 2020 2070  _videos[0].    p
+0001b720: 616e 656c 735f 6d65 7461 203d 205b 0a20  anels_meta = [. 
+0001b730: 2020 2020 2020 2067 6574 5f76 6964 656f         get_video
+0001b740: 5f6d 6574 615f 6461 7461 2876 6964 656f  _meta_data(video
+0001b750: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
+0001b760: 290a 2020 2020 2020 2020 666f 7220 7669  ).        for vi
+0001b770: 6465 6f5f 7061 7468 2069 6e20 5b6c 6f77  deo_path in [low
+0001b780: 6572 5f70 6174 682c 2075 7070 6572 5f70  er_path, upper_p
+0001b790: 6174 685d 0a20 2020 205d 0a20 2020 206d  ath].    ].    m
+0001b7a0: 6f73 6169 635f 7061 7468 203d 206f 732e  osaic_path = os.
+0001b7b0: 7061 7468 2e6a 6f69 6e28 7465 6d70 5f64  path.join(temp_d
+0001b7c0: 6972 2c20 226d 6f73 6169 632e 6d70 3422  ir, "mosaic.mp4"
+0001b7d0: 290a 2020 2020 6966 2076 6572 626f 7365  ).    if verbose
+0001b7e0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+0001b7f0: 224a 6f69 6e69 6e67 2075 7070 6572 2061  "Joining upper a
+0001b800: 6e64 206c 6f77 6572 2072 6967 6874 206d  nd lower right m
+0001b810: 6f73 6169 632e 2e2e 2028 5374 6570 2033  osaic... (Step 3
+0001b820: 2f34 2922 290a 2020 2020 7665 7274 6963  /4)").    vertic
+0001b830: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
+0001b840: 6e61 746f 7228 0a20 2020 2020 2020 2076  nator(.        v
+0001b850: 6964 656f 5f70 6174 6873 3d5b 7570 7065  ideo_paths=[uppe
+0001b860: 725f 7061 7468 2c20 6c6f 7765 725f 7061  r_path, lower_pa
+0001b870: 7468 5d2c 0a20 2020 2020 2020 2077 6964  th],.        wid
+0001b880: 7468 5f70 783d 6d61 7828 5b78 5b22 7769  th_px=max([x["wi
+0001b890: 6474 6822 5d20 666f 7220 7820 696e 2070  dth"] for x in p
+0001b8a0: 616e 656c 735f 6d65 7461 5d29 2c0a 2020  anels_meta]),.  
+0001b8b0: 2020 2020 2020 7361 7665 5f70 6174 683d        save_path=
+0001b8c0: 6d6f 7361 6963 5f70 6174 682c 0a20 2020  mosaic_path,.   
+0001b8d0: 2020 2020 2067 7075 3d67 7075 2c0a 2020       gpu=gpu,.  
+0001b8e0: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
+0001b8f0: 7262 6f73 652c 0a20 2020 2029 0a20 2020  rbose,.    ).   
+0001b900: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
+0001b910: 2020 2020 2070 7269 6e74 2822 4a6f 696e       print("Join
+0001b920: 696e 6720 6c65 6674 2061 6e64 2072 6967  ing left and rig
+0001b930: 6874 206d 6f73 6169 632e 2e2e 2028 5374  ht mosaic... (St
+0001b940: 6570 2034 2f34 2922 290a 2020 2020 686f  ep 4/4)").    ho
+0001b950: 7269 7a6f 6e74 616c 5f76 6964 656f 5f63  rizontal_video_c
+0001b960: 6f6e 6361 7465 6e61 746f 7228 0a20 2020  oncatenator(.   
+0001b970: 2020 2020 2076 6964 656f 5f70 6174 6873       video_paths
+0001b980: 3d5b 6c61 7267 655f 6d6f 7361 6963 5f70  =[large_mosaic_p
+0001b990: 6174 682c 206d 6f73 6169 635f 7061 7468  ath, mosaic_path
+0001b9a0: 5d2c 0a20 2020 2020 2020 2068 6569 6768  ],.        heigh
+0001b9b0: 745f 6964 783d 302c 0a20 2020 2020 2020  t_idx=0,.       
+0001b9c0: 2073 6176 655f 7061 7468 3d73 6176 655f   save_path=save_
+0001b9d0: 7061 7468 2c0a 2020 2020 2020 2020 6770  path,.        gp
+0001b9e0: 753d 6770 752c 0a20 2020 2029 0a20 2020  u=gpu,.    ).   
+0001b9f0: 2074 696d 6572 2e73 746f 705f 7469 6d65   timer.stop_time
+0001ba00: 7228 290a 2020 2020 7368 7574 696c 2e72  r().    shutil.r
+0001ba10: 6d74 7265 6528 7465 6d70 5f64 6972 290a  mtree(temp_dir).
+0001ba20: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0001ba30: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+0001ba40: 2020 2020 2020 2020 2020 2066 224d 6978             f"Mix
+0001ba50: 6564 206d 6f73 6169 6320 636f 6e63 6174  ed mosaic concat
+0001ba60: 656e 6174 696f 6e20 636f 6d70 6c65 7465  enation complete
+0001ba70: 2e20 5361 7665 6420 6174 207b 7361 7665  . Saved at {save
+0001ba80: 5f70 6174 687d 2028 456c 6170 7365 6420  _path} (Elapsed 
+0001ba90: 7469 6d65 3a20 7b74 696d 6572 2e65 6c61  time: {timer.ela
+0001baa0: 7073 6564 5f74 696d 655f 7374 727d 732e  psed_time_str}s.
+0001bab0: 2922 0a20 2020 2020 2020 2029 0a0a 0a64  )".        )...d
+0001bac0: 6566 2063 6c69 705f 7669 6465 6f73 5f62  ef clip_videos_b
+0001bad0: 795f 6672 616d 655f 6964 7328 0a20 2020  y_frame_ids(.   
+0001bae0: 2066 696c 655f 7061 7468 733a 204c 6973   file_paths: Lis
+0001baf0: 745b 556e 696f 6e5b 7374 722c 206f 732e  t[Union[str, os.
+0001bb00: 5061 7468 4c69 6b65 5d5d 2c0a 2020 2020  PathLike]],.    
+0001bb10: 6672 6d5f 6964 733a 204c 6973 745b 4c69  frm_ids: List[Li
+0001bb20: 7374 5b69 6e74 5d5d 2c0a 2020 2020 7361  st[int]],.    sa
+0001bb30: 7665 5f64 6972 3a20 4f70 7469 6f6e 616c  ve_dir: Optional
+0001bb40: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
+0001bb50: 6174 684c 696b 655d 5d20 3d20 4e6f 6e65  athLike]] = None
+0001bb60: 2c0a 293a 0a20 2020 2022 2222 0a20 2020  ,.):.    """.   
+0001bb70: 2043 6c69 7020 7669 6465 6f73 2073 7065   Clip videos spe
+0001bb80: 6369 6669 6564 2062 7920 6672 616d 6520  cified by frame 
+0001bb90: 4944 7320 286e 756d 6265 7273 292e 0a0a  IDs (numbers)...
+0001bba0: 2020 2020 3a70 6172 616d 204c 6973 745b      :param List[
+0001bbb0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+0001bbc0: 7468 4c69 6b65 5d5d 2066 696c 655f 7061  thLike]] file_pa
+0001bbd0: 7468 733a 204c 6973 7420 6f66 2070 6174  ths: List of pat
+0001bbe0: 6873 2074 6f20 696e 7075 7420 7669 6465  hs to input vide
+0001bbf0: 6f20 6669 6c65 732e 0a20 2020 203a 7061  o files..    :pa
+0001bc00: 7261 6d20 4c69 7374 5b4c 6973 745b 696e  ram List[List[in
+0001bc10: 745d 5d20 6672 6d5f 6964 733a 204c 6973  t]] frm_ids: Lis
+0001bc20: 7420 6f66 206c 6973 7473 2063 6f6e 7461  t of lists conta
+0001bc30: 696e 696e 6720 7374 6172 7420 616e 6420  ining start and 
+0001bc40: 656e 6420 6672 616d 6520 4944 7320 666f  end frame IDs fo
+0001bc50: 7220 6561 6368 2076 6964 656f 2e0a 2020  r each video..  
+0001bc60: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+0001bc70: 6c5b 556e 696f 6e5b 7374 722c 206f 732e  l[Union[str, os.
+0001bc80: 5061 7468 4c69 6b65 5d5d 2073 6176 655f  PathLike]] save_
+0001bc90: 6469 723a 2020 4469 7265 6374 6f72 7920  dir:  Directory 
+0001bca0: 746f 2073 6176 6520 7468 6520 636c 6970  to save the clip
+0001bcb0: 7065 6420 7669 6465 6f73 2e20 4966 204e  ped videos. If N
+0001bcc0: 6f6e 652c 2076 6964 656f 7320 7769 6c6c  one, videos will
+0001bcd0: 2062 6520 7361 7665 6420 696e 2074 6865   be saved in the
+0001bce0: 2073 616d 6520 6469 7265 6374 6f72 7920   same directory 
+0001bcf0: 6173 2074 6865 2069 6e70 7574 2076 6964  as the input vid
+0001bd00: 656f 7320 7769 7468 2066 7261 6d65 206e  eos with frame n
+0001bd10: 756d 6265 7273 2061 7320 7375 6666 6978  umbers as suffix
+0001bd20: 2e0a 2020 2020 3a72 6574 7572 6e3a 204e  ..    :return: N
+0001bd30: 6f6e 652e 0a0a 2020 2020 3a65 7861 6d70  one...    :examp
+0001bd40: 6c65 3a0a 2020 2020 3e3e 3e20 6669 6c65  le:.    >>> file
+0001bd50: 5f70 6174 6873 203d 205b 272f 5573 6572  _paths = ['/User
+0001bd60: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+0001bd70: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+0001bd80: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
+0001bd90: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
+0001bda0: 6f6c 6465 722f 6672 616d 6573 2f6f 7574  older/frames/out
+0001bdb0: 7075 742f 7061 7468 5f70 6c6f 7473 2f54  put/path_plots/T
+0001bdc0: 7269 616c 2020 2020 3130 2e6d 7034 272c  rial    10.mp4',
+0001bdd0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0001bde0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0001bdf0: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0001be00: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0001be10: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
+0001be20: 6d65 732f 6f75 7470 7574 2f70 6174 685f  mes/output/path_
+0001be30: 706c 6f74 732f 5472 6961 6c20 2020 2031  plots/Trial    1
+0001be40: 305f 312e 6d70 3427 5d0a 2020 2020 3e3e  0_1.mp4'].    >>
+0001be50: 3e20 6672 6d5f 6964 7320 3d20 5b5b 302c  > frm_ids = [[0,
+0001be60: 2032 305d 2c20 5b32 302c 2034 305d 5d0a   20], [20, 40]].
+0001be70: 2020 2020 3e3e 3e20 636c 6970 5f76 6964      >>> clip_vid
+0001be80: 656f 735f 6279 5f66 7261 6d65 5f69 6473  eos_by_frame_ids
+0001be90: 2866 696c 655f 7061 7468 733d 6669 6c65  (file_paths=file
+0001bea0: 5f70 6174 6873 2c20 6672 6d5f 6964 733d  _paths, frm_ids=
+0001beb0: 6672 6d5f 6964 732c 2073 6176 655f 6469  frm_ids, save_di
+0001bec0: 723d 272f 5573 6572 732f 7369 6d6f 6e2f  r='/Users/simon/
+0001bed0: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0001bee0: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0001bef0: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+0001bf00: 726f 6a65 6374 5f66 6f6c 6465 722f 6672  roject_folder/fr
+0001bf10: 616d 6573 2f6f 7574 7075 742f 7061 7468  ames/output/path
+0001bf20: 5f70 6c6f 7473 2f74 7269 616c 5f63 6e74  _plots/trial_cnt
+0001bf30: 2729 0a20 2020 2022 2222 0a0a 2020 2020  ').    """..    
+0001bf40: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+0001bf50: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+0001bf60: 2020 2063 6865 636b 5f76 616c 6964 5f6c     check_valid_l
+0001bf70: 7374 280a 2020 2020 2020 2020 6461 7461  st(.        data
+0001bf80: 3d66 696c 655f 7061 7468 732c 0a20 2020  =file_paths,.   
+0001bf90: 2020 2020 2073 6f75 7263 653d 636c 6970       source=clip
+0001bfa0: 5f76 6964 656f 735f 6279 5f66 7261 6d65  _videos_by_frame
+0001bfb0: 5f69 6473 2e5f 5f6e 616d 655f 5f2c 0a20  _ids.__name__,. 
+0001bfc0: 2020 2020 2020 2076 616c 6964 5f64 7479         valid_dty
+0001bfd0: 7065 733d 2873 7472 2c29 2c0a 2020 2020  pes=(str,),.    
+0001bfe0: 2020 2020 6d69 6e5f 6c65 6e3d 312c 0a20      min_len=1,. 
+0001bff0: 2020 2029 0a20 2020 2063 6865 636b 5f76     ).    check_v
+0001c000: 616c 6964 5f6c 7374 280a 2020 2020 2020  alid_lst(.      
+0001c010: 2020 6461 7461 3d66 726d 5f69 6473 2c0a    data=frm_ids,.
+0001c020: 2020 2020 2020 2020 736f 7572 6365 3d63          source=c
+0001c030: 6c69 705f 7669 6465 6f73 5f62 795f 6672  lip_videos_by_fr
+0001c040: 616d 655f 6964 732e 5f5f 6e61 6d65 5f5f  ame_ids.__name__
+0001c050: 2c0a 2020 2020 2020 2020 7661 6c69 645f  ,.        valid_
+0001c060: 6474 7970 6573 3d28 6c69 7374 2c29 2c0a  dtypes=(list,),.
+0001c070: 2020 2020 2020 2020 6578 6163 745f 6c65          exact_le
+0001c080: 6e3d 6c65 6e28 6669 6c65 5f70 6174 6873  n=len(file_paths
+0001c090: 292c 0a20 2020 2029 0a20 2020 2066 6f72  ),.    ).    for
+0001c0a0: 2063 6e74 2c20 6920 696e 2065 6e75 6d65   cnt, i in enume
+0001c0b0: 7261 7465 2866 726d 5f69 6473 293a 0a20  rate(frm_ids):. 
+0001c0c0: 2020 2020 2020 2063 6865 636b 5f76 616c         check_val
+0001c0d0: 6964 5f6c 7374 280a 2020 2020 2020 2020  id_lst(.        
+0001c0e0: 2020 2020 6461 7461 3d69 2c0a 2020 2020      data=i,.    
+0001c0f0: 2020 2020 2020 2020 736f 7572 6365 3d66          source=f
+0001c100: 2263 6c69 705f 7669 6465 6f73 5f62 795f  "clip_videos_by_
+0001c110: 6672 616d 655f 636f 756e 742e 5f5f 6e61  frame_count.__na
+0001c120: 6d65 5f20 6672 6d5f 6964 7320 7b63 6e74  me_ frm_ids {cnt
+0001c130: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+0001c140: 7661 6c69 645f 6474 7970 6573 3d28 696e  valid_dtypes=(in
+0001c150: 742c 292c 0a20 2020 2020 2020 2020 2020  t,),.           
+0001c160: 2065 7861 6374 5f6c 656e 3d32 2c0a 2020   exact_len=2,.  
+0001c170: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c180: 6966 2069 5b30 5d20 3e3d 2069 5b31 5d3a  if i[0] >= i[1]:
+0001c190: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001c1a0: 7365 2046 7261 6d65 5261 6e67 6545 7272  se FrameRangeErr
+0001c1b0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0001c1c0: 2020 2020 6d73 673d 6622 5374 6172 7420      msg=f"Start 
+0001c1d0: 6672 616d 6520 666f 7220 7669 6465 6f20  frame for video 
+0001c1e0: 7b69 7d20 6973 2061 6674 6572 206f 7220  {i} is after or 
+0001c1f0: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
+0001c200: 656e 6420 6672 616d 6520 287b 695b 305d  end frame ({i[0]
+0001c210: 7d2c 207b 695b 315d 7d29 222c 0a20 2020  }, {i[1]})",.   
+0001c220: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+0001c230: 7263 653d 636c 6970 5f76 6964 656f 735f  rce=clip_videos_
+0001c240: 6279 5f66 7261 6d65 5f69 6473 2e5f 5f6e  by_frame_ids.__n
+0001c250: 616d 655f 5f2c 0a20 2020 2020 2020 2020  ame__,.         
+0001c260: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+0001c270: 2869 5b30 5d20 3c20 3029 206f 7220 2869  (i[0] < 0) or (i
+0001c280: 5b31 5d20 3c20 3129 3a0a 2020 2020 2020  [1] < 1):.      
+0001c290: 2020 2020 2020 7261 6973 6520 4672 616d        raise Fram
+0001c2a0: 6552 616e 6765 4572 726f 7228 0a20 2020  eRangeError(.   
+0001c2b0: 2020 2020 2020 2020 2020 2020 206d 7367               msg
+0001c2c0: 3d66 2253 7461 7274 2066 7261 6d65 2068  =f"Start frame h
+0001c2d0: 6173 2074 6f20 6265 2061 7420 6c65 6173  as to be at leas
+0001c2e0: 7420 3020 616e 6420 656e 6420 6672 616d  t 0 and end fram
+0001c2f0: 6520 6861 7320 746f 2062 6520 6174 206c  e has to be at l
+0001c300: 6561 7374 2031 222c 0a20 2020 2020 2020  east 1",.       
+0001c310: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+0001c320: 636c 6970 5f76 6964 656f 735f 6279 5f66  clip_videos_by_f
+0001c330: 7261 6d65 5f69 6473 2e5f 5f6e 616d 655f  rame_ids.__name_
+0001c340: 5f2c 0a20 2020 2020 2020 2020 2020 2029  _,.            )
+0001c350: 0a20 2020 2076 6964 656f 5f6d 6574 615f  .    video_meta_
+0001c360: 6461 7461 203d 205b 6765 745f 7669 6465  data = [get_vide
+0001c370: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
+0001c380: 6f5f 7061 7468 3d78 2920 666f 7220 7820  o_path=x) for x 
+0001c390: 696e 2066 696c 655f 7061 7468 735d 0a20  in file_paths]. 
+0001c3a0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0001c3b0: 6528 6c65 6e28 7669 6465 6f5f 6d65 7461  e(len(video_meta
+0001c3c0: 5f64 6174 6129 293a 0a20 2020 2020 2020  _data)):.       
+0001c3d0: 2069 6620 2866 726d 5f69 6473 5b69 5d5b   if (frm_ids[i][
+0001c3e0: 305d 203e 2076 6964 656f 5f6d 6574 615f  0] > video_meta_
+0001c3f0: 6461 7461 5b69 5d5b 2266 7261 6d65 5f63  data[i]["frame_c
+0001c400: 6f75 6e74 225d 2920 6f72 2028 0a20 2020  ount"]) or (.   
+0001c410: 2020 2020 2020 2020 2066 726d 5f69 6473           frm_ids
+0001c420: 5b69 5d5b 315d 203e 2076 6964 656f 5f6d  [i][1] > video_m
+0001c430: 6574 615f 6461 7461 5b69 5d5b 2266 7261  eta_data[i]["fra
+0001c440: 6d65 5f63 6f75 6e74 225d 0a20 2020 2020  me_count"].     
+0001c450: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001c460: 2020 7261 6973 6520 4672 616d 6552 616e    raise FrameRan
+0001c470: 6765 4572 726f 7228 0a20 2020 2020 2020  geError(.       
+0001c480: 2020 2020 2020 2020 206d 7367 3d66 2756           msg=f'V
+0001c490: 6964 656f 207b 692b 317d 2068 6173 207b  ideo {i+1} has {
+0001c4a0: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+0001c4b0: 695d 5b22 6672 616d 655f 636f 756e 7422  i]["frame_count"
+0001c4c0: 5d7d 2066 7261 6d65 732c 2063 616e 6e6f  ]} frames, canno
+0001c4d0: 7420 7573 6520 7374 6172 7420 616e 6420  t use start and 
+0001c4e0: 656e 6420 6672 616d 6520 7b66 726d 5f69  end frame {frm_i
+0001c4f0: 6473 5b69 5d7d 272c 0a20 2020 2020 2020  ds[i]}',.       
+0001c500: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+0001c510: 636c 6970 5f76 6964 656f 735f 6279 5f66  clip_videos_by_f
+0001c520: 7261 6d65 5f69 6473 2e5f 5f6e 616d 655f  rame_ids.__name_
+0001c530: 5f2c 0a20 2020 2020 2020 2020 2020 2029  _,.            )
+0001c540: 0a20 2020 2069 6620 7361 7665 5f64 6972  .    if save_dir
+0001c550: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0001c560: 2020 2020 2020 6368 6563 6b5f 6966 5f64        check_if_d
+0001c570: 6972 5f65 7869 7374 7328 0a20 2020 2020  ir_exists(.     
+0001c580: 2020 2020 2020 2069 6e5f 6469 723d 7361         in_dir=sa
+0001c590: 7665 5f64 6972 2c0a 2020 2020 2020 2020  ve_dir,.        
+0001c5a0: 2020 2020 736f 7572 6365 3d63 6c69 705f      source=clip_
+0001c5b0: 7669 6465 6f73 5f62 795f 6672 616d 655f  videos_by_frame_
+0001c5c0: 6964 732e 5f5f 6e61 6d65 5f5f 2c0a 2020  ids.__name__,.  
+0001c5d0: 2020 2020 2020 2020 2020 6372 6561 7465            create
+0001c5e0: 5f69 665f 6e6f 745f 6578 6973 743d 5472  _if_not_exist=Tr
+0001c5f0: 7565 2c0a 2020 2020 2020 2020 290a 2020  ue,.        ).  
+0001c600: 2020 666f 7220 636e 742c 2066 696c 655f    for cnt, file_
+0001c610: 7061 7468 2069 6e20 656e 756d 6572 6174  path in enumerat
+0001c620: 6528 6669 6c65 5f70 6174 6873 293a 0a20  e(file_paths):. 
+0001c630: 2020 2020 2020 2076 6964 656f 5f74 696d         video_tim
+0001c640: 6572 203d 2053 696d 6261 5469 6d65 7228  er = SimbaTimer(
+0001c650: 7374 6172 743d 5472 7565 290a 2020 2020  start=True).    
+0001c660: 2020 2020 6469 722c 2076 6964 656f 5f6e      dir, video_n
+0001c670: 616d 652c 2065 7874 203d 2067 6574 5f66  ame, ext = get_f
+0001c680: 6e5f 6578 7428 6669 6c65 7061 7468 3d66  n_ext(filepath=f
+0001c690: 696c 655f 7061 7468 290a 2020 2020 2020  ile_path).      
+0001c6a0: 2020 735f 662c 2065 5f66 203d 2066 726d    s_f, e_f = frm
+0001c6b0: 5f69 6473 5b63 6e74 5d5b 305d 2c20 6672  _ids[cnt][0], fr
+0001c6c0: 6d5f 6964 735b 636e 745d 5b31 5d0a 2020  m_ids[cnt][1].  
+0001c6d0: 2020 2020 2020 7072 696e 7428 6622 5472        print(f"Tr
+0001c6e0: 696d 6d69 6e67 207b 7669 6465 6f5f 6e61  imming {video_na
+0001c6f0: 6d65 7d20 6672 6f6d 2066 7261 6d65 207b  me} from frame {
+0001c700: 735f 667d 2074 6f20 6672 616d 6520 7b65  s_f} to frame {e
+0001c710: 5f66 7d2e 2e2e 2229 0a20 2020 2020 2020  _f}...").       
+0001c720: 2069 6620 7361 7665 5f64 6972 2069 7320   if save_dir is 
+0001c730: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001c740: 2020 2020 2020 6f75 745f 7061 7468 203d        out_path =
+0001c750: 206f 732e 7061 7468 2e6a 6f69 6e28 7361   os.path.join(sa
+0001c760: 7665 5f64 6972 2c20 6f73 2e70 6174 682e  ve_dir, os.path.
+0001c770: 6261 7365 6e61 6d65 2866 696c 655f 7061  basename(file_pa
+0001c780: 7468 2929 0a20 2020 2020 2020 2065 6c73  th)).        els
+0001c790: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+0001c7a0: 7574 5f70 6174 6820 3d20 6f73 2e70 6174  ut_path = os.pat
+0001c7b0: 682e 6a6f 696e 2864 6972 2c20 6622 7b76  h.join(dir, f"{v
+0001c7c0: 6964 656f 5f6e 616d 657d 5f7b 735f 667d  ideo_name}_{s_f}
+0001c7d0: 5f7b 655f 667d 7b65 7874 7d22 290a 2020  _{e_f}{ext}").  
+0001c7e0: 2020 2020 2020 636d 6420 3d20 6627 6666        cmd = f'ff
+0001c7f0: 6d70 6567 202d 6920 227b 6669 6c65 5f70  mpeg -i "{file_p
+0001c800: 6174 687d 2220 2d76 6620 2274 7269 6d3d  ath}" -vf "trim=
+0001c810: 7b73 5f66 7d3a 7b65 5f66 7d2c 7365 7470  {s_f}:{e_f},setp
+0001c820: 7473 3d50 5453 2d53 5441 5254 5054 5322  ts=PTS-STARTPTS"
+0001c830: 202d 633a 7620 6c69 6278 3236 3420 2d63   -c:v libx264 -c
+0001c840: 3a61 2061 6163 202d 6c6f 676c 6576 656c  :a aac -loglevel
+0001c850: 2065 7272 6f72 202d 7374 6174 7320 227b   error -stats "{
+0001c860: 6f75 745f 7061 7468 7d22 202d 7927 0a20  out_path}" -y'. 
+0001c870: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
+0001c880: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
+0001c890: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
+0001c8a0: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
+0001c8b0: 2020 2020 2020 2020 7669 6465 6f5f 7469          video_ti
+0001c8c0: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
+0001c8d0: 0a20 2020 2020 2020 2070 7269 6e74 280a  .        print(.
+0001c8e0: 2020 2020 2020 2020 2020 2020 6622 5669              f"Vi
+0001c8f0: 6465 6f20 7b76 6964 656f 5f6e 616d 657d  deo {video_name}
+0001c900: 2063 6f6d 706c 6574 6520 2865 6c61 7073   complete (elaps
+0001c910: 6564 2074 696d 6520 7b76 6964 656f 5f74  ed time {video_t
+0001c920: 696d 6572 2e65 6c61 7073 6564 5f74 696d  imer.elapsed_tim
+0001c930: 655f 7374 727d 7329 220a 2020 2020 2020  e_str}s)".      
+0001c940: 2020 290a 2020 2020 7469 6d65 722e 7374    ).    timer.st
+0001c950: 6f70 5f74 696d 6572 2829 0a20 2020 2069  op_timer().    i
+0001c960: 6620 7361 7665 5f64 6972 2069 7320 4e6f  f save_dir is No
+0001c970: 6e65 3a0a 2020 2020 2020 2020 7374 646f  ne:.        stdo
+0001c980: 7574 5f73 7563 6365 7373 280a 2020 2020  ut_success(.    
+0001c990: 2020 2020 2020 2020 6d73 673d 6622 7b6c          msg=f"{l
+0001c9a0: 656e 2866 696c 655f 7061 7468 7329 7d20  en(file_paths)} 
+0001c9b0: 7669 6465 6f28 7329 2063 6c69 7070 6564  video(s) clipped
+0001c9c0: 2062 7920 6672 616d 6522 2c0a 2020 2020   by frame",.    
+0001c9d0: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
+0001c9e0: 7469 6d65 3d74 696d 6572 2e65 6c61 7073  time=timer.elaps
+0001c9f0: 6564 5f74 696d 655f 7374 722c 0a20 2020  ed_time_str,.   
+0001ca00: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+0001ca10: 0a20 2020 2020 2020 2073 7464 6f75 745f  .        stdout_
+0001ca20: 7375 6363 6573 7328 0a20 2020 2020 2020  success(.       
+0001ca30: 2020 2020 206d 7367 3d66 227b 6c65 6e28       msg=f"{len(
+0001ca40: 6669 6c65 5f70 6174 6873 297d 2076 6964  file_paths)} vid
+0001ca50: 656f 2873 2920 636c 6970 7065 6420 6279  eo(s) clipped by
+0001ca60: 2066 7261 6d65 2061 6e64 2073 6176 6564   frame and saved
+0001ca70: 2069 6e20 7b73 6176 655f 6469 727d 222c   in {save_dir}",
+0001ca80: 0a20 2020 2020 2020 2020 2020 2065 6c61  .            ela
+0001ca90: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
+0001caa0: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
+0001cab0: 2c0a 2020 2020 2020 2020 290a 0a0a 2320  ,.        )...# 
+0001cac0: 7669 6465 6f5f 7061 7468 7320 3d20 5b27  video_paths = ['
+0001cad0: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+0001cae0: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+0001caf0: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+0001cb00: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+0001cb10: 6563 745f 666f 6c64 6572 2f6d 6572 6765  ect_folder/merge
+0001cb20: 2f54 7269 616c 2020 2020 3130 5f63 6c69  /Trial    10_cli
+0001cb30: 7070 6564 5f67 616e 7474 2e6d 7034 272c  pped_gantt.mp4',
+0001cb40: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
+0001cb50: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
+0001cb60: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0001cb70: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0001cb80: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+0001cb90: 726f 6a65 6374 5f66 6f6c 6465 722f 6d65  roject_folder/me
+0001cba0: 7267 652f 5472 6961 6c20 2020 2031 305f  rge/Trial    10_
+0001cbb0: 636c 6970 7065 642e 6d70 3427 2c0a 2320  clipped.mp4',.# 
+0001cbc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001cbd0: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+0001cbe0: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+0001cbf0: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+0001cc00: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+0001cc10: 6563 745f 666f 6c64 6572 2f6d 6572 6765  ect_folder/merge
+0001cc20: 2f54 7269 616c 2020 2020 3130 5f63 6c69  /Trial    10_cli
+0001cc30: 7070 6564 5f6c 696e 652e 6d70 3427 2c0a  pped_line.mp4',.
+0001cc40: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001cc50: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0001cc60: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0001cc70: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0001cc80: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0001cc90: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
+0001cca0: 6765 2f54 7269 616c 2020 2020 2033 5f63  ge/Trial     3_c
+0001ccb0: 6c69 7070 6564 2e6d 7034 275d 0a23 0a23  lipped.mp4'].#.#
+0001ccc0: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
+0001ccd0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001cce0: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001ccf0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001cd00: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+0001cd10: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+0001cd20: 6f73 2f54 7269 616c 2020 2020 3130 2e6d  os/Trial    10.m
+0001cd30: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
+0001cd40: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
+0001cd50: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+0001cd60: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+0001cd70: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+0001cd80: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+0001cd90: 722f 6d65 7267 652f 5472 6961 6c20 2020  r/merge/Trial   
+0001cda0: 2031 305f 636c 6970 7065 645f 6761 6e74   10_clipped_gant
+0001cdb0: 742e 6d70 3427 2c0a 2320 2020 2020 2020  t.mp4',.#       
+0001cdc0: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
+0001cdd0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
+0001cde0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
+0001cdf0: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
+0001ce00: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
+0001ce10: 6c64 6572 2f6d 6572 6765 2f54 7269 616c  lder/merge/Trial
+0001ce20: 2020 2020 3130 5f63 6c69 7070 6564 5f6c      10_clipped_l
+0001ce30: 696e 652e 6d70 3427 2c0a 2320 2020 2020  ine.mp4',.#     
+0001ce40: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
+0001ce50: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+0001ce60: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+0001ce70: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+0001ce80: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+0001ce90: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
+0001cea0: 616c 2020 2020 2033 5f63 6c69 7070 6564  al     3_clipped
+0001ceb0: 2e6d 7034 275d 0a23 0a23 2073 6176 655f  .mp4'].#.# save_
+0001cec0: 7061 7468 203d 2027 2f55 7365 7273 2f73  path = '/Users/s
+0001ced0: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+0001cee0: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+0001cef0: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+0001cf00: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+0001cf10: 6572 2f6d 6572 6765 2f6f 7574 2e6d 7034  er/merge/out.mp4
+0001cf20: 270a 0a23 0a23 2076 6964 656f 5f70 6174  '..#.# video_pat
+0001cf30: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
+0001cf40: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+0001cf50: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+0001cf60: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+0001cf70: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+0001cf80: 722f 6672 616d 6573 2f6f 7574 7075 742f  r/frames/output/
+0001cf90: 6761 6e74 745f 706c 6f74 732f 5472 6961  gantt_plots/Tria
+0001cfa0: 6c20 2020 2031 302e 6d70 3427 2c0a 2320  l    10.mp4',.# 
+0001cfb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001cfc0: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+0001cfd0: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+0001cfe0: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+0001cff0: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+0001d000: 6563 745f 666f 6c64 6572 2f76 6964 656f  ect_folder/video
+0001d010: 732f 5472 6961 6c20 2020 2031 302e 6d70  s/Trial    10.mp
+0001d020: 3427 2c0a 2320 2020 2020 2020 2020 2020  4',.#           
+0001d030: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
+0001d040: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+0001d050: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+0001d060: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
+0001d070: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
+0001d080: 2f66 7261 6d65 732f 6f75 7470 7574 2f6c  /frames/output/l
+0001d090: 696e 655f 706c 6f74 2f54 7269 616c 2020  ine_plot/Trial  
+0001d0a0: 2020 3130 2e6d 7034 272c 0a23 2020 2020    10.mp4',.#    
+0001d0b0: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
+0001d0c0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+0001d0d0: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+0001d0e0: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+0001d0f0: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+0001d100: 5f66 6f6c 6465 722f 6672 616d 6573 2f6f  _folder/frames/o
+0001d110: 7574 7075 742f 6c69 6e65 5f70 6c6f 742f  utput/line_plot/
+0001d120: 5472 6961 6c20 2020 2020 332e 6d70 3427  Trial     3.mp4'
+0001d130: 5d0a 2320 7361 7665 5f70 6174 6820 3d20  ].# save_path = 
+0001d140: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001d150: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001d160: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001d170: 2f52 4154 5f4e 4f52 2f70 726f 6a65 6374  /RAT_NOR/project
+0001d180: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
+0001d190: 6573 742f 6e65 772f 626c 616e 6b5f 7465  est/new/blank_te
+0001d1a0: 7374 2e6d 7034 270a 0a23 2076 6964 656f  st.mp4'..# video
+0001d1b0: 5f70 6174 6873 203d 205b 272f 5573 6572  _paths = ['/User
+0001d1c0: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+0001d1d0: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+0001d1e0: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
+0001d1f0: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
+0001d200: 6f6c 6465 722f 7669 6465 6f73 2f54 7269  older/videos/Tri
+0001d210: 616c 2020 2020 3130 2e6d 7034 272c 0a23  al    10.mp4',.#
+0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d230: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001d240: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001d250: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001d260: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+0001d270: 6a65 6374 5f66 6f6c 6465 722f 6672 616d  ject_folder/fram
+0001d280: 6573 2f6f 7574 7075 742f 6c69 6e65 5f70  es/output/line_p
+0001d290: 6c6f 742f 5472 6961 6c20 2020 2031 302e  lot/Trial    10.
+0001d2a0: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
+0001d2b0: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
+0001d2c0: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+0001d2d0: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+0001d2e0: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+0001d2f0: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+0001d300: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
+0001d310: 2f6c 696e 655f 706c 6f74 2f54 7269 616c  /line_plot/Trial
+0001d320: 2020 2020 2033 2e6d 7034 275d 0a0a 2320       3.mp4']..# 
+0001d330: 6d69 7865 645f 6d6f 7361 6963 5f63 6f6e  mixed_mosaic_con
+0001d340: 6361 7465 6e61 746f 7228 7669 6465 6f5f  catenator(video_
+0001d350: 7061 7468 733d 7669 6465 6f5f 7061 7468  paths=video_path
+0001d360: 732c 2073 6176 655f 7061 7468 3d73 6176  s, save_path=sav
+0001d370: 655f 7061 7468 2c20 6770 753d 4661 6c73  e_path, gpu=Fals
+0001d380: 652c 2076 6572 626f 7365 3d54 7275 6529  e, verbose=True)
+0001d390: 0a                                       .
```

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.90.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.90.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.90.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.90.4/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.90.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.90.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.90.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.90.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.90.4/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.90.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.90.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.90.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.90.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.90.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.90.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.90.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.90.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.90.3
+Version: 1.90.4
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,15 @@
 simba/sandbox/lcs.py
 simba/sandbox/line_locate_point.py
 simba/sandbox/line_plot.py
 simba/sandbox/line_plot_plotly.py
 simba/sandbox/linear_fretchet.py
 simba/sandbox/linestring_path.py
 simba/sandbox/madmedianrule.py
+simba/sandbox/make_path_plot.py
 simba/sandbox/make_splash.py
 simba/sandbox/margalef_diversification_index.py
 simba/sandbox/mcnamar.py
 simba/sandbox/menhinicks_index.py
 simba/sandbox/mosaic.py
 simba/sandbox/multiframe_is_shape_covered.py
 simba/sandbox/multifrm_to_points.py
```

### Comparing `Simba-UW-tf-dev-1.90.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.90.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/LICENSE` & `Simba-UW-tf-dev-1.90.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.90.4/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.90.4/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_stats.py` & `Simba-UW-tf-dev-1.90.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.90.4/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.90.4/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.90.4/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.90.4/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.90.4/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.90.4/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.90.4/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.90.4/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.90.4/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.90.4/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.90.4/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.3/README.md` & `Simba-UW-tf-dev-1.90.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 - [Mutual exclusivity using heuristic rules in SimBA](docs/mutual_exclusivity_heuristic_rules.md) 📗
 - [Compute feature subsets in SimBA](docs/feature_subsets.md) 📕 
 - [Kleinberg markov chain classification smoothing in SimBA](docs/kleinberg_filter.md) 🔗
 - [Cue-light analyses in SimBA](docs/cue_light_tutorial.md)💡💡
 - [Bounding boxes in SimBA](docs/anchored_rois.md)📦
 - [Reversing the directionality of classifiers in SimBA](docs/reverse_annotations.md) ⏪
 - [Spike-time correlation coefficients in SimBA](docs/FSTTC.md) 📔
+- [Spontaneous alternation in SimBA](/docs/spontaneous_alternation.md)🌽
 - [Analysing animal directions in SimBA](docs/directionality_between_animals.md) 🧭
 - [Recommended hardware](https://github.com/sgoldenlab/simba/blob/master/misc/system_requirements.md) 🖥️
 - [Downloading compressed data from the SimBA OSF repository](https://github.com/sgoldenlab/simba/blob/master/docs/using_OSF.md) 💾
 
 ## Resource 💾
 
 All data (classifiers etc.) is available on our [Open Science Framework repository](https://osf.io/tmu6y/). For a schematic overview of the data respository folder structure (as of March-20-2020), click [HERE](https://github.com/sgoldenlab/simba/blob/master/images/OSF_folder_structure_031820.jpg).
```

### Comparing `Simba-UW-tf-dev-1.90.3/setup.py` & `Simba-UW-tf-dev-1.90.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.90.3",
+    version="1.90.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

