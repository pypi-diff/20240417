# Comparing `tmp/specvizitor-0.3.1.tar.gz` & `tmp/specvizitor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specvizitor-0.3.1.tar", max compression
+gzip compressed data, was "specvizitor-0.4.0.tar", max compression
```

## Comparing `specvizitor-0.3.1.tar` & `specvizitor-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
--rw-r--r--   0        0        0     1532 2023-02-09 15:18:12.389760 specvizitor-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     2960 2023-06-25 12:46:39.526235 specvizitor-0.3.1/README.md
--rw-r--r--   0        0        0      788 2023-07-14 17:33:24.061027 specvizitor-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.1/specvizitor/__init__.py
--rw-r--r--   0        0        0       31 2023-03-26 14:02:46.928611 specvizitor-0.3.1/specvizitor/__main__.py
--rw-r--r--   0        0        0     1370 2023-03-26 18:01:07.869089 specvizitor-0.3.1/specvizitor/appdata.py
--rw-r--r--   0        0        0      133 2023-07-13 11:53:21.467570 specvizitor-0.3.1/specvizitor/config/__init__.py
--rw-r--r--   0        0        0      465 2023-03-26 15:05:35.249523 specvizitor-0.3.1/specvizitor/config/appearance.py
--rw-r--r--   0        0        0      276 2023-03-22 23:56:11.227608 specvizitor-0.3.1/specvizitor/config/cache.py
--rw-r--r--   0        0        0      893 2023-07-13 17:03:20.853015 specvizitor-0.3.1/specvizitor/config/config.py
--rw-r--r--   0        0        0     2192 2023-07-14 14:11:47.060084 specvizitor-0.3.1/specvizitor/config/data_widgets.py
--rw-r--r--   0        0        0      226 2023-07-07 13:16:05.483242 specvizitor-0.3.1/specvizitor/config/spectral_lines.py
--rw-r--r--   0        0        0     2683 2023-03-13 17:19:17.930862 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:19:10.482762 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward.svg
--rw-r--r--   0        0        0     2672 2023-03-13 17:19:35.231095 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1526 2023-03-13 17:19:28.327002 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward.svg
--rw-r--r--   0        0        0     2096 2023-03-13 18:11:02.673646 specvizitor-0.3.1/specvizitor/data/icons/dark/dark-mode.svg
--rw-r--r--   0        0        0     3408 2023-03-13 17:12:33.185381 specvizitor-0.3.1/specvizitor/data/icons/dark/gear.svg
--rw-r--r--   0        0        0     5541 2023-03-13 17:27:50.753743 specvizitor-0.3.1/specvizitor/data/icons/dark/reset-dock-state.svg
--rw-r--r--   0        0        0     2062 2023-03-13 17:28:09.813997 specvizitor-0.3.1/specvizitor/data/icons/dark/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:40:05.591719 specvizitor-0.3.1/specvizitor/data/icons/dark/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.1/specvizitor/data/icons/dark/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/data/icons/dark/star.svg
--rw-r--r--   0        0        0     2682 2023-03-13 17:45:48.524369 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:42:40.537824 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward.svg
--rw-r--r--   0        0        0     2671 2023-03-13 17:45:37.424219 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1525 2023-03-13 17:45:42.380285 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward.svg
--rw-r--r--   0        0        0     2112 2023-03-13 17:45:23.436029 specvizitor-0.3.1/specvizitor/data/icons/light/dark-mode.svg
--rw-r--r--   0        0        0     3409 2023-03-13 17:44:57.135674 specvizitor-0.3.1/specvizitor/data/icons/light/gear.svg
--rw-r--r--   0        0        0     5540 2023-03-13 17:44:49.051565 specvizitor-0.3.1/specvizitor/data/icons/light/reset-dock-state.svg
--rw-r--r--   0        0        0     2063 2023-03-13 17:43:52.838804 specvizitor-0.3.1/specvizitor/data/icons/light/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:43:45.198700 specvizitor-0.3.1/specvizitor/data/icons/light/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.1/specvizitor/data/icons/light/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/data/icons/light/star.svg
--rw-r--r--   0        0        0      241 2023-07-13 17:13:08.073189 specvizitor-0.3.1/specvizitor/data/presets/config.yml
--rw-r--r--   0        0        0     1487 2023-07-14 14:11:47.032083 specvizitor-0.3.1/specvizitor/data/presets/data_widgets.yml
--rw-r--r--   0        0        0       35 2023-07-13 12:25:06.556814 specvizitor-0.3.1/specvizitor/data/presets/legacy.txt
--rw-r--r--   0        0        0     1493 2023-07-07 13:15:44.638933 specvizitor-0.3.1/specvizitor/data/presets/spectral_lines.yml
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.1/specvizitor/io/__init__.py
--rw-r--r--   0        0        0     1902 2023-03-22 20:25:42.255721 specvizitor-0.3.1/specvizitor/io/catalogue.py
--rw-r--r--   0        0        0     4747 2023-07-13 16:57:19.751915 specvizitor-0.3.1/specvizitor/io/inspection_data.py
--rw-r--r--   0        0        0     7192 2023-07-12 23:18:39.255228 specvizitor-0.3.1/specvizitor/io/viewer_data.py
--rw-r--r--   0        0        0     3399 2023-07-13 12:45:33.020219 specvizitor-0.3.1/specvizitor/main.py
--rw-r--r--   0        0        0        0 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/plugins/__init__.py
--rw-r--r--   0        0        0     6583 2023-07-14 17:20:41.934176 specvizitor-0.3.1/specvizitor/plugins/grizli.py
--rw-r--r--   0        0        0      445 2023-07-14 17:20:41.950176 specvizitor-0.3.1/specvizitor/plugins/plugin_core.py
--rw-r--r--   0        0        0        1 2023-03-13 11:54:43.456351 specvizitor-0.3.1/specvizitor/utils/__init__.py
--rw-r--r--   0        0        0     1131 2023-07-12 22:59:17.563036 specvizitor-0.3.1/specvizitor/utils/logs.py
--rw-r--r--   0        0        0     4330 2023-07-13 12:01:03.747251 specvizitor-0.3.1/specvizitor/utils/params.py
--rw-r--r--   0        0        0      776 2023-03-14 22:55:55.102789 specvizitor-0.3.1/specvizitor/utils/table_tools.py
--rw-r--r--   0        0        0      451 2023-03-24 14:14:40.377012 specvizitor-0.3.1/specvizitor/utils/widget_tools.py
--rw-r--r--   0        0        0      982 2023-03-22 17:47:30.671778 specvizitor-0.3.1/specvizitor/widgets/AbstractWidget.py
--rw-r--r--   0        0        0     7683 2023-07-14 17:16:26.498606 specvizitor-0.3.1/specvizitor/widgets/DataViewer.py
--rw-r--r--   0        0        0     4160 2023-03-22 20:25:42.283721 specvizitor-0.3.1/specvizitor/widgets/FileBrowser.py
--rw-r--r--   0        0        0     4650 2023-07-13 11:53:21.439570 specvizitor-0.3.1/specvizitor/widgets/Image2D.py
--rw-r--r--   0        0        0     1356 2023-07-13 11:54:42.376026 specvizitor-0.3.1/specvizitor/widgets/LazyViewerElement.py
--rw-r--r--   0        0        0    20188 2023-07-14 16:21:03.684717 specvizitor-0.3.1/specvizitor/widgets/MainWindow.py
--rw-r--r--   0        0        0     7917 2023-03-26 13:59:44.845098 specvizitor-0.3.1/specvizitor/widgets/NewFile.py
--rw-r--r--   0        0        0     5560 2023-03-26 18:01:07.881089 specvizitor-0.3.1/specvizitor/widgets/ObjectInfo.py
--rw-r--r--   0        0        0     9409 2023-07-13 17:25:57.015814 specvizitor-0.3.1/specvizitor/widgets/Plot1D.py
--rw-r--r--   0        0        0     2449 2023-03-22 17:47:30.659778 specvizitor-0.3.1/specvizitor/widgets/QuickSearch.py
--rw-r--r--   0        0        0     2766 2023-07-14 11:54:18.387960 specvizitor-0.3.1/specvizitor/widgets/ReviewForm.py
--rw-r--r--   0        0        0     3465 2023-03-22 19:59:56.339180 specvizitor-0.3.1/specvizitor/widgets/Section.py
--rw-r--r--   0        0        0     7339 2023-07-11 20:32:31.598754 specvizitor-0.3.1/specvizitor/widgets/Settings.py
--rw-r--r--   0        0        0     5279 2023-03-25 12:42:40.560273 specvizitor-0.3.1/specvizitor/widgets/SmartSlider.py
--rw-r--r--   0        0        0     8587 2023-07-14 14:35:42.596406 specvizitor-0.3.1/specvizitor/widgets/Spec1D.py
--rw-r--r--   0        0        0     3454 2023-03-23 00:24:35.185243 specvizitor-0.3.1/specvizitor/widgets/TableColumns.py
--rw-r--r--   0        0        0     7568 2023-07-14 16:28:29.607076 specvizitor-0.3.1/specvizitor/widgets/ToolBar.py
--rw-r--r--   0        0        0     4884 2023-07-13 11:54:56.392115 specvizitor-0.3.1/specvizitor/widgets/ViewerElement.py
--rw-r--r--   0        0        0        0 2023-03-13 12:09:30.251077 specvizitor-0.3.1/specvizitor/widgets/__init__.py
--rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 specvizitor-0.3.1/setup.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 specvizitor-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1532 2023-10-23 08:53:53.000000 specvizitor-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1351 2024-04-17 13:19:22.727160 specvizitor-0.4.0/README.md
+-rw-r--r--   0        0        0      903 2024-04-17 16:24:11.359970 specvizitor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/__init__.py
+-rw-r--r--   0        0        0       31 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/__main__.py
+-rw-r--r--   0        0        0     1412 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/appdata.py
+-rw-r--r--   0        0        0      136 2023-11-17 10:15:06.000000 specvizitor-0.4.0/specvizitor/config/__init__.py
+-rw-r--r--   0        0        0      549 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/appearance.py
+-rw-r--r--   0        0        0      316 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/cache.py
+-rw-r--r--   0        0        0     1403 2024-04-12 18:36:53.235882 specvizitor-0.4.0/specvizitor/config/config.py
+-rw-r--r--   0        0        0     2807 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/data_widgets.py
+-rw-r--r--   0        0        0      242 2023-11-17 10:15:06.000000 specvizitor-0.4.0/specvizitor/config/spectral_lines.py
+-rw-r--r--   0        0        0     2683 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward.svg
+-rw-r--r--   0        0        0     2672 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1526 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward.svg
+-rw-r--r--   0        0        0     2096 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/dark-mode.svg
+-rw-r--r--   0        0        0     3408 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/gear.svg
+-rw-r--r--   0        0        0     5541 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/reset-dock-state.svg
+-rw-r--r--   0        0        0     2062 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/star.svg
+-rw-r--r--   0        0        0     2682 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward.svg
+-rw-r--r--   0        0        0     2671 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1525 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward.svg
+-rw-r--r--   0        0        0     2112 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/dark-mode.svg
+-rw-r--r--   0        0        0     3409 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/gear.svg
+-rw-r--r--   0        0        0     5540 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/reset-dock-state.svg
+-rw-r--r--   0        0        0     2063 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/star.svg
+-rw-r--r--   0        0        0      347 2024-04-12 18:57:29.896161 specvizitor-0.4.0/specvizitor/data/presets/config.yml
+-rw-r--r--   0        0        0     2197 2024-04-16 15:53:33.245075 specvizitor-0.4.0/specvizitor/data/presets/data_widgets.yml
+-rw-r--r--   0        0        0       35 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/presets/legacy.txt
+-rw-r--r--   0        0        0     1957 2024-04-03 13:06:15.000000 specvizitor-0.4.0/specvizitor/data/presets/spectral_lines.yml
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/io/__init__.py
+-rw-r--r--   0        0        0     6617 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/io/catalog.py
+-rw-r--r--   0        0        0     7098 2024-04-14 10:45:37.736696 specvizitor-0.4.0/specvizitor/io/inspection_data.py
+-rw-r--r--   0        0        0    11659 2024-04-16 15:53:33.257075 specvizitor-0.4.0/specvizitor/io/viewer_data.py
+-rw-r--r--   0        0        0     3878 2024-03-21 12:29:30.000000 specvizitor-0.4.0/specvizitor/main.py
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/plugins/__init__.py
+-rw-r--r--   0        0        0      532 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/plugins/plugin_core.py
+-rw-r--r--   0        0        0     2920 2024-04-03 17:18:45.000000 specvizitor-0.4.0/specvizitor/plugins/sviz-eiger.py
+-rw-r--r--   0        0        0     6367 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/plugins/sviz-grizli.py
+-rw-r--r--   0        0        0        1 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/utils/__init__.py
+-rw-r--r--   0        0        0     1296 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/logs.py
+-rw-r--r--   0        0        0     4388 2024-03-15 11:33:34.000000 specvizitor-0.4.0/specvizitor/utils/params.py
+-rw-r--r--   0        0        0      954 2024-02-16 22:41:49.000000 specvizitor-0.4.0/specvizitor/utils/qt_tools.py
+-rw-r--r--   0        0        0      972 2023-12-07 21:01:49.000000 specvizitor-0.4.0/specvizitor/utils/widgets/AbstractWidget.py
+-rw-r--r--   0        0        0      521 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/ColorBar.py
+-rw-r--r--   0        0        0     4447 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/FileBrowser.py
+-rw-r--r--   0        0        0      713 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/MyViewBox.py
+-rw-r--r--   0        0        0    12377 2024-03-21 13:18:35.000000 specvizitor-0.4.0/specvizitor/utils/widgets/ParamTable.py
+-rw-r--r--   0        0        0     3465 2024-03-21 13:35:19.000000 specvizitor-0.4.0/specvizitor/utils/widgets/Section.py
+-rw-r--r--   0        0        0      208 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/__init__.py
+-rw-r--r--   0        0        0    14987 2024-04-17 15:17:46.467357 specvizitor-0.4.0/specvizitor/widgets/DataViewer.py
+-rw-r--r--   0        0        0     6898 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Image2D.py
+-rw-r--r--   0        0        0     3477 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/InspectionEditor.py
+-rw-r--r--   0        0        0     4647 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/InspectionResults.py
+-rw-r--r--   0        0        0    28172 2024-04-15 13:02:55.200442 specvizitor-0.4.0/specvizitor/widgets/MainWindow.py
+-rw-r--r--   0        0        0     7916 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/NewFile.py
+-rw-r--r--   0        0        0     5221 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/ObjectInfo.py
+-rw-r--r--   0        0        0     3854 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Plot1D.py
+-rw-r--r--   0        0        0     2537 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/QuickSearch.py
+-rw-r--r--   0        0        0    16112 2024-04-12 19:10:29.663993 specvizitor-0.4.0/specvizitor/widgets/Settings.py
+-rw-r--r--   0        0        0     6390 2024-04-15 16:03:47.642782 specvizitor-0.4.0/specvizitor/widgets/SmartSlider.py
+-rw-r--r--   0        0        0     4144 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Subsets.py
+-rw-r--r--   0        0        0     3454 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/TableColumns.py
+-rw-r--r--   0        0        0     7099 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/ToolBar.py
+-rw-r--r--   0        0        0    17618 2024-04-15 22:04:47.006961 specvizitor-0.4.0/specvizitor/widgets/ViewerElement.py
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/widgets/__init__.py
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 specvizitor-0.4.0/PKG-INFO
```

### Comparing `specvizitor-0.3.1/LICENSE.txt` & `specvizitor-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/appdata.py` & `specvizitor-0.4.0/specvizitor/appdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from astropy.table import Table
-
 from dataclasses import dataclass
 import logging
 import pathlib
 
