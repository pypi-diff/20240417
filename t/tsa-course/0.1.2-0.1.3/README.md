# Comparing `tmp/tsa_course-0.1.2.tar.gz` & `tmp/tsa_course-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsa_course-0.1.2.tar", last modified: Tue Apr 16 23:12:56 2024, max compression
+gzip compressed data, was "tsa_course-0.1.3.tar", last modified: Tue Apr 16 23:37:22 2024, max compression
```

## Comparing `tsa_course-0.1.2.tar` & `tsa_course-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.1.2/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:12:56.729710 tsa_course-0.1.2/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     7460 2024-04-16 17:34:58.000000 tsa_course-0.1.2/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-16 23:12:56.729710 tsa_course-0.1.2/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-16 23:11:51.000000 tsa_course-0.1.2/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/tsa_course/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.1.2/tsa_course/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)    13578 2024-04-16 23:11:32.000000 tsa_course-0.1.2/tsa_course/lecture11.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:12:56.729710 tsa_course-0.1.2/tsa_course.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      242 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-16 23:12:56.000000 tsa_course-0.1.2/tsa_course.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:37:22.189711 tsa_course-0.1.3/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.1.3/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:37:22.189711 tsa_course-0.1.3/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     7460 2024-04-16 17:34:58.000000 tsa_course-0.1.3/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-16 23:37:22.189711 tsa_course-0.1.3/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-16 23:37:17.000000 tsa_course-0.1.3/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:37:22.189711 tsa_course-0.1.3/tsa_course/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.1.3/tsa_course/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)    13645 2024-04-16 23:36:51.000000 tsa_course-0.1.3/tsa_course/lecture11.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-16 23:37:22.189711 tsa_course-0.1.3/tsa_course.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8180 2024-04-16 23:37:22.000000 tsa_course-0.1.3/tsa_course.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      242 2024-04-16 23:37:22.000000 tsa_course-0.1.3/tsa_course.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-16 23:37:22.000000 tsa_course-0.1.3/tsa_course.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-16 23:37:22.000000 tsa_course-0.1.3/tsa_course.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-16 23:37:22.000000 tsa_course-0.1.3/tsa_course.egg-info/top_level.txt
```

### Comparing `tsa_course-0.1.2/LICENSE` & `tsa_course-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsa_course-0.1.2/PKG-INFO` & `tsa_course-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.1.2 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.1.3 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `tsa_course-0.1.2/README.md` & `tsa_course-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tsa_course-0.1.2/setup.py` & `tsa_course-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tsa_course",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     python_requires='>=3.10',
     install_requires=[
         'numpy>1.19.5',
         'matplotlib',
         'scipy',
         'tqdm'
```

### Comparing `tsa_course-0.1.2/tsa_course/lecture11.py` & `tsa_course-0.1.3/tsa_course/lecture11.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,25 +317,25 @@
         le_list.append(LEs.max())
 
         x0 = solution.y[:,-1]
 
     mle = np.array(le_list)
     pos_idx = np.where(mle > 0)[0]
     neg_idx = np.where(mle < 0)[0]
-    _, axes = plt.subplots(4, 1, figsize=(20, 20))
+    _, axes = plt.subplots(4, 1, figsize=(15, 15))
     axes[0].plot(px_max, maxima_x, 'ko', markersize=0.5, alpha=0.3, label="Local maxima")
-    axes[0].plot(px_min, minima_x, 'ro', markersize=0.5, alpha=0.3, label="Local minima")
+    axes[0].plot(px_min, minima_x, 'o', color='tab:blue', markersize=0.2, alpha=0.3, label="Local minima")
     axes[0].legend(loc='upper left', markerscale=10)
     axes[0].set_ylabel("x-values")
     axes[1].plot(py_max, maxima_y, 'ko', markersize=0.5, alpha=0.3, label="Local maxima")
-    axes[1].plot(py_min, minima_y, 'ro', markersize=0.5, alpha=0.3, label="Local minima")
+    axes[1].plot(py_min, minima_y, 'o', color='tab:blue', markersize=0.2, alpha=0.3, label="Local minima")
     axes[1].legend(loc='upper left', markerscale=10)
     axes[1].set_ylabel("y-values")
     axes[2].plot(pz_max, maxima_z, 'ko', markersize=0.5, alpha=0.3, label="Local maxima")
-    axes[2].plot(pz_min, minima_z, 'ro', markersize=0.5, alpha=0.3, label="Local minima")
+    axes[2].plot(pz_min, minima_z, 'o', color='tab:blue', markersize=0.2, alpha=0.3, label="Local minima")
     axes[2].legend(loc='upper left', markerscale=10)
     axes[2].set_ylabel("z-values")
-    axes[3].plot(parameters[:,p_idx][pos_idx], mle[pos_idx], 'ro', markersize=2.5, alpha=0.5)
+    axes[3].plot(parameters[:,p_idx][pos_idx], mle[pos_idx], 'o', color='tab:red', markersize=2.5, alpha=0.5)
     axes[3].plot(parameters[:,p_idx][neg_idx], mle[neg_idx], 'ko', markersize=2.5, alpha=0.5)
     axes[3].set_ylabel("Maximum Lyapunov Exponents")
     axes[3].set_xlabel("Parameter Value")
     axes[3].axhline(0, color='k', lw=.5, alpha=.5)
```

### Comparing `tsa_course-0.1.2/tsa_course.egg-info/PKG-INFO` & `tsa_course-0.1.3/tsa_course.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.1.2 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.1.3 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

