# Comparing `tmp/poreanalyser-0.0.4.tar.gz` & `tmp/poreanalyser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poreanalyser-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "poreanalyser-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `poreanalyser-0.0.4.tar` & `poreanalyser-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    26526 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/LICENSE
--rw-r--r--   0        0        0     7594 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py
--rw-r--r--   0        0        0    28702 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py
--rw-r--r--   0        0        0      821 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/conductance.py
--rw-r--r--   0        0        0     3909 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/download_files.py
--rwxr-xr-x   0        0        0  1962791 2024-04-09 22:27:30.353061 poreanalyser-0.0.4/PoreAnalyser/hole2/hole
--rwxr-xr-x   0        0        0    31085 2024-04-09 22:27:30.353061 poreanalyser-0.0.4/PoreAnalyser/hole2/sos_triangle
--rwxr-xr-x   0        0        0  2878646 2024-04-09 22:27:30.365061 poreanalyser-0.0.4/PoreAnalyser/hole2/sph_process
--rw-r--r--   0        0        0     8576 2024-04-09 22:27:30.365061 poreanalyser-0.0.4/PoreAnalyser/hole_analysis.py
--rw-r--r--   0        0        0  1315926 2024-04-09 22:27:30.369061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb
--rw-r--r--   0        0        0   294331 2024-04-09 22:27:30.373061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0  1153849 2024-04-09 22:27:30.377061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb
--rw-r--r--   0        0        0  1154174 2024-04-09 22:27:30.381061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb
--rw-r--r--   0        0        0   472405 2024-04-09 22:27:30.381061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb
--rw-r--r--   0        0        0   483623 2024-04-09 22:27:30.385061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb
--rw-r--r--   0        0        0   543505 2024-04-09 22:27:30.389061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb
--rw-r--r--   0        0        0   610576 2024-04-09 22:27:30.389061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb
--rw-r--r--   0        0        0   938821 2024-04-09 22:27:30.393061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb
--rw-r--r--   0        0        0  1122891 2024-04-09 22:27:30.397061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb
--rw-r--r--   0        0        0   255471 2024-04-09 22:27:30.397061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb
--rw-r--r--   0        0        0   353668 2024-04-09 22:27:30.401061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb
--rw-r--r--   0        0        0  1126446 2024-04-09 22:27:30.405061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb
--rw-r--r--   0        0        0   365834 2024-04-09 22:27:30.405061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb
--rw-r--r--   0        0        0   311491 2024-04-09 22:27:30.409061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0    16898 2024-04-09 22:27:30.409061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_pathway_ellipse.txt
--rw-r--r--   0        0        0  1126121 2024-04-09 22:27:30.413061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb
--rw-r--r--   0        0        0  1120916 2024-04-09 22:27:30.417061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi.pdb
--rw-r--r--   0        0        0    16497 2024-04-09 22:27:30.417061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi_aligned_z.pdb_pathway_ellipse.txt
--rw-r--r--   0        0        0  1275076 2024-04-09 22:27:30.421061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1.pdb
--rw-r--r--   0        0        0  1196534 2024-04-09 22:27:30.425061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb
--rw-r--r--   0        0        0  1196859 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb
--rw-r--r--   0        0        0   243451 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0    16047 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_pathway_ellipse.txt
--rw-r--r--   0        0        0    60805 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.s
--rw-r--r--   0        0        0  1196859 2024-04-09 22:27:30.437061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb
--rw-r--r--   0        0        0  1153849 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb
--rw-r--r--   0        0        0    59106 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph
--rw-r--r--   0        0        0    16086 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/poreanalyser.py
--rw-r--r--   0        0        0      361 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/__init__.py
--rw-r--r--   0        0        0     2251 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/test_conductance.py
--rw-r--r--   0        0        0     3372 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipse.py
--rw-r--r--   0        0        0     4204 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipsoid_optimisation.py
--rw-r--r--   0        0        0     1198 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_hole.py
--rw-r--r--   0        0        0      345 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_visualization.py
--rw-r--r--   0        0        0    16323 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/visualization.py
--rw-r--r--   0        0        0     4765 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/README.md
--rw-r--r--   0        0        0      764 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      321 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/requirements.txt
--rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 poreanalyser-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7594 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py
+-rw-r--r--   0        0        0    28702 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py
+-rw-r--r--   0        0        0      821 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/PoreAnalyser/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/PoreAnalyser/conductance.py
+-rw-r--r--   0        0        0     4091 2024-04-17 15:18:14.255057 poreanalyser-0.0.5/PoreAnalyser/download_files.py
+-rwxr-xr-x   0        0        0  1962791 2024-04-17 15:18:14.267057 poreanalyser-0.0.5/PoreAnalyser/hole2/hole
+-rwxr-xr-x   0        0        0    31085 2024-04-17 15:18:14.267057 poreanalyser-0.0.5/PoreAnalyser/hole2/sos_triangle
+-rwxr-xr-x   0        0        0  2878646 2024-04-17 15:18:14.279057 poreanalyser-0.0.5/PoreAnalyser/hole2/sph_process
+-rw-r--r--   0        0        0     8576 2024-04-17 15:18:14.279057 poreanalyser-0.0.5/PoreAnalyser/hole_analysis.py
+-rw-r--r--   0        0        0  1315926 2024-04-17 15:18:14.283057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9.pdb
+-rw-r--r--   0        0        0   294331 2024-04-17 15:18:14.287057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0  1153849 2024-04-17 15:18:14.291057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb
+-rw-r--r--   0        0        0  1154174 2024-04-17 15:18:14.295057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb
+-rw-r--r--   0        0        0   472405 2024-04-17 15:18:14.295057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb
+-rw-r--r--   0        0        0   483623 2024-04-17 15:18:14.299057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb
+-rw-r--r--   0        0        0   543505 2024-04-17 15:18:14.299057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb
+-rw-r--r--   0        0        0   610576 2024-04-17 15:18:14.303057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb
+-rw-r--r--   0        0        0   938821 2024-04-17 15:18:14.307057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb
+-rw-r--r--   0        0        0  1122891 2024-04-17 15:18:14.311057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb
+-rw-r--r--   0        0        0   255471 2024-04-17 15:18:14.311057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb
+-rw-r--r--   0        0        0   353668 2024-04-17 15:18:14.315057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb
+-rw-r--r--   0        0        0  1126446 2024-04-17 15:18:14.319057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb
+-rw-r--r--   0        0        0   365834 2024-04-17 15:18:14.319057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb
+-rw-r--r--   0        0        0   311491 2024-04-17 15:18:14.319057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0    16898 2024-04-17 15:18:14.323057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0  1126121 2024-04-17 15:18:14.327057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb
+-rw-r--r--   0        0        0  1120916 2024-04-17 15:18:14.331057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tvi.pdb
+-rw-r--r--   0        0        0    16497 2024-04-17 15:18:14.331057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tvi_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0  1275076 2024-04-17 15:18:14.335057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1.pdb
+-rw-r--r--   0        0        0  1196534 2024-04-17 15:18:14.339057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb
+-rw-r--r--   0        0        0  1196859 2024-04-17 15:18:14.343057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb
+-rw-r--r--   0        0        0   243451 2024-04-17 15:18:14.347057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0    16047 2024-04-17 15:18:14.347057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0    60805 2024-04-17 15:18:14.347057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.s
+-rw-r--r--   0        0        0  1196859 2024-04-17 15:18:14.351057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb
+-rw-r--r--   0        0        0  1153849 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb
+-rw-r--r--   0        0        0    59106 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph
+-rw-r--r--   0        0        0    20618 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/poreanalyser.py
+-rw-r--r--   0        0        0      361 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/__init__.py
+-rw-r--r--   0        0        0     2251 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/test_conductance.py
+-rw-r--r--   0        0        0     3372 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/test_ellipse.py
+-rw-r--r--   0        0        0     4204 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/test_ellipsoid_optimisation.py
+-rw-r--r--   0        0        0     1198 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/test_hole.py
+-rw-r--r--   0        0        0      345 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/tests/test_visualization.py
+-rw-r--r--   0        0        0    15395 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/PoreAnalyser/visualization.py
+-rw-r--r--   0        0        0     4765 2024-04-17 15:18:14.355057 poreanalyser-0.0.5/README.md
+-rw-r--r--   0        0        0      779 2024-04-17 15:18:14.367057 poreanalyser-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      335 2024-04-17 15:18:14.367057 poreanalyser-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 poreanalyser-0.0.5/PKG-INFO
```

### Comparing `poreanalyser-0.0.4/LICENSE` & `poreanalyser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py` & `poreanalyser-0.0.5/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py` & `poreanalyser-0.0.5/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/__init__.py` & `poreanalyser-0.0.5/PoreAnalyser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 #from .hole_analysis import hole_analysis 
 #sys.path.append('ProbeParticleEllipsoid/')
 #from ellipsoid_optimisation import ellipsoid_optimisation as ellipsoid_analysis 
 #from visualization import write_pdb_with_pore_surface, plt_ellipsoid_pathway, pathway_visu, st_write_ellipsoid, write_pdb_with_ellipsoid_surface, example_xy_plane, compare_volume, render_visu
 #from download_files import download_output, download_Ellipsoid_output
 #from ellipsoid_optimisation import ellipsoid_pathway
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = 'David Seiferth'
 
 from .hole_analysis import hole_analysis
 
 import numpy as np