+from .io.catalog import Catalog
 from .io.inspection_data import InspectionData
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class AppData:
 
     output_path: pathlib.Path | None = None  # the path to the output (a.k.a. inspection) file
-    cat: Table | None = None                 # the catalogue
-    review: InspectionData | None = None      # inspection results
+    cat: Catalog | None = None               # the catalogue
+    review: InspectionData | None = None     # inspection results
 
     j: int = None  # the index of the current object
 
     def create(self, **kwargs):
         """ Initialize the inspection data object.
         """
         if self.cat is None:
             logger.error("Failed to initialize inspection data: the catalogue not loaded to the memory")
             return
 
-        self.review = InspectionData.create(self.cat['id'], **kwargs)
+        self.review = InspectionData.create(*[list(self.cat.get_col(ind)) for ind in self.cat.indices], **kwargs)
 
     def read(self):
         """ Read the inspection file.
         """
         if self.output_path is None:
             logger.error("Failed to read the inspection file: the file path not specified")
             return
```

### Comparing `specvizitor-0.3.1/specvizitor/config/config.py` & `specvizitor-0.4.0/specvizitor/config/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 from dataclasses import dataclass, field
+from typing import Any
 
 from ..utils.params import Params
 
 
 @dataclass
 class Catalogue:
     filename: str | None = None
-    translate: dict[str, list[str]] | None = None
+    translate: dict[str, list[str]] = field(default_factory=dict)
 
 
 @dataclass
-class Data:
+class Image:
+    filename: str
+    wcs_source: str | None = None
+    loader: str = 'auto'
+    loader_params: dict[str, Any] = field(default_factory=dict)
+
+
+@dataclass
+class DataSource:
     dir: str = '.'
+    recursive_search: bool = False
+    images: dict[str, Image] = field(default_factory=dict)
     id_pattern: str = r'\d+'
-    enabled_unit_aliases: dict[str, str] | None = None
+    enabled_unit_aliases: dict[str, list[str]] = field(default_factory=dict)
 
 
 @dataclass
 class Appearance:
-    theme: str = 'light'
+    theme: str = 'dark'
     antialiasing: bool = False
     viewer_spacing: int = 5
     viewer_margins: int = 5
 
 
 @dataclass
-class ReviewForm:
-    default_flags: list[str] | None = None
+class InspectionResults:
+    default_flags: list[str] = field(default_factory=list)
+
+
+@dataclass
+class DataViewer:
+    redshift_step: float = 0.05
+    redshift_small_step: float = 0.0025
 
 
 @dataclass
 class Config(Params):
-    appearance: Appearance = field(default_factory=lambda: Appearance())
-    catalogue: Catalogue = field(default_factory=lambda: Catalogue())
-    data: Data = field(default_factory=lambda: Data())
-    review_form: ReviewForm = field(default_factory=lambda: ReviewForm())
+    appearance: Appearance = field(default_factory=Appearance)
+    catalogue: Catalogue = field(default_factory=Catalogue)
+    data: DataSource = field(default_factory=DataSource)
+    data_viewer: DataViewer = field(default_factory=DataViewer)
+    inspection_results: InspectionResults = field(default_factory=InspectionResults)
     plugins: list[str] = field(default_factory=list)
```

### Comparing `specvizitor-0.3.1/specvizitor/config/data_widgets.py` & `specvizitor-0.4.0/specvizitor/config/data_widgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,124 @@
 from dataclasses import dataclass, field
 from typing import Any
 
 from ..utils.params import Params
 
 
 @dataclass
+class Limits:
+    min: float | None = None
+    max: float | None = None
+
+
+@dataclass
+class ColorBarLimits(Limits):
+    type: str = 'minmax'
+
+
+@dataclass
 class Slider:
     visible: bool = True
+    link_to: str | None = None
 
     min_value: float = 0
     max_value: float = 100
     step: float = 1
     default_value: float = 0
 
-    name_in_catalogue: str | None = None
+    catalog_name: str | None = None
     show_text_editor: bool = False
     n_decimal_places: int = 6
 
+    show_save_button: bool = False
+
 
 @dataclass
 class ColorBar:
     visible: bool = True
+    link_to: str | None = None
+
+    limits: ColorBarLimits = field(default_factory=ColorBarLimits)
 
 
 @dataclass
-class Limits:
-    min: float | None = None
-    max: float | None = None
+class SpectralLines:
+    visible: bool = False
+    color: str | None = None
 
 
 @dataclass
-class Label:
-    position: str | None = None
+class LinePlot:
+    x: str
+    y: str
+    color: str | None = None
+    hide_label: bool = False
 
 
 @dataclass
 class Axis:
-    name: str | None = None
+    visible: bool = True
+    link_to: str | None = None
+
     unit: str | None = None
     scale: str = 'linear'
+    label: str | None = None
     limits: Limits = field(default_factory=Limits)
-    label: Label = field(default_factory=Label)
-
-
-@dataclass
-class LazyViewerElement:
-    visible: bool = True
-    position: str | None = None
-    relative_to: str | None = None
 
 
 @dataclass
 class DataElement:
+    source: str | None = None
     filename_keyword: str | None = None
     loader: str = 'auto'
-    loader_params: dict[str, Any] | None = None
+    loader_params: dict[str, Any] = field(default_factory=dict)
 
 
 @dataclass
-class ViewerElement(LazyViewerElement):
-    data: DataElement = field(default_factory=DataElement)
-    smoothing_slider: Slider = field(default_factory=lambda: Slider(max_value=3, step=0.05))
-    dock_title_fmt: str | None = None
+class ImageDataElement(DataElement):
+    cutout_size: float | None = None
 
 
 @dataclass
-class Image(ViewerElement):
-    rotate: int | None = None
-    scale: float | None = None
-    container: str = 'ViewBox'
-    color_bar: ColorBar = field(default_factory=ColorBar)
-    central_axes: str | None = None
-    crosshair: bool = False
+class ViewerElement:
+    visible: bool = True
+    position: str | None = None
+    relative_to: str | None = None
+    dock_title_fmt: str = 'short'
 
+    data: DataElement = field(default_factory=DataElement)
 
-@dataclass
-class Plot1D(ViewerElement):
     x_axis: Axis = field(default_factory=Axis)
     y_axis: Axis = field(default_factory=Axis)
 
+    spectral_lines: SpectralLines = field(default_factory=SpectralLines)
+    smoothing_slider: Slider = field(default_factory=lambda: Slider(max_value=3, step=0.05))
+    redshift_slider: Slider = field(default_factory=lambda: Slider(visible=False, max_value=10, step=1e-6,
+                                                                   show_text_editor=True, show_save_button=True))
+
+
+@dataclass
+class ImageCentralAxes:
+    x: bool = False
+    y: bool = False
+
 
 @dataclass
-class SpectrumRegion(LazyViewerElement):
-    window_size: str = '300 Angstrom'
+class Image(ViewerElement):
+    data: ImageDataElement = field(default_factory=ImageDataElement)
+
+    wcs_transform: bool = False
+    rotate: float | None = None
+    color_bar: ColorBar = field(default_factory=ColorBar)
+    central_axes: ImageCentralAxes = field(default_factory=ImageCentralAxes)
+    central_crosshair: bool = False
 
 
 @dataclass
-class Spectrum(Plot1D):
-    data: DataElement = field(default_factory=lambda: DataElement(loader='specutils'))
-    redshift_slider: Slider = field(default_factory=lambda: Slider(max_value=10, step=1e-4))
-    tracked_lines: dict[str, SpectrumRegion] | None = None
+class Plot1D(ViewerElement):
+    plots: dict[str, LinePlot] = field(default_factory=dict)
 
 
 @dataclass
 class DataWidgets(Params):
