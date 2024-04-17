# Comparing `tmp/AIPyS-0.0.8.tar.gz` & `tmp/AIPyS-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.0.8.tar", last modified: Tue Apr 16 14:02:38 2024, max compression
+gzip compressed data, was "AIPyS-0.0.9.tar", last modified: Tue Apr 16 19:28:38 2024, max compression
```

## Comparing `AIPyS-0.0.8.tar` & `AIPyS-0.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.598814 AIPyS-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:37.773306 AIPyS-0.0.8/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.121455 AIPyS-0.0.8/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7580 2024-04-15 18:55:22.000000 AIPyS-0.0.8/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.0.8/AIPyS/CLI/area_analysis.py
--rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.0.8/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.8/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.8/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.8/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.8/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:37.727261 AIPyS-0.0.8/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.165596 AIPyS-0.0.8/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.8/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.241393 AIPyS-0.0.8/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.8/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.8/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.8/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.0.8/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.8/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.8/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:37.730250 AIPyS-0.0.8/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.319403 AIPyS-0.0.8/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.8/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-04-16 13:55:44.000000 AIPyS-0.0.8/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.8/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/segmentation/cellpose/__init__.py
--rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.0.8/AIPyS/segmentation/cellpose/plotObjectAreas.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.329577 AIPyS-0.0.8/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.8/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.411446 AIPyS-0.0.8/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    13755 2024-04-15 18:45:15.000000 AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.8/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.8/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.535728 AIPyS-0.0.8/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3838 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 14:02:37.000000 AIPyS-0.0.8/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3838 2024-04-16 14:02:38.593824 AIPyS-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 14:02:38.598814 AIPyS-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1407 2024-04-16 14:01:49.000000 AIPyS-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:37.736233 AIPyS-0.0.8/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.430585 AIPyS-0.0.8/web_app/AreasViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/AreasViz/__init__.py
--rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.0.8/web_app/AreasViz/app.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.461927 AIPyS-0.0.8/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.0.8/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.502814 AIPyS-0.0.8/web_app/TableViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/TableViz/__init__.py
--rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.8/web_app/TableViz/app.py
--rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/TableViz/distplot.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:02:38.530741 AIPyS-0.0.8/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.8/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4589 2024-04-16 13:40:50.000000 AIPyS-0.0.8/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.966559 AIPyS-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.229108 AIPyS-0.0.9/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.516514 AIPyS-0.0.9/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7580 2024-04-15 18:55:22.000000 AIPyS-0.0.9/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.0.9/AIPyS/CLI/area_analysis.py
+-rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.0.9/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.9/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.9/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.9/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.9/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.191005 AIPyS-0.0.9/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.563189 AIPyS-0.0.9/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.9/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.630362 AIPyS-0.0.9/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.9/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.9/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.9/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.0.9/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.9/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.9/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.192486 AIPyS-0.0.9/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.696271 AIPyS-0.0.9/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.9/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-04-16 13:55:44.000000 AIPyS-0.0.9/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.9/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/segmentation/cellpose/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.0.9/AIPyS/segmentation/cellpose/plotObjectAreas.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.709195 AIPyS-0.0.9/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.9/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.801384 AIPyS-0.0.9/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    12982 2024-04-16 18:37:13.000000 AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.9/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.9/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.917593 AIPyS-0.0.9/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3838 2024-04-16 19:28:37.000000 AIPyS-0.0.9/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2024-04-16 19:28:38.000000 AIPyS-0.0.9/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 19:28:37.000000 AIPyS-0.0.9/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-16 19:28:37.000000 AIPyS-0.0.9/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-04-16 19:28:37.000000 AIPyS-0.0.9/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 19:28:37.000000 AIPyS-0.0.9/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3838 2024-04-16 19:28:38.950051 AIPyS-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 19:28:38.966559 AIPyS-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2024-04-16 19:28:31.000000 AIPyS-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.195693 AIPyS-0.0.9/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.817272 AIPyS-0.0.9/web_app/AreasViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/AreasViz/__init__.py
+-rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.0.9/web_app/AreasViz/app.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.848630 AIPyS-0.0.9/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.0.9/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.882581 AIPyS-0.0.9/web_app/TableViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/TableViz/__init__.py
+-rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.9/web_app/TableViz/app.py
+-rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/TableViz/distplot.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:28:38.900423 AIPyS-0.0.9/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.9/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4589 2024-04-16 18:40:03.000000 AIPyS-0.0.9/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.0.8/AIPyS/CLI/aipys.py` & `AIPyS-0.0.9/AIPyS/CLI/aipys.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/CLI/area_analysis.py` & `AIPyS-0.0.9/AIPyS/CLI/area_analysis.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/CLI/loadParameters.py` & `AIPyS-0.0.9/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/CLI/promptParameters.py` & `AIPyS-0.0.9/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/CLI/set_parameters.py` & `AIPyS-0.0.9/AIPyS/CLI/set_parameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/CLI/test.py` & `AIPyS-0.0.9/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/DataLoad.py` & `AIPyS-0.0.9/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.0.9/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.0.9/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.0.9/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.0.9/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.0.9/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/Baysian_training.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.0.9/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.0.9/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.0.9/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.0.9/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/cellpose/plotObjectAreas.py` & `AIPyS-0.0.9/AIPyS/segmentation/cellpose/plotObjectAreas.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.0.9/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.0.9/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -303,43 +303,27 @@
     y = np.array(arr_area).reshape(-1, 1)  # Reshape data to 2D array required by GMM
     # Define the range of components to test
     n_components = np.arange(1, 3)
     # Fit GMM models for 1 and 2 components
     models = [GaussianMixture(n_components=n, random_state=42).fit(y) for n in n_components]
     # Evaluate models using Bayesian Information Criterion (BIC)
     BIC_scores = [model.bic(y) for model in models]
