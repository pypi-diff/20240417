# Comparing `tmp/multidst-0.0.1.tar.gz` & `tmp/multidst-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidst-0.0.1.tar", last modified: Thu Apr 11 13:31:36 2024, max compression
+gzip compressed data, was "multidst-0.0.2.tar", last modified: Wed Apr 17 18:08:26 2024, max compression
```

## Comparing `multidst-0.0.1.tar` & `multidst-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:31:36.622245 multidst-0.0.1/
--rw-rw-rw-   0        0        0      267 2024-04-11 13:31:36.619083 multidst-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-05 18:29:30.000000 multidst-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 13:31:36.450298 multidst-0.0.1/multidst/
--rw-rw-rw-   0        0        0       80 2024-04-07 20:03:31.000000 multidst-0.0.1/multidst/__init__.py
--rw-rw-rw-   0        0        0     3115 2024-04-11 12:20:23.000000 multidst-0.0.1/multidst/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:31:36.582896 multidst-0.0.1/multidst/methods/
--rw-rw-rw-   0        0        0      560 2024-04-05 18:55:56.000000 multidst-0.0.1/multidst/methods/BH.py
--rw-rw-rw-   0        0        0      553 2024-04-05 18:26:19.000000 multidst-0.0.1/multidst/methods/BY.py
--rw-rw-rw-   0        0        0      175 2024-04-07 09:51:41.000000 multidst-0.0.1/multidst/methods/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-05 18:55:56.000000 multidst-0.0.1/multidst/methods/bonf.py
--rw-rw-rw-   0        0        0      980 2024-04-05 18:26:26.000000 multidst-0.0.1/multidst/methods/holm_bonf.py
--rw-rw-rw-   0        0        0     3122 2024-04-11 12:09:21.000000 multidst-0.0.1/multidst/methods/qval.py
--rw-rw-rw-   0        0        0     1339 2024-04-05 18:27:20.000000 multidst-0.0.1/multidst/methods/sgof.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:31:36.610581 multidst-0.0.1/multidst/utils/
--rw-rw-rw-   0        0        0       97 2024-04-07 16:43:17.000000 multidst-0.0.1/multidst/utils/__init__.py
--rw-rw-rw-   0        0        0     3472 2024-04-11 07:33:15.000000 multidst-0.0.1/multidst/utils/common_indices.py
--rw-rw-rw-   0        0        0    13712 2024-04-11 12:46:06.000000 multidst-0.0.1/multidst/utils/visualization.py
--rw-rw-rw-   0        0        0     7504 2024-04-11 08:13:12.000000 multidst-0.0.1/multidst/utils/weighting.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:31:36.614312 multidst-0.0.1/multidst.egg-info/
--rw-rw-rw-   0        0        0      267 2024-04-11 13:31:36.000000 multidst-0.0.1/multidst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-11 13:31:36.000000 multidst-0.0.1/multidst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:31:36.000000 multidst-0.0.1/multidst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-11 13:31:36.000000 multidst-0.0.1/multidst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 13:31:36.000000 multidst-0.0.1/multidst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 13:31:36.622245 multidst-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-04-11 13:31:24.000000 multidst-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:08:26.225406 multidst-0.0.2/
+-rw-rw-rw-   0        0        0      267 2024-04-17 18:08:26.224393 multidst-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-05 18:29:30.000000 multidst-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 18:08:26.171566 multidst-0.0.2/multidst/
+-rw-rw-rw-   0        0        0       80 2024-04-07 20:03:31.000000 multidst-0.0.2/multidst/__init__.py
+-rw-rw-rw-   0        0        0     3121 2024-04-17 18:02:26.000000 multidst-0.0.2/multidst/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:08:26.210496 multidst-0.0.2/multidst/methods/
+-rw-rw-rw-   0        0        0      560 2024-04-05 18:55:56.000000 multidst-0.0.2/multidst/methods/BH.py
+-rw-rw-rw-   0        0        0      553 2024-04-05 18:26:19.000000 multidst-0.0.2/multidst/methods/BY.py
+-rw-rw-rw-   0        0        0      175 2024-04-07 09:51:41.000000 multidst-0.0.2/multidst/methods/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-05 18:55:56.000000 multidst-0.0.2/multidst/methods/bonf.py
+-rw-rw-rw-   0        0        0      980 2024-04-05 18:26:26.000000 multidst-0.0.2/multidst/methods/holm_bonf.py
+-rw-rw-rw-   0        0        0     3122 2024-04-11 12:09:21.000000 multidst-0.0.2/multidst/methods/qval.py
+-rw-rw-rw-   0        0        0     1339 2024-04-05 18:27:20.000000 multidst-0.0.2/multidst/methods/sgof.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:08:26.219730 multidst-0.0.2/multidst/utils/
+-rw-rw-rw-   0        0        0       97 2024-04-07 16:43:17.000000 multidst-0.0.2/multidst/utils/__init__.py
+-rw-rw-rw-   0        0        0     3472 2024-04-17 18:04:08.000000 multidst-0.0.2/multidst/utils/common_indices.py
+-rw-rw-rw-   0        0        0    13712 2024-04-17 18:04:24.000000 multidst-0.0.2/multidst/utils/visualization.py
+-rw-rw-rw-   0        0        0     7548 2024-04-17 18:07:25.000000 multidst-0.0.2/multidst/utils/weighting.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:08:26.222021 multidst-0.0.2/multidst.egg-info/
+-rw-rw-rw-   0        0        0      267 2024-04-17 18:08:25.000000 multidst-0.0.2/multidst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-17 18:08:25.000000 multidst-0.0.2/multidst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 18:08:25.000000 multidst-0.0.2/multidst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-17 18:08:25.000000 multidst-0.0.2/multidst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 18:08:25.000000 multidst-0.0.2/multidst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 18:08:26.225406 multidst-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      415 2024-04-17 18:08:04.000000 multidst-0.0.2/setup.py
```

### Comparing `multidst-0.0.1/multidst/functions.py` & `multidst-0.0.2/multidst/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,12 @@
       sig_df = pd.DataFrame(sig_len_dict, index=[0])
       print("\n",sig_df, "\n")
 
     return sig_dict
 
 import random
 
