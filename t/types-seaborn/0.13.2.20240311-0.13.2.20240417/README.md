# Comparing `tmp/types-seaborn-0.13.2.20240311.tar.gz` & `tmp/types-seaborn-0.13.2.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-seaborn-0.13.2.20240311.tar", last modified: Mon Mar 11 02:18:09 2024, max compression
+gzip compressed data, was "types-seaborn-0.13.2.20240417.tar", last modified: Wed Apr 17 02:17:28 2024, max compression
```

## Comparing `types-seaborn-0.13.2.20240311.tar` & `types-seaborn-0.13.2.20240417.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.472959 types-seaborn-0.13.2.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-11 02:18:08.000000 types-seaborn-0.13.2.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:18:08.000000 types-seaborn-0.13.2.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.464959 types-seaborn-0.13.2.20240311/seaborn-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-11 02:18:08.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.464959 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/groupby.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/moves.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/plot.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/scales.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/subplots.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_core/typing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/area.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/bar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/dot.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/line.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/counting.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/density.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/order.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/_stats/regression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/algorithms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/axisgrid.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/categorical.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/cm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/seaborn-stubs/colors/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/colors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/colors/crayons.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/colors/xkcd_rgb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/distributions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/seaborn-stubs/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/appdirs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/docscrape.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/husl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/kde.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/external/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/matrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/miscplot.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/objects.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/palettes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/rcmod.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/regression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/relational.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-11 02:14:35.000000 types-seaborn-0.13.2.20240311/seaborn-stubs/widgets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:18:09.472959 types-seaborn-0.13.2.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-11 02:18:08.000000 types-seaborn-0.13.2.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:09.468959 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-11 02:18:09.000000 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-11 02:18:09.000000 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:18:09.000000 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-11 02:18:09.000000 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 02:18:09.000000 types-seaborn-0.13.2.20240311/types_seaborn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.313440 types-seaborn-0.13.2.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-17 02:17:27.000000 types-seaborn-0.13.2.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:27.000000 types-seaborn-0.13.2.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-17 02:17:28.313440 types-seaborn-0.13.2.20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.305440 types-seaborn-0.13.2.20240417/seaborn-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 02:17:27.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.309440 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/groupby.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/moves.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/plot.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/scales.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/subplots.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_core/typing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.309440 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/area.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/dot.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.309440 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/counting.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/density.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/order.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/_stats/regression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/algorithms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/axisgrid.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/categorical.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/cm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.309440 types-seaborn-0.13.2.20240417/seaborn-stubs/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/colors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/colors/crayons.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/colors/xkcd_rgb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/distributions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.309440 types-seaborn-0.13.2.20240417/seaborn-stubs/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/appdirs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/docscrape.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/husl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/kde.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/external/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/matrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/miscplot.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/objects.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/palettes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:27.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/rcmod.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/regression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/relational.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-17 02:16:41.000000 types-seaborn-0.13.2.20240417/seaborn-stubs/widgets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:28.313440 types-seaborn-0.13.2.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-17 02:17:27.000000 types-seaborn-0.13.2.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:28.313440 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-17 02:17:28.000000 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-17 02:17:28.000000 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:28.000000 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 02:17:28.000000 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 02:17:28.000000 types-seaborn-0.13.2.20240417/types_seaborn.egg-info/top_level.txt
```

### Comparing `types-seaborn-0.13.2.20240311/CHANGELOG.md` & `types-seaborn-0.13.2.20240417/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.13.2.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 0.13.2.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 0.13.2.20240310 (2024-03-10)
 
 Bump mypy to 1.9, add to json.encoder, small fixups (#11549)
```

### Comparing `types-seaborn-0.13.2.20240311/PKG-INFO` & `types-seaborn-0.13.2.20240417/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-seaborn
-Version: 0.13.2.20240311
+Version: 0.13.2.20240417
 Summary: Typing stubs for seaborn
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/seaborn.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-seaborn` aims to provide accurate annotations
 for `seaborn==0.13.2`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/seaborn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/data.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/data.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/groupby.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/groupby.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # Signature based on pandas.core.groupby.generic.DataFrameGroupBy.aggregate
     # args and kwargs possible values depend on func which itself can be
     # an attribute name, a mapping, a callable, or lead to a jitted numba function
     def agg(
         self,
         data: DataFrame,
         func: _AggFuncTypeFrame = ...,
-        *args: Incomplete,
+        *args,
         engine: str | None = None,
         engine_kwargs: dict[str, bool] | None = None,
-        **kwargs: Incomplete,
+        **kwargs,
     ) -> DataFrame: ...
     def apply(
         self, data: DataFrame, func: Callable[Concatenate[DataFrame, _P], DataFrame], *args: _P.args, **kwargs: _P.kwargs
     ) -> DataFrame: ...
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/moves.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/moves.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/plot.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/plot.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 def theme_context(params: dict[str, Any]) -> Generator[None, None, None]: ...
 def build_plot_signature(cls: _ClsT) -> _ClsT: ...  # -> _ClsT & "__signature__ protocol"
 
 class ThemeConfig(mpl.RcParams):
     THEME_GROUPS: list[str]
     def __init__(self) -> None: ...
     def reset(self) -> None: ...
-    def update(self, other: SupportsKeysAndGetItem[Incomplete, Incomplete] | None = None, /, **kwds: Incomplete) -> None: ...  # type: ignore[override]
+    def update(self, other: SupportsKeysAndGetItem[Incomplete, Incomplete] | None = None, /, **kwds) -> None: ...  # type: ignore[override]
 
 class DisplayConfig(TypedDict):
     format: Literal["png", "svg"]
     scaling: float
     hidpi: bool
 
 class PlotConfig:
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/properties.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/rules.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/rules.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/scales.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/scales.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -89,12 +89,12 @@
     def set_data_interval(self, vmin: float, vmax: float) -> None: ...
     def get_data_interval(self) -> tuple[float, float]: ...
     def get_tick_space(self) -> int: ...
     def set_major_locator(self, locator: Locator) -> None: ...
     def set_major_formatter(self, formatter: Formatter) -> None: ...
     def set_minor_locator(self, locator: Locator) -> None: ...
     def set_minor_formatter(self, formatter: Formatter) -> None: ...
-    def set_units(self, units: Incomplete) -> None: ...
-    def update_units(self, x: Incomplete) -> None: ...
-    def convert_units(self, x: Incomplete) -> Incomplete: ...
+    def set_units(self, units) -> None: ...
+    def update_units(self, x) -> None: ...
+    def convert_units(self, x): ...
     def get_scale(self) -> ScaleBase: ...
     def get_majorticklocs(self) -> NDArray[Incomplete]: ...
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/subplots.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/subplots.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_core/typing.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_core/typing.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from numpy import ndarray
 from pandas import DataFrame, Index, Series, Timedelta, Timestamp
 
 @type_check_only
 class SupportsDataFrame(Protocol):
     # `__dataframe__` should return pandas.core.interchange.dataframe_protocol.DataFrame
     # but this class needs to be defined as a Protocol, not as an ABC.
-    def __dataframe__(self, nan_as_null: bool = ..., allow_copy: bool = ...) -> Incomplete: ...
+    def __dataframe__(self, nan_as_null: bool = ..., allow_copy: bool = ...): ...
 
 ColumnName: TypeAlias = str | bytes | date | datetime | timedelta | bool | complex | Timestamp | Timedelta
 Vector: TypeAlias = Series[Any] | Index[Any] | ndarray[Any, Any]
 VariableSpec: TypeAlias = ColumnName | Vector | None
 VariableSpecList: TypeAlias = list[VariableSpec] | Index[Any] | None
 DataSource: TypeAlias = DataFrame | SupportsDataFrame | Mapping[Any, Incomplete] | None
 OrderSpec: TypeAlias = Iterable[str] | None
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/area.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/area.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/bar.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/bar.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/base.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/base.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/dot.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/dot.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/_marks/line.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/_marks/line.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/algorithms.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/algorithms.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/axisgrid.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/axisgrid.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         in_layout: bool = ...,
         label: object = ...,
         mouseover: bool = ...,
         navigate: bool = ...,
         path_effects: list[AbstractPathEffect] = ...,
         picker: bool | float | Callable[[Artist, MouseEvent], tuple[bool, dict[Any, Any]]] | None = ...,
         position: Bbox | tuple[float, float, float, float] = ...,
-        prop_cycle: Incomplete = ...,  # TODO: use cycler.Cycler when cycler gets typed
+        prop_cycle=...,  # TODO: use cycler.Cycler when cycler gets typed
         rasterization_zorder: float | None = ...,
         rasterized: bool = ...,
         sketch_params: float | None = ...,
         snap: bool | None = ...,
         subplotspec: SubplotSpec = ...,
         title: str = ...,
         transform: Transform | None = ...,
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/categorical.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/categorical.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from _typeshed import Incomplete
 from collections.abc import Callable, Iterable
 from typing import Any, Literal
 
 from matplotlib.axes import Axes
 from matplotlib.typing import ColorType, LineStyleType, MarkerType
 
 from ._core.typing import ColumnName, DataSource, Default, NormSpec
@@ -67,17 +66,17 @@
     density_norm: Literal["area", "count", "width"] = "area",
     common_norm: bool | None = False,
     hue_norm: NormSpec = None,
     formatter: Callable[[Any], str] | None = None,
     log_scale: _LogScale | None = None,
     native_scale: bool = False,
     legend: _Legend = "auto",
-    scale: Incomplete = ...,  # deprecated
-    scale_hue: Incomplete = ...,  # deprecated
-    bw: Incomplete = ...,  # deprecated
+    scale=...,  # deprecated
+    scale_hue=...,  # deprecated
+    bw=...,  # deprecated
     inner_kws: dict[str, Any] | None = None,
     ax: Axes | None = None,
     **kwargs: Any,
 ) -> Axes: ...
 def boxenplot(
     data: DataSource | _DataSourceWideForm | None = None,
     *,
@@ -102,15 +101,15 @@
     trust_alpha: float = 0.05,
     showfliers: bool = True,
     hue_norm: NormSpec = None,
     log_scale: _LogScale | None = None,
     native_scale: bool = False,
     formatter: Callable[[Any], str] | None = None,
     legend: _Legend = "auto",
-    scale: Incomplete = ...,  # deprecated
+    scale=...,  # deprecated
     box_kws: dict[str, Any] | None = None,
     flier_kws: dict[str, Any] | None = None,
     line_kws: dict[str, Any] | None = None,
     ax: Axes | None = None,
     **kwargs: Any,
 ) -> Axes: ...
 def stripplot(
@@ -186,17 +185,17 @@
     gap: float = 0,
     log_scale: _LogScale | None = None,
     native_scale: bool = False,
     formatter: Callable[[Any], str] | None = None,
     legend: _Legend = "auto",
     capsize: float = 0,
     err_kws: dict[str, Any] | None = None,
-    ci: Incomplete = ...,  # deprecated
-    errcolor: Incomplete = ...,  # deprecated
-    errwidth: Incomplete = ...,  # deprecated
+    ci=...,  # deprecated
+    errcolor=...,  # deprecated
+    errwidth=...,  # deprecated
     ax: Axes | None = None,
     **kwargs: Any,
 ) -> Axes: ...
 def pointplot(
     data: DataSource | _DataSourceWideForm | None = None,
     *,
     x: ColumnName | _Vector | None = None,
@@ -219,18 +218,18 @@
     log_scale: _LogScale | None = None,
     native_scale: bool = False,
     orient: Literal["v", "h", "x", "y"] | None = None,
     capsize: float = 0,
     formatter: Callable[[Any], str] | None = None,
     legend: _Legend = "auto",
     err_kws: dict[str, Any] | None = None,
-    ci: Incomplete = ...,  # deprecated
-    errwidth: Incomplete = ...,  # deprecated
-    join: Incomplete = ...,  # deprecated
-    scale: Incomplete = ...,  # deprecated
+    ci=...,  # deprecated
+    errwidth=...,  # deprecated
+    join=...,  # deprecated
+    scale=...,  # deprecated
     ax: Axes | None = None,
     **kwargs: Any,
 ) -> Axes: ...
 def countplot(
     data: DataSource | _DataSourceWideForm | None = None,
     *,
     x: ColumnName | _Vector | None = None,
@@ -286,10 +285,10 @@
     hue_norm: NormSpec = None,
     legend: _Legend = "auto",
     legend_out: bool = True,
     sharex: bool = True,
     sharey: bool = True,
     margin_titles: bool = False,
     facet_kws: dict[str, Any] | None = None,
-    ci: Incomplete = ...,  # deprecated
+    ci=...,  # deprecated
     **kwargs: Any,
 ) -> FacetGrid: ...
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/distributions.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/distributions.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/external/docscrape.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/external/docscrape.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/external/husl.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/external/husl.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/external/kde.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/external/kde.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/external/version.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/external/version.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/matrix.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/matrix.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     cbar_kws: dict[str, Incomplete] | None = None,
     cbar_ax: Axes | None = None,
     square: bool = False,
     xticklabels: Literal["auto"] | bool | int | Sequence[str] = "auto",
     yticklabels: Literal["auto"] | bool | int | Sequence[str] = "auto",
     mask: NDArray[np.bool_] | DataFrame | None = None,
     ax: Axes | None = None,
-    **kwargs: Incomplete,
+    **kwargs,
 ) -> Axes: ...
 
 class _DendrogramPlotter:
     axis: int
     array: NDArray[Incomplete]
     data: DataFrame
     shape: tuple[int, int]
@@ -146,29 +146,27 @@
         col_cluster: bool,
         metric: str,
         method: str,
         row_linkage: NDArray[Incomplete] | None,
         col_linkage: NDArray[Incomplete] | None,
         tree_kws: dict[str, Incomplete] | None,
     ) -> None: ...
-    def plot_colors(self, xind: _ArrayLikeInt_co, yind: _ArrayLikeInt_co, **kws: Incomplete) -> None: ...
-    def plot_matrix(
-        self, colorbar_kws: dict[str, Incomplete], xind: _ArrayLikeInt_co, yind: _ArrayLikeInt_co, **kws: Incomplete
-    ) -> None: ...
+    def plot_colors(self, xind: _ArrayLikeInt_co, yind: _ArrayLikeInt_co, **kws) -> None: ...
+    def plot_matrix(self, colorbar_kws: dict[str, Incomplete], xind: _ArrayLikeInt_co, yind: _ArrayLikeInt_co, **kws) -> None: ...
     def plot(
         self,
         metric: str,
         method: str,
         colorbar_kws: dict[str, Incomplete] | None,
         row_cluster: bool,
         col_cluster: bool,
         row_linkage: NDArray[Incomplete] | None,
         col_linkage: NDArray[Incomplete] | None,
         tree_kws: dict[str, Incomplete] | None,
-        **kws: Incomplete,
+        **kws,
     ) -> Self: ...
 
 def clustermap(
     data: (
         _ListLikeU
         | DataFrame
         | dict[Incomplete, Incomplete]
@@ -190,9 +188,9 @@
     row_colors: Incomplete | None = None,
     col_colors: Incomplete | None = None,
     mask: NDArray[np.bool_] | DataFrame | None = None,
     dendrogram_ratio: float | tuple[float, float] = 0.2,
     colors_ratio: float | tuple[float, float] = 0.03,
     cbar_pos: tuple[float, float, float, float] | None = (0.02, 0.8, 0.05, 0.18),
     tree_kws: dict[str, Incomplete] | None = None,
-    **kwargs: Incomplete,
+    **kwargs,
 ) -> ClusterGrid: ...
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/objects.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/objects.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/palettes.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/palettes.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/rcmod.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/rcmod.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/regression.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/regression.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/relational.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/relational.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/utils.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,15 @@
     a: float | ArrayLike, which: float | ArrayLike = 95, axis: SupportsIndex | Sequence[SupportsIndex] | None = None
 ) -> NDArray[np.float64]: ...
 def get_dataset_names() -> list[str]: ...
 def get_data_home(data_home: str | None = None) -> str: ...
 def load_dataset(name: str, cache: bool = True, data_home: str | None = None, **kws: Any) -> DataFrame: ...
 def axis_ticklabels_overlap(labels: Iterable[Text]) -> bool: ...
 def axes_ticklabels_overlap(ax: Axes) -> tuple[bool, bool]: ...
-def locator_to_legend_entries(
-    locator: Locator, limits: Iterable[float], dtype: Incomplete
-) -> tuple[list[Incomplete], list[str]]: ...
+def locator_to_legend_entries(locator: Locator, limits: Iterable[float], dtype) -> tuple[list[Incomplete], list[str]]: ...
 @overload
 def relative_luminance(color: ColorType) -> float: ...  # type: ignore[overload-overlap]
 @overload
 def relative_luminance(color: Sequence[ColorType]) -> NDArray[np.float64]: ...
 @overload
 def relative_luminance(color: ColorType | Sequence[ColorType] | ArrayLike) -> float | NDArray[np.float64]: ...
 def to_utf8(obj: object) -> str: ...
```

### Comparing `types-seaborn-0.13.2.20240311/seaborn-stubs/widgets.pyi` & `types-seaborn-0.13.2.20240417/seaborn-stubs/widgets.pyi`

 * *Files identical despite different names*

### Comparing `types-seaborn-0.13.2.20240311/setup.py` & `types-seaborn-0.13.2.20240417/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-seaborn` aims to provide accurate annotations
 for `seaborn==0.13.2`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/seaborn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="0.13.2.20240311",
+      version="0.13.2.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/seaborn.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['matplotlib>=3.8', 'numpy>=1.20', 'pandas-stubs'],
       packages=['seaborn-stubs'],
-      package_data={'seaborn-stubs': ['__init__.pyi', '_core/__init__.pyi', '_core/data.pyi', '_core/exceptions.pyi', '_core/groupby.pyi', '_core/moves.pyi', '_core/plot.pyi', '_core/properties.pyi', '_core/rules.pyi', '_core/scales.pyi', '_core/subplots.pyi', '_core/typing.pyi', '_marks/__init__.pyi', '_marks/area.pyi', '_marks/bar.pyi', '_marks/base.pyi', '_marks/dot.pyi', '_marks/line.pyi', '_marks/text.pyi', '_stats/__init__.pyi', '_stats/aggregation.pyi', '_stats/base.pyi', '_stats/counting.pyi', '_stats/density.pyi', '_stats/order.pyi', '_stats/regression.pyi', 'algorithms.pyi', 'axisgrid.pyi', 'categorical.pyi', 'cm.pyi', 'colors/__init__.pyi', 'colors/crayons.pyi', 'colors/xkcd_rgb.pyi', 'distributions.pyi', 'external/__init__.pyi', 'external/appdirs.pyi', 'external/docscrape.pyi', 'external/husl.pyi', 'external/kde.pyi', 'external/version.pyi', 'matrix.pyi', 'miscplot.pyi', 'objects.pyi', 'palettes.pyi', 'rcmod.pyi', 'regression.pyi', 'relational.pyi', 'utils.pyi', 'widgets.pyi', 'METADATA.toml']},
+      package_data={'seaborn-stubs': ['__init__.pyi', '_core/__init__.pyi', '_core/data.pyi', '_core/exceptions.pyi', '_core/groupby.pyi', '_core/moves.pyi', '_core/plot.pyi', '_core/properties.pyi', '_core/rules.pyi', '_core/scales.pyi', '_core/subplots.pyi', '_core/typing.pyi', '_marks/__init__.pyi', '_marks/area.pyi', '_marks/bar.pyi', '_marks/base.pyi', '_marks/dot.pyi', '_marks/line.pyi', '_marks/text.pyi', '_stats/__init__.pyi', '_stats/aggregation.pyi', '_stats/base.pyi', '_stats/counting.pyi', '_stats/density.pyi', '_stats/order.pyi', '_stats/regression.pyi', 'algorithms.pyi', 'axisgrid.pyi', 'categorical.pyi', 'cm.pyi', 'colors/__init__.pyi', 'colors/crayons.pyi', 'colors/xkcd_rgb.pyi', 'distributions.pyi', 'external/__init__.pyi', 'external/appdirs.pyi', 'external/docscrape.pyi', 'external/husl.pyi', 'external/kde.pyi', 'external/version.pyi', 'matrix.pyi', 'miscplot.pyi', 'objects.pyi', 'palettes.pyi', 'rcmod.pyi', 'regression.pyi', 'relational.pyi', 'utils.pyi', 'widgets.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.9",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-seaborn-0.13.2.20240311/types_seaborn.egg-info/PKG-INFO` & `types-seaborn-0.13.2.20240417/types_seaborn.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-seaborn
-Version: 0.13.2.20240311
+Version: 0.13.2.20240417
 Summary: Typing stubs for seaborn
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/seaborn.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-seaborn` aims to provide accurate annotations
 for `seaborn==0.13.2`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/seaborn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-seaborn-0.13.2.20240311/types_seaborn.egg-info/SOURCES.txt` & `types-seaborn-0.13.2.20240417/types_seaborn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 seaborn-stubs/categorical.pyi
 seaborn-stubs/cm.pyi
 seaborn-stubs/distributions.pyi
 seaborn-stubs/matrix.pyi
 seaborn-stubs/miscplot.pyi
 seaborn-stubs/objects.pyi
 seaborn-stubs/palettes.pyi
+seaborn-stubs/py.typed
 seaborn-stubs/rcmod.pyi
 seaborn-stubs/regression.pyi
 seaborn-stubs/relational.pyi
 seaborn-stubs/utils.pyi
 seaborn-stubs/widgets.pyi
 seaborn-stubs/_core/__init__.pyi
 seaborn-stubs/_core/data.pyi
```