```

### Comparing `poreanalyser-0.0.4/PoreAnalyser/conductance.py` & `poreanalyser-0.0.5/PoreAnalyser/conductance.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/download_files.py` & `poreanalyser-0.0.5/PoreAnalyser/download_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
                     path_save, names ):
     # To zip entire directory use command “shutil.make_archive(“name”,”zip”, root_dir)
     # To select the files to zip use command “ZipFile.write(filename)”
     # shutil.make_archive('', 'zip', dir_name)
     with ZipFile("poreFinding_HOLE_output.zip", "w") as newzip:
             newzip.write(pdb_name+'.vmd')
             newzip.write("visualise_pathway_hole.tcl")
+            newzip.write("pymol_pore_visu.py")
+            newzip.write("chimera_pore.py")
             newzip.write(path_save + names[0] + '_circle.pdb')
             newzip.write(pdb_name+'.pdb')
             newzip.write("README.md")
             newzip.write("hole.out")
             newzip.write('hole_pathway_profile.csv')
             newzip.write(fn)
     with open("poreFinding_HOLE_output.zip", "rb") as file:
@@ -69,14 +71,16 @@
     # To zip entire directory use command “shutil.make_archive(“name”,”zip”, root_dir)
     # To select the files to zip use command “ZipFile.write(filename)”
     # shutil.make_archive('', 'zip', dir_name)
     with ZipFile("poreFinding_Ellipsoid_output.zip", "w") as newzip:
             ### vmd ###
             newzip.write(pdb_name+'.pdb_pathway_ellipse.vmd')
             newzip.write("visualise_pathway_hole.tcl")
