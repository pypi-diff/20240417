# Comparing `tmp/feagi_connector-0.0.4.tar.gz` & `tmp/feagi_connector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector-0.0.4.tar", last modified: Tue Apr  9 17:16:10 2024, max compression
+gzip compressed data, was "feagi_connector-0.0.5.tar", last modified: Wed Apr 17 16:41:53 2024, max compression
```

## Comparing `feagi_connector-0.0.4.tar` & `feagi_connector-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/PIL_retina.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/feagi_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/pns_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/retina.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector/sensorimotor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/sensorimotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/testing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 17:16:00.000000 feagi_connector-0.0.4/feagi_connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.629633 feagi_connector-0.0.5/feagi_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/PIL_retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/feagi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/pns_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.629633 feagi_connector-0.0.5/feagi_connector/sensorimotor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/sensorimotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/testing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 16:41:44.000000 feagi_connector-0.0.5/feagi_connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/feagi_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/setup.cfg
```

### Comparing `feagi_connector-0.0.4/LICENSE` & `feagi_connector-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/PKG-INFO` & `feagi_connector-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.4/README.md` & `feagi_connector-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/PIL_retina.py` & `feagi_connector-0.0.5/feagi_connector/PIL_retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/actuators.py` & `feagi_connector-0.0.5/feagi_connector/actuators.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/configuration.py` & `feagi_connector-0.0.5/feagi_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/feagi_interface.py` & `feagi_connector-0.0.5/feagi_connector/feagi_interface.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/pns_gateway.py` & `feagi_connector-0.0.5/feagi_connector/pns_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,20 +165,20 @@
 def gaze_control_update(message_from_feagi, capabilities):
     """
     Update the gaze from the gaze opu cortical area
     """
     if 'o__gaz' in message_from_feagi["opu_data"]:
         for data_point in message_from_feagi["opu_data"]['o__gaz']:
             device_id = data_point.split('-')[0]
-            if int(device_id) in [0, 1]:
+            if str(device_id) in ['0', '1']:
                 feagi_aptr = (int(data_point.split('-')[-1]))
                 aptr_cortical_size = full_list_dimension['o__gaz']['cortical_dimensions'][2] - 1
                 max_range = capabilities['camera']['vision_range'][1]
                 min_range = capabilities['camera']['vision_range'][0]
-                capabilities['camera']["gaze_control"][int(device_id)] = int(
+                capabilities['camera']["gaze_control"][str(device_id)] = int(
                     ((feagi_aptr / aptr_cortical_size) * (max_range - min_range)) + min_range)
             # Comment new method out
             # processed_data_point = feagi.block_to_array(data_point)
             # device_id = processed_data_point[0]
             # device_power = message_from_feagi["opu_data"]['o__gaz'][data_point]
             # if device_power == 100:
             #     device_power -= 1
@@ -189,20 +189,20 @@
 def pupil_control_update(message_from_feagi, capabilities):
     """
     Update pupil size from the pupil opu cortical area
     """
     if 'o__pup' in message_from_feagi["opu_data"]:
         for data_point in message_from_feagi["opu_data"]['o__pup']:
             device_id = data_point.split('-')[0]
-            if int(device_id) in [0, 1]:
+            if str(device_id) in ['0', '1']:
                 feagi_aptr = (int(data_point.split('-')[-1]))
                 aptr_cortical_size = full_list_dimension['o__pup']['cortical_dimensions'][2] - 1
                 max_range = capabilities['camera']['vision_range'][1]
                 min_range = capabilities['camera']['vision_range'][0]
-                capabilities['camera']["pupil_control"][int(device_id)] = int(((feagi_aptr /
+                capabilities['camera']["pupil_control"][str(device_id)] = int(((feagi_aptr /
                                                                                 aptr_cortical_size) * (
                                                                                        max_range - min_range)) + min_range)
         # comment new method out
         # for data_point in message_from_feagi["opu_data"]['o__pup']:
         #     processed_data_point = feagi.block_to_array(data_point)
         #     device_id = processed_data_point[0]
         #     device_power = message_from_feagi["opu_data"]['o__pup'][data_point]
```

### Comparing `feagi_connector-0.0.4/feagi_connector/retina.py` & `feagi_connector-0.0.5/feagi_connector/retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/router.py` & `feagi_connector-0.0.5/feagi_connector/router.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/sensors.py` & `feagi_connector-0.0.5/feagi_connector/sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,7 +53,17 @@
 
 def add_sound_to_feagi_data(hear_list, message_to_feagi):
     return pns.append_sensory_data_for_feagi('hearing', hear_list, message_to_feagi)
 
 
 def add_generic_input_to_feagi_data(generic_list, message_to_feaggi):
     return pns.append_sensory_data_for_feagi('generic_ipu', generic_list, message_to_feaggi)
+
+
+def add_agent_status(status, message_to_feagi, agent_settings):
+    if "data" not in message_to_feagi:
+        message_to_feagi["data"] = {}
+    if status:
+        message_to_feagi["data"]['connected_agents'] = [agent_settings['agent_id']]
+    else:
+        message_to_feagi["data"]['connected_agents'] = []
+    return message_to_feagi
```

### Comparing `feagi_connector-0.0.4/feagi_connector/testing_mode.py` & `feagi_connector-0.0.5/feagi_connector/testing_mode.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector/trainer.py` & `feagi_connector-0.0.5/feagi_connector/trainer.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/feagi_connector.egg-info/PKG-INFO` & `feagi_connector-0.0.5/feagi_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.4/feagi_connector.egg-info/SOURCES.txt` & `feagi_connector-0.0.5/feagi_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.4/setup.cfg` & `feagi_connector-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector
-version = 0.0.4
+version = 0.0.5
 author = Neuraville Inc.
 author_email = info@feagi.org
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi-connector
 project_urls =
```

