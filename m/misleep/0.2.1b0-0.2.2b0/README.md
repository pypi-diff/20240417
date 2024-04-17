# Comparing `tmp/misleep-0.2.1b0.tar.gz` & `tmp/misleep-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.2.1b0.tar", last modified: Mon Apr 15 11:49:07 2024, max compression
+gzip compressed data, was "misleep-0.2.2b0.tar", last modified: Wed Apr 17 11:29:29 2024, max compression
```

## Comparing `misleep-0.2.1b0.tar` & `misleep-0.2.2b0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.322926 misleep-0.2.1b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.1b0/LICENSE
--rw-rw-rw-   0        0        0     2968 2024-04-15 11:49:07.321926 misleep-0.2.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2024-04-15 03:11:05.000000 misleep-0.2.1b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.298926 misleep-0.2.1b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.1b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      523 2024-04-15 11:48:54.000000 misleep-0.2.1b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.304926 misleep-0.2.1b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.1b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     6697 2024-04-15 11:23:51.000000 misleep-0.2.1b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    56191 2024-04-15 11:22:51.000000 misleep-0.2.1b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.307927 misleep-0.2.1b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.1b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.1b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.310927 misleep-0.2.1b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.1b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24854 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/uis/save_data_dialog_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     3375 2024-04-15 10:35:14.000000 misleep-0.2.1b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.312926 misleep-0.2.1b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.1b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     6268 2024-04-15 11:24:05.000000 misleep-0.2.1b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     4785 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.314926 misleep-0.2.1b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.1b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.1b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.2.1b0/misleep/preprocessing/signals.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.1b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.316926 misleep-0.2.1b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.1b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.1b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.318926 misleep-0.2.1b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.1b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.1b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.1b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.1b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.300926 misleep-0.2.1b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     2968 2024-04-15 11:49:07.000000 misleep-0.2.1b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-04-15 11:49:07.000000 misleep-0.2.1b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:49:07.000000 misleep-0.2.1b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-15 11:49:07.000000 misleep-0.2.1b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 11:49:07.000000 misleep-0.2.1b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 11:49:07.322926 misleep-0.2.1b0/setup.cfg
--rw-rw-rw-   0        0        0     2157 2024-04-15 11:48:50.000000 misleep-0.2.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:49:07.321926 misleep-0.2.1b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.1b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.1b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.1b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.1b0/test/test_show.py
--rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.1b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.1b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.1b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.847330 misleep-0.2.2b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.2b0/LICENSE
+-rw-rw-rw-   0        0        0     2969 2024-04-17 11:29:29.847330 misleep-0.2.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1871 2024-04-17 11:10:21.000000 misleep-0.2.2b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.823330 misleep-0.2.2b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.2b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      532 2024-04-17 11:26:31.000000 misleep-0.2.2b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.829330 misleep-0.2.2b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.2b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     7443 2024-04-17 11:26:19.000000 misleep-0.2.2b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    56484 2024-04-17 11:23:33.000000 misleep-0.2.2b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.833331 misleep-0.2.2b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.2b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.2b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.837331 misleep-0.2.2b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.2b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    24912 2024-04-17 03:11:18.000000 misleep-0.2.2b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     4884 2024-04-17 11:15:15.000000 misleep-0.2.2b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.838330 misleep-0.2.2b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     6268 2024-04-15 11:24:05.000000 misleep-0.2.2b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.2b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.840331 misleep-0.2.2b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.2b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.2b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.2.2b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.2b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.842331 misleep-0.2.2b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.843331 misleep-0.2.2b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.2b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.2b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.826331 misleep-0.2.2b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     2969 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 11:29:29.847330 misleep-0.2.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     2154 2024-04-17 11:11:27.000000 misleep-0.2.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.846331 misleep-0.2.2b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.2b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.2b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.2b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.2b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.2b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.2b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.2b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.2.1b0/LICENSE` & `misleep-0.2.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/PKG-INFO` & `misleep-0.2.2b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -33,15 +33,15 @@
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
-pip install misleep==0.1.3b
+pip install misleep==0.2.2b0
 ```
 
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into
```

