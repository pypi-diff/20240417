# Comparing `tmp/tmgtoolkit-0.1.1.tar.gz` & `tmp/tmgtoolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmgtoolkit-0.1.1.tar", last modified: Thu Apr 11 07:35:37 2024, max compression
+gzip compressed data, was "tmgtoolkit-0.1.2.tar", last modified: Wed Apr 17 09:41:06 2024, max compression
```

## Comparing `tmgtoolkit-0.1.1.tar` & `tmgtoolkit-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-11 07:35:37.279838 tmgtoolkit-0.1.1/
--rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.1/LICENSE.md
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-11 07:35:37.279838 tmgtoolkit-0.1.1/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.1/README.md
--rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.1/pyproject.toml
--rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-04-11 07:35:37.279838 tmgtoolkit-0.1.1/setup.cfg
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-11 07:35:37.273171 tmgtoolkit-0.1.1/src/
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-11 07:35:37.276505 tmgtoolkit-0.1.1/src/tmgtoolkit/
--rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/__init__.py
--rw-r--r--   0 ej        (1000) wheel      (998)     3053 2024-04-10 19:50:56.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/constants.py
--rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-04-10 20:05:19.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/plotting.py
--rw-r--r--   0 ej        (1000) wheel      (998)    12885 2024-04-10 11:39:53.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/spm.py
--rw-r--r--   0 ej        (1000) wheel      (998)    18623 2024-04-10 11:39:56.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/time_series.py
--rw-r--r--   0 ej        (1000) wheel      (998)     3208 2024-04-10 11:40:01.000000 tmgtoolkit-0.1.1/src/tmgtoolkit/tmgio.py
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-11 07:35:37.279838 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-11 07:35:37.000000 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      392 2024-04-11 07:35:37.000000 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-04-11 07:35:37.000000 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-04-11 07:35:37.000000 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/requires.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-04-11 07:35:37.000000 tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/
+-rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.2/LICENSE.md
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.2/README.md
+-rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.2/pyproject.toml
+-rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/setup.cfg
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.603046 tmgtoolkit-0.1.2/src/
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.603046 tmgtoolkit-0.1.2/src/tmgtoolkit/
+-rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/__init__.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     3298 2024-04-17 08:36:30.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/constants.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-04-10 20:05:19.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/plotting.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    14809 2024-04-17 08:36:20.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/spm.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    18630 2024-04-12 13:27:22.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/time_series.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     3283 2024-04-13 07:30:15.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/tmgio.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      410 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/requires.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/tests/
+-rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-04-17 09:39:29.000000 tmgtoolkit-0.1.2/tests/test_mwe.py
```

### Comparing `tmgtoolkit-0.1.1/LICENSE.md` & `tmgtoolkit-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.1/PKG-INFO` & `tmgtoolkit-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tmgtoolkit-0.1.1/README.md` & `tmgtoolkit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.1/setup.cfg` & `tmgtoolkit-0.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tmgtoolkit
-version = 0.1.1
+version = 0.1.2
 author = Elijan Mastnak
 author_email = admin@ejmastnak.com
 description = Time series analysis of tensiomyography (TMG) data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejmastnak/tmgtoolkit
 project_urls =
```

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit/constants.py` & `tmgtoolkit-0.1.2/src/tmgtoolkit/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -75,14 +75,43 @@
       'z_line2': 3,
       'z_fill1': 1,
       'z_fill2': 2,
       'x_axis_color': '#000000',
       'x_axis_linestyle': ':',
       'legend_alpha': 1.0,
     }
-    
+
 class NamedTupleTypes:
-    TmgParams = namedtuple('TmgParams', ['dm', 'td', 'tc', 'ts', 'tr'])
-    ExtremumParams = namedtuple('ExtremumParams', ['max_time', 'max', 'min_time', 'min'])
-    SpmTStatistic = namedtuple('SpmTStatistic', ['t_statistic', 'spm_t'])
-    SpmTInference = namedtuple('SpmTInference', ['alpha', 'p', 'threshold', 'clusters'])
-    SpmCluster = namedtuple('SpmCluster', ['p', 'start_time', 'end_time', 'centroid_time', 'centroid', 'extremum_time', 'extremum', 'area'])
+    TmgParams = namedtuple('TmgParams', [
+        'dm',
+        'td',
+        'tc',
+        'ts',
+        'tr'
+        ])
+    ExtremumParams = namedtuple('ExtremumParams', [
+        'max_time',
+        'max',
+        'min_time',
+        'min'
+        ])
+    SpmTStatistic = namedtuple('SpmTStatistic', [
+        't_statistic',
+        'spm_t'
+        ])
+    SpmTInference = namedtuple('SpmTInference', [
+        'alpha',
+        'p',
+        'threshold',
+        'clusters'
+        ])
+    SpmCluster = namedtuple('SpmCluster', [
+        'idx',
+        'p',
+        'start_time',
+        'end_time',
+        'centroid_time',
+        'centroid',
+        'extremum_time',
+        'extremum',
+        'area'
+        ])
```

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit/plotting.py` & `tmgtoolkit-0.1.2/src/tmgtoolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit/spm.py` & `tmgtoolkit-0.1.2/src/tmgtoolkit/spm.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             by the spm1d library. Meant for internal use only and subject to
             change in future versions.
         Access fields with e.g. `spm_ts.t_statistic`.
 
     """
     if mitigate_iir_filter_artefact:
         group1, group2 = _mitigate_iir_filter_artefact(group1, group2)
+    group1, group2 = _equalize_columns(group1, group2)
     spm_t = spm1d.stats.ttest_paired(group1.T, group2.T)
     return NamedTupleTypes.SpmTStatistic(t_statistic=spm_t.z, spm_t=spm_t)
 
 
 def get_spm_t_inference(spm_ts, t=None, alpha=0.05, two_tailed=True):
     """Performs SPM inference on the inputted SPM t-statistic data.
 
