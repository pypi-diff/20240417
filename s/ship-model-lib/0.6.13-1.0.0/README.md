# Comparing `tmp/ship_model_lib-0.6.13.tar.gz` & `tmp/ship_model_lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ship_model_lib-0.6.13.tar", last modified: Mon Mar 11 07:55:12 2024, max compression
+gzip compressed data, was "ship_model_lib-1.0.0.tar", last modified: Wed Apr 17 06:38:50 2024, max compression
```

## Comparing `ship_model_lib-0.6.13.tar` & `ship_model_lib-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.589484 ship_model_lib-0.6.13/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/dependencies/B_series_coefficients.npy
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/dependencies/Re_correction.npy
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.589484 ship_model_lib-0.6.13/ship_model_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60358 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    45207 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/added_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    30007 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/calm_water_resistance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/ship_model_lib/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/data/create_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/data/drag_coefficient.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/propulsor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/ship_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/ship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/ship_model_lib/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/ship_model_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 07:55:12.000000 ship_model_lib-0.6.13/ship_model_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:55:12.593484 ship_model_lib-0.6.13/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    33659 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/tests/test_added_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/tests/test_machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/tests/test_propulsor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-03-11 07:55:07.000000 ship_model_lib-0.6.13/tests/test_ship_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.350578 ship_model_lib-1.0.0/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/dependencies/B_series_coefficients.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/dependencies/Re_correction.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.354578 ship_model_lib-1.0.0/ship_model_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63365 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45217 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/added_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30021 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/calm_water_resistance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.354578 ship_model_lib-1.0.0/ship_model_lib/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/drag_coefficient.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/operation_profile_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/propulsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/ship_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19887 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/ship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/ship_model_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33659 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_added_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_propulsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_ship_model.py
```

### Comparing `ship_model_lib-0.6.13/LICENSE` & `ship_model_lib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/PKG-INFO` & `ship_model_lib-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ship_model_lib
-Version: 0.6.13
+Version: 1.0.0
 Summary: Model library for the hydrodynamics, energy system and fuel calculation
 Home-page: https://github.com/developer/https://github.com/SINTEF/shipdesignlab/
 Author: SINTEF Ocean
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: Ship Energy Model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ship_model_lib-0.6.13/dependencies/B_series_coefficients.npy` & `ship_model_lib-1.0.0/dependencies/B_series_coefficients.npy`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/settings.ini` & `ship_model_lib-1.0.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = ship_model_lib
 min_python = 3.10
 # x-release-please-start-version
-version = 0.6.13
+version = 1.0.0
 # x-release-please-end
 
 ### OPTIONAL ###
 
 requirements = pandas>=2.0.0 pandas<3 scipy>=1.11.0 scipy<2 operation_profile_lib~=0.1.11 matplotlib~=3.8.2 plotly~=5.13.0
 # dev_requirements =
 # console_scripts =
```

