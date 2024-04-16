# Comparing `tmp/gama_config-2.2.0.tar.gz` & `tmp/gama_config-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_config-2.2.0.tar", last modified: Wed Apr 10 12:27:42 2024, max compression
+gzip compressed data, was "gama_config-2.3.0.tar", last modified: Tue Apr 16 22:04:42 2024, max compression
```

## Comparing `gama_config-2.2.0.tar` & `gama_config-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.296596 gama_config-2.2.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-10 12:27:42.292596 gama_config-2.2.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      957 2024-04-10 12:26:35.000000 gama_config-2.2.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)      147 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2134 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2681 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/gama_vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    15464 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_cameras.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      655 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3732 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_urdf.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1476 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1720 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/schemas/gama_gs.schema.json
--rw-rw-r--   0 runner    (1000) runner    (1001)     7598 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/schemas/gama_vessel.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)      314 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/helpers.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_generate_urdf.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1885 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_read_gama_gs_config.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4800 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_read_gama_vessel_config.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      667 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:26.000000 gama_config-2.2.0/gama_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      902 2024-04-10 12:27:42.296596 gama_config-2.2.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 12:26:35.000000 gama_config-2.2.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:42.961054 gama_config-2.3.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-16 22:04:42.961054 gama_config-2.3.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      957 2024-04-16 22:03:46.000000 gama_config-2.3.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:42.961054 gama_config-2.3.0/gama_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      147 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2176 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2706 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/gama_vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    15473 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/generate_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      655 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3724 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/generate_urdf.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1476 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:42.961054 gama_config-2.3.0/gama_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1769 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/schemas/gama_gs.schema.json
+-rw-rw-r--   0 runner    (1000) runner    (1001)     8357 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/schemas/gama_vessel.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:42.961054 gama_config-2.3.0/gama_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      314 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/test/helpers.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/test/test_generate_urdf.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1885 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/test/test_read_gama_gs_config.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4800 2024-04-16 22:03:46.000000 gama_config-2.3.0/gama_config/test/test_read_gama_vessel_config.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:42.961054 gama_config-2.3.0/gama_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-16 22:04:42.000000 gama_config-2.3.0/gama_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      667 2024-04-16 22:04:42.000000 gama_config-2.3.0/gama_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-16 22:04:42.000000 gama_config-2.3.0/gama_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-16 22:04:42.000000 gama_config-2.3.0/gama_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-16 22:04:42.000000 gama_config-2.3.0/gama_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-16 22:04:25.000000 gama_config-2.3.0/gama_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      902 2024-04-16 22:04:42.961054 gama_config-2.3.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-16 22:03:46.000000 gama_config-2.3.0/setup.py
```

### Comparing `gama_config-2.2.0/PKG-INFO` & `gama_config-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_config
-Version: 2.2.0
+Version: 2.3.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: dacite
 Requires-Dist: PyYAML
 Requires-Dist: dc-schema
-Requires-Dist: greenstream-config==2.12.0
+Requires-Dist: greenstream-config==2.13.3
 Requires-Dist: gr-urchin
 
 # GAMA Config
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
```

### Comparing `gama_config-2.2.0/README.md` & `gama_config-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/gama_config/gama_gs.py` & `gama_config-2.3.0/gama_config/gama_gs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     THRUSTMASTER_COMBO = "thrustmaster_combo"
     WARTHOG = "warthog"
     WARTHOG_COMBO = "warthog_combo"
     AERONAV = "aeronav"
     SINGLE_UNKNOWN = "single_unknown"
     DUAL_UNKNOWN = "dual_unknown"
     GLADIATOR = "gladiator"
+    LOGITECH_EXTREME = "logitech_extreme"
 
 
 class Network(str, Enum):
     SHARED = "shared"
     HOST = "host"
```

### Comparing `gama_config-2.2.0/gama_config/gama_vessel.py` & `gama_config-2.3.0/gama_config/gama_vessel.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     prod: bool = False
     log_level: LogLevel = LogLevel.INFO
     ubiquity_user: Optional[str] = None
     ubiquity_pass: Optional[str] = None
     ubiquity_ip: Optional[str] = None
     static_peers: Optional[str] = None
     camera_overrides: Optional[List[Optional[CameraOverride]]] = None
