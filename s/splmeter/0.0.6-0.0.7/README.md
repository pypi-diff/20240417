# Comparing `tmp/splmeter-0.0.6.tar.gz` & `tmp/splmeter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splmeter-0.0.6.tar", last modified: Fri Nov 10 20:05:44 2023, max compression
+gzip compressed data, was "splmeter-0.0.7.tar", last modified: Wed Apr 17 20:08:55 2024, max compression
```

## Comparing `splmeter-0.0.6.tar` & `splmeter-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:44.980040 splmeter-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-10 20:05:38.000000 splmeter-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-11-10 20:05:44.980040 splmeter-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-10 20:05:38.000000 splmeter-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-10 20:05:38.000000 splmeter-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 20:05:44.980040 splmeter-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:44.980040 splmeter-0.0.6/splmeter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:44.980040 splmeter-0.0.6/splmeter/measure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/measure/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/measure/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:44.980040 splmeter-0.0.6/splmeter/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/processing/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/processing/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-10 20:05:38.000000 splmeter-0.0.6/splmeter/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 20:05:44.980040 splmeter-0.0.6/splmeter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-11-10 20:05:44.000000 splmeter-0.0.6/splmeter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-11-10 20:05:44.000000 splmeter-0.0.6/splmeter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 20:05:44.000000 splmeter-0.0.6/splmeter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-10 20:05:44.000000 splmeter-0.0.6/splmeter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-10 20:05:44.000000 splmeter-0.0.6/splmeter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:55.502642 splmeter-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 20:08:44.000000 splmeter-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-17 20:08:55.502642 splmeter-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 20:08:44.000000 splmeter-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 20:08:44.000000 splmeter-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:08:55.502642 splmeter-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:55.502642 splmeter-0.0.7/splmeter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:55.502642 splmeter-0.0.7/splmeter/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/measure/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/measure/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:55.502642 splmeter-0.0.7/splmeter/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/processing/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/processing/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 20:08:44.000000 splmeter-0.0.7/splmeter/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:55.502642 splmeter-0.0.7/splmeter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-17 20:08:55.000000 splmeter-0.0.7/splmeter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 20:08:55.000000 splmeter-0.0.7/splmeter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:08:55.000000 splmeter-0.0.7/splmeter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 20:08:55.000000 splmeter-0.0.7/splmeter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 20:08:55.000000 splmeter-0.0.7/splmeter.egg-info/top_level.txt
```

### Comparing `splmeter-0.0.6/LICENSE` & `splmeter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/PKG-INFO` & `splmeter-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splmeter
-Version: 0.0.6
+Version: 0.0.7
 Summary: SPLMeter
 Author-email: Sumeet <s.saini@ufl.edu>
 Project-URL: Homepage, https://github.com/Sumeet2807/splmeter
 Project-URL: Bug Tracker, https://github.com/Sumeet2807/splmeter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `splmeter-0.0.6/pyproject.toml` & `splmeter-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "splmeter"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sumeet", email="s.saini@ufl.edu" },
 ]
 description = "SPLMeter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `splmeter-0.0.6/splmeter/base.py` & `splmeter-0.0.7/splmeter/base.py`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/splmeter/measure/frequency.py` & `splmeter-0.0.7/splmeter/measure/frequency.py`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/splmeter/measure/time.py` & `splmeter-0.0.7/splmeter/measure/time.py`

 * *Files 15% similar despite different names*

```diff
@@ -127,14 +127,71 @@
         new_sig_arr = np.max(compute_array,axis=1)
         new_signal = SoundLevel().from_signal(signal)
         new_signal.amplitude = new_sig_arr
         new_signal.fs = 1/self.output_resolution
 
         return new_signal
 
+class Lmin(BaseModule):
+    """Calculates min sound pressure level for a given signal.
+
+    """
+     
+    def init(self, compute_window, output_resolution=1, start_time=0):
+        """Init
+
+        Args:
+            compute_window (float): window size to consider for finding min
+            output_resolution (int, optional): Output will be calculated every n seconds. Defaults to 1.
+        """
+        self.compute_window = compute_window
+        self.output_resolution = output_resolution
+        self.start_time = start_time
+        self.name = 'minimum time-weighted sound level(Lmin)'
+        self.parameters['Compute window/time'] = compute_window
+        self.parameters['Output resolution'] = output_resolution
+        self.register_supported_signal_type(SoundLevel)
+
+
+    
+    def process(self,signal):
+        """Process
+
+        Args:
+            signal (SoundPressure): Sound pressure level instance to be processed
+
+
+        Returns:
+            SoundLevel: Sound level instance
+        """
+        self.output_resolution = max(self.output_resolution, 1/signal.fs)
+        input_fs = signal.fs
+        sig_arr = signal.amplitude
+        compute_window_index_size = int(input_fs*self.compute_window)
+        compute_window_step_size = int(input_fs*self.output_resolution)
+        if compute_window_step_size <= 0:
+            compute_window_step_size = 1
+        start_index = int(self.start_time*input_fs)
+        buffer = int(max(0,(compute_window_index_size - start_index)))
+        start_index += buffer
+
+        sig_arr=np.concatenate([np.array([0]*buffer),sig_arr],axis=0)
+
+        # if start_index >= sig_arr.shape[0]:
+        #     raise Exception('Not enough samples in signal for the specified sample rate, compute window & time')
+        
+    
+        indices = [np.arange(x-compute_window_index_size,x) for x in range(start_index,sig_arr.shape[0],compute_window_step_size)]
+        compute_array = np.take(sig_arr,indices)
+        new_sig_arr = np.min(compute_array,axis=1)
+        new_signal = SoundLevel().from_signal(signal)
+        new_signal.amplitude = new_sig_arr
+        new_signal.fs = 1/self.output_resolution
+
+        return new_signal
 
 class Lpeak(BaseModule):
     """Calculates peak sound pressure signal for a given signal.
 
     """
      
     def init(self, compute_window, output_resolution=1, start_time=0, max_input_fs=1000,reference_pressure = 2.0e-5):
```

### Comparing `splmeter-0.0.6/splmeter/processing/frequency.py` & `splmeter-0.0.7/splmeter/processing/frequency.py`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/splmeter/processing/time.py` & `splmeter-0.0.7/splmeter/processing/time.py`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/splmeter/visualizer.py` & `splmeter-0.0.7/splmeter/visualizer.py`

 * *Files identical despite different names*

### Comparing `splmeter-0.0.6/splmeter.egg-info/PKG-INFO` & `splmeter-0.0.7/splmeter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splmeter
-Version: 0.0.6
+Version: 0.0.7
 Summary: SPLMeter
 Author-email: Sumeet <s.saini@ufl.edu>
 Project-URL: Homepage, https://github.com/Sumeet2807/splmeter
 Project-URL: Bug Tracker, https://github.com/Sumeet2807/splmeter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