+            newzip.write("pymol_pore_visu.py")
+            newzip.write("chimera_pore.py")
             ### pdb files ### 
             newzip.write(path_save + pdb_name + '.pdb_ellipsoid.pdb')
             newzip.write(pdb_name+'.pdb')
 
             newzip.write("README.md")
             newzip.write(pdb_name + '.pdb_pathway_ellipse.txt')
             newzip.write(fn)
```

### Comparing `poreanalyser-0.0.4/PoreAnalyser/hole2/hole` & `poreanalyser-0.0.5/PoreAnalyser/hole2/hole`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/hole2/sos_triangle` & `poreanalyser-0.0.5/PoreAnalyser/hole2/sos_triangle`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/hole2/sph_process` & `poreanalyser-0.0.5/PoreAnalyser/hole2/sph_process`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/hole_analysis.py` & `poreanalyser-0.0.5/PoreAnalyser/hole_analysis.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_pathway_ellipse.txt` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_pathway_ellipse.txt`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tvi.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi_aligned_z.pdb_pathway_ellipse.txt` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/7tvi_aligned_z.pdb_pathway_ellipse.txt`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_pathway_ellipse.txt` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_pathway_ellipse.txt`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.s` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z.s`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph` & `poreanalyser-0.0.5/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/poreanalyser.py` & `poreanalyser-0.0.5/PoreAnalyser/poreanalyser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 #bla = os.getcwd() + '/PoreFinding/'
 bla = os.path.realpath(__file__)[:-15] 
 print(bla)
 import sys
 sys.path.append(bla)
 import hole_analysis as hole_analysis
-from visualization import write_pdb_with_pore_surface, plt_ellipsoid_pathway, pathway_visu, st_write_ellipsoid, write_pdb_with_ellipsoid_surface, example_xy_plane, compare_volume, render_visu
+from visualization import write_pdb_with_pore_surface, plt_ellipsoid_pathway, pathway_visu, st_write_ellipsoid, write_pdb_with_ellipsoid_surface, example_xy_plane, compare_volume #, render_visu
 import MDAnalysis
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 try:
     import multiprocessing 
     print("Number of processors: ", multiprocessing.cpu_count())
@@ -38,14 +38,19 @@
     - D_cation (float, optional): Diffusion coefficient of the cation. Default is 1.8e-9 m^2/s (value for potassium).
     - D_anion (float, optional): Diffusion coefficient of the anion. Default is 2.032e-9 m^2/s (value for chloride).
     - popt (list, optional): Parameters for the conductivity model. Default is [1.40674664, 1.25040698].
         - popt[0] (float): Scaling parameter of radius for the conductivity model (dimension 1/Angstrom).
         - popt[1] (float): Shift parameter of the sigmoid function for the conductivity model (dimenionless).
     - temp (int, optional): Temperature in Kelvin. Default is 300.
     - c_m (float, optional): Concentration in mol/l. Default is 0.15.
+    - trajectory (bool, optional): Flag indicating whether the input is a trajectory. Default is False.
+        - If trajectory is True, the input pdb_array should contain the path to the topology file and the trajectory file.
+        - pdb_array[0]: Path to the topology file.
+        - pdb_array[1]: Path to the trajectory file.
+    - traj_frames (int, optional): Number of frames to extract from the trajectory. Default is 1.
 
     Attributes:
     - pdb_array (list): List of file paths to the input PDB models.
     - align_bool (bool): Flag indicating whether to align the models.
     - end_radius (float): Radius of the spherical probe particle.
     - pathway_sel (str): Atom selection string for identifying the pathway.
     - path_save (str): Path to save analysis results.
@@ -61,59 +66,90 @@
     - bulk conductivity (float): Bulk conductivity of the system.
 
     Methods:
     - hole_analysis: Perform hole analysis on the set of PDB models.
     - ellipsoid_analysis: Perform ellipsoid analysis on a specific PDB model.
     - plt_pathway_ellipsoid: Plot ellipsoid analysis results for a specific model.
     - pathway_visualisation: Visualize the pathway for a specific model.
-    - pathway_rendering: Render the pathway for a specific model.
     - conductance_estimation: Estimate the conductance of the pore using a conductivity model.
+    - plt_trajectory_average: Plot the trajectory average of the radius / radii profile.
 
     Example:
     >>> pdb_models = ['model1.pdb', 'model2.pdb']
     >>> pore_analysis = PoreAnalysis(pdb_array=pdb_models, opt_method='nelder-mead')
     >>> pore_analysis.hole_analysis()
     >>> pore_analysis.ellipsoid_analysis(index_model=0)
     >>> pore_analysis.plt_pathway_ellipsoid(index_model=0)
     >>> pore_analysis.pathway_visualisation(index_model=0)
     >>> pore_analysis.pathway_rendering(index_model=0)
     >>> pore_analysis.conductance_estimation(index_model=0)
+
+    Example with trajectory:
+    >>> pdb_models = [fname+'.tpr', fname+'.xtc']
+    >>> pore_analysis = PoreAnalysis(pdb_array=pdb_models, trajectory=True, traj_frames=10)
+    >>> pore_analysis.hole_analysis()
+    >>> pore_analysis.plt_trajectory_average(HOLE_profile=True)
+    >>> for i in range(10): pore_analysis.ellipsoid_analysis(index_model=i)
+    >>> pore_analysis.plt_trajectory_average(HOLE_profile=False)
     """
     def __init__(self, pdb_array, opt_method='nelder-mead',
                  align_bool=True, end_radius=15, pathway_sel='protein',
                  path_save = '', 
                  num_circle=24, clipping=100,
                  D_cation=1.8e-9, D_anion=2.032e-9,
                  popt = [1.40674664, 1.25040698], 
-                 temp=300, c_m=0.15
+                 temp=300, c_m=0.15,
+                 trajectory=False,
+                 traj_frames=1, 
                  ):
-        self.pdb_array = pdb_array
+        self.trajectory = trajectory
+        if trajectory:
+            self.traj_frames = traj_frames 
+            # write out frames from trajectory file
+            top = pdb_array[0]
+            conf = pdb_array[1]
+            fname = conf.split('/')[-1].split('.')[0]
+            u = MDAnalysis.Universe(top, conf)
+            protein = u.select_atoms(pathway_sel)
+            indices = np.arange(0, len(u.trajectory), int((len(u.trajectory))/(traj_frames)))[:traj_frames]
+            self.pdb_array = []
+            for i in indices:
+                u.trajectory[i]
+                s = path_save+fname+str(i)+'.pdb'
+                protein.write(s)
+                self.pdb_array.append(s)
+        else:
+            self.pdb_array = pdb_array
+        print('pdb_array, self'  , self.pdb_array, 'input',  pdb_array )    
         self.align_bool = align_bool
         self.end_radius = end_radius
         self.pathway_sel = pathway_sel
         self.path_save = path_save
         labels = []
         names_aligned = []
-        for ele in pdb_array:
+        for ele in self.pdb_array:
             splits = ele.split('/')[-1]
-            labels.append(splits[:-4])
-            names_aligned.append(ele[:-4]+'_aligned_z.pdb')
+            labels.append(splits.split('.')[0] ) #splits[:-4]
+            names_aligned.append(ele.split('.')[-2] +'_aligned_z.pdb') # ele[:-4]
         self.labels = labels
         self.names_aligned = names_aligned
+        print('self.labels', self.labels )
+        print('self.names_aligned', self.names_aligned)
 
         self.opt_method = opt_method
 
         self.num_circle = num_circle  # for point cloud visualization of pore surface
         self.clipping = clipping # 3d visualisation of pore surface
 
         self.hole_fig = None 
         self.hole_df = None 
 
         self.ellipsoid_dfs = {}
 
+
         ### conductance estimation ###
         self.popt = popt
         e = 1.6022*1e-19 # C
         J2kcal = 1/4184 # 1 kcalth = 4184 J
         kT = 1.380*1e-23 *temp #* J2kcal# J/K
         # mobility
         mu_Na = D_cation/kT
@@ -158,14 +194,85 @@
         self.hole_fig = fig
         self.hole_df = df 
         for i in range(len(self.pdb_array)):
             write_pdb_with_pore_surface(path=self.path_save, name=self.names_aligned[i], 
                                         end_radius=self.end_radius, num_circle = self.num_circle)
         return fig, df  
     
+    def plt_trajectory_average(self, num_bins=100, f_size=20, title='', HOLE_profile=True):
+        """
+        Plot the trajectory average of the hole radius.
+        Parameters:
+        - num_bins (int, optional): Number of bins for the plot. Default is 100.
+        - f_size (int, optional): Font size for the plot. Default is 20.
+        - title (str, optional): Title for the plot. Default is an empty string.
+        - HOLE_profile (bool, optional): Flag indicating whether to plot the HOLE 
+            profile or the PoreAnalysor profile. Default is True.
+        Returns:
+        Figure  and dataframe
+        """
+        z = np.array([])
+        if HOLE_profile:
+            r = np.array([])
+            for l in self.labels:
+                z = np.append(z, self.hole_df[l+' z [A]'])
+                r = np.append(r, self.hole_df[l+' Radius [A]'])
+            df = pd.DataFrame({'z':z, 'r':r})
+            bin_edges = pd.cut(df['z'], bins=num_bins)
+            grouped = df.groupby(bin_edges)
+            result = grouped.agg({
+                'z': ['mean', 'std'],
+                'r': ['mean', 'std'], })
+            self.av_hole = result 
+        else:
+            a = np.array([])
+            b = np.array([])
+            for key in self.ellipsoid_dfs:
+                df_PA = self.ellipsoid_dfs[key]
+                z = np.append(z, df_PA.z)
+                a = np.append(a, df_PA.a)
+                b = np.append(b, df_PA.b)
+            df = pd.DataFrame({'z':z, 'a':a, 'b':b})
+            bin_edges = pd.cut(df['z'], bins=num_bins)
+            grouped = df.groupby(bin_edges)
+            result = grouped.agg({
+                'z': ['mean', 'std'],
+                'a': ['mean', 'std'],
+                'b': ['mean', 'std'],
+            })
+            self.av_PA = result 
+            
+        fig, ax = plt.subplots()
+        ax.set_title(title+' trajectory average', fontsize=f_size)
+        if HOLE_profile:
+            plt.plot(result['z']['mean'], result['r']['mean'], label='r', color='blue'  )
+            plt.fill_between(
+                result['z']['mean'], result['r']['mean']-result['r']['std'],  result['r']['mean']+result['r']['std'],
+                color='blue', alpha=0.2,
+            )
+        else:
+            plt.plot(result['z']['mean'], result['a']['mean'], label='a', color='blue'  )
+            plt.plot(result['z']['mean'], result['b']['mean'], label='b', color='orange'  )
+            plt.fill_between(
+                result['z']['mean'], result['a']['mean']-result['a']['std'],  result['a']['mean']+result['a']['std'],
+                color='blue', alpha=0.2,
+            )
+            plt.fill_between(
+                result['z']['mean'], result['b']['mean']-result['b']['std'],  result['b']['mean']+result['b']['std'],
+                color='orange', alpha=0.2,
+            )
+        ax.set_ylim([0, self.end_radius+10])
+        ax.set_ylabel('Radius ($\AA$)', fontsize=f_size)
+        ax.set_xlabel('z ($\AA$)', fontsize=f_size)
+        ax.tick_params(axis='both', which='major', labelsize=f_size)
+        ax.legend(prop={'size': f_size})
+        fig.tight_layout()
+        plt.show()
+        return fig, result
+    
     def ellipsoid_analysis(self, index_model=0, 
                            plot_lines=True, legend_outside=False, title='', f_size=15):
         """
         Perform ellipsoid analysis on a specific PDB model.
 
         Parameters:
         - index_model (int, optional): Index of the model in the pdb_array. Default is 0.
@@ -200,15 +307,15 @@
                     comments='#', delimiter=',')
         df_res = pd.DataFrame(data=res, columns=['x', 'y', 'z', 'a', 'b', 'theta'])
         df_res.sort_values('z', inplace=True)
 
         self.ellipsoid_dfs[self.labels[index_model]] = df_res
 
         write_pdb_with_ellipsoid_surface(p='', pdbname=self.names_aligned[index_model], 
-                                     fname=self.names_aligned[0]+'_pathway_ellipse.txt', num_circle = self.num_circle)
+                                     fname=self.names_aligned[index_model]+'_pathway_ellipse.txt', num_circle = self.num_circle)
         return df_res
 
     def plt_pathway_ellipsoid(self, index_model=0, title='', f_size=15):
         """
         Plot ellipsoid analysis results for a specific model.
 
         Parameters:
@@ -246,26 +353,14 @@
         xyzview = pathway_visu(path=self.path_save, #path='', 
                                name=self.names_aligned[index_model], 
                                f_end=f_end, pathway_sel=self.pathway_sel,
                                clipping=self.clipping,
                                )
         # f_end='_ellipsoid.pdb' f_end='_circle.pdb'
         return xyzview
-    
-    def pathway_rendering(self, index_model=0, f_end='_circle.pdb', outname='out'):
-        """
-        Render the pathway for a specific model.
-
-        Parameters:
-        - index_model (int, optional): Index of the model in the pdb_array. Default is 0.
-        - f_end (str, optional): File ending for the visualization file. Default is '_circle.pdb'.
-        - outname
-        """
-        render_visu(path='', name=self.names_aligned[index_model], 
-                    f_end=f_end, outname=outname, streamlit=False)
         
     def conductance_estimation(self, index_model=0, f_size=15):
         """
         Estimate the conductance of the pore using a conductivity model.
         Parameters:
         - index_model (int, optional): Index of the model in the pdb_array. Default is 0.
         - f_size (int, optional): Font size for the plot. Default is 15.
```

