# Comparing `tmp/wedap-0.0.8.tar.gz` & `tmp/wedap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedap-0.0.8.tar", last modified: Tue Sep 19 16:33:41 2023, max compression
+gzip compressed data, was "wedap-0.0.9.tar", last modified: Fri Sep 22 19:15:53 2023, max compression
```

## Comparing `wedap-0.0.8.tar` & `wedap-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.472569 wedap-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-09-19 16:33:09.000000 wedap-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-19 16:33:41.472569 wedap-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2023-09-19 16:33:09.000000 wedap-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.468569 wedap-0.0.8/mdap/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/md_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.468569 wedap-0.0.8/mdap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:09.000000 wedap-0.0.8/mdap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 16:33:41.472569 wedap-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-09-19 16:33:09.000000 wedap-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.468569 wedap-0.0.8/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:09.000000 wedap-0.0.8/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.472569 wedap-0.0.8/wedap/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-19 16:33:09.000000 wedap-0.0.8/wedap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-09-19 16:33:09.000000 wedap-0.0.8/wedap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21191 2023-09-19 16:33:09.000000 wedap-0.0.8/wedap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    54424 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21058 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.472569 wedap-0.0.8/wedap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.472569 wedap-0.0.8/wedap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/tests/make_h5_plot_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/tests/test_h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-09-19 16:33:10.000000 wedap-0.0.8/wedap/tests/test_h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 16:33:41.472569 wedap-0.0.8/wedap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-19 16:33:41.000000 wedap-0.0.8/wedap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.281544 wedap-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-09-22 19:15:11.000000 wedap-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-22 19:15:53.277544 wedap-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2023-09-22 19:15:11.000000 wedap-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/md_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/make_md_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/test_md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 19:15:53.281544 wedap-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-09-22 19:15:12.000000 wedap-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:12.000000 wedap-0.0.9/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21191 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54756 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21016 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/make_h5_plot_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/test_h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/test_h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/top_level.txt
```

### Comparing `wedap-0.0.8/LICENSE` & `wedap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/PKG-INFO` & `wedap-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 0.0.8
+Version: 0.0.9
 Summary: weighted ensemble data analysis and plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
```

### Comparing `wedap-0.0.8/README.md` & `wedap-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/mdap/__main__.py` & `wedap-0.0.9/mdap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/mdap/command_line.py` & `wedap-0.0.9/mdap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/mdap/md_pdist.py` & `wedap-0.0.9/mdap/md_pdist.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                  *args, **kwargs):
         """
         TODO: add XYZ interval to proc (default 1)
 
         Parameters
         ----------
         data_type : str
-            'timeseries' for 1 dataset, or 'pdist' for 2D. scatter for 3d? (TODO)
+            'time' for 1 dataset timeseries, or 'pdist' for everything else.
         Xname : str or list of str
             target data for x axis, default None.
         Xindex : int
             If X.ndim > 2, use this to index.
         Yname : str or list of str
             target data for y axis, default None.
         Yindex : int
@@ -68,16 +68,16 @@
             Optionally put custom bin ranges.
         no_pbar : bool
             Optionally do not include the progress bar for pdist generation.
         timescale : int
             Default ps to µs (10**6). Converts frames to time.
         TODO: maybe also binsfromexpression?
         """
-        if data_type is None or data_type not in ["timeseries", "pdist"]:
-            raise ValueError("Must input valid data_type str: `timeseries` or `pdist`")
+        if data_type is None or data_type not in ["time", "pdist"]:
+            raise ValueError("Must input valid data_type str: `time` or `pdist`")
         else:
             self.data_type = data_type
         self.p_units = p_units
         self.T = T
 
         self.Xname = Xname
         self.Xindex = Xindex
@@ -169,15 +169,15 @@
         #X = X[np.logical_not(np.isnan(X))]
 
         # numpy equivalent to: ax.hist2d(c2[:,1], aux)
         hist, x_edges = np.histogram(X, bins=self.bins[0], range=self.histrange_x)
         # let each row list bins with common y range
         hist = np.transpose(hist)
         # convert histogram counts to p_units
