# Comparing `tmp/dg_face_tracking-0.0.9-py3-none-any.whl.zip` & `tmp/dg_face_tracking-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,70 +1,71 @@
-Zip file size: 125960 bytes, number of entries: 68
--rw-r--r--  2.0 unx      617 b- defN 24-Apr-04 22:39 dg_face_tracking/DataFaceApp.py
--rw-r--r--  2.0 unx      210 b- defN 24-Apr-04 22:39 dg_face_tracking/__init__.py
--rw-r--r--  2.0 unx      216 b- defN 24-Apr-04 22:39 dg_face_tracking/_version.py
--rw-r--r--  2.0 unx     2615 b- defN 24-Apr-04 22:39 dg_face_tracking/config_rt.py
--rw-r--r--  2.0 unx     1931 b- defN 24-Apr-04 22:39 dg_face_tracking/embeds_compare.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-04 22:39 dg_face_tracking/embeds_estimate.py
--rw-r--r--  2.0 unx     3473 b- defN 24-Apr-04 22:39 dg_face_tracking/estimate_accuracy.py
--rw-r--r--  2.0 unx     8408 b- defN 24-Apr-04 22:39 dg_face_tracking/face_tracker_controller.py
--rw-r--r--  2.0 unx     1464 b- defN 24-Apr-04 22:39 dg_face_tracking/track_faces.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/__init__.py
--rw-r--r--  2.0 unx     1642 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/consumer.py
--rw-r--r--  2.0 unx      764 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/consumer_factory.py
--rw-r--r--  2.0 unx     4687 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/embeds_writer.py
--rw-r--r--  2.0 unx     3965 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/lancedb_writer.py
--rw-r--r--  2.0 unx     4865 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/localdb_writer.py
--rw-r--r--  2.0 unx     6353 b- defN 24-Apr-04 22:39 dg_face_tracking/Consumers/pairwise_stats.py
--rw-r--r--  2.0 unx     1368 b- defN 24-Apr-04 22:39 dg_face_tracking/Data/basedata.py
--rw-r--r--  2.0 unx     2804 b- defN 24-Apr-04 22:39 dg_face_tracking/Data/face_data.py
--rw-r--r--  2.0 unx     1656 b- defN 24-Apr-04 22:39 dg_face_tracking/Data/frame_data.py
--rw-r--r--  2.0 unx     4660 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/CameraSource.py
--rw-r--r--  2.0 unx     6933 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/DatasetSource.py
--rw-r--r--  2.0 unx    12206 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/FolderSource.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/__init__.py
--rw-r--r--  2.0 unx     5366 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/datasource.py
--rw-r--r--  2.0 unx      841 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/datasource_factory.py
--rw-r--r--  2.0 unx    24168 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/face_tracker.py
--rw-r--r--  2.0 unx    31736 b- defN 24-Apr-04 22:39 dg_face_tracking/DataSource/face_tracker_demo.py
--rw-r--r--  2.0 unx     1572 b- defN 24-Apr-04 22:39 dg_face_tracking/Database/DBAdapter.py
--rw-r--r--  2.0 unx    11902 b- defN 24-Apr-04 22:39 dg_face_tracking/Database/LocalDBAdapter.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-04 22:39 dg_face_tracking/Database/__init__.py
--rw-r--r--  2.0 unx     9561 b- defN 24-Apr-04 22:39 dg_face_tracking/Database/vectstore.py
--rw-r--r--  2.0 unx    13408 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/DataFaceDoc.py
--rw-r--r--  2.0 unx      908 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/DataFaceFrontend.py
--rw-r--r--  2.0 unx     5965 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/DataFaceView.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/__init__.py
--rw-r--r--  2.0 unx      305 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/frontend_factory.py
--rw-r--r--  2.0 unx     5194 b- defN 24-Apr-04 22:39 dg_face_tracking/Frontend/main_window.py
--rw-r--r--  2.0 unx     1583 b- defN 24-Apr-04 22:39 dg_face_tracking/Process/dg_process.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/__init__.py
--rw-r--r--  2.0 unx     4294 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/deepface_embedder.py
--rw-r--r--  2.0 unx    13784 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/face_detector.py
--rw-r--r--  2.0 unx     9165 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/face_embedder.py
--rw-r--r--  2.0 unx     7113 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/lancedb_searcher.py
--rw-r--r--  2.0 unx     5357 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/processor.py
--rw-r--r--  2.0 unx     1171 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/processor_factory.py
--rw-r--r--  2.0 unx     4267 b- defN 24-Apr-04 22:39 dg_face_tracking/Processors/tracker.py
--rw-r--r--  2.0 unx     1212 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/__init__.py
--rw-r--r--  2.0 unx    13749 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/camera_motion.py
--rw-r--r--  2.0 unx    18314 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/distances.py
--rw-r--r--  2.0 unx    10088 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/filter.py
--rw-r--r--  2.0 unx    11844 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/metrics.py
--rw-r--r--  2.0 unx    39668 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/tracker.py
--rw-r--r--  2.0 unx     3866 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/utils.py
--rw-r--r--  2.0 unx    13518 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/video.py
--rw-r--r--  2.0 unx      397 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/__init__.py
--rw-r--r--  2.0 unx     3754 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/absolute_grid.py
--rw-r--r--  2.0 unx    11207 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/color.py
--rw-r--r--  2.0 unx     7694 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/draw_boxes.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/draw_points.py
--rw-r--r--  2.0 unx    10620 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/drawer.py
--rw-r--r--  2.0 unx     6002 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/fixed_camera.py
--rw-r--r--  2.0 unx     8593 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/path.py
--rw-r--r--  2.0 unx      912 b- defN 24-Apr-04 22:39 dg_face_tracking/norfair/drawing/utils.py
--rw-r--r--  2.0 unx     5224 b- defN 24-Apr-04 22:39 dg_face_tracking-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 22:39 dg_face_tracking-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 24-Apr-04 22:39 dg_face_tracking-0.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-04 22:39 dg_face_tracking-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6542 b- defN 24-Apr-04 22:39 dg_face_tracking-0.0.9.dist-info/RECORD
-68 files, 416668 bytes uncompressed, 115310 bytes compressed:  72.3%
+Zip file size: 127138 bytes, number of entries: 69
+-rw-r--r--  2.0 unx      617 b- defN 24-Apr-17 01:56 dg_face_tracking/DataFaceApp.py
+-rw-r--r--  2.0 unx      250 b- defN 24-Apr-17 01:56 dg_face_tracking/__init__.py
+-rw-r--r--  2.0 unx      216 b- defN 24-Apr-17 01:56 dg_face_tracking/_version.py
+-rw-r--r--  2.0 unx     2615 b- defN 24-Apr-17 01:56 dg_face_tracking/config_rt.py
+-rw-r--r--  2.0 unx     1931 b- defN 24-Apr-17 01:56 dg_face_tracking/embeds_compare.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-17 01:56 dg_face_tracking/embeds_estimate.py
+-rw-r--r--  2.0 unx     3473 b- defN 24-Apr-17 01:56 dg_face_tracking/estimate_accuracy.py
+-rw-r--r--  2.0 unx     8408 b- defN 24-Apr-17 01:56 dg_face_tracking/face_tracker_controller.py
+-rw-r--r--  2.0 unx      788 b- defN 24-Apr-17 01:56 dg_face_tracking/manage_db.py
+-rw-r--r--  2.0 unx     2106 b- defN 24-Apr-17 01:56 dg_face_tracking/track_faces.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/__init__.py
+-rw-r--r--  2.0 unx     1642 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/consumer.py
+-rw-r--r--  2.0 unx      764 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/consumer_factory.py
+-rw-r--r--  2.0 unx     4687 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/embeds_writer.py
+-rw-r--r--  2.0 unx     3965 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/lancedb_writer.py
+-rw-r--r--  2.0 unx     4865 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/localdb_writer.py
+-rw-r--r--  2.0 unx     6353 b- defN 24-Apr-17 01:56 dg_face_tracking/Consumers/pairwise_stats.py
+-rw-r--r--  2.0 unx     1368 b- defN 24-Apr-17 01:56 dg_face_tracking/Data/basedata.py
+-rw-r--r--  2.0 unx     2804 b- defN 24-Apr-17 01:56 dg_face_tracking/Data/face_data.py
+-rw-r--r--  2.0 unx     1656 b- defN 24-Apr-17 01:56 dg_face_tracking/Data/frame_data.py
+-rw-r--r--  2.0 unx     4660 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/CameraSource.py
+-rw-r--r--  2.0 unx     6933 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/DatasetSource.py
+-rw-r--r--  2.0 unx    12206 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/FolderSource.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/__init__.py
+-rw-r--r--  2.0 unx     5366 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/datasource.py
+-rw-r--r--  2.0 unx      841 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/datasource_factory.py
+-rw-r--r--  2.0 unx    24168 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/face_tracker.py
+-rw-r--r--  2.0 unx    31983 b- defN 24-Apr-17 01:56 dg_face_tracking/DataSource/face_tracker_demo.py
+-rw-r--r--  2.0 unx     1572 b- defN 24-Apr-17 01:56 dg_face_tracking/Database/DBAdapter.py
+-rw-r--r--  2.0 unx    11902 b- defN 24-Apr-17 01:56 dg_face_tracking/Database/LocalDBAdapter.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-17 01:56 dg_face_tracking/Database/__init__.py
+-rw-r--r--  2.0 unx    10047 b- defN 24-Apr-17 01:56 dg_face_tracking/Database/vectstore.py
+-rw-r--r--  2.0 unx    13408 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/DataFaceDoc.py
+-rw-r--r--  2.0 unx      908 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/DataFaceFrontend.py
+-rw-r--r--  2.0 unx     5965 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/DataFaceView.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/__init__.py
+-rw-r--r--  2.0 unx      305 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/frontend_factory.py
+-rw-r--r--  2.0 unx     5194 b- defN 24-Apr-17 01:56 dg_face_tracking/Frontend/main_window.py
+-rw-r--r--  2.0 unx     1583 b- defN 24-Apr-17 01:56 dg_face_tracking/Process/dg_process.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/__init__.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/deepface_embedder.py
+-rw-r--r--  2.0 unx    13784 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/face_detector.py
+-rw-r--r--  2.0 unx     9165 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/face_embedder.py
+-rw-r--r--  2.0 unx     7113 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/lancedb_searcher.py
+-rw-r--r--  2.0 unx     5357 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/processor.py
+-rw-r--r--  2.0 unx     1171 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/processor_factory.py
+-rw-r--r--  2.0 unx     4267 b- defN 24-Apr-17 01:56 dg_face_tracking/Processors/tracker.py
+-rw-r--r--  2.0 unx     1212 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/__init__.py
+-rw-r--r--  2.0 unx    13749 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/camera_motion.py
+-rw-r--r--  2.0 unx    18314 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/distances.py
+-rw-r--r--  2.0 unx    10088 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/filter.py
+-rw-r--r--  2.0 unx    11844 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/metrics.py
+-rw-r--r--  2.0 unx    39668 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/tracker.py
+-rw-r--r--  2.0 unx     3866 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/utils.py
+-rw-r--r--  2.0 unx    13518 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/video.py
+-rw-r--r--  2.0 unx      397 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/__init__.py
+-rw-r--r--  2.0 unx     3754 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/absolute_grid.py
+-rw-r--r--  2.0 unx    11207 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/color.py
+-rw-r--r--  2.0 unx     7694 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/draw_boxes.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/draw_points.py
+-rw-r--r--  2.0 unx    10620 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/drawer.py
+-rw-r--r--  2.0 unx     6002 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/fixed_camera.py
+-rw-r--r--  2.0 unx     8593 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/path.py
+-rw-r--r--  2.0 unx      912 b- defN 24-Apr-17 01:56 dg_face_tracking/norfair/drawing/utils.py
+-rw-r--r--  2.0 unx     6100 b- defN 24-Apr-17 01:56 dg_face_tracking-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 01:56 dg_face_tracking-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 24-Apr-17 01:56 dg_face_tracking-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 01:56 dg_face_tracking-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6628 b- defN 24-Apr-17 01:56 dg_face_tracking-0.1.2.dist-info/RECORD
+69 files, 419833 bytes uncompressed, 116354 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -18,14 +18,17 @@
 
 Filename: dg_face_tracking/estimate_accuracy.py
 Comment: 
 
 Filename: dg_face_tracking/face_tracker_controller.py
 Comment: 
 