@@ -107,14 +108,15 @@
         - `alpha` (float): alpha used for inference.
         - `p` (float): p value for entire inference.
         - `threshold` (float): SPM t-statistic significance threshold value.
         - `clusters` (list): a list of SpmCluster namedtuples summarizing each
               supra-threshold cluster, or an empty list if the inference did
               not produce supra-threshold clusters. Each SpmCluster namedtuple
               has the following fields:
+              - `idx` (int): the cluster's 0-based index within `clusters`
               - `p` (float): the cluster's p value.
               - `start_time` (float): time at which the cluster begins, in the
                   same units as `t`.
               - `end_time` (float): time at which the cluster ends, in the same
                     units as `t`.
               - `centroid_time` (float): time of the cluster's centroid, in the
                     same units as `t`.
@@ -126,15 +128,14 @@
               - `extremum` (float): SPM t-statistic value of the cluster's
                 extremum.
               - `area` (float): the cluster's area, i.e. area of the region
                     bounded by the SPM t-statistic curve and the horizontal
                     line at the significance threshold
                     `spm_t_inference.threshold` from the cluster's `start_time`
                     to the cluster's `end_time`.
-        - `num_clusters` (int): the number of supra-threshold clusters.
         Access fields with e.g. `spm_t_inference.p` for the value of `p`.
     """
     spm_ti = spm_ts.spm_t.inference(alpha=alpha, two_tailed=two_tailed, interp=True)
 
     if t is None:
         t = np.arange(spm_ts.t_statistic)
 
@@ -189,14 +190,64 @@
     if mean2 > mean1:
         group2 = group2 - np.mean(mean2 - mean1)
     else:
         group1 = group1 - np.mean(mean1 - mean2)
     return (group1, group2)
 
 
+def _equalize_columns(group1, group2):
+    """Ensures inputted 2D arrays have the same number of columns.
+
+    Context: 2D arrays inputted to `spm1d`'s analysis functions require that
+    the arrays have the same number of rows and columns. This function
+    equalizes the number of columns in the inputted data, if necessary, so that
+    the data can be analyzed with `spm1d`.
+
+    The function works by computing the mean of the array with fewer columns,
+    and repeatedly appending this mean column to the array with fewer columns
+    until the number of columns in `group1` and `group2` are equal.
+
+    Parameters
+    ----------
+    group1 : ndarray
+        2D Numpy array holding at least two time series, as for
+        `get_spm_t_statistic`.
+    group2 : ndarray
+        2D Numpy array holding at least two time series, as for
+        `get_spm_t_statistic`.
+
+    Returns
+    -------
+    group_tuple : tuple
+        Tuple holding equalized versions of `group1` and `group2`; fields are
+        0. `group1` (ndarray)
+        1. `group2` (ndarray)
+    """
+    rows = group1.shape[0]
+    cols1 = group1.shape[1]
+    cols2 = group2.shape[1]
+    if cols1 == cols2:
+        return (group1, group2)
+
+    elif cols1 < cols2:
+        padded_group1 = np.zeros((rows, cols2))
+        padded_group1[:, 0:cols1] = group1
+        mean1 = np.mean(group1, axis=1)
+        for c in range(cols1, cols2):
+            padded_group1[:, c] = mean1
+        return (padded_group1, group2)
+    elif cols2 < cols1:
+        padded_group2 = np.zeros((rows, cols1))
+        padded_group2[:, 0:cols2] = group2
+        mean2 = np.mean(group2, axis=1)
+        for c in range(cols2, cols1):
+            padded_group2[:, c] = mean2
+        return (group1, padded_group2)
+
+
 def _get_spm_clusters(spm_ti, t):
     """Returns information describing an SPM inference object's clusters.
 
     Returns a list of SpmCluster namedtuples summarizing the supra-threshold
     clusters in the SPM inference object `spm_ti`.
 
     Parameters
