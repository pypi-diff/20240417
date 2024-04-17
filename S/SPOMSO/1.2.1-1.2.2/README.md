# Comparing `tmp/SPOMSO-1.2.1.tar.gz` & `tmp/spomso-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPOMSO-1.2.1.tar", last modified: Mon Mar 18 16:57:41 2024, max compression
+gzip compressed data, was "spomso-1.2.2.tar", last modified: Wed Apr 17 13:53:22 2024, max compression
```

## Comparing `SPOMSO-1.2.1.tar` & `spomso-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     7652 2023-07-06 11:30:39.000000 SPOMSO-1.2.1/LICENSE
--rw-rw-r--   0 ropac     (1000) ropac     (1000)      629 2023-07-06 11:30:39.000000 SPOMSO-1.2.1/LICENSE_NOTICE
--rw-r--r--   0 ropac     (1000) ropac     (1000)      558 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/PKG-INFO
-drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/SPOMSO.egg-info/
--rw-r--r--   0 ropac     (1000) ropac     (1000)      558 2024-03-18 16:57:41.000000 SPOMSO-1.2.1/SPOMSO.egg-info/PKG-INFO
--rw-rw-r--   0 ropac     (1000) ropac     (1000)      808 2024-03-18 16:57:41.000000 SPOMSO-1.2.1/SPOMSO.egg-info/SOURCES.txt
--rw-rw-r--   0 ropac     (1000) ropac     (1000)        1 2024-03-18 16:57:41.000000 SPOMSO-1.2.1/SPOMSO.egg-info/dependency_links.txt
--rw-rw-r--   0 ropac     (1000) ropac     (1000)       12 2024-03-18 16:57:41.000000 SPOMSO-1.2.1/SPOMSO.egg-info/requires.txt
--rw-rw-r--   0 ropac     (1000) ropac     (1000)        7 2024-03-18 16:57:41.000000 SPOMSO-1.2.1/SPOMSO.egg-info/top_level.txt
--rw-rw-r--   0 ropac     (1000) ropac     (1000)       38 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/setup.cfg
--rw-rw-r--   0 ropac     (1000) ropac     (1000)      749 2024-03-18 16:56:50.000000 SPOMSO-1.2.1/setup.py
-drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/spomso/
--rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 SPOMSO-1.2.1/spomso/__init__.py
-drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/spomso/cores/
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     4598 2024-03-11 16:50:22.000000 SPOMSO-1.2.1/spomso/cores/__init__.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     7719 2024-03-12 15:02:17.000000 SPOMSO-1.2.1/spomso/cores/combine.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    14458 2024-03-12 15:02:17.000000 SPOMSO-1.2.1/spomso/cores/geom.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    19859 2024-03-13 10:21:02.000000 SPOMSO-1.2.1/spomso/cores/geom_2d.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    23533 2024-03-13 10:22:51.000000 SPOMSO-1.2.1/spomso/cores/geom_3d.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     1371 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/geom_core_2d_direct.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     2062 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/geom_core_3d_direct.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     8225 2024-03-12 12:38:00.000000 SPOMSO-1.2.1/spomso/cores/geom_vector.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     4795 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/geom_vector_special.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     7282 2024-03-13 11:18:36.000000 SPOMSO-1.2.1/spomso/cores/helper_functions.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    59146 2024-03-12 15:02:17.000000 SPOMSO-1.2.1/spomso/cores/modifications.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    23003 2024-03-13 10:47:38.000000 SPOMSO-1.2.1/spomso/cores/post_processing.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     6947 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/sdf_2D.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     8747 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/sdf_3D.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)    16617 2024-03-15 14:26:24.000000 SPOMSO-1.2.1/spomso/cores/transformations.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     3393 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/vector_functions.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     6540 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/vector_functions_special.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)     4040 2024-01-08 11:04:38.000000 SPOMSO-1.2.1/spomso/cores/vector_modification_functions.py
-drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-03-18 16:57:41.631046 SPOMSO-1.2.1/spomso/jax_cores/
--rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 SPOMSO-1.2.1/spomso/jax_cores/__init__.py
--rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 SPOMSO-1.2.1/spomso/jax_cores/sdf_core_jax.py
+drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-04-17 13:53:22.734432 spomso-1.2.2/
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     7652 2023-07-06 11:30:39.000000 spomso-1.2.2/LICENSE
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)      629 2023-07-06 11:30:39.000000 spomso-1.2.2/LICENSE_NOTICE
+-rw-r--r--   0 ropac     (1000) ropac     (1000)      553 2024-04-17 13:53:22.734432 spomso-1.2.2/PKG-INFO
+drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-04-17 13:53:22.734432 spomso-1.2.2/SPOMSO.egg-info/
+-rw-r--r--   0 ropac     (1000) ropac     (1000)      553 2024-04-17 13:53:22.000000 spomso-1.2.2/SPOMSO.egg-info/PKG-INFO
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)      808 2024-04-17 13:53:22.000000 spomso-1.2.2/SPOMSO.egg-info/SOURCES.txt
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)        1 2024-04-17 13:53:22.000000 spomso-1.2.2/SPOMSO.egg-info/dependency_links.txt
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)       12 2024-04-17 13:53:22.000000 spomso-1.2.2/SPOMSO.egg-info/requires.txt
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)        7 2024-04-17 13:53:22.000000 spomso-1.2.2/SPOMSO.egg-info/top_level.txt
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)       38 2024-04-17 13:53:22.734432 spomso-1.2.2/setup.cfg
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)      744 2024-04-17 13:18:35.000000 spomso-1.2.2/setup.py
+drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-04-17 13:53:22.734432 spomso-1.2.2/spomso/
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 spomso-1.2.2/spomso/__init__.py
+drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-04-17 13:53:22.734432 spomso-1.2.2/spomso/cores/
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     4598 2024-03-11 16:50:22.000000 spomso-1.2.2/spomso/cores/__init__.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     7719 2024-03-12 15:02:17.000000 spomso-1.2.2/spomso/cores/combine.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    14460 2024-04-17 11:58:43.000000 spomso-1.2.2/spomso/cores/geom.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    19859 2024-03-13 10:21:02.000000 spomso-1.2.2/spomso/cores/geom_2d.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    23533 2024-03-13 10:22:51.000000 spomso-1.2.2/spomso/cores/geom_3d.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     1371 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/geom_core_2d_direct.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     2062 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/geom_core_3d_direct.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     8225 2024-03-12 12:38:00.000000 spomso-1.2.2/spomso/cores/geom_vector.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     4795 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/geom_vector_special.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     7282 2024-03-13 11:18:36.000000 spomso-1.2.2/spomso/cores/helper_functions.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    59146 2024-03-12 15:02:17.000000 spomso-1.2.2/spomso/cores/modifications.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    23003 2024-03-13 10:47:38.000000 spomso-1.2.2/spomso/cores/post_processing.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     6947 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/sdf_2D.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     8747 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/sdf_3D.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)    16617 2024-03-15 14:26:24.000000 spomso-1.2.2/spomso/cores/transformations.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     3393 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/vector_functions.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     6540 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/vector_functions_special.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)     4040 2024-01-08 11:04:38.000000 spomso-1.2.2/spomso/cores/vector_modification_functions.py
+drwxrwxr-x   0 ropac     (1000) ropac     (1000)        0 2024-04-17 13:53:22.734432 spomso-1.2.2/spomso/jax_cores/
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 spomso-1.2.2/spomso/jax_cores/__init__.py
+-rw-rw-r--   0 ropac     (1000) ropac     (1000)        0 2023-06-26 12:19:36.000000 spomso-1.2.2/spomso/jax_cores/sdf_core_jax.py
```

### Comparing `SPOMSO-1.2.1/LICENSE` & `spomso-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/LICENSE_NOTICE` & `spomso-1.2.2/LICENSE_NOTICE`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/PKG-INFO` & `spomso-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SPOMSO
-Version: 1.2.1
+Version: 1.2.2
 Summary: SPOMSO
-Home-page: https://github.com/peterropac/Aegolius/tree/main/Code
+Home-page: https://github.com/peterropac/Aegolius/tree/main
 Author: Peter Ropač
 Author-email: <peter.ropac@fmf.uni-lj.si>
 Keywords: python,geometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `SPOMSO-1.2.1/SPOMSO.egg-info/PKG-INFO` & `spomso-1.2.2/SPOMSO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SPOMSO
