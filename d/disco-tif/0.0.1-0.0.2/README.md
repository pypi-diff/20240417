# Comparing `tmp/disco-tif-0.0.1.tar.gz` & `tmp/disco-tif-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disco-tif-0.0.1.tar", last modified: Wed Apr 17 09:06:58 2024, max compression
+gzip compressed data, was "disco-tif-0.0.2.tar", last modified: Wed Apr 17 13:30:45 2024, max compression
```

## Comparing `disco-tif-0.0.1.tar` & `disco-tif-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 09:06:58.669588 disco-tif-0.0.1/
--rw-r--r--   0 bbloss     (501) staff       (20)       52 2024-04-17 07:44:12.000000 disco-tif-0.0.1/HISTORY.md
--rw-r--r--   0 bbloss     (501) staff       (20)      177 2024-04-17 08:10:11.000000 disco-tif-0.0.1/MANIFEST.in
--rw-r--r--   0 bbloss     (501) staff       (20)      426 2024-04-17 09:06:58.669371 disco-tif-0.0.1/PKG-INFO
--rw-r--r--   0 bbloss     (501) staff       (20)      408 2024-04-17 08:06:49.000000 disco-tif-0.0.1/README.md
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 09:06:58.667446 disco-tif-0.0.1/disco_tif/
--rw-r--r--   0 bbloss     (501) staff       (20)        0 2024-04-16 12:56:23.000000 disco-tif-0.0.1/disco_tif/__init__.py
--rw-r--r--   0 bbloss     (501) staff       (20)     1980 2024-04-16 13:04:31.000000 disco-tif-0.0.1/disco_tif/geotiff_plotting.py
--rw-r--r--   0 bbloss     (501) staff       (20)     8979 2024-04-16 16:04:04.000000 disco-tif-0.0.1/disco_tif/hillshades_pca.py
--rw-r--r--   0 bbloss     (501) staff       (20)    18863 2024-04-16 13:27:45.000000 disco-tif-0.0.1/disco_tif/process_sb_tiff.py
--rw-r--r--   0 bbloss     (501) staff       (20)     8901 2024-04-16 13:18:49.000000 disco-tif-0.0.1/disco_tif/write_mapfile.py
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 09:06:58.669032 disco-tif-0.0.1/disco_tif.egg-info/
--rw-r--r--   0 bbloss     (501) staff       (20)      426 2024-04-17 09:06:58.000000 disco-tif-0.0.1/disco_tif.egg-info/PKG-INFO
--rw-r--r--   0 bbloss     (501) staff       (20)      341 2024-04-17 09:06:58.000000 disco-tif-0.0.1/disco_tif.egg-info/SOURCES.txt
--rw-r--r--   0 bbloss     (501) staff       (20)        1 2024-04-17 09:06:58.000000 disco-tif-0.0.1/disco_tif.egg-info/dependency_links.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       62 2024-04-17 09:06:58.000000 disco-tif-0.0.1/disco_tif.egg-info/requires.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       10 2024-04-17 09:06:58.000000 disco-tif-0.0.1/disco_tif.egg-info/top_level.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       38 2024-04-17 09:06:58.669628 disco-tif-0.0.1/setup.cfg
--rw-r--r--   0 bbloss     (501) staff       (20)      783 2024-04-17 09:05:24.000000 disco-tif-0.0.1/setup.py
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.740183 disco-tif-0.0.2/
+-rw-r--r--   0 bbloss     (501) staff       (20)      157 2024-04-17 13:28:35.000000 disco-tif-0.0.2/HISTORY.md
+-rw-r--r--   0 bbloss     (501) staff       (20)     1077 2024-04-17 12:41:43.000000 disco-tif-0.0.2/LICENSE.md
+-rw-r--r--   0 bbloss     (501) staff       (20)      177 2024-04-17 08:10:11.000000 disco-tif-0.0.2/MANIFEST.in
+-rw-r--r--   0 bbloss     (501) staff       (20)      502 2024-04-17 13:30:45.739960 disco-tif-0.0.2/PKG-INFO
+-rw-r--r--   0 bbloss     (501) staff       (20)     5149 2024-04-17 13:23:53.000000 disco-tif-0.0.2/README.md
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.738670 disco-tif-0.0.2/disco_tif/
+-rw-r--r--   0 bbloss     (501) staff       (20)        0 2024-04-16 12:56:23.000000 disco-tif-0.0.2/disco_tif/__init__.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     1980 2024-04-16 13:04:31.000000 disco-tif-0.0.2/disco_tif/geotiff_plotting.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     8979 2024-04-16 16:04:04.000000 disco-tif-0.0.2/disco_tif/hillshades_pca.py
+-rw-r--r--   0 bbloss     (501) staff       (20)    19512 2024-04-17 12:13:28.000000 disco-tif-0.0.2/disco_tif/process_sb_tiff.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     8901 2024-04-16 13:18:49.000000 disco-tif-0.0.2/disco_tif/write_mapfile.py
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.739710 disco-tif-0.0.2/disco_tif.egg-info/
+-rw-r--r--   0 bbloss     (501) staff       (20)      502 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/PKG-INFO
+-rw-r--r--   0 bbloss     (501) staff       (20)      352 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/SOURCES.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)        1 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/dependency_links.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       62 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/requires.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       10 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/top_level.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       38 2024-04-17 13:30:45.740232 disco-tif-0.0.2/setup.cfg
+-rw-r--r--   0 bbloss     (501) staff       (20)      855 2024-04-17 13:29:39.000000 disco-tif-0.0.2/setup.py
```

### Comparing `disco-tif-0.0.1/disco_tif/geotiff_plotting.py` & `disco-tif-0.0.2/disco_tif/geotiff_plotting.py`

 * *Files identical despite different names*

### Comparing `disco-tif-0.0.1/disco_tif/hillshades_pca.py` & `disco-tif-0.0.2/disco_tif/hillshades_pca.py`

 * *Files identical despite different names*

### Comparing `disco-tif-0.0.1/disco_tif/process_sb_tiff.py` & `disco-tif-0.0.2/disco_tif/process_sb_tiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,48 +249,61 @@
 def make_rgba_tiff_from_single_Band(single_band_tiff_path, 
                                     data_min_max=None, 
                                     min_max_method='percentile', 
                                     clip_perc=[1, 99], 
                                     color_palette_name=None, 
                                     cmap_method='pseudo_hist_norm',
                                     output_tif=False,
+                                    generate_lookup_tables=False,
                                     plot_rgba_raster=False,
                                    ):
     '''Function to take a single band geotiff file, apply a colormap to the data, and write a rgba geotiff to file
 
 Input parameters:
  - single_band_tiff_path: 
      complete path to single-band-geotiff
 
  - data_min_max: 
      default = None
      Can take a list of lenth: 2, ex: [0, 500]
-     This function will automatically apply min/max values based on the 1 and 99 percentiles of the data values (excluding no-data values).
+     if not spcified, this function will automatically apply min/max values based on the clip_perc values
  
  - min_max_method:
-     default = 'percentile'
+     default = 'percentile'; only relevant if data_min_max==None.
      Also accepts 'data_absolute'. 
      'percentile' uses the percentiles used in clip_perc. 
      'data_absolute' uses the minimum and maximum values of the data
  
  - clip_perc
-     default = [1, 99]
+     default = [1, 99]; only relevant if data_min_max==None.
      Percentile values to clip the data values to if no data_min_max is specified.
  
  - color_palette_name
      default = None
      Desired color pallet based on matplotlib colormaps. 
      https://matplotlib.org/stable/users/explain/colors/colormaps.html
      If None, the funtion will automatically create a new "EMerald_Custom_Colormap"
  
  - cmap_method:
      defualt = 'pseudo_hist_norm'
      Method to determine where the color breaks should be. Also accepts 'pseudo_linear'
      'pseudo_hist_norm' will produce a linear colormap for data values below 0 and a histogram normalized colormap for the positive values
      'pseudo_linear' will produce a linear colormap for data values below 0 and a separate linear colormap for the positive values.
+
+ - output_tif:
+     default = False
+     If new geotiff are desired as outputs this must be set to True
+
+ - generate_lookup_tables:
+     defaule = False
+     If set to True look up tables will be generated and written to file. This includes a look up table that can be applied to the single-band geotiff in QGIS and maybe other GIS software.
+
+ - plot_rgba_raster
+     default=False
+     If set to True this will generate new matplotlib figures.
     '''
 
     if data_min_max is not None:
         assert len(data_min_max)==2, "len of data_min_max must be 2"
         assert data_min_max[0] < data_min_max[1], "first value must be less than second value"
         assert data_min_max[1] > 0, "This should really be a bigger number, but at least this will save dividing by a zero..."
     assert len(clip_perc)==2, "len of data_min_max must be 2"
