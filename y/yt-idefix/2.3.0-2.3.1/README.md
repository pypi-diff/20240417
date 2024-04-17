# Comparing `tmp/yt_idefix-2.3.0.tar.gz` & `tmp/yt_idefix-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.3.0.tar", last modified: Sat Jul 15 16:54:22 2023, max compression
+gzip compressed data, was "yt_idefix-2.3.1.tar", last modified: Wed Apr 17 08:32:45 2024, max compression
```

## Comparing `yt_idefix-2.3.0.tar` & `yt_idefix-2.3.1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.630823 yt_idefix-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34819 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.146507 yt_idefix-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.150507 yt_idefix-2.3.1/src/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/src/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:33.000000 yt_idefix-2.3.1/src/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/src/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 08:32:45.000000 yt_idefix-2.3.1/src/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:32:45.154507 yt_idefix-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 08:32:36.000000 yt_idefix-2.3.1/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-17 08:32:36.000000 yt_idefix-2.3.1/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 08:32:36.000000 yt_idefix-2.3.1/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-17 08:32:36.000000 yt_idefix-2.3.1/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 08:32:36.000000 yt_idefix-2.3.1/tests/test_xdmf.py
```

### Comparing `yt_idefix-2.3.0/LICENSE` & `yt_idefix-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/PKG-INFO` & `yt_idefix-2.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.3.0
+Version: 2.3.1
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -14,34 +14,36 @@
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: HDF5
 License-File: LICENSE