-        hist = self._normalize(hist)
+        hist = self._normalize(hist, self.p_units)
         # get bin midpoints
         midpoints_x = (x_edges[:-1] + x_edges[1:]) / 2
 
         return midpoints_x, hist
 
     def pdist_2d(self):
         """
@@ -191,20 +191,22 @@
         Y = self._get_md_data(self.Yname, self.Yindex, self.Yinterval)
     
         try:
             # numpy equivalent to: ax.hist2d(c2[:,1], aux)
             hist, x_edges, y_edges = np.histogram2d(X, Y, bins=self.bins, 
                                                     range=[self.histrange_x, self.histrange_y])
         except ValueError as e:
-            print(f"{e}: do the size of the x {X.shape} and y {Y.shape} inputs match? --Xinterval and --Yinterval can be adjusted.")
-            sys.exit(0)
+            message = f"{e}: do the size of the x {X.shape} and y {Y.shape} inputs match? "
+            message += f"--Xinterval and --Yinterval can be adjusted."
+            raise ValueError(message)
+        
         # let each row list bins with common y range
         hist = np.transpose(hist)
         # convert histogram counts to p_units
-        hist = self._normalize(hist)
+        hist = self._normalize(hist, self.p_units)
         # get bin midpoints
         midpoints_x = (x_edges[:-1] + x_edges[1:]) / 2
         midpoints_y = (y_edges[:-1] + y_edges[1:]) / 2
 
         return midpoints_x, midpoints_y, hist
         
     def pdist_3d(self):
@@ -221,33 +223,20 @@
 
         return X, Y, Z
 
     def pdist(self):
         """
         Main public method with pdist generation controls.
         """ 
-        # TODO: need to consolidate the Y 2d vs 1d stuff somehow
-
-        # TODO: if I can get rid of this or optimize it, I can then use the 
-            # original methods of each pdist by themselves
-        # TODO: only if histrange is None
-        # if self.histrange_x is None:
-        #     # get the optimal histrange
-        #     self.histrange_x = self._get_histrange(self.Xname, self.Xindex)
-        # # if using 2D pdist
-        # # TODO: needs to handle array input or None input
-        # if isinstance(self.Yname, (str, np.ndarray)) and self.histrange_y is None:
-        #     self.histrange_y = self._get_histrange(self.Yname, self.Yindex)
-
         # return timeseries data
         if self.data_type == "time":
             X, Y = self.timeseries()
             return X, Y, np.ones((X.shape[0]))
         # return pdist data
-        # TODO: t/e block to catch mismatched data lengths and print lengths
+        # TODO: t/e block to catch mismatched data lengths and print lengths?
         elif self.data_type == "pdist":
             # for 3D datasets, e.g. scatter
             if self.Yname and self.Zname:
                 return self.pdist_3d()
             # if 2D, return 2D dataset
             if self.Yname:
                 return self.pdist_2d()
```

### Comparing `wedap-0.0.8/mdap/md_plot.py` & `wedap-0.0.9/mdap/md_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/setup.py` & `wedap-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('./LICENSE') as f:
     lic = f.read()
 
 packages = find_packages()
 
 setup(
     name='wedap',
-    version='0.0.8',
+    version='0.0.9',
     description='weighted ensemble data analysis and plotting',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Darian T. Yang',
     author_email='dty7@pitt.edu',
     install_requires=['numpy', 'matplotlib', 'h5py', 'scipy', 'gif', 'tqdm'],
     url='https://github.com/darianyang/wedap',
```

### Comparing `wedap-0.0.8/wedap/__main__.py` & `wedap-0.0.9/wedap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/wedap/command_line.py` & `wedap-0.0.9/wedap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/wedap/h5_pdist.py` & `wedap-0.0.9/wedap/h5_pdist.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 # Suppress divide-by-zero in log
 np.seterr(divide='ignore', invalid='ignore')
 
 class H5_Pdist():
     """
     These class methods generate probability distributions from a WESTPA H5 file.
     """
-    # TODO: is setting aux_y to None the best approach to 1D plot settings?
     def __init__(self, h5="west.h5", data_type=None, Xname="pcoord", Xindex=0, Yname=None, 
                  Yindex=0, Zname=None, Zindex=0, H5save_out=None, Xsave_name=None, Ysave_name=None,
                  Zsave_name=None, data_proc=None, first_iter=1, last_iter=None, bins=(100,100), 
                  p_units='kT', T=298, weighted=True, skip_basis=None, skip_basis_out=None,
                  histrange_x=None, histrange_y=None, no_pbar=False, step_iter=1, *args, **kwargs):
         """
         Parameters
