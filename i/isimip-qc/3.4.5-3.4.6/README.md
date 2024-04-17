# Comparing `tmp/isimip-qc-3.4.5.tar.gz` & `tmp/isimip_qc-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isimip-qc-3.4.5.tar", last modified: Tue Mar 12 12:42:35 2024, max compression
+gzip compressed data, was "isimip_qc-3.4.6.tar", last modified: Wed Apr 17 07:38:48 2024, max compression
```

## Comparing `isimip-qc-3.4.5.tar` & `isimip_qc-3.4.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.341166 isimip-qc-3.4.5/
--rw-r--r--   0 buechner  (2091) users      (100)     1102 2023-09-20 09:43:17.000000 isimip-qc-3.4.5/LICENSE
--rw-r--r--   0 buechner  (2091) users      (100)    14134 2024-03-12 12:42:35.338169 isimip-qc-3.4.5/PKG-INFO
--rw-r--r--   0 buechner  (2091) users      (100)    11734 2024-03-12 12:40:02.000000 isimip-qc-3.4.5/README.md
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.323861 isimip-qc-3.4.5/isimip_qc/
--rw-r--r--   0 buechner  (2091) users      (100)       32 2024-03-12 12:40:31.000000 isimip-qc-3.4.5/isimip_qc/__init__.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.293167 isimip-qc-3.4.5/isimip_qc/checks/
--rw-r--r--   0 buechner  (2091) users      (100)     3912 2024-01-31 09:45:49.000000 isimip-qc-3.4.5/isimip_qc/checks/3d.py
--rw-r--r--   0 buechner  (2091) users      (100)      769 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/checks/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)     4127 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/checks/attributes.py
--rw-r--r--   0 buechner  (2091) users      (100)     2954 2024-02-02 12:22:43.000000 isimip-qc-3.4.5/isimip_qc/checks/dataset.py
--rw-r--r--   0 buechner  (2091) users      (100)     5304 2023-09-26 11:45:52.000000 isimip-qc-3.4.5/isimip_qc/checks/dimensions.py
--rw-r--r--   0 buechner  (2091) users      (100)      709 2024-03-12 12:40:02.000000 isimip-qc-3.4.5/isimip_qc/checks/experiments.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.314166 isimip-qc-3.4.5/isimip_qc/checks/variables/
--rw-r--r--   0 buechner  (2091) users      (100)        0 2023-09-20 09:43:17.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)     7072 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/latlon.py
--rw-r--r--   0 buechner  (2091) users      (100)     6918 2023-09-21 13:03:19.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/time.py
--rw-r--r--   0 buechner  (2091) users      (100)     5151 2023-09-21 13:03:19.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/time_resolution.py
--rw-r--r--   0 buechner  (2091) users      (100)    14373 2024-02-02 12:30:57.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/var.py
--rw-r--r--   0 buechner  (2091) users      (100)     5397 2023-11-24 12:37:07.000000 isimip-qc-3.4.5/isimip_qc/checks/variables/var3d.py
--rw-r--r--   0 buechner  (2091) users      (100)     2022 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/config.py
--rw-r--r--   0 buechner  (2091) users      (100)      524 2023-09-20 09:43:17.000000 isimip-qc-3.4.5/isimip_qc/exceptions.py
--rw-r--r--   0 buechner  (2091) users      (100)     1692 2023-09-20 09:43:17.000000 isimip-qc-3.4.5/isimip_qc/fixes.py
--rw-r--r--   0 buechner  (2091) users      (100)    10335 2024-03-12 12:40:02.000000 isimip-qc-3.4.5/isimip_qc/main.py
--rw-r--r--   0 buechner  (2091) users      (100)    10181 2023-09-28 10:34:22.000000 isimip-qc-3.4.5/isimip_qc/models.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.374531 isimip-qc-3.4.5/isimip_qc/utils/
--rw-r--r--   0 buechner  (2091) users      (100)        0 2023-09-20 09:43:17.000000 isimip-qc-3.4.5/isimip_qc/utils/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)      360 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/utils/datamodel.py
--rw-r--r--   0 buechner  (2091) users      (100)     1123 2023-09-28 10:34:22.000000 isimip-qc-3.4.5/isimip_qc/utils/experiments.py
--rw-r--r--   0 buechner  (2091) users      (100)     1345 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/utils/files.py
--rw-r--r--   0 buechner  (2091) users      (100)      224 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/isimip_qc/utils/logging.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-03-12 12:42:35.334166 isimip-qc-3.4.5/isimip_qc.egg-info/
--rw-r--r--   0 buechner  (2091) users      (100)    14134 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/PKG-INFO
--rw-r--r--   0 buechner  (2091) users      (100)      896 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/SOURCES.txt
--rw-r--r--   0 buechner  (2091) users      (100)        1 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/dependency_links.txt
--rw-r--r--   0 buechner  (2091) users      (100)       50 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/entry_points.txt
--rw-r--r--   0 buechner  (2091) users      (100)      116 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/requires.txt
--rw-r--r--   0 buechner  (2091) users      (100)       10 2024-03-12 12:42:35.000000 isimip-qc-3.4.5/isimip_qc.egg-info/top_level.txt
--rw-r--r--   0 buechner  (2091) users      (100)     1953 2023-09-21 12:43:01.000000 isimip-qc-3.4.5/pyproject.toml
--rw-r--r--   0 buechner  (2091) users      (100)       38 2024-03-12 12:42:35.341172 isimip-qc-3.4.5/setup.cfg
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.528978 isimip_qc-3.4.6/
+-rw-r--r--   0 buechner  (2091) users      (100)     1102 2023-09-20 09:43:17.000000 isimip_qc-3.4.6/LICENSE
+-rw-r--r--   0 buechner  (2091) users      (100)    14134 2024-04-17 07:38:48.524981 isimip_qc-3.4.6/PKG-INFO
+-rw-r--r--   0 buechner  (2091) users      (100)    11734 2024-03-12 12:40:02.000000 isimip_qc-3.4.6/README.md
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.442978 isimip_qc-3.4.6/isimip_qc/
+-rw-r--r--   0 buechner  (2091) users      (100)       32 2024-04-17 07:35:27.000000 isimip_qc-3.4.6/isimip_qc/__init__.py
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.480979 isimip_qc-3.4.6/isimip_qc/checks/
+-rw-r--r--   0 buechner  (2091) users      (100)     3912 2024-01-31 09:45:49.000000 isimip_qc-3.4.6/isimip_qc/checks/3d.py
+-rw-r--r--   0 buechner  (2091) users      (100)      769 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/checks/__init__.py
+-rw-r--r--   0 buechner  (2091) users      (100)     4127 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/checks/attributes.py
+-rw-r--r--   0 buechner  (2091) users      (100)     2954 2024-02-02 12:22:43.000000 isimip_qc-3.4.6/isimip_qc/checks/dataset.py
+-rw-r--r--   0 buechner  (2091) users      (100)     5304 2023-09-26 11:45:52.000000 isimip_qc-3.4.6/isimip_qc/checks/dimensions.py
+-rw-r--r--   0 buechner  (2091) users      (100)      709 2024-03-12 12:40:02.000000 isimip_qc-3.4.6/isimip_qc/checks/experiments.py
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.499980 isimip_qc-3.4.6/isimip_qc/checks/variables/
+-rw-r--r--   0 buechner  (2091) users      (100)        0 2023-09-20 09:43:17.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/__init__.py
+-rw-r--r--   0 buechner  (2091) users      (100)     6854 2024-04-17 07:33:50.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/latlon.py
+-rw-r--r--   0 buechner  (2091) users      (100)     6918 2023-09-21 13:03:19.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/time.py
+-rw-r--r--   0 buechner  (2091) users      (100)     5151 2023-09-21 13:03:19.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/time_resolution.py
+-rw-r--r--   0 buechner  (2091) users      (100)    14373 2024-02-02 12:30:57.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/var.py
+-rw-r--r--   0 buechner  (2091) users      (100)     5397 2023-11-24 12:37:07.000000 isimip_qc-3.4.6/isimip_qc/checks/variables/var3d.py
+-rw-r--r--   0 buechner  (2091) users      (100)     2022 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/config.py
+-rw-r--r--   0 buechner  (2091) users      (100)      524 2023-09-20 09:43:17.000000 isimip_qc-3.4.6/isimip_qc/exceptions.py
+-rw-r--r--   0 buechner  (2091) users      (100)     1692 2023-09-20 09:43:17.000000 isimip_qc-3.4.6/isimip_qc/fixes.py
+-rw-r--r--   0 buechner  (2091) users      (100)    10335 2024-03-12 12:40:02.000000 isimip_qc-3.4.6/isimip_qc/main.py
+-rw-r--r--   0 buechner  (2091) users      (100)    10181 2023-09-28 10:34:22.000000 isimip_qc-3.4.6/isimip_qc/models.py
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.516979 isimip_qc-3.4.6/isimip_qc/utils/
+-rw-r--r--   0 buechner  (2091) users      (100)        0 2023-09-20 09:43:17.000000 isimip_qc-3.4.6/isimip_qc/utils/__init__.py
+-rw-r--r--   0 buechner  (2091) users      (100)      360 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/utils/datamodel.py
+-rw-r--r--   0 buechner  (2091) users      (100)     1123 2023-09-28 10:34:22.000000 isimip_qc-3.4.6/isimip_qc/utils/experiments.py
+-rw-r--r--   0 buechner  (2091) users      (100)     1345 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/utils/files.py
+-rw-r--r--   0 buechner  (2091) users      (100)      224 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/isimip_qc/utils/logging.py
+drwxr-xr-x   0 buechner  (2091) users      (100)        0 2024-04-17 07:38:48.520979 isimip_qc-3.4.6/isimip_qc.egg-info/
+-rw-r--r--   0 buechner  (2091) users      (100)    14134 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/PKG-INFO
+-rw-r--r--   0 buechner  (2091) users      (100)      896 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 buechner  (2091) users      (100)        1 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 buechner  (2091) users      (100)       50 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/entry_points.txt
+-rw-r--r--   0 buechner  (2091) users      (100)      116 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/requires.txt
+-rw-r--r--   0 buechner  (2091) users      (100)       10 2024-04-17 07:38:48.000000 isimip_qc-3.4.6/isimip_qc.egg-info/top_level.txt
+-rw-r--r--   0 buechner  (2091) users      (100)     1953 2023-09-21 12:43:01.000000 isimip_qc-3.4.6/pyproject.toml
+-rw-r--r--   0 buechner  (2091) users      (100)       38 2024-04-17 07:38:48.529978 isimip_qc-3.4.6/setup.cfg
```

### Comparing `isimip-qc-3.4.5/LICENSE` & `isimip_qc-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/PKG-INFO` & `isimip_qc-3.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimip-qc
-Version: 3.4.5
+Version: 3.4.6
 Summary: A command line tool for the quality control of climate impact data of the ISIMIP project.
 Author-email: Matthias Büchner <buechner@pik-potsdam.de>, Jochen Klar <jochen.klar@pik-potsdam.de>
 Maintainer-email: Matthias Büchner <buechner@pik-potsdam.de>
 License: MIT License
         
         Copyright (c) 2020 Potsdam Institute for Climate Impact Research