+Requires-Dist: inifix>=4.1.0
+Requires-Dist: numpy>=1.19.3
+Requires-Dist: yt>=4.2.0
+Requires-Dist: typing-extensions>=4.4.0; python_version < "3.12"
+Provides-Extra: hdf5
+Requires-Dist: h5py>=3.1.0; extra == "hdf5"
 
 
 # yt_idefix
 [![PyPI](https://img.shields.io/pypi/v/yt-idefix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/yt_idefix/)
-[![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
@@ -63,63 +65,76 @@
 compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
-Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
-
 ```python
-# Examples
 ds = yt.load(
-    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+    "data.0010.vtk",
+    definitions_header="../definitions.h",
+    inifile="example.ini",
 )
-ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
-The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
+Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
-Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
+```python
+ds = yt.load("data.0010.vtk", geometry="spherical")
+```
 
+The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. Data is always interpreted as dimensionful.
+For Pluto simulation, metadata is retrieved from `definitions.h` and `pluto.ini` to guess the proper on-disk units automatically.
+
+Units may also be provided at runtime using the `units_override` argument
 ```python
-# Examples on units
-ds = yt.load("data.0010.vtk", unit_system="mks")
+ds = yt.load(
+    "data.0010.vtk",
+    units_override={
+        "length_unit": (100.0, "au"),
+        "mass_unit": yt.units.mass_sun,
+    },
+)
+```
+Note that other units will also be changed for consistency (Pluto).
 
-units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
+Displayed units can also be controled using the `unit_system` argument.
+Accepted values are `"cgs"` (default), `"mks"` and `"code"`.
 
-# Caution that other units will also be changed for consistency!
-ds = yt.load("data.0010.vtk", unit_override=unit_override)
+```python
+ds = yt.load("data.0010.vtk", unit_system="mks")
 ```
-With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
+
+With Pluto data, units not specified with `units_override` will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
 
 ```python
 {"magnetic_unit", "velocity_unit", "density_unit"},
 {"velocity_unit", "time_unit", "length_unit"},
-{"density_unit", "length_unit", "mass_unit"},
+{"density_unit", "length_unit", "mass_unit"}
 ```
 
 yt is able to provide some derived fields from existed fields, e.g., `"cell_volume"`. Fields related to element species can be created according to primordial abundances of H and He, through `default_species_fields` (`"neutral"` and `"ionized"`) parameters.
 
 ```python
-# Example
 ds = yt.load("data.0010.vtk", default_species_fields="ionized")
 ```
 
-### Convention of field names
-The outputs are loaded from disk with field names in uppercase. This normalization is only applied to the standard outputs but user-defined outputs and Pluto's ion fraction outputs.
+### Conventions on field names
+
+Field names of on-disk fields for density, pressure, velocity and magnetic field components are always normalized to upper case, even if Pluto may use lowercase in some versions.
 
 ```python
-# Example
-ds.field_list
-# Output:
-# [('pluto-vtk', 'PRS'),   # standard output
-#  ('pluto-vtk', 'RHO'),   # standard output
-#  ('pluto-vtk', 'VX1'),   # standard output
-#  ('pluto-vtk', 'VX2'),   # standard output
-#  ('pluto-vtk', 'VX3'),   # standard output
-#  ('pluto-vtk', 'temp')]  # This is a user-defined output
+>>> ds.field_list
+[('pluto-vtk', 'PRS'),
+ ('pluto-vtk', 'RHO'),
+ ('pluto-vtk', 'VX1'),
+ ('pluto-vtk', 'VX2'),
+ ('pluto-vtk', 'VX3')]
 ```
+
+This normalization is only applied to non-user-defined outputs and Pluto's ion
+fraction outputs.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_idefix-2.3.0/README.md` & `yt_idefix-2.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 
 # yt_idefix
 [![PyPI](https://img.shields.io/pypi/v/yt-idefix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/yt_idefix/)
-[![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
@@ -33,63 +31,76 @@
 compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
-Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
-
 ```python
-# Examples
 ds = yt.load(
-    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+    "data.0010.vtk",
+    definitions_header="../definitions.h",
+    inifile="example.ini",
 )
-ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
-The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
+Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
-Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
+```python
+ds = yt.load("data.0010.vtk", geometry="spherical")
+```
 
+The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. Data is always interpreted as dimensionful.
+For Pluto simulation, metadata is retrieved from `definitions.h` and `pluto.ini` to guess the proper on-disk units automatically.
+
+Units may also be provided at runtime using the `units_override` argument
 ```python
-# Examples on units
-ds = yt.load("data.0010.vtk", unit_system="mks")
+ds = yt.load(
+    "data.0010.vtk",
+    units_override={
+        "length_unit": (100.0, "au"),
+        "mass_unit": yt.units.mass_sun,
+    },
+)
+```
+Note that other units will also be changed for consistency (Pluto).
 
-units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
+Displayed units can also be controled using the `unit_system` argument.
+Accepted values are `"cgs"` (default), `"mks"` and `"code"`.
 
-# Caution that other units will also be changed for consistency!
-ds = yt.load("data.0010.vtk", unit_override=unit_override)
+```python
+ds = yt.load("data.0010.vtk", unit_system="mks")
 ```
-With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
+
+With Pluto data, units not specified with `units_override` will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
 
 ```python
 {"magnetic_unit", "velocity_unit", "density_unit"},
 {"velocity_unit", "time_unit", "length_unit"},
-{"density_unit", "length_unit", "mass_unit"},
+{"density_unit", "length_unit", "mass_unit"}
 ```
 
 yt is able to provide some derived fields from existed fields, e.g., `"cell_volume"`. Fields related to element species can be created according to primordial abundances of H and He, through `default_species_fields` (`"neutral"` and `"ionized"`) parameters.
 
 ```python
-# Example
 ds = yt.load("data.0010.vtk", default_species_fields="ionized")
 ```
 
-### Convention of field names
-The outputs are loaded from disk with field names in uppercase. This normalization is only applied to the standard outputs but user-defined outputs and Pluto's ion fraction outputs.
+### Conventions on field names
+
+Field names of on-disk fields for density, pressure, velocity and magnetic field components are always normalized to upper case, even if Pluto may use lowercase in some versions.
 
 ```python
-# Example
-ds.field_list
-# Output:
-# [('pluto-vtk', 'PRS'),   # standard output
-#  ('pluto-vtk', 'RHO'),   # standard output
-#  ('pluto-vtk', 'VX1'),   # standard output
-#  ('pluto-vtk', 'VX2'),   # standard output
-#  ('pluto-vtk', 'VX3'),   # standard output
-#  ('pluto-vtk', 'temp')]  # This is a user-defined output
+>>> ds.field_list
+[('pluto-vtk', 'PRS'),
+ ('pluto-vtk', 'RHO'),
+ ('pluto-vtk', 'VX1'),
+ ('pluto-vtk', 'VX2'),
+ ('pluto-vtk', 'VX3')]
 ```
+
+This normalization is only applied to non-user-defined outputs and Pluto's ion
+fraction outputs.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_idefix-2.3.0/pyproject.toml` & `yt_idefix-2.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,28 @@
     "Framework :: Matplotlib",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: AIX",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Typing :: Typed",
 ]
 keywords = [
     "astronomy astrophysics visualization amr adaptivemeshrefinement",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "inifix>=4.1.0",
-    "numpy>=1.17.3",
+    "numpy>=1.19.3",
     "yt>=4.2.0",
-    "typing-extensions>=4.1.0 ; python_version < '3.11'"
+    "typing-extensions>=4.4.0 ; python_version < '3.12'"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "yt_idefix.__version__"}
 
 [project.optional-dependencies]
@@ -74,15 +73,15 @@
     "py.typed",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
-[tool.ruff]
+[tool.ruff.lint]
 exclude = [
     "*/api.py",
     "*/__init__.py",
 ]
 select = [
     "E",
     "F",
@@ -95,29 +94,32 @@
     "UP",   # pyupgrade
     "I",    # isort
 ]
 ignore = [
     "E501",  # line too long
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 known-third-party = [
   "numpy",
   "matplotlib",
   "unyt",
   "yaml",
   "pytest",
 ]
 known-first-party = ["yt", "yt_idefix"]
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.9
 show_error_codes = true
 warn_unused_configs = true
 warn_unreachable = true
 show_error_context = true
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
+    # already patched (but not released) upstream:
+    # https://github.com/dateutil/dateutil/pull/1285
+    'ignore:datetime\.datetime\.utcfromtimestamp\(\) is deprecated:DeprecationWarning',
 ]
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/_io/commons.py` & `yt_idefix-2.3.1/src/yt_idefix/_io/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Literal, NamedTuple, Tuple
+from typing import Any, Literal, NamedTuple
 
 import numpy as np
 
 Prec = Literal["d", "f", "i", "?"]
 Dim = Literal[1, 2, 3]
 
 
@@ -96,11 +96,11 @@
         )
     return coords
 
 
 # map field name to numpy array init data:
 # precision (-> datatype), dimensionality, [nx, ny, nz]
 # the np.ndarray is assumed to contain *dim* elements
-IdefixFieldProperties = Dict[str, Tuple[Prec, Dim, np.ndarray]]
+IdefixFieldProperties = dict[str, tuple[Prec, Dim, np.ndarray]]
 
 # Map various str keys to scalars and arrays
-IdefixMetadata = Dict[str, Any]
+IdefixMetadata = dict[str, Any]
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.3.1/src/yt_idefix/_io/dmp_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,58 +112,54 @@
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: bool,
     skip_data: Literal[True],
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: Literal[True],
     skip_data: Literal[False],
-) -> float:
-    ...
+) -> float: ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: Literal[False],
     skip_data: Literal[False],
