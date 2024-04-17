# Comparing `tmp/tfv-1.0.8.1.tar.gz` & `tmp/tfv-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfv-1.0.8.1.tar", last modified: Tue Apr 16 02:39:12 2024, max compression
+gzip compressed data, was "tfv-1.0.9.tar", last modified: Tue Apr 16 04:18:59 2024, max compression
```

## Comparing `tfv-1.0.8.1.tar` & `tfv-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:39:12.354152 tfv-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-16 02:38:36.000000 tfv-1.0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2311 2024-04-16 02:39:12.354152 tfv-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-04-16 02:38:36.000000 tfv-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-16 02:38:37.000000 tfv-1.0.8.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-04-16 02:39:12.354152 tfv-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 02:38:37.000000 tfv-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:39:12.350152 tfv-1.0.8.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tests/test_bed_restart.py
--rw-rw-rw-   0 root         (0) root         (0)     3982 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tests/test_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tests/test_timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     9153 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tests/test_xarray_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:39:12.352152 tfv-1.0.8.1/tfv/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8835 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/_grid_to_tfv.py
--rw-rw-rw-   0 root         (0) root         (0)    46370 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18282 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/miscellaneous.py
--rw-rw-rw-   0 root         (0) root         (0)     4724 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/mldatetime.py
--rw-rw-rw-   0 root         (0) root         (0)     8488 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/particles.py
--rw-rw-rw-   0 root         (0) root         (0)    14697 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/restart.py
--rw-rw-rw-   0 root         (0) root         (0)    15812 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)    20439 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/viewer.py
--rw-rw-rw-   0 root         (0) root         (0)    50116 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/visual.py
--rw-rw-rw-   0 root         (0) root         (0)    87084 2024-04-16 02:38:37.000000 tfv-1.0.8.1/tfv/xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:39:12.353152 tfv-1.0.8.1/tfv.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2311 2024-04-16 02:39:12.000000 tfv-1.0.8.1/tfv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-16 02:39:12.000000 tfv-1.0.8.1/tfv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 02:39:12.000000 tfv-1.0.8.1/tfv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      145 2024-04-16 02:39:12.000000 tfv-1.0.8.1/tfv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-16 02:39:12.000000 tfv-1.0.8.1/tfv.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:18:59.230772 tfv-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-16 04:18:24.000000 tfv-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-16 04:18:59.230772 tfv-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-04-16 04:18:24.000000 tfv-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-16 04:18:25.000000 tfv-1.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-04-16 04:18:59.231772 tfv-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 04:18:25.000000 tfv-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:18:59.227772 tfv-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-16 04:18:25.000000 tfv-1.0.9/tests/test_bed_restart.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2024-04-16 04:18:25.000000 tfv-1.0.9/tests/test_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-16 04:18:25.000000 tfv-1.0.9/tests/test_timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     9153 2024-04-16 04:18:25.000000 tfv-1.0.9/tests/test_xarray_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:18:59.229772 tfv-1.0.9/tfv/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8835 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/_grid_to_tfv.py
+-rw-rw-rw-   0 root         (0) root         (0)    46370 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18282 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/miscellaneous.py
+-rw-rw-rw-   0 root         (0) root         (0)     4724 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/mldatetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     8488 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/particles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14697 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/restart.py
+-rw-rw-rw-   0 root         (0) root         (0)    15812 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)    20439 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/viewer.py
+-rw-rw-rw-   0 root         (0) root         (0)    50116 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/visual.py
+-rw-rw-rw-   0 root         (0) root         (0)    87198 2024-04-16 04:18:25.000000 tfv-1.0.9/tfv/xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:18:59.230772 tfv-1.0.9/tfv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-16 04:18:59.000000 tfv-1.0.9/tfv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-16 04:18:59.000000 tfv-1.0.9/tfv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 04:18:59.000000 tfv-1.0.9/tfv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-16 04:18:59.000000 tfv-1.0.9/tfv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-16 04:18:59.000000 tfv-1.0.9/tfv.egg-info/top_level.txt
```

### Comparing `tfv-1.0.8.1/LICENSE` & `tfv-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/PKG-INFO` & `tfv-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfv
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: Post processing tools for TUFLOW FV results
 Home-page: https://gitlab.com/TUFLOW/tfv
 Author: TUFLOW Support
 Author-email: support@tuflow.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tfv-1.0.8.1/README.md` & `tfv-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/setup.cfg` & `tfv-1.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tfv