+Filename: dg_face_tracking/manage_db.py
+Comment: 
+
 Filename: dg_face_tracking/track_faces.py
 Comment: 
 
 Filename: dg_face_tracking/Consumers/__init__.py
 Comment: 
 
 Filename: dg_face_tracking/Consumers/consumer.py
@@ -183,23 +186,23 @@
 
 Filename: dg_face_tracking/norfair/drawing/path.py
 Comment: 
 
 Filename: dg_face_tracking/norfair/drawing/utils.py
 Comment: 
 
-Filename: dg_face_tracking-0.0.9.dist-info/METADATA
+Filename: dg_face_tracking-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dg_face_tracking-0.0.9.dist-info/WHEEL
+Filename: dg_face_tracking-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dg_face_tracking-0.0.9.dist-info/entry_points.txt
+Filename: dg_face_tracking-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dg_face_tracking-0.0.9.dist-info/top_level.txt
+Filename: dg_face_tracking-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dg_face_tracking-0.0.9.dist-info/RECORD
+Filename: dg_face_tracking-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dg_face_tracking/__init__.py

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 Path(__file__).resolve()
 
 from ._version import __version__, __version_info__
+
 from .track_faces import track_faces
+from .Face2ID.face2id import face2id
 
 
 def _command_entrypoint(arg_str=None):
     track_faces()