+    record: bool = False
 
 
 def parse_vessel_config(config: dict[str, Any]) -> GamaVesselConfig:
     return from_dict(
         GamaVesselConfig,
         config,
         config=Config(cast=[Mode, Network, Variant, LogLevel]),
```

### Comparing `gama_config-2.2.0/gama_config/generate_cameras.py` & `gama_config-2.3.0/gama_config/generate_cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             fov=125.0,
             camera_frame_topic=None,
             camera_info_topic="sensors/cameras/bow_color/camera_info",
             camera_info_ext_topic="sensors/cameras/bow_color/camera_info_ext",
             k_intrinsic=k_intrinsic,
             # distortion_parameters=distortion_parameters,
             offsets=Offsets(
-                roll=0.0,
-                pitch=radians(20.0),
+                roll=radians(2.0),
+                pitch=radians(5.85),
                 yaw=0.0,
                 forward=3.190,
                 left=0.015,
                 up=-0.205,
             ),
         ),
         Camera(
```

### Comparing `gama_config-2.2.0/gama_config/generate_schemas.py` & `gama_config-2.3.0/gama_config/generate_schemas.py`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/gama_config/generate_urdf.py` & `gama_config-2.3.0/gama_config/generate_urdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         )
         urdf._joints.append(
             Joint(
                 name="baselink_to_radar",
                 parent="base_link",
                 child="radar",
                 joint_type="fixed",
-                origin=xyz_rpy_to_matrix([0.0, 0.0, radar_height, 0.0, 0.0, radians(-3)]),
+                origin=xyz_rpy_to_matrix([0.0, 0.0, radar_height, 0.0, 0.0, 0.0]),
             )
         )
 
     urdf.save(file_path)
 
     # stringify urdf response for robot description
     with open(file_path) as infp:
```

### Comparing `gama_config-2.2.0/gama_config/helpers.py` & `gama_config-2.3.0/gama_config/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/gama_config/schemas/gama_gs.schema.json` & `gama_config-2.3.0/gama_config/schemas/gama_gs.schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'$defs'": "{'Mode': {'enum': {insert: [(9, 'gladiator'), (10, 'logitech_extreme')]}}}"}*

```diff
@@ -16,15 +16,17 @@
                 "xbox",
                 "thrustmaster",
                 "thrustmaster_combo",
                 "warthog",
                 "warthog_combo",
                 "aeronav",
                 "single_unknown",
-                "dual_unknown"
+                "dual_unknown",
+                "gladiator",
+                "logitech_extreme"
             ],
             "title": "Mode"
         },
         "Network": {
             "enum": [
                 "shared",
                 "host"
```

### Comparing `gama_config-2.2.0/gama_config/schemas/gama_vessel.schema.json` & `gama_config-2.3.0/gama_config/schemas/gama_vessel.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924962144945699%*

 * *Differences: {"'$defs'": "{'CameraOverride': {'properties': {'k_intrinsic': OrderedDict([('anyOf', "*

 * *            "[OrderedDict([('type', 'array'), ('items', OrderedDict([('type', 'number')]))]), "*

 * *            "OrderedDict([('type', 'null')])]), ('default', None)]), 'distortion_parameters': "*

 * *            "OrderedDict([('anyOf', [OrderedDict([('type', 'array'), ('items', "*

 * *            "OrderedDict([('type', 'number')]))]), OrderedDict([('type', 'null')])]), ('default', "*

 * *            "None)]), 'distortion_model': OrderedDi […]*

```diff
@@ -28,46 +28,68 @@
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
+                "distortion_model": {
+                    "default": "plumb_bob",
+                    "type": "string"
+                },
+                "distortion_parameters": {
+                    "anyOf": [
+                        {
+                            "items": {
+                                "type": "number"
+                            },
+                            "type": "array"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null
+                },
                 "elements": {
                     "anyOf": [
                         {
                             "items": {
                                 "type": "string"
                             },
                             "type": "array"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "focal_length_mm": {
+                "fov": {
                     "anyOf": [
                         {
                             "type": "number"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
-                "fov": {
+                "k_intrinsic": {
                     "anyOf": [
                         {
-                            "type": "number"
+                            "items": {
+                                "type": "number"
+                            },
+                            "type": "array"
                         },
                         {
                             "type": "null"
                         }
-                    ]
+                    ],
+                    "default": null
                 },
                 "name": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
@@ -157,25 +179,35 @@
                             "type": "string"
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": "color"
+                },
+                "undistort_image": {
+                    "anyOf": [
+                        {
+                            "type": "boolean"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": false
                 }
             },
             "required": [
                 "name",
                 "order",
                 "elements",
                 "pixel_width",
                 "pixel_height",
                 "sensor_width_mm",
                 "sensor_height_mm",
-                "focal_length_mm",
                 "fov",
                 "camera_frame_topic",
                 "camera_info_topic",
                 "camera_info_ext_topic"
             ],
             "title": "CameraOverride",
             "type": "object"
@@ -348,14 +380,18 @@
             ],
             "default": "shared"
         },
         "prod": {
             "default": false,
             "type": "boolean"
         },
+        "record": {
+            "default": false,
+            "type": "boolean"
+        },
         "ros_domain_id": {
             "default": 0,
             "type": "integer"
         },
         "static_peers": {
             "anyOf": [
                 {
```

### Comparing `gama_config-2.2.0/gama_config/test/test_read_gama_gs_config.py` & `gama_config-2.3.0/gama_config/test/test_read_gama_gs_config.py`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/gama_config/test/test_read_gama_vessel_config.py` & `gama_config-2.3.0/gama_config/test/test_read_gama_vessel_config.py`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/gama_config.egg-info/PKG-INFO` & `gama_config-2.3.0/gama_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_config
-Version: 2.2.0
+Version: 2.3.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: dacite
 Requires-Dist: PyYAML
 Requires-Dist: dc-schema
-Requires-Dist: greenstream-config==2.12.0
+Requires-Dist: greenstream-config==2.13.3
 Requires-Dist: gr-urchin
 
 # GAMA Config
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
```

### Comparing `gama_config-2.2.0/gama_config.egg-info/SOURCES.txt` & `gama_config-2.3.0/gama_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gama_config-2.2.0/setup.cfg` & `gama_config-2.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_config
-version = 2.2.0
+version = 2.3.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 [options]
 packages = find:
 install_requires = 
 	setuptools
 	dacite
 	PyYAML
 	dc-schema
-	greenstream-config==2.12.0
+	greenstream-config==2.13.3
 	gr-urchin
 zip_safe = true
 
 [options.package_data]
 gama_config = 
 	**/*.json
 	**/*.py
```