@@ -219,31 +270,33 @@
         
     """
     # See _get_params_of_spm_cluster in frontiers/src/spm_analysis.py
     if spm_ti.clusters is None:
         return []
 
     clusters = []
-    for cluster in spm_ti.clusters:
-        clusters.append(_analyze_spm1d_cluster(cluster, t))
+    for idx, cluster in enumerate(spm_ti.clusters):
+        clusters.append(_analyze_spm1d_cluster(cluster, t, idx))
     return clusters
 
 
-def _analyze_spm1d_cluster(cluster, t):
+def _analyze_spm1d_cluster(cluster, t, idx):
     """Returns an SpmCluster namedtuple summarizing an SPM Cluster object.
 
     Parameters
     ----------
     spm1d_cluster : spm1d._clusters.Cluster
         An spm1d Cluster object representing a suprathreshold cluster
         associated with an SPM inference.
     t : ndarray
         1D Numpy array holding the time (or other independent variable) values
         on which the SPM t-statistic curve used to compute the inference object
         `spm_ti` is defined. See `get_spm_t_inference` for details.
+    idx : int
+        The cluster's 0-based index within its parent `clusters` list.
 
     Returns
     ----------
     cluster : SpmCluster
         An SpmCluster namedtuple summarizing the inputted
         spm1d._clusters.Cluster object. See `get_spm_t_inference` for
         documentation of SpmCluster fields.
@@ -270,13 +323,13 @@
     cluster_area = area_above_x - threshold*(idxs[-1] - idxs[0])
 
     start_time = _idx_to_time(start_idx, t)
     end_time = _idx_to_time(end_idx, t)
     centroid_time = _idx_to_time(centroid_idx, t)
     extremum_time = _idx_to_time(extremum_idx, t)
 
-    return NamedTupleTypes.SpmCluster(p=cluster.P, start_time=start_time,
+    return NamedTupleTypes.SpmCluster(idx=idx, p=cluster.P, start_time=start_time,
                                       end_time=end_time,
                                       centroid_time=centroid_time,
                                       centroid=centroid,
                                       extremum_time=extremum_time,
                                       extremum=extremum, area=cluster_area)
```

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit/time_series.py` & `tmgtoolkit-0.1.2/src/tmgtoolkit/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
     ----------
     time : float
         Approximate independent variable value, in units of `t`, corresponding
         to `idx`; loosely, an estimate of the value t(idx) if `t` were
         continuous.
     """
     if idx.is_integer():
-        return t[int(idx)]
+        return float(t[int(idx)])
 
     idx_floor = math.floor(idx)
     idx_ceil = math.ceil(idx)
     ratio = (idx - idx_floor)/(idx_ceil - idx_floor)
 
     t_floor = t[idx_floor]
     t_ceil = t[idx_ceil]
```

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit/tmgio.py` & `tmgtoolkit-0.1.2/src/tmgtoolkit/tmgio.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     if skipcols is None:
         skipcols = IoConstants.TMG_EXCEL_MAGIC_VALUES['data_start_col_idx']
 
     usecols = lambda col: col >= skipcols and ((col < (ncols + skipcols)) if ncols is not None else True)
     return pd.read_excel(fname, header=None, skiprows=skiprows, nrows=nrows, usecols=usecols).values
 
 
-def split_data_for_spm(data, numsets, n1, n2):
+def split_data_for_spm(data, numsets, n1, n2, nrows=None):
     """Splits structured inputted data into two groups for analysis with SPM.
 
     Splits the time series in the inputted 2D array `data` into two groups, 1
     and 2, that can then be compared to each other with SPM analysis.
 
     The function assumes `data` has a well-defined structure, namely that the
     time series in `data` are divided into `numsets` sets, where each set
@@ -68,14 +68,17 @@
         Tuple holding group 1 and group 2 series. Fields are
         0 (group1) : ndarray
             2D Numpy array holding group 1 measurements.
         1 (group2) : ndarray
             2D Numpy array holding group 2 measurements.
 
     """
+    if nrows is None:
+        nrows = data.shape[0]
+
     idxs1 = []
     idxs2 = []
     n = n1 + n2
     for s in range(numsets):
         idxs1.extend(range(s*n, s*n + n1))
         idxs2.extend(range(s*n + n1, (s + 1)*n))
-    return (data[:, idxs1], data[:, idxs2])
+    return (data[:nrows, idxs1], data[:nrows, idxs2])
```

### Comparing `tmgtoolkit-0.1.1/src/tmgtoolkit.egg-info/PKG-INFO` & `tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