### Comparing `misleep-0.2.1b0/README.md` & `misleep-0.2.2b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
-pip install misleep==0.1.3b
+pip install misleep==0.2.2b0
 ```
 
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into
```

### Comparing `misleep-0.2.1b0/misleep/gui/about.py` & `misleep-0.2.2b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/dialog.py` & `misleep-0.2.2b0/misleep/gui/dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -154,27 +154,41 @@
         super().__init__(parent)
 
         # Enable high dpi devices
         QCoreApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
         self.setupUi(self)
 
         self.ACTimeEditor.setDisabled(True)
-        self.ResetTimeCheckBox.clicked.connect(self.enable_time_editor)
+        self.TransferStartTimeEdit.setDisabled(True)
+        self.ResetTimeCheckBox.clicked.connect(self.enable_ac_time_editor)
+        self.ResetTransferStartTimeCheckBox.clicked.connect(self.enable_start_time_editor)
         
-    def enable_time_editor(self):
+    def enable_ac_time_editor(self):
         self.ACTimeEditor.setEnabled(True)
 
+    def enable_start_time_editor(self):
+        self.TransferStartTimeEdit.setEnabled(True)
+
     def transfer(self, config, mianno, ac_time):
         """Transfer result to dataframe, triggered by okay button"""
 
         if self.ResetTimeCheckBox.isChecked():
             ac_time = self.ACTimeEditor.dateTime().toPyDateTime()
         else:
             ac_time = datetime.datetime.strptime(ac_time, "%Y%m%d-%H:%M:%S")
         
+        if self.ResetTransferStartTimeCheckBox.isChecked():
+            start_time = self.TransferStartTimeEdit.dateTime().toPyDateTime()
+            if start_time > ac_time:
+                delay_seconds = (start_time - ac_time).seconds
+                mianno._marker = mianno.marker[delay_seconds:]
+                mianno._start_end = mianno.start_end[delay_seconds:]
+                mianno._sleep_state = mianno.sleep_state[delay_seconds:]
+                ac_time = start_time
+        
         
         fd, _ = QFileDialog.getSaveFileName(self, "Save transfered result",
                                                 f"{config['gui']['openpath'].split('/')[0]}/transfer_result.xlsx", 
                                                 "*.xlsx;;")
         if fd == '':
             return
```

### Comparing `misleep-0.2.1b0/misleep/gui/main_window.py` & `misleep-0.2.2b0/misleep/gui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -912,14 +912,15 @@
 
             # Add marker label
             self.mianno.marker.append([sec, label_name])
 
             self.plot_marker_line()
         
             self.is_saved = False
+            self.AnnotationPathLabel.setText('*Annotation path:')
 
         if self.StartEndRadio.isChecked():
             x = round(event.xdata / self.midata.sf[
                         self.show_idx[np.where(self.signal_ax == event.inaxes)[0][0] - 1]
                     ]
                 , 3) + self.current_sec
             # start end ms 
@@ -1285,14 +1286,15 @@
             return
         
         if len(self.start_end) == 2:
             self.mianno.sleep_state[self.start_end[0]: self.start_end[1]] = \
                 [sleep_type] * (self.start_end[1] - self.start_end[0])
         
         self.is_saved = False
+        self.AnnotationPathLabel.setText('*Annotation path:')
         self.replot_sleep_state_bg(state=sleep_type)
         self.plot_hypo()
 
     def append_start_end(self):
         """Append start end label to self.mianno.start_end
         Triggered by self.AnnotateBt
         """
@@ -1315,14 +1317,15 @@
         # Add start_end label to self.mianno.start_end
         self.mianno.start_end.append(
             [self.start_end_ms[0], self.start_end_ms[1], label_name])
 
         self.plot_start_end_label_line()
     
         self.is_saved = False
+        self.AnnotationPathLabel.setText('*Annotation path:')
 
     def about_bar_dispatcher(self, signal):
         """Triggered by AboutBar action, show About dialog"""
         if signal.text() == "About":
             self.about_dialog.exec()
 
     def load_bar_dispatcher(self, signal):