@@ -355,32 +368,33 @@
         ep.plot_bands(clipped_data_with_nan,
                       cmap = EMeraldCustomColormap,
                       title=f"{sbpath.split(os.path.sep)[-1]}\n{suffix.replace('_', ' ')}",
                       ax=ax,
                      )
         plt.tight_layout()
         plt.show()    
-    
-    outfilepaths = build_1_component_color_tables(cmap=EMerald_custom_colors_hexcolorcodes,
-                                                  data_breaks=data_breaks,
-                                                  data=data,
-                                                  no_data_value=no_data_value,
-                                                  new_multiband_lut_path=new_multiband_lut_path )
-    for fp in outfilepaths:
-        print(f"Wrote 1component LUT files to: '{fp}'")
-
-    outfilepaths = build_4_component_color_tables(single_band_tiff_path=single_band_tiff_path,
-                                                  cmap=EMeraldCustomColormap,
-                                                  data=data,
-                                                  no_data_value=no_data_value,
-                                                  percentile_breaks=percentile_breaks,
-                                                  data_breaks=data_breaks,
-                                                  outfile=new_multiband_tiff_path)
-    for fp in outfilepaths:
-        print(f"wrote 4component Lut files to: '{fp}''")
+
+    if generate_lookup_tables:
+        outfilepaths = build_1_component_color_tables(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                      data_breaks=data_breaks,
+                                                      data=data,
+                                                      no_data_value=no_data_value,
+                                                      new_multiband_lut_path=new_multiband_lut_path )
+        for fp in outfilepaths:
+            print(f"Wrote 1component LUT files to: '{fp}'")
+    
+        outfilepaths = build_4_component_color_tables(single_band_tiff_path=single_band_tiff_path,
+                                                      cmap=EMeraldCustomColormap,
+                                                      data=data,
+                                                      no_data_value=no_data_value,
+                                                      percentile_breaks=percentile_breaks,
+                                                      data_breaks=data_breaks,
+                                                      outfile=new_multiband_tiff_path)
+        for fp in outfilepaths:
+            print(f"wrote 4component Lut files to: '{fp}''")
     
     if output_tif:
         # apply EMeraldCustomColormap to data
         rgba_data = EMeraldCustomColormap(normalized_data) * (colormap_length-1)  # Scale to 0-255 range
         
         # 3. Convert to RGB Channels:
         rgb_data = rgba_data[:, :, :3]  # Extract RGB channels
```

### Comparing `disco-tif-0.0.1/disco_tif/write_mapfile.py` & `disco-tif-0.0.2/disco_tif/write_mapfile.py`

 * *Files identical despite different names*

### Comparing `disco-tif-0.0.1/setup.py` & `disco-tif-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 
 import os,sys
 from setuptools import setup, find_packages
 
 setup(name = 'disco-tif',
-      version = "0.0.1",
+      version = "0.0.2",
       url = 'https://github.com/emerald-geomodelling/disco-tif',
       author = "Benjamin Bloss",
       author_email = 'bb@emrld.no',
       description = "Geotiff processing utilities",
       install_requires = ["seaborn",
                           "rasterio",
                           "numpy",
                           "pandas",
                           "matplotlib",
                           "earthpy",
                           "scikit-learn",
                          ],
       long_description = "Geotiff processing utilities",
       include_package_data = True,
-      keywords = 'raster_processing',
+      keywords = ['raster_processing', 'EMerald_custom_colormap', 'hillshade', 'pca'],
+      license = 'MIT',
       packages = find_packages(),
      )
```