```

## dg_face_tracking/_version.py

```diff
@@ -2,9 +2,9 @@
 # _version.py: package version
 #
 # Copyright DeGirum Corporation 2024
 # All rights reserved
 #
 
 # >>> increment version here vvv
-__version_info__ = ("0", "0", "9")
+__version_info__ = ("0", "1", "2")
 __version__ = ".".join(__version_info__)
```

## dg_face_tracking/track_faces.py

```diff
@@ -1,14 +1,15 @@
 import argparse
 import os, sys
 
 from pathlib import Path
 Path(__file__).resolve()
 
 from .face_tracker_controller import FaceTrackerController
+from .manage_db import list_embeds_db, delete_entry_db
 
 
 def track_faces():
     default_deployment = "docker"
     default_config_name = ""
     default_command = ""
 
@@ -20,29 +21,46 @@
                            choices=["cloud","local", "docker"],
                            help="deployment type: cloud or local",
                            default=default_deployment)
     parser.add_argument("-e", "--exec",
                            help="execute service command",
                            choices=["delete_embeds"],
                            default=default_config_name)
+    parser.add_argument("-l", "--list",
+                           help="list entries in embeds db",
+                           action="store_true")
+    parser.add_argument("-r", "--remove",
+                           help="remove embeds db entry",
+                           default="")
+
+
     command = default_command
