# Comparing `tmp/spc_toolbox-0.1.1.tar.gz` & `tmp/spc_toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spc_toolbox-0.1.1.tar", max compression
+gzip compressed data, was "spc_toolbox-0.1.2.tar", max compression
```

## Comparing `spc_toolbox-0.1.1.tar` & `spc_toolbox-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-04 18:11:46.861269 spc_toolbox-0.1.1/LICENSE
--rw-r--r--   0        0        0     2392 2024-04-04 18:12:45.362203 spc_toolbox-0.1.1/README.md
--rw-r--r--   0        0        0      460 2024-04-15 19:00:53.023774 spc_toolbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14913 2024-04-15 19:28:06.702897 spc_toolbox-0.1.1/spc_toolbox/ControlChart.py
--rw-r--r--   0        0        0     1689 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/IChart.py
--rw-r--r--   0        0        0     1624 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/MRChart.py
--rw-r--r--   0        0        0     1822 2024-04-15 18:54:12.966686 spc_toolbox-0.1.1/spc_toolbox/PChart.py
--rw-r--r--   0        0        0     2440 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/RChart.py
--rw-r--r--   0        0        0     2309 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/SChart.py
--rw-r--r--   0        0        0     1820 2024-04-15 18:53:18.006678 spc_toolbox-0.1.1/spc_toolbox/UChart.py
--rw-r--r--   0        0        0     3384 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/XBarChart.py
--rw-r--r--   0        0        0      258 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/__init__.py
--rw-r--r--   0        0        0     2877 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/utils.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 spc_toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 18:11:46.861269 spc_toolbox-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2392 2024-04-04 18:12:45.362203 spc_toolbox-0.1.2/README.md
+-rw-r--r--   0        0        0      460 2024-04-17 11:19:46.937206 spc_toolbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    16444 2024-04-17 12:05:25.828557 spc_toolbox-0.1.2/spc_toolbox/ControlChart.py
+-rw-r--r--   0        0        0     1689 2024-04-04 18:12:44.562190 spc_toolbox-0.1.2/spc_toolbox/IChart.py
+-rw-r--r--   0        0        0     1667 2024-04-16 07:54:12.039974 spc_toolbox-0.1.2/spc_toolbox/MRChart.py
+-rw-r--r--   0        0        0     1874 2024-04-16 09:30:56.780959 spc_toolbox-0.1.2/spc_toolbox/PChart.py
+-rw-r--r--   0        0        0     2440 2024-04-04 18:12:44.562190 spc_toolbox-0.1.2/spc_toolbox/RChart.py
+-rw-r--r--   0        0        0     2309 2024-04-04 18:12:44.562190 spc_toolbox-0.1.2/spc_toolbox/SChart.py
+-rw-r--r--   0        0        0     1820 2024-04-16 08:07:42.268985 spc_toolbox-0.1.2/spc_toolbox/UChart.py
+-rw-r--r--   0        0        0     3384 2024-04-04 18:12:44.582191 spc_toolbox-0.1.2/spc_toolbox/XBarChart.py
+-rw-r--r--   0        0        0      258 2024-04-04 18:12:44.582191 spc_toolbox-0.1.2/spc_toolbox/__init__.py
+-rw-r--r--   0        0        0     2877 2024-04-04 18:12:44.582191 spc_toolbox-0.1.2/spc_toolbox/utils.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 spc_toolbox-0.1.2/PKG-INFO
```

### Comparing `spc_toolbox-0.1.1/LICENSE` & `spc_toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/README.md` & `spc_toolbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/ControlChart.py` & `spc_toolbox-0.1.2/spc_toolbox/ControlChart.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,19 +263,45 @@
         
         if fig is None and ax is None:
             fig, ax = plt.subplots(figsize=(10, 6))
 
         ax.set_title(f"{self.__class__.__name__}")
         ax.set_xlabel(self.x.name)
         ax.set_ylabel(self.y.name)
-        ax.plot(self.x, self.upper_control_limit, 'r--', label='UCL')
-        ax.plot(self.x, self.center_line, color='green', linestyle='-', label='CL')
-        ax.plot(self.x, self.lower_control_limit, 'r--', label='LCL')
+        ax.step(self.x, self.upper_control_limit, 'r--', label='UCL')
+        ax.step(self.x, self.center_line, color='green', linestyle='-', label='CL')
+        ax.step(self.x, self.lower_control_limit, 'r--', label='LCL')
         ax.plot(self.x, self.y, marker='o', linestyle='-')
 
