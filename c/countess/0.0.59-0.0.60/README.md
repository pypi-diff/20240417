# Comparing `tmp/countess-0.0.59.tar.gz` & `tmp/countess-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.59.tar", last modified: Tue Apr 16 05:18:19 2024, max compression
+gzip compressed data, was "countess-0.0.60.tar", last modified: Wed Apr 17 01:52:58 2024, max compression
```

## Comparing `countess-0.0.59.tar` & `countess-0.0.60.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.59/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.59/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-16 05:18:19.841561 countess-0.0.59/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-16 05:16:27.000000 countess-0.0.59/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.833561 countess-0.0.59/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-16 05:16:27.000000 countess-0.0.59/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.59/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.59/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-05 06:49:16.000000 countess-0.0.59/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.59/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19404 2024-04-12 03:37:47.000000 countess-0.0.59/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-16 04:58:09.000000 countess-0.0.59/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-16 04:58:09.000000 countess-0.0.59/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.59/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18396 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)    20442 2024-04-12 03:37:47.000000 countess-0.0.59/countess/gui/icons/countess.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5104 2024-04-15 03:16:30.000000 countess-0.0.59/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20505 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14479 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-05 06:49:16.000000 countess-0.0.59/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     9359 2024-04-15 09:54:50.000000 countess-0.0.59/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.59/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-05 05:13:40.000000 countess-0.0.59/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.59/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3854 2024-04-08 01:06:06.000000 countess-0.0.59/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.59/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3524 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.59/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.59/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.59/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.59/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18172 2024-04-12 03:37:47.000000 countess-0.0.59/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1651 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-05 06:49:16.000000 countess-0.0.59/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-16 05:18:19.841561 countess-0.0.59/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.59/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-05 05:13:41.000000 countess-0.0.59/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-05 05:13:41.000000 countess-0.0.59/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.59/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.424577 countess-0.0.60/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.60/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.60/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-17 01:52:58.424577 countess-0.0.60/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-17 01:52:44.000000 countess-0.0.60/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.416577 countess-0.0.60/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-17 01:52:44.000000 countess-0.0.60/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.416577 countess-0.0.60/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.60/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.60/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-05 06:49:16.000000 countess-0.0.60/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.60/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19404 2024-04-12 03:37:47.000000 countess-0.0.60/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-16 04:58:09.000000 countess-0.0.60/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-16 04:58:09.000000 countess-0.0.60/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.416577 countess-0.0.60/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.60/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18396 2024-04-16 04:58:09.000000 countess-0.0.60/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.420577 countess-0.0.60/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.60/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.60/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20442 2024-04-12 03:37:47.000000 countess-0.0.60/countess/gui/icons/countess.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.60/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.60/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.60/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5104 2024-04-15 03:16:30.000000 countess-0.0.60/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20505 2024-04-16 04:58:09.000000 countess-0.0.60/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-05 05:13:40.000000 countess-0.0.60/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14475 2024-04-17 01:52:24.000000 countess-0.0.60/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-05 06:49:16.000000 countess-0.0.60/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9359 2024-04-15 09:54:50.000000 countess-0.0.60/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.420577 countess-0.0.60/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.60/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-05 05:13:40.000000 countess-0.0.60/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.60/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3854 2024-04-17 01:44:42.000000 countess-0.0.60/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.60/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3524 2024-04-16 04:58:09.000000 countess-0.0.60/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.60/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.420577 countess-0.0.60/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.60/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.60/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.60/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18172 2024-04-12 03:37:47.000000 countess-0.0.60/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.420577 countess-0.0.60/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1651 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-17 01:52:58.000000 countess-0.0.60/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-05 06:49:16.000000 countess-0.0.60/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-17 01:52:58.424577 countess-0.0.60/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.60/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-17 01:52:58.420577 countess-0.0.60/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-05 05:13:41.000000 countess-0.0.60/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-05 05:13:41.000000 countess-0.0.60/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.60/tests/test_plugins.py
```

### Comparing `countess-0.0.59/LICENSE.txt` & `countess-0.0.60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/PKG-INFO` & `countess-0.0.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.59
+Version: 0.0.60
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.59
+# CountESS 0.0.60
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.59/README.md` & `countess-0.0.60/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.59
+# CountESS 0.0.60
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.59/countess/core/config.py` & `countess-0.0.60/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/core/logger.py` & `countess-0.0.60/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/core/parameters.py` & `countess-0.0.60/countess/core/parameters.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/core/pipeline.py` & `countess-0.0.60/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/core/plugins.py` & `countess-0.0.60/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/config.py` & `countess-0.0.60/countess/gui/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/icons/countess.gif` & `countess-0.0.60/countess/gui/icons/countess.gif`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/logger.py` & `countess-0.0.60/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/main.py` & `countess-0.0.60/countess/gui/main.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/mini_browser.py` & `countess-0.0.60/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/tabular.py` & `countess-0.0.60/countess/gui/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
     # detecting this surely?
 
     def _column_yscrollcommand(self, y1, y2):
         # All this actually does is to detect if there's
         # too many rows for the window, in which case it
         # trims them off.  Once there's the right number
         # of rows, this won't get called any more.
-        span = int((float(y2) - float(y1)) * self.height) + 1
+        span = int((float(y2) - float(y1)) * self.height)
         if span > 0 and span != self.height:
             self.height = span
             self.refresh()
 
     def _configure(self, *_):
         # the delay lets the sub-elements configure
         # themselves before we try to measure them.
```

### Comparing `countess-0.0.59/countess/gui/tree.py` & `countess-0.0.60/countess/gui/tree.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/gui/widgets.py` & `countess-0.0.60/countess/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/collate.py` & `countess-0.0.60/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/column.py` & `countess-0.0.60/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/correlation.py` & `countess-0.0.60/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/csv.py` & `countess-0.0.60/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/data_table.py` & `countess-0.0.60/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/expression.py` & `countess-0.0.60/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/fastq.py` & `countess-0.0.60/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/group_by.py` & `countess-0.0.60/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/hgvs_parser.py` & `countess-0.0.60/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/join.py` & `countess-0.0.60/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/mutagenize.py` & `countess-0.0.60/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/pivot.py` & `countess-0.0.60/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/python.py` & `countess-0.0.60/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/regex.py` & `countess-0.0.60/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/sequence.py` & `countess-0.0.60/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/plugins/variant.py` & `countess-0.0.60/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/utils/pandas.py` & `countess-0.0.60/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/utils/parallel.py` & `countess-0.0.60/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess/utils/variant.py` & `countess-0.0.60/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess.egg-info/PKG-INFO` & `countess-0.0.60/countess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.59
+Version: 0.0.60
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.59
+# CountESS 0.0.60
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.59/countess.egg-info/SOURCES.txt` & `countess-0.0.60/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/countess.egg-info/entry_points.txt` & `countess-0.0.60/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/pyproject.toml` & `countess-0.0.60/pyproject.toml`

 * *Files identical despite different names*

### Comparing `countess-0.0.59/tests/test_plugins.py` & `countess-0.0.60/tests/test_plugins.py`

 * *Files identical despite different names*