+    list_db = False
+    delete_entry = ""
     try:
         args = parser.parse_args()
         config_name = args.config
         deployment = args.deployment
         command = args.exec
+        list_db = args.list
+        delete_entry = args.remove
     except Exception as e:
         pass
 
-    if command == "delete_embeds":
-        if os.path.isfile("embeds.db"):
-            os.remove("embeds.db")
-
-    try:
-        ft = FaceTrackerController(deployment, config_name)
-        ft.run()
-    except:
-        print("DataFace: main: Failed to Config controller")
+    if delete_entry != "":
+        delete_entry_db("embeds.db", delete_entry)
+    elif list_db:
+        list_embeds_db("embeds.db")
+    else:
+        if command == "delete_embeds":
+            if os.path.isfile("embeds.db"):
+                os.remove("embeds.db")
+
+        try:
+            ft = FaceTrackerController(deployment, config_name)
+            ft.run()
+        except:
+            print("DataFace: main: Failed to Config controller")
 
 
 if __name__ == "__main__":
     track_faces()
```

## dg_face_tracking/DataSource/face_tracker_demo.py

```diff
@@ -549,16 +549,18 @@
     def start(self):
         self.display_thread.start()
         super(FaceTrackerDemo, self).start()
         self.start_time = time.time()
 
     def stop(self):
         """
-        Stop DataSource service
+        Stop Face Tracker Demo service
         """