```

### Comparing `isimip-qc-3.4.5/README.md` & `isimip_qc-3.4.6/README.md`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/3d.py` & `isimip_qc-3.4.6/isimip_qc/checks/3d.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/__init__.py` & `isimip_qc-3.4.6/isimip_qc/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/attributes.py` & `isimip_qc-3.4.6/isimip_qc/checks/attributes.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/dataset.py` & `isimip_qc-3.4.6/isimip_qc/checks/dataset.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/dimensions.py` & `isimip_qc-3.4.6/isimip_qc/checks/dimensions.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/experiments.py` & `isimip_qc-3.4.6/isimip_qc/checks/experiments.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/variables/latlon.py` & `isimip_qc-3.4.6/isimip_qc/checks/variables/latlon.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,18 +126,14 @@
                 if model == 'dbem':
                     if var.name == 'lat':
                         minimum = -89.75
                         maximum = 89.75
                     elif var.name == 'lon':
                         minimum = -179.75
                         maximum = 179.75
-                elif model == 'dbpm' or model == 'zoomss':
-                    if climate_forcing == 'ipsl-cm6a-lr' and var.name == 'lon':
-                        minimum = -180.
-                        maximum = 179.
 
                 if np.min(var) != minimum:
                     file.error('First value of variable "%s" is %s. Must be %s.', variable, np.min(var), minimum)
 
                 if np.max(var) != maximum:
                     file.error('Last value of variable "%s" is %s. Must be %s.', variable, np.max(var), maximum)
```

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/variables/time.py` & `isimip_qc-3.4.6/isimip_qc/checks/variables/time.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/variables/time_resolution.py` & `isimip_qc-3.4.6/isimip_qc/checks/variables/time_resolution.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/variables/var.py` & `isimip_qc-3.4.6/isimip_qc/checks/variables/var.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/checks/variables/var3d.py` & `isimip_qc-3.4.6/isimip_qc/checks/variables/var3d.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/config.py` & `isimip_qc-3.4.6/isimip_qc/config.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/exceptions.py` & `isimip_qc-3.4.6/isimip_qc/exceptions.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/fixes.py` & `isimip_qc-3.4.6/isimip_qc/fixes.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/main.py` & `isimip_qc-3.4.6/isimip_qc/main.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/models.py` & `isimip_qc-3.4.6/isimip_qc/models.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/utils/experiments.py` & `isimip_qc-3.4.6/isimip_qc/utils/experiments.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc/utils/files.py` & `isimip_qc-3.4.6/isimip_qc/utils/files.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/isimip_qc.egg-info/PKG-INFO` & `isimip_qc-3.4.6/isimip_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimip-qc
-Version: 3.4.5
+Version: 3.4.6
 Summary: A command line tool for the quality control of climate impact data of the ISIMIP project.
 Author-email: Matthias Büchner <buechner@pik-potsdam.de>, Jochen Klar <jochen.klar@pik-potsdam.de>
 Maintainer-email: Matthias Büchner <buechner@pik-potsdam.de>
 License: MIT License
         
         Copyright (c) 2020 Potsdam Institute for Climate Impact Research
```

### Comparing `isimip-qc-3.4.5/isimip_qc.egg-info/SOURCES.txt` & `isimip_qc-3.4.6/isimip_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.4.5/pyproject.toml` & `isimip_qc-3.4.6/pyproject.toml`

 * *Files identical despite different names*