-
-    # # Plot BIC scores to visualize the best model
-    # plt.figure(figsize=(8, 4))
-    # plt.plot(n_components, BIC_scores, marker='o')
-    # plt.title('BIC Scores by Number of Components')
-    # plt.xlabel('Number of Components')
-    # plt.ylabel('BIC Score')
-    # plt.xticks(n_components)
-    # plt.show()
-
     # Select the model with the lowest BIC
     best_model = models[np.argmin(BIC_scores)]
 
     # Assuming the best model has two components (as expected)
-    #if best_model.n_components == 2:
-    means = np.sort(best_model.means_.flatten())
-    std_dev = np.sqrt(best_model.covariances_.flatten())
-        # Estimate a potential threshold
-    threshold = (means[0] + means[1]) / 2
-        # print(f"Estimated threshold between populations: {threshold}")
-
-        # # Optionally, plot the distribution and the threshold
-        # plt.hist(y, bins=30, density=True, alpha=0.6, color='g')
-        # xmin, xmax = plt.xlim()
-        # x = np.linspace(xmin, xmax, 100)
-        # for mean, std in zip(means, std_dev):
-        #     p = np.exp(-(x - mean)**2 / (2 * std**2)) / (np.sqrt(2 * np.pi) * std)
-        #     plt.plot(x, p, 'k', linewidth=2)
-        # plt.axvline(x=threshold, color='red', linestyle='dashed', linewidth=2)
-        # plt.title('Fit results and estimated threshold')
-        # plt.show()
-    if isinstance(threshold, (int, float)) and threshold > 0:
-        return threshold
-    else:
-        return "na"
+    if best_model.n_components == 2:
+        means = np.sort(best_model.means_.flatten())
+        std_dev = np.sqrt(best_model.covariances_.flatten())
+            # Estimate a potential threshold
+        try:
+            threshold = (means[0] + means[1]) / 2
+        except Exception:
+            threshold = -1
+        if isinstance(threshold, (int, float)) and threshold > 0:
+            return threshold
+        else:
+            threshold =  "na"
+            return threshold
+    threshold =  "na"
+    return threshold
```

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.0.9/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.0.9/AIPyS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.8/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.0.9/AIPyS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/LICENSE` & `AIPyS-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/PKG-INFO` & `AIPyS-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.8/setup.py` & `AIPyS-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
-
 setup(
     name="AIPyS",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
                                     'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz', 'web_app.AreasViz',]),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:main',
```

### Comparing `AIPyS-0.0.8/web_app/AreasViz/app.py` & `AIPyS-0.0.9/web_app/AreasViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/web_app/Image_labeling/app.py` & `AIPyS-0.0.9/web_app/Image_labeling/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/web_app/Image_labeling/draft.py` & `AIPyS-0.0.9/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/web_app/TableViz/app.py` & `AIPyS-0.0.9/web_app/TableViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/web_app/TableViz/distplot.py` & `AIPyS-0.0.9/web_app/TableViz/distplot.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.8/web_app/measure_length/app.py` & `AIPyS-0.0.9/web_app/measure_length/app.py`

 * *Files identical despite different names*