+        self.vstore.dump("embeds.db")
+
         if self.video_writer is not None:
             self.video_writer.release()
         elapsed_time = time.time() - self.start_time
         fps = self.frames_processed / elapsed_time
         print("\n=========== Stopping FaceTrackerDemo ===========")
         print(f"FaceTracker Demo: {self.frames_processed} frames processed in {elapsed_time:.1f} sec ({fps:.1f} fps)")
         self.config.stop()
@@ -592,15 +594,17 @@
                     continue
                 if self.fps <= 0 or time_passed > time_lag:
                     prev_time = curr_time
                     ret, frame = self.stream.read()
                     if not ret:
                         if self.loop and self.is_file_input:
                             self.stream.set(cv2.CAP_PROP_POS_FRAMES, 0)
-                        print("Video Source: missing frame")
+                        print(f"Video Source: missing frame. Frames processed: {self.frames_processed}")
+                        self.stream.release()
+                        self.stream = None
                         self.open_video_stream(self.camera_id)
                         continue
                     self.frames_processed += 1
                     if self.frames_processed >= self.max_frames > 0:
                         raise EmptyQueue
                     if self.video_writer is not None:
                         self.video_writer.write(frame)
@@ -610,14 +614,16 @@
 
         except EmptyQueue:
             # No more data in dataset or max frames reached
             self.stop()
         finally:
             print("Video Source: finally: releasing stream")
             self.stream.release()
+            print("Video Source: finally: dumping embeds.db")
+            self.vstore.dump(self.db_path)
 
     def result_process(self):
         win_capt = "Faces"
         cv2.namedWindow(win_capt, cv2.WINDOW_NORMAL)
         while not self.is_stopped():
             result = self.result_queue.get()
             if result is None:
@@ -815,15 +821,14 @@
             # is_from_selected_track = data.get_property('selected', False)
             # if not self.track_selected or (self.track_selected and is_from_selected_track):
             if need2add: #(stored_global_id is None or (stored_global_id == global_id)):
                 # print(f"update_object_id: vstore.add object_id: {object_id},  label: {label}")
                 vstore.add(object_id, embeds, label, global_id=global_id)
                 #if stored_global_id is None:
                 vstore.add_metadata(object_id, global_id=global_id)
-                vstore.dump(self.db_path)
         else:
             # print(f"update_object_id: vstore.update object_id: {object_id},  label: {label}")
             vstore.update(object_id, label)
 
 
 def mouse_click(event, x, y,  flags, param: FaceTrackerDemo):
     if not isinstance(param, FaceTrackerDemo):
```

## dg_face_tracking/Database/vectstore.py

```diff
@@ -22,14 +22,20 @@
         self.storage = dict()     # each key defines a class, vectors are stored in a deque
         self.labels = dict()      # {class_id: label}
         self.metadata = dict()    # class' metadata
 
     def is_present(self, class_id):
         return class_id in self.storage
 
+    def num_classes(self):
+        return len(self.labels.items())
+
+    def get_class_label(self, class_id):
+        return self.labels[class_id] if class_id in self.labels else None
+
     def class_size(self, class_id):
         if not self.is_present(class_id):
             return 0
         return len(self.storage[class_id])
 
     def max_class_size(self):
         max_size = 0
@@ -73,14 +79,24 @@
 
     def size(self):
         _size = 0
         for vects in self.storage.values():
             _size += len(vects)
         return _size
 
+    def list_entries(self):
+        return [e for e in self.labels.values()]
+
+    def del_entry(self, entry):
+        for class_id, label in self.labels.items():
+            if label == entry:
+                self.delete(class_id)
+                return True
+        return False
+
     def add(self, class_id: str, vect: np.ndarray, label: str = "", **kvarg):
         if self.vect_size <= 0:
             self.vect_size = vect.size
         elif self.vect_size != vect.size:
             raise ValueError(f"VectStore: add: wrong vector size {vect.size}, should be {self.vect_size} ")
 
         if class_id not in self.storage:
@@ -117,25 +133,25 @@
     def __next__(self):
         if self.curr_class > self.end:
             raise StopIteration
         else:
             self.num += 1
             return self.num - 1
 