@@ -121,66 +120,24 @@
         self.h5_name = h5
         self.h5 = h5py.File(h5, mode="r")
 
         if data_type is None or data_type not in ["evolution", "average", "instant"]:
             raise ValueError("Must input valid data_type str: `evolution`, `average`, or `instant`")
         else:
             self.data_type = data_type
-        
-        # # save requested p_units
-        # self.requested_p_units = p_units        
-        # # have to change to raw for adding counts and will be normalized later
-        # self.p_units = "raw"
 
         self.p_units = str(p_units)
 
         self.T = int(T)
         self.weighted = weighted
 
-        # TODO: Default pcoord for either dim?
-        # TODO: clean up and condense this name processing section
-        # add auxdata prefix if not using pcoord and not using array input
-        # doing it in two conditional blocks since numpy as warning with comparing array to string
-        # this way it only does the string comparison if Xname is a string
-        if isinstance(Xname, str):
-            if Xname != "pcoord":
-                Xname = "auxdata/" + Xname
-        self.Xname = Xname
-        # TODO: set this up as an arg to be able to process 3D+ arrays form aux
-        # need to define the index if pcoord is 3D+ array, index is ndim - 1
-        self.Xindex = Xindex
-
-        # for 1D plots, but could be better (TODO)
-        if Yname is not None and isinstance(Yname, str):
-            # for common case of evolution with extra Yname input
-            if Yname and data_type == "evolution":
-                message = "\nDefaulting to evolution plot for --data-type, since you put a --Yname arg, " + \
-                          "\nDid you mean to use --data-type of `average` or `instant`?"
-                warn(message)
-            # add auxdata prefix if not using pcoord and not using array input
-            if Yname != "pcoord":
-                Yname = "auxdata/" + Yname
-            # before comparing X and Y, make sure they are both strings
-            if isinstance(Xname, str):
-                # for the common case where one plots pcoord/aux 0 and pcoord/aux 1
-                if Xname == Yname and Xindex == 0 and Yindex == 0:
-                    Yindex = 1
-                    message = "\nSetting --Yindex to 1 (2nd dimension) since Xname/Yname " + \
-                              "and Xindex/Yindex were the same."
-                    warn(message)
-        self.Yname = Yname
-        self.Yindex = Yindex
-
-        # for replacing the Z axis pdist with a dataset
-        if Zname is not None and isinstance(Zname, str):
-            # add auxdata prefix if not using pcoord and not using array input
-            if Zname != "pcoord":
-                Zname = "auxdata/" + Zname
-        self.Zname = Zname
-        self.Zindex = Zindex
+        # process XYZ names and indicies
+        self.Xname, self.Xindex = self._process_name_and_index(Xname, Xindex, Xname, Yname)
+        self.Yname, self.Yindex = self._process_name_and_index(Yname, Yindex, Xname, Yname)
+        self.Zname, self.Zindex = self._process_name_and_index(Zname, Zindex, Xname, Yname)
 
         # XYZ save into new h5 file options
         self.H5save_out = H5save_out
         self.Xsave_name = Xsave_name
         self.Ysave_name = Ysave_name
         self.Zsave_name = Zsave_name
         if H5save_out is not None:
