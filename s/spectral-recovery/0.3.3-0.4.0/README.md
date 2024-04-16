# Comparing `tmp/spectral_recovery-0.3.3.tar.gz` & `tmp/spectral_recovery-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectral_recovery-0.3.3.tar", last modified: Fri Apr  5 18:45:23 2024, max compression
+gzip compressed data, was "spectral_recovery-0.4.0.tar", last modified: Tue Apr 16 23:51:08 2024, max compression
```

## Comparing `spectral_recovery-0.3.3.tar` & `spectral_recovery-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.765288 spectral_recovery-0.3.3/
--rw-rw-rw-   0        0        0    10349 2023-10-11 06:09:47.000000 spectral_recovery-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    16166 2024-04-05 18:45:24.741288 spectral_recovery-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3325 2024-01-02 16:59:25.000000 spectral_recovery-0.3.3/README.md
--rw-rw-rw-   0        0        0     1192 2024-04-05 18:44:34.000000 spectral_recovery-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 18:45:24.768343 spectral_recovery-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:23.990643 spectral_recovery-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.116820 spectral_recovery-0.3.3/src/scripts/
--rw-rw-rw-   0        0        0        0 2023-10-11 06:09:52.000000 spectral_recovery-0.3.3/src/scripts/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-03-12 20:57:23.000000 spectral_recovery-0.3.3/src/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.401751 spectral_recovery-0.3.3/src/spectral_recovery/
--rw-rw-rw-   0        0        0      485 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/__init__.py
--rw-rw-rw-   0        0        0      566 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/_config.py
--rw-rw-rw-   0        0        0     4597 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/_utils.py
--rw-rw-rw-   0        0        0      517 2024-03-12 20:57:23.000000 spectral_recovery-0.3.3/src/spectral_recovery/enums.py
--rw-rw-rw-   0        0        0     3709 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/indices.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.672863 spectral_recovery-0.3.3/src/spectral_recovery/io/
--rw-rw-rw-   0        0        0        0 2024-02-13 22:18:33.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/__init__.py
--rw-rw-rw-   0        0        0     4797 2024-03-28 17:22:15.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/polygon.py
--rw-rw-rw-   0        0        0     8536 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/raster.py
--rw-rw-rw-   0        0        0    11227 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/metrics.py
--rw-rw-rw-   0        0        0     9548 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/plotting.py
--rw-rw-rw-   0        0        0    20944 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/restoration.py
--rw-rw-rw-   0        0        0    11375 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/targets.py
--rw-rw-rw-   0        0        0     5766 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/timeseries.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.720682 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/
--rw-rw-rw-   0        0        0    16166 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:08.109236 spectral_recovery-0.4.0/
+-rw-rw-rw-   0        0        0    10349 2024-04-16 22:44:32.000000 spectral_recovery-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    16620 2024-04-16 23:51:08.102024 spectral_recovery-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2024-04-16 23:41:17.000000 spectral_recovery-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1197 2024-04-16 23:50:51.000000 spectral_recovery-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:51:08.109236 spectral_recovery-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:07.881554 spectral_recovery-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:07.914555 spectral_recovery-0.4.0/src/scripts/
+-rw-rw-rw-   0        0        0        0 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/scripts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:08.013092 spectral_recovery-0.4.0/src/spectral_recovery/
+-rw-rw-rw-   0        0        0      483 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/__init__.py
+-rw-rw-rw-   0        0        0      246 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/_config.py
+-rw-rw-rw-   0        0        0     5345 2024-04-16 23:41:18.000000 spectral_recovery-0.4.0/src/spectral_recovery/_utils.py
+-rw-rw-rw-   0        0        0      517 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/enums.py
+-rw-rw-rw-   0        0        0     6101 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/indices.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:08.084992 spectral_recovery-0.4.0/src/spectral_recovery/io/
+-rw-rw-rw-   0        0        0        0 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/io/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/io/polygon.py
+-rw-rw-rw-   0        0        0     8509 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/io/raster.py
+-rw-rw-rw-   0        0        0    11102 2024-04-16 23:41:11.000000 spectral_recovery-0.4.0/src/spectral_recovery/metrics.py
+-rw-rw-rw-   0        0        0     8990 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/plotting.py
+-rw-rw-rw-   0        0        0    14042 2024-04-16 23:41:11.000000 spectral_recovery-0.4.0/src/spectral_recovery/restoration.py
+-rw-rw-rw-   0        0        0     7926 2024-04-16 23:41:18.000000 spectral_recovery-0.4.0/src/spectral_recovery/targets.py
+-rw-rw-rw-   0        0        0     5766 2024-04-16 22:44:33.000000 spectral_recovery-0.4.0/src/spectral_recovery/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:51:08.093025 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/
+-rw-rw-rw-   0        0        0    16620 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      307 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-16 23:51:07.000000 spectral_recovery-0.4.0/src/spectral_recovery.egg-info/top_level.txt
```

### Comparing `spectral_recovery-0.3.3/LICENSE` & `spectral_recovery-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.3/PKG-INFO` & `spectral_recovery-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral_recovery
-Version: 0.3.3
+Version: 0.4.0
 Author-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 Maintainer-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -188,40 +188,42 @@
 Requires-Dist: geopandas>=0.13.2
 Requires-Dist: rioxarray>=0.14.1
 Requires-Dist: rasterio>=1.3.7
 Requires-Dist: xarray>=2023.5.0
 Requires-Dist: spyndex==0.5.0
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: click>=8.1.3
-Requires-Dist: dask<2024.3,>=2023.5.1
-Requires-Dist: distributed<2024.3,>=2023.5.1
+Requires-Dist: dask>=2023.5.1
+Requires-Dist: distributed>=2023.5.1
+Requires-Dist: dask-expr>=1.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: prettytable>=3.9.0
 Provides-Extra: test
 Requires-Dist: pytest>=7.3.2; extra == "test"
 Requires-Dist: pytest-mock==3.12.0; extra == "test"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint-exit; extra == "lint"
 Requires-Dist: black==23.12.0; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 
 # (pre-release) spectral-recovery: spectral recovery analysis of forested ecosystems
 