-    images: dict[str, Image] | None
-    plots: dict[str, Plot1D] | None
-    spectra: dict[str, Spectrum] | None
+    images: dict[str, Image] = field(default_factory=dict)
+    plots: dict[str, Plot1D] = field(default_factory=dict)
```

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward-starred.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward-starred.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/dark-mode.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/gear.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/reset-dock-state.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/reset-view.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/screenshot.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/star-empty.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/dark/star.svg` & `specvizitor-0.4.0/specvizitor/data/icons/dark/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward-starred.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward-starred.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/dark-mode.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/gear.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/reset-dock-state.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/reset-view.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/screenshot.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/star-empty.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/icons/light/star.svg` & `specvizitor-0.4.0/specvizitor/data/icons/light/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/data/presets/data_widgets.yml` & `specvizitor-0.4.0/specvizitor/data/presets/data_widgets.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,65 @@
 images:
   Image Cutout:
     data:
       filename_keyword: full.fits
       loader_params:
         extname: DSCI
-    crosshair: true
+    x_axis:
+      visible: false
+    y_axis:
+      visible: false
+    color_bar:
+      limits:
+        type: 'zscale'
+    central_crosshair: true
 
   Spectrum 2D:
     position: bottom
     relative_to: Image Cutout
+    dock_title_fmt: long
     data:
       filename_keyword: stack.fits
       loader_params:
         extname: SCI
-        extver: F444W
-    container: PlotItem
-    central_axes: x
+        extver_index: -1
+    x_axis:
+      link_to: Spectrum 1D
+    y_axis:
+      visible: false
+    color_bar: &cbar_defaults
+      limits:
+        type: user
+        min: -0.015
+        max: 0.015
+    central_axes:
+      x: true
+    redshift_slider:
+      visible: false
+      max_value: 10
+      step: 1.0e-6
+      link_to: Spectrum 1D
+    spectral_lines:
+      visible: true
 
   Line Map 1: &linemap_defaults
     position: right
     relative_to: Image Cutout
     data:
       filename_keyword: full.fits
       loader_params:
         extname: LINE
         silent: true
     dock_title_fmt: short
-    crosshair: true
+    x_axis:
+      visible: false
+    y_axis:
+      visible: false
+    color_bar: *cbar_defaults
+    central_crosshair: true
   Line Map 2: *linemap_defaults
   Line Map 3: *linemap_defaults
   Line Map 4: *linemap_defaults
   Line Map 5: *linemap_defaults
   Line Map 6: *linemap_defaults
   Line Map 7: *linemap_defaults
 
@@ -38,36 +67,46 @@
   Redshift PDF:
     position: right
     relative_to: Line Map 7
     data:
       filename_keyword: full.fits
     smoothing_slider:
       visible: False
-    x_axis:
-      name: zgrid
+    plots:
+      pdf:
+        x: zgrid
+        y: pdf
+        hide_label: true
     y_axis:
-      name: pdf
       scale: log
       limits:
         min: -3
 
-spectra:
   Spectrum 1D:
     position: bottom
     relative_to: Spectrum 2D
+    dock_title_fmt: long
     data:
       filename_keyword: 1D.fits
-      loader: specutils
+    x_axis:
+      label: wavelength
     y_axis:
-      label:
-        position: right
+      limits:
+        min: -0.5
+        max: 1.5
+    plots:
+      flux:
+        x: wave
+        y: flux
+      err:
+        x: wave
+        y: err
+        color: red
     redshift_slider:
-      min_value: 0
-      max_value: 12
-      step: 0.000001
-      default_value: 6
-      name_in_catalogue: redshift
-      show_text_editor: True
-    tracked_lines:
-      Ha:
-        position: right
-        relative_to: Redshift PDF
+      visible: true
+      max_value: 10
+      step: 1.0e-6
+      catalog_name: redshift
+      show_text_editor: true
+      show_save_button: true
+    spectral_lines:
+      visible: true
```

### Comparing `specvizitor-0.3.1/specvizitor/data/presets/spectral_lines.yml` & `specvizitor-0.4.0/specvizitor/data/presets/spectral_lines.yml`

 * *Files 17% similar despite different names*

```diff
@@ -12,34 +12,47 @@
   # Balmer series [1], [3]
   Ha: 6564.633
   Hb: 4862.688
   Hg: 4341.682
   Hd: 4102.897
   H7: 3971.195
   H8: 3890.151
+  H9: 3836.470
+  H10: 3798.980
+  H11: 3771.700
 
   # Paschen series [2]
   PaA: 18756.1
   PaB: 12821.6
   PaG: 10941.1
   PaD: 10052.1
   PaE: 9548.6
+  Pa10: 9231.5
+  Pa11: 9017.4
+  Pa12: 8865.2
 
   # Brackett series [2]
   BrA: 40522.6
   BrB: 26258.7
   BrG: 21661.2
   BrD: 19450.9
   BrE: 18179.1
+  Br10: 17366.9
+  Br11: 16811.1
+  Br12: 16411.7
 
   # Pfund series [2]
   PfB: 46537.8
   PfG: 37405.6
   PfD: 32969.9
   PfE: 30392.0
+  Pf11: 28730.0
+  Pf12: 27582.7
+  Pf13: 26751.3
+  Pf14: 26126.5
 
   # He-I lines [1], [3]
   HeI-3890: 3889.751
   HeI-5877: 5877.243
   HeI-6680: 6679.996
   HeI-7067: 7067.125
   HeI-1083 1: 10832.057
@@ -70,15 +83,33 @@
 
   # Carbon lines
   CIII 1: 1906.683
   CIII 2: 1908.734
   CIV 1: 1548.187
   CIV 2: 1550.770
 
+  # CO bands
+  CO(2-0): 22935.00
+  CO(3-1): 23227.00
+  CO(4-2): 23525.00
+  CO(5-3): 23829.00
+  CO(6-4): 24127.00
+  CO(7-5): 24425.00
+
   # Magnesium lines [1], [3]
   MgII 1: 2796.35
   MgII 2: 2803.53
 
+  # Neon lines
+  NeIII: 3870.16
+
+  # Iron lines
+  FeII-12570: 12570.0
+  FeII-16440: 16440.0
+
+  # PAHs
+  PAH 3.3mum: 32900.00
+
 # references:
 # [1] https://physics.nist.gov/PhysRefData/Handbook/Tables/hydrogentable2.htm
 # [2] https://www.gemini.edu/observing/resources/near-ir-resources/spectroscopy/hydrogen-recombination-lines
 # [3] http://www.astro.uu.se/valdwiki/Air-to-vacuum%20conversion
```

### Comparing `specvizitor-0.3.1/specvizitor/io/inspection_data.py` & `specvizitor-0.4.0/specvizitor/io/inspection_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,72 +6,103 @@
 from dataclasses import dataclass, field
 import logging
 import pathlib
 
 
 logger = logging.getLogger(__name__)
 
+REDSHIFT_FILL_VALUE = -1.0
+
 
 class WriterBase(ABC):
     @abstractmethod
     def write(self, df: pd.DataFrame, filename: pathlib.Path):
         pass
 
 
 class CSVWriter(WriterBase):
     def write(self, df: pd.DataFrame, filename: pathlib.Path):
-        df.to_csv(filename, index_label='id')
+        df.to_csv(filename)
 
 
 class FITSWriter(WriterBase):
     def write(self, df: pd.DataFrame, filename: pathlib.Path):
-        t: Table = Table.from_pandas(df)
+        t: Table = Table.from_pandas(df.reset_index())
         t.write(filename, overwrite=True)
 
 
 @dataclass
 class InspectionData:
     df: pd.DataFrame
-    default_columns: list[str] = field(default_factory=lambda: ['starred', 'comment'])
+    default_columns: list[str] = field(default_factory=lambda: ['starred', 'z_sviz', 'comment'])
+
+    @staticmethod
+    def _add_default_columns(df: pd.DataFrame):
+        # objects starred by the user
+        if 'starred' not in df.columns:
+            df['starred'] = False
+
+        # redshifts saved by the user
+        if 'z_sviz' not in df.columns:
+            df['z_sviz'] = REDSHIFT_FILL_VALUE
+
+        # column for user comments
+        if 'comment' not in df.columns:
+            df['comment'] = ''
+        else:
+            df['comment'] = df['comment'].fillna('')
+
+        return df
 
     @classmethod
-    def create(cls, ids, flags: list[str] | None = None):
+    def create(cls, *args, flags: list[str] | None = None):
         """ Create a new instance of the InspectionData class with a Pandas dataframe containing:
               - a column of IDs;
               - a column for comments;
               - one column per each user-defined flag.
-        @param ids: the list of IDs
         @param flags: the list of user-defined flags
         @return: an instance of the InspectionData class
         """
 
-        df = pd.DataFrame(index=ids).sort_index()
-        df['starred'] = False
-        df['comment'] = ''
+        try:
+            if len(args) == 1:
+                index = pd.Index(args[0], name='id')
+            else:
+                index = pd.MultiIndex.from_arrays(args, names=('id',) + tuple(f'id{i + 1}' for i in range(1, len(args))))
+        except TypeError as e:
+            logger.error(f'Failed to create the inspection file: {e}')
+            return None
+
+        df = pd.DataFrame(index=index)
+        df = cls._add_default_columns(df)
+
+        review = cls(df=df)
 
         if flags is not None:
             for cname in flags:
-                df[cname] = False
+                review.add_flag_column(cname)
 
-        return cls(df=df)
+        return review
 
     @classmethod
     def read(cls, filename: str | pathlib.Path):
         """ Read an existing inspection file
         @param filename: the input filename
         @return: an instance of the InspectionData class
         """
 
         # TODO: validate the input
         df = pd.read_csv(filename, index_col='id')
 
-        if 'starred' not in df.columns:
-            df['starred'] = False
+        i = 1
+        while f'id{i + 1}' in df.columns:
+            df.set_index(f'id{i + 1}', append=True, inplace=True)
+            i += 1
 
-        df['comment'] = '' if 'comment' not in df.columns else df['comment'].fillna('')
+        df = cls._add_default_columns(df)
 
         review = cls(df=df)
         review.reorder_columns()
 
         return review
 
     def write(self, filename: pathlib.Path, fmt: str = 'csv'):
@@ -96,56 +127,95 @@
     def n_objects(self) -> int | None:
         """
         @return: the total number of objects under inspection.
         """
         return len(self.df)
 
     @property
-    def ids(self) -> np.array:
+    def ids(self):
+        """ Primary IDs.
+        """
+        return self.df.index.get_level_values(0)
+
+    @property
+    def ids_full(self):
+        """ All available IDs.
+        """
         return self.df.index.values
 
     @property
     def ids_are_int(self) -> bool:
-        return pd.api.types.is_integer_dtype(self.df.index)
+        return pd.api.types.is_integer_dtype(self.ids)
+
+    @property
+    def indices(self) -> list[str]:
+        return self.df.index.names
 
     @property
     def user_defined_columns(self) -> list[str]:
         return [cname for cname in self.df.columns if cname not in self.default_columns]
 
     @property
     def flag_columns(self) -> list[str]:
         return [cname for cname in self.user_defined_columns if pd.api.types.is_bool_dtype(self.df[cname])]
 
-    @property
-    def has_starred(self) -> bool:
-        return self.df['starred'].sum() > 0
+    def add_flag_column(self, column_name: str):
+        self.df[column_name] = False
 
     def reorder_columns(self):
         self.df = self.df[self.default_columns + self.user_defined_columns]
 
+    def rename_column(self, old_name: str, new_name: str):
+        if old_name not in self.user_defined_columns:
+            logger.error(f"Failed to rename a column: Column not found (column: {old_name})")
+            return
+        self.df.rename(columns={old_name: new_name}, inplace=True)
+
+    def delete_column(self, column_name: str):
+        if column_name not in self.user_defined_columns:
+            logger.error(f"Failed to delete a column: Column not found (column: {column_name})")
+            return
+        self.df.drop(column_name, axis=1, inplace=True)
+
+    def to_list(self):
+        return self.df.values.tolist()
+
+    def has_data(self, column_name: str) -> bool:
+        if column_name in self.flag_columns or column_name == 'starred':
+            return self.df[column_name].sum() > 0
+        else:
+            logger.warning(f"Cannot determine if a column has data or not (column: {column_name})")
+            return True
+
     def get_value(self, j: int, cname: str):
         return self.df.iat[j, self.df.columns.get_loc(cname)]
 
-    def get_id(self, j: int) -> int | str | None:
+    def get_id(self, j: int, full=False) -> str | int | tuple | None:
         try:
-            obj_id = self.ids[j]
+            obj_id = self.ids[j] if not full else self.ids_full[j]
         except (TypeError, IndexError):
             return
 
