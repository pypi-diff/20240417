# Comparing `tmp/tsa_course-0.0.1.tar.gz` & `tmp/tsa_course-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsa_course-0.0.1.tar", last modified: Tue Apr 16 17:30:04 2024, max compression
+gzip compressed data, was "tsa_course-0.1.2.tar", last modified: Tue Apr 16 23:12:56 2024, max compression
```

## Comparing `tsa_course-0.0.1.tar` & `tsa_course-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 17:30:04.801706 tsa_course-0.0.1/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.0.1/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     7795 2024-04-16 17:30:04.801706 tsa_course-0.0.1/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     7075 2024-04-13 17:01:30.000000 tsa_course-0.0.1/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-16 17:30:04.801706 tsa_course-0.0.1/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-16 17:29:48.000000 tsa_course-0.0.1/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 17:30:04.801706 tsa_course-0.0.1/tsa_course/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.0.1/tsa_course/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)    13839 2024-04-16 17:12:52.000000 tsa_course-0.0.1/tsa_course/lecture11.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 17:30:04.801706 tsa_course-0.0.1/tsa_course.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     7795 2024-04-16 17:30:04.000000 tsa_course-0.0.1/tsa_course.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      242 2024-04-16 17:30:04.000000 tsa_course-0.0.1/tsa_course.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-16 17:30:04.000000 tsa_course-0.0.1/tsa_course.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-16 17:30:04.000000 tsa_course-0.0.1/tsa_course.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-16 17:30:04.000000 tsa_course-0.0.1/tsa_course.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.1.2/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:12:56.729710 tsa_course-0.1.2/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     7460 2024-04-16 17:34:58.000000 tsa_course-0.1.2/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-16 23:12:56.729710 tsa_course-0.1.2/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-16 23:11:51.000000 tsa_course-0.1.2/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/tsa_course/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.1.2/tsa_course/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)    13578 2024-04-16 23:11:32.000000 tsa_course-0.1.2/tsa_course/lecture11.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/tsa_course.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      242 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/top_level.txt
```

### Comparing `tsa_course-0.0.1/LICENSE` & `tsa_course-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsa_course-0.0.1/PKG-INFO` & `tsa_course-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-Metadata-Version: 2.1
-Name: tsa_course
-Version: 0.0.1
-Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
-Author: Filippo Maria Bianchi
-Author-email: filippombianchi@gmail.com
-Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
-Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>1.19.5
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: tqdm
-
 # Time Series Analysis with Python
 
 <div align="center">
-   <img src="logo.png" style="width: 5cm; display: block; margin: auto;">
+   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 </div>
 
 <br>
 <div align="center">
 📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
 </div>
 <br>
@@ -175,18 +156,18 @@
    ```
 
 ## 🎥 Notebook format and slides
 
 The notebooks are structured as a sequence of slides to be presented using [RISE](https://rise.readthedocs.io/en/latest/).
 If you open a notebook you will see the following structure:
 
-<img src="notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
 
 The top-right button indicates the type of slide, which is stored in the metadata of the cell. To enable the visualization of the slide type you must first install RISE and then on the top menu select `View -> Cell Toolbar -> Slieshow`. Also, to split the cells like in the example, you must enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html).
 
 By pressing the `Enter\Exit RISE Slideshow` button at the top you can enter the slideshow presentation.
 
-<img src="notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
 
 See the [RISE documentation](https://rise.readthedocs.io/en/latest/) for more info.
```

#### html2text {}

