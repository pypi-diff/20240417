# Comparing `tmp/emmet-api-0.82.1.tar.gz` & `tmp/emmet-api-0.82.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.82.1.tar", last modified: Wed Apr  3 16:51:24 2024, max compression
+gzip compressed data, was "emmet-api-0.82.2.tar", last modified: Wed Apr 17 00:47:46 2024, max compression
```

## Comparing `emmet-api-0.82.1.tar` & `emmet-api-0.82.2.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 16:51:19.000000 emmet-api-0.82.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 16:51:24.985550 emmet-api-0.82.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 16:51:19.000000 emmet-api-0.82.1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.945550 emmet-api-0.82.1/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.957550 emmet-api-0.82.1/emmet/api/routes/materials/conversion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/conversion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/conversion_electrodes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.961550 emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.965550 emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.969550 emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 16:51:19.000000 emmet-api-0.82.1/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.973550 emmet-api-0.82.1/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 16:51:24.000000 emmet-api-0.82.1/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-04-03 16:51:19.000000 emmet-api-0.82.1/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-03 16:51:19.000000 emmet-api-0.82.1/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-03 16:51:19.000000 emmet-api-0.82.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:51:24.989549 emmet-api-0.82.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-03 16:51:19.000000 emmet-api-0.82.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 16:51:19.000000 emmet-api-0.82.1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.949550 emmet-api-0.82.1/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.953550 emmet-api-0.82.1/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.977550 emmet-api-0.82.1/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.981550 emmet-api-0.82.1/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:24.985550 emmet-api-0.82.1/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 16:51:19.000000 emmet-api-0.82.1/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-17 00:47:41.000000 emmet-api-0.82.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-17 00:47:46.729479 emmet-api-0.82.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 00:47:41.000000 emmet-api-0.82.2/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.685479 emmet-api-0.82.2/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.693479 emmet-api-0.82.2/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.693479 emmet-api-0.82.2/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.693479 emmet-api-0.82.2/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.697479 emmet-api-0.82.2/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/conversion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/conversion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/conversion_electrodes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.701479 emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.705479 emmet-api-0.82.2/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.709479 emmet-api-0.82.2/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.713479 emmet-api-0.82.2/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-17 00:47:41.000000 emmet-api-0.82.2/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 00:47:46.000000 emmet-api-0.82.2/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-04-17 00:47:41.000000 emmet-api-0.82.2/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-17 00:47:41.000000 emmet-api-0.82.2/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-17 00:47:41.000000 emmet-api-0.82.2/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:47:46.729479 emmet-api-0.82.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-17 00:47:41.000000 emmet-api-0.82.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-17 00:47:41.000000 emmet-api-0.82.2/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.717479 emmet-api-0.82.2/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.689479 emmet-api-0.82.2/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.693479 emmet-api-0.82.2/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.721479 emmet-api-0.82.2/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.725479 emmet-api-0.82.2/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:46.729479 emmet-api-0.82.2/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 00:47:41.000000 emmet-api-0.82.2/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.82.1/Dockerfile` & `emmet-api-0.82.2/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-FROM materialsproject/devops:python-3.1010.24 as base
+FROM materialsproject/devops:python-3.1013.8 as base
 RUN apt-get update && apt-get install -y --no-install-recommends libopenblas-dev libjpeg62 && apt-get clean
 
 FROM base as builder
 RUN apt-get update && apt-get install -y --no-install-recommends gcc git g++ cmake make libsnappy-dev wget && apt-get clean
 ENV PATH /root/.local/bin:$PATH
 WORKDIR /emmet-api
 ENV PIP_FLAGS "--user --no-cache-dir --compile"
 COPY requirements/deployment.txt ./requirements.txt
 RUN pip install $PIP_FLAGS --upgrade pip pip-tools setuptools-scm && \
-    pip-sync requirements.txt --pip-args "$PIP_FLAGS"
+  pip-sync requirements.txt --pip-args "$PIP_FLAGS"
 
 COPY emmet emmet
 COPY setup.py .
 ARG API_VERSION
 RUN SETUPTOOLS_SCM_PRETEND_VERSION=${API_VERSION} pip install $PIP_FLAGS --no-deps .
 RUN wget -q https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh && \
-    chmod +x wait-for-it.sh && mv wait-for-it.sh /root/.local/bin/
+  chmod +x wait-for-it.sh && mv wait-for-it.sh /root/.local/bin/
 
 FROM base
 COPY --from=builder /root/.local/lib/python3.10/site-packages /root/.local/lib/python3.10/site-packages
 COPY --from=builder /root/.local/bin /root/.local/bin
 COPY --from=builder /usr/lib/x86_64-linux-gnu/libsnappy* /usr/lib/x86_64-linux-gnu/
 COPY --from=builder /emmet-api /emmet-api
 WORKDIR /emmet-api
 ARG VERSION
 ENV PATH=/root/.local/bin:$PATH \
-    PYTHONUNBUFFERED=1 \
-    FLASK_APP=emmet-api \
-    FLASK_ENV=production \
-    PORT=10001 \
-    NUM_WORKERS=4 \
-    RELOAD="" \
-    MAX_REQUESTS=0 \
-    MAX_REQUESTS_JITTER=0 \
-    DD_TRACE_HOST=localhost:8126 \
-    DD_SERVICE=next-gen-api \
-    DD_ENV=prod \
-    DD_VERSION=$VERSION
+  PYTHONUNBUFFERED=1 \
+  FLASK_APP=emmet-api \
+  FLASK_ENV=production \
+  PORT=10001 \
+  NUM_WORKERS=4 \
+  RELOAD="" \
+  MAX_REQUESTS=0 \
+  MAX_REQUESTS_JITTER=0 \
+  DD_TRACE_HOST=localhost:8126 \
+  DD_SERVICE=next-gen-api \
+  DD_ENV=prod \
+  DD_VERSION=$VERSION
 
 COPY app.py .
 COPY material_resources.py .
 COPY molecule_resources.py .
 COPY start.sh .
 RUN chmod +x start.sh
 
 LABEL com.datadoghq.ad.logs='[{"source": "gunicorn", "service": "next-gen-api"}]'
 
 EXPOSE 10001 20001
-CMD wait-for-it.sh $DD_TRACE_HOST -q -s -t 60 -- ./start.sh
+CMD ./start.sh
```

### Comparing `emmet-api-0.82.1/app.py` & `emmet-api-0.82.2/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/api.py` & `emmet-api-0.82.2/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.82.2/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.82.2/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/documentation.py` & `emmet-api-0.82.2/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/global_header.py` & `emmet-api-0.82.2/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/core/settings.py` & `emmet-api-0.82.2/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.82.2/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.82.2/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.82.2/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.82.2/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.82.2/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/_messages/resources.py` & `emmet-api-0.82.2/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/dois/resources.py` & `emmet-api-0.82.2/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.82.2/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/conversion_electrodes/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/conversion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/insertion_electrodes/utils.py` & `emmet-api-0.82.2/emmet/api/routes/materials/insertion_electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.82.2/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.82.2/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.82.2/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.82.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.82.2/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.82.2/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.82.2/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.82.2/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/utils.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.82.2/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.82.2/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/material_resources.py` & `emmet-api-0.82.2/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/molecule_resources.py` & `emmet-api-0.82.2/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/requirements/deployment.txt` & `emmet-api-0.82.2/requirements/deployment.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,75 +53,75 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (emmet/emmet-api/setup.py)
 envier==0.5.1
     # via ddtrace
 exceptiongroup==1.2.0
     # via
     #   anyio
     #   cattrs
 fastapi==0.110.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 gunicorn==21.2.0
     # via emmet-api (emmet/emmet-api/setup.py)
 h11==0.14.0
     # via uvicorn
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via opentelemetry-api
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   -r python/requirements.txt
     #   pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
@@ -130,40 +130,40 @@
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 numpy==1.26.4
     # via
     #   -r python/requirements.txt
     #   contourpy
     #   maggma
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   -r python/requirements.txt
     #   pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
@@ -173,29 +173,29 @@
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (emmet/emmet-api/setup.py)
 pymongo==4.6.3
     # via