@@ -1345,29 +1348,31 @@
         """Triggered by ToolBar action, transfer result"""
         if signal.text() == "Transfer Result":
             self.transfer_result()
 
     def transfer_result(self):
         """Transfer result into file"""
         self.transfer_result_dialog.ACTimeEditor.setDateTime(self.ac_time)
+        self.transfer_result_dialog.TransferStartTimeEdit.setDateTime(self.ac_time)
         self.transfer_result_dialog.exec_()
         if self.label_dialog.closed:
             return
         self.transfer_result_dialog.transfer(config=self.config,
                                              mianno=self.mianno,
                                              ac_time=self.midata.time)
 
     def save_anno(self):
         """Save annotation into file"""
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
         saved = save_thread.save_anno()
         if saved:
             self.is_saved = True
-            QMessageBox.about(self, "Info", "Annotation saved")
+            
+            self.AnnotationPathLabel.setText('Annotation path:')
         save_thread.quit()
 
     def save_data(self):
         """Save data into file"""
         
     
     def auto_save(self):
```

### Comparing `misleep-0.2.1b0/misleep/gui/resources/entire_logo.png` & `misleep-0.2.2b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/resources/logo.png` & `misleep-0.2.2b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/resources/misleep.py` & `misleep-0.2.2b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/spec_window.py` & `misleep-0.2.2b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/thread.py` & `misleep-0.2.2b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/uis/about_ui.py` & `misleep-0.2.2b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.2.2b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.2.2b0/misleep/gui/uis/main_window_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         self.label_4 = QtWidgets.QLabel(self.dockWidgetContents_3)
         self.label_4.setObjectName("label_4")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_4)
         self.DataPathEdit = QtWidgets.QLineEdit(self.dockWidgetContents_3)
         self.DataPathEdit.setReadOnly(True)
         self.DataPathEdit.setObjectName("DataPathEdit")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.DataPathEdit)
-        self.label_5 = QtWidgets.QLabel(self.dockWidgetContents_3)
-        self.label_5.setObjectName("label_5")
-        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_5)
+        self.AnnotationPathLabel = QtWidgets.QLabel(self.dockWidgetContents_3)
+        self.AnnotationPathLabel.setObjectName("AnnotationPathLabel")
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.AnnotationPathLabel)
         self.AnnoPathEdit = QtWidgets.QLineEdit(self.dockWidgetContents_3)
         self.AnnoPathEdit.setReadOnly(True)
         self.AnnoPathEdit.setObjectName("AnnoPathEdit")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.AnnoPathEdit)
         self.label_6 = QtWidgets.QLabel(self.dockWidgetContents_3)
         self.label_6.setObjectName("label_6")
         self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_6)
@@ -351,15 +351,15 @@
         QtCore.QMetaObject.connectSlotsByName(MiSleep)
 
     def retranslateUi(self, MiSleep):
         _translate = QtCore.QCoreApplication.translate
         MiSleep.setWindowTitle(_translate("MiSleep", "MiSleep"))
         self.MetaDock.setWindowTitle(_translate("MiSleep", "Meta"))
         self.label_4.setText(_translate("MiSleep", "Data path:"))
-        self.label_5.setText(_translate("MiSleep", "Annotation path:"))
+        self.AnnotationPathLabel.setText(_translate("MiSleep", "Annotation path:"))
         self.label_6.setText(_translate("MiSleep", "Acquisition Time:"))
         self.AcTimeEdit.setDisplayFormat(_translate("MiSleep", "yyyy/MM/dd HH:mm:ss"))
         self.ChannelDock.setWindowTitle(_translate("MiSleep", "Channel"))
         self.DeleteChBt.setText(_translate("MiSleep", "Delete"))
         self.HideChBt.setText(_translate("MiSleep", "Hide"))
         self.ScalerDownBt.setText(_translate("MiSleep", "-"))
         self.label.setText(_translate("MiSleep", "Scaler:"))