-Version: 1.2.1
+Version: 1.2.2
 Summary: SPOMSO
-Home-page: https://github.com/peterropac/Aegolius/tree/main/Code
+Home-page: https://github.com/peterropac/Aegolius/tree/main
 Author: Peter Ropač
 Author-email: <peter.ropac@fmf.uni-lj.si>
 Keywords: python,geometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `SPOMSO-1.2.1/SPOMSO.egg-info/SOURCES.txt` & `spomso-1.2.2/SPOMSO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/setup.py` & `spomso-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 DESCRIPTION = 'SPOMSO'
 LONG_DESCRIPTION = 'Python package for generating geometry with SDFs.'
 
 # Setting up
 setup(
     name="SPOMSO",
     version=VERSION,
     author="Peter Ropač",
     author_email="<peter.ropac@fmf.uni-lj.si>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    url='https://github.com/peterropac/Aegolius/tree/main/Code',
+    url='https://github.com/peterropac/Aegolius/tree/main',
     packages=find_packages(),
     install_requires=['numpy', 'scipy'],
     keywords=['python', 'geometry'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
```

### Comparing `SPOMSO-1.2.1/spomso/cores/__init__.py` & `spomso-1.2.2/spomso/cores/__init__.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/combine.py` & `spomso-1.2.2/spomso/cores/combine.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom.py` & `spomso-1.2.2/spomso/cores/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 D - number of dimensions (2,3);
                 N - number of points in the point cloud.
 
         Returns:
             Signed Distance Field of shape (N,).
         """
         self._sdf = self.modified_object
-        return self.apply(self._sdf, co, self.geo_parameters)
+        return self.apply(self._sdf, co, self._geo_parameters)
 
     def propagate(self, co: np.ndarray, *parameters_: tuple) -> np.ndarray:
         """
         Applies the modifications and transformations (in that order) to the SDF and returns the map of the
         Signed Distance Field. Similar to create but is meant to be used as input to construct new geometry.
 
         Args:
