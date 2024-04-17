# Comparing `tmp/ehdg_tools-4.1.0.tar.gz` & `tmp/ehdg_tools-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_tools-4.1.0.tar", last modified: Tue Mar 12 02:07:00 2024, max compression
+gzip compressed data, was "ehdg_tools-4.2.0.tar", last modified: Wed Apr 17 02:20:21 2024, max compression
```

## Comparing `ehdg_tools-4.1.0.tar` & `ehdg_tools-4.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 02:07:00.101575 ehdg_tools-4.1.0/
--rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.1.0/LICENSE
--rw-rw-rw-   0        0        0     3001 2024-03-12 02:07:00.100578 ehdg_tools-4.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.1.0/README.md
--rw-rw-rw-   0        0        0      699 2024-03-12 02:06:19.000000 ehdg_tools-4.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 02:07:00.101575 ehdg_tools-4.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 02:07:00.077597 ehdg_tools-4.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 02:07:00.085618 ehdg_tools-4.1.0/src/ehdg_tools/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.1.0/src/ehdg_tools/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.1.0/src/ehdg_tools/ehdg_buffers.py
--rw-rw-rw-   0        0        0      530 2023-12-04 12:16:10.000000 ehdg_tools-4.1.0/src/ehdg_tools/ehdg_functions.py
--rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.1.0/src/ehdg_tools/ehdg_okn_checker.py
--rw-rw-rw-   0        0        0   115844 2024-03-12 02:05:35.000000 ehdg_tools-4.1.0/src/ehdg_tools/ehdg_plotter.py
--rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.1.0/src/ehdg_tools/ehdg_updater.py
-drwxrwxrwx   0        0        0        0 2024-03-12 02:07:00.099581 ehdg_tools-4.1.0/src/ehdg_tools.egg-info/
--rw-rw-rw-   0        0        0     3001 2024-03-12 02:07:00.000000 ehdg_tools-4.1.0/src/ehdg_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-03-12 02:07:00.000000 ehdg_tools-4.1.0/src/ehdg_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 02:07:00.000000 ehdg_tools-4.1.0/src/ehdg_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-12 02:07:00.000000 ehdg_tools-4.1.0/src/ehdg_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 02:20:21.740228 ehdg_tools-4.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3001 2024-04-17 02:20:21.739230 ehdg_tools-4.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.0/README.md
+-rw-rw-rw-   0        0        0      699 2024-04-17 02:19:11.000000 ehdg_tools-4.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:20:21.740228 ehdg_tools-4.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 02:20:21.716773 ehdg_tools-4.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 02:20:21.726236 ehdg_tools-4.2.0/src/ehdg_tools/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.0/src/ehdg_tools/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.0/src/ehdg_tools/ehdg_buffers.py
+-rw-rw-rw-   0        0        0      530 2023-12-04 12:16:10.000000 ehdg_tools-4.2.0/src/ehdg_tools/ehdg_functions.py
+-rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.0/src/ehdg_tools/ehdg_okn_checker.py
+-rw-rw-rw-   0        0        0   117308 2024-04-17 02:17:15.000000 ehdg_tools-4.2.0/src/ehdg_tools/ehdg_plotter.py
+-rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.0/src/ehdg_tools/ehdg_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:20:21.738232 ehdg_tools-4.2.0/src/ehdg_tools.egg-info/
+-rw-rw-rw-   0        0        0     3001 2024-04-17 02:20:21.000000 ehdg_tools-4.2.0/src/ehdg_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-17 02:20:21.000000 ehdg_tools-4.2.0/src/ehdg_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:20:21.000000 ehdg_tools-4.2.0/src/ehdg_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 02:20:21.000000 ehdg_tools-4.2.0/src/ehdg_tools.egg-info/top_level.txt
```

### Comparing `ehdg_tools-4.1.0/LICENSE` & `ehdg_tools-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/PKG-INFO` & `ehdg_tools-4.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.1.0
+Version: 4.2.0
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_tools-4.1.0/README.md` & `ehdg_tools-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/pyproject.toml` & `ehdg_tools-4.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_tools"
-version = "4.1.0"
+version = "4.2.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python library useful tools for ABI Eye Health Diagnostic Group"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools/ehdg_buffers.py` & `ehdg_tools-4.2.0/src/ehdg_tools/ehdg_buffers.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools/ehdg_functions.py` & `ehdg_tools-4.2.0/src/ehdg_tools/ehdg_functions.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools/ehdg_okn_checker.py` & `ehdg_tools-4.2.0/src/ehdg_tools/ehdg_okn_checker.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools/ehdg_plotter.py` & `ehdg_tools-4.2.0/src/ehdg_tools/ehdg_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2007,14 +2007,52 @@
         else:
             print("There is only 1 logmar level in the given data.")
             print("Therefore, we cannot draw simpler graph. It needs at least 2 logmar level.")
     else:
         print("There is nothing to plot")
 
 
+def raw_plot(input_csv_dir, plot_info, output_dir=None):
+    x_data_column_name = plot_info["x_data_column_name"]
+    y_data_column_name = plot_info["y_data_column_name"]
+    graph_line_color = plot_info["graph_line_color"]
+    graph_line_thickness = plot_info["graph_line_thickness"]
+    mean_offset = plot_info["mean_offset"]
+
+    if output_dir is None:
+        csv_file_name = os.path.basename(input_csv_dir)
+        plot_image_name = str(csv_file_name).replace(".csv", ".png")
+        output_dir = str(input_csv_dir).replace(csv_file_name, plot_image_name)
+
+    x_array = get_data_array(input_csv_dir, x_data_column_name)
+    y_array = get_data_array(input_csv_dir, y_data_column_name)
+
+    x_array_max = math.ceil(max(x_array))
+
+    if x_array_max <= 100:
+        x_fig_size = int(x_array_max * 2)
+    else:
+        x_fig_size = int(x_array_max * 0.8)
+
+    figsize = (x_fig_size, 5)
+    plt.figure(figsize=figsize)
+    plt.margins(x=0.001)
+    plt.xlabel(x_data_column_name)
+    plt.ylabel(y_data_column_name)
+    y_limit_mean = np.mean(y_array)
+    y_lower_limit = y_limit_mean - mean_offset
+    y_upper_limit = y_limit_mean + mean_offset
+    plt.ylim(y_lower_limit, y_upper_limit)
+    x_axis_array = np.arange(start=min(x_array), stop=max(x_array), step=1)
+    plt.xticks(x_axis_array)
+    plt.plot(x_array, y_array, color=graph_line_color, linewidth=graph_line_thickness)
+    plt.savefig(output_dir)
+    plt.close()
+
+
 def get_plot_info_for_simpler(data_dir, plot_info_input, referenced_csv_dir_input):
     x_label = plot_info_input["x_label"]
     y_label = plot_info_input["y_label"]
     x_data_column_name = plot_info_input["x_data_column_name"]
     y_data_column_name = plot_info_input["y_data_column_name"]
     x_axis_limit = plot_info_input["x_axis_limit"]
     y_axis_limit = plot_info_input["y_axis_limit"]
```

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools/ehdg_updater.py` & `ehdg_tools-4.2.0/src/ehdg_tools/ehdg_updater.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.1.0/src/ehdg_tools.egg-info/PKG-INFO` & `ehdg_tools-4.2.0/src/ehdg_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.1.0
+Version: 4.2.0
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

