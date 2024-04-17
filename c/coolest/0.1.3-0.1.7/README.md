# Comparing `tmp/coolest-0.1.3.tar.gz` & `tmp/coolest-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolest-0.1.3.tar", last modified: Wed Apr 17 09:49:36 2024, max compression
+gzip compressed data, was "coolest-0.1.7.tar", last modified: Wed Apr 17 13:24:59 2024, max compression
```

## Comparing `coolest-0.1.3.tar` & `coolest-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.414562 coolest-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 09:49:31.000000 coolest-0.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 09:49:31.000000 coolest-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-17 09:49:36.414562 coolest-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-17 09:49:31.000000 coolest-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.402562 coolest-0.1.3/coolest/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.406562 coolest-0.1.3/coolest/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25834 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/composable_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/plot_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    49576 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.406562 coolest-0.1.3/coolest/api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/profiles/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/profiles/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/profiles/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    28422 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.406562 coolest-0.1.3/coolest/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.410562 coolest-0.1.3/coolest/template/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/fits_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/lensing_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/lensing_entity_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/likelihood_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/mass_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/mass_light_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/profile_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.414562 coolest-0.1.3/coolest/template/classes/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/profiles/light.py
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/profiles/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/regularization_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.414562 coolest-0.1.3/coolest/template/classes/regularizations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/regularizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/regularizations/pixelated.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/classes/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-17 09:49:31.000000 coolest-0.1.3/coolest/template/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:49:36.414562 coolest-0.1.3/coolest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-17 09:49:36.000000 coolest-0.1.3/coolest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-17 09:49:36.000000 coolest-0.1.3/coolest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:49:36.000000 coolest-0.1.3/coolest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 09:49:36.000000 coolest-0.1.3/coolest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:49:36.000000 coolest-0.1.3/coolest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 09:49:31.000000 coolest-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:49:36.414562 coolest-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 09:49:31.000000 coolest-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.737978 coolest-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 13:24:50.000000 coolest-0.1.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 13:24:50.000000 coolest-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-17 13:24:59.737978 coolest-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-17 13:24:50.000000 coolest-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.729978 coolest-0.1.7/coolest/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.729978 coolest-0.1.7/coolest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25834 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/composable_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/plot_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49576 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.729978 coolest-0.1.7/coolest/api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/profiles/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/profiles/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/profiles/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28422 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.733978 coolest-0.1.7/coolest/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.733978 coolest-0.1.7/coolest/template/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/fits_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/lensing_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/lensing_entity_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/likelihood_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/mass_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/mass_light_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/profile_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.737978 coolest-0.1.7/coolest/template/classes/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/profiles/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/profiles/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/regularization_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.737978 coolest-0.1.7/coolest/template/classes/regularizations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/regularizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/regularizations/pixelated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/classes/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-17 13:24:50.000000 coolest-0.1.7/coolest/template/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:59.737978 coolest-0.1.7/coolest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-17 13:24:59.000000 coolest-0.1.7/coolest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 13:24:59.000000 coolest-0.1.7/coolest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:24:59.000000 coolest-0.1.7/coolest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 13:24:59.000000 coolest-0.1.7/coolest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 13:24:59.000000 coolest-0.1.7/coolest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 13:24:50.000000 coolest-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 13:24:59.737978 coolest-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-17 13:24:50.000000 coolest-0.1.7/setup.py
```

### Comparing `coolest-0.1.3/LICENSE` & `coolest-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/PKG-INFO` & `coolest-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: coolest
-Version: 0.1.3
-Summary: builtins Author: COOLEST developers, Email: aymeric.galan@gmail.com, Year: 2021-2024, Standard for Strong Gravitational Lens Modeling
+Version: 0.1.7
+Summary: Standard for Strong Gravitational Lensing Analyses
 Home-page: https://github.com/aymgal/COOLEST
-Author: COOLEST developers
+Download-URL: https://github.com/aymgal/coolest/archive/refs/tags/v0.1.7.tar.gz
+Author: Aymeric Galan & COOLEST contributors
 Author-email: aymeric.galan@gmail.com
 License: GPL-3.0
