# Comparing `tmp/stemdiff-5.2.5.tar.gz` & `tmp/stemdiff-5.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemdiff-5.2.5.tar", last modified: Mon Mar 18 18:47:57 2024, max compression
+gzip compressed data, was "stemdiff-5.2.6.tar", last modified: Wed Apr 17 14:57:33 2024, max compression
```

## Comparing `stemdiff-5.2.5.tar` & `stemdiff-5.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 18:47:57.775991 stemdiff-5.2.5/
--rw-rw-rw-   0        0        0      243 2023-12-12 18:35:41.000000 stemdiff-5.2.5/CITATION
--rw-rw-rw-   0        0        0     1340 2023-12-12 18:35:41.000000 stemdiff-5.2.5/LICENCE
--rw-rw-rw-   0        0        0      139 2021-12-12 12:41:30.000000 stemdiff-5.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4197 2024-03-18 18:47:57.775991 stemdiff-5.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3523 2024-03-18 18:43:15.000000 stemdiff-5.2.5/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 18:47:57.776991 stemdiff-5.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-10 12:47:30.000000 stemdiff-5.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:47:57.760978 stemdiff-5.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 18:47:57.772662 stemdiff-5.2.5/src/stemdiff/
--rw-rw-rw-   0        0        0     1996 2024-03-18 18:43:15.000000 stemdiff-5.2.5/src/stemdiff/__init__.py
--rw-rw-rw-   0        0        0     5969 2023-12-20 17:09:50.000000 stemdiff-5.2.5/src/stemdiff/dbase.py
--rw-rw-rw-   0        0        0    11798 2024-03-18 18:43:15.000000 stemdiff-5.2.5/src/stemdiff/detectors.py
--rw-rw-rw-   0        0        0     4610 2023-12-20 17:09:50.000000 stemdiff-5.2.5/src/stemdiff/gvars.py
--rw-rw-rw-   0        0        0    47940 2024-03-18 18:43:15.000000 stemdiff-5.2.5/src/stemdiff/io.py
--rw-rw-rw-   0        0        0    14591 2023-12-20 17:09:50.000000 stemdiff-5.2.5/src/stemdiff/sum.py
--rw-rw-rw-   0        0        0     8014 2024-02-16 10:14:34.000000 stemdiff-5.2.5/src/stemdiff/summ.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:47:57.774986 stemdiff-5.2.5/src/stemdiff.egg-info/
--rw-rw-rw-   0        0        0     4197 2024-03-18 18:47:57.000000 stemdiff-5.2.5/src/stemdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-03-18 18:47:57.000000 stemdiff-5.2.5/src/stemdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 18:47:57.000000 stemdiff-5.2.5/src/stemdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-03-18 18:47:57.000000 stemdiff-5.2.5/src/stemdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 18:47:57.000000 stemdiff-5.2.5/src/stemdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 14:57:33.348609 stemdiff-5.2.6/
+-rw-rw-rw-   0        0        0      243 2023-12-12 18:35:42.000000 stemdiff-5.2.6/CITATION
+-rw-rw-rw-   0        0        0     1340 2023-12-12 18:35:42.000000 stemdiff-5.2.6/LICENCE
+-rw-rw-rw-   0        0        0      139 2021-12-12 12:41:30.000000 stemdiff-5.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4197 2024-04-17 14:57:33.348609 stemdiff-5.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3523 2024-03-18 18:43:16.000000 stemdiff-5.2.6/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:57:33.348609 stemdiff-5.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-10 12:47:30.000000 stemdiff-5.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:57:33.317531 stemdiff-5.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 14:57:33.340868 stemdiff-5.2.6/src/stemdiff/
+-rw-rw-rw-   0        0        0     1998 2024-04-17 13:41:39.000000 stemdiff-5.2.6/src/stemdiff/__init__.py
+-rw-rw-rw-   0        0        0     5985 2024-04-17 13:42:21.000000 stemdiff-5.2.6/src/stemdiff/dbase.py
+-rw-rw-rw-   0        0        0    11850 2024-04-17 14:16:40.000000 stemdiff-5.2.6/src/stemdiff/detectors.py
+-rw-rw-rw-   0        0        0     4453 2024-04-17 14:28:51.000000 stemdiff-5.2.6/src/stemdiff/gvars.py
+-rw-rw-rw-   0        0        0    48011 2024-04-17 14:35:30.000000 stemdiff-5.2.6/src/stemdiff/io.py
+-rw-rw-rw-   0        0        0    14607 2024-04-17 13:46:40.000000 stemdiff-5.2.6/src/stemdiff/sum.py
+-rw-rw-rw-   0        0        0     8030 2024-04-17 13:46:52.000000 stemdiff-5.2.6/src/stemdiff/summ.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:57:33.348609 stemdiff-5.2.6/src/stemdiff.egg-info/
+-rw-rw-rw-   0        0        0     4197 2024-04-17 14:57:33.000000 stemdiff-5.2.6/src/stemdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-17 14:57:33.000000 stemdiff-5.2.6/src/stemdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:57:33.000000 stemdiff-5.2.6/src/stemdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-17 14:57:33.000000 stemdiff-5.2.6/src/stemdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 14:57:33.000000 stemdiff-5.2.6/src/stemdiff.egg-info/top_level.txt
```

### Comparing `stemdiff-5.2.5/LICENCE` & `stemdiff-5.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `stemdiff-5.2.5/PKG-INFO` & `stemdiff-5.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 5.2.5
+Version: 5.2.6
 Summary: Convert 4D-STEM data to 2D-powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stemdiff-5.2.5/README.md` & `stemdiff-5.2.6/README.md`

 * *Files identical despite different names*

