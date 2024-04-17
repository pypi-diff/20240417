# Comparing `tmp/ignutils-0.0.6.tar.gz` & `tmp/ignutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignutils-0.0.6.tar", last modified: Fri Apr 12 14:41:14 2024, max compression
+gzip compressed data, was "ignutils-0.0.7.tar", last modified: Wed Apr 17 13:31:37 2024, max compression
```

## Comparing `ignutils-0.0.6.tar` & `ignutils-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,124 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-12 14:41:14.724990 ignutils-0.0.6/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-12 14:41:07.000000 ignutils-0.0.6/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-12 14:41:14.724990 ignutils-0.0.6/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      602 2024-04-12 14:41:07.000000 ignutils-0.0.6/README.md
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-12 14:41:14.724990 ignutils-0.0.6/ignutils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       33 2024-04-12 14:41:07.000000 ignutils-0.0.6/ignutils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3070 2024-04-12 14:41:07.000000 ignutils-0.0.6/ignutils/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-12 14:41:14.724990 ignutils-0.0.6/ignutils.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-12 14:41:14.000000 ignutils-0.0.6/ignutils.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      252 2024-04-12 14:41:14.000000 ignutils-0.0.6/ignutils.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-12 14:41:14.000000 ignutils-0.0.6/ignutils.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       10 2024-04-12 14:41:14.000000 ignutils-0.0.6/ignutils.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-12 14:41:14.000000 ignutils-0.0.6/ignutils.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      806 2024-04-12 14:41:07.000000 ignutils-0.0.6/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-12 14:41:07.000000 ignutils-0.0.6/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-12 14:41:14.724990 ignutils-0.0.6/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-12 14:41:07.000000 ignutils-0.0.7/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1291 2024-04-17 13:31:37.374993 ignutils-0.0.7/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3893 2024-04-17 13:31:28.000000 ignutils-0.0.7/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      753 2024-04-17 13:31:28.000000 ignutils-0.0.7/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      303 2024-04-17 12:21:27.000000 ignutils-0.0.7/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-17 13:31:37.374993 ignutils-0.0.7/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.306993 ignutils-0.0.7/src/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.334993 ignutils-0.0.7/src/ignutils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3649 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45289 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/active_augmentation.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4159 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/algo_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.342993 ignutils-0.0.7/src/ignutils/autoui_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3885 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/autogui_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    20681 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/autotest_recplayback.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2484 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/calculator_demo.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.346993 ignutils-0.0.7/src/ignutils/calib_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1412 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/angle_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6380 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/charuco_mono_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16504 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/charuco_stereo_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14815 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/infer_depth.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5981 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3770 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6312 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3647 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_undistort.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    44010 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/optimize_depth.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7902 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/point_depth_demo.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10569 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/pose_estimate.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7728 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/rs_crop_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10662 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_3d_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14560 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4941 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10057 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5667 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_record.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.346993 ignutils-0.0.7/src/ignutils/cam_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      871 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5755 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/camera_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1676 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/gopro_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6950 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/realsense_reader.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    12744 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/clone_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5347 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/config_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37875 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/contour_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4201 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/docker_utils.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)     9782 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/draw_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14237 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/file_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1094 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/filter_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8726 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/fisheye_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4775 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/geom_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5746 2024-04-17 13:31:28.000000 ignutils-0.0.7/src/ignutils/gpu_utils.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    24667 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/img_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3061 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/json_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1663 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/keyboard_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5654 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/labelme_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10540 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/license_check.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    20812 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/mouse_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2094 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/multi_process_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.350993 ignutils-0.0.7/src/ignutils/o3d_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1196 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/plot_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3372 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/read_rosbag.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8528 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/registration_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.350993 ignutils-0.0.7/src/ignutils/registration/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      916 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4521 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/ecc_register.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    18564 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/keypoint_register.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1825 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/register_abstract.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1257 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/register_wrapper.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8253 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/superglue_register.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.366993 ignutils-0.0.7/src/ignutils/selenium/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1254 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/selenium/selenium_test.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12894 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/show_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5265 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/ssh_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/stitch_det_track/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6126 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/extract_gps_data.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8250 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/register_seq.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5518 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/stitch.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45952 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/stitch_det_track_seq.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2891 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/unique_identifier.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3232 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/system_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      993 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/timer_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19564 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/transform_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5449 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/transfrom_crops.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1756 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/typehint_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/video_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      826 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2887 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/dump_frames.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2596 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/exif_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3740 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/folder_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3275 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/play_video.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12810 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8329 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_sync.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4369 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_writer.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.306993 ignutils-0.0.7/src/ignutils/vo/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/vo/mono_vo/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3882 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/Visualization.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1964 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_det.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2983 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_track.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6374 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/find_match.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6074 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/main.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22917 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/mono_VO.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2181 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/optimizer.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      684 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/vo/stereo_vo/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5071 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/stereo_vo/data_handler.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    23487 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/stereo_vo/stereo_vo.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/src/ignutils/workflow/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      107 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/__main__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8004 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/filter_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6494 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/keras_seg_mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    17255 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    25301 2024-04-17 11:53:25.000000 ignutils-0.0.7/src/ignutils/workflow/node_config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4818 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/node_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5086 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/seg_mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12781 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/workflow_main.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3435 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/yaml_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/src/ignutils.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1291 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3868 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      304 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/top_level.txt
```

### Comparing `ignutils-0.0.6/LICENSE` & `ignutils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.6/ignutils/json_utils.py` & `ignutils-0.0.7/src/ignutils/json_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class TestJsonUtils(unittest.TestCase):
     """test json utils"""
 
     @classmethod
     def setUpClass(cls):
         """Edit sample docker daemon config file with nvidia runtime."""
-        cls.FILENAME = "ignutils/samples/daemon_sample.json"
+        cls.FILENAME = "samples/daemon_sample.json"
         cls.key_list = ("runtimes", "nvidia", "path")
         cls.val = random.random()
         cls.VALUE = "/usr/bin/nvidia-container-runtime - " + str(cls.val)
 
     def test_edit_json(self):
         """tests the edit json function"""
         print("Testing edit json function \n")
```

### Comparing `ignutils-0.0.6/pyproject.toml` & `ignutils-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ignutils"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
-  { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
+  { name="Ignitarium", email="jerin.antony@ignitarium.com" },
 ]
 description = "A small CV test package"
-readme = "README.md"
+# readme = "pypi/README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
-Homepage = "https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/tree/main?ref_type=heads"
-Issues = "https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/issues"
+Homepage = "https://gitlab.ignitarium.in/ign-ai/internal/ignutils"
+Issues = "https://gitlab.ignitarium.in/ign-ai/internal/ignutils/-/issues"
```

