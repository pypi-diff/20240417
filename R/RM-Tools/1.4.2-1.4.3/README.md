# Comparing `tmp/RM-Tools-1.4.2.tar.gz` & `tmp/rm_tools-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RM-Tools-1.4.2.tar", last modified: Thu Apr 11 02:00:24 2024, max compression
+gzip compressed data, was "rm_tools-1.4.3.tar", last modified: Wed Apr 17 01:45:04 2024, max compression
```

## Comparing `RM-Tools-1.4.2.tar` & `rm_tools-1.4.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.659025 RM-Tools-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-11 02:00:24.659025 RM-Tools-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.655025 RM-Tools-1.4.2/RM_Tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 02:00:24.000000 RM-Tools-1.4.2/RM_Tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.651025 RM-Tools-1.4.2/RMtools_1D/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/calculate_RMSF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.651025 RM-Tools-1.4.2/RMtools_1D/cats/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/cats/catComplex.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/cats/cat_simple_doQUfit.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/cats/catalogue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/cats/catalogue1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/cats/testCat.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/clean_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/do_QUfit_1D_mnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/do_RMclean_1D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/do_RMsynth_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/do_RMsynth_1D_fromFITS.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/mk_test_ascii_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.655025 RM-Tools-1.4.2/RMtools_1D/models_ns/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/models_ns/m7.py
--rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/rmtools_bwdepol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_1D/rmtools_bwpredict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.655025 RM-Tools-1.4.2/RMtools_3D/
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/RMpeakfit_3D.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/assemble_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/create_chunks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/do_RMclean_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/do_RMsynth_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/do_fitIcube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/extract_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/make_freq_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/mk_test_cube_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMtools_3D/rescale_I_model_3D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:00:24.655025 RM-Tools-1.4.2/RMutils/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/mpfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_FITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    84116 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_RM.py
--rw-r--r--   0 runner    (1001) docker     (127)    47521 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_plotFITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_plotTk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/RMutils/util_rec.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:00:24.659025 RM-Tools-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-11 02:00:20.000000 RM-Tools-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 01:45:00.000000 rm_tools-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-17 01:45:00.000000 rm_tools-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 01:45:04.734009 rm_tools-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-17 01:45:00.000000 rm_tools-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/RM_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/calculate_RMSF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/cats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catComplex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/cat_simple_doQUfit.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catalogue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catalogue1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/testCat.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/clean_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_QUfit_1D_mnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMclean_1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D_fromFITS.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/mk_test_ascii_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/models_ns/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/rmtools_bwdepol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/rmtools_bwpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.730009 rm_tools-1.4.3/RMtools_3D/
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/RMpeakfit_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/assemble_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/create_chunks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_RMclean_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_RMsynth_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_fitIcube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/extract_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/make_freq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/mk_test_cube_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/rescale_I_model_3D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/RMutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/mpfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_FITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84116 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_RM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_plotFITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_plotTk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:45:04.734009 rm_tools-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-17 01:45:00.000000 rm_tools-1.4.3/setup.py
```

### Comparing `RM-Tools-1.4.2/LICENSE.txt` & `rm_tools-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/PKG-INFO` & `rm_tools-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.2
+Version: 1.4.3
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.2.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.3.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RM-Tools-1.4.2/README.md` & `rm_tools-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RM_Tools.egg-info/PKG-INFO` & `rm_tools-1.4.3/RM_Tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.2
+Version: 1.4.3
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.2.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.3.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RM-Tools-1.4.2/RM_Tools.egg-info/SOURCES.txt` & `rm_tools-1.4.3/RM_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RM_Tools.egg-info/entry_points.txt` & `rm_tools-1.4.3/RM_Tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/calculate_RMSF.py` & `rm_tools-1.4.3/RMtools_1D/calculate_RMSF.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/cats/catComplex.csv` & `rm_tools-1.4.3/RMtools_1D/cats/catComplex.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/cats/cat_simple_doQUfit.bat` & `rm_tools-1.4.3/RMtools_1D/cats/cat_simple_doQUfit.bat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/cats/catalogue.csv` & `rm_tools-1.4.3/RMtools_1D/cats/catalogue.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/cats/catalogue1.csv` & `rm_tools-1.4.3/RMtools_1D/cats/catalogue1.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/cats/testCat.dat` & `rm_tools-1.4.3/RMtools_1D/cats/testCat.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/clean_model.py` & `rm_tools-1.4.3/RMtools_1D/clean_model.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/do_QUfit_1D_mnest.py` & `rm_tools-1.4.3/RMtools_1D/do_QUfit_1D_mnest.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/do_RMclean_1D.py` & `rm_tools-1.4.3/RMtools_1D/do_RMclean_1D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/do_RMsynth_1D.py` & `rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/do_RMsynth_1D_fromFITS.py` & `rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D_fromFITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/mk_test_ascii_data.py` & `rm_tools-1.4.3/RMtools_1D/mk_test_ascii_data.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m1.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m1.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m11.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m11.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m111.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m111.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m2.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m2.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m3.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m3.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m4.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m4.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m5.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m5.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m6.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m6.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/models_ns/m7.py` & `rm_tools-1.4.3/RMtools_1D/models_ns/m7.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/rmtools_bwdepol.py` & `rm_tools-1.4.3/RMtools_1D/rmtools_bwdepol.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_1D/rmtools_bwpredict.py` & `rm_tools-1.4.3/RMtools_1D/rmtools_bwpredict.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/RMpeakfit_3D.py` & `rm_tools-1.4.3/RMtools_3D/RMpeakfit_3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     phiArr,
     fwhmRMSF,
     lamSqArr_m2,
     lam0Sq,
     product_list,
     noiseArr=None,
     stokesIcube=None,