-        if self.ids_are_int:
-            # convert from int64 to int
+        if self.ids_are_int and not isinstance(obj_id, tuple):
+            # convert int64 to int
             obj_id = int(obj_id)
 
         return obj_id
 
-    def get_id_loc(self, obj_id: str):
+    def get_id_loc(self, obj_id: str | int) -> int:
         if self.ids_are_int:
             obj_id = int(obj_id)
 
-        return self.df.index.get_loc(obj_id)
+        j = self.df.index.get_loc(obj_id)
+        if isinstance(j, slice):
+            j = j.start  # use the first available secondary ID
+        elif isinstance(j, np.ndarray):
+            j = np.argmax(j)
+
+        return int(j)
 
     def update_value(self, j: int, cname: str, value):
         self.df.iat[j, self.df.columns.get_loc(cname)] = value
 
     def validate_id(self, obj_id: str | int) -> bool:
         if self.ids_are_int:
             try:
```

### Comparing `specvizitor-0.3.1/specvizitor/main.py` & `specvizitor-0.4.0/specvizitor/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import argparse
 import importlib
 import logging
 import pathlib
 from platformdirs import user_config_dir, user_cache_dir
 import sys
 
-from .config.appearance import set_up_appearance
-from .config import Config, DataWidgets, SpectralLines, Cache
-from .io.viewer_data import add_enabled_aliases
+from .config.appearance import setup_appearance
+from .config import Config, DataWidgets, SpectralLineData, Cache
+from .io.viewer_data import add_unit_aliases
 from .utils.params import LocalFile
 
 from .widgets.MainWindow import MainWindow
 
 logger = logging.getLogger(__name__)
 
 ORGANIZATION_NAME = 'FRESCO'
@@ -56,37 +56,50 @@
 
         for f in local_files.values():
             f.delete()  # safe delete
 
     config = Config.read_user_params(local_files['config'], default='config.yml')
 
     # register unit aliases
-    if config.data.enabled_unit_aliases is not None:
-        add_enabled_aliases(config.data.enabled_unit_aliases)
+    add_unit_aliases(config.data.enabled_unit_aliases)
 
-    # start the application
-    app = QtWidgets.QApplication(sys.argv)
-    app.setOrganizationName(ORGANIZATION_NAME)
-    app.setApplicationName(APPLICATION_NAME.capitalize())
-    logger.info("Application started")
-
-    # set up the GUI appearance
-    set_up_appearance(cfg=config.appearance)
-
-    # "discover" and "register" plugins (to be updated)
-    plugins = [importlib.import_module("specvizitor.plugins." + plugin_name).Plugin()
-               for plugin_name in config.plugins]
-
-    # create the main window
-    window = MainWindow(config=config,
-                        cache=Cache.read_user_params(local_files['cache']),
-                        viewer_cfg=DataWidgets.read_user_params(local_files['widgets'], default='data_widgets.yml'),
-                        spectral_lines=SpectralLines.read_user_params(local_files['lines'],
-                                                                      default='spectral_lines.yml'),
-                        plugins=plugins)
-    window.show()
+    # "discover" and "register" plugins
+    plugins = []
+    undiscovered_plugins = []
+    for plugin_name in config.plugins:
+        try:
+            plugins.append(importlib.import_module("specvizitor.plugins." + plugin_name).Plugin())
+        except ModuleNotFoundError:
+            logger.warning(f'Plugin not found: {plugin_name}')
+            undiscovered_plugins.append(plugin_name)
+
+    config.plugins = [plugin_name for plugin_name in config.plugins if plugin_name not in undiscovered_plugins]
+    config.save()
+
+    exit_code = MainWindow.EXIT_CODE_REBOOT
+    while exit_code == MainWindow.EXIT_CODE_REBOOT:
+        # start the application
+        app = QtWidgets.QApplication(sys.argv)
+        app.setOrganizationName(ORGANIZATION_NAME)
+        app.setApplicationName(APPLICATION_NAME.capitalize())
+        logger.info("Application started")
+
+        # set up the GUI appearance
+        setup_appearance(cfg=config.appearance)
+
+        # create the main window
+        window = MainWindow(config=config,
+                            cache=Cache.read_user_params(local_files['cache']),
+                            widget_cfg=DataWidgets.read_user_params(local_files['widgets'], default='data_widgets.yml'),
+                            spectral_lines=SpectralLineData.read_user_params(local_files['lines'],
+                                                                             default='spectral_lines.yml'),
+                            plugins=plugins)
+        window.show()
 
-    sys.exit(app.exec_())
+        exit_code = app.exec_()
+        app = None
+
+    sys.exit(exit_code)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `specvizitor-0.3.1/specvizitor/utils/logs.py` & `specvizitor-0.4.0/specvizitor/utils/logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 import logging
 
 from qtpy import QtWidgets
 
 
 class QLogHandler(logging.Handler):
     def emit(self, record):
-        LogMessageBox(record.levelno, record.msg, parent=QtWidgets.QApplication.focusWidget())
+        msg = record.msg
+        if isinstance(msg, Exception):
+            msg = str(msg)
+            if msg.startswith("'") and msg.endswith("'"):
+                msg = msg[1:-1]
+        LogMessageBox(record.levelno, msg, parent=QtWidgets.QApplication.focusWidget())
 
 
 class LogMessageBox(QtWidgets.QMessageBox):
     PACKAGE = __package__.split('.')[0].capitalize()  # the name of the top-level package
 
     LOGGING_LEVELS = {
         logging.INFO: QtWidgets.QMessageBox.Information,
         logging.WARNING: QtWidgets.QMessageBox.Warning,
         logging.ERROR: QtWidgets.QMessageBox.Warning,
         logging.CRITICAL: QtWidgets.QMessageBox.Critical
     }
 
     def __init__(self, level: int, message: str, parent=None):
-        super().__init__(LogMessageBox.LOGGING_LEVELS[level], '{} Message'.format(self.PACKAGE), message, parent=parent)
+        super().__init__(self.LOGGING_LEVELS[level], '{} Message'.format(self.PACKAGE), message, parent=parent)
         self.show()
 
 
 def qlog(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         root_logger = logging.getLogger()
```

### Comparing `specvizitor-0.3.1/specvizitor/utils/params.py` & `specvizitor-0.4.0/specvizitor/utils/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,23 +87,23 @@
         try:
             user_params = read_yaml(file.path)
         except FileNotFoundError:
             pass
         except yaml.YAMLError:
             logger.error(f'Failed to parse `{file.path}`. The file will be overwritten.')
         else:
-            # TODO: patch the user config file using dictdiffer
             try:
+                # TODO: patch the user config file using dictdiffer
                 user_params = dacite.from_dict(data_class=cls, data=user_params, config=dacite.Config())
             except (WrongTypeError, MissingValueError):
                 user_params = None
                 logger.error(f'Failed to create a dataclass from `{file.path}`. The file will be overwritten.')
 
         if user_params is None:
-            file.backup()
+            file.delete()
         else:
             params = user_params
 
         params._user_file = file
         params.save()
 
         return params
@@ -131,15 +131,15 @@
 
     def get_user_params_filename(self) -> str | None:
         return str(self._user_file.path.resolve()) if self._user_file is not None else None
 
 
 def read_yaml(filename) -> dict:
     with open(filename, "r") as yaml_file:
-        return yaml.safe_load(yaml_file)
+        return yaml.safe_load(yaml_file) or {}  # return empty dictionary if the file is empty
 
 
 def filter_none_values(data):
     if isinstance(data, dict):
         return {k: filter_none_values(v) for k, v in data.items() if v is not None}
     return data
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/AbstractWidget.py` & `specvizitor-0.4.0/specvizitor/utils/widgets/AbstractWidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from qtpy import QtWidgets
 
 import abc
 
-from ..utils.widget_tools import get_widgets
+from ..qt_tools import get_widgets
 
 
 class QtAbcMeta(type(QtWidgets.QWidget), type(abc.ABC)):
     pass
 
 
 class AbstractWidget(QtWidgets.QWidget, abc.ABC, metaclass=QtAbcMeta):
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/FileBrowser.py` & `specvizitor-0.4.0/specvizitor/utils/widgets/FileBrowser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 import qtpy.compat
-from qtpy import QtWidgets
+from qtpy import QtCore, QtWidgets
 
 import logging
 import pathlib
 
 from .AbstractWidget import AbstractWidget
 
 logger = logging.getLogger(__name__)
 
 
 class FileBrowser(AbstractWidget):
+    textChanged = QtCore.Signal(str)
+
     OpenFile = 0
     # OpenFiles = 1
     OpenDirectory = 2
     SaveFile = 3
 
     def __init__(self, mode=OpenFile, filename_extensions='All files (*.*)', default_path=None,
-                 title: str = '', title_width: int | None = None, button_text='Browse...', parent=None):
+                 title: str = '', title_width: int | None = None, button_text='Browse...',
+                 line_edit_width=700, parent=None):
 
         self._browser_mode = mode
         self._filter = filename_extensions  # example: 'Images (*.png *.xpm *.jpg);;Text files (*.txt)'
         self._default_path = None if default_path is None else str(pathlib.Path(default_path).resolve())
 
         self._title = title
         self._title_width = title_width
         self._button_text = button_text
+        self._line_edit_width = line_edit_width
 
         self._label: QtWidgets.QLabel | None = None
         self._line_edit: QtWidgets.QLineEdit | None = None
         self._button: QtWidgets.QPushButton | None = None
 
         super().__init__(parent=parent)
 
     def init_ui(self):
         self._label = QtWidgets.QLabel(self._title, self)
         if self._title_width is None:
             self._label.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum)
         else:
             self._label.setFixedWidth(self._title_width)
+        if not self._title:
+            self._label.setVisible(False)
 
         self._line_edit = QtWidgets.QLineEdit(self)
-        self._line_edit.setMinimumWidth(700)
+        self._line_edit.setMinimumWidth(self._line_edit_width)
         self._line_edit.setText(self._default_path)
 
         self._button = QtWidgets.QPushButton(self._button_text, self)
         self._button.setFixedWidth(120)
 
+        self._line_edit.textChanged.connect(self.textChanged.emit)
         self._button.clicked.connect(self._browse)
 
     def set_layout(self):
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
 
     def populate(self):
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/MainWindow.py` & `specvizitor-0.4.0/specvizitor/widgets/MainWindow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,112 @@
-from astropy.table import Table
 import qtpy.compat
 from qtpy import QtWidgets, QtCore, QtGui
+import numpy as np
 
 from dataclasses import asdict
 from importlib.metadata import version
 import logging
 import pathlib
 
 from ..appdata import AppData
-from ..config import config as cfg
-from ..config.appearance import set_up_appearance
-from ..config import Config, Cache, DataWidgets, SpectralLines
-from ..io.catalogue import read_cat, create_cat
+from ..config import Config, Cache, DataWidgets, SpectralLineData
+from ..config.appearance import setup_appearance
+from ..io.catalog import Catalog
 from ..io.inspection_data import InspectionData
-from ..utils.logs import LogMessageBox
+from ..plugins.plugin_core import PluginCore
 from ..utils.params import save_yaml
 
 from .DataViewer import DataViewer
 from .NewFile import NewFile
 from .ObjectInfo import ObjectInfo
 from .QuickSearch import QuickSearch
-from .ReviewForm import ReviewForm
+from .InspectionResults import InspectionResults
+from .InspectionEditor import InspectionEditor
+from .Subsets import Subsets
 from .Settings import Settings
 from .ToolBar import ToolBar
 
 logger = logging.getLogger(__name__)
 
 
 class MainWindow(QtWidgets.QMainWindow):
+    EXIT_CODE_REBOOT = -42
+
     project_loaded = QtCore.Signal(InspectionData)
+    object_selected = QtCore.Signal(int, InspectionData, object)
     data_requested = QtCore.Signal()
-    object_selected = QtCore.Signal(int, InspectionData, Table, cfg.Data)
+    save_action_invoked = QtCore.Signal()
+    delete_action_invoked = QtCore.Signal()
 
     theme_changed = QtCore.Signal()
     catalogue_changed = QtCore.Signal(object)