@@ -206,31 +163,95 @@
         self.bins = bins
         self.skip_basis = skip_basis
         self.skip_basis_out = skip_basis_out
 
         # initialize weights
         self._init_weights()
 
-        # integer for the amount of frames saved (length) per tau (e.g. 101 for 100 ps tau)
-        self.tau = self._get_data_array("pcoord", 0, self.first_iter).shape[1]
-
         # n_particles for each iteration
-        self.n_particles = self.h5["summary"]["n_particles"]#[self.first_iter-1:self.last_iter]
+        self.n_particles = self.h5["summary"]["n_particles"]
 
         # TODO: I wonder if both of these attributes are needed (total only used by reshape data array)
         #       I should note somewhere that data array must be for the same length/iters as the west.h5 file
         # the sum of n segments in all specified iterations and all iterations overall
         self.current_particles = np.sum(self.h5["summary"]["n_particles"][self.first_iter-1:self.last_iter])
         # do not include the final (empty) iteration
         self.total_particles = np.sum(self.h5["summary"]["n_particles"][:-1])
 
+        # integer for the amount of frames saved (length) per tau (e.g. 101 for 100 ps tau)
+        self.tau = self._get_data_array("pcoord", 0, self.first_iter).shape[1]
+
         self.histrange_x = histrange_x
         self.histrange_y = histrange_y
         self.no_pbar = no_pbar
 
+        # accounts for array and filename input XYZnames
+        self._check_XYZnames()
+
+    def _process_name_and_index(self, name, index, Xname, Yname):
+        """
+        Consolidated logic for taking input XYZnames and outputting the 
+        corrected name and index.
+
+        Parameters
+        ----------
+        name : str
+            Input XYZ name.
+        index : int
+            Input XYZ index 
+        Xname : str
+        Yname : str
+        
+        Returns
+        -------
+        name : str
+            Corrected XYZ name.
+        index : int
+            Corrected XYZ index.
+        """
+        if name is not None and isinstance(name, str):
+            # add auxdata prefix if not using "pcoord" and not using array or filename input
+            if name != "pcoord" and name[-4:] != ".":
+                name = "auxdata/" + name
+            # for common case of evolution with extra Yname input
+            if self.data_type == "evolution":
+                warn("\nDefaulting to evolution plot for --data-type, since you put a --Yname arg.\n"
+                    "Did you mean to use --data-type of `average` or `instant`?")
+            # for common case where one plots "pcoord/aux 0" and "pcoord/aux 1"
+            elif isinstance(name, str) and name == Yname and Xname == Yname and index == 0:
+                index = 1
+                warn("\nSetting --Yindex to 1 (2nd dimension) since Xname/Yname and Xindex/Yindex were the same.")
+        return name, index
+
+    def _check_XYZnames(self):
+        """
+        Check XYZnames for array and filename input (if found, initialize).
+        Replaces self.Xname, self.Yname, and self.Zname attrs as needed.
+        """
+        XYZnames = ["Xname", "Yname", "Zname"]
+        for name in XYZnames:
+            attr_value = getattr(self, name)
+            # reshape 1d input raw data array (if given) into 3d array
+            if isinstance(attr_value, np.ndarray):
+                setattr(self, name, self.reshape_total_data_array(attr_value))
+            # if input isn't an auxname but an allowed filename for input
+            elif isinstance(attr_value, str) and attr_value[-4] == ".":
+                # for .npy binary files or pkl files
+                if attr_value[-4:] in [".npy", ".npz", ".pkl"]:
+                    data = np.load(attr_value, allow_pickle=True)
+                # text files
+                elif attr_value[-4:] in [".dat", ".txt"]:
+                    data = np.genfromtxt(attr_value)
+                else:
+                    raise ValueError("File ending must be '.dat', '.txt', '.npy', '.npz', or '.pkl'")
+                # need to reshape so that the columns go depth wise
+                data = data.reshape(data.shape[0], 1, -1)
+                # reshape the array again to fit into current westpa seg per iter shape and set
+                setattr(self, name, self.reshape_total_data_array(data))
+
     def _init_weights(self):
         """
         Initialize the weight array.
         """
         #for iter in range(self.first_iter, self.last_iter + 1):
         # have to make array start from iteration 1 to index well during weighting
         # but only for using skipping basis