-version = 1.0.8.1
+version = 1.0.9
 description = Post processing tools for TUFLOW FV results
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/TUFLOW/tfv
 author = TUFLOW Support
 author_email = support@tuflow.com
 classifiers =
```

### Comparing `tfv-1.0.8.1/tests/test_bed_restart.py` & `tfv-1.0.9/tests/test_bed_restart.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tests/test_extractor.py` & `tfv-1.0.9/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tests/test_timeseries.py` & `tfv-1.0.9/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tests/test_xarray_accessor.py` & `tfv-1.0.9/tests/test_xarray_accessor.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/_grid_to_tfv.py` & `tfv-1.0.9/tfv/_grid_to_tfv.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/extractor.py` & `tfv-1.0.9/tfv/extractor.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/geometry.py` & `tfv-1.0.9/tfv/geometry.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/miscellaneous.py` & `tfv-1.0.9/tfv/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/mldatetime.py` & `tfv-1.0.9/tfv/mldatetime.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/particles.py` & `tfv-1.0.9/tfv/particles.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/restart.py` & `tfv-1.0.9/tfv/restart.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/timeseries.py` & `tfv-1.0.9/tfv/timeseries.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/viewer.py` & `tfv-1.0.9/tfv/viewer.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/visual.py` & `tfv-1.0.9/tfv/visual.py`

 * *Files identical despite different names*

### Comparing `tfv-1.0.8.1/tfv/xarray.py` & `tfv-1.0.9/tfv/xarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,31 +290,31 @@
                 self.xtr = FvExtractor(self._obj)
                 self.__convert_coords__()
             except TypeError:
                 print(
                     "Data does not appear to be a valid TUFLOW FV spatial netcdf file"
                 )
 
-    def get_cell_index(self, x, y):
+    def get_cell_index(self, x: Union[float, np.ndarray], y: Union[float, np.ndarray]) -> np.ndarray:
         """Returns the cell index(s) containing coordinate(s) x and y.
 
         Multiple cell indexes will be returned using this command if x/y are 1D.
 
         Args:
-            x (float): x-coordinate
-            y (float): y-coordinate
+            x ([float, np.ndarray]): x-coordinate
+            y ([float, np.ndarray]): y-coordinate
 
         Returns:
             cell_index (int): index of corresponding cell containing coordinates (x,y)
         """
         return self.xtr.get_cell_index(x, y)
     
 
-    def get_cell_inpolygon(self, polygon):
-        """Returns the cell indexes inside a specified polygon.
+    def get_cell_inpolygon(self, polygon: np.ndarray) -> np.ndarray:
+        """Returns cell indexes intersected by a polygon.
 
         The polygon should be provided as either a 2D Numpy ndarray (i.e., Nx2 array), 
         or if the `Shapely` package is available, a WKT String polygon or shapely Polygon object can be provided.
 
         Args:
             polygon ([np.ndarray, str, shapely.geometry.Polygon]): A single polygon feature, provided as a 2D numpy array (Nx2).
                 If `shapely` is available, polygon may also be provided as a wkt string, or a shapely Polygon feature.
```

### Comparing `tfv-1.0.8.1/tfv.egg-info/PKG-INFO` & `tfv-1.0.9/tfv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfv
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: Post processing tools for TUFLOW FV results
 Home-page: https://gitlab.com/TUFLOW/tfv
 Author: TUFLOW Support
 Author-email: support@tuflow.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