### Comparing `poreanalyser-0.0.4/PoreAnalyser/tests/test_conductance.py` & `poreanalyser-0.0.5/PoreAnalyser/tests/test_conductance.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipse.py` & `poreanalyser-0.0.5/PoreAnalyser/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipsoid_optimisation.py` & `poreanalyser-0.0.5/PoreAnalyser/tests/test_ellipsoid_optimisation.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/tests/test_hole.py` & `poreanalyser-0.0.5/PoreAnalyser/tests/test_hole.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/PoreAnalyser/visualization.py` & `poreanalyser-0.0.5/PoreAnalyser/visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,42 +283,20 @@
     with open(path+name + f_end) as ifile:
         sph2 = "".join([x for x in ifile])
     xyzview.addModelsAsFrames(sph2)
     xyzview.addSurface(py3Dmol.SES,{'opacity':0.9,'color':'lightblue'}, {'model': -1})
     xyzview.zoomTo()
     xyzview.rotate(90,'y',0)
     xyzview.render()
-    uri = xyzview.pngURI()
-    print('pngURI', uri)
-    #png =  xyzview.png() # AssertionError: Must instantiate viewer before generating image.
+    #uri = xyzview.pngURI()
+    #print('pngURI', uri)
+    #png = xyzview.png() # AssertionError: Must instantiate viewer before generating image.
     #print('png', png)
     return xyzview
 