@@ -213,37 +213,37 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   -r python/requirements.txt
     #   pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (emmet/emmet-api/setup.py)
@@ -255,17 +255,17 @@
     # via
     #   ddsketch
     #   ddtrace
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
@@ -273,15 +273,15 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   anyio
     #   asgiref
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,114 +53,114 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
 exceptiongroup==1.2.0
     # via
     #   anyio
     #   cattrs
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via opentelemetry-api
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2024.3.31
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.20.0
     # via pymatgen
@@ -168,29 +168,29 @@
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymongo==4.6.3
     # via
@@ -208,37 +208,37 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -248,17 +248,17 @@
     # via
     #   ddsketch
     #   ddtrace
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
@@ -266,15 +266,15 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   anyio
     #   asgiref
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -65,95 +65,104 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
 exceptiongroup==1.2.0
     # via
     #   anyio
     #   cattrs
     #   pytest
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.3
+filelock==3.13.4
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.42.2
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==6.4.0
+    # via
+    #   matplotlib
+    #   spglib
 iniconfig==2.0.0
     # via pytest
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via
     #   emmet-api (setup.py)
     #   flask
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -161,15 +170,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.5.3
     # via
@@ -190,15 +199,15 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.2
+mkdocstrings[python]==0.24.3
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.9.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
@@ -233,27 +242,27 @@
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
@@ -276,35 +285,35 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.7.1
     # via
@@ -341,37 +350,37 @@
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -384,17 +393,17 @@
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
@@ -409,40 +418,45 @@
     #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-types-requests==2.31.0.20240402
+types-requests==2.31.0.6
     # via emmet-api (setup.py)
-types-setuptools==69.2.0.20240317
+types-setuptools==69.5.0.20240415
     # via emmet-api (setup.py)
-typing-extensions==4.10.0
+types-urllib3==1.26.25.14
+    # via types-requests
+typing-extensions==4.11.0
     # via
+    #   aioitertools
     #   anyio
     #   asgiref
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
+    #   mkdocstrings
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
+    #   starlette
     #   uvicorn
 tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==2.2.1
+urllib3==1.26.18
     # via
     #   botocore
     #   requests
-    #   types-requests
 uvicorn==0.29.0
     # via maggma
 virtualenv==20.25.1
     # via pre-commit
 watchdog==4.0.0
     # via mkdocs
 wcmatch==8.5.1
@@ -452,11 +466,13 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.18.1
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,110 +53,110 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via opentelemetry-api
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2024.3.31
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.20.0
     # via pymatgen
@@ -164,29 +164,29 @@
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymongo==4.6.3
     # via
@@ -204,37 +204,37 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -244,17 +244,17 @@
     # via
     #   ddsketch
     #   ddtrace
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
@@ -262,15 +262,15 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   pydantic
     #   pydantic-core
     #   pydash
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -65,90 +65,95 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
+exceptiongroup==1.2.0
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.3
+filelock==3.13.4
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.42.2
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via opentelemetry-api
 iniconfig==2.0.0
     # via pytest
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via
     #   emmet-api (setup.py)
     #   flask
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -156,15 +161,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.5.3
     # via
@@ -185,15 +190,15 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.2
+mkdocstrings[python]==0.24.3
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.9.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
@@ -212,15 +217,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
@@ -228,27 +233,27 @@
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
@@ -271,35 +276,35 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.7.1
     # via
@@ -336,37 +341,37 @@
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -379,47 +384,56 @@
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-types-requests==2.31.0.20240402
+types-requests==2.31.0.20240406
     # via emmet-api (setup.py)
-types-setuptools==69.2.0.20240317
+types-setuptools==69.5.0.20240415
     # via emmet-api (setup.py)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
+    #   anyio
+    #   asgiref
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
+    #   uvicorn
 tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==2.2.1
     # via
     #   botocore
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.9.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,79 +53,81 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
 exceptiongroup==1.2.0
     # via
     #   anyio
     #   cattrs
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==6.4.0
-    # via matplotlib
-itsdangerous==2.1.2
+    # via
+    #   matplotlib
+    #   spglib
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2024.3.31
     # via