-    def search(self, query: np.ndarray, max_results: int = 10, **kvarg):
+    def search(self, query: np.ndarray, max_results: int = 10, min_class=3, **kvarg):
         results = deque()
         if self.vect_size <= 0:
             return results
 
         if query.size != self.vect_size:
             raise ValueError(f"VectStore: search: size of query {query.size} differs from size of stored vectors {self.vect_size}")
         min_heap = []   # heap of (1-score, class_id) tuples
 
         for class_id in self.storage:
-            if len(self.storage[class_id]) < 3:
+            if len(self.storage[class_id]) < min_class:
                 continue
             for data in self.storage[class_id]:
                 vect = data['vect']
                 score = vect @ query
                 if len(min_heap) < max_results:
                     heapq.heappush(min_heap, (score, class_id))
                 else:
```

## Comparing `dg_face_tracking-0.0.9.dist-info/METADATA` & `dg_face_tracking-0.1.2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dg_face_tracking
-Version: 0.0.9
+Version: 0.1.2
 Summary: DeGirum Face Tracking Application Package
 Home-page: https://github.com/degirum
 Author: DeGirum Corp.
 Author-email: support@degirum.com
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -99,15 +99,42 @@
 - Set the valid paths for catalogue (`catalogue_path`) and the datasets path (`datasets_path`);
 - Set the dataset name (`dataset_name`)
 
 Run the application.
 
 To stop running, press Ctrl+C
 
-## 5. CI/CD
+## 5. Face to ID functionality
+
+To label a cropped face image: import `face2id` function
+   ```
+   from dg_face_tracking.Face2ID.face2id import face2id
+   ```
+Interface:
+   ```
+   def face2id(img: Union[str, np.ndarray],
+            deployment: str = "docker",
+            async_support: bool = False,
+            verbose: bool = False) -> str:
+   ```
+Parameters:
+   ```
+    img : str or ndarray: face image as base64 encoded png or numpy array
+    deployment: ["cloud", "local", "docker"]
+    async_support: bool: do we need to enable async support
+    verbose: bool: for testing purpose only
+   ```
+Return value: json string
+   ```
+    {"label": "<some label or empty string>", "error": "<error message or empty string>"}
+   ```
+Label can be a name of a person, `unknown` or empty (in case of internal error)
+Error is empty string on success or contains some error message
+
+## 6. CI/CD
 
 To make new release perform the following steps:
 
 1. Assign new git tag by running the following command:
 
     ```
     ./rel-tag.sh x.y.z
```

## Comparing `dg_face_tracking-0.0.9.dist-info/RECORD` & `dg_face_tracking-0.1.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 dg_face_tracking/DataFaceApp.py,sha256=v4w12XC8tXZcHT9L_A93ceXCIf8h0clWDBZ10Jzd21Y,617
-dg_face_tracking/__init__.py,sha256=SWFsMrfNzomLor10-IgGeaE5V6fXMmSBegpH9Y0KY7I,210
-dg_face_tracking/_version.py,sha256=BvtWtDVTe5Q27TM_k7yaESLnLOilqLNaM_i3OVpSeIA,216
+dg_face_tracking/__init__.py,sha256=UMPv5K1ux02Qfzj2eqxDhnnFMgULfRPCDKxXBtzIbU4,250
+dg_face_tracking/_version.py,sha256=L7KiKmCBvQHgqN8XPF4ICggj-L6f2m-jIAktRbt53gQ,216
 dg_face_tracking/config_rt.py,sha256=uoh8Xf7N_y7Lg5gXhYPO-Msk0x54lXvkVRvBYB3qRME,2615
 dg_face_tracking/embeds_compare.py,sha256=ZdpoURTW9YlP8g0vFp7VB4C0gcunY-XFC2YoP9DCJ8o,1931
 dg_face_tracking/embeds_estimate.py,sha256=FRqmQsZTfm80kusa3HtjS1H3POK3q2pGXpdvi-Es42k,2579
 dg_face_tracking/estimate_accuracy.py,sha256=wSKDra0b8Ticmb_vLAtsheyknfBbnC1QOAoJJEqQU_Y,3473
 dg_face_tracking/face_tracker_controller.py,sha256=xmUqMdweNZkso3E8kLAxPGFiM7OzMa8ooR82rMqoBKA,8408