```diff
@@ -1,18 +1,10 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.0.1 Summary: A collection of
-scripts and functions used in the course 'Time Series Analysis with Python'
-Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
-Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
-handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy>1.19.5 Requires-Dist: matplotlib Requires-Dist:
-scipy Requires-Dist: tqdm # Time Series Analysis with Python
-                                  [logo.png]
+# Time Series Analysis with Python
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+                                   logo.png]
 
                               ð _R_e_a_d_ _t_h_e_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
@@ -81,18 +73,22 @@
 and navigate to the location with the yml file you just downloaded. - If you
 are on Windows, open the Miniconda shell. 4. Install the environment with ```
 {bash} > conda env create -f env.yml ``` 5. Activate your environment: ```
 {bash} > conda activate pytsa ``` 6. Go to the folder with the notebooks 7.
 Launch Jupyter Lab with the command ```{bash} > jupyter lab ``` ## ð¥
 Notebook format and slides The notebooks are structured as a sequence of slides
 to be presented using [RISE](https://rise.readthedocs.io/en/latest/). If you
-open a notebook you will see the following structure: [notebooks/00/media/
-slides_nb.png]The top-right button indicates the type of slide, which is stored
-in the metadata of the cell. To enable the visualization of the slide type you
-must first install RISE and then on the top menu select `View -> Cell Toolbar -
-> Slieshow`. Also, to split the cells like in the example, you must enable
-`Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
+open a notebook you will see the following structure: [https://
+raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/
+00/media/slides_nb.png]The top-right button indicates the type of slide, which
+is stored in the metadata of the cell. To enable the visualization of the slide
+type you must first install RISE and then on the top menu select `View -> Cell
+Toolbar -> Slieshow`. Also, to split the cells like in the example, you must
+enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
 nbextensions.readthedocs.io/en/latest/index.html). By pressing the `Enter\Exit
 RISE Slideshow` button at the top you can enter the slideshow presentation.
-[notebooks/00/media/slides_rise.png][notebooks/00/media/slides_rise2.png]
-[notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise.png][https://raw.githubusercontent.com/
+FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png]
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
 rise.readthedocs.io/en/latest/) for more info.
```

### Comparing `tsa_course-0.0.1/README.md` & `tsa_course-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,30 @@
+Metadata-Version: 2.1
+Name: tsa_course
+Version: 0.1.2
+Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
+Author: Filippo Maria Bianchi
+Author-email: filippombianchi@gmail.com
+Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
+Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>1.19.5
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: tqdm
+
 # Time Series Analysis with Python
 
 <div align="center">
-   <img src="logo.png" style="width: 5cm; display: block; margin: auto;">
+   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 </div>
 
 <br>
 <div align="center">
 📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
 </div>
 <br>
@@ -156,18 +175,18 @@
    ```
 
 ## 🎥 Notebook format and slides
 
 The notebooks are structured as a sequence of slides to be presented using [RISE](https://rise.readthedocs.io/en/latest/).
 If you open a notebook you will see the following structure:
 
-<img src="notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
 
 The top-right button indicates the type of slide, which is stored in the metadata of the cell. To enable the visualization of the slide type you must first install RISE and then on the top menu select `View -> Cell Toolbar -> Slieshow`. Also, to split the cells like in the example, you must enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html).
 
 By pressing the `Enter\Exit RISE Slideshow` button at the top you can enter the slideshow presentation.
 
-<img src="notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
 
 See the [RISE documentation](https://rise.readthedocs.io/en/latest/) for more info.
```

#### html2text {}