-) -> np.ndarray:
-    ...
+) -> np.ndarray: ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: bool,
     skip_data: bool,
-) -> float | np.ndarray | None:
-    ...
+) -> float | np.ndarray | None: ...
 
 
 def read_chunk(
     fh,
     ndim,
     dim,
     dtype,
@@ -201,42 +197,39 @@
     fh: BinaryIO,
     ndim: int,
     dim: np.ndarray,
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: Literal[True],
-) -> float:
-    ...
+) -> float: ...
 
 
 @overload
 def read_serial(
     fh: BinaryIO,
     ndim: int,
     dim: np.ndarray,
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: Literal[False],
-) -> np.ndarray:
-    ...
+) -> np.ndarray: ...
 
 
 @overload
 def read_serial(
     fh: BinaryIO,
     ndim: int,
     dim: np.ndarray,
     dtype: str,
     *,
     byteorder: ByteOrder,
     is_scalar: bool = False,
-) -> float | np.ndarray:
-    ...
+) -> float | np.ndarray: ...
 
 
 def read_serial(fh, ndim, dim, dtype, *, byteorder, is_scalar=False):
     """Emulate Idefix's OutputDump::ReadSerial"""
     assert ndim == 1  # corresponds to an error raised in IDEFIX
     return read_chunk(
         fh,
@@ -253,40 +246,37 @@
 def read_distributed(
     fh: BinaryIO,
     dim: np.ndarray,
     *,
     byteorder: ByteOrder,
     dtype: str,
     skip_data: Literal[False],
-) -> np.ndarray:
-    ...
+) -> np.ndarray: ...
 
 
 @overload
 def read_distributed(
     fh: BinaryIO,
     dim: np.ndarray,
     *,
     byteorder: ByteOrder,
     dtype: str,
     skip_data: Literal[True],
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def read_distributed(
     fh: BinaryIO,
     dim: np.ndarray,
     *,
     byteorder: ByteOrder,
     dtype: str,
     skip_data: bool = False,
-) -> np.ndarray | None:
-    ...
+) -> np.ndarray | None: ...
 
 
 def read_distributed(fh, dim, *, byteorder, dtype, skip_data):
     """Emulate Idefix's OutputDump::ReadDistributed"""
     # note: OutputDump::ReadDistributed only reads doubles
     # because chunks written as integers are small enough
     # that parallelization is counter productive.
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/_io/h5_io.py` & `yt_idefix-2.3.1/src/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/src/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.3.1/src/yt_idefix/_io/vtk_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,25 @@
 @overload
 def read_single_field(
     fh: BinaryIO,
     *,
     shape: tuple[int, int, int],
     offset: int | None = None,
     skip_data: Literal[False],
-) -> np.ndarray:
-    ...
+) -> np.ndarray: ...
 
 
 @overload
 def read_single_field(
     fh: BinaryIO,
     *,
     shape: tuple[int, int, int],
     offset: int | None = None,
     skip_data: Literal[True],
-) -> None:
-    ...
+) -> None: ...
 
 
 def read_single_field(
     fh,
     *,
     shape,
     offset=None,
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/data_structures.py` & `yt_idefix-2.3.1/src/yt_idefix/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
+import sys
 import warnings
 import weakref
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from typing import TYPE_CHECKING, Final, Literal
 
@@ -19,29 +20,33 @@
 from yt.funcs import setdefaultattr
 from yt.geometry.api import Geometry
 from yt.geometry.grid_geometry_handler import GridIndex
 from yt.utilities.lib.misc_utilities import (  # type: ignore [import]
     _obtain_coords_and_widths,
 )
 from yt.utilities.on_demand_imports import _h5py as h5py
-from yt_idefix._backports import removesuffix
 
 from ._io import C_io, dmp_io, h5_io, vtk_io
 from ._io.commons import IdefixFieldProperties, IdefixMetadata
 from .definitions import _PlutoBaseUnits, pluto_def_constants
 from .fields import (
     IdefixDmpFields,
     IdefixVtkFields,
     PlutoFields,
 )
 
 # import IO classes to ensure they are properly registered,
 # even though we don't call them directly
 from .io import IdefixDmpIO, IdefixVtkIO, PlutoVtkIO  # noqa
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 if TYPE_CHECKING:
     # these should really be unyt_array,
     # but mypy doesn't recognize it as a valid type as of unyt 2.9.3 and mypy 0.991
     XSpans = np.ndarray
     YSpans = np.ndarray
     ZSpans = np.ndarray
     XCoords = np.ndarray
@@ -61,44 +66,49 @@
         self.Parent = None
         self.Children = []
         self.Level = level
         self.ActiveDimensions = dims
 
 
 class GoodBoyHierarchy(GridIndex, ABC):
+    _load_requirements = ["inifix"]
     grid = SingleGrid
 
     def __init__(self, ds, dataset_type="idefix"):
         self.dataset_type = dataset_type
         self.dataset = weakref.proxy(ds)
         # for now, the index file is the dataset!
         self.index_filename = self.dataset.filename
         self.directory = os.path.dirname(self.index_filename)
         # float type for the simulation edges and must be float64 now
         self.float_type = np.float64
         super().__init__(ds, dataset_type)
 
+    @override
     def _detect_output_fields(self):
         self.field_list = [
             (self.dataset_type, f) for f in self.dataset._detected_field_list
         ]
 
+    @override
     def _count_grids(self):
         self.num_grids = 1
 
+    @override
     def _parse_index(self):
         self.grid_left_edge[0][:] = self.ds.domain_left_edge[:]
         self.grid_right_edge[0][:] = self.ds.domain_right_edge[:]
         self.grid_dimensions[0][:] = self.ds.domain_dimensions[:]
         self.grid_particle_count[0][0] = 0
 
         # Idefix/Pluto are not AMR
         self.grid_levels[0][0] = 0
         self.min_level = self.max_level = 0
 
+    @override
     def _populate_grid_objects(self):
         # the minimal form of this method is
         #
         # for g in self.grids:
         #     g._prepare_grid()
         #     g._setup_dx()
         #
@@ -133,14 +143,15 @@
     @abstractmethod
     @cached_property
     def _cell_centers(self) -> tuple[XCoords, YCoords, ZCoords]:
         # must return a 3-tuple of 1D unyt_array
         # with unit "code_length" and dtype float64
         ...
 
+    @override
     def _icoords_to_fcoords(
         self,
         icoords: np.ndarray,
         ires: np.ndarray,
         axes: tuple[int, ...] | None = None,
     ):
         if axes is None:
@@ -163,14 +174,15 @@
     def _get_field_offset_index(self) -> dict[str, int]:
         HEADER_SIZE: int = 256
         with open(self.index_filename, "rb") as fh:
             fh.seek(HEADER_SIZE)
             field_index = ...
         return field_index  # type: ignore
 
+    @override
     def _parse_index(self):
         super()._parse_index()
         self._field_offsets = self._get_field_offset_index()
 
 
 class VtkHierarchy(FieldOffsetHierarchy):
     def _get_field_offset_index(self) -> dict[str, int]:
@@ -308,16 +320,16 @@
     Abstract class that defines interfaces common to all concrete dataset classes in this module
     """
 
     # defined in subclasses
     _dataset_type: str
     _default_inifile: str
     _default_definitions_header: str
-    _version_regexp: re.Pattern
 
+    @override
     def __init__(
         self,
         filename,
         *,
         dataset_type: str | None = None,  # deleguated to child classes # NOQA: ARG002
         units_override: dict[str, str] | None = None,
         unit_system: Literal["cgs", "mks", "code"] = "cgs",
@@ -368,14 +380,15 @@
             len(candidates := list(root_dir.glob(f"*{ext}"))) == 1
             and (file := candidates[0]).name == default
         ):
             return str(file.absolute())
         else:
             return ""
 
+    @override
     def _parse_parameter_file(self):
         # base method, intended to be subclassed
         # parse the version hash
         self.parameters["code version"] = self._get_code_version()
 
         # idefix is never cosmological
         self.cosmological_simulation = 0
@@ -442,14 +455,15 @@
         lines = C_io.strip_comments(body).split("\n")
 
         for line in lines:
             if (geom_match := re.fullmatch(_DEF_GEOMETRY_REGEXP, line)) is not None:
                 self.parameters["definitions"]["geometry"] = geom_match.group(1).lower()
                 return
 
+    @override
     def _set_code_unit_attributes(self):
         # This is where quantities are created that represent the various
         # on-disk units.  These are the currently available quantities which
         # should be set, along with examples of how to set them to standard
         # values.
         #
         # self.length_unit = self.quan(1.0, "cm")
@@ -469,46 +483,45 @@
     def _read_data_header(self) -> str:
         pass
 
     def _get_code_version(self) -> str:
         # we assume the version string is somewhere in the first two
         # lines, which is general enough for the data formats we support
         lines = self._read_data_header().splitlines()
-        header = "\n".join(lines[: (min(len(lines), 2))])
-        regexp = self.__class__._version_regexp
-        match = re.search(regexp, header)
+        version_line = [L for L in lines if not L.startswith(("# *", "# vtk"))][0]
+        match = re.search(r"\d+\.\d+\.?\d*[-\w+]*", version_line)
         if match is None:
+            header = "\n".join(lines)
             warnings.warn(
                 f"Could not determine code version from file header {header!r}",
                 stacklevel=2,
             )
             return "unknown"
 
         return match.group()
 
 
 class IdefixDataset(GoodboyDataset, ABC):
     _default_inifile = "idefix.ini"
     _default_definitions_header = "definitions.hpp"
-    _version_regexp = re.compile(r"v\d+\.\d+\.?\d*[-\w+]*")
 
 
 class StaticPlutoDataset(GoodboyDataset, ABC):
     # PlutoDataset is already used as a class name in yt.frontends.chombo
     # the key difference being that, in this extension frontend
     # we only support static grid formats (as opposed to chombo-pluto, which is AMR)
     _default_inifile = "pluto.ini"
     _default_definitions_header = "definitions.h"
     _field_info_class = PlutoFields
-    _version_regexp = re.compile(r"\d+\.\d+\.?\d*[-\w+]*")
 
     @abstractmethod
     def _get_log_file(self) -> str:
         pass
 
+    @override
     def _parse_parameter_file(self):
         super()._parse_parameter_file()
 
         if (match := re.search(r"\.(\d*)\.", self.filename)) is None:
             raise RuntimeError(
                 f"Failed to parse output number from file name {self.filename}"
             )
@@ -530,14 +543,15 @@
             self.current_time = float(match.group(1))
         else:
             ytLogger.warning(
                 "Failed to retrieve time from %s, setting current_time = -1",
                 log_file,
             )
 
+    @override
     def _set_code_unit_attributes(self):
         """Conversion between physical units and code units."""
 
         # Pluto's base units are length, velocity and density, but here we consider
         # length, mass and time as base units. Since it can make us easy to calculate
         # all units when self.units_override is not None.
 
@@ -612,14 +626,15 @@
         "magnetic_unit": "gauss",
         "temperature_unit": "K",
         # this is the one difference with Dataset.default_units:
         # we accept density_unit as a valid override
         "density_unit": "g/cm**3",
     }
 
+    @override
     def _parse_definitions_header(self) -> None:
         """Read some metadata from header file 'definitions.h'."""
         self.parameters["definitions"] = {}
         if not self._definitions_header:
             ytLogger.warning(
                 "%s was not found. Code units will be set to 1.0 in cgs.",
                 self._default_definitions_header,
@@ -674,14 +689,15 @@
         return str(self.parameters["definitions"].get(key, 1.0))
 
     def _get_constants(self, match: re.Match) -> str:
         """Replace matched constant string with its value"""
         key = match.group()
         return str(pluto_def_constants[key])
 
+    @override
     @classmethod
     def _validate_units_override_keys(cls, units_override):
         """Check that units in units_override are able to derive three base units:
         mass, length and time
         """
 
         # YT supports overriding other normalisations, this method ensures consistency
@@ -717,14 +733,15 @@
 
 class VtkMixin(Dataset):
     _index_class = VtkHierarchy
 
     def _read_data_header(self) -> str:
         return vtk_io.read_header(self.filename)
 
+    @override
     def _parse_parameter_file(self):
         # parse metadata
         with open(self.filename, "rb") as fh:
             md = vtk_io.read_metadata(fh)
         self.parameters.update(md)
 
         super()._parse_parameter_file()
@@ -761,14 +778,15 @@
 
 
 class IdefixDmpDataset(IdefixDataset):
     _dataset_type = "idefix-dmp"
     _index_class = IdefixDmpHierarchy
     _field_info_class = IdefixDmpFields
 
+    @override
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header_string = dmp_io.read_header(filename)
             return re.match(r"Idefix .* Dump Data", header_string) is not None
         except Exception:
             return False
@@ -776,14 +794,15 @@
     def _get_fields_metadata(self) -> tuple[IdefixFieldProperties, IdefixMetadata]:
         # read everything except large arrays
         return dmp_io.read_idefix_dmpfile(self.filename, skip_data=True)
 
     def _read_data_header(self) -> str:
         return dmp_io.read_header(self.filename)
 
+    @override
     def _parse_parameter_file(self):
         fprops, fdata = self._get_fields_metadata()
         self.parameters.update(fdata)
 
         self._detected_field_list = [k for k in fprops if re.match(r"^V[sc]-", k)]
 
         # parse the grid
@@ -808,52 +827,57 @@
         super()._parse_parameter_file()
 
 
 class IdefixVtkDataset(VtkMixin, IdefixDataset):
     _dataset_type = "idefix-vtk"
     _field_info_class = IdefixVtkFields
 
+    @override
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
         else:
             return "Idefix" in header
 
 
 class PlutoVtkDataset(VtkMixin, StaticPlutoDataset):
     _dataset_type = "pluto-vtk"
 
+    @override
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
         else:
             return "PLUTO" in header
 
+    @override
     def _get_log_file(self) -> str:
         return os.path.join(self.directory, "vtk.out")
 
 
 class PlutoXdmfDataset(StaticPlutoDataset):
     _dataset_type = "pluto-xdmf"
     _index_class = PlutoXdmfHierarchy
 
+    @override
     def _get_log_file(self) -> str:
         if (suffix := re.search(r"(flt|dbl)\.h5$", self.filename)) is not None:
             return os.path.join(self.directory, f"{suffix.group()}.out")
         else:
             raise RuntimeError(
                 f"Failed to detect log file associated with {self.filename}"
             )
 
+    @override
     def _parse_parameter_file(self):
         """
         Filenames are data.<snapnum>.<dbl/flt>.h5
         <snapnum> needs to be parse from the filename.
         <snapnum> is the corresponding entry in the <dbl/flt>.h5.out file
         Example <dbl/flt>.h5.out file:
             0 0.000000e+00 1.000000e-04 0 single_file little rho vx1 vx2 vx3 prs tr1 tr2 tr3 Temp ndens PbykB mach
@@ -910,19 +934,20 @@
             body = fh.read()
 
         if (res := re.match(r"(#.*\n)+", body)) is not None:
             return res.group()
         else:
             return ""
 
+    @override
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         if not (
             filename.endswith((".dbl.h5", ".flt.h5"))
-            and os.path.isfile(removesuffix(filename, ".h5") + ".xmf")
+            and os.path.isfile(filename.removesuffix(".h5") + ".xmf")
             and os.path.isfile(
                 os.path.join(
                     os.path.dirname(filename), os.path.basename(filename[-6:]) + ".out"
                 )
             )
         ):
             return False
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/definitions.py` & `yt_idefix-2.3.1/src/yt_idefix/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any
 
 import numpy as np
 
 # Physical constants in c.g.s units defined in $PLUTO_DIR/Src/pluto.h
 # The values are copied from PLUTO 4.4-patch-2
 pluto_def_constants = {
     "CONST_AH": 1.008,
@@ -35,15 +35,15 @@
 
 
 class _PlutoBaseUnits:
     """Derive base units from a given combination of units"""
 
     _base_unit_list = ("mass_unit", "length_unit", "time_unit")
 
-    def __init__(self, unit_combination: Dict[str, Any]):
+    def __init__(self, unit_combination: dict[str, Any]):
         # Fow now, unit_combination has been validated before passed in
         # But we still need to check the number of units here for insurance
         if len(unit_combination) != 3:
             raise ValueError(
                 "_PlutoBaseUnits requires a combination of 3 units "
                 f"({len(unit_combination)} given)"
             )
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix/fields.py` & `yt_idefix-2.3.1/src/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/src/yt_idefix/io.py` & `yt_idefix-2.3.1/src/yt_idefix/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from abc import ABC, abstractmethod
-from typing import BinaryIO, Tuple, cast
+from typing import BinaryIO, cast
 
 import numpy as np
 
 from yt.utilities.io_handler import BaseIOHandler, BaseParticleIOHandler
 from yt.utilities.on_demand_imports import _h5py as h5py
 
 from ._io import dmp_io, vtk_io
@@ -45,15 +45,15 @@
         pass
 
 
 class PlutoVtkIO(SingleGridIO):
     _dataset_type = "pluto-vtk"
 
     def _read_single_field(self, fh: BinaryIO, offset: int) -> np.ndarray:
-        shape = cast(Tuple[int, int, int], tuple(self.ds.domain_dimensions))
+        shape = cast(tuple[int, int, int], tuple(self.ds.domain_dimensions))
         return vtk_io.read_single_field(fh, shape=shape, offset=offset, skip_data=False)
 
 
 class IdefixVtkIO(PlutoVtkIO, BaseParticleIOHandler):
     _dataset_type = "idefix-vtk"
 
     def _read_particle_coords(self, chunks, ptf):
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.3.1/src/yt_idefix.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yt-idefix
-Version: 2.3.0
+Name: yt_idefix
+Version: 2.3.1
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -14,34 +14,36 @@
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: HDF5
 License-File: LICENSE
+Requires-Dist: inifix>=4.1.0
+Requires-Dist: numpy>=1.19.3
+Requires-Dist: yt>=4.2.0
+Requires-Dist: typing-extensions>=4.4.0; python_version < "3.12"
+Provides-Extra: hdf5
+Requires-Dist: h5py>=3.1.0; extra == "hdf5"
 
 
 # yt_idefix
 [![PyPI](https://img.shields.io/pypi/v/yt-idefix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/yt_idefix/)
-[![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
@@ -63,63 +65,76 @@
 compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
-Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
-
 ```python
-# Examples
 ds = yt.load(
-    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+    "data.0010.vtk",
+    definitions_header="../definitions.h",
+    inifile="example.ini",
 )
-ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
-The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
+Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
-Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
+```python
+ds = yt.load("data.0010.vtk", geometry="spherical")
+```
 
+The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. Data is always interpreted as dimensionful.
+For Pluto simulation, metadata is retrieved from `definitions.h` and `pluto.ini` to guess the proper on-disk units automatically.
+
+Units may also be provided at runtime using the `units_override` argument
 ```python
-# Examples on units
-ds = yt.load("data.0010.vtk", unit_system="mks")
+ds = yt.load(
+    "data.0010.vtk",
+    units_override={
+        "length_unit": (100.0, "au"),
+        "mass_unit": yt.units.mass_sun,
+    },
+)
+```
+Note that other units will also be changed for consistency (Pluto).
 
-units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
+Displayed units can also be controled using the `unit_system` argument.
+Accepted values are `"cgs"` (default), `"mks"` and `"code"`.
 
-# Caution that other units will also be changed for consistency!
-ds = yt.load("data.0010.vtk", unit_override=unit_override)
+```python
+ds = yt.load("data.0010.vtk", unit_system="mks")
 ```
-With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
+
+With Pluto data, units not specified with `units_override` will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
 
 ```python
 {"magnetic_unit", "velocity_unit", "density_unit"},
 {"velocity_unit", "time_unit", "length_unit"},
-{"density_unit", "length_unit", "mass_unit"},
+{"density_unit", "length_unit", "mass_unit"}
 ```
 
 yt is able to provide some derived fields from existed fields, e.g., `"cell_volume"`. Fields related to element species can be created according to primordial abundances of H and He, through `default_species_fields` (`"neutral"` and `"ionized"`) parameters.
 
 ```python
-# Example
 ds = yt.load("data.0010.vtk", default_species_fields="ionized")
 ```
 
-### Convention of field names
-The outputs are loaded from disk with field names in uppercase. This normalization is only applied to the standard outputs but user-defined outputs and Pluto's ion fraction outputs.
+### Conventions on field names
+
+Field names of on-disk fields for density, pressure, velocity and magnetic field components are always normalized to upper case, even if Pluto may use lowercase in some versions.
 
 ```python
-# Example
-ds.field_list
-# Output:
-# [('pluto-vtk', 'PRS'),   # standard output
-#  ('pluto-vtk', 'RHO'),   # standard output
-#  ('pluto-vtk', 'VX1'),   # standard output
-#  ('pluto-vtk', 'VX2'),   # standard output
-#  ('pluto-vtk', 'VX3'),   # standard output
-#  ('pluto-vtk', 'temp')]  # This is a user-defined output
+>>> ds.field_list
+[('pluto-vtk', 'PRS'),
+ ('pluto-vtk', 'RHO'),
+ ('pluto-vtk', 'VX1'),
+ ('pluto-vtk', 'VX2'),
+ ('pluto-vtk', 'VX3')]
 ```
+
+This normalization is only applied to non-user-defined outputs and Pluto's ion
+fraction outputs.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_idefix-2.3.0/src/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.3.1/src/yt_idefix.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 src/yt_idefix/__init__.py
-src/yt_idefix/_backports.py
 src/yt_idefix/api.py
 src/yt_idefix/data_structures.py
 src/yt_idefix/definitions.py
 src/yt_idefix/fields.py
 src/yt_idefix/io.py
 src/yt_idefix/misc.py
 src/yt_idefix/py.typed
```

### Comparing `yt_idefix-2.3.0/tests/test_C_io.py` & `yt_idefix-2.3.1/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/tests/test_dmp.py` & `yt_idefix-2.3.1/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/tests/test_vtk.py` & `yt_idefix-2.3.1/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.3.0/tests/test_xdmf.py` & `yt_idefix-2.3.1/tests/test_xdmf.py`

 * *Files identical despite different names*