-dg_face_tracking/track_faces.py,sha256=tYhNK3w3oe06q_grNHitJFvWI8eWX6ClandelYOQ7Jo,1464
+dg_face_tracking/manage_db.py,sha256=CnjxG5CGysls6BB09TDia_BLpDQn8rSY0wKG-TDrK5Q,788
+dg_face_tracking/track_faces.py,sha256=lBKAKi-iZMfvskNlvJbbu3ChKXRe4q60FP1sXfWh6bo,2106
 dg_face_tracking/Consumers/__init__.py,sha256=ipTDkSDa3WQ4jgaDW3vOPTFVoGg64wDCpgw85hVUYJc,50
 dg_face_tracking/Consumers/consumer.py,sha256=qkaHcMMfNbKraTkvhvg8bCgryiWEdA-eM7xmSN_l-6g,1642
 dg_face_tracking/Consumers/consumer_factory.py,sha256=maekqM_-p7Pi3A7O-WrctsR_296oQj69ptPWDIzwvyk,764
 dg_face_tracking/Consumers/embeds_writer.py,sha256=jAm2Tx230AE30pmrfCnICoUZKHAGdEWoGdpfrWJ6b8k,4687
 dg_face_tracking/Consumers/lancedb_writer.py,sha256=2eCLYreHCu_U46OywKJp2lKS62seBpY3ia2cCGk-qhg,3965
 dg_face_tracking/Consumers/localdb_writer.py,sha256=RkuTEROlkmo5LwwjyJP5vgXvjb6XxPP2BSq4L8NNux8,4865
 dg_face_tracking/Consumers/pairwise_stats.py,sha256=hclyMemSHeh2nf8U9R9CStE2P2aXH1wkK-nfNoIHnwo,6353
@@ -20,19 +21,19 @@
 dg_face_tracking/DataSource/CameraSource.py,sha256=_eaYqJtf53WsRPkIHrzBwmPgV9y64KJgOOPbS-ylX2I,4660
 dg_face_tracking/DataSource/DatasetSource.py,sha256=yHXOgSxC6RVZ0Ad_H49xb3pg9hketVea7Rrc5sKc8Es,6933
 dg_face_tracking/DataSource/FolderSource.py,sha256=FuQ16DTMYqJUxTrLmr9CprNEZkukQO9oZPpgptHLG4M,12206
 dg_face_tracking/DataSource/__init__.py,sha256=ipTDkSDa3WQ4jgaDW3vOPTFVoGg64wDCpgw85hVUYJc,50
 dg_face_tracking/DataSource/datasource.py,sha256=SUQIE8tsEZ2L00xrKJ3ym1FM_m5u8q_GIu2wXk4P45M,5366
 dg_face_tracking/DataSource/datasource_factory.py,sha256=5uv-5YN3qbkEUb5pZ9XcNLk1AGzLp3YOtULadWaVY7k,841
 dg_face_tracking/DataSource/face_tracker.py,sha256=uYMyaoDxtv4YbFDA4NpzhK7332HIUR1gYN7r-2CqWs4,24168
-dg_face_tracking/DataSource/face_tracker_demo.py,sha256=EpKSxz6YvRAau11tASKjOnBSeLFQfxJvdULPxGyBUW4,31736
+dg_face_tracking/DataSource/face_tracker_demo.py,sha256=4tnc6pwz3r0xWbBuwNzNKqTQ-v6WS7wA1K4pHZ1CMMM,31983
 dg_face_tracking/Database/DBAdapter.py,sha256=eh8PGvV_J-rn0S5VWKUpvY0nAbH-p1b_Zm_kOpQ2hh4,1572
 dg_face_tracking/Database/LocalDBAdapter.py,sha256=op37_5yYYWVdpgN0WLcTq65VBy1hOdIGL6adarAzzNY,11902
 dg_face_tracking/Database/__init__.py,sha256=ipTDkSDa3WQ4jgaDW3vOPTFVoGg64wDCpgw85hVUYJc,50
