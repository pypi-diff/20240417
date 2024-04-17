# Comparing `tmp/esi-utils-pager-1.0.8.tar.gz` & `tmp/esi-utils-pager-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi-utils-pager-1.0.8.tar", last modified: Fri Oct 13 23:23:51 2023, max compression
+gzip compressed data, was "esi-utils-pager-1.0.9.tar", last modified: Fri Feb  9 19:42:00 2024, max compression
```

## Comparing `esi-utils-pager-1.0.8.tar` & `esi-utils-pager-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.965621 esi-utils-pager-1.0.8/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/LICENSE.md
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6784 2023-10-13 23:23:51.965621 esi-utils-pager-1.0.8/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3637 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1262 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-10-13 23:23:51.965621 esi-utils-pager-1.0.8/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.953621 esi-utils-pager-1.0.8/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.953621 esi-utils-pager-1.0.8/src/esi_utils_pager/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:22:01.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.957621 esi-utils-pager-1.0.8/src/esi_utils_pager/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2830 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/bin/pagerlite.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7810 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/calc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/country.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.965621 esi-utils-pager-1.0.8/src/esi_utils_pager/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/countries.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_casualty.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_casualty.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_collapse_mmi.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_inventory.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_inventory.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_workforce.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_workforce.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/econexposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    22938 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/emploss.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/exposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/growth.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/pandas_container.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2468 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2023-10-13 23:08:52.000000 esi-utils-pager-1.0.8/src/esi_utils_pager/semimodel.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-13 23:23:51.957621 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6784 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1363 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      289 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2023-10-13 23:23:51.000000 esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.944348 esi-utils-pager-1.0.9/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/LICENSE.md
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7121 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3982 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-02-09 19:42:00.944348 esi-utils-pager-1.0.9/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.916347 esi-utils-pager-1.0.9/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.924347 esi-utils-pager-1.0.9/src/esi_utils_pager/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:40:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.928347 esi-utils-pager-1.0.9/src/esi_utils_pager/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4454 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/bin/pagerlite.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7859 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/calc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/country.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/src/esi_utils_pager/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/countries.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/econexposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    22938 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/emploss.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/exposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/growth.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/pandas_container.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2468 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/semimodel.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7121 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1363 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/top_level.txt
```

### Comparing `esi-utils-pager-1.0.8/LICENSE.md` & `esi-utils-pager-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/PKG-INFO` & `esi-utils-pager-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.0.8
+Version: 1.0.9
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -56,15 +56,15 @@
 License-File: LICENSE.md
 Requires-Dist: esi-utils-io
 Requires-Dist: esi-utils-time
 Requires-Dist: fiona
 Requires-Dist: h5py
 Requires-Dist: mapio>=0.8.5
 Requires-Dist: numpy<2.0.0
-Requires-Dist: openpyxl<=3.0.10
+Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: PyYAML
 Requires-Dist: rasterio
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: xlrd
 Provides-Extra: dev
@@ -157,14 +157,22 @@
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
 (fatality/economic) PAGER model results to a tabular format. To see the help for this program:
 
 `pagerlite -h`
 
+There are three input modes for pagerlite:
+
+ - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
+ - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
+ - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+    (these files can be in sub-directories).
+
+
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.8/README.md` & `esi-utils-pager-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,22 @@
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
 (fatality/economic) PAGER model results to a tabular format. To see the help for this program:
 
 `pagerlite -h`
 
+There are three input modes for pagerlite:
+
+ - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
+ - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
+ - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+    (these files can be in sub-directories).
+
+
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.8/pyproject.toml` & `esi-utils-pager-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 dependencies = [
     "esi-utils-io",
     "esi-utils-time",
     "fiona",
     "h5py",
     "mapio>=0.8.5",
     "numpy<2.0.0",
-    "openpyxl<=3.0.10",
+    "openpyxl",
     "pandas",
     "PyYAML",
     "rasterio",
     "scipy",
     "shapely",
     "xlrd"
 ]
```

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/calc.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     expframe = pd.DataFrame(data=exp_rows)
     for key, value in master_row.items():
         expframe[key] = value
     allcols = expframe.columns
     remainder = set(allcols) - set(master_row.keys())
     newcols = list(master_row.keys()) + sorted(list(remainder))
-    expframe = expframe[newcols]
+    expframe = expframe[newcols].copy()
     maxmmi_array = []
     for _, row in expframe.iterrows():
         mmi_idx = row[headers] > 1000
         if not len(mmi_idx[mmi_idx].index):
             maxmmi_array.append(0)
             continue
         maxmmi_col = mmi_idx[mmi_idx].index[-1]
@@ -182,14 +182,15 @@
             final_frame["TotalSemiFatalities"] = btotal
             ecoframe = ecoframe.join(final_frame, on=["CountryCode"])
 
     return ecoframe
 
 
 def calc_pager_events(gridfolder, verbose, run_semi):
+    gridfolder = pathlib.Path(gridfolder)
     # read config file
     config = read_config()
     # Make sure grid.xml file exists
     if not gridfolder.is_dir():
         print(f"ShakeMap Grid folder {gridfolder} does not exist.")
         sys.exit(1)
```

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/config.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/config.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/country.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/country.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/countries.xlsx` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/countries.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/economy.xml` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/economy.xml`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/fatality.xml` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_casualty.hdf` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_casualty.xlsx` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_collapse_mmi.hdf` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_collapse_mmi.xlsx` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_inventory.hdf` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_inventory.xlsx` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_workforce.hdf` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/data/semi_workforce.xlsx` & `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/econexposure.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/econexposure.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/emploss.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/emploss.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/exposure.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/exposure.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/growth.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/growth.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/probs.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/probs.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager/semimodel.py` & `esi-utils-pager-1.0.9/src/esi_utils_pager/semimodel.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/PKG-INFO` & `esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.0.8
+Version: 1.0.9
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -56,15 +56,15 @@
 License-File: LICENSE.md
 Requires-Dist: esi-utils-io
 Requires-Dist: esi-utils-time
 Requires-Dist: fiona
 Requires-Dist: h5py
 Requires-Dist: mapio>=0.8.5
 Requires-Dist: numpy<2.0.0
-Requires-Dist: openpyxl<=3.0.10
+Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: PyYAML
 Requires-Dist: rasterio
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: xlrd
 Provides-Extra: dev
@@ -157,14 +157,22 @@
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
 (fatality/economic) PAGER model results to a tabular format. To see the help for this program:
 
 `pagerlite -h`
 
+There are three input modes for pagerlite:
+
+ - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
+ - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
+ - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+    (these files can be in sub-directories).
+
+
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.8/src/esi_utils_pager.egg-info/SOURCES.txt` & `esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