```diff
@@ -1,9 +1,19 @@
-# Time Series Analysis with Python
-                                  [logo.png]
+Metadata-Version: 2.1 Name: tsa_course Version: 0.1.2 Summary: A collection of
+scripts and functions used in the course 'Time Series Analysis with Python'
+Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
+URL: Documentation, https://filippomb.github.io/python-time-series-handbook
+Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
+handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: numpy>1.19.5 Requires-Dist: matplotlib Requires-Dist:
+scipy Requires-Dist: tqdm # Time Series Analysis with Python
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+                                   logo.png]
 
                               ð _R_e_a_d_ _t_h_e_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
@@ -72,18 +82,22 @@
 and navigate to the location with the yml file you just downloaded. - If you
 are on Windows, open the Miniconda shell. 4. Install the environment with ```
 {bash} > conda env create -f env.yml ``` 5. Activate your environment: ```
 {bash} > conda activate pytsa ``` 6. Go to the folder with the notebooks 7.
 Launch Jupyter Lab with the command ```{bash} > jupyter lab ``` ## ð¥
 Notebook format and slides The notebooks are structured as a sequence of slides
 to be presented using [RISE](https://rise.readthedocs.io/en/latest/). If you
-open a notebook you will see the following structure: [notebooks/00/media/
-slides_nb.png]The top-right button indicates the type of slide, which is stored
-in the metadata of the cell. To enable the visualization of the slide type you
-must first install RISE and then on the top menu select `View -> Cell Toolbar -
-> Slieshow`. Also, to split the cells like in the example, you must enable
-`Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
+open a notebook you will see the following structure: [https://
+raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/
+00/media/slides_nb.png]The top-right button indicates the type of slide, which
+is stored in the metadata of the cell. To enable the visualization of the slide
+type you must first install RISE and then on the top menu select `View -> Cell
+Toolbar -> Slieshow`. Also, to split the cells like in the example, you must
+enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
 nbextensions.readthedocs.io/en/latest/index.html). By pressing the `Enter\Exit
 RISE Slideshow` button at the top you can enter the slideshow presentation.
-[notebooks/00/media/slides_rise.png][notebooks/00/media/slides_rise2.png]
-[notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise.png][https://raw.githubusercontent.com/
+FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png]
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
 rise.readthedocs.io/en/latest/) for more info.