-dg_face_tracking/Database/vectstore.py,sha256=7xCUuwEEbcljW53tmDyp-7YxUZ3cpw6BMu8rbs8TEGY,9561
+dg_face_tracking/Database/vectstore.py,sha256=LfaU7lOQ5wcV_TwIbwqBtzFiJzcFz23Y_as42mqPw9k,10047
 dg_face_tracking/Frontend/DataFaceDoc.py,sha256=pc5EuCJUC9dd6h0PS4iuXYxoGZH1LCszW73AiIE_dXw,13408
 dg_face_tracking/Frontend/DataFaceFrontend.py,sha256=TuTuH4-MR5Nmui3zNNuZwZnMdtK5Y6-x5vStQd-F3dw,908
 dg_face_tracking/Frontend/DataFaceView.py,sha256=QvnvgNkCiIvcOiFVRTO1NKN7JKRw---6fFVNcECfW9Q,5965
 dg_face_tracking/Frontend/__init__.py,sha256=ipTDkSDa3WQ4jgaDW3vOPTFVoGg64wDCpgw85hVUYJc,50
 dg_face_tracking/Frontend/frontend_factory.py,sha256=huoIZDgh4F42JZHKCDgscN31XS98h0-gs6atqH_tACY,305
 dg_face_tracking/Frontend/main_window.py,sha256=awGVtCIr3iyjyPjymeUEx0wNKl1Lwz9pq50YIbst5Bc,5194
 dg_face_tracking/Process/dg_process.py,sha256=xWARtSO2vZAbY26iWzTyrizsAyMhGprjFz-uR9ojmA4,1583
@@ -57,12 +58,12 @@
 dg_face_tracking/norfair/drawing/color.py,sha256=KIptTABXZ9X3-CHBi7O6dl46-8P9fSWUGIEIrfJfBT8,11207
 dg_face_tracking/norfair/drawing/draw_boxes.py,sha256=xdRiEGnOX4oxn1QOi956RKfOcoOKS2Na8PXLAgQ2FzA,7694
 dg_face_tracking/norfair/drawing/draw_points.py,sha256=gB5Dm4Eht-MAJRRqk0fGOoCNO28x6fHZyehPungMguc,11955
 dg_face_tracking/norfair/drawing/drawer.py,sha256=v0Ccce0OiWvUw04HKNpeyK7Rru1JjXiJlcB4PH4U7Wo,10620
 dg_face_tracking/norfair/drawing/fixed_camera.py,sha256=KAJCWYgym986hbzCBnr7kKa3A0qVYmTBoaL4LLq4O6E,6002
 dg_face_tracking/norfair/drawing/path.py,sha256=rA5EnnD_9Wj0OYv4h3-ccxn_VRrQqaNt8eFLAJXQc0k,8593
 dg_face_tracking/norfair/drawing/utils.py,sha256=g-mcTdpbfBQ1s-3Wy6CgfkCbImh1RGr3L7QZy2LjT10,912
-dg_face_tracking-0.0.9.dist-info/METADATA,sha256=W9W4bZXAylGrfLEYRefJkhmbcqLhuWn897rsU-cC-FA,5224
-dg_face_tracking-0.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dg_face_tracking-0.0.9.dist-info/entry_points.txt,sha256=ovgHU9wCkHRnHpdbwJosT_GZGHaoSIA6qUvn6gk_88U,74
-dg_face_tracking-0.0.9.dist-info/top_level.txt,sha256=a-hi1DQ_XruLP9Xm7BYdiR_88Vf2hlg9WabZkO1qJKQ,17
-dg_face_tracking-0.0.9.dist-info/RECORD,,
+dg_face_tracking-0.1.2.dist-info/METADATA,sha256=RIX6QeaOEG1yeGJ6-w8KyHXwLO352rqPNOpIanuzmao,6100
+dg_face_tracking-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dg_face_tracking-0.1.2.dist-info/entry_points.txt,sha256=ovgHU9wCkHRnHpdbwJosT_GZGHaoSIA6qUvn6gk_88U,74
+dg_face_tracking-0.1.2.dist-info/top_level.txt,sha256=a-hi1DQ_XruLP9Xm7BYdiR_88Vf2hlg9WabZkO1qJKQ,17
+dg_face_tracking-0.1.2.dist-info/RECORD,,
```