### Comparing `stemdiff-5.2.5/setup.py` & `stemdiff-5.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.2.5/src/stemdiff/__init__.py` & `stemdiff-5.2.6/src/stemdiff/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-STEMDIFF package
-----------------
+Package: STEMDIFF
+-----------------
 Conversion of a 4D-STEM dataset to a 2D-powder diffration pattern.
 
 * Input = 4D-STEM dataset = 2D-array of 2D-NBD patterns.
     - 2D-array = usually one (or more) two-dimensional scanning array(s).
     - 2D-NBD = monocrystalline-like nanobeam diffraction pattern.
 * Output = 2D-powder diffraction pattern
     - The final 2D-diffractogram is a specific summation of 2D-NBD patterns.
@@ -26,15 +26,15 @@
 * IDIFF is imported below so that it could be used as: sd.idiff.some_module
 * IDIFF modules are:
     - idiff.bcorr = background correction/subtraction
     - idiff.deconv = advanced deconvolution methods
     - idiff.ncore = noise correction/reduction
     - idiff.psf = estimate of PSF function
 '''
-__version__ = "5.2.5"
+__version__ = "5.2.6"
 
 # Import modules of stemdiff package
 # this enables us to use modules as follows:
 # >>> import stemdiff as sd
 # >>> sd.io.Datafiles.read(SDATA, '000_001.dat')
 import stemdiff.dbase
 import stemdiff.detectors
```

### Comparing `stemdiff-5.2.5/src/stemdiff/dbase.py` & `stemdiff-5.2.6/src/stemdiff/dbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.dbase
---------------
+Module: stemdiff.dbase
+----------------------
 Functions to calculate, save and re-read the database of 4D-STEM datafiles.
 
 * The database is saved as a pandas.DataFrame object,
   which contains the following data for each datafile:
   filename, XY-center coordinates, MaximumIntensity, NoOfPeaks, ShannonEntropy.
 * The database enables fast filtering of datafiles
   and fast access to datafile features,
```

### Comparing `stemdiff-5.2.5/src/stemdiff/detectors.py` & `stemdiff-5.2.6/src/stemdiff/detectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.detectors
-------------------
+Module: stemdiff.detectors
+--------------------------
 Description of detectors that can be used in stemdiff package.
 
 This module is basically a container of classes.
 Each class describes a 2D STEM detector, from which we can read datafiles.
 The description of the detector not difficult.
 All we need to define is the detector name,
 a few technical parameters described below,
@@ -59,15 +59,15 @@
     print('List of knonw detectors = classes defined in stemdiff.detectors:')
     for detector in detectors:
         print(detector)
 
 
 def describe_detector(detector_object):
     '''