```

### Comparing `tsa_course-0.0.1/setup.py` & `tsa_course-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tsa_course",
-    version="0.0.1",
+    version="0.1.2",
     packages=find_packages(),
     python_requires='>=3.10',
     install_requires=[
         'numpy>1.19.5',
         'matplotlib',
         'scipy',
         'tqdm'
```

### Comparing `tsa_course-0.0.1/tsa_course/lecture11.py` & `tsa_course-0.1.2/tsa_course/lecture11.py`

 * *Files 12% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     The variational equation calculates the time derivative of the variational matrix using the Jacobian of the ODE function.
     
     The variational matrix represents the sensitivity of the system state to initial conditions.
     
     The output is a flattened array representing the time derivative of the variational matrix, which can be used for numerical integration.
     
     Example usage:
-    
+    --------------
     >>> t = np.linspace(0, 10, 100)
     >>> Phi = np.eye(num_dimensions, dtype=np.float64).flatten()
     >>> x = np.array([1.0, 2.0, 3.0])
     >>> dPhi_dt = _variational_equation(t, Phi, x, fjac, p)
     """
     num_dimensions = len(x)
     Phi_matrix = np.reshape(Phi, (num_dimensions, num_dimensions))
@@ -233,42 +233,50 @@
     # compute LEs
     LE_history = np.cumsum(np.log(LE + 1e-10), axis=0) / np.tile(t[1:], (num_dimensions, 1)).T
 
     LEs = LE_history[-1, :]
     return LEs, LE_history
 
 
-def plot_bifurcation_diagram(func, func_jac, s0, time_vector, parameters, p_idx, max_time=None):
+def plot_bifurcation_diagram(func, func_jac, x0, time_vector, parameters, p_idx, max_time=None):
     """
-    This function computes and plots the bifurcation diagram for a set of ordinary differential equations (ODEs). 
-    It takes as input the ODE function, its Jacobian, initial conditions, time vector, range of parameter values, 
-    and the index of the parameter to vary in the bifurcation diagram. The ODE function should be defined as a 
-    callable that takes arguments for the current state and time, and returns the derivative of the state with 
-    respect to time. The Jacobian function should be defined as a callable that takes arguments for the current 
-    state and time, and returns the Jacobian matrix of the ODE function. The initial conditions should be specified 
-    as an array-like object. The time vector should be an array-like object representing the time points at which 
-    to evaluate the ODEs. The range of parameter values should be specified as an array-like object. The index of 
-    the parameter to vary in the bifurcation diagram should be an integer. The function will compute the solution 
-    of the ODEs for each parameter value in the range, and plot the bifurcation diagram showing the local maxima 
-    and minima of the state variables, as well as the maximum Lyapunov exponents as a function of the parameter value.
-    
-    :param func: ODE function. Must take arguments like func(t, x, p) where x and t are 
-                 the state and time *now*, and p is a tuple of parameters. If there are 
-                 no model parameters, p should be set to the empty tuple.
-    :type func: callable
-    :param func_jac: Jacobian of func.
-    :type func_jac: callable
-    :param s0: Initial conditions.
-    :type s0: array_like
-    :param time_vector: Time vector for the integration.
-    :type time_vector: array_like
-    :param parameters: Range of parameter values to explore.
-    :type parameters: array_like
-    :param p_idx: Index of the parameter to vary in the bifurcation diagram.
-    :type p_idx: int
+    Computes and plots the bifurcation diagram for a set of ordinary differential equations (ODEs).
+
+    Parameters:
+    ----------
+    func : function
+        ODE function. Must take arguments like func(t, x, p) where x and t are 
+        the state and time *now*, and p is a tuple of parameters. If there are 
+        no model parameters, p should be set to the empty tuple.
+    func_jac : function
+        Jacobian of func.
+    x0 : array_like
+        Initial conditions.
+    time_vector : array_like
+        Time vector for the integration.
+    parameters : array_like
+        Range of parameter values to explore.
+    p_idx : int
+        Index of the parameter to vary in the bifurcation diagram.
+
+    Notes:
+    ------
+    The ODE function should be defined as a callable that takes arguments for the current state and time, and returns the derivative of the state with respect to time.
+
+    The Jacobian function should be defined as a callable that takes arguments for the current state and time, and returns the Jacobian matrix of the ODE function.
+
+    The initial conditions should be specified as an array-like object.
+
+    The time vector should be an array-like object representing the time points at which to evaluate the ODEs.
+
+    The range of parameter values should be specified as an array-like object.
+
+    The index of the parameter to vary in the bifurcation diagram should be an integer.
+
+    The function will compute the solution of the ODEs for each parameter value in the range, and plot the bifurcation diagram showing the local maxima and minima of the state variables, as well as the maximum Lyapunov exponents as a function of the parameter value.
     """
     maxima_x = []
     minima_x = []
     px_max = []
     px_min = []
     maxima_y = []
     minima_y = []
@@ -278,15 +286,15 @@
     minima_z = []
     pz_max = []
     pz_min = []
     le_list = []
 
     for _p in tqdm(parameters):
 
-        solution = solve_ivp(func, [time_vector[0], time_vector[-1]], s0, args=_p, t_eval=time_vector)
+        solution = solve_ivp(func, [time_vector[0], time_vector[-1]], x0, args=_p, t_eval=time_vector)
 
         local_max_x, _ = find_peaks(solution.y[0])
         local_min_x, _ = find_peaks(-1*solution.y[0])
         local_max_y, _ = find_peaks(solution.y[1])
         local_min_y, _ = find_peaks(-1*solution.y[1])
         local_max_z, _ = find_peaks(solution.y[2])
         local_min_z, _ = find_peaks(-1*solution.y[2])
@@ -301,18 +309,18 @@
         py_min.extend([_p[p_idx]] * len(local_min_y))
         maxima_z.extend(solution.y[2, local_max_z])
         minima_z.extend(solution.y[2, local_min_z])
         pz_max.extend([_p[p_idx]] * len(local_max_z))
         pz_min.extend([_p[p_idx]] * len(local_min_z))
 
         LE_time = time_vector if max_time is None else time_vector[:max_time]
-        LEs, _ = computeLE(func, func_jac, s0, LE_time, p=_p)
+        LEs, _ = computeLE(func, func_jac, x0, LE_time, p=_p)
         le_list.append(LEs.max())
 
-        s0 = solution.y[:,-1]
+        x0 = solution.y[:,-1]
 
     mle = np.array(le_list)
     pos_idx = np.where(mle > 0)[0]
     neg_idx = np.where(mle < 0)[0]
     _, axes = plt.subplots(4, 1, figsize=(20, 20))
     axes[0].plot(px_max, maxima_x, 'ko', markersize=0.5, alpha=0.3, label="Local maxima")
     axes[0].plot(px_min, minima_x, 'ro', markersize=0.5, alpha=0.3, label="Local minima")
```

### Comparing `tsa_course-0.0.1/tsa_course.egg-info/PKG-INFO` & `tsa_course-0.1.2/tsa_course.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.0.1
+Version: 0.1.2
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # Time Series Analysis with Python
 
 <div align="center">
-   <img src="logo.png" style="width: 5cm; display: block; margin: auto;">
+   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 </div>
 
 <br>
 <div align="center">
 📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
 </div>
 <br>
@@ -175,18 +175,18 @@
    ```
 
 ## 🎥 Notebook format and slides
 
 The notebooks are structured as a sequence of slides to be presented using [RISE](https://rise.readthedocs.io/en/latest/).
 If you open a notebook you will see the following structure:
 
-<img src="notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_nb.png" style="width: 50%" align="center">
 
 The top-right button indicates the type of slide, which is stored in the metadata of the cell. To enable the visualization of the slide type you must first install RISE and then on the top menu select `View -> Cell Toolbar -> Slieshow`. Also, to split the cells like in the example, you must enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html).
 
 By pressing the `Enter\Exit RISE Slideshow` button at the top you can enter the slideshow presentation.
 
-<img src="notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
-<img src="notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png" style="width: 40%" align="center">
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise3.png" style="width: 40%" align="center">
 
 See the [RISE documentation](https://rise.readthedocs.io/en/latest/) for more info.
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.0.1 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.1.2 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: numpy>1.19.5 Requires-Dist: matplotlib Requires-Dist:
 scipy Requires-Dist: tqdm # Time Series Analysis with Python
-                                  [logo.png]
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+                                   logo.png]
 
                               ð _R_e_a_d_ _t_h_e_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
@@ -81,18 +82,22 @@
 and navigate to the location with the yml file you just downloaded. - If you
 are on Windows, open the Miniconda shell. 4. Install the environment with ```
 {bash} > conda env create -f env.yml ``` 5. Activate your environment: ```
 {bash} > conda activate pytsa ``` 6. Go to the folder with the notebooks 7.
 Launch Jupyter Lab with the command ```{bash} > jupyter lab ``` ## ð¥
 Notebook format and slides The notebooks are structured as a sequence of slides
 to be presented using [RISE](https://rise.readthedocs.io/en/latest/). If you
-open a notebook you will see the following structure: [notebooks/00/media/
-slides_nb.png]The top-right button indicates the type of slide, which is stored
-in the metadata of the cell. To enable the visualization of the slide type you
-must first install RISE and then on the top menu select `View -> Cell Toolbar -
-> Slieshow`. Also, to split the cells like in the example, you must enable
-`Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
+open a notebook you will see the following structure: [https://
+raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/notebooks/
+00/media/slides_nb.png]The top-right button indicates the type of slide, which
+is stored in the metadata of the cell. To enable the visualization of the slide
+type you must first install RISE and then on the top menu select `View -> Cell
+Toolbar -> Slieshow`. Also, to split the cells like in the example, you must
+enable `Split Cells Notebook` from the [nbextensions](https://jupyter-contrib-
 nbextensions.readthedocs.io/en/latest/index.html). By pressing the `Enter\Exit
 RISE Slideshow` button at the top you can enter the slideshow presentation.
-[notebooks/00/media/slides_rise.png][notebooks/00/media/slides_rise2.png]
-[notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise.png][https://raw.githubusercontent.com/
+FilippoMB/python-time-series-handbook/main/notebooks/00/media/slides_rise2.png]
+[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
+notebooks/00/media/slides_rise3.png]See the [RISE documentation](https://
 rise.readthedocs.io/en/latest/) for more info.
```

