# Comparing `tmp/PVNet_summation-0.1.3.tar.gz` & `tmp/pvnet_summation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet_summation-0.1.3.tar", last modified: Thu Feb 29 17:04:07 2024, max compression
+gzip compressed data, was "pvnet_summation-0.1.4.tar", last modified: Wed Apr 17 13:22:54 2024, max compression
```

## Comparing `PVNet_summation-0.1.3.tar` & `pvnet_summation-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.215064 PVNet_summation-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-29 17:04:07.215064 PVNet_summation-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.215064 PVNet_summation-0.1.3/PVNet_summation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-29 17:04:07.000000 PVNet_summation-0.1.3/PVNet_summation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-29 17:04:07.000000 PVNet_summation-0.1.3/PVNet_summation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 17:04:07.000000 PVNet_summation-0.1.3/PVNet_summation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-29 17:04:07.000000 PVNet_summation-0.1.3/PVNet_summation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 17:04:07.000000 PVNet_summation-0.1.3/PVNet_summation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.211064 PVNet_summation-0.1.3/pvnet_summation/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.211064 PVNet_summation-0.1.3/pvnet_summation/data/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/data/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.211064 PVNet_summation-0.1.3/pvnet_summation/models/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/pvnet_summation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 17:04:07.215064 PVNet_summation-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:07.215064 PVNet_summation-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-29 17:04:03.000000 PVNet_summation-0.1.3/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/PVNet_summation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 13:22:54.000000 pvnet_summation-0.1.4/PVNet_summation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 13:22:54.000000 pvnet_summation-0.1.4/PVNet_summation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:22:54.000000 pvnet_summation-0.1.4/PVNet_summation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-17 13:22:54.000000 pvnet_summation-0.1.4/PVNet_summation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 13:22:54.000000 pvnet_summation-0.1.4/PVNet_summation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/pvnet_summation/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/pvnet_summation/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/data/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/pvnet_summation/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/pvnet_summation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:54.809896 pvnet_summation-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 13:22:50.000000 pvnet_summation-0.1.4/tests/test_end2end.py
```

### Comparing `PVNet_summation-0.1.3/LICENSE` & `pvnet_summation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/PKG-INFO` & `pvnet_summation-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PVNet_summation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for training summation model for PVNet
 Author: James Fulton
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ocf_datapipes==3.2.*
-Requires-Dist: pvnet==3.0.*
+Requires-Dist: ocf_datapipes>=3.3.19
+Requires-Dist: pvnet>=3.0.25
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: xarray
 Requires-Dist: ipykernel
 Requires-Dist: h5netcdf
 Requires-Dist: torch>=2.0.0
```

### Comparing `PVNet_summation-0.1.3/PVNet_summation.egg-info/PKG-INFO` & `pvnet_summation-0.1.4/PVNet_summation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PVNet_summation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for training summation model for PVNet
 Author: James Fulton
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ocf_datapipes==3.2.*
-Requires-Dist: pvnet==3.0.*
+Requires-Dist: ocf_datapipes>=3.3.19
+Requires-Dist: pvnet>=3.0.25
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: xarray
 Requires-Dist: ipykernel
 Requires-Dist: h5netcdf
 Requires-Dist: torch>=2.0.0
```

### Comparing `PVNet_summation-0.1.3/PVNet_summation.egg-info/SOURCES.txt` & `pvnet_summation-0.1.4/PVNet_summation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/pvnet_summation/callbacks.py` & `pvnet_summation-0.1.4/pvnet_summation/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/pvnet_summation/data/datamodule.py` & `pvnet_summation-0.1.4/pvnet_summation/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/pvnet_summation/models/base_model.py` & `pvnet_summation-0.1.4/pvnet_summation/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,30 +61,31 @@
         # This setting is only used when lr is tuned with callback
         self.lr = None
 
         self.forecast_minutes = self.pvnet_model.forecast_minutes
         self.output_quantiles = output_quantiles
 
         # Number of timestemps for 30 minutely data
-        self.forecast_len_30 = self.forecast_minutes // 30
+        self.forecast_len = self.forecast_minutes // 30
 
-        self.weighted_losses = WeightedLosses(forecast_length=self.forecast_len_30)
+        self.weighted_losses = WeightedLosses(forecast_length=self.forecast_len)
 
         self._accumulated_metrics = MetricAccumulator()
         self._accumulated_y = PredAccumulator()
         self._accumulated_y_hat = PredAccumulator()
         self._accumulated_y_sum = PredAccumulator()
         self._accumulated_times = PredAccumulator()
+        self._horizon_maes = MetricAccumulator()
 
         self.use_quantile_regression = self.output_quantiles is not None
 
         if self.use_quantile_regression:
-            self.num_output_features = self.forecast_len_30 * len(self.output_quantiles)
+            self.num_output_features = self.forecast_len * len(self.output_quantiles)
         else:
-            self.num_output_features = self.forecast_len_30
+            self.num_output_features = self.forecast_len
 
         if self.pvnet_model.use_quantile_regression:
             self.pvnet_output_shape = (
                 317,
                 self.pvnet_model.forecast_len,
                 len(self.pvnet_model.output_quantiles),
             )
```

### Comparing `PVNet_summation-0.1.3/pvnet_summation/models/model.py` & `pvnet_summation-0.1.4/pvnet_summation/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             x_in = x["pvnet_outputs"]
 
         x_in = torch.flatten(x_in, start_dim=1)
         out = self.model(x_in)
 
         if self.use_quantile_regression:
             # Shape: batch_size, seq_length * num_quantiles
-            out = out.reshape(out.shape[0], self.forecast_len_30, len(self.output_quantiles))
+            out = out.reshape(out.shape[0], self.forecast_len, len(self.output_quantiles))
 
         if self.predict_difference_from_sum:
             gsp_sum = self.sum_of_gsps(x)
 
             if self.use_quantile_regression:
                 gsp_sum = gsp_sum.unsqueeze(-1)
```

### Comparing `PVNet_summation-0.1.3/pvnet_summation/training.py` & `pvnet_summation-0.1.4/pvnet_summation/training.py`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/pvnet_summation/utils.py` & `pvnet_summation-0.1.4/pvnet_summation/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet_summation-0.1.3/setup.py` & `pvnet_summation-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="PVNet_summation",
-    version="0.1.3",
+    version="0.1.4",
     license="MIT",
     description="Package for training summation model for PVNet",
     author="James Fulton",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `PVNet_summation-0.1.3/tests/conftest.py` & `pvnet_summation-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

