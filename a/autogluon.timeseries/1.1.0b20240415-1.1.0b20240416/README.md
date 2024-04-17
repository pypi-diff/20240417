# Comparing `tmp/autogluon.timeseries-1.1.0b20240415.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.0b20240415.tar", last modified: Mon Apr 15 09:05:01 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240416.tar", last modified: Tue Apr 16 09:05:13 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.0b20240415.tar` & `autogluon.timeseries-1.1.0b20240416.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.312670 autogluon.timeseries-1.1.0b20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.312670 autogluon.timeseries-1.1.0b20240415/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.316670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.316670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.316670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:37.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.320670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81823 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.324670 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 09:03:38.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:01.316670 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:05:01.000000 autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.481828 autogluon.timeseries-1.1.0b20240416/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.481828 autogluon.timeseries-1.1.0b20240416/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.485828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.485828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.485828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.489828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81910 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59104 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.493828 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19585 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-16 09:03:38.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:05:13.485828 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:05:13.000000 autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.0b20240415/PKG-INFO` & `autogluon.timeseries-1.1.0b20240416/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240415
+Version: 1.1.0b20240416
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240415/setup.py` & `autogluon.timeseries-1.1.0b20240416/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     chronos_large={
         "hyperparameters": {"Chronos": {"model_path": "large", "batch_size": 8}},
         "skip_model_selection": True,
     },
     chronos_ensemble={
         "hyperparameters": {
             "Chronos": {"model_path": "small"},
-            **get_default_hps("default"),
+            **get_default_hps("light_inference"),
         }
     },
     chronos_large_ensemble={
         "hyperparameters": {
             "Chronos": {"model_path": "large", "batch_size": 8},
-            **get_default_hps("default"),
+            **get_default_hps("light_inference"),
         }
     },
 )
 
 TIMESERIES_PRESETS_ALIASES = dict(
     chronos="chronos_small",
     best="best_quality",
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,18 @@
             df = pd.merge(df, static_features, how="left", on=ITEMID, suffixes=(None, "_static_feat"))
 
         for col in self.metadata.known_covariates_real:
             # Normalize non-boolean features using mean_abs scaling
             if not df[col].isin([0, 1]).all():
                 df[f"__scaled_{col}"] = df[col] / df[col].abs().groupby(df[ITEMID]).mean().reindex(df[ITEMID]).values
 
+        # Convert float64 to float32 to reduce memory usage
+        float64_cols = list(df.select_dtypes(include="float64"))
+        df[float64_cols] = df[float64_cols].astype("float32")
+
         # We assume that df is sorted by 'unique_id' inside `TimeSeriesPredictor._check_and_prepare_data_frame`
         return df.rename(columns=column_name_mapping)
 
     def _fit(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,14 @@
         """Fast implementation of forward fill in numpy."""
         idx = np.arange(len(arr))
         mask = np.isnan(arr)
         idx[mask] = 0
         return arr[np.maximum.accumulate(idx)]
 
     forecast = {}
-    # Convert to float64 since std computation can be unstable in float32
-    target = target.astype(np.float64)
     # At least seasonal_period + 2 values are required to compute sigma for seasonal naive
     if len(target) > seasonal_period + 1 and seasonal_period > 1:
         if np.isnan(target[-(seasonal_period + 2) :]).any():
             target = numpy_ffill(target)
 
         indices = [len(target) - seasonal_period + k % seasonal_period for k in range(prediction_length)]
         forecast["mean"] = target[indices]
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/models/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,29 +75,31 @@
 DEFAULT_MODEL_NAMES = {v: k for k, v in MODEL_TYPES.items()}
 DEFAULT_MODEL_PRIORITY = dict(
     Naive=100,
     SeasonalNaive=100,
     Average=100,
     SeasonalAverage=100,
     Zero=100,
-    NPTS=90,
-    ETS=90,
-    CrostonSBA=90,
-    Theta=80,
-    DynamicOptimizedTheta=80,
-    AutoETS=80,
-    AutoARIMA=70,
-    RecursiveTabular=60,
-    Chronos=50,
-    DirectTabular=50,
+    RecursiveTabular=90,
+    DirectTabular=85,
+    # All local models are grouped together to make sure that joblib parallel pool is reused
+    NPTS=80,
+    ETS=80,
+    CrostonSBA=80,
+    Theta=75,
+    DynamicOptimizedTheta=75,
+    AutoETS=70,
+    AutoARIMA=60,
+    Chronos=55,
+    # Models that can early stop are trained at the end
+    TemporalFusionTransformer=45,
     DeepAR=40,
-    TemporalFusionTransformer=30,
-    WaveNet=25,
-    PatchTST=20,
+    PatchTST=30,
     # Models below are not included in any presets
+    WaveNet=25,
     AutoCES=10,
     ARIMA=10,
     ADIDA=10,
     IMAPA=10,
     SimpleFeedForward=10,
 )
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
@@ -124,14 +126,21 @@
             "SeasonalNaive": {},
             "ETS": {},
             "Theta": {},
             "RecursiveTabular": {},
             "DirectTabular": {},
             "TemporalFusionTransformer": {},
         },
+        "light_inference": {
+            "SeasonalNaive": {},
+            "DirectTabular": {},
+            "RecursiveTabular": {},
+            "TemporalFusionTransformer": {},
+            "PatchTST": {},
+        },
         "default": {
             "SeasonalNaive": {},
             "CrostonSBA": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "NPTS": {},
             "DynamicOptimizedTheta": {},
@@ -139,14 +148,15 @@
             "RecursiveTabular": {
                 "tabular_hyperparameters": {"NN_TORCH": {"proc.impute_strategy": "constant"}, "GBM": {}},
             },
             "DirectTabular": {},
             "TemporalFusionTransformer": {},
             "PatchTST": {},
             "DeepAR": {},
+            "Chronos": {"model_path": "base"},
         },
     }
     return default_model_hps[key]
 
 
 def get_preset_models(
     freq: str,
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
         Returns
         -------
         df : TimeSeriesDataFrame
             Preprocessed data in TimeSeriesDataFrame format.
         """
         df = self._to_data_frame(data, name=name)
-        df = df.astype({self.target: "float32"})
+        df = df.astype({self.target: "float64"})
         # MultiIndex.is_monotonic_increasing checks if index is sorted by ["item_id", "timestamp"]
         if not df.index.is_monotonic_increasing:
             df = df.sort_index()
             df._cached_freq = None  # in case frequency was incorrectly cached as IRREGULAR_TIME_INDEX_FREQSTR
 
         # Ensure that data has a regular frequency that matches the predictor frequency
         if self.freq is None:
@@ -495,24 +495,26 @@
 
             - ``"fast_training"``: fit simple statistical models (``ETS``, ``Theta``, ``Naive``, ``SeasonalNaive``) + fast tree-based models ``RecursiveTabular``
               and ``DirectTabular``. These models are fast to train but may not be very accurate.
             - ``"medium_quality"``: all models mentioned above + deep learning model ``TemporalFusionTransformer``. Default setting that produces good forecasts
               with reasonable training time.
             - ``"high_quality"``: All ML models available in AutoGluon + additional statistical models (``NPTS``, ``AutoETS``, ``AutoARIMA``, ``CrostonSBA``,
               ``DynamicOptimizedTheta``). Much more accurate than ``medium_quality``, but takes longer to train.
-            - ``"best_quality"``: Same models as in ``"high_quality"`, but performs validation with multiple backtests. Usually better than ``high_quality``, but takes even longer to train.
+            - ``"best_quality"``: Same models as in ``"high_quality"``, but performs validation with multiple backtests. Usually better than ``high_quality``, but takes even longer to train.
 
             Available presets with the `Chronos <https://github.com/amazon-science/chronos-forecasting>`_ model:
 
             - ``"chronos_{model_size}"``: where model size is one of ``tiny,mini,small,base,large``. Uses the Chronos pretrained model for zero-shot forecasting.
               See the documentation for ``ChronosModel`` or see `Hugging Face <https://huggingface.co/collections/amazon/chronos-models-65f1791d630a8d57cb718444>`_ for more information.
               Note that a GPU is required for model sizes ``small``, ``base`` and ``large``.
             - ``"chronos"``: alias for ``"chronos_small"``.
-            - ``"chronos_ensemble"``: builds an ensemble of the models specified in ``"high_quality"`` and ``"chronos_small"``.
-            - ``"chronos_large_ensemble"``: builds an ensemble of the models specified in ``"high_quality"`` and ``"chronos_large"``.
+            - ``"chronos_ensemble"``: builds an ensemble of seasonal naive, tree-based and deep learning models with fast inference
+              and ``"chronos_small"``.
+            - ``"chronos_large_ensemble"``: builds an ensemble of seasonal naive, tree-based and deep learning models
+              with fast inference and ``"chronos_large"``.
 
             Details for these presets can be found in ``autogluon/timeseries/configs/presets_configs.py``. If not
             provided, user-provided values for ``hyperparameters`` and ``hyperparameter_tune_kwargs`` will be used
             (defaulting to their default values specified below).
         hyperparameters : str or dict, optional
             Determines what models are trained and what hyperparameters are used by each model.
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
                     time_reserved_for_ensemble = 0.0
                 time_left_for_model = (time_left - time_reserved_for_ensemble) / (num_base_models - i)
                 if time_left <= 0:
                     logger.info(f"Stopping training due to lack of time remaining. Time left: {time_left:.1f} seconds")
                     break
 
             if random_seed is not None:
-                seed_everything(random_seed)
+                seed_everything(random_seed + i)
 
             if contains_searchspace(model.get_user_params()):
                 fit_log_message = f"Hyperparameter tuning model {model.name}. "
                 if time_left is not None:
                     fit_log_message += (
                         f"Tuning model for up to {time_left_for_model:.1f}s of the {time_left:.1f}s remaining."
                     )
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 class ContinuousAndCategoricalFeatureGenerator(PipelineFeatureGenerator):
     """Generates categorical and continuous features for time series models.
 
     Imputes missing categorical features with the most frequent value in the training set.
     """
 
-    def __init__(self, verbosity: int = 0, minimum_cat_count=2, float_dtype: str = "float32", **kwargs):
+    def __init__(self, verbosity: int = 0, minimum_cat_count=2, float_dtype: str = "float64", **kwargs):
         generators = [
             CategoryFeatureGenerator(minimum_cat_count=minimum_cat_count, fillna="mode"),
             IdentityFeatureGenerator(infer_features_in_args={"valid_raw_types": [R_INT, R_FLOAT]}),
         ]
         super().__init__(
             generators=[generators],
             post_generators=[],
@@ -107,34 +107,36 @@
         # Ignore the '__dummy__' feature generated by PipelineFeatureGenerator if none of the features are informative
         return transformed.drop(columns=["__dummy__"], errors="ignore")
 
 
 class TimeSeriesFeatureGenerator:
     """Takes care of preprocessing for static_features and past/known covariates.
 
-    All covariates & static features are converted into either float32 or categorical dtype.
+    All covariates & static features are converted into either float64 or categorical dtype.
 
     Missing values in the target column are left as-is but missing values in static features & covariates are imputed.
     Imputation logic is as follows:
     1. For all categorical columns (static, past, known), we fill missing values with the mode of the training set.
     2. For real static features, we impute missing values with the median of the training set.
     3. For real covariates (past, known), we ffill + bfill within each time series. If for some time series all
         covariate values are missing, we fill them with the median of the training set.
     """
 
-    def __init__(self, target: str, known_covariates_names: List[str], float_dtype: str = "float32"):
+    def __init__(self, target: str, known_covariates_names: List[str], float_dtype: str = "float64"):
         self.target = target
         self.float_dtype = float_dtype
         self._is_fit = False
         self.known_covariates_names = list(known_covariates_names)
         self.past_covariates_names = []
-        self.known_covariates_pipeline = ContinuousAndCategoricalFeatureGenerator()
-        self.past_covariates_pipeline = ContinuousAndCategoricalFeatureGenerator()
+        self.known_covariates_pipeline = ContinuousAndCategoricalFeatureGenerator(float_dtype=float_dtype)
+        self.past_covariates_pipeline = ContinuousAndCategoricalFeatureGenerator(float_dtype=float_dtype)
         # Cat features with cat_count=1 are fine in static_features since they are repeated for all time steps in a TS
-        self.static_feature_pipeline = ContinuousAndCategoricalFeatureGenerator(minimum_cat_count=1)
+        self.static_feature_pipeline = ContinuousAndCategoricalFeatureGenerator(
+            minimum_cat_count=1, float_dtype=float_dtype
+        )
         self.covariate_metadata: CovariateMetadata = None
         self._train_covariates_real_median: Optional[pd.Series] = None
         self._train_static_real_median: Optional[pd.Series] = None
 
     @property
     def required_column_names(self) -> List[str]:
         return [self.target] + list(self.known_covariates_names) + list(self.past_covariates_names)
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240416/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240415
+Version: 1.1.0b20240416
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240415/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240416/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.0b20240415
-autogluon.common==1.1.0b20240415
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240415
+autogluon.core[raytune]==1.1.0b20240416
+autogluon.common==1.1.0b20240416
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240416
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