@@ -403,8 +403,8 @@
         self.actionShow.setText(_translate("MiSleep", "Show"))
         self.actionSave_data.setText(_translate("MiSleep", "Save Data"))
         self.actionSave_Annotation.setText(_translate("MiSleep", "Save Annotation"))
         self.actionAbout.setText(_translate("MiSleep", "About"))
         self.actionMerge_Data.setText(_translate("MiSleep", "Merge Data"))
         self.actionTransfer_Result.setText(_translate("MiSleep", "Transfer Result"))
         self.actionTransfer_Result.setToolTip(_translate("MiSleep", "Transfer Result"))
-from misleep.gui.resources import misleep
+from misleep.gui.resources import misleep
```

### Comparing `misleep-0.2.1b0/misleep/gui/uis/save_data_dialog_ui.py` & `misleep-0.2.2b0/misleep/gui/uis/save_data_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.2.2b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/gui/utils.py` & `misleep-0.2.2b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/io/annotation_io.py` & `misleep-0.2.2b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/io/base.py` & `misleep-0.2.2b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/io/signal_io.py` & `misleep-0.2.2b0/misleep/io/signal_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,20 @@
     try:
         # Use scipy to load
         raw_data = list(scipy_loadmat(data_path).values())[-1]
         names = raw_data.dtype.names
 
         # If old version misleep data
         if names is None:
-            signals = raw_data
-            channels = [f'ch{each + 1}' for each in range(raw_data.shape[0])]
-            sf = [305. for _ in range(raw_data.shape[0])]
+            if raw_data.shape[0] > raw_data.shape[1]:
+                signals = raw_data.T
+            else:
+                signals = raw_data
+            channels = [f'ch{each + 1}' for each in range(signals.shape[0])]
+            sf = [305. for _ in range(signals.shape[0])]
             time = datetime.datetime.now().strftime("%Y%m%d-%H:%M:%S")
             return MiData(signals=signals, channels=channels, sf=sf, time=time)
 
         raw_data = raw_data[0][0]
         # Whether saved by python
         if 'save' in names:
             channels = list(raw_data['channels'])
@@ -84,17 +87,21 @@
             sf = [float(each) for each in raw_data['sf']]
             signals = [raw_data[each] for each in channels]
             time = raw_data['time'][0]
             return MiData(signals=signals, channels=channels, sf=sf, time=time)
     
         except Exception:
             # If old version misleep data
-            signals = raw_data
-            channels = [f'ch{each + 1}' for each in range(raw_data.shape[0])]
-            sf = [305. for _ in range(raw_data.shape[0])]
+            if raw_data.shape[0] > raw_data.shape[1]:
+                signals = raw_data.T
+            else:
+                signals = raw_data
+            
+            channels = [f'ch{each + 1}' for each in range(signals.shape[0])]
+            sf = [305. for _ in range(signals.shape[0])]
             time = datetime.datetime.now().strftime("%Y%m%d-%H:%M:%S")
             return MiData(signals=signals, channels=channels, sf=sf, time=time)  
 
 
 def write_mat(signals, channels, sf, time, mat_file=None):
     """
     Write data to .mat file
```

### Comparing `misleep-0.2.1b0/misleep/preprocessing/spectral.py` & `misleep-0.2.2b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/utils/annotation.py` & `misleep-0.2.2b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/utils/signals.py` & `misleep-0.2.2b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/viz/hypnogram.py` & `misleep-0.2.2b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/viz/signals.py` & `misleep-0.2.2b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep/viz/spectral.py` & `misleep-0.2.2b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/misleep.egg-info/PKG-INFO` & `misleep-0.2.2b0/misleep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -33,15 +33,15 @@
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
-pip install misleep==0.1.3b
+pip install misleep==0.2.2b0
 ```
 
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into
```

### Comparing `misleep-0.2.1b0/misleep.egg-info/SOURCES.txt` & `misleep-0.2.2b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/setup.py` & `misleep-0.2.2b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.2.1 Beta"
+VERSION = "0.2.2b0"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.2.1b0/test/test_midata.py` & `misleep-0.2.2b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/test/test_signal_io.py` & `misleep-0.2.2b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/test/test_signals_viz.py` & `misleep-0.2.2b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.1b0/test/test_spectral_viz.py` & `misleep-0.2.2b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

