# Comparing `tmp/ediff-0.2.tar.gz` & `tmp/ediff-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediff-0.2.tar", last modified: Wed Nov  1 11:06:01 2023, max compression
+gzip compressed data, was "ediff-0.2.2.tar", last modified: Wed Apr 17 21:15:14 2024, max compression
```

## Comparing `ediff-0.2.tar` & `ediff-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-11-01 11:06:01.484544 ediff-0.2/
--rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:53.000000 ediff-0.2/LICENCE
--rw-rw-rw-   0        0        0     2354 2023-11-01 11:06:01.482166 ediff-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1818 2023-11-01 11:00:33.000000 ediff-0.2/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-01 11:06:01.484544 ediff-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2021-12-09 19:47:58.000000 ediff-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-01 11:06:01.424433 ediff-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-11-01 11:06:01.473652 ediff-0.2/src/ediff/
--rw-rw-rw-   0        0        0      132 2023-11-01 10:57:14.000000 ediff-0.2/src/ediff/__init__.py
--rw-rw-rw-   0        0        0     1044 2023-08-10 12:00:36.000000 ediff-0.2/src/ediff/background.py
--rw-rw-rw-   0        0        0    80819 2023-10-27 19:06:05.000000 ediff-0.2/src/ediff/center.py
--rw-rw-rw-   0        0        0     6444 2023-10-27 11:42:27.000000 ediff-0.2/src/ediff/io.py
--rw-rw-rw-   0        0        0    29101 2023-10-05 14:38:38.000000 ediff-0.2/src/ediff/pxrd.py
--rw-rw-rw-   0        0        0     4657 2023-10-27 11:42:27.000000 ediff-0.2/src/ediff/radial.py
-drwxrwxrwx   0        0        0        0 2023-11-01 11:06:01.480395 ediff-0.2/src/ediff.egg-info/
--rw-rw-rw-   0        0        0     2354 2023-11-01 11:06:01.000000 ediff-0.2/src/ediff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-11-01 11:06:01.000000 ediff-0.2/src/ediff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-01 11:06:01.000000 ediff-0.2/src/ediff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-11-01 11:06:01.000000 ediff-0.2/src/ediff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.676257 ediff-0.2.2/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 ediff-0.2.2/LICENCE
+-rw-rw-rw-   0        0        0     2742 2024-04-17 21:15:14.676257 ediff-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2204 2024-04-17 21:08:45.000000 ediff-0.2.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 21:15:14.676257 ediff-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2021-12-09 19:48:00.000000 ediff-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.644303 ediff-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.667742 ediff-0.2.2/src/ediff/
+-rw-rw-rw-   0        0        0     1623 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/background.py
+-rw-rw-rw-   0        0        0    82026 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/center.py
+-rw-rw-rw-   0        0        0     6813 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/io.py
+-rw-rw-rw-   0        0        0    29312 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/pxrd.py
+-rw-rw-rw-   0        0        0     4659 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/radial.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.676257 ediff-0.2.2/src/ediff.egg-info/
+-rw-rw-rw-   0        0        0     2742 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/top_level.txt
```

### Comparing `ediff-0.2/LICENCE` & `ediff-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ediff-0.2/PKG-INFO` & `ediff-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.2
+Version: 0.2.2
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -14,32 +14,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 EDIFF :: processing of powder electron diffraction patterns
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
-	- bkgr = background subtraction
+	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
-	- radial = calculate radial distribution (2D-pattern to 1D-pattern) 
+	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
 
 Installation
 ------------
-* `pip install bground` = interactive background subtraction
-* `pip install ediff`   = EDIFF program itself (uses bground internally)
+* Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
+* `pip install scikit-image` = 3rd party package for advanced image processing 
+* `pip install pymatgen` = 3rd party package employed in PXRD calculation
+* `pip install bground`= our package, interactive background subtraction
+* `pip install ediff` = EDIFF package itself (uses all packages above)
 
 Quick start
 -----------
 * See how it works:
-	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
+	- Look at [worked example](https://www.dropbox.com/scl/fi/3hb78voxd17wb3fzh9n1p/01_ediff_au.nb.pdf?rlkey=qmbvwaw80o1gbe262hwgjvmgx&dl=0)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
-	- Look at `00readme.txt` and run the example in Jupyter.
+	- Download [complete examples with data](https://www.dropbox.com/scl/fo/td6rkdgp2usxosj1vqeku/h?rlkey=41carfdej5h2f8f4yscbuvagm&dl=0)
+	  and scripts and basic instructions.
+	- After downloading, unzip it and follow the instructions in *readme* file.
 
 Documentation, help and examples
 --------------------------------
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/ediff/)
   with [documentation](https://mirekslouf.github.io/ediff/docs).
@@ -47,11 +51,12 @@
 Versions of EDIFF
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
-* Version 0.1.0 = 1st semi-complete version with basic documentation
-* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
-* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
+* Version 0.1   = 1st semi-complete version with basic documentation
+* Version 0.1.1 = improved/simplified outputs
+* Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
+* Version 0.2.2 = consolidation, update of docs and examples on www
```

### Comparing `ediff-0.2/README.md` & `ediff-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 EDIFF :: processing of powder electron diffraction patterns
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
-	- bkgr = background subtraction
+	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
-	- radial = calculate radial distribution (2D-pattern to 1D-pattern) 
+	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
 
 Installation
 ------------
-* `pip install bground` = interactive background subtraction
-* `pip install ediff`   = EDIFF program itself (uses bground internally)
+* Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
+* `pip install scikit-image` = 3rd party package for advanced image processing 
+* `pip install pymatgen` = 3rd party package employed in PXRD calculation
+* `pip install bground`= our package, interactive background subtraction
+* `pip install ediff` = EDIFF package itself (uses all packages above)
 
 Quick start
 -----------
 * See how it works:
-	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
+	- Look at [worked example](https://www.dropbox.com/scl/fi/3hb78voxd17wb3fzh9n1p/01_ediff_au.nb.pdf?rlkey=qmbvwaw80o1gbe262hwgjvmgx&dl=0)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
-	- Look at `00readme.txt` and run the example in Jupyter.
+	- Download [complete examples with data](https://www.dropbox.com/scl/fo/td6rkdgp2usxosj1vqeku/h?rlkey=41carfdej5h2f8f4yscbuvagm&dl=0)
+	  and scripts and basic instructions.
+	- After downloading, unzip it and follow the instructions in *readme* file.
 
 Documentation, help and examples
 --------------------------------
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/ediff/)
   with [documentation](https://mirekslouf.github.io/ediff/docs).
@@ -31,11 +35,12 @@
 Versions of EDIFF
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
-* Version 0.1.0 = 1st semi-complete version with basic documentation
-* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
-* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
+* Version 0.1   = 1st semi-complete version with basic documentation
+* Version 0.1.1 = improved/simplified outputs
+* Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
+* Version 0.2.2 = consolidation, update of docs and examples on www
```

### Comparing `ediff-0.2/setup.py` & `ediff-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2/src/ediff/center.py` & `ediff-0.2.2/src/ediff/center.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 '''
-Module ediff.center
--------------------
+Module: ediff.center
+--------------------
 Find center of 2D diffraction pattern. 
-
-CenterDet, aktualizace 06-10-23 CentDet update, methods compatibility
 '''
 
+# CenterDet
+# PS 2023-10-06: CentDet update, methods compatibility
+# MS 2023-11-26: Improved code formatting and docs + TODO notes for PS  
+    
+
 import numpy as np
 import skimage as sk
 import matplotlib.pyplot as plt
 from matplotlib.patches import Circle
 from matplotlib.legend_handler import HandlerBase
 
 import ediff.io
 
 from skimage.measure import moments
 from skimage.transform import hough_circle, hough_circle_peaks
 
-
-import warnings
 import sys
+import warnings
 warnings.filterwarnings("ignore")
 
 
 class CenterEstimator:
     '''
     Detection of the center of diffraction patterns.
     
-    - Perform Hough transform to detect circles in image
-    - Manually selected 3 points defining a circular diffraction pattern 
-      to calculate center coordinates
-    - Visualize results
+    The center can be estimated in one of the following ways:
     
-    SUBCLASS : CenterAdjustment
-    - adjust position of the detected center 
+    * Center of the intensity/mass in selected area.
+    * Center from three points (defined interactivelly)
+      which define one ring in a powder electron diffraction pattern.
+    * Center estimated from Hough transform,
+      which detects circles in the diffraction pattern.
+    
+    SUBCLASS : CenterLocator
+    
+    * the subclass refines the position of the estimated center 
         
     Parameters
     ----------
     image_path : string
         direct path to an image with diffraction patterns
     detection_method : string
         Selection of a method for center calculation. String codes are:
@@ -59,30 +65,31 @@
     cmap : str, optional, default is 'gray'
         Name of matplotlib colormap.
         Any valid colormap ('viridis','magma') can be used.
     messages : bool, optional, default is False
         Print to terminal additional messages about program run.
     
     Returns
-    -------    
-    self.x : float64
+    -------
+    self.x : float
         x-coordinate of the detected center
-    self.y : float64
+    self.y : float
         y-coordinate of the detected center
-    self.r : float64
-        radius of the detected center (if available, othervise returns None)
-                    
+    self.r : float
+        radius of the detected center (if available, othervise returns None)        
     '''
     
     def __init__(self, input_image, 
                        detection_method = None, 
                        correction_method = None,
                        heq = False, 
                        icut = None,
                        cmap = 'gray',
+                       csquare=50,
+                       cintensity=0.8,
                        messages = False):
         
         # Initialize attributes
         self.input_image = input_image
         
         # Allow input images (np.ndarray) and image path
         if isinstance(input_image, np.ndarray):
@@ -104,23 +111,99 @@
         self.preprocess_images(preInit = 1)
 
         # Determine detection method
         if detection_method == 'manual':
             self.x, self.y, self.r = self.detection_3points()
             
         elif detection_method == 'intensity':
-            self.x, self.y, self.r = self.detection_intensity()
+            self.x, self.y, self.r = self.detection_intensity(csquare, cintensity)
 
         elif detection_method == 'hough':
             self.x, self.y, self.r = self.detection_Hough()  
         else:
             print("Incorrect method for detection selected")
             sys.exit()
+
             
+    def detection_intensity(self, csquare, cintensity, plot_results=0):
+        '''
+        Find center of intensity/mass of an array.
+        
+        Parameters
+        ----------
+        arr : 2D-numpy array
+            The array, whose intensity center will be determined.
+        csquare : int, optional, default is 20
+            The size/edge of the square in the (geometrical) center.
+            The intensity center will be searched only within the central square.
+            Reasons: To avoid other spots/diffractions and
+            to minimize the effect of possible intensity assymetry around center. 
+        cintensity : float, optional, default is 0.8
+            The intensity fraction.
+            When searching the intensity center, we will consider only
+            pixels with intensity > max.intensity.
+            
+        Returns
+        -------
+        xc,yc : float,float
+            XY-coordinates of the intensity/mass center of the array.
+            Round XY-coordinates if you use them for image/array calculations.
+        '''  
+        
+        # (1) Get image/array size
+        image = np.copy(self.to_refine)
+        arr = np.copy(image)
+        xsize,ysize = arr.shape
+        
+        # (2) Calculate borders around the central square
+        xborder = (xsize - csquare) // 2
+        yborder = (ysize - csquare) // 2
+        
+        # (3) Create the central square,
+        # from which the intensity center will be detected
+        arr2 = arr[xborder:-xborder,yborder:-yborder].copy()
+        
+        # (4) In the central square,
+        # set all values below cintenstity to zero
+        arr2 = np.where(arr2>np.max(arr2)*cintensity, arr2, 0)
+        
+        # (5) Determine the intensity center from image moments
+        # see image moments in...
+        # skimage: https://scikit-image.org/docs/dev/api/skimage.measure.html
+        # wikipedia: https://en.wikipedia.org/wiki/Image_moment -> Centroid
+        # ---
+        # (a) Calculate 1st central moments of the image
+        M = moments(arr2,1)
+        # (b) Calculate the intensity center = centroid according to www-help
+        (self.x, self.y) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
+        # (c) We have centroid of the central square
+        # but we have to recalculate it to the whole image
+        (self.x, self.y) = (self.x + xborder, self.y + yborder)
+        # (d) Radius of a diffraction ring is hardcoded to 100 here
+        # TODO: consider improving/correcting/removing in the future
+        self.r = 100
+        
+        # (6) User information (if required)
+        if self.messages:
+            print("--- IntensityCenter = center of intensity/mass ---")
+            print(f"Center coordinates [x, y]: [{self.x:.3f}, {self.y:.3f}]")
+            print("---")
+
+        # (7) Plot results (if required)
+        if plot_results == 1:
+           self.visualize_center(self.x, self.y, self.r) 
                 
+        # (8) Return the results:
+        # a) XY-coordinates of the center
+        # b) radius of the circle/diff.ring,
+        #    from which the center was determined
+        # ! radius of the circle is just hardcoded here - see TODO note above
+        return(self.x, self.y, self.r)
+
+            
     def detection_3points(self, plot_results=1):
         '''         
         In the input image, select manually 3 points defining a circle using
         a key press event 
             - press '1' to select a point
                 
         If the user is not satisfied with the point selection, it can be
@@ -167,29 +250,31 @@
         plt.rcParams['keymap.forward'].append('right')
  
         plt.title("Select 3 points defining one of diffraction circles", 
                   fontsize = 20)
         ax.imshow(im, cmap = self.cmap)
         ax.axis('off')
 
- 
         # User information:
         if self.messages:
-            print("--- Manual diffraction pattern detection ---")
+            print("--- ThreePoints = semi-automated center detection ---")
             print()
             print("Select 3 points to define a circle in the diffractogram:")
             print("Use these keys for the selection:")
             print("  - '1' : define a point at current cursor position")
             print("  - '2' : delete the last point")
             print("  - '3' : delete the point closest to the cursor")
             print("  - 'd' : done = finished = go to the next step")
             print()
             print("Close the figure to terminate. No center will be detected.")
+            print("---")
        
         # Enable interactive mode
+        # (figure is updated after every plotting command
+        # (so that calling figure.show() is not necessary
         plt.ion()
  
         # Initialize the list of coordinates
         self.coords = [] 
         
         # Initialize all flags and counters
         calculate_circle_flag = False          # press 'd' event
@@ -223,39 +308,37 @@
                     pointer_x, pointer_y = event.xdata, event.ydata
                     distances = [
                         np.sqrt((x - pointer_x)**2 + (y - pointer_y)**2)
                         for x, y in self.coords]
                     closest_index = np.argmin(distances)
                     del self.coords[closest_index]
     
-                    # Redraw the image without the deleted point
+                    ## Redraw the image without the deleted point
                     ax.clear()
                     ax.imshow(self.to_refine, cmap = self.cmap)
                     for x, y in self.coords:
-
                         ax.scatter(x, y, 
                                    c='r', marker='x', 
                                    s=self.marker_size)
 
                     my_plot_title = (
                         "Select 3 points to define "
                         "one of diffraction circles.")
                     plt.title(my_plot_title, fontsize=20)
                     
                     # Retore the previous zoom level
                     ax.set_xlim(current_xlim)
                     ax.set_ylim(current_ylim)
                     ax.axis('off')
-
- 
+                    
                     fig.canvas.draw()
                 else:
                     print("No points to delete.")
     
-            ## Delete recent point (last added) -- independent on the cursor
+            # Delete recent point (last added) -- independent on the cursor
             if event.key == '2':
                 # Check if there are points to delete
                 if point_counter > 0:  
                     point_counter -= 1
                     if len(self.coords) > 0:
                         # Delete the last point in the list
                         del self.coords[-1]
@@ -300,15 +383,15 @@
                         self.coords.append(new_point)
     
                         # Visualize the selected point on the image
                         ax.scatter(event.xdata, event.ydata, 
                                    c='r', marker='x', 
                                    s=self.marker_size)
 
-                        # Retore the previous zoom level
+                        # Restore the previous zoom level
                         ax.set_xlim(current_xlim)
                         ax.set_ylim(current_ylim)
                         ax.axis('off')
 
                         fig.canvas.draw()
     
                         point_counter += 1
@@ -336,16 +419,15 @@
         cid0 = fig.canvas.mpl_connect('key_press_event', onkeypress)
 
         # Show the plot
         plt.tight_layout()
         ax.axis('off')
 
         plt.show(block=False)
-
-        
+      
         # Wait for 'd' key event or close the figure if no points are selected
         while not calculate_circle_flag and not termination_flag:
  
             try:
                 plt.waitforbuttonpress(timeout=0.1)
                 # Store the zoom level
                 current_xlim = ax.get_xlim()
@@ -357,16 +439,15 @@
                     self.calculate_circle(plot_results=0)
                     
                     ax.clear()
                     ax.imshow(self.to_refine, cmap = self.cmap)
                     # Retore the previous zoom level
                     ax.set_xlim(current_xlim)
                     ax.set_ylim(current_ylim)
-                
- 
+                 
                     circle = plt.Circle(
                         (self.x, self.y), self.r, color='r', fill=False)
                     ax.add_artist(circle)
         
                     # Plot center point
                     center, = ax.plot(self.x, self.y, 'rx', markersize=12)
                     plt.title('Manually adjust the position of the center using keys.')
@@ -379,34 +460,36 @@
 
             except KeyboardInterrupt:
                 print("Execution manually interrupted by user.")
                 break
             except ValueError as e:
                 print("ValueError:", e)
                 break
-
-            
+           
         # If the termination_flag is True, stop the code
         if termination_flag: 
              print("No points selected. Returned None values.")
              sys.exit()
              return None, None, None
         
         # Disconnect key press events
         fig.canvas.mpl_disconnect(cid0) 
         
         # local variables save
         self.center = center
         
-        
+        self.backip = [self.x, self.y, self.r]
         # Manually adjust the calculated center coordinates
         self.x, self.y, self.r = self.adjustment_3points(fig, circle, center)
 
- 
-        return self.x, self.y, self.r
+        # Return the results:
+        # a) XY-coordinates of the center
+        # b) radius of the circle/diff.ring,
+        #    from which the center was determined
+        return(self.x, self.y, self.r)
 
     
     def adjustment_3points(self, fig, circle, center, plot_results=0):
         '''
         Adjustment of the center position calculated from 3 points.
         Interactive refinement using keys:
 
@@ -535,15 +618,15 @@
         # Wait for 'd' key press or figure closure
         while not termination_flag:
             try:
                 plt.waitforbuttonpress(timeout=0.1)
             except KeyboardInterrupt:
                 # If the user manually closes the figure, terminate the loop
                 termination_flag = True
-         
+                
         # Turn off interactive mode
         plt.ioff()
         
         # Display the final figure with the selected center position and radius
         plt.tight_layout()
 
         plt.show(block=False)
@@ -555,82 +638,16 @@
         # Print results
         if self.messages:
             print("CenterEstimator :: manual detection + adjustment")
             print(f"Center coordinates: {xy[0]:.2f} {xy[1]:.2f}")
         
     
         return xy[0], xy[1], r
-        
-        
-    def detection_intensity(self, csquare=20, cintensity=0.5, plot_results=0):
-        '''
-        Find center of intensity/mass of an array.
-        
-        Parameters
-        ----------
-        arr : 2D-numpy array
-            The array, whose intensity center will be determined.
-        csquare : int, optional, default is 20
-            The size/edge of the square in the (geometrical) center.
-            The intensity center will be searched only within the central square.
-            Reasons: To avoid other spots/diffractions and
-            to minimize the effect of possible intensity assymetry around center. 
-        cintensity : float, optional, default is 0.8
-            The intensity fraction.
-            When searching the intensity center, we will consider only
-            pixels with intensity > max.intensity.
-            
-        Returns
-        -------
-        xc,yc : float,float
-            XY-coordinates of the intensity/mass center of the array.
-            Round XY-coordinates if you use them for image/array calculations.
-        '''  
-        
-        # Get image/array size
-        image = np.copy(self.to_refine)
-        arr = np.copy(image)
-        xsize,ysize = arr.shape
-        
-        # Calculate borders around the central square
-        xborder = (xsize - csquare) // 2
-        yborder = (ysize - csquare) // 2
-        
-        # Create central square = cut off the borders
-        arr2 = arr[xborder:-xborder,yborder:-yborder].copy()
-        
-        # In the central square, set all values below cintenstity to zero
-        arr2 = np.where(arr2>np.max(arr2)*cintensity, arr2, 0)
-        
-        # Calculate 1st central moments of the image
-        M = moments(arr2,1)
-        
-        # Calculate the intensity center = centroid according to www-help
-        (self.x, self.y) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
-        
-        # We have centroid of the central square => recalculate to whole image
-        (self.x, self.y) = (self.x + xborder, self.y + yborder)
-        self.r = 100
-        
-        # User information:
-        if self.messages:
-            print("--------- Diffraction pattern detection via intensity detection ----------")
-            print("Central coordinate [ x, y ]: [{:.3f}, {:.3f}]".format(float(self.x), 
-                                                                         float(self.y)))
-            print("--------------------------------------------------------------------------")
-
-        # Plot result of the Hough transform
-        if plot_results == 1:
-           self.visualize_center(self.x, self.y, self.r) 
-        
-        
-        # Return results
-        return self.x, self.y, self.r
-
     
+        
     def detection_Hough(self, plot_results=0):
         '''        
         Perform Hough transform to detect center of diffraction patterns.
         This is a method to automatically detect circular diffraction patterns
         
         Parameters
         ----------
@@ -808,17 +825,15 @@
                        ncol=2, 
                        bbox_to_anchor=(0.5,-0.1), 
                        mode='expand', 
                        frameon=False)
             plt.axis('off')
             plt.tight_layout()
             plt.show(block=False)
-        else:
-            pass
-            #plt.close('all')
+
         
         self.center = (self.x, self.y)
         self.circle = plt.Circle((self.x,self.y),self.r)
         
 
         return self.x, self.y, self.r, self.center, self.circle
 
@@ -931,15 +946,15 @@
             - 'manual' : manual detection via 3 points
             - 'intensity' : detection via maximum intensity
             - 'hough' : automatic detection via Hough transform
     correction_method : string
        Selection of a method for center position correction. Default is None.
        String codes are:
            - 'manual' : manual corection 
-           - 'variance' : correction via variance minimization 
+           - 'var' : correction via variance minimization 
            - 'sum' : correction via sum maximization
     heq : boolean
         Allow histogram equalization. The default is 0 (no enhancement)
     icut : boolean
         Allow image enhancement. The default is 0 (no enhancement)
 
 
@@ -949,55 +964,71 @@
         adjusted x-coordinate of the detected center
     self.yy : int32
         adjusted y-coordinate of the detected center
     self.rr : int32
         radius of the detected center
     '''
     
+
     def __init__(self, image_path,
                  detection_method, correction_method=None, 
                  heq=False, icut=None, cmap='gray',
                  messages=False, final_replot=False):
         
         # (1) Call the constructor of the base class to initialize its methods
         super().__init__(image_path,
             detection_method, correction_method,
             heq=heq, icut=icut, cmap=cmap, messages=messages)
         
 
         # (2) Define additional parameter
-        self.final_replot = final_replot
         self.messages = messages
         self.image_path = image_path
 
 
         # (3) Run correction method and get refined parameters
         if correction_method is not None:
             self.ret = 1
             if correction_method == 'manual':
                 if detection_method == 'manual':
-                    self.xx, self.yy, self.rr = self.x, self.y, self.r
-                    self.x, self.y, self.r = self.backip[0], self.backip[1], self.r
-                    if self.final_replot:
-                        self.visualize_refinement(
-                            self.backip[0], self.backip[1], self.r, 
-                            (self.xx, self.yy), self.r)
+                    self.yy, self.xx, self.rr = self.x, self.y, self.r
+                    self.y, self.x, self.r = self.backip[0], self.backip[1], self.r
+                elif detection_method == 'intensity':
+                    self.yy, self.xx, self.rr = \
+                        self.ref_interactive(self.y, self.x, self.r)
                 else:
-                    self.xx, self.yy, self.rr = \
+                    self.yy, self.xx, self.rr = \
                         self.ref_interactive(self.x, self.y, self.r)
-            elif correction_method == 'variance':
+                        
+            elif correction_method == 'var':
                 self.xx, self.yy, self.rr = \
-                    self.ref_minimize_var(self.x, self.y, self.r)
+                    self.ref_var(self.x, self.y, self.r)
+                if detection_method == 'manual':
+                    self.xx, self.yy = self.yy, self.xx
+                    self.x, self.y = self.y, self.x
+                    
             elif correction_method == 'sum':
                 self.xx, self.yy, self.rr = \
-                    self.ref_maximize_sum(self.x, self.y, self.r)
+                    self.ref_sum(self.x, self.y, self.r)
+                if detection_method == 'manual':
+                    self.xx, self.yy = self.yy, self.xx
+                    self.x, self.y = self.y, self.x
+
             else:
                 print("Incorrect method for correction selected")
                 sys.exit()
+            
+            if detection_method == 'hough':
+                self.x, self.y = self.y, self.x
+                self.xx, self.yy = self.yy, self.xx
 
+            if final_replot:
+                self.visualize_refinement(
+                    self.y, self.x, self.r, 
+                    (self.yy, self.xx), self.rr)
         else:
             self.ret = 2
 
 
     def preprocess_images(self, preInit=0, preHough=0, preManual=0, preVar = 0, 
                           preSum = 0, preInt=0):
         """
@@ -1216,18 +1247,17 @@
         Returns
         -------
         x : float
             x-coordinate of the center detected via detection_method
         y : float
             y-coordinate of the center detected via detection_method
         xx : float
-            x-coordinate of the center detected via correction_method
+            x-coordinate of the center detected via refinement_method
         yy : float
-           y-coordinate of the center detected via detection_method
-           
+            y-coordinate of the center detected via refinement_method
         """
         
         if self.ret == 1:
             # Convert to float
             if type(self.x) != float:
                 self.x, self.y, self.xx, self.yy, self.r, self.rr = \
                     [float(value) for value in (self.x, self.y, 
@@ -1281,14 +1311,15 @@
         x : float64
             new x-coordinate of the center
         y : float64
             new y-coordinate of the center
         r : float64
             new radius of the circular diffraction pattern
         '''
+        
         # Load original image
         im = np.copy(self.to_refine)
         
         # Initialize variables and flags
         xy = np.array((px, py))
         r = np.copy(pr)
         termination_flag = False
@@ -1317,15 +1348,15 @@
         plt.rcParams['keymap.forward'].append('right')
         
         circle = plt.Circle(
             (px, py), pr, color='r', fill=False)
         ax.add_artist(circle)
 
         # Plot center point
-        center, = ax.plot(self.x, self.y, 'rx', markersize=12)
+        center, = ax.plot(px, py, 'rx', markersize=12)
                     
 
         plt.title('Manually adjust the center position.', 
                   fontsize=20)
 
         ax.imshow(im, cmap = self.cmap)
         ax.axis('off')
@@ -1422,23 +1453,19 @@
         if termination_flag: 
             plt.close()  # Close the figure
 
         # Print results
         if self.messages:
             print("CenterEstimator :: manual detection + adjustment")
             print(f"Center coordinates: {xy[0]:.2f} {xy[1]:.2f}")
-        
-        # Plot results
-        if self.final_replot:
-            self.visualize_refinement(px, py, pr, xy, r)
-                
+                       
         return xy[0], xy[1], r
 
         
-    def ref_minimize_var(self, px, py, pr, plot_results = 0):
+    def ref_var(self, px, py, pr, plot_results = 0):
         '''         
         Adjust center coordinates of a detected circular diffraction pattern.
         The center adjustment is based on variance minimization.
         
         The 8-neighbourhood pixels (x) of the current center (o) 
         will be tested regarding the minimization:
     
@@ -1583,29 +1610,24 @@
             or  (bckup[0] < bckup[1] and not best_center[0] < best_center[1])):
             best_center = best_center[::-1]
         
         ## (2) worsened final maximum intensity sum than the initial one
         if np.round(init_var,-2) < np.round(min_intensity_var,-2):
             print("Refinement redundant.")
             best_center = np.copy(bckup)
-
-        # Refinement visualization
-        if self.final_replot:
-            self.visualize_refinement(
-                   bckup[0], bckup[1], bckup[2], (best_center), best_radius)
     
         # Print results
         if self.messages:
             print("CenterLocator: manual detection + adjustment:")
             print(f"Estimated center {px:.2f} {py:.2f}")
                 
         return best_center[0], best_center[1], best_radius
     
     
-    def ref_maximize_sum(self, px, py, pr, plot_results=1):
+    def ref_sum(self, px, py, pr, plot_results=1):
         ''' 
         Adjust center position based on gradient optimization method
         via maximization of intensity sum.
         
         The 8-neighbourhood pixels (x) of the current center (o) 
         will be tested regarding the maximization:
     
@@ -1750,20 +1772,14 @@
             or  (bckup[0] < bckup[1] and not best_center[0] < best_center[1])):
             best_center = best_center[::-1]
         
         ## (2) worsened final maximum intensity sum than the initial one
         if np.round(init_sum,-2) > np.round(max_intensity_sum,-2):
             print("Refinement redundant.")
             best_center = np.copy(bckup)
-
-        # Refinement visualization
-        if plot_results == 1:
-            if self.final_replot:
-                self.visualize_refinement(
-                    bckup[0], bckup[1], bckup[2], (best_center), best_radius)
     
         # Print results
         if self.messages:
             print("CenterLocator: manual detection + adjustment:")
             print(f"Estimated center {px:.2f} {py:.2f}")
                 
         return best_center[0], best_center[1], best_radius
@@ -1946,15 +1962,14 @@
         marker = Circle((x, y), r, facecolor=orig_handle.get_facecolor(),
                         edgecolor=orig_handle.get_edgecolor(),
                         linewidth=orig_handle.get_linewidth(),
                         transform=trans)
         return [marker]
         
 
-        
 class IntensityCenter: 
     '''
     Simple center determination for a symmetric diffractogram.
     
     * The center is determined as a center of intensity.
     * This works well for simple, symmetric diffraction patters, which are:
       (i) without beamstopper, (ii) pre-centered, and (iii) powder-like.
@@ -1973,15 +1988,15 @@
     >>>     arr, csquare=30, cintensity=0.8)
     >>>
     >>> # (2) New way = newer (and more universal) CenterLocator class:
     >>> xc,yc = ediff.center.CenterLocator(
     >>>     arr, detection_method='intensity', csquare=30, cintensity=0.8)
     '''
     
-    
+    @staticmethod
     def center_of_intensity(arr, csquare=20, cintensity=0.8):
         '''
         Find center of intensity/mass of an array.
         
         Parameters
         ----------
         arr : 2D-numpy array
@@ -2013,10 +2028,11 @@
         arr2 = np.where(arr2>np.max(arr2)*cintensity, arr2, 0)
         # Calculate 1st central moments of the image
         M = sk.measure.moments(arr2,1)
         # Calculate the intensity center = centroid according to www-help
         (xc,yc) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
         # We have centroid of the central square => recalculate to whole image
         (xc,yc) = (xc+xborder,yc+yborder)
+        
         ## Return the final center
         return(xc,yc)
```

### Comparing `ediff-0.2/src/ediff/io.py` & `ediff-0.2.2/src/ediff/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-Module ediff.io
----------------
+Module: ediff.io
+----------------
 Input/output functions for package ediff.    
 '''
 
 from PIL import Image
 
 import numpy as np
 import matplotlib.pyplot as plt
@@ -64,21 +64,22 @@
         size = (size[0]/2.54, size[1]/2.54)
         plt.rcParams.update({'figure.figsize' : size})
     if dpi:  # Figure dpi
         plt.rcParams.update({'figure.dpi' : dpi})
     if fontsize:  # Global font size
         plt.rcParams.update({'font.size' : fontsize})
     # (2) Additional default parameters ---------------------------------------
-    plt.rcParams.update({
-        'lines.linewidth'    : 0.8,
-        'axes.linewidth'     : 0.6,
-        'xtick.major.width'  : 0.6,
-        'ytick.major.width'  : 0.6,
-        'grid.linewidth'     : 0.6,
-        'grid.linestyle'     : ':'})
+    if my_defaults:  # Default rcParams if not forbidden by my_defaults=False
+        plt.rcParams.update({
+            'lines.linewidth'    : 0.8,
+            'axes.linewidth'     : 0.6,
+            'xtick.major.width'  : 0.6,
+            'ytick.major.width'  : 0.6,
+            'grid.linewidth'     : 0.6,
+            'grid.linestyle'     : ':'})
     # (3) Further user-defined parameter in rcParams format -------------------
     if my_rcParams:  # Other possible rcParams in the form of dictionary
         plt.rcParams.update(my_rcParams)
 
 
 def plot_radial_distributions(
         data_to_plot, xlimit, ylimit, output_file=None):
@@ -110,21 +111,25 @@
 
     Returns
     -------
     Nothing
         The output is the plot on screen
         (and in *output file* if the *output* argument was given).
     
-    Technical note
-    --------------
-    This function is quite flexible.
-    It can plot one radial distribution or more.
-    It can take data from PNG-files, TXT-files, 2D-arrays and 1D-arrays.
-    This makes the code a bit more complex, but it is convenient for the user.
-    A fast comparison of three 1D-distributions from three 2D-diffractograms:
+    Technical notes
+    ---------------
+    * This function is quite flexible.
+    * It can plot one radial distribution or more.
+    * It can take data from PNG-files, TXT-files, 2D-arrays and 1D-arrays.
+    * If the input is a PNG-file or2D-array,
+      the center is just *estimated* as as the center of intensity;
+      therefore, this works only for good diffractograms with a central spot.
+    * This makes the code a more complex, but it is convenient for the user.
+    * An example of fast comparison of three 1D-distributions
+      taken from three 2D-diffractograms in the form of 16-bit PNG images:
     
     >>> ediff.io.plot_radial_distributions(
     >>>     data_to_plot = [
     >>>         ['sum_all_16bit.png', 'k:',  'All data'],
     >>>         ['sum_f_16bit.png',   'b--', 'F data'],
     >>>         ['sum_fd_16bit.png',  'r-',  'FD data']]
     >>>     xlimit=200, ylimit=300,
```

### Comparing `ediff-0.2/src/ediff/pxrd.py` & `ediff-0.2.2/src/ediff/pxrd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 '''
-Module ediff.pxrd
------------------
+Module: ediff.pxrd
+------------------
 Calculation of powder X-ray diffraction patterns.    
 '''
 
 import sys
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy.signal import convolve as spConvolve
 from pymatgen.core.structure import Structure as pmStructure
 from pymatgen.analysis.diffraction.xrd import XRDCalculator as pmXRDCalculator
 
+
 class Crystal:
     '''
     Define crystal structure.
     
     Parameters
     ----------
     structure : structure object
@@ -34,14 +35,15 @@
         * Temperature factors characterize thermal movement of atoms.
         * If a float value is given,
           all elements have this temperature factor value.
         * If a dictionary is given,
           the elements have the values defined in the dictionary;
           a sample input dictionary: `temp_factors = {'Na':1.2, 'Cl':1.1}`.
     '''
+
     
     def __init__(self, structure, temp_factors=0.8):
         '''
         * Initialize Crystal object.
         * The parameters are described above in class definition.
         '''
         # (1) Define structure
@@ -56,14 +58,15 @@
             # Temperature factors were given as dictionary
             self.temp_factors = temp_factors
         else:
             # Temp.factors are not dictionary => we suppose a number
             # (the number is a universal temperature factor for all atoms
             self.temp_factors = self.get_elements_with_temp_factors(
                 self.structure, temp_factors)
+
     
     @staticmethod
     def read_structure_from_CIF(CIF):
         '''
         Read crystall structure from CIF file.
 
         Parameters
@@ -82,14 +85,15 @@
               *pymatgen.core.structure.Structure*.
             * Nevertheless, in the structure objects are usually
               created from CIF files (pymatgen is hidden for a common user).
          '''
         structure = pmStructure.from_file(CIF)
         return(structure)
 
+
     def get_elements(self, structure):
         '''
         Get a list of all elements, which are contained in given structure.
 
         Parameters
         ----------
         structure : structure object
@@ -118,14 +122,15 @@
         list_of_atoms = []
         for site in structure:
             for sp, occu in site.species.items():
                 list_of_atoms.append(sp.symbol)
         list_of_elements = np.unique(list_of_atoms)
         return(list_of_elements)
 
+
     def get_elements_with_temp_factors(self, structure, B=0.8):
         '''
         Get a dictionary, which contains symbols and temperature factors
         of all elements, which are present in given structure.
 
         Parameters
         ----------
@@ -150,35 +155,41 @@
         * The function is just used internally, when setting
           temperature factors of the elements contained in given *structure*.
          '''
         elements = self.get_elements(structure)
         elements_with_temp_factors = dict.fromkeys(elements, B)
         return(elements_with_temp_factors)
 
+
+
 class Experiment:
     '''
     Define experimental parameters.
     
     Parameters
     ----------
     wavelength : float
         Wavelength of the X-rays.
         Typical values are 1.54 A (CuKa) or 0.71 A (MoKa).
     two_theta_range: list/tuple of two floats
         Minimal and maximal diffraction angle;
         both values are TwoTheta angle in [deg] (for given *wavelength*).
     '''
+
+
     def __init__(self, wavelength, two_theta_range):
         '''
         * Initialize Experimental object.
         * The parameters are described above in class definition.
         '''
         self.wavelength = wavelength
         self.two_theta_range = two_theta_range
 
+
+
 class PlotParameters:
     '''
     Define local+global parameters for plotting.
     
     Parameters
     ----------
     title : str
@@ -187,34 +198,38 @@
         Quantity for X-axis.
     rcParams : dict; optional, the default is empty dictionary {}
         The dictionary should have the format of mathplotlib.pyplot.rcParams.
         The argmument is passed to matplotlib.pyplot.rcParams.update.
         This enables to override current rcParams, if necessary.
     '''
     
+
     def __init__(self, title=None, x_axis='q', xlim=None, rcParams={}):
         '''
         * Initialize PlotParameters object.
         * The parameters are described above in class definition.
         '''
         
         # Initialize basic parameters
         self.title = title
         self.x_axis = x_axis
         self.xlim = xlim
         if rcParams: plt.rcParams.update(rcParams)
        
+
+
 class PeakProfiles:
     '''
     Define profile of diffraction peaks.
 
     * This class is employed only as a namespace.
     * It contains three functions/definitions of diffratction peak profiles.
     '''
 
+
     def gaussian(X,m,s):
         '''
         Gaussian function (~ profile for PXRD calculation).
     
         Parameters
         ----------
         X : numpy array
@@ -227,14 +242,15 @@
         Returns
         -------
         NumPy array
             The array with Y-values of the function; Y = Gaussian(X).
         '''
         return( 1/(s*np.sqrt(2*np.pi)) * np.exp(-(X-m)**2/(2*s**2)) )
     
+
     def lorentzian(X,m,s):
         '''
         Lorentzian function (~ profile for PXRD calculation).
     
         Parameters
         ----------
         X : numpy array
@@ -247,14 +263,15 @@
         Returns
         -------
         NumPy array
             The array with Y-values of the functin; Y = Lorenzian(X).
         '''
         return( 1/np.pi * s/((X-m)**2 + s**2) )
     
+
     def pseudo_voigt(X,m,s,n=0.5):
         '''
         Pseudo-Voigt function (~ profile for PXRD calculation).
     
         Parameters
         ----------
         X : numpy array
@@ -292,14 +309,16 @@
         # (Pseudo-Voigt = n * Gausian + (1-n) * Lorenzian)
         pseudo_voigt = \
             n * PeakProfiles.gaussian(X,m,sg) \
             + (1-n) * PeakProfiles.lorentzian(X,m,s)
         # (3) Return calculated function    
         return(pseudo_voigt)
 
+
+
 class PXRDcalculation:
     '''
     Define calculation of PXRD = powder X-ray diffraction pattern.
     
     Parameters
     ----------
     crystal : ediff.pxrd.Crystal object
@@ -319,15 +338,16 @@
         while for more realistic diffractograms it may be slightly increased. 
     peak_profile_type : None or ediff.pxrd.PeakProfiles object, optional
         Profile of the calculated diffraction peaks.
         The default is PeakProfiles.pseudo_voigt.
         This default is suitable for common calculations
         and does not have to be changed (in great majority of cases).
     '''
-  
+
+    
     def __init__(self, crystal, experiment, plot_parameters,      
                  peak_profile_sigma = 0.03,
                  peak_profile_type = PeakProfiles.pseudo_voigt):
         '''
         Initialize PXRDcalcualtion object.
         The parameters are described above in class definition.
         '''
@@ -335,28 +355,30 @@
         self.experiment = experiment
         self.plot_parameters = plot_parameters
         self.peak_profile_sigma = peak_profile_sigma
         self.peak_profile_type = peak_profile_type 
         self.diffractions = self.calculate_diffractions()
         self.diffractogram = self.calculate_diffractogram()
 
+
     def calculate_diffractions(self):
         # (1) Calculate intensities
         calculation = pmXRDCalculator(
             wavelength = self.experiment.wavelength,
             debye_waller_factors=(self.crystal.temp_factors))
         diffractions = calculation.get_pattern(
             self.crystal.structure,
             two_theta_range = self.experiment.two_theta_range)
         # (2) Transform diffractions: PyMatGen structure => pd.DataFrame
         diffractions_df = self.diffractions_to_dframe(diffractions)
         # (3) Return calculated diffractions
         # (pandas.DataFrame with cols: TwoTheta, h,k,l, dhkl, S, q, Intensity
         return(diffractions_df)
         
+
     def calculate_diffractogram(self):
         # (1) Base diffraction profile
         # = diffractogram with zero intensities
         # = interval theta_min to theta_max with step=0.001, zero intensities
         th1,th2 = th1,th2 = self.experiment.two_theta_range
         numpoints = (th2-th1) * 100 + 1
         diffractogram_2theta = np.linspace(th1, th2, numpoints, endpoint=True)
@@ -398,21 +420,23 @@
         # (4) Final diffraction profile
         # = diffraction profile with additional columns (S,q)
         # = original cols (TwoTheta, Intensity) => (TwoTheta,S,q,Intensity)
         df = self.add_diffraction_vectors_to_diffractogram(df)
         # (5) Return diffractogram
         return(df)
         
+
     def print_diffractions(self):
         '''
         Print the calculated diffractions to stdout.
         '''
         table = PXRDcalculation.dframe_to_table(self.diffractions)
         print(table)
             
+
     def save_diffractions(self, output_file):
         '''
         Save the calculated diffractions to *output_file*.
         
         Parameters
         ----------
         output_file : str
@@ -425,46 +449,55 @@
         try:
             with open(output_file, 'w') as fh:
                 table = PXRDcalculation.dframe_to_table(self.diffractions)
                 print(table, file=fh)
         except:
             print(f'Error saving diffractions to {output_file}!')
     
+
     def plot_diffractions(self, outfile=None):
         '''
         Plot the calculated diffractions.
         
         Parameters
         ----------
         outfile : str, optional, the default is none
             Name of the output file.
             If not given, the plot is just shown, but not saved.
 
         Returns
         -------
-        * None; the output is the plot on the screen (and outfile).
-        * Note that the plot shows just diffraction intensities, not profiles.
-        * Use *plot_diffractogram* for diffractogram with intensity profiles.
+        None
+            The output is the plot on the screen (and outfile).
+            This function plots just diffraction intensities,
+            not profiles.
+            Use ediff.pxrd.plot_diffractions
+            for diffractogram with intensity profiles.
         '''
+        
         # (1) Make local copies of pre-defined parameters (just convenience)
         df      = self.diffractions
         x_axis  = self.plot_parameters.x_axis
+        
         # (2) Prepare the plot
         plt.vlines(df[x_axis],0,df.Ihkl, lw=2)
+        
         # (3) Set plot details
         # (external function, common to diffractions and diffractogram plots
         self.set_plot_details(x_axis)
+        
         # (4) Save/show the plot...
         # In Spyder: plot is always shown
         # In CLI: plot is saved (if outfile is defined) or it is just shown
         if outfile != None: 
             plt.savefig(outfile) 
         else:
             plt.show()
         
+
     def plot_diffractions_with_indexes(self):
         '''
         Plot indexed diffractions.
         
         Important - interactive plots in Spyder
         ---------------------------------------
         * This function can create interactive plot.
@@ -529,46 +562,54 @@
         ax.xaxis.set_minor_locator(AutoMinorLocator(5))
         # (5) Final adjustments
         fig.tight_layout()
         fig.show()
         # (6) Revert to original rcParams.
         plt.rcParams.update(original_rcParams)
         
+
     def print_diffractogram(self):
         self.print_diffractions()
         print('-----')
         print('* Just diffraction intensities, not the whole pattern.')
         print('* Reason: the whole diffraction pattern is too long.')
         print('* Note: save_diffractogram save the pattern to TXT-file.')
     
+
     def save_diffractogram(self, outfile):
         my_title = 'Calculated PXRD diffractogram\n'
         np.savetxt(
             outfile,
             np.array(self.diffractogram),
             fmt = ['%6.2f','%8.4f','%8.4f','%8.4f'],
             header = my_title + 
                 'Columns: TwoTheta[deg], S[1/A], q[1/A], Intensity')
     
-    def plot_diffractogram(self, outfile, x_axis='q'):
+
+    def plot_diffractogram(self, outfile, x_axis='q', dpi=300):
+        
         # (1) Make local copies of pre-defined parameters (just convenience)
         df     = self.diffractogram
         x_axis = self.plot_parameters.x_axis
+        
         # (2) Prepare the plot
         plt.plot(df[x_axis],df.Intensity)
+        
         # (3) Set plot details
         # (external function, common to diffractions and diffractogram plots
         self.set_plot_details(x_axis)
+        
         # (4) Save/show the plot...
         # In Spyder: plot is always shown
         # In CLI: plot is saved (if outfile is defined) or it is just shown
         if outfile != None: 
-            plt.savefig(outfile) 
+            plt.savefig(outfile, dpi=dpi) 
         else:
             plt.show()
+
         
     @staticmethod    
     def diffractions_to_dframe(intensities):
         # Prepare hkl indexes
         h = []; k = []; l = []
         # Test if the structure is hexagonal
         hexagonal = (len(intensities.hkls[0][0]['hkl']) == 4)
@@ -598,14 +639,15 @@
                 np.transpose(
                     [intensities.x,
                      h, k, i, l, intensities.d_hkls, intensities.y]),
                 columns=['TwoTheta','h','k','i', 'l','dhkl','Ihkl'])
             df.insert(loc=6, column='S', value=1/df.dhkl)
             df.insert(loc=7, column='q', value=2*np.pi*df.S)
         return(df)
+
     
     @staticmethod
     def dframe_to_table(dframe):
         # POZOR: parametr formatters je zaludny!
         # * musi to byt sada funkci, takze...
         #   NEfunguji string-formaty '%.3f' - nejsou to funkce
         #   NEfunguji f-stringy - nelze prazdne - f'{8.3f}' ani f'{:8.3f}'
@@ -645,28 +687,30 @@
                     'l'        : '{:3.0f}'.format,
                     'dhkl'     : '{:7.3f}'.format,
                     'S'        : '{:7.3f}'.format,
                     'q'        : '{:7.3f}'.format,
                     'Ihkl'     : '{:9.3f}'.format})
         return(table)
 
+
     def add_diffraction_vectors_to_diffractogram(self, df):
         # Prepare wavelenght (just shortcut for convenience)
         wavelength = self.experiment.wavelength
         # Insert a column with the calculated values of diffration vector S
         df.insert(loc = 1,
                   column = 'S',
                   value = 2*np.sin(df.TwoTheta/2*np.pi/180) / wavelength)
         # Insert a column with the calculated values of difraction vector q
         df.insert(loc = 2,
                   column = 'q',
                   value = 2*np.pi * df.S)
         # Return the modified/extended DataFrame
         return(df)
 
+
     def set_plot_details(self, x_axis):
         # (1) Make local copies of pre-defined parameters (just convenience)
         title   = self.plot_parameters.title
         x_axis  = self.plot_parameters.x_axis
         my_xlim = self.plot_parameters.xlim
         # (2) Set plot title (only if it is defined)
         if title != None: plt.title(title)
```

### Comparing `ediff-0.2/src/ediff/radial.py` & `ediff-0.2.2/src/ediff/radial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-Module ediff.radial
--------------------
+Module: ediff.radial
+--------------------
 The conversion of a 2D powder diffraction pattern
 to a 1D powder diffraction pattern = radially averaged intensity distribution.
 '''
 
 import numpy as np
 import ediff.center
```

### Comparing `ediff-0.2/src/ediff.egg-info/PKG-INFO` & `ediff-0.2.2/src/ediff.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.2
+Version: 0.2.2
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -14,32 +14,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 EDIFF :: processing of powder electron diffraction patterns
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
-	- bkgr = background subtraction
+	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
-	- radial = calculate radial distribution (2D-pattern to 1D-pattern) 
+	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
 
 Installation
 ------------
-* `pip install bground` = interactive background subtraction
-* `pip install ediff`   = EDIFF program itself (uses bground internally)
+* Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
+* `pip install scikit-image` = 3rd party package for advanced image processing 
+* `pip install pymatgen` = 3rd party package employed in PXRD calculation
+* `pip install bground`= our package, interactive background subtraction
+* `pip install ediff` = EDIFF package itself (uses all packages above)
 
 Quick start
 -----------
 * See how it works:
-	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
+	- Look at [worked example](https://www.dropbox.com/scl/fi/3hb78voxd17wb3fzh9n1p/01_ediff_au.nb.pdf?rlkey=qmbvwaw80o1gbe262hwgjvmgx&dl=0)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
-	- Look at `00readme.txt` and run the example in Jupyter.
+	- Download [complete examples with data](https://www.dropbox.com/scl/fo/td6rkdgp2usxosj1vqeku/h?rlkey=41carfdej5h2f8f4yscbuvagm&dl=0)
+	  and scripts and basic instructions.
+	- After downloading, unzip it and follow the instructions in *readme* file.
 
 Documentation, help and examples
 --------------------------------
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/ediff/)
   with [documentation](https://mirekslouf.github.io/ediff/docs).
@@ -47,11 +51,12 @@
 Versions of EDIFF
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
-* Version 0.1.0 = 1st semi-complete version with basic documentation
-* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
-* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
+* Version 0.1   = 1st semi-complete version with basic documentation
+* Version 0.1.1 = improved/simplified outputs
+* Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
+* Version 0.2.2 = consolidation, update of docs and examples on www
```