@@ -146,25 +148,25 @@
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.20.0
     # via pymatgen
@@ -172,29 +174,29 @@
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymongo==4.6.3
     # via
@@ -212,37 +214,37 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -252,17 +254,17 @@
     # via
     #   ddsketch
     #   ddtrace
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
@@ -270,15 +272,15 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   aioitertools
     #   anyio
     #   asgiref
     #   bytecode
     #   cattrs
     #   ddtrace
```

### Comparing `emmet-api-0.82.1/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.82.2/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
@@ -20,19 +20,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
 blinker==1.7.0
     # via flask
-boto3==1.34.76
+boto3==1.34.85
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.76
+botocore==1.34.85
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -65,102 +65,90 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.7.5
+ddtrace==2.8.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.0
+emmet-core==0.82.1
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.0
-    # via
-    #   anyio
-    #   cattrs
-    #   pytest
 fastapi==0.110.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.3
+filelock==3.13.4
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
-flask==3.0.2
+flask==3.0.3
     # via mongogrant
-fonttools==4.50.0
+fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.42.2
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==6.4.0
-    # via matplotlib
+    # via opentelemetry-api
 iniconfig==2.0.0
     # via pytest
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via
     #   emmet-api (setup.py)
     #   flask
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
 jsonschema==4.21.1
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.0
+maggma==0.64.1
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -168,15 +156,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.5.3
     # via
@@ -197,15 +185,15 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.2
+mkdocstrings[python]==0.24.3
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.9.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
@@ -224,15 +212,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
@@ -240,27 +228,27 @@
     #   pandas
     #   pymatgen
     #   scipy
     #   shapely
     #   spglib
 opentelemetry-api==1.24.0
     # via ddtrace
-orjson==3.10.0
+orjson==3.10.1
     # via maggma
 packaging==24.0
     # via
     #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.1
+pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
@@ -283,35 +271,35 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
 pydash==8.0.0
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
-pymatgen==2024.3.1
+pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.7.1
     # via
@@ -348,37 +336,37 @@
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==25.1.2
+pyzmq==26.0.0
     # via maggma
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.17.40
+ruamel-yaml==0.18.6
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.3
     # via
@@ -391,70 +379,56 @@
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
-spglib==2.3.1
+spglib==2.4.0
     # via pymatgen
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via ddtrace
 sshtunnel==0.4.0
     # via maggma
 starlette==0.37.2
     # via fastapi
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-types-requests==2.31.0.6
+types-requests==2.31.0.20240406
     # via emmet-api (setup.py)
-types-setuptools==69.2.0.20240317
+types-setuptools==69.5.0.20240415
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.14
-    # via types-requests
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
-    #   aioitertools
-    #   anyio
-    #   asgiref
-    #   bytecode
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
-    #   mkdocstrings
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
-    #   starlette
-    #   uvicorn
 tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
+    #   types-requests
 uvicorn==0.29.0
     # via maggma
 virtualenv==20.25.1
     # via pre-commit
 watchdog==4.0.0
     # via mkdocs
 wcmatch==8.5.1
@@ -464,13 +438,11 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.18.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.82.1/setup.py` & `emmet-api-0.82.2/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/_consumer/test_query_operators.py` & `emmet-api-0.82.2/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/_general_store/test_query_operators.py` & `emmet-api-0.82.2/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/core/test_mapi.py` & `emmet-api-0.82.2/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.82.2/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/electrodes/test_utils.py` & `emmet-api-0.82.2/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/materials/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/materials/test_utils.py` & `emmet-api-0.82.2/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/summary/test_hint_scheme.py` & `emmet-api-0.82.2/tests/materials/summary/test_hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/summary/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.82.2/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.82.2/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/synthesis/test_utils.py` & `emmet-api-0.82.2/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/tasks/test_utils.py` & `emmet-api-0.82.2/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/materials/xas/test_query_operators.py` & `emmet-api-0.82.2/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/tasks/test_utils.py` & `emmet-api-0.82.2/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.82.1/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.82.2/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

