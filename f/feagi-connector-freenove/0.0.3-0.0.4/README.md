# Comparing `tmp/feagi_connector_freenove-0.0.3.tar.gz` & `tmp/feagi_connector_freenove-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector_freenove-0.0.3.tar", last modified: Tue Apr  9 20:34:34 2024, max compression
+gzip compressed data, was "feagi_connector_freenove-0.0.4.tar", last modified: Wed Apr 17 16:43:06 2024, max compression
```

## Comparing `feagi_connector_freenove-0.0.3.tar` & `feagi_connector_freenove-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:34:34.622863 feagi_connector_freenove-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 20:34:34.622863 feagi_connector_freenove-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:34:34.622863 feagi_connector_freenove-0.0.3/feagi_connector_freenove/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2332 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/ADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/Led.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2619 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/PCA9685.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/configuration.json
--rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/verify.sh
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:34:34.622863 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 20:34:34.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 20:34:34.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:34:34.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 20:34:34.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 20:34:34.000000 feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 20:34:22.000000 feagi_connector_freenove-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 20:34:34.626863 feagi_connector_freenove-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:43:06.714961 feagi_connector_freenove-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-17 16:43:06.714961 feagi_connector_freenove-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:43:06.714961 feagi_connector_freenove-0.0.4/feagi_connector_freenove/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2332 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/ADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/Led.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2619 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/PCA9685.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/configuration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25158 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/verify.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:43:06.714961 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-17 16:43:06.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 16:43:06.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:43:06.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 16:43:06.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 16:43:06.000000 feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 16:42:54.000000 feagi_connector_freenove-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-17 16:43:06.718961 feagi_connector_freenove-0.0.4/setup.cfg
```

### Comparing `feagi_connector_freenove-0.0.3/LICENSE` & `feagi_connector_freenove-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/PKG-INFO` & `feagi_connector_freenove-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector_freenove
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville INC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector_freenove-0.0.3/README.md` & `feagi_connector_freenove-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/ADC.py` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/ADC.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/Led.py` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/Led.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/PCA9685.py` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/PCA9685.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/__main__.py` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/__main__.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/configuration.json` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/configuration.json`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/controller.py` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,15 @@
             message_from_feagi = pns.message_from_feagi
             if message_from_feagi and message_from_feagi != None:
                 # Fetch data such as motor, servo, etc and pass to a function (you make ur own action.
                 obtained_signals = pns.obtain_opu_data(message_from_feagi)
                 action(obtained_signals, led_tracking_list, feagi_settings, capabilities,
                        rolling_window, motor, servo, led, runtime_data)
 
-            if raw_frame_internal['0'] != []:
+            if raw_frame_internal['0'] is not []:
                 raw_frame = raw_frame_internal['0']
                 if len(default_capabilities['camera']['blink']) > 0:
                     raw_frame = default_capabilities['camera']['blink']
                 # Post image into vision
                 previous_frame_data, rgb, default_capabilities = \
                     retina.process_visual_stimuli(raw_frame, default_capabilities,
                                                   previous_frame_data,
```

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/setup.sh` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/setup.sh`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove/verify.sh` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove/verify.sh`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/PKG-INFO` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector_freenove
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville INC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector_freenove-0.0.3/feagi_connector_freenove.egg-info/SOURCES.txt` & `feagi_connector_freenove-0.0.4/feagi_connector_freenove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.3/setup.cfg` & `feagi_connector_freenove-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector_freenove
-version = 0.0.3
+version = 0.0.4
 author = Neuraville INC
 author_email = info@feagi.org
 description = Feagi agent freenove to connect feagi with your freenove_smartcar.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```