+    weightType="uniform",
 ):
     """
     Performs the 1D FDF peak fitting used in RMsynth/RMclean_1D, pixelwise on
     all pixels in a 3D FDF cube.
 
     Inputs:
         FDF: FDF cube (3D array). This is assumed to be in astropy axis ordering
@@ -87,16 +88,23 @@
             Ifreq0Arr = stokesIcube[idx, :, :]
     else:
         Ifreq0Arr = np.ones(map_size)
         stokesIcube = np.ones((freqArr_Hz.size, map_size[0], map_size[1]))
 
     # compute weights if needed:
     if noiseArr is not None:
-        weightArr = 1.0 / np.power(noiseArr, 2.0)
-        weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
+        if weightType == "variance":
+            weightArr = 1.0 / np.power(noiseArr, 2.0)
+            weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
+        elif weightType == "uniform":
+            weightArr = np.ones(lamSqArr_m2.shape, dtype=np.float32)
+            weightArr = np.where(np.isnan(noiseArr), 0.0, weightArr)
+        else:
+            raise Exception("Invalid weight type; must be 'uniform' or 'variance'")
+
         dFDF = Ifreq0Arr * np.sqrt(
             np.sum(weightArr**2 * np.nan_to_num(noiseArr) ** 2)
             / (np.sum(weightArr)) ** 2
         )
 
     else:
         weightArr = np.ones(lamSqArr_m2.shape, dtype=np.float32)
@@ -374,14 +382,20 @@
     )
     parser.add_argument(
         "-n",
         dest="noiseFile",
         default=None,
         help="FITS file or cube containing noise values [None].",
     )
+    parser.add_argument(
+        "-w",
+        dest="weightType",
+        default="uniform",
+        help="weighting ['uniform'] (all 1s) or 'variance' used in rmsynth3d, affects uncertainty estimation.",
+    )
 
     args = parser.parse_args()
 
     # Check for incompatible options:
     if args.peak_only and args.all_products:
         print("Please select at most ONE of the -a and -p flags.")
         sys.exit()
@@ -470,14 +484,15 @@
         phiArr_radm2,
         fwhmRMSF,
         lambdaSqArr_m2,
         lam0Sq,
         product_list,
         noiseArr=rmsArr,
         stokesIcube=dataI,
+        weightType=args.weightType,
     )
 
     save_maps(map_dict, args.output_name[0], header)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RM-Tools-1.4.2/RMtools_3D/assemble_chunks.py` & `rm_tools-1.4.3/RMtools_3D/assemble_chunks.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/create_chunks.py` & `rm_tools-1.4.3/RMtools_3D/create_chunks.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/do_RMclean_3D.py` & `rm_tools-1.4.3/RMtools_3D/do_RMclean_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/do_RMsynth_3D.py` & `rm_tools-1.4.3/RMtools_3D/do_RMsynth_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/do_fitIcube.py` & `rm_tools-1.4.3/RMtools_3D/do_fitIcube.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/extract_region.py` & `rm_tools-1.4.3/RMtools_3D/extract_region.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/make_freq_file.py` & `rm_tools-1.4.3/RMtools_3D/make_freq_file.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/mk_test_cube_data.py` & `rm_tools-1.4.3/RMtools_3D/mk_test_cube_data.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMtools_3D/rescale_I_model_3D.py` & `rm_tools-1.4.3/RMtools_3D/rescale_I_model_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/mpfit.py` & `rm_tools-1.4.3/RMutils/mpfit.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/normalize.py` & `rm_tools-1.4.3/RMutils/normalize.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/util_FITS.py` & `rm_tools-1.4.3/RMutils/util_FITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/util_RM.py` & `rm_tools-1.4.3/RMutils/util_RM.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/util_misc.py` & `rm_tools-1.4.3/RMutils/util_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,15 @@
                 + 9 * lnx**4 * cov[2, 2]
                 + 12 * lnx**3 * cov[2, 3]
                 + 6 * lnx**2 * cov[2, 4]
                 + 4 * lnx**2 * cov[3, 3]
                 + 4 * lnx * cov[3, 4]
                 + cov[4, 4]
             ),
-            g2
+            np.abs(g2)
             * np.sqrt(
                 lnx**10 * cov[0, 0]
                 + 2 * lnx**9 * cov[0, 1]
                 + 2 * lnx**8 * cov[0, 2]
                 + 2 * lnx**7 * cov[0, 3]
                 + 2 * lnx**6 * cov[0, 4]
                 + 2 * lnx**5 / g * np.log(10) * cov[0, 5]
```

### Comparing `RM-Tools-1.4.2/RMutils/util_plotFITS.py` & `rm_tools-1.4.3/RMutils/util_plotFITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/util_plotTk.py` & `rm_tools-1.4.3/RMutils/util_plotTk.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/RMutils/util_rec.py` & `rm_tools-1.4.3/RMutils/util_rec.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.2/setup.py` & `rm_tools-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import setup
 
 NAME = "RM-Tools"
 DESCRIPTION = "RM-synthesis, RM-clean and QU-fitting on polarised radio spectra"
 URL = "https://github.com/CIRADA-Tools/RM-Tools"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.4.2"
+VERSION = "1.4.3"
 DOWNLOAD_URL = (
     "https://github.com/CIRADA-Tools/RM-Tools/archive/v" + VERSION + ".tar.gz"
 )
 
 REQUIRED = [
     "numpy<2",
     "scipy",
```