+        # Define a list of colors for visual distinction
+        colors = ['red', 'purple', 'orange', 'brown', 'pink', 'yellow', 'cyan', 'magenta', 'gray', 'green']
+
+        # Evaluate the rules
+        rule_results = self.evaluate_rules()
+
+        # To ensure each rule is represented once in the legend, we will keep track of which rules have been added
+        added_rules = set()
+
+        # Plot the points where rules are satisfied, if results are boolean Series
+        for index, (rule_name, results) in enumerate(rule_results.items()):
+            if isinstance(results, pd.Series) and results.dtype == bool:
+                satisfied_indices = results.index[results == True]
+                color = colors[index % len(colors)]  # Cycle through colors list
+                # Only add the rule to the legend the first time it is encountered
+                for idx in satisfied_indices:
+                    if rule_name not in added_rules:
+                        ax.plot([self.x.loc[idx]], [self.y.loc[idx]], 'o', markersize=7, color=color, label=rule_name)
+                        added_rules.add(rule_name)  # Mark this rule as added to the legend
+                    else:
+                        ax.plot([self.x.loc[idx]], [self.y.loc[idx]], 'o', markersize=7, markeredgewidth=2, color=color, label="_nolegend_")
+
+        # Adding and customizing the legend
+        ax.legend(fontsize='xx-small', title_fontsize='xx-small', loc='upper right')
+
+
 class CompositeControlChart:
     def __init__(self, charts: List[ControlChart]):
         """
         Initializes a CompositeControlChart object with a list of ControlChart objects.
         
         Parameters:
         - charts (List[ControlChart]): A list of ControlChart objects to be combined into a composite chart.
@@ -374,14 +400,16 @@
         - kwargs: Keyword arguments to be passed to the fit method of each ControlChart object.
         
         Returns:
         - The CompositeControlChart object with the data fitted for each ControlChart object in the list.
         """
         for chart in self.charts:
             chart.fit(**kwargs)
+
+        self.df = pd.concat([chart.df for chart in self.charts], axis=1)
         return self
 
     def plot(self):
         """
         Plots the CompositeControlChart object.
         """
         fig, axs = plt.subplots(1, len(self.charts), figsize=(len(self.charts) * 10, 6))
```

### Comparing `spc_toolbox-0.1.1/spc_toolbox/IChart.py` & `spc_toolbox-0.1.2/spc_toolbox/IChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/MRChart.py` & `spc_toolbox-0.1.2/spc_toolbox/MRChart.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             raise TypeError("values must be a Series.")
         if type(n) != int:
             raise ValueError("n must be an integer.")
         if n < 1:
             raise ValueError("n must be greater than 0.")
         
         moving_range = values.diff(n - 1).abs()
+        moving_range.name = "Moving Range"
         moving_range_average = values.diff(n - 1).abs().mean()
 
         D4 = get_chart_constant('D4', n)
         D3 = get_chart_constant('D3', n)
         d2 = get_chart_constant('d2', n)
         self.sigma = moving_range_average / d2
```

### Comparing `spc_toolbox-0.1.1/spc_toolbox/PChart.py` & `spc_toolbox-0.1.2/spc_toolbox/PChart.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,22 @@
             raise TypeError("defectives must be a Series.")
         if not isinstance(sample_sizes, pd.Series) and not isinstance(sample_sizes, int):
             raise TypeError("sample_sizes must be a Series or an integer.")
         if type(z) != float:
             raise TypeError("z must be a float.")
 
         proportions = defectives / sample_sizes
+        proportions.name = "Proportions"
 
         overall_proportion = defectives.sum() / sample_sizes.sum()
+        average_sample_size = sample_sizes.sum() / len(sample_sizes) # 
 
-        std_dev = np.sqrt(proportions * (1 - proportions) / sample_sizes)
+        std_dev = np.sqrt(proportions * (1 - proportions) / average_sample_size)
         self.sigma = std_dev
 
         center_line = overall_proportion
-        # center_line = pd.Series([average_proportion] * len(index))
+
         upper_control_limit = overall_proportion + z * std_dev
         lower_control_limit = np.maximum(overall_proportion - z * std_dev, 0)
 
         super().fit(index, proportions, lower_control_limit, center_line, upper_control_limit)
         return self
```

### Comparing `spc_toolbox-0.1.1/spc_toolbox/RChart.py` & `spc_toolbox-0.1.2/spc_toolbox/RChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/SChart.py` & `spc_toolbox-0.1.2/spc_toolbox/SChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/UChart.py` & `spc_toolbox-0.1.2/spc_toolbox/UChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/XBarChart.py` & `spc_toolbox-0.1.2/spc_toolbox/XBarChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/spc_toolbox/utils.py` & `spc_toolbox-0.1.2/spc_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.1/PKG-INFO` & `spc_toolbox-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spc-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolbox for Statistical Process Control
 Author: Philip Solarz
 Author-email: philip.solarz@teliacompany.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