### Comparing `ship_model_lib-0.6.13/setup.py` & `ship_model_lib-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/_modidx.py` & `ship_model_lib-1.0.0/ship_model_lib/_modidx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Autogenerated by nbdev
 
 d = {
     "settings": {
-        "branch": "master",
+        "branch": "main",
         "doc_baseurl": "/ship_model_lib/",
         "doc_host": "https://developer.github.io",
-        "git_url": "https://github.com/developer/https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/DesignLab/_git/ship_model_lib/",
+        "git_url": "https://github.com/developer/https://github.com/SINTEF/shipdesignlab/",
         "lib_path": "ship_model_lib",
     },
     "syms": {
         "ship_model_lib.added_resistance": {
             "ship_model_lib.added_resistance.AddedResistance": (
                 "addedresistance.html#addedresistance",
                 "ship_model_lib/added_resistance.py",
@@ -712,14 +712,68 @@
                 "ship_model_lib/machinery.py",
             ),
             "ship_model_lib.machinery.PowerSourceWithSpecificFuelConsumption.get_specific_fuel_consumption_g_per_kwh": (
                 "machinery.html#powersourcewithspecificfuelconsumption.get_specific_fuel_consumption_g_per_kwh",
                 "ship_model_lib/machinery.py",
             ),
         },
+        "ship_model_lib.operation_profile_structure": {
+            "ship_model_lib.operation_profile_structure.Location": (
+                "operation_profile_structure.html#location",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Location.__init__": (
+                "operation_profile_structure.html#location.__init__",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Location.to_dict": (
+                "operation_profile_structure.html#location.to_dict",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Location.to_dict_scalar": (
+                "operation_profile_structure.html#location.to_dict_scalar",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.OperationPoint": (
+                "operation_profile_structure.html#operationpoint",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.OperationPoint.__init__": (
+                "operation_profile_structure.html#operationpoint.__init__",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.OperationPoint.to_dict": (
+                "operation_profile_structure.html#operationpoint.to_dict",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.OperationPoint.to_dict_scalar": (
+                "operation_profile_structure.html#operationpoint.to_dict_scalar",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Weather": (
+                "operation_profile_structure.html#weather",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Weather.__init__": (
+                "operation_profile_structure.html#weather.__init__",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Weather.get_weather_at_index": (
+                "operation_profile_structure.html#weather.get_weather_at_index",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Weather.to_dict": (
+                "operation_profile_structure.html#weather.to_dict",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+            "ship_model_lib.operation_profile_structure.Weather.to_dict_scalar": (
+                "operation_profile_structure.html#weather.to_dict_scalar",
+                "ship_model_lib/operation_profile_structure.py",
+            ),
+        },
         "ship_model_lib.propulsor": {
             "ship_model_lib.propulsor.OpenWaterPropellerCurvePoint": (
                 "propulsor.html#openwaterpropellercurvepoint",
                 "ship_model_lib/propulsor.py",
             ),
             "ship_model_lib.propulsor.Propulsor": (
                 "propulsor.html#propulsor",
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib/added_resistance.py` & `ship_model_lib-1.0.0/ship_model_lib/added_resistance.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Callable, Union, TypeVar, Tuple
 
 import pandas as pd
-from operation_profile_lib.operation_profile_structure import Weather
+from .operation_profile_structure import Weather
 from scipy import interpolate
 from scipy.special import jv, yv
 from scipy.integrate import quad, dblquad, simpson
 from scipy.special import gamma
 
 from .types import WaveSpectrumType, ShipType
-from .utility import get_interpolation_1d_function, Interpolated1DValue, kn_to_m_per_s
+from ship_model_lib.utility import (
+    get_interpolation_1d_function,
+    Interpolated1DValue,
+    kn_to_m_per_s,
+)
 from .ship_dimensions import ShipDimensionsAddedResistance
 import numpy as np
 
 # %% ../01_AddedResistance.ipynb 7
 Numeric = TypeVar("Numeric", float, np.ndarray)
 
 # Define logger
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib/calm_water_resistance.py` & `ship_model_lib-1.0.0/ship_model_lib/calm_water_resistance.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 # %% ../00_CalmWaterResistance.ipynb 10
 from typing import Optional
 from abc import ABC, abstractmethod
 from typing import List, Tuple, Union
 from enum import Enum
 
 # from mes_util.constants import KINEMATIC_VISCOSITY_WATER
-from .ship_dimensions import (
+from ship_model_lib.ship_dimensions import (
     ShipDimensionsHollenbachSingleScrew,
     ShipDimensionsHollenbachTwinScrew,
 )
 import numpy as np
 from scipy.optimize import root_scalar
 
 GRAVITY = 9.81
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib/data/create_table.py` & `ship_model_lib-1.0.0/ship_model_lib/data/create_table.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/data/drag_coefficient.csv` & `ship_model_lib-1.0.0/ship_model_lib/data/drag_coefficient.csv`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/machinery.py` & `ship_model_lib-1.0.0/ship_model_lib/machinery.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Optional, Union, Callable, List, TypeVar, NamedTuple
 import numpy as np
 from plotly.subplots import make_subplots
 from plotly.graph_objs import Figure as PlotlyFigure
-from ship_model_lib.utility import get_interpolation_1d_function, Interpolated1DValue
+from .utility import get_interpolation_1d_function, Interpolated1DValue
 from .types import PropulsionType, EmissionType
 
 Numeric = TypeVar("Numeric", np.ndarray, float)
 
 
 @dataclass
 class Point:
@@ -90,14 +90,15 @@
     _CO2_HFO: float = 3.11
     _CO2_NG: float = 2.75
     _CO2_Hydrogen: float = 0.0
     _CO2_Ammonia: float = 0.0
     _CO2_LPG: float = 3.01
     _CO2_MGO: float = 3.15
     _CO2_Methanol = 1.37
+
     # kg CO2 / kg fuel from engineeringtoolbox.com
 
     def __post_init__(self):
         total_fraction = sum(
             [
                 getattr(self, fuel_type)
                 for fuel_type in self.__dict__
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib/propulsor.py` & `ship_model_lib-1.0.0/ship_model_lib/propulsor.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/ship_dimensions.py` & `ship_model_lib-1.0.0/ship_model_lib/ship_dimensions.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/ship_model.py` & `ship_model_lib-1.0.0/ship_model_lib/ship_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from ship_model_lib.added_resistance import (
     WaveSpectrumType,
     AddedResistanceByStaWave2,
     AddedResistanceBySeaMarginCurve,
     AddedResistanceBySNNM,
     AddedResistanceWindITTC,
 )
-from operation_profile_lib.operation_profile_structure import Weather, OperationPoint
+from .operation_profile_structure import Weather, OperationPoint
 from .utility import kn_to_m_per_s, m_per_s_to_kn, Interpolated1DValue
 from ship_model_lib.machinery import (
     Point,
     Curve,
     EmissionType,
     EmissionFactor,
     FuelByMassFraction,
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib/types.py` & `ship_model_lib-1.0.0/ship_model_lib/types.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib/utility.py` & `ship_model_lib-1.0.0/ship_model_lib/utility.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/ship_model_lib.egg-info/PKG-INFO` & `ship_model_lib-1.0.0/ship_model_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ship_model_lib
-Version: 0.6.13
+Version: 1.0.0
 Summary: Model library for the hydrodynamics, energy system and fuel calculation
 Home-page: https://github.com/developer/https://github.com/SINTEF/shipdesignlab/
 Author: SINTEF Ocean
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: Ship Energy Model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ship_model_lib-0.6.13/ship_model_lib.egg-info/SOURCES.txt` & `ship_model_lib-1.0.0/ship_model_lib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dependencies/B_series_coefficients.npy
 dependencies/Re_correction.npy
 ship_model_lib/__init__.py
 ship_model_lib/_modidx.py
 ship_model_lib/added_resistance.py
 ship_model_lib/calm_water_resistance.py
 ship_model_lib/machinery.py
+ship_model_lib/operation_profile_structure.py
 ship_model_lib/propulsor.py
 ship_model_lib/ship_dimensions.py
 ship_model_lib/ship_model.py
 ship_model_lib/types.py
 ship_model_lib/utility.py
 ship_model_lib.egg-info/PKG-INFO
 ship_model_lib.egg-info/SOURCES.txt
```

### Comparing `ship_model_lib-0.6.13/tests/test_added_resistance.py` & `ship_model_lib-1.0.0/tests/test_added_resistance.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/tests/test_machinery.py` & `ship_model_lib-1.0.0/tests/test_machinery.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/tests/test_propulsor.py` & `ship_model_lib-1.0.0/tests/test_propulsor.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-0.6.13/tests/test_ship_model.py` & `ship_model_lib-1.0.0/tests/test_ship_model.py`

 * *Files identical despite different names*