-[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
+
 
 ---
 Github: [https://github.com/PEOPLE-ER/Spectral-Recovery/](https://github.com/PEOPLE-ER/Spectral-Recovery/)
 
 Documentation: [https://people-er.github.io/Spectral-Recovery/](https://people-er.github.io/Spectral-Recovery/)
 
 PyPi: [https://pypi.org/project/spectral-recovery/](https://pypi.org/project/spectral-recovery/)
 
-Interactive Notebooks: Coming soon!
+Interactive Notebooks (Binder): [https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ---
 ## Overview
 
 **spectral-recovery** is an open-source project and Python package that provides computationally simple, centralized, and reproducible methods for performing [spectral recovery analysis](https://people-er.github.io/Spectral-Recovery/about/#13-looking-at-recovery-trajectories) of forests using satellite imagery.
 
 The package provides straight-forward interfaces to help coordinate the many moving parts of spectral recovery analysis. Users provide restoration site locations, restoration dates, and annual composites of spectral data, while spectral-recovery handles computing the spectral indices, recovery targets, recovery metrics, and more!
@@ -233,15 +235,15 @@
 ```{bash}
 pip install spectral-recovery
 ```
 
 ## Documentation
 
 - View background information, static tutorials, and API references in our [project documentation.](https://people-er.github.io/Spectral-Recovery/)
-- Try out an interactive notebook (Coming soon!)
+- Try out an interactive notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ## Contributing
 
 - Report bugs, suggest features, and see what others are saying on our [GitHub Issues](https://github.com/PEOPLE-ER/Spectral-Recovery/issues) page.
 - Start discussions about the tool on our [discussion page](https://github.com/PEOPLE-ER/Spectral-Recovery/discussions).
 - Want to contribute code? See our [CONTRIBUTING](https://github.com/PEOPLE-ER/Spectral-Recovery/blob/main/CONTRIBUTING.md) document for more information.
```

### Comparing `spectral_recovery-0.3.3/README.md` & `spectral_recovery-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # (pre-release) spectral-recovery: spectral recovery analysis of forested ecosystems
 
-[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
+
 
 ---
 Github: [https://github.com/PEOPLE-ER/Spectral-Recovery/](https://github.com/PEOPLE-ER/Spectral-Recovery/)
 
 Documentation: [https://people-er.github.io/Spectral-Recovery/](https://people-er.github.io/Spectral-Recovery/)
 
 PyPi: [https://pypi.org/project/spectral-recovery/](https://pypi.org/project/spectral-recovery/)
 
-Interactive Notebooks: Coming soon!
+Interactive Notebooks (Binder): [https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ---
 ## Overview
 
 **spectral-recovery** is an open-source project and Python package that provides computationally simple, centralized, and reproducible methods for performing [spectral recovery analysis](https://people-er.github.io/Spectral-Recovery/about/#13-looking-at-recovery-trajectories) of forests using satellite imagery.
 
 The package provides straight-forward interfaces to help coordinate the many moving parts of spectral recovery analysis. Users provide restoration site locations, restoration dates, and annual composites of spectral data, while spectral-recovery handles computing the spectral indices, recovery targets, recovery metrics, and more!
@@ -25,15 +26,15 @@
 ```{bash}
 pip install spectral-recovery
 ```
 
 ## Documentation
 
 - View background information, static tutorials, and API references in our [project documentation.](https://people-er.github.io/Spectral-Recovery/)
-- Try out an interactive notebook (Coming soon!)
+- Try out an interactive notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ## Contributing
 
 - Report bugs, suggest features, and see what others are saying on our [GitHub Issues](https://github.com/PEOPLE-ER/Spectral-Recovery/issues) page.
 - Start discussions about the tool on our [discussion page](https://github.com/PEOPLE-ER/Spectral-Recovery/discussions).
 - Want to contribute code? See our [CONTRIBUTING](https://github.com/PEOPLE-ER/Spectral-Recovery/blob/main/CONTRIBUTING.md) document for more information.
 
@@ -53,8 +54,8 @@
 
 [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `spectral_recovery-0.3.3/pyproject.toml` & `spectral_recovery-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
-version = "0.3.3"
+version = "0.4.0"
 dependencies = [
     "geopandas >= 0.13.2",
     "rioxarray >= 0.14.1",
     "rasterio >= 1.3.7",
     "xarray >= 2023.5.0",
     "spyndex == 0.5.0",
     "numpy >= 1.24.3",
     "click >= 8.1.3",
-    "dask >= 2023.5.1, < 2024.3",
-    "distributed >= 2023.5.1, < 2024.3",
+    "dask >= 2023.5.1",
+    "distributed >= 2023.5.1",
+    "dask-expr >= 1.0",
     "matplotlib >= 3.7.1",
     "seaborn >= 0.12.2",
     "prettytable >= 3.9.0",
 ]
 
 [project.optional-dependencies]
 test = [
```

### Comparing `spectral_recovery-0.3.3/src/scripts/cli.py` & `spectral_recovery-0.4.0/src/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/_utils.py` & `spectral_recovery-0.4.0/src/spectral_recovery/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utility functions for spectral-recovery."""
 
 import functools
 import spyndex as spx
+import xarray as xr
 
 from rioxarray.exceptions import MissingCRS
 from prettytable import PrettyTable, ALL
 
 
 def maintain_rio_attrs(func: callable) -> callable:
     """A wrapper for maintaining rioxarray crs/encoding info.
@@ -35,20 +36,37 @@
         Notes
         -----
         The first argument passed to a wrapped function (keyword or
         non-keyword) must be the xarray DataArray whose rio info
         is to be maintained.
 
         """
-        # Take the first argument
-        if args:
-            xarray_obj = args[0]
-        else:
-            # NOTE: this only works for Python 3.6+ where dicts keep insertion order by default
-            xarray_obj = next(iter(kwargs.values()))
+        kwarg_vals = list(kwargs.values())
+        # Take the first xarray arg
+        arg_da = [isinstance(arg, xr.DataArray) for arg in args]
+        kwarg_da = [isinstance(kwv, xr.DataArray) for kwv in kwarg_vals]
+        if sum(arg_da + kwarg_da) > 1:
+            epsgs = []
+            for i, val in enumerate(arg_da):
+                if val:
+                    crs = args[i].rio.crs
+                    epsgs.append(crs)
+            for i, val in enumerate(kwarg_da):
+                if val:
+                    crs = kwarg_vals[i].rio.crs
+                    epsgs.append(crs)
+            if not epsgs.count(epsgs[0]) == len(epsgs):
+                raise ValueError(f"Ambiguous input for wrapper. CRS on xarray.DataArray inputs do not match.")
+        for i, val in enumerate(arg_da):
+            if val:
+                xarray_obj = args[i]
+        for i, val in enumerate(kwarg_da):
+            if val:
+                xarray_obj = kwarg_vals[i]
+
         result = func(*args, **kwargs)
         try:
             result.rio.write_crs(xarray_obj.rio.crs, inplace=True)
         except MissingCRS:
             # TODO: add warning log here?
             pass
         result.rio.update_encoding(xarray_obj.encoding, inplace=True)
```

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/enums.py` & `spectral_recovery-0.4.0/src/spectral_recovery/enums.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/io/raster.py` & `spectral_recovery-0.4.0/src/spectral_recovery/io/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 
 from spectral_recovery._utils import bands_pretty_table, common_and_long_to_short
 from rasterio._err import CPLE_AppDefinedError
 
 from spectral_recovery._config import (
     VALID_YEAR,
     REQ_DIMS,
-    SUPPORTED_PLATFORMS,
     STANDARD_BANDS,
 )
 
 COMMON_LONG_SHORT_DICT = common_and_long_to_short(STANDARD_BANDS)
 BANDS_TABLE = bands_pretty_table()
 
 
 def read_timeseries(
     path_to_tifs: List[str] | str,
     band_names: Dict[int, str] = None,
     path_to_mask: str = None,
-    array_type: str = "numpy",
+    array_type: str = "dask",
 ):
     """Reads and stacks a list of tifs into a 4D DataArray.
 
     Parameters
     ----------
     path_to_tifs : list of str
         List of paths to TIFs or path to directory containing TIFs.
```

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/metrics.py` & `spectral_recovery-0.4.0/src/spectral_recovery/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 
 from spectral_recovery._utils import maintain_rio_attrs
 from spectral_recovery.restoration import RestorationArea
 from spectral_recovery.indices import compute_indices
-from spectral_recovery.targets import MedianTarget
 
 
 NEG_TIMESTEP_MSG = "timestep cannot be negative."
 VALID_PERC_MSP = "percent must be between 0 and 100."
 METRIC_FUNCS = {}
 
 
@@ -25,24 +24,22 @@
 
 
 @maintain_rio_attrs
 def compute_metrics(
     timeseries_data: xr.DataArray,
     restoration_polygons: gpd.GeoDataFrame,
     metrics: List[str],
-    reference_polygons: gpd.GeoDataFrame = None,
+    recovery_target: xr.DataArray,
     timestep: int = 5,
     percent_of_target: int = 80,
-    recovery_target_method=MedianTarget(scale="polygon"),
 ):
     restoration_area = RestorationArea(
-        restoration_polygon=restoration_polygons,
-        reference_polygons=reference_polygons,
+        restoration_site=restoration_polygons,
         composite_stack=timeseries_data,
-        recovery_target_method=recovery_target_method,
+        recovery_target=recovery_target,
     )
     m_results = []
     for m in metrics:
         try:
             m_func = METRIC_FUNCS[m.lower()]
         except KeyError:
             raise ValueError(f"{m} is not a valid metric choice!")
@@ -239,18 +236,17 @@
 
     try:
         y2r_v = y2r_v.squeeze("time")
     except KeyError:
         pass
     return y2r_v
 
+
 @register_metric
-def rri(
-    ra: RestorationArea, params: Dict = {"timestep": 5}
-) -> xr.DataArray:
+def rri(ra: RestorationArea, params: Dict = {"timestep": 5}) -> xr.DataArray:
     """Per-pixel RRI.
 
     A modified version of the commonly used RI, the RRI accounts for
     noise in trajectory by using the maximum from the 4th or 5th year
     in monitoring window. The metric relates recovery magnitude to
     disturbance magnitude, and is the change in index value in 4 or 5
     years divided by the change due to disturbance.
@@ -276,21 +272,29 @@
     if params["timestep"] == 0:
         raise ValueError("timestep for RRI must be greater than 0.")
 
     rest_post_tm1 = str(int(ra.restoration_start) + (params["timestep"] - 1))
     rest_post_t = str(int(ra.restoration_start) + params["timestep"])
 
     if pd.to_datetime(rest_post_tm1) not in ra.restoration_image_stack.time.values:
-        raise ValueError(f"{rest_post_tm1} (year of timestep - 1) not found in time dim.")
-    if  pd.to_datetime(rest_post_t) not in ra.restoration_image_stack.time.values:
+        raise ValueError(
+            f"{rest_post_tm1} (year of timestep - 1) not found in time dim."
+        )
+    if pd.to_datetime(rest_post_t) not in ra.restoration_image_stack.time.values:
         raise ValueError(f"{rest_post_t} (year of timestep) not found in time dim.")
 
-    max_rest_t_tm1 = ra.restoration_image_stack.sel(time=slice(rest_post_tm1, rest_post_t)).max(dim=["time"])
-    rest_start = ra.restoration_image_stack.sel(time=ra.restoration_start).drop_vars("time")
-    dist_start = ra.restoration_image_stack.sel(time=ra.disturbance_start).drop_vars("time")
+    max_rest_t_tm1 = ra.restoration_image_stack.sel(
+        time=slice(rest_post_tm1, rest_post_t)
+    ).max(dim=["time"])
+    rest_start = ra.restoration_image_stack.sel(time=ra.restoration_start).drop_vars(
+        "time"
+    )
+    dist_start = ra.restoration_image_stack.sel(time=ra.disturbance_start).drop_vars(
+        "time"
+    )
     dist_end = rest_start
 
     rri_v = (max_rest_t_tm1 - rest_start) / (dist_start - dist_end)
     # if dist_pre_1_2 has length greater than one we will need to squeeze the time dim
     try:
         rri_v = rri_v.squeeze("time")
     except KeyError:
```

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/plotting.py` & `spectral_recovery-0.4.0/src/spectral_recovery/plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,67 +6,71 @@
 import seaborn as sns
 
 from matplotlib.lines import Line2D
 from matplotlib.patches import Patch
 from matplotlib.legend_handler import HandlerPatch
 
 from spectral_recovery.restoration import RestorationArea
-from spectral_recovery.targets import MedianTarget
 from spectral_recovery.indices import compute_indices
 
 
 # TODO: Refactor. Bring plot_spectral_trajectory into this module.
 def plot_spectral_trajectory(
     timeseries_data: xr.DataArray,
     restoration_polygons: gpd.GeoDataFrame,
-    reference_polygons: gpd.GeoDataFrame = None,
-    recovery_target_method=MedianTarget(scale="polygon"),
+    recovery_target: xr.DataArray,
+    reference_start: str = None, 
+    reference_end: str = None, 
     path: str = None,
 ):
     """Plot the spectral trajectory of the restoration polygon
 
     Parameters
     ----------
     timeseries_data : xr.DataArray
         Timeseries data (annual composites)
     restoration_polygons : gpd.GeoDataFrame
         Restoration polygon and dates
     indices : list of str
         Indices to visualize trajectory for
-    reference_polygons : gpd.GeoDataFrame, optional
-        The refernce polygons to compute recovery target with
     indices_constants : dict
         Constant values for indices
     recovery_target_method : callable
         Recovery target method to derive recovery target values
 
     """
     restoration_area = RestorationArea(
-        restoration_polygon=restoration_polygons,
-        reference_polygons=reference_polygons,
+        restoration_site=restoration_polygons,
         composite_stack=timeseries_data,
-        recovery_target_method=recovery_target_method,
+        recovery_target=recovery_target,
     )
     if path:
-        plot_ra(ra=restoration_area, path=path)
+        plot_ra(ra=restoration_area, reference_start=reference_start, reference_end=reference_end, path=path)
     else:
-        plot_ra(ra=restoration_area)
+        plot_ra(ra=restoration_area, reference_start=reference_start, reference_end=reference_end,)
 
 
-def plot_ra(ra: RestorationArea, path: str = None, legend: bool = True) -> None:
+def plot_ra(
+        ra: RestorationArea,
+        reference_start: str, 
+        reference_end: str,
+        path: str = None,
+        legend: bool = True,
+        ) -> None:
     """Create spectral trajectory plot of the RestorationArea (ra)
 
     Parameters
     ----------
     ra : spectral_recovery.restoration.RestorationArea
         The restoration area to plot.
     path : str, optional
         The path to save the plot to.
     """
-    hist_ref_sys = ra.reference_polygons is None
+
+    plot_ref_window = bool(reference_start and reference_end)
 
     stats = ra.restoration_image_stack.satts.stats()
     stats = stats.sel(
         stats=[
             "median",
             "mean",
         ]
@@ -116,20 +120,20 @@
             x="time",
             y="reco_targets",
             ax=axi,
             color="black",
             linestyle=(0, (3, 5, 1, 5)),
             lw=1,
         )
-        _draw_trajectory_windows(ra, axi, palette, hist_ref_sys)
+        _draw_trajectory_windows(ra, reference_start, reference_end, axi, palette, plot_ref_window)
         _set_axis_labels(ra, axi, band, data["time"].unique().tolist())
     (
         labels,
         custom_handles,
-    ) = _custom_legend_labels_handles(ra, palette, hist_ref_sys)
+    ) = _custom_legend_labels_handles(ra, palette, plot_ref_window)
 
     if legend:
         plt.figlegend(
             labels=labels,
             handles=custom_handles,
             loc="lower center",
             fancybox=True,
@@ -154,15 +158,15 @@
         rotation=45,
         ha="right",
     )
     axi.set_xlabel("Year")
     axi.set_ylabel(f"{title} Value")
 
 
-def _draw_trajectory_windows(ra, axi, palette, hist_ref_sys):
+def _draw_trajectory_windows(ra, refs, refe, axi, palette, plot_ref_window):
     """Draw the trajectory windows onto subplots.
 
     Uses two verticle dashed lines to delimit the start and
     end years of a window. If the start and end years are
     not the same year, then the space between the two dashed lines
     is filled in (vertical span). Each window (i.e line/span group)
     is coloured a distinct colour.
@@ -200,39 +204,39 @@
     axi.axvspan(
         ra.disturbance_start,
         ra.restoration_start,
         alpha=0.2,
         color=palette[3],
     )
 
-    if hist_ref_sys:
+    if plot_ref_window:
         # if deriving target from recovery polygon, draw reference window
         axi.axvline(
-            x=ra.reference_years[0],
+            x=refs,
             color=palette[4],
             linestyle="dashed",
             lw=1,
         )
         axi.axvspan(
-            ra.reference_years[0],
-            ra.reference_years[1],
+            refs,
+            refe,
             alpha=0.2,
             color=palette[4],
         )
         # only draw line if reference ye
-        if ra.reference_years[1] != ra.disturbance_start:
+        if refe != refs:
             axi.axvline(
-                x=ra.reference_years[1],
+                x=refe,
                 color=palette[4],
                 linestyle="dashed",
                 lw=1,
             )
 
 
-def _custom_legend_labels_handles(ra, palette, hist_ref_sys) -> Tuple[List, List]:
+def _custom_legend_labels_handles(ra, palette, plot_ref_window) -> Tuple[List, List]:
     """Create a custom legend to match trajectory plots
 
     Returns
     -------
     tuple of lists
         custom labels and handles to pass to ``figlegend``
 
@@ -255,28 +259,15 @@
 
     labels = [
         "median",
         "mean",
         "disturbance window",
         "recovery window",
     ]
-    if hist_ref_sys:
-        if isinstance(ra.recovery_target_method, MedianTarget):
-            if ra.recovery_target_method.scale == "pixel":
-                custom_handles.insert(
-                    2,
-                    (recovery_target_line),
-                )
-                labels.insert(2, "recovery target (estimated mean)")
-            else:
-                custom_handles.insert(
-                    2,
-                    recovery_target_line,
-                )
-                labels.insert(2, "recovery target")
+    if plot_ref_window:
 
         custom_handles.insert(3, reference_years_patch)
         labels.insert(3, "reference year(s)")
     else:
         custom_handles.insert(
             2,
             recovery_target_line,
```

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery/timeseries.py` & `spectral_recovery-0.4.0/src/spectral_recovery/timeseries.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery.egg-info/PKG-INFO` & `spectral_recovery-0.4.0/src/spectral_recovery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral_recovery
-Version: 0.3.3
+Version: 0.4.0
 Author-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 Maintainer-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -188,40 +188,42 @@
 Requires-Dist: geopandas>=0.13.2
 Requires-Dist: rioxarray>=0.14.1
 Requires-Dist: rasterio>=1.3.7
 Requires-Dist: xarray>=2023.5.0
 Requires-Dist: spyndex==0.5.0
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: click>=8.1.3
-Requires-Dist: dask<2024.3,>=2023.5.1
-Requires-Dist: distributed<2024.3,>=2023.5.1
+Requires-Dist: dask>=2023.5.1
+Requires-Dist: distributed>=2023.5.1
+Requires-Dist: dask-expr>=1.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: prettytable>=3.9.0
 Provides-Extra: test
 Requires-Dist: pytest>=7.3.2; extra == "test"
 Requires-Dist: pytest-mock==3.12.0; extra == "test"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint-exit; extra == "lint"
 Requires-Dist: black==23.12.0; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 
 # (pre-release) spectral-recovery: spectral recovery analysis of forested ecosystems
 
-[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/spectral-recovery.svg)](https://badge.fury.io/py/spectral-recovery) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
+
 
 ---
 Github: [https://github.com/PEOPLE-ER/Spectral-Recovery/](https://github.com/PEOPLE-ER/Spectral-Recovery/)
 
 Documentation: [https://people-er.github.io/Spectral-Recovery/](https://people-er.github.io/Spectral-Recovery/)
 
 PyPi: [https://pypi.org/project/spectral-recovery/](https://pypi.org/project/spectral-recovery/)
 
-Interactive Notebooks: Coming soon!
+Interactive Notebooks (Binder): [https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ---
 ## Overview
 
 **spectral-recovery** is an open-source project and Python package that provides computationally simple, centralized, and reproducible methods for performing [spectral recovery analysis](https://people-er.github.io/Spectral-Recovery/about/#13-looking-at-recovery-trajectories) of forests using satellite imagery.
 
 The package provides straight-forward interfaces to help coordinate the many moving parts of spectral recovery analysis. Users provide restoration site locations, restoration dates, and annual composites of spectral data, while spectral-recovery handles computing the spectral indices, recovery targets, recovery metrics, and more!
@@ -233,15 +235,15 @@
 ```{bash}
 pip install spectral-recovery
 ```
 
 ## Documentation
 
 - View background information, static tutorials, and API references in our [project documentation.](https://people-er.github.io/Spectral-Recovery/)
-- Try out an interactive notebook (Coming soon!)
+- Try out an interactive notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PEOPLE-ER/Spectral-Recovery/HEAD?labpath=docs%2Fnotebooks%2F)
 
 ## Contributing
 
 - Report bugs, suggest features, and see what others are saying on our [GitHub Issues](https://github.com/PEOPLE-ER/Spectral-Recovery/issues) page.
 - Start discussions about the tool on our [discussion page](https://github.com/PEOPLE-ER/Spectral-Recovery/discussions).
 - Want to contribute code? See our [CONTRIBUTING](https://github.com/PEOPLE-ER/Spectral-Recovery/blob/main/CONTRIBUTING.md) document for more information.
```

### Comparing `spectral_recovery-0.3.3/src/spectral_recovery.egg-info/SOURCES.txt` & `spectral_recovery-0.4.0/src/spectral_recovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