@@ -53,15 +53,15 @@
                 N - number of points in the point cloud.
             parameters_: can be empty
 
         Returns:
             Signed Distance Field of shape (N,).
         """
         self._sdf = self.modified_object
-        return self.apply(self._sdf, co, self.geo_parameters)
+        return self.apply(self._sdf, co, self._geo_parameters)
 
     def point_cloud(self, co: np.ndarray) -> np.ndarray:
         """Creates a point cloud from the interior points of the SDF.
 
         Args:
             co: Point cloud of coordinates (D, N);
         """
```

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_2d.py` & `spomso-1.2.2/spomso/cores/geom_2d.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_3d.py` & `spomso-1.2.2/spomso/cores/geom_3d.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_core_2d_direct.py` & `spomso-1.2.2/spomso/cores/geom_core_2d_direct.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_core_3d_direct.py` & `spomso-1.2.2/spomso/cores/geom_core_3d_direct.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_vector.py` & `spomso-1.2.2/spomso/cores/geom_vector.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/geom_vector_special.py` & `spomso-1.2.2/spomso/cores/geom_vector_special.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/helper_functions.py` & `spomso-1.2.2/spomso/cores/helper_functions.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/modifications.py` & `spomso-1.2.2/spomso/cores/modifications.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/post_processing.py` & `spomso-1.2.2/spomso/cores/post_processing.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/sdf_2D.py` & `spomso-1.2.2/spomso/cores/sdf_2D.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/sdf_3D.py` & `spomso-1.2.2/spomso/cores/sdf_3D.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/transformations.py` & `spomso-1.2.2/spomso/cores/transformations.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/vector_functions.py` & `spomso-1.2.2/spomso/cores/vector_functions.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/vector_functions_special.py` & `spomso-1.2.2/spomso/cores/vector_functions_special.py`

 * *Files identical despite different names*

### Comparing `SPOMSO-1.2.1/spomso/cores/vector_modification_functions.py` & `spomso-1.2.2/spomso/cores/vector_modification_functions.py`

 * *Files identical despite different names*