@@ -268,25 +289,23 @@
             Name of the dataset that is being placed into the h5 file.
 
         Returns
         -------
         data : ndarray
             Dataset of interest from the H5 file.
         """
-        # if the user puts in an array object instead of a string dataset name
+        # if the user puts in an array object or filename instead of a string dataset name
+        # for filename case, should have been converted to an array upon init
         if isinstance(name, np.ndarray):
-            # first reshape 1d input raw data array into 3d array
-            # currently, this is done during pdist method
-            #data = self.reshape_total_data_array(name)
-
             # need to parse data for segments only in current iteration
             # segments are each row, but in input they are all concatenated
             n_segs_up_to_iter = np.sum(self.n_particles[self.first_iter-1:iteration-1])
             n_segs_including_iter = np.sum(self.n_particles[self.first_iter-1:iteration])
             data = name[n_segs_up_to_iter:n_segs_including_iter,:,:]
+
         # name should be a string for the h5 file dataset name
         elif isinstance(name, str):
             # this t/e block is to catch non-existent aux data names
             try:
                 data = np.array(self.h5[f"iterations/iter_{iteration:08d}/{name}"])
             except KeyError:
                 message = f"{name} is not a valid object in the h5 file. \n" + \
@@ -1066,25 +1085,26 @@
 
         try:
             array = array.reshape(self.total_particles, self.tau, -1)
         # e.g. ValueError: cannot reshape array of size 303000 into shape (3000,100,newaxis)
         except ValueError as e:
             array = array.reshape(self.total_particles, self.tau - 1, -1)
             message = "\nYou may be using an input data array which did not include the rst file datapoints. " + \
-                      "\nThis may be fine, but note that you shouldn't create a new H5 file using this array."
-            warn(e + message)
-            # TODO: does this work?
+                      "\nThis will work, but note that you shouldn't create a new H5 file using this array."
+            warn(f"{e} {message}")
             # the case where the array does not have rst data included
             # put the new first column as the first value of each row (segment)
             # TODO: this is a temp hack for the no rst shape data
             # noting that both arrays must have same ndims for hstack
-            #print(f"original shape: {data.shape}")
-            #print(f"to stack shape: {data[:,0,:]}")
-            array = np.hstack((np.atleast_3d(array[:,0,:]), array)) # TODO: test this
-            #print(f"new shape: {data.shape}")
+            #print(f"original shape: {array.shape}")
+            #print(f"to stack shape: {np.atleast_3d(array[:,0,:]).shape}")
+            # make array for all first col vals reshape so that the columns go depth wise
+            firstcols = array[:,0,:].reshape(array.shape[0], 1, -1)
+            array = np.hstack((firstcols, array))
+            #print(f"new shape: {array.shape}")
 
         # TODO: the above works to solve the shape issue but if I wanted to fill out a new dataset in
         # the h5 file, it would be missing the first value, which links walkers.
         # maybe I can use the parent IDs to link it manually, but note I would have to
         # go through and parse by my self.n_particles array to separate iterations.
         # put conditional if shape[1] = tau vs tau - 1 for creating dataset (to add parent data point)
         # note that the first iteration I need to pull from somewhere else? It's calculated from the
@@ -1115,36 +1135,28 @@
                 self.weights = self._new_weights_from_skip_basis()
             # if the wrong amount of args are input and != n_bstates
             except IndexError as e:
                 message = f"IndexError ({e}) for bstate input ({self.skip_basis}): " + \
                           f"Did you use the correct amount of bstates {self.n_bstates}?"
                 warn(message)
 
-        # reshape 1d input raw data array (if given) into 3d array
-        if isinstance(self.Xname, np.ndarray):
-            self.Xname = self.reshape_total_data_array(self.Xname)
-        if isinstance(self.Yname, np.ndarray):
-            self.Yname = self.reshape_total_data_array(self.Yname)
-        if isinstance(self.Zname, np.ndarray):
-            self.Zname = self.reshape_total_data_array(self.Zname)
-
         # TODO: could make this it's own method
         # if requested, save out a new H5 file with the input data array in new aux name
         if self.H5save_out is not None:
             for iter in range(self.first_iter, self.last_iter + 1):
                 if self.Xsave_name:
                     self._get_data_array(self.Xname, self.Xindex, iter, self.H5save_out, self.Xsave_name)
                 if self.Ysave_name:
                     self._get_data_array(self.Yname, self.Yindex, iter, self.H5save_out, self.Ysave_name)
                 if self.Zsave_name:
                     self._get_data_array(self.Zname, self.Zindex, iter, self.H5save_out, self.Zsave_name)
 
         # TODO: need to consolidate the Y 2d vs 1d stuff somehow
 
-        # TODO: testing multi_h5: putting the whole thing in a loop over each h5 file
+        # multi_h5: putting the whole thing in a loop over each h5 file
         # loop histranges to find the best hist range for all input h5 files
         # loop each pdist return, sum and normalize at the end
 
         # collect each histrange for each file 
         xranges = []
         yranges = []
         # go through each file and find a consistent histrange if histrangeXY is None
```

### Comparing `wedap-0.0.8/wedap/h5_plot.py` & `wedap-0.0.9/wedap/h5_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,18 @@
         # or getting them from w_pdist h5 file, or from H5_Pdist output file
         # user inputs XYZ
         if X is None and Y is None and Z is None:
             super().__init__(*args, **kwargs)
             # save the user requested p_units and changes p_units to raw
             if self.jointplot:
                 # will be re-normed later on
-                X, Y, Z = H5_Pdist(*args, **kwargs).pdist(normalize=False)
+                X, Y, Z = self.pdist(normalize=False)
             else:
                 # TODO: tuple unpacking to deal with variable item return
-                X, Y, Z = H5_Pdist(*args, **kwargs).pdist()
+                X, Y, Z = self.pdist()
         # need to set this when using mdap, shouldn't affect anything else
         # since joint plot dists must be changed from raw to requested p_units
         if self.jointplot and "p_units" in kwargs:
             self.requested_p_units = kwargs["p_units"]
         else:
             self.requested_p_units = "kT"
```

### Comparing `wedap-0.0.8/wedap/tests/make_h5_plot_test_data.py` & `wedap-0.0.9/wedap/tests/make_h5_plot_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/wedap/tests/test_h5_pdist.py` & `wedap-0.0.9/wedap/tests/test_h5_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/wedap/tests/test_h5_plot.py` & `wedap-0.0.9/wedap/tests/test_h5_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.8/wedap.egg-info/PKG-INFO` & `wedap-0.0.9/wedap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 0.0.8
+Version: 0.0.9
 Summary: weighted ensemble data analysis and plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
```

### Comparing `wedap-0.0.8/wedap.egg-info/SOURCES.txt` & `wedap-0.0.9/wedap.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 setup.py
 mdap/__init__.py
 mdap/__main__.py
 mdap/command_line.py
 mdap/md_pdist.py
 mdap/md_plot.py
 mdap/styles/__init__.py
+mdap/tests/__init__.py
+mdap/tests/make_md_pdist_test_data.py
+mdap/tests/test_md_pdist.py
 styles/__init__.py
 wedap/__init__.py
 wedap/__main__.py
 wedap/command_line.py
 wedap/h5_pdist.py
 wedap/h5_plot.py
 wedap.egg-info/PKG-INFO
```

