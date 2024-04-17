# Comparing `tmp/geocube-0.5.1.tar.gz` & `tmp/geocube-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocube-0.5.1.tar", last modified: Mon Mar 18 14:21:32 2024, max compression
+gzip compressed data, was "geocube-0.5.2.tar", last modified: Wed Apr 17 15:49:27 2024, max compression
```

## Comparing `geocube-0.5.1.tar` & `geocube-0.5.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.813618 geocube-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-18 14:21:21.000000 geocube-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-18 14:21:21.000000 geocube-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-18 14:21:21.000000 geocube-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-18 14:21:21.000000 geocube-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-18 14:21:32.813618 geocube-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-18 14:21:21.000000 geocube-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/cli/commands/make_geocube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/cli/geocube.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/geo_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/geo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/geo_utils/geobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/rasterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/vector_to_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube/xarray_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/xarray_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-18 14:21:21.000000 geocube-0.5.1/geocube/xarray_extensions/vectorxarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:21:32.809618 geocube-0.5.1/geocube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 14:21:32.000000 geocube-0.5.1/geocube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-18 14:21:21.000000 geocube-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-18 14:21:32.813618 geocube-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-18 14:21:21.000000 geocube-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.850742 geocube-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-17 15:49:18.000000 geocube-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-17 15:49:18.000000 geocube-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-17 15:49:18.000000 geocube-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 15:49:18.000000 geocube-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-17 15:49:27.850742 geocube-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-17 15:49:18.000000 geocube-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.842742 geocube-0.5.2/geocube/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/cli/commands/make_geocube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/cli/geocube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube/geo_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/geo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/geo_utils/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/rasterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/vector_to_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube/xarray_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/xarray_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 15:49:18.000000 geocube-0.5.2/geocube/xarray_extensions/vectorxarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:49:27.846742 geocube-0.5.2/geocube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 15:49:27.000000 geocube-0.5.2/geocube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 15:49:18.000000 geocube-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 15:49:27.850742 geocube-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 15:49:18.000000 geocube-0.5.2/setup.py
```

### Comparing `geocube-0.5.1/AUTHORS.rst` & `geocube-0.5.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/CONTRIBUTING.rst` & `geocube-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/LICENSE` & `geocube-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/PKG-INFO` & `geocube-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocube
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tool to convert geopandas vector data into rasterized xarray data.
 Home-page: https://github.com/corteva/geocube
 Download-URL: http://python.org/pypi/geocube
 Author: geocube Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: geocube,GDAL,rasterize,vector
```

### Comparing `geocube-0.5.1/README.rst` & `geocube-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/_show_versions.py` & `geocube-0.5.2/geocube/_show_versions.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/api/core.py` & `geocube-0.5.2/geocube/api/core.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/cli/commands/make_geocube.py` & `geocube-0.5.2/geocube/cli/commands/make_geocube.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/cli/geocube.py` & `geocube-0.5.2/geocube/cli/geocube.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/geo_utils/geobox.py` & `geocube-0.5.2/geocube/geo_utils/geobox.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/logger.py` & `geocube-0.5.2/geocube/logger.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/rasterize.py` & `geocube-0.5.2/geocube/rasterize.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/vector.py` & `geocube-0.5.2/geocube/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             mask = data_array != data_array.rio.nodata
 
     # vectorize generator
     vectorized_data = (
         (value, shapely.geometry.shape(polygon))
         for polygon, value in rasterio.features.shapes(
             data_array,
-            transform=data_array.rio.transform(),
+            transform=data_array.rio.transform(recalc=True),
             mask=mask,
         )
     )
 
     if data_array.name:
         name = data_array.name
     else:
```

### Comparing `geocube-0.5.1/geocube/vector_to_cube.py` & `geocube-0.5.2/geocube/vector_to_cube.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube/xarray_extensions/vectorxarray.py` & `geocube-0.5.2/geocube/xarray_extensions/vectorxarray.py`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/geocube.egg-info/PKG-INFO` & `geocube-0.5.2/geocube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocube
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tool to convert geopandas vector data into rasterized xarray data.
 Home-page: https://github.com/corteva/geocube
 Download-URL: http://python.org/pypi/geocube
 Author: geocube Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: geocube,GDAL,rasterize,vector
```

### Comparing `geocube-0.5.1/geocube.egg-info/SOURCES.txt` & `geocube-0.5.2/geocube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocube-0.5.1/setup.cfg` & `geocube-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 author = geocube Contributors
 author_email = alansnow21@gmail.com
 name = geocube
-version = 0.5.1
+version = 0.5.2
 description = Tool to convert geopandas vector data into rasterized xarray data.
 keywords = geocube, GDAL, rasterize, vector
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = BSD license
 license_files = LICENSE
 platform = any
```