+Project-URL: Documentation, https://coolest.readthedocs.io/
+Project-URL: Changelog, https://github.com/aymgal/COOLEST/blob/main/HISTORY.md
+Keywords: coolest,lensing,gravitation,astrophysics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.6.3
 Requires-Dist: jsonpickle>=2.0.0
@@ -17,20 +21,20 @@
 Provides-Extra: opt
 Requires-Dist: matplotlib>=3.7.0; extra == "opt"
 Requires-Dist: lenstronomy>=1.11.0; extra == "opt"
 Requires-Dist: ipython; extra == "opt"
 Requires-Dist: ipykernel; extra == "opt"
 Requires-Dist: getdist>=1.3.2; extra == "opt"
 
-<img src="docs/_static/coolest_logo.png#gh-light-mode-only" width="200" alt="COOLEST logo" />
-<img src="docs/_static/coolest_logo_dark_bg.png#gh-dark-mode-only" width="200" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo.png#gh-light-mode-only" width="600" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo_dark_bg.png#gh-dark-mode-only" width="600" alt="COOLEST logo" />
 
-# COOLEST: a standard for strong gravitational lensing studies
+# Standard for Strong Gravitational Lensing Analyses
 
-![PyPi python support](https://img.shields.io/badge/Python-3.8-blue)
+![PyPi python support](https://img.shields.io/badge/Python-3.11-blue)
 [![Tests](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml/badge.svg?branch=main)](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/aymgal/COOLEST/badge.svg)](https://coveralls.io/github/aymgal/COOLEST)
 [![Documentation Status](https://readthedocs.org/projects/coolest/badge/?version=latest)](https://coolest.readthedocs.io/en/latest/?badge=latest)
 ![License](https://img.shields.io/github/license/aymgal/COOLEST)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05567/status.svg)](https://doi.org/10.21105/joss.05567)
 
 ## What is COOLEST?
```

### Comparing `coolest-0.1.3/README.md` & `coolest-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-<img src="docs/_static/coolest_logo.png#gh-light-mode-only" width="200" alt="COOLEST logo" />
-<img src="docs/_static/coolest_logo_dark_bg.png#gh-dark-mode-only" width="200" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo.png#gh-light-mode-only" width="600" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo_dark_bg.png#gh-dark-mode-only" width="600" alt="COOLEST logo" />
 
-# COOLEST: a standard for strong gravitational lensing studies
+# Standard for Strong Gravitational Lensing Analyses
 
-![PyPi python support](https://img.shields.io/badge/Python-3.8-blue)
+![PyPi python support](https://img.shields.io/badge/Python-3.11-blue)
 [![Tests](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml/badge.svg?branch=main)](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/aymgal/COOLEST/badge.svg)](https://coveralls.io/github/aymgal/COOLEST)
 [![Documentation Status](https://readthedocs.org/projects/coolest/badge/?version=latest)](https://coolest.readthedocs.io/en/latest/?badge=latest)
 ![License](https://img.shields.io/github/license/aymgal/COOLEST)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05567/status.svg)](https://doi.org/10.21105/joss.05567)
 
 ## What is COOLEST?
```

### Comparing `coolest-0.1.3/coolest/__init__.py` & `coolest-0.1.7/coolest/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 This file initializes the coolest module
 and provides some basic information about the package.
 
 """
 
 # Set the package release version
-version_info = (0, 1, 3)
+version_info = (0, 1, 7)
 __version__ = '.'.join(str(c) for c in version_info)
 
 # Set the package details
-__author__ = 'COOLEST developers'
+__author__ = 'Aymeric Galan & COOLEST contributors'
 __email__ = 'aymeric.galan@gmail.com'
 __year__ = '2021-2024'
-__credits__ = 'COOLEST developers'
+__credits__ = 'COOLEST contributors'
 __url__ = 'https://github.com/aymgal/COOLEST'
-__description__ = 'Standard for Strong Gravitational Lens Modeling'
-
-# Default package properties
+__description__ = 'Standard for Strong Gravitational Lensing Analyses'
 __license__ = 'GPL-3.0'
-__about__ = ('{} Author: {}, Email: {}, Year: {}, {}'
-             ''.format(__name__, __author__, __email__, __year__,
-                       __description__))
-
```

### Comparing `coolest-0.1.3/coolest/api/analysis.py` & `coolest-0.1.7/coolest/api/analysis.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/composable_models.py` & `coolest-0.1.7/coolest/api/composable_models.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/coordinates.py` & `coolest-0.1.7/coolest/api/coordinates.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/plot_util.py` & `coolest-0.1.7/coolest/api/plot_util.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/plotting.py` & `coolest-0.1.7/coolest/api/plotting.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/profiles/light.py` & `coolest-0.1.7/coolest/api/profiles/light.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/profiles/mass.py` & `coolest-0.1.7/coolest/api/profiles/mass.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/profiles/util.py` & `coolest-0.1.7/coolest/api/profiles/util.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/api/util.py` & `coolest-0.1.7/coolest/api/util.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/base.py` & `coolest-0.1.7/coolest/template/classes/base.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/coordinates.py` & `coolest-0.1.7/coolest/template/classes/coordinates.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/cosmology.py` & `coolest-0.1.7/coolest/template/classes/cosmology.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/fits_file.py` & `coolest-0.1.7/coolest/template/classes/fits_file.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/galaxy.py` & `coolest-0.1.7/coolest/template/classes/galaxy.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/grid.py` & `coolest-0.1.7/coolest/template/classes/grid.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/instrument.py` & `coolest-0.1.7/coolest/template/classes/instrument.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/lensing_entity.py` & `coolest-0.1.7/coolest/template/classes/lensing_entity.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/lensing_entity_list.py` & `coolest-0.1.7/coolest/template/classes/lensing_entity_list.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/likelihood_list.py` & `coolest-0.1.7/coolest/template/classes/likelihood_list.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/mass_field.py` & `coolest-0.1.7/coolest/template/classes/mass_field.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/mass_light_model.py` & `coolest-0.1.7/coolest/template/classes/mass_light_model.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/noise.py` & `coolest-0.1.7/coolest/template/classes/noise.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/observation.py` & `coolest-0.1.7/coolest/template/classes/observation.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/parameter.py` & `coolest-0.1.7/coolest/template/classes/parameter.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/probabilities.py` & `coolest-0.1.7/coolest/template/classes/probabilities.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/profile.py` & `coolest-0.1.7/coolest/template/classes/profile.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/profile_list.py` & `coolest-0.1.7/coolest/template/classes/profile_list.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/profiles/light.py` & `coolest-0.1.7/coolest/template/classes/profiles/light.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/profiles/mass.py` & `coolest-0.1.7/coolest/template/classes/profiles/mass.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/psf.py` & `coolest-0.1.7/coolest/template/classes/psf.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/regularization.py` & `coolest-0.1.7/coolest/template/classes/regularization.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/regularization_list.py` & `coolest-0.1.7/coolest/template/classes/regularization_list.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/regularizations/pixelated.py` & `coolest-0.1.7/coolest/template/classes/regularizations/pixelated.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/classes/util.py` & `coolest-0.1.7/coolest/template/classes/util.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/info.py` & `coolest-0.1.7/coolest/template/info.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/json.py` & `coolest-0.1.7/coolest/template/json.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/lazy.py` & `coolest-0.1.7/coolest/template/lazy.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest/template/standard.py` & `coolest-0.1.7/coolest/template/standard.py`

 * *Files identical despite different names*

### Comparing `coolest-0.1.3/coolest.egg-info/PKG-INFO` & `coolest-0.1.7/coolest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: coolest
-Version: 0.1.3
-Summary: builtins Author: COOLEST developers, Email: aymeric.galan@gmail.com, Year: 2021-2024, Standard for Strong Gravitational Lens Modeling
+Version: 0.1.7
+Summary: Standard for Strong Gravitational Lensing Analyses
 Home-page: https://github.com/aymgal/COOLEST
-Author: COOLEST developers
+Download-URL: https://github.com/aymgal/coolest/archive/refs/tags/v0.1.7.tar.gz
+Author: Aymeric Galan & COOLEST contributors
 Author-email: aymeric.galan@gmail.com
 License: GPL-3.0
+Project-URL: Documentation, https://coolest.readthedocs.io/
+Project-URL: Changelog, https://github.com/aymgal/COOLEST/blob/main/HISTORY.md
+Keywords: coolest,lensing,gravitation,astrophysics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.6.3
 Requires-Dist: jsonpickle>=2.0.0
@@ -17,20 +21,20 @@
 Provides-Extra: opt
 Requires-Dist: matplotlib>=3.7.0; extra == "opt"
 Requires-Dist: lenstronomy>=1.11.0; extra == "opt"
 Requires-Dist: ipython; extra == "opt"
 Requires-Dist: ipykernel; extra == "opt"
 Requires-Dist: getdist>=1.3.2; extra == "opt"
 
-<img src="docs/_static/coolest_logo.png#gh-light-mode-only" width="200" alt="COOLEST logo" />
-<img src="docs/_static/coolest_logo_dark_bg.png#gh-dark-mode-only" width="200" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo.png#gh-light-mode-only" width="600" alt="COOLEST logo" />
+<img src="https://raw.githubusercontent.com/aymgal/COOLEST/main/images/full_logo_dark_bg.png#gh-dark-mode-only" width="600" alt="COOLEST logo" />
 
-# COOLEST: a standard for strong gravitational lensing studies
+# Standard for Strong Gravitational Lensing Analyses
 
-![PyPi python support](https://img.shields.io/badge/Python-3.8-blue)
+![PyPi python support](https://img.shields.io/badge/Python-3.11-blue)
 [![Tests](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml/badge.svg?branch=main)](https://github.com/aymgal/COOLEST/actions/workflows/ci-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/aymgal/COOLEST/badge.svg)](https://coveralls.io/github/aymgal/COOLEST)
 [![Documentation Status](https://readthedocs.org/projects/coolest/badge/?version=latest)](https://coolest.readthedocs.io/en/latest/?badge=latest)
 ![License](https://img.shields.io/github/license/aymgal/COOLEST)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05567/status.svg)](https://doi.org/10.21105/joss.05567)
 
 ## What is COOLEST?
```

### Comparing `coolest-0.1.3/coolest.egg-info/SOURCES.txt` & `coolest-0.1.7/coolest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AUTHORS.md
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 coolest/__init__.py
 coolest.egg-info/PKG-INFO
 coolest.egg-info/SOURCES.txt
 coolest.egg-info/dependency_links.txt
 coolest.egg-info/requires.txt
 coolest.egg-info/top_level.txt
```

### Comparing `coolest-0.1.3/setup.py` & `coolest-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 infopath = os.path.abspath(os.path.join(os.path.dirname(__file__),
                            name, '__init__.py'))
 with open(infopath) as open_file:
     exec(open_file.read(), release_info)
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
     readme = f.read()
 
 # Python version
 python_requires = '>=3.7'
 
 # Required packages
 install_requires = [
@@ -30,25 +29,29 @@
     'matplotlib>=3.7.0',    # for plotting
     'lenstronomy>=1.11.0',  # for shapelets light profiles
     'ipython',              # for running example notebooks
     'ipykernel',            # notebooks in custom environment
     'getdist>=1.3.2',       # for making corner plots
 ]
 
+version = release_info['__version__']
+
 setuptools.setup(
     name=name,
     author=release_info['__author__'],
     author_email=release_info['__email__'],
-    version=release_info['__version__'],
+    version=version,
     url=release_info['__url__'],
+    download_url=f"https://github.com/aymgal/coolest/archive/refs/tags/v{version}.tar.gz",
     packages=setuptools.find_packages(),
     license=release_info['__license__'],
-    description=release_info['__about__'],
-    long_description=long_description,
+    description=release_info['__description__'],
+    long_description=readme,
     long_description_content_type='text/markdown',
+    keywords=["coolest", "lensing", "gravitation", "astrophysics"],
 
     python_requires=python_requires,
     install_requires=install_requires,
 
     extras_require={
         "opt": install_optional,  # installable via `pip install coolest[opt]`
     },
```