-    Print the description of the detector on the screen.
+    Global method: the description of the detector on the screen.
     
     Parameters
     ----------
     detector_object : object of any class in stemdiff.detectors
         The initialized detector object.
         The object contains description of the detector.
         It is created by calling init method of any stemdiff.detectors class.
@@ -79,15 +79,16 @@
         
     Example
     -------
     >>> # Short example
     >>> # (minimalistic example
     >>> import stemdiff as sd
     >>> my_detector = sd.detectors.TimePix()
-    >>> my_detector.self_describe()
+    >>> my_detector.self_describe()     # OO-interface, indirect call
+    >>> describe_detector(my_detector)  # procedural interface, direct call
     >>>
     >>> # Real usage
     >>> # (in STEMDIFF scripts,
     >>> # (the detector is usually defined
     >>> # (within stemdiff.gvars.SourceData object
     >>> import stemdiff as sd
     >>> SDATA = sd.gvars.SourceData(
@@ -141,20 +142,18 @@
     * binary data files, usually with DAT extension
     * a 1D arrays of 16-bit intensities = np.uint16 values
     '''
 
     
     def __init__(self, detector_name='TimePix', 
                  detector_size=256, max_intensity=11810, 
-                 data_type=np.uint16, upscale=4):
-        '''
-        * The initialization of TimePix detector objects.
-        * The parameters are described above in class definition.
-        * Auto-documentation list (some of) the initialization parameters.
-        '''
+                 data_type=np.uint16, upscale=4):   
+        # The initialization of TimePix detector objects.
+        # The parameters are described above in class definition.
+        # -----
         self.detector_name = detector_name
         self.detector_size = detector_size
         self.max_intensity = max_intensity
         self.data_type = data_type
         self.upscale = upscale
 
     def self_describe(self):
@@ -255,28 +254,27 @@
         The upscaling coefficient increases the detector resolution.
         Surprisingly enough, the upscaling helps to improve final resolution.
     
     Returns
     -------
     Secom detector object.
     
-    Format of Secom datafiles
-    ---------------------------
+    Format of SECOM datafiles
+    -------------------------
     * image files, TIFF format
     * 16-bit images = images containing np.uint16 values
     '''
 
     
     def __init__(self, detector_name='Secom', 
                  detector_size=2048, max_intensity=65536,
                  data_type=np.uint16, upscale=1):
-        '''
-        Initialize parameters of Secom detector.
-        The parameters are described above in class definition.
-        '''
+        # The initialization of Secom detector objects.
+        # The parameters are described above in class definition.
+        # -----
         self.detector_name = detector_name
         self.detector_size = detector_size
         self.max_intensity = max_intensity
         self.data_type = data_type
         self.upscale = upscale
```

### Comparing `stemdiff-5.2.5/src/stemdiff/gvars.py` & `stemdiff-5.2.6/src/stemdiff/gvars.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.gvars
---------------
+Module: stemdiff.gvars
+----------------------
 Global variables/objects for package stemdiff.
 
 The global variables are used throughout the whole program.
 In order to be easily accessible, they are defined as two objects:
     
 * SourceData = an object defining the input datafiles.
 * DiffImages = an object desribing basic/common features of all NBD patterns.
@@ -49,23 +49,21 @@
         This parameter is passed to Path.glob method from pathlib library.
         It is strongly recommeded to use r-strings.
         Example1: `datafiles = r'*.dat'` = all `*.dat` files in parent_dir;
         Example2: `datafiles = r'??/*.dat'` = all `*.dat` in subdirs `01,02...`
     
     Returns
     -------
-    DataFiles object.
+    DataFiles object
     '''
 
     def __init__(self, detector, data_dir, filenames):
-        '''
-        * The initialization of SourceData objects.
-        * The parameters are described above in class definition.
-        * Auto-documentation list (some of) the initialization parameters.
-        '''
+        # The initialization of SourceData objects.
+        # The parameters are described above in class definition.
+        # -----
         self.detector = detector
         self.data_dir = Path(data_dir)
         self.filenames = self.data_dir.glob(filenames)
 
         
 class DiffImages:
     '''
@@ -93,26 +91,24 @@
     peak_height : float, optional, default is 100
         Search for peaks whose intensity > peak_height.
     peak_dist : integer, optional, default is 3
         Minimal distance between possible neighboring peaks.
 
     Returns
     -------
-    DiffImages object.
+    DiffImages object
     '''
     
     def __init__(self, 
                  imgsize=100, psfsize=30,
                  ctype=2, csquare=20, cintensity=0.8,
                  peak_height=100, peak_dist=3):
-        '''
-        * The initialization of DiffImages objects.
-        * The parameters are described above in class definition.
-        * Auto-documentation list (some of) the initialization parameters.
-        ''' 
+        # The initialization of DiffImages objects.
+        # The parameters are described above in class definition.
+        # -----
         self.imgsize = imgsize
         self.psfsize = psfsize
         self.ctype = ctype
         self.csquare = csquare
         self.cintensity = cintensity
         self.peak_height = peak_height
         self.peak_dist = peak_dist
```

### Comparing `stemdiff-5.2.5/src/stemdiff/io.py` & `stemdiff-5.2.6/src/stemdiff/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.io
------------
+Module: stemdiff.io
+-------------------
 Input/output functions for package stemdiff.
 
 Three types of stemdiff.io objects
 
 * Datafiles = files on disk, saved directly from a 2D-STEM detector.
 * Arrays = the datafiles converted to numpy array objects.
 * Images = the datafiles converted to PNG files.
@@ -65,25 +65,27 @@
         Size of the font used in figure labels etc.
     my_rcParams : dict, optional, default is None
         Dictionary in plt.rcParams format
         containing any other allowed global plot parameters.
 
     Returns
     -------
-    None; the result is a modification of the global plt.rcParams variable.
+    None
+        The result is a modification of the global plt.rcParams variable.
     '''
     # This function just calls the final function in Plotting module.
     # (left in the main namespace of the package as it is frequently used
     Plots.set_plot_parameters(size, dpi, fontsize, my_rcParams)
     
     
 class Datafiles:
     '''
     Datafiles class = a collection of functions
-    that work with datafiles from 2D-STEM detector saved as files in a disk.
+    that work with datafiles from 2D-STEM detector
+    (assumption: the datafiles were saved as standard files on a disk).
     '''
 
     def read(SDATA, filename):
         '''
         Read a datafile from STEM detector to an array.
         
         Parameters
```

### Comparing `stemdiff-5.2.5/src/stemdiff/sum.py` & `stemdiff-5.2.6/src/stemdiff/sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.sum
-------------
+Module: stemdiff.sum
+--------------------
 The summation of 4D-STEM datafiles to create one 2D powder diffraction file.
 
 * stemdiff.sum = this module, which runs on a single core (serial processing)
 * stemdiff.summ = sister module running on multiple cores (parallel processing)
 
 To perform the summation, we just call function sum_datafiles:
```

### Comparing `stemdiff-5.2.5/src/stemdiff/summ.py` & `stemdiff-5.2.6/src/stemdiff/summ.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.summ
--------------
+Module: stemdiff.summ
+---------------------
 The summation of 4D-STEM datafiles to create one 2D powder diffraction file.
 
 * The summation runs on all available cores (parallel processing).
 * This module takes functions from semdiff.sum, but runs them parallelly. 
 
 The key function of the module (for a user) = stemdiff.summ.sum_datafiles:
```

### Comparing `stemdiff-5.2.5/src/stemdiff.egg-info/PKG-INFO` & `stemdiff-5.2.6/src/stemdiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 5.2.5
+Version: 5.2.6
 Summary: Convert 4D-STEM data to 2D-powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
 Classifier: Programming Language :: Python :: 3
```