-p_values = [random.uniform(0,1) for i in range(1000)]
-multitest(p_values, alpha=0.05, sigplot=True, results = True)
-multitest(p_values, alpha=0.05, sigplot=False, results=True)
+# p_values = [random.uniform(0,1) for i in range(1000)]
+# multitest(p_values, alpha=0.05, sigplot=True, results = True)
+# multitest(p_values, alpha=0.05, sigplot=False, results=True)
```

### Comparing `multidst-0.0.1/multidst/methods/BH.py` & `multidst-0.0.2/multidst/methods/BH.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/methods/BY.py` & `multidst-0.0.2/multidst/methods/BY.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/methods/bonf.py` & `multidst-0.0.2/multidst/methods/bonf.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/methods/holm_bonf.py` & `multidst-0.0.2/multidst/methods/holm_bonf.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/methods/qval.py` & `multidst-0.0.2/multidst/methods/qval.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/methods/sgof.py` & `multidst-0.0.2/multidst/methods/sgof.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/utils/common_indices.py` & `multidst-0.0.2/multidst/utils/common_indices.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/utils/visualization.py` & `multidst-0.0.2/multidst/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.1/multidst/utils/weighting.py` & `multidst-0.0.2/multidst/utils/weighting.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,36 +145,36 @@
 
     return optimal_weights, weighted_list, optimal_weights1
 
 
 ### Examples
 
 ## Example 01 - Using Multi-Weights
-p_values = np.random.random(22)
+# p_values = np.random.random(22)
 
-p_values
-l0 = [1, 2,3]  # Example list l0
-l1 = [4, 5, 6]  # Example list l1
-l2 = []  # Example list l2
-l3 = [10, 11, 12,7,8,9]  # Example list l3
-l4 = [13, 14, 15]  # Example list l4
-l5 = [16, 17, 18]  # Example list l5
-l6 = [19, 20, 21,0]  # Example list l6
-
-weighting = weighted_p_list(p_values, weights="multi")
-weighting[0]
-weighting[1]
-
-
-# Example 02 - Using IHW
-p_values = [0.5, 0.05, 0.2, 0.3, 0.01]
-weights = [1.5, 0.8, 1.0, 0.5, 1.2]
-
-calculated_weights, calculated_weighted_p_values = weighted_p_list(p_values, weights=weights)
-
-# Print the calculated weights and weighted p-values
-print("Calculated weights:", calculated_weights)
-print("Calculated weighted p-values:", calculated_weighted_p_values)
-
-import random
-p_values = [random.uniform(0,0.03) for i in range(1000)]
-weighted_p_list(p_values, weights="multi",max_weight=1.5, min_weight = 0.5)[0]
+# p_values
+# l0 = [1, 2,3]  # Example list l0
+# l1 = [4, 5, 6]  # Example list l1
+# l2 = []  # Example list l2
+# l3 = [10, 11, 12,7,8,9]  # Example list l3
+# l4 = [13, 14, 15]  # Example list l4
+# l5 = [16, 17, 18]  # Example list l5
+# l6 = [19, 20, 21,0]  # Example list l6
+
+# weighting = weighted_p_list(p_values, weights="multi")
+# weighting[0]
+# weighting[1]
+
+
+# # Example 02 - Using IHW
+# p_values = [0.5, 0.05, 0.2, 0.3, 0.01]
+# weights = [1.5, 0.8, 1.0, 0.5, 1.2]
+
+# calculated_weights, calculated_weighted_p_values = weighted_p_list(p_values, weights=weights)
+
+# # Print the calculated weights and weighted p-values
+# print("Calculated weights:", calculated_weights)
+# print("Calculated weighted p-values:", calculated_weighted_p_values)
+
+# import random
+# p_values = [random.uniform(0,0.03) for i in range(1000)]
+# weighted_p_list(p_values, weights="multi",max_weight=1.5, min_weight = 0.5)[0]
```

### Comparing `multidst-0.0.1/multidst.egg-info/SOURCES.txt` & `multidst-0.0.2/multidst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