-def render_visu(path, name, f_end='_circle.pdb',outname='', streamlit=True ):
-    u = MDAnalysis.Universe(path+name, topology_format='pdb', format='pdb')
-    u2 = MDAnalysis.Universe(path+name + f_end, topology_format='pdb', format='pdb')
-    v = nv.show_mdanalysis(u.atoms)
-
-    v.clear_representations(component=0)
-    v.add_representation('cartoon', color='blue', component=0)
-    v.add_trajectory(u2.atoms)
-    v.add_surface(component=1,
-                probeRadius=0.1, surfaceType='ms')
-    v._remote_call("setSize", target="Widget", args=["1200px", "800px"])
-    v.control.spin([0, 1, 0], 3.1415/2)
-    v.center()
-    if streamlit:
-        im1 = v.render_image()
-        with open('nglview'+outname+'.png', 'wb') as fh:
-            fh.write(im1.value) 
-        print('renderd', im1)
-    else:
-        print('renderd via download', 'nglview'+outname+'.png')
-        v.download_image('nglview'+outname+'.png')
-    return v 
 
 def st_write_ellipsoid():
     st.subheader("Path finding with ellipsoidal probe particle")
     string1 = '1. Load HOLE output file with positions and radii of probes.\n'
     string2 = '2. Loop through all spherical probe particles:\n'
     string3 = 'a) Ellipsoid initialized with spherical probe particle parameters from HOLE output.\n'
     string4 = 'b) First Nelder-Mead 4-dim optimization to insert ellipsoid with smaller bounds for parameters [x, y, r1, θ ].\n'
```

### Comparing `poreanalyser-0.0.4/README.md` & `poreanalyser-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.4/pyproject.toml` & `poreanalyser-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 [project]
 name = "PoreAnalyser"
 authors = [{name = "David Seiferth", email = "david.seiferth@oriel.ox.ac.uk"}]
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "PoreAnalyser package based on HOLE and MDAnalysis"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">=3.6"
 dependencies = [
+#python<=3.11,
 'numpy >=1.0, <1.23.0',
 'MDAnalysis >=2.0, <3.0',
 'matplotlib>=0.1',
 'pandas>=1.3',
 'streamlit>=1.0',
 'stmol==0.0.9',
 'py3Dmol',
```

### Comparing `poreanalyser-0.0.4/PKG-INFO` & `poreanalyser-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PoreAnalyser
-Version: 0.0.4
+Version: 0.0.5
 Summary: PoreAnalyser package based on HOLE and MDAnalysis
 Author-email: David Seiferth <david.seiferth@oriel.ox.ac.uk>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy >=1.0, <1.23.0
 Requires-Dist: MDAnalysis >=2.0, <3.0
 Requires-Dist: matplotlib>=0.1
```