+    data_source_changed = QtCore.Signal()
+    spectral_lines_changed = QtCore.Signal()
     visible_columns_updated = QtCore.Signal(list)
     dock_layout_updated = QtCore.Signal(dict)
     viewer_configuration_updated = QtCore.Signal(DataWidgets)
 
+    starred_state_updated = QtCore.Signal(bool, bool)
     screenshot_path_selected = QtCore.Signal(str)
 
-    def __init__(self, config: Config, cache: Cache, viewer_cfg: DataWidgets,
-                 spectral_lines: SpectralLines | None = None, plugins=None, parent=None):
+    subset_loaded = QtCore.Signal(str, object)
+    subset_inspection_paused = QtCore.Signal(bool)
+    subset_inspection_stopped = QtCore.Signal()
+
+    zen_mode_activated = QtCore.Signal()
+    zen_mode_deactivated = QtCore.Signal()
+
+    def __init__(self,
+                 config: Config | None = None,
+                 cache: Cache | None = None,
+                 widget_cfg: DataWidgets | None = None,
+                 spectral_lines: SpectralLineData | None = None,
+                 plugins: list[PluginCore] | None = None,
+                 parent=None):
+
         super().__init__(parent)
 
         self.rd = AppData()
-        
-        self._config = config
-        self._cache = cache
 
-        self._viewer_cfg = viewer_cfg
-        self._spectral_lines = spectral_lines
+        self._config = config if config else Config()
+        self._cache = cache if cache else Cache()
+        self._widget_cfg = widget_cfg if widget_cfg else DataWidgets()
+        self._spectral_lines = spectral_lines if spectral_lines else SpectralLineData()
+        self._plugins: list[PluginCore] = plugins if plugins is not None else []
+
+        self._subset_cat: Catalog | None = None
+        self._subset_inspection_paused: bool = False
 
-        self._plugins = plugins
+        self._restart_requested = False
 
+        self.interface_hidden: bool = False
         self.was_maximized: bool = False
         self.setFocusPolicy(QtCore.Qt.StrongFocus)
 
         self._update_window_title()  # set the title of the main window
         # self.setWindowIcon(QtGui.QIcon('logo2_2.png'))
 
         # add a status bar
         # self.statusBar().showMessage("Message in the statusbar")
 
+        QtWidgets.QShortcut('Ctrl+S', self, self.save_action_invoked.emit)
+        QtWidgets.QShortcut('Ctrl+D', self, self.delete_action_invoked.emit)
+        QtWidgets.QShortcut('Esc', self, lambda: self._exit_fullscreen() if self.isFullScreen() else None)
+
         self._data_viewer: DataViewer | None = None
         self._commands_bar: ToolBar | None = None
         self._quick_search: QuickSearch | None = None
         self._object_info: ObjectInfo | None = None
-        self._review_form: ReviewForm | None = None
+        self._inspection_res: InspectionResults | None = None
+        self._subsets: Subsets | None = None
 
         self._quick_search_dock: QtWidgets.QDockWidget | None = None
         self._object_info_dock: QtWidgets.QDockWidget | None = None
-        self._review_form_dock: QtWidgets.QDockWidget | None = None
+        self._inspection_res_dock: QtWidgets.QDockWidget | None = None
+        self._subsets_dock: QtWidgets.QDockWidget | None = None
 
         self.init_ui()
         self.populate()
         self.connect()
 
         self.restore_window_state()
 
@@ -88,25 +119,30 @@
             self.load_catalogue()
 
         # update the list of catalogue columns visible in the object info widget
         # write "is not None" explicitly in case visible_columns == []
         if self.rd.cat and self._cache.visible_columns is not None:
             self.visible_columns_updated.emit(self._cache.visible_columns)
 
+        # load the subset to the memory
+        if self._cache.last_subset_file:
+            self.load_subset(reset_index=False)
+
         # read cache and try to load the last active project
         if self._cache.last_inspection_file:
             self.open_file(self._cache.last_inspection_file, self._cache.last_object_index)
 
     def init_ui(self):
         # create a central widget
-        self._data_viewer = DataViewer(self._viewer_cfg, self._config.appearance,
-                                       spectral_lines=self._spectral_lines, plugins=self._plugins, parent=self)
+        self._data_viewer = DataViewer(self._config.data_viewer, self._config.data, self._widget_cfg,
+                                       self._config.appearance, spectral_lines=self._spectral_lines,
+                                       plugins=self._plugins, parent=self)
 
         # create a toolbar
-        self._commands_bar = ToolBar(self.rd, self._config.appearance, parent=self)
+        self._commands_bar = ToolBar(self._config.appearance, parent=self)
         self._commands_bar.setObjectName('Toolbar')
         self._commands_bar.setEnabled(True)
 
         # create a quick search widget
         self._quick_search = QuickSearch(parent=self)
         self._quick_search_dock = QtWidgets.QDockWidget('Quick Search', self)
         self._quick_search_dock.setObjectName('Quick Search')
@@ -115,18 +151,24 @@
         # create a widget displaying information about the object
         self._object_info = ObjectInfo(parent=self)
         self._object_info_dock = QtWidgets.QDockWidget('Object Information', self)
         self._object_info_dock.setObjectName('Object Information')
         self._object_info_dock.setWidget(self._object_info)
 
         # create a widget for writing comments
-        self._review_form = ReviewForm(cfg=self._config.review_form, parent=self)
-        self._review_form_dock = QtWidgets.QDockWidget('Review Form', self)
-        self._review_form_dock.setObjectName('Review Form')
-        self._review_form_dock.setWidget(self._review_form)
+        self._inspection_res = InspectionResults(cfg=self._config.inspection_results, parent=self)
+        self._inspection_res_dock = QtWidgets.QDockWidget('Inspection Results', self)
+        self._inspection_res_dock.setObjectName('Inspection Results')
+        self._inspection_res_dock.setWidget(self._inspection_res)
+
+        # create a widget for inspecting a subset of objects
+        self._subsets = Subsets(parent=self)
+        self._subsets_dock = QtWidgets.QDockWidget('Subsets', self)
+        self._subsets_dock.setObjectName('Subsets')
+        self._subsets_dock.setWidget(self._subsets)
 
         self._init_menu()
 
     def _init_menu(self):
         self._menu = self.menuBar()
 
         self._file = self._menu.addMenu("&File")
@@ -139,62 +181,55 @@
         self._open_file = QtWidgets.QAction("&Open...")
         self._open_file.triggered.connect(self._open_file_action)
         self._open_file.setShortcut(QtGui.QKeySequence('Ctrl+O'))
         self._file.addAction(self._open_file)
 
         self._file.addSeparator()
 
-        self._save = QtWidgets.QAction("&Save...")
-        self._save.triggered.connect(self._save_action)
-        self._save.setShortcut(QtGui.QKeySequence('Ctrl+S'))
-        self._save.setEnabled(False)
-        self._file.addAction(self._save)
-
-        self._save_as = QtWidgets.QAction("Save As...")
-        self._save_as.triggered.connect(self._save_as_action)
-        self._save_as.setShortcut(QtGui.QKeySequence('Shift+Ctrl+S'))
-        self._save_as.setEnabled(False)
-        self._file.addAction(self._save_as)
-
-        self._file.addSeparator()
-
         self._export = QtWidgets.QAction("&Export FITS Table...")
         self._export.triggered.connect(self._export_action)
         self._export.setEnabled(False)
         self._file.addAction(self._export)
 
         self._file.addSeparator()
 
-        self._quit = QtWidgets.QAction("&Quit...")
+        self._quit = QtWidgets.QAction("&Quit")
         self._quit.triggered.connect(self._exit_action)
         self._quit.setShortcut(QtGui.QKeySequence('Ctrl+Q'))
         self._file.addAction(self._quit)
 
         self._view = self._menu.addMenu("&View")
 
         self._reset_view = QtWidgets.QAction("Reset View")
         self._reset_view.setEnabled(False)
         self._reset_view.triggered.connect(self._data_viewer.view_reset.emit)
+        self._reset_view.setShortcut('F5')
         self._view.addAction(self._reset_view)
 
         self._reset_dock_layout = QtWidgets.QAction("Reset Layout")
         self._reset_dock_layout.setEnabled(False)
         self._reset_dock_layout.triggered.connect(self._data_viewer.init_docks)
         self._view.addAction(self._reset_dock_layout)
 
         self._view.addSeparator()
 
+        self._zen = QtWidgets.QAction("Hide Interface")
+        self._zen.triggered.connect(lambda:
+                                    self._hide_interface() if not self.interface_hidden else self._show_interface())
+        self._zen.setShortcut('H')
+        self._view.addAction(self._zen)
+
+        self._view.addSeparator()
+
         self._fullscreen = QtWidgets.QAction("Fullscreen")
         self._fullscreen.triggered.connect(lambda:
                                            self._exit_fullscreen() if self.isFullScreen() else self._enter_fullscreen())
         self._fullscreen.setShortcut('F11')
         self._view.addAction(self._fullscreen)
 
-        QtWidgets.QShortcut('Esc', self, lambda: self._exit_fullscreen() if self.isFullScreen() else None)
-
         self._widgets = self._menu.addMenu("&Widgets")
 
         self._add_widget = QtWidgets.QAction("Add...")
         self._add_widget.setEnabled(False)
         self._widgets.addAction(self._add_widget)
 
         self._widgets.addSeparator()
@@ -205,14 +240,18 @@
 
         self._restore_viewer_config = QtWidgets.QAction("Restore...")
         self._restore_viewer_config.triggered.connect(self._restore_viewer_config_action)
         self._widgets.addAction(self._restore_viewer_config)
 
         self._tools = self._menu.addMenu("&Tools")
 
+        self._inspect_subset = QtWidgets.QAction("Inspect Subset...")
+        self._inspect_subset.triggered.connect(self._inspect_subset_action)
+        self._tools.addAction(self._inspect_subset)
+
         self._screenshot = QtWidgets.QAction("Take Screenshot...")
         self._screenshot.triggered.connect(self._screenshot_action)
         self._tools.addAction(self._screenshot)
 
         self._tools.addSeparator()
 
         self._settings = QtWidgets.QAction("Se&ttings...")
@@ -222,58 +261,81 @@
         self._help = self._menu.addMenu("&Help")
         self._about = QtWidgets.QAction("&About...")
         self._about.triggered.connect(self._about_action)
         self._help.addAction(self._about)
 
     def connect(self):
         # connect the main window to the child widgets
-        for w in (self._data_viewer, self._commands_bar, self._quick_search, self._object_info, self._review_form):
+        for w in (self._data_viewer, self._commands_bar, self._quick_search, self._object_info, self._inspection_res,
+                  self._subsets):
             self.project_loaded.connect(w.load_project)
 
-        for w in (self._data_viewer, self._object_info, self._review_form):
+        for w in (self._data_viewer, self._object_info, self._inspection_res):
             self.data_requested.connect(w.collect)
 
-        for w in (self._data_viewer, self._commands_bar, self._object_info, self._review_form):
+        for w in (self._data_viewer, self._commands_bar, self._object_info, self._inspection_res, self._subsets):
             self.object_selected.connect(w.load_object)
 
         self.theme_changed.connect(self._data_viewer.init_ui)
-        self.theme_changed.connect(self._commands_bar.set_icons)
+        self.theme_changed.connect(self._commands_bar._set_icons)
         self.catalogue_changed.connect(self._object_info.update_table_items)
+        self.data_source_changed.connect(self._data_viewer.load_field_images)
+        self.spectral_lines_changed.connect(self._data_viewer.spectral_lines_changed.emit)
         self.visible_columns_updated.connect(self._object_info.update_visible_columns)
-
         self.dock_layout_updated.connect(self._data_viewer.restore_dock_layout)
         self.viewer_configuration_updated.connect(self._data_viewer.update_viewer_configuration)
 
+        self.starred_state_updated.connect(self._commands_bar.update_star_button_icon)
         self.screenshot_path_selected.connect(self._data_viewer.take_screenshot)
 
