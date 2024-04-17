# Comparing `tmp/ehdg_pupil_detector-3.1.1.tar.gz` & `tmp/ehdg_pupil_detector-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.1.1.tar", last modified: Tue Apr 16 01:16:31 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.1.2.tar", last modified: Tue Apr 16 04:43:35 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.1.1.tar` & `ehdg_pupil_detector-3.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.947422 ehdg_pupil_detector-3.1.1/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.1/LICENSE
--rw-rw-rw-   0        0        0     4068 2024-04-16 01:16:31.946426 ehdg_pupil_detector-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.1/README.md
--rw-rw-rw-   0        0        0     1148 2024-04-16 01:15:36.000000 ehdg_pupil_detector-3.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 01:16:31.947422 ehdg_pupil_detector-3.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.916506 ehdg_pupil_detector-3.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.923486 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    11990 2024-04-16 01:15:13.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opmtrack.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.944431 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4068 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.868942 ehdg_pupil_detector-3.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4068 2024-04-16 04:43:35.867945 ehdg_pupil_detector-3.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.2/README.md
+-rw-rw-rw-   0        0        0     1148 2024-04-16 04:32:50.000000 ehdg_pupil_detector-3.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 04:43:35.868942 ehdg_pupil_detector-3.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.833538 ehdg_pupil_detector-3.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.841500 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    12338 2024-04-16 04:37:00.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opmtrack.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.865949 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4068 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.1.1/LICENSE` & `ehdg_pupil_detector-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.1/PKG-INFO` & `ehdg_pupil_detector-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.1.1/README.md` & `ehdg_pupil_detector-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.1/pyproject.toml` & `ehdg_pupil_detector-3.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.1.1"
+version = "3.1.2"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,18 +49,15 @@
     temp_dict["ellipse_axis_b"] = ellipse_axis_b
     temp_dict["ellipse_angle"] = ellipse_angle
 
     return temp_dict
 
 
 # This function is to redetect with pupil detector by given detector and tiny fill buffer
-def opm_detect(trial_video, out_dir, config_dict, buffer_length_input, direction_input=None):
-    out_folder = os.path.join(out_dir, "opmtrack_result")
-    if not os.path.isdir(out_folder):
-        os.mkdir(out_folder)
+def opm_detect(trial_video, out_folder, config_dict, buffer_length_input, direction_input=None):
     out_csv_dir = os.path.join(out_folder, "result.csv")
     out_video_dir = os.path.join(out_folder, "result.mp4")
 
     detector = ehdg_pupil_detector.Detector()
     buffer = TinyFillBuffer(buffer_length_input)
     detector.update_config(config_dict)
     updated_properties = detector.get_config_info()
@@ -153,63 +150,72 @@
                     if not got_first_data:
                         got_first_data = True
                     else:
                         temp_dict = get_data_dict(return_data, frame_rate, frame_width, frame_height, direction_input)
                         csv_writer.writerow(temp_dict)
                 destination_file.close()
                 v_writer.release()
-                print(f"The opmtrack_result folder is created in {out_dir}.")
                 print(f"Result folder dir: {out_folder}.")
                 print(f"Result csv dir: {out_csv_dir}.")
                 print(f"Result video dir: {out_video_dir}.")
                 break
 
 
 def main():
     parser = argparse.ArgumentParser(prog='opmtrack',
                                      description='OKNTRACK package.')
     opmtrack_version = importlib.metadata.version('ehdg_pupil_detector')
     parser.add_argument('--version', action='version', version=opmtrack_version),
     parser.add_argument("-i", dest="input_video", required=False, default=None,
                         metavar="input video")
-    parser.add_argument("-o", dest="output_directory", required=False, default=None,
-                        metavar="output directory")
+    parser.add_argument("-o", dest="output_folder", required=False, default=None,
+                        metavar="output folder")
     parser.add_argument("-c", dest="opm_config", required=False, default=None,
                         metavar="opm detector config")
     parser.add_argument("-d", dest="direction_input", required=False, default=None,
                         metavar="direction input")
     parser.add_argument("-bl", dest="buffer_length", required=False, default=None,
                         metavar="buffer length")
 
     args = parser.parse_args()
     input_video = args.input_video
-    output_directory = args.output_directory
+    output_folder = args.output_folder
     opm_config = args.opm_config
     direction_input = args.direction_input
     buffer_length = args.buffer_length
 
     default_buffer_length = 7
 
     if not os.path.isfile(input_video):
         print(f"Input video is invalid.")
         print(f"Input video: {input_video} is invalid.")
         return
 
+    input_video_name = os.path.basename(input_video)
+    output_directory = str(input_video).replace(input_video_name, str(output_folder))
     if os.path.isfile(output_directory):
         print(f"Output directory must be directory not file.")
         print(f"Output directory: {output_directory}.")
         return
     else:
         if not os.path.isdir(output_directory):
             try:
                 os.mkdir(output_directory)
+                print(f"Output directory is created.")
+                print(f"Output directory: {output_directory}.")
             except FileNotFoundError:
                 print(f"Output directory cannot be created.")
                 print(f"Output directory: {output_directory}.")
                 return
+            except OSError:
+                print(f"Output directory cannot be created.")
+                print(f"Output directory: {output_directory}.")
+                print(f"Invalid output folder input.")
+                print(f"Output folder input: {output_folder}.")
+                return
 
     if opm_config is None:
         opm_config = get_config_location("ehdg_pupil_detector", "opm_detector_config.json")
         try:
             with open(opm_config) as opm_config_info:
                 opm_config_dict = commentjson.load(opm_config_info)
         except FileNotFoundError:
```

### Comparing `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