+        self.subset_loaded.connect(self._subsets.load_subset)
+        self.subset_inspection_paused.connect(self._subsets.pause_inspecting_subset)
+        self.subset_inspection_stopped.connect(self._subsets.stop_inspecting_subset)
+
+        self.save_action_invoked.connect(self._data_viewer.request_redshift)
+        self.delete_action_invoked.connect(self._inspection_res.clear_redshift_value)
+
+        self.zen_mode_activated.connect(self._data_viewer.hide_interface)
+        self.zen_mode_deactivated.connect(self._data_viewer.restore_visibility)
+
         # connect the child widgets to the main window
-        self._quick_search.id_selected.connect(self._select_by_id)
-        self._quick_search.index_selected.connect(self._select_by_index)
-        self._commands_bar.object_selected.connect(self.load_object)
+        self._quick_search.id_selected.connect(self.load_by_id)
+        self._quick_search.index_selected.connect(self.load_by_index)
+
+        self._subsets.inspect_button_clicked.connect(self._inspect_subset_action)
+        self._subsets.pause_inspecting_button_clicked.connect(self._pause_inspecting_subset_action)
+        self._subsets.stop_inspecting_button_clicked.connect(self._stop_inspecting_subset_action)
+
+        self._commands_bar.navigation_button_clicked.connect(self.switch_object)
+        self._commands_bar.star_button_clicked.connect(self.update_starred_state)
         self._commands_bar.screenshot_button_clicked.connect(self._screenshot_action)
         self._commands_bar.settings_button_clicked.connect(self._settings_action)
 
-        self._data_viewer.data_collected.connect(self._save_viewer_data)
-        self._object_info.data_collected.connect(self._save_obj_info_data)
-        self._review_form.data_collected.connect(self._save_review_data)
+        self._inspection_res.edit_button_clicked.connect(self._edit_inspection_file_action)
+
+        self._data_viewer.data_collected.connect(self.save_viewer_data)
+        self._object_info.data_collected.connect(self.save_obj_info_data)
+        self._inspection_res.data_collected.connect(self.save_review_data)
 
         # connect the child widgets between each other
+        self._data_viewer.redshift_obtained.connect(self._inspection_res.set_redshift_value)
         self._commands_bar.reset_view_button_clicked.connect(self._data_viewer.view_reset.emit)
         self._commands_bar.reset_layout_button_clicked.connect(self._data_viewer.init_docks)
 
     def populate(self):
         self.setCentralWidget(self._data_viewer)
 
         self.addToolBar(QtCore.Qt.TopToolBarArea, self._commands_bar)
         self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._quick_search_dock)
         self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._object_info_dock)
-        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._review_form_dock)
+        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._inspection_res_dock)
+        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._subsets_dock)
 
     def load_catalogue(self):
-        cat = read_cat(self._config.catalogue.filename, translate=self._config.catalogue.translate)
+        cat = Catalog.read(self._config.catalogue.filename, translate=self._config.catalogue.translate)
         if cat is None:
             self._config.catalogue.filename = None
             self._config.save()
 
         self.update_catalogue(cat)
 
     def restore_window_state(self):
@@ -288,16 +350,20 @@
     def _new_file_action(self):
         """ Create a new inspection file via the NewFile dialog.
         """
         dialog = NewFile(cfg=self._config, parent=self)
         dialog.catalogue_changed.connect(self.update_catalogue)
         dialog.output_path_selected.connect(self.update_output_path)
         if dialog.exec():
-            self.rd.create(flags=self._config.review_form.default_flags)
-            self.load_project()
+            self.rd.create(flags=self._config.inspection_results.default_flags)
+            if self.rd.review is not None:
+                self.load_project()
+            else:
+                self.update_catalogue(None)
+                self.update_output_path(None)
 
     def _open_file_action(self):
         """ Open an existing inspection file via QFileDialog.
         """
         path = qtpy.compat.getopenfilename(self, caption='Open Inspection File', filters='CSV Files (*.csv)')[0]
         if path:
             self.open_file(path)
@@ -307,23 +373,24 @@
         @param path: path to the inspection file
         @param cached_index:
         """
         path = pathlib.Path(path)
         if path.exists():
             self.update_output_path(path)
             self.rd.read()
-            self.update_catalogue(self.rd.cat)  # in case the catalogue hasn't been initialized before
+            if self.rd.cat is None:
+                self.update_catalogue(None)  # in case the catalogue hasn't been initialized before
             self.load_project(cached_index)
         else:
             logger.warning('Inspection file not found (path: {})'.format(path))
 
     def load_project(self, j: int | None = None):
         """ Update the state of the main window and activate the central widget after loading inspection data.
         """
-        for w in (self._save, self._save_as, self._export, self._reset_view, self._reset_dock_layout):
+        for w in (self._export, self._reset_view, self._reset_dock_layout):
             w.setEnabled(True)
 
         self.project_loaded.emit(self.rd.review)
 
         if j is None or (j < 0 or j >= self.rd.review.n_objects):
             j = 0
 
@@ -340,66 +407,95 @@
 
         self.rd.j = j
 
         # cache the index of the object
         self._cache.last_object_index = j
         self._cache.save()
 
-        self.object_selected.emit(self.rd.j, self.rd.review, self.rd.cat, self._config.data)
+        # get object data from the catalogue
+        obj_id = self.rd.review.get_id(j, full=True)
+        cat_entry = self.rd.cat.get_cat_entry(obj_id)
+
+        self.object_selected.emit(self.rd.j, self.rd.review, cat_entry)
 
         self._update_window_title()
 
-    def reload(self):
-        if self.rd.j is not None:
-            self.load_object(self.rd.j)
+    @QtCore.Slot(str, bool)
+    def switch_object(self, command: str, switch_to_starred: bool):
+        if command not in ('next', 'previous'):
+            logger.error(f'Unknown command: {command}')
+            return
+
+        if switch_to_starred and not self.rd.review.has_data('starred'):
+            logger.error('No starred objects found')
+            return
+
+        j_upd = self._update_index(self.rd.j, command)
+        if self._subset_cat and not self._subset_inspection_paused:
+            while True:
+                subset_entry = self._subset_cat.get_cat_entry(self.rd.review.get_id(j_upd, full=True),
+                                                              ignore_missing=True)
+                if subset_entry is not None:
+                    break
+
+                j_upd = self._update_index(j_upd, command)
+                if j_upd == self.rd.j:  # in case no other ID from the subset is found
+                    logger.warning('No other IDs found in the subset')
+                    break
+
+        elif switch_to_starred:
+            while not self.rd.review.get_value(j_upd, 'starred'):
+                j_upd = self._update_index(j_upd, command)
+
+        self.load_object(j_upd)
+
+    def _update_index(self, obj_index: int, command: str) -> int:
+        j_upd = obj_index
+
+        if command == 'next':
+            j_upd += 1
+        elif command == 'previous':
+            j_upd -= 1
 
-    def _update_window_title(self):
-        title = ''
-        if self.rd.output_path is not None:
-            title += f'{self.rd.output_path.name} – '
-        if self.rd.j is not None:
-            title += f'ID {self.rd.review.get_id(self.rd.j)} [#{self.rd.j + 1}/{self.rd.review.n_objects}] – '
-        title += 'Specvizitor'
-        self.setWindowTitle(title)
+        j_upd = j_upd % self.rd.review.n_objects
+        return j_upd
 
     @QtCore.Slot(str)
-    def _select_by_id(self, obj_id: str):
+    def load_by_id(self, obj_id: str):
         if self.rd.review.validate_id(obj_id):
             self.setFocus()
             self.load_object(self.rd.review.get_id_loc(obj_id))
 
     @QtCore.Slot(int)
-    def _select_by_index(self, index: int):
+    def load_by_index(self, index: int):
         if self.rd.review.validate_index(index):
             self.setFocus()
             self.load_object(index - 1)
 
-    def _save_action(self):
-        """ Instead of saving inspection results, display a message saying that the auto-save mode is enabled.
-        """
-        msg = 'The project data is saved automatically'
-        if self.rd.output_path is not None:
-            msg += ' to {}'.format(self.rd.output_path)
-        LogMessageBox(logging.INFO, msg, parent=self)
+    def _reload(self):
+        if self.rd.j is not None:
+            self.load_object(self.rd.j)
 
-    def _save_as_action(self):
-        path = qtpy.compat.getsavefilename(self, caption='Save/Save As',
-                                           basedir=str(self.rd.output_path),
-                                           filters='CSV Files (*.csv)')[0]
-        if path:
-            self.update_output_path(pathlib.Path(path).resolve())
-            self.rd.save()
+    def _update_window_title(self):
+        title = ''
+        if self.rd.output_path is not None:
+            title += f'{self.rd.output_path.name} – '
+        if self.rd.j is not None:
+            title += (f'ID {self.rd.review.get_id(self.rd.j, full=True)}'
+                      f' [#{self.rd.j + 1}/{self.rd.review.n_objects}] – ')
+        title += 'Specvizitor'
+        self.setWindowTitle(title)
 
     def _export_action(self):
         path = qtpy.compat.getsavefilename(self, caption='Export To FITS',
                                            basedir=str(self.rd.output_path.with_suffix('.fits')),
                                            filters='FITS Files (*.fits)')[0]
 
         if path:
-            self.rd.review.write(self.rd.output_path.with_suffix('.fits'), 'fits')
+            self.rd.review.write(path, 'fits')
 
     def _exit_action(self):
         if self.rd.j is not None:
             self.data_requested.emit()
 
         # save the state and geometry of the main window
         settings = QtCore.QSettings()
@@ -409,96 +505,188 @@
         self.close()
         logger.info("Application closed")
 
     def _restore_viewer_config_action(self):
         path = qtpy.compat.getopenfilename(self, caption='Open Viewer Configuration',
                                            filters='YAML Files (*.yml)')[0]
         if path:
-            new_viewer_cfg = self._viewer_cfg.replace_params(pathlib.Path(path))
+            new_viewer_cfg = self._widget_cfg.replace_params(pathlib.Path(path))
             if new_viewer_cfg is None:
                 logger.error('Failed to restore the viewer configuration')
             else:
-                self._viewer_cfg = new_viewer_cfg
-                self._viewer_cfg.save()
+                self._widget_cfg = new_viewer_cfg
+                self._widget_cfg.save()
 
-                self.viewer_configuration_updated.emit(self._viewer_cfg)
+                self.viewer_configuration_updated.emit(self._widget_cfg)
 
-                self.reload()
+                self._reload()
 
                 logger.info('Viewer configuration restored')
 
     def _backup_viewer_config_action(self):
         path = qtpy.compat.getsavefilename(self, caption='Save Viewer Configuration',
                                            basedir=str(pathlib.Path() / 'data_widgets.yml'),
                                            filters='YAML Files (*.yml)')[0]
 
         if path:
-            save_yaml(path, asdict(self._viewer_cfg))
+            save_yaml(path, asdict(self._widget_cfg))
             logger.info('Viewer configuration saved')
 
+    def _hide_interface(self):
+        self.interface_hidden = True
+        self._zen.setText('Show Interface')
+        self.zen_mode_activated.emit()
+
+    def _show_interface(self):
+        self.interface_hidden = False
+        self._zen.setText('Hide Interface')
+        self.zen_mode_deactivated.emit()
+
     def _enter_fullscreen(self):
         self.was_maximized = True if self.isMaximized() else False
         self.showFullScreen()
 
     def _exit_fullscreen(self):
         self.showNormal()
         if self.was_maximized:
             self.showMaximized()
 
+    def _edit_inspection_file_action(self):
+        dialog = InspectionEditor(review=self.rd.review, parent=self)
+        dialog.inspection_fields_updated.connect(self.update_inspection_fields)
+        if dialog.exec():
+            self.project_loaded.emit(self.rd.review)
+
+    def _inspect_subset_action(self):
+        path = qtpy.compat.getopenfilename(self, caption='Open Subset')[0]
+        if path:
+            self._cache.last_subset_file = path
+            self._cache.save()
+            self.load_subset()
+
+    def load_subset(self, reset_index=True):
+        subset_path = self._cache.last_subset_file
+        subset = Catalog.read(subset_path, translate=self._config.catalogue.translate)
+        if subset:
+            subset.add_column(np.arange(len(subset)), name='__index__', index=0)
+
+            self._subset_cat = subset
+            self.subset_loaded.emit(subset_path, subset)
+
+            if reset_index:
+                self.load_by_id(self._subset_cat.get_col('id')[0])
+        else:
+            self._cache.last_subset_file = None
+            self._cache.save()
+
+    def _pause_inspecting_subset_action(self):
+        self._subset_inspection_paused = not self._subset_inspection_paused
+        self.subset_inspection_paused.emit(self._subset_inspection_paused)
+
+    def _stop_inspecting_subset_action(self):
+        self._subset_cat = None
+        self._subset_inspection_paused = False
+
+        self._cache.last_subset_file = None
+        self._cache.save()
+
+        self.subset_inspection_stopped.emit()
+
     def _screenshot_action(self):
         default_filename = f'{self.rd.output_path.stem.replace(" ", "_")}_ID{self.rd.review.get_id(self.rd.j)}.png'
         path, extension = qtpy.compat.getsavefilename(self, caption='Save/Save As',
                                                       basedir=str(pathlib.Path().resolve() / default_filename),
                                                       filters='Images (*.png)')
         if path:
             self.screenshot_path_selected.emit(path)
 
     def _settings_action(self):
-        dialog = Settings(self._config, parent=self)
+        self._restart_requested = False
+
+        dialog = Settings(self.rd.cat, self._config, self._spectral_lines, parent=self)
+
         dialog.appearance_changed.connect(self.update_appearance)
         dialog.catalogue_changed.connect(self.update_catalogue)
+        dialog.spectral_lines_changed.connect(self.spectral_lines_changed.emit)
+        dialog.data_source_changed.connect(self.data_source_changed.emit)
+
+        dialog.restart_requested.connect(self.restart)
+
         if dialog.exec():
-            self.reload()
+            if not self._restart_requested:
+                self._reload()
 
-    @QtCore.Slot(bool)
-    def update_appearance(self, theme_changed: bool = False):
-        set_up_appearance(self._config.appearance)
-        if theme_changed:
-            self.theme_changed.emit()
+    @QtCore.Slot()
+    def update_appearance(self):
+        setup_appearance(self._config.appearance, update_theme=False)
 
     @QtCore.Slot(object)
-    def update_catalogue(self, cat: Table | None):
+    def update_catalogue(self, cat: Catalog | None):
         if cat is None and self.rd.review is not None:
-            self.rd.cat = create_cat(self.rd.review.ids)
+            self.rd.cat = Catalog.create(self.rd.review.ids_full)
         else:
             self.rd.cat = cat
         self.catalogue_changed.emit(self.rd.cat)
 
     @QtCore.Slot(pathlib.Path)
-    def update_output_path(self, path: pathlib.Path):
+    def update_output_path(self, path: pathlib.Path | None):
         self.rd.output_path = path
-        self._cache.last_inspection_file = str(path)
+        self._cache.last_inspection_file = None if path is None else str(path)
         self._cache.save()
         self._update_window_title()
 
+    @QtCore.Slot(list, list, bool)
+    def update_inspection_fields(self, fields: list[tuple[str, str]], is_deleted: list[bool], set_as_default: bool):
+        old_columns = self.rd.review.user_defined_columns
+        for i, old_name in enumerate(old_columns):
+            new_name = fields[i][0]
+            if is_deleted[i]:
+                self.rd.review.delete_column(column_name=old_name)
+            elif old_name != new_name:
+                self.rd.review.rename_column(old_name=old_name, new_name=new_name)
+
+        for field in fields[len(old_columns):]:
+            new_name, new_type = field[0], field[1]
+            if new_type == 'boolean':
+                self.rd.review.add_flag_column(column_name=new_name)
+
+        if set_as_default:
+            default_flags = self.rd.review.flag_columns
+            self._config.inspection_results.default_flags = default_flags
+            self._config.save()
+
     def _about_action(self):
         QtWidgets.QMessageBox.about(self, "About Specvizitor", "Specvizitor v{}".format(version('specvizitor')))
 
     def closeEvent(self, _):
         self._exit_action()
 
+    @QtCore.Slot()
+    def update_starred_state(self):
+        starred = not self.rd.review.get_value(self.rd.j, 'starred')
+        self.rd.review.update_value(self.rd.j, 'starred', starred)
+
+        self.starred_state_updated.emit(starred, self.rd.review.has_data('starred'))
+
     @QtCore.Slot(dict)
-    def _save_viewer_data(self, layout: dict):
+    def save_viewer_data(self, layout: dict):
         self._cache.dock_layout = layout
         self._cache.save()
 
     @QtCore.Slot(list)
-    def _save_obj_info_data(self, visible_columns: list[str]):
+    def save_obj_info_data(self, visible_columns: list[str]):
         self._cache.visible_columns = visible_columns
         self._cache.save()
 
-    @QtCore.Slot(str, dict)
-    def _save_review_data(self, comments: str, checkboxes: dict[str, bool]):
+    @QtCore.Slot(float, str, dict)
+    def save_review_data(self, redshift: float, comments: str, checkboxes: dict[str, bool]):
+        self.rd.review.update_value(self.rd.j, 'z_sviz', redshift)
         self.rd.review.update_value(self.rd.j, 'comment', comments)
         for cname, is_checked in checkboxes.items():
             self.rd.review.update_value(self.rd.j, cname, is_checked)
         self.rd.save()
+
+    @QtCore.Slot()
+    def restart(self):
+        self._restart_requested = True
+        self._exit_action()
+        QtWidgets.QApplication.exit(MainWindow.EXIT_CODE_REBOOT)
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/NewFile.py` & `specvizitor-0.4.0/specvizitor/widgets/NewFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from qtpy import QtWidgets, QtCore
 
 import logging
 import pathlib
 
 from ..config import config
-from ..io.catalogue import read_cat, create_cat, cat_browser
+from ..io.catalog import Catalog, cat_browser
 from ..io.viewer_data import get_ids_from_dir, data_browser
 from ..utils.logs import qlog
-
-from .FileBrowser import FileBrowser
+from ..utils.widgets import FileBrowser
 
 logger = logging.getLogger(__name__)
 
 
 class NewFile(QtWidgets.QDialog):
     output_path_selected = QtCore.Signal(pathlib.Path)
     catalogue_changed = QtCore.Signal(object)
@@ -135,21 +134,21 @@
     @qlog
     def get_catalogue(self):
         # create a new catalogue if necessary
         if self._browsers['cat'].isHidden():
             ids = get_ids_from_dir(self._browsers['data'].path, self._id_pattern.text())
             if ids is None:
                 return
-            return create_cat(ids)
+            return Catalog.create(ids)
 
         # otherwise, load an existing catalogue
         data_dir = self._browsers['data'].path if self._filter_check_box.isChecked() else None
 
-        return read_cat(self._browsers['cat'].path, translate=self.cfg.catalogue.translate, data_dir=data_dir,
-                        id_pattern=self.cfg.data.id_pattern)
+        return Catalog.read(self._browsers['cat'].path, translate=self.cfg.catalogue.translate, data_dir=data_dir,
+                            id_pattern=self.cfg.data.id_pattern)
 
     def accept(self):
         if not self.validate():
             return
 
         cat = self.get_catalogue()
         if cat is None:
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/ObjectInfo.py` & `specvizitor-0.4.0/specvizitor/widgets/ObjectInfo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,101 @@
-from astropy.coordinates import SkyCoord
-from astropy.table import Table
 from qtpy import QtWidgets, QtCore
 
 import logging
 
+from ..io.catalog import Catalog
 from ..io.inspection_data import InspectionData
-from ..utils.table_tools import column_not_found_message
+from ..utils.widgets import AbstractWidget
 
-from .AbstractWidget import AbstractWidget
 from .TableColumns import TableColumns
 
-
 logger = logging.getLogger(__name__)
 
 
 class ObjectInfo(AbstractWidget):
     data_collected = QtCore.Signal(list)
 
     def __init__(self, parent=None):
-        self.all_columns: list[str] | None = None
+        self.all_columns: dict[str, str] | None = None
         self.visible_columns: list[str] | None = None
 
         self._table: QtWidgets.QTableWidget | None = None
-        self._table_items: list[tuple[QtWidgets.QTableWidgetItem, QtWidgets.QTableWidgetItem]] | None = None
+        self._table_items: dict[str, list[tuple[QtWidgets.QTableWidgetItem, QtWidgets.QTableWidgetItem]]] | None = None
 
         self._search_label: QtWidgets.QLabel | None = None
         self._search_lineedit: QtWidgets.QLineEdit | None = None
         self._display_options: QtWidgets.QPushButton | None = None
 
         super().__init__(parent=parent)
         self.setEnabled(False)
         self.setSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
 
-    def create_table_items(self):
+    def _create_table_items(self):
         if self.all_columns is None:
-            self._table_items = []
+            self._table_items = {}
             return
 
-        table_items = []
-        for cname in self.all_columns:
-            cname_item = QtWidgets.QTableWidgetItem(cname)
+        table_items = {}
+        for cname, cname_annotated in self.all_columns.items():
+            cname_item = QtWidgets.QTableWidgetItem(cname_annotated)
             value_item = QtWidgets.QTableWidgetItem('')
 
-            table_items.append((cname_item, value_item))
+            table_items[cname] = cname_item, value_item
 
         self._table_items = table_items
 
-    def set_table_items(self):
+    def _set_table_items(self):
         self._table.setRowCount(len(self._table_items))
-        for i, row in enumerate(self._table_items):
+        for i, row in enumerate(self._table_items.values()):
             self._table.setItem(i, 0, row[0])
             self._table.setItem(i, 1, row[1])
 
     @QtCore.Slot(object)
-    def update_table_items(self, cat: Table | None):
-        self.all_columns = cat.colnames if cat is not None else None
-        self.create_table_items()
-        self.set_table_items()
+    def update_table_items(self, cat: Catalog | None):
+        self.all_columns = cat.annotated_colnames if cat is not None else None
 
-        self.update_visible_columns(self.all_columns)
+        self._create_table_items()
+        self._set_table_items()
+        if self.all_columns:
+            self.update_visible_columns(list(self.all_columns.keys()))
 
     @QtCore.Slot()
     def update_view(self):
-        for i, row in enumerate(self._table_items):
-            cname = row[0].text()
+        for i, cname in enumerate(self._table_items.keys()):
             if cname in self.visible_columns and self._search_lineedit.text() in cname:
                 self._table.showRow(i)
             else:
                 self._table.hideRow(i)
 
     @QtCore.Slot(list)
     def update_visible_columns(self, visible_columns: list[str] | None):
         self.visible_columns = visible_columns
         self.update_view()
 
     def init_ui(self):
         self._table = QtWidgets.QTableWidget(self)
         self._table.setColumnCount(2)
         self._table.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self._table.horizontalHeader().hide()
+        # self._table.horizontalHeader().hide()
         self._table.horizontalHeader().setStretchLastSection(True)
-        self._table.horizontalHeader().setSectionResizeMode(0, QtWidgets.QHeaderView.ResizeToContents)
-        # self._table.setHorizontalHeaderLabels(('key', 'value'))
+        # self._table.horizontalHeader().setSectionResizeMode(0, QtWidgets.QHeaderView.ResizeToContents)
+        self._table.setHorizontalHeaderLabels(('Key', 'Value'))
+        self._table.verticalHeader().hide()
         self._table.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
 
         self._search_label = QtWidgets.QLabel("Search:", self)
         self._search_label.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum)
         self._search_lineedit = QtWidgets.QLineEdit(self)
         self._search_lineedit.setSizePolicy(QtWidgets.QSizePolicy.Ignored, QtWidgets.QSizePolicy.Maximum)
         self._search_lineedit.setMinimumWidth(50)
         self._display_options = QtWidgets.QPushButton("Columns...", self)
         self._display_options.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum)
 
         self._search_lineedit.textChanged[str].connect(self.update_view)
-        self._display_options.pressed.connect(self._display_options_action)
+        self._display_options.clicked.connect(self._display_options_action)
 
     def set_layout(self):
         self.setLayout(QtWidgets.QVBoxLayout())
 
     def populate(self):
         self.layout().addWidget(self._table)
 
@@ -108,38 +106,33 @@
 
         self.layout().addLayout(sub_layout)
 
     @QtCore.Slot()
     def load_project(self):
         self.setEnabled(True)
 
-    @QtCore.Slot(int, InspectionData, Table)
-    def load_object(self, j: int, review: InspectionData, cat: Table):
-        try:
-            cat.loc[review.get_id(j)]
-        except KeyError:
-            logger.warning('Object not found in the catalogue (ID: {})'.format(review.get_id(j)))
+    @QtCore.Slot(int, InspectionData, object)
+    def load_object(self, _, __, cat_entry: Catalog | None):
+
+        if cat_entry is None:
+            for row in self._table_items.values():
+                row[1].setText('')
             return
 
-        for row in self._table_items:
-            cname = row[0].text()
+        for cname, row in self._table_items.items():
             try:
-                row[1].setText(str(cat.loc[review.get_id(j)][cname]))
-            except KeyError:
-                logger.warning(column_not_found_message(cname, cat.meta.get('aliases')))
+                value = cat_entry.get_col(cname)
+                value = f'{value:.8f}' if isinstance(value, float) else str(value)
+                row[1].setText(value)
+            except KeyError as e:
+                logger.warning(e)
                 row[1].setText('')
 
-        # if 'ra' in self._cat.colnames and 'dec' in self._cat.colnames:
-        #     c = SkyCoord(ra=self._cat['ra'][self._j], dec=self._cat['dec'][self._j], frame='icrs', unit='deg')
-        #     ra, dec = c.to_string('hmsdms').split(' ')
-        #     self.ra_label.setText("RA: {}".format(ra))
-        #     self.dec_label.setText("Dec: {}".format(dec))
-
     @QtCore.Slot()
     def collect(self):
         self.data_collected.emit(self.visible_columns)
 
     def _display_options_action(self):
-        dialog = TableColumns(self.all_columns, self.visible_columns, parent=self)
+        dialog = TableColumns(list(self.all_columns.keys()), self.visible_columns, parent=self)
         dialog.visible_columns_updated.connect(self.update_visible_columns)
         if dialog.exec():
             pass
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/QuickSearch.py` & `specvizitor-0.4.0/specvizitor/widgets/QuickSearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from qtpy import QtWidgets, QtCore
 
 import logging
 
-from .AbstractWidget import AbstractWidget
+from ..utils.widgets import AbstractWidget
+
 
 logger = logging.getLogger(__name__)
 
 
 class QuickSearch(AbstractWidget):
     id_selected = QtCore.Signal(str)
     index_selected = QtCore.Signal(int)
@@ -21,24 +22,26 @@
         self.setEnabled(False)
         self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum)
 
     def init_ui(self):
         # create a `Go to ID` button
         self._go_to_id_button = QtWidgets.QPushButton(self)
         self._go_to_id_button.setText('Go to ID')
-        self._go_to_id_button.setFixedWidth(110)
+        self._go_to_id_button.setFixedWidth(90)
 
         self._id_field = QtWidgets.QLineEdit(self)
+        self._id_field.setMinimumWidth(60)
 
         # create a `Go to index` button
         self._go_to_index_button = QtWidgets.QPushButton(self)
         self._go_to_index_button.setText('Go to #')
-        self._go_to_index_button.setFixedWidth(110)
+        self._go_to_index_button.setFixedWidth(90)
 
         self._index_field = QtWidgets.QLineEdit(self)
+        self._index_field.setMinimumWidth(60)
 
         self._go_to_id_button.clicked.connect(self.go_to_id)
         self._id_field.returnPressed.connect(self.go_to_id)
         self._go_to_index_button.clicked.connect(self.go_to_index)
         self._index_field.returnPressed.connect(self.go_to_index)
 
     def set_layout(self):
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/Section.py` & `specvizitor-0.4.0/specvizitor/utils/widgets/Section.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.1/specvizitor/widgets/SmartSlider.py` & `specvizitor-0.4.0/specvizitor/widgets/SmartSlider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from astropy.table import Table
 import numpy as np
 from qtpy import QtWidgets, QtCore
 
 import logging
 
-from ..utils.table_tools import column_not_found_message
-from .AbstractWidget import AbstractWidget
-
+from ..io.catalog import Catalog
+from ..utils.widgets import AbstractWidget
 
 logger = logging.getLogger(__name__)
 
 
-class SmartSlider(QtWidgets.QSlider):
+class SmartSliderBase(QtWidgets.QSlider):
     value_changed = QtCore.Signal()
 
     def __init__(self, min_value=0, max_value=100, step=1, default_value=0,
                  orientation=QtCore.Qt.Orientation.Vertical, parent=None):
 
         super().__init__(orientation, parent)
 
@@ -41,96 +39,110 @@
             return 1
 
     @property
     def index(self):
         return self._index
 
     @index.setter
-    def index(self, i):
+    def index(self, i: int):
         self._index = i
         self.setValue(i)
 
     @property
     def value(self):
         return self._arr[self.index - 1]
 
-    def index_from_value(self, value):
+    def index_from_value(self, value: float):
         i = self._arr.searchsorted(value, side='right')
         return i if i > 0 else 1
 
     def reset(self):
         self.index = self.default_index
 
     def value_changed_action(self, index: int):
         self.index = index
         self.value_changed.emit()
 
 
-class SmartSliderWithEditor(AbstractWidget):
+class SmartSlider(AbstractWidget):
     value_changed = QtCore.Signal(float)
+    save_button_clicked = QtCore.Signal(float)
+
+    def __init__(self, short_name: str = 'x', full_name: str | None = None, action: str | None = None,
+                 visible: bool = True, catalog_name: str | None = None, link_to: str | None = None,
+                 show_text_editor: bool = False, n_decimal_places: int = 6, show_save_button: bool = False,
+                 parent=None, **kwargs):
 
-    def __init__(self, parameter: str = 'x', full_name: str | None = None, action: str | None = None,
-                 visible: bool = True, name_in_catalogue: str | None = None, show_text_editor: bool = False,
-                 n_decimal_places: int = 6, parent=None, **kwargs):
+        if catalog_name is not None:
+            self.short_name = catalog_name
+        else:
+            self.short_name = short_name
 
-        self.parameter = parameter if name_in_catalogue is None else name_in_catalogue
-        self.full_name = parameter if full_name is None else full_name
+        self.full_name = short_name if full_name is None else full_name
         self.action = f"change {self.full_name}" if action is None else action
 
-        self.name_in_catalogue = name_in_catalogue
+        self.catalog_name = catalog_name
+        self.link_to = link_to
         self.show_text_editor = show_text_editor
         self.n_decimal_places = n_decimal_places
+        self.show_save_button = show_save_button
 
         self._slider_kwargs = kwargs
 
-        self._slider: SmartSlider | None = None
+        self._slider: SmartSliderBase | None = None
         self._label: QtWidgets.QLabel | None = None
         self._editor: QtWidgets.QLineEdit | None = None
+        self._save_button: QtWidgets.QPushButton | None = None
 
         super().__init__(parent=parent)
         self.setHidden(not visible)
 
-        self._default_value_backup = self._slider.default_value
+        self._default_value_fallback = self._slider.default_value
 
     def init_ui(self):
         # create a slider
-        if self.show_text_editor:
-            orientation = QtCore.Qt.Orientation.Horizontal
-        else:
-            orientation = QtCore.Qt.Orientation.Vertical
-
-        self._slider = SmartSlider(orientation=orientation, parent=self, **self._slider_kwargs)
+        orientation = QtCore.Qt.Orientation.Horizontal if self.show_text_editor else QtCore.Qt.Orientation.Vertical
+        self._slider = SmartSliderBase(orientation=orientation, parent=self, **self._slider_kwargs)
         self._slider.setToolTip(f'Slide to {self.action}')
 
         # create a label
-        self._label = QtWidgets.QLabel(f'{self.parameter} =', self)
+        self._label = QtWidgets.QLabel(f'{self.short_name} =', self)
 
         # create a text editor
         self._editor = QtWidgets.QLineEdit(self)
         self._editor.setMaximumWidth(120)
 
-        self._label.setHidden(not self.show_text_editor)
-        self._editor.setHidden(not self.show_text_editor)
+        # create a save button
+        self._save_button = QtWidgets.QPushButton('Save!', self)
+
+        self._label.setVisible(self.show_text_editor)
+        self._editor.setVisible(self.show_text_editor)
+        self._save_button.setVisible(self.show_save_button)
 
         self._slider.value_changed.connect(self.update_from_slider)
         self._editor.returnPressed.connect(self._update_from_editor)
+        self._save_button.clicked.connect(self.save_redshift)
 
     def set_layout(self):
         self.setLayout(QtWidgets.QGridLayout())
         self.set_geometry(spacing=5, margins=0)
 
     def populate(self):
         self.layout().addWidget(self._slider, 1, 1, 1, 1)
         self.layout().addWidget(self._label, 1, 2, 1, 1)
         self.layout().addWidget(self._editor, 1, 3, 1, 1)
+        self.layout().addWidget(self._save_button, 1, 4, 1, 1)
 
     @property
     def value(self):
         return self._slider.value
 
+    def set_value(self, value):
+        self._slider.index = self._slider.index_from_value(value)
+
     def _update_editor_text(self):
         self._editor.setText('{value:.{num_decimal_places}f}'.format(value=self.value,
                                                                      num_decimal_places=self.n_decimal_places))
 
     def update_from_slider(self):
         self._update_editor_text()
         self.value_changed.emit(self.value)
@@ -142,22 +154,40 @@
             # the true slider value might stay the same, which would require a manual update of the text editor
             self._update_editor_text()
 
         except ValueError:
             logger.error(f'Invalid {self.full_name} value: {self._editor.text()}')
             self.reset()
 
-    def update_default_value(self, cat: Table, object_id):
+    @QtCore.Slot()
+    def save_redshift(self):
+        self.save_button_clicked.emit(self.value)
+
+    @QtCore.Slot(float)
+    def change_redshift(self, delta_z: float):
+        self._slider.index = self._slider.index_from_value(self._slider.value + delta_z)
+
+    def update_default_value(self, default_value: float):
+        self._slider.default_value = default_value
+
+    def update_default_value_from_catalog(self, cat_entry: Catalog | None):
+        if cat_entry is None or self.catalog_name is None:
+            self._slider.default_value = self._default_value_fallback
+            return
+
         try:
-            self._slider.default_value = cat.loc[object_id][self.name_in_catalogue]
-        except KeyError:
-            logger.warning(column_not_found_message(self.name_in_catalogue, cat.meta.get('aliases')))
-            self._slider.default_value = self._default_value_backup
+            self._slider.default_value = cat_entry.get_col(self.catalog_name)
+        except KeyError as e:
+            logger.warning(e)
+            self._slider.default_value = self._default_value_fallback
 
     def reset(self):
+        if self.link_to is not None:
+            return
+
         self._slider.reset()
 
         # see a comment in _update_from_editor
         self._update_editor_text()
 
     def clear(self):
         self._editor.setText("")
```

### Comparing `specvizitor-0.3.1/specvizitor/widgets/TableColumns.py` & `specvizitor-0.4.0/specvizitor/widgets/TableColumns.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         self._create_checkboxes()
         self._add_table_items()
 
         # add OK/Cancel buttons
         self._button_box = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel, self)
 
-        self._check_all.pressed.connect(partial(self._all_action, True))
-        self._uncheck_all.pressed.connect(partial(self._all_action, False))
+        self._check_all.clicked.connect(partial(self._all_action, True))
+        self._uncheck_all.clicked.connect(partial(self._all_action, False))
 
         self._button_box.accepted.connect(self.accept)
         self._button_box.rejected.connect(self.reject)
 
     def set_layout(self):
         self.setLayout(QtWidgets.QVBoxLayout())
```

