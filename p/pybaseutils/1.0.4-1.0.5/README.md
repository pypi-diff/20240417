# Comparing `tmp/pybaseutils-1.0.4.tar.gz` & `tmp/pybaseutils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaseutils-1.0.4.tar", last modified: Tue Mar 12 01:03:59 2024, max compression
+gzip compressed data, was "pybaseutils-1.0.5.tar", last modified: Wed Apr 17 03:54:49 2024, max compression
```

## Comparing `pybaseutils-1.0.4.tar` & `pybaseutils-1.0.5.tar`

### file list

```diff
@@ -1,247 +1,250 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.243769 pybaseutils-1.0.4/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.4/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-03-12 01:03:59.243521 pybaseutils-1.0.4/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.4/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.133169 pybaseutils-1.0.4/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-03-12 01:03:56.000000 pybaseutils-1.0.4/pybaseutils/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.137861 pybaseutils-1.0.4/pybaseutils/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.4/pybaseutils/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.4/pybaseutils/audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.4/pybaseutils/audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.4/pybaseutils/audio/vad_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/base64_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.4/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.139503 pybaseutils-1.0.4/pybaseutils/build_utils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.4/pybaseutils/build_utils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.4/pybaseutils/build_utils/cython_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.4/pybaseutils/build_utils/pyarmor_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.141396 pybaseutils-1.0.4/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.4/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.4/pybaseutils/config_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.148803 pybaseutils-1.0.4/pybaseutils/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.4/pybaseutils/converter/build_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.4/pybaseutils/converter/build_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.4/pybaseutils/converter/build_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.4/pybaseutils/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6011 2023-11-23 10:15:35.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_voc2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.4/pybaseutils/converter/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.4/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.152352 pybaseutils-1.0.4/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.4/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10572 2024-03-01 02:06:03.000000 pybaseutils-1.0.4/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.4/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.4/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.159412 pybaseutils-1.0.4/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.4/pybaseutils/dataloader/base_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7605 2024-03-11 07:32:55.000000 pybaseutils-1.0.4/pybaseutils/dataloader/base_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6285 2023-09-26 07:26:12.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_det.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7882 2024-02-05 03:34:25.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_ins.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6811 2023-09-26 07:44:31.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_kps.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17343 2024-03-11 11:27:31.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17368 2024-03-11 09:25:09.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13252 2024-02-05 03:38:27.000000 pybaseutils-1.0.4/pybaseutils/dataloader/parser_yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.4/pybaseutils/dataloader/voc_seg_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    38291 2024-02-20 06:49:28.000000 pybaseutils-1.0.4/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.163466 pybaseutils-1.0.4/pybaseutils/filter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/filter/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/filter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.4/pybaseutils/filter/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/filter/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.4/pybaseutils/filter/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.4/pybaseutils/filter/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.4/pybaseutils/filter/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.164014 pybaseutils-1.0.4/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.4/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.4/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103108 2024-03-01 01:59:53.000000 pybaseutils-1.0.4/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4480 2023-08-11 03:00:05.000000 pybaseutils-1.0.4/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.4/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.167484 pybaseutils-1.0.4/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.4/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.4/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.169897 pybaseutils-1.0.4/pybaseutils/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.4/pybaseutils/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.4/pybaseutils/pose/bones_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.4/pybaseutils/pose/human_pose.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.4/pybaseutils/pose/pose_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.171268 pybaseutils-1.0.4/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.4/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.4/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/pycpp/main.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.172169 pybaseutils-1.0.4/pybaseutils/server/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.4/pybaseutils/server/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.4/pybaseutils/server/apm_server.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.4/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.4/pybaseutils/singleton_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.4/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.4/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.175852 pybaseutils-1.0.4/pybaseutils/tracking/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/tracking/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/tracking/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.4/pybaseutils/tracking/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.4/pybaseutils/tracking/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.4/pybaseutils/tracking/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.4/pybaseutils/tracking/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.4/pybaseutils/tracking/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.178150 pybaseutils-1.0.4/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.4/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5104 2024-02-05 11:42:05.000000 pybaseutils-1.0.4/pybaseutils/transforms/face_alignment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5150 2024-02-21 06:07:01.000000 pybaseutils-1.0.4/pybaseutils/transforms/transform_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.4/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.4/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.4/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.135726 pybaseutils-1.0.4/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-03-12 01:03:59.000000 pybaseutils-1.0.4/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6805 2024-03-12 01:03:59.000000 pybaseutils-1.0.4/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-03-12 01:03:59.000000 pybaseutils-1.0.4/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.4/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-03-12 01:03:59.000000 pybaseutils-1.0.4/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-03-12 01:03:59.243854 pybaseutils-1.0.4/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.4/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.199418 pybaseutils-1.0.4/test_py/
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.203005 pybaseutils-1.0.4/test_py/WebCrawler/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.4/test_py/WebCrawler/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.4/test_py/WebCrawler/search_image.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.4/test_py/WebCrawler/search_image_for_baidu.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/test_py/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.208349 pybaseutils-1.0.4/test_py/aije/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.4/test_py/aije/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.4/test_py/aije/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1005 2024-02-02 01:28:34.000000 pybaseutils-1.0.4/test_py/aije/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      420 2023-09-25 03:45:53.000000 pybaseutils-1.0.4/test_py/aije/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3774 2024-03-07 03:54:50.000000 pybaseutils-1.0.4/test_py/aije/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.4/test_py/aije/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2023-11-23 10:03:31.000000 pybaseutils-1.0.4/test_py/aije/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.4/test_py/aije/video_demo.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.212678 pybaseutils-1.0.4/test_py/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.4/test_py/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.4/test_py/audio/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.4/test_py/audio/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.4/test_py/audio/main_read.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.4/test_py/audio/segment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.4/test_py/audio/speechbrain_asr_indoor_prod.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.4/test_py/audio/speechbrain_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.4/test_py/class_attribute.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.4/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.225922 pybaseutils-1.0.4/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.4/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.4/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.4/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.4/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.4/test_py/converter/FL3D_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.4/test_py/converter/FreiHAND2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.4/test_py/converter/MTFL2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.4/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2718 2024-02-21 06:07:01.000000 pybaseutils-1.0.4/test_py/converter/WaterMeters.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.4/test_py/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.4/test_py/converter/convert_gesture2hand.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.4/test_py/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.4/test_py/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.4/test_py/converter/fatigue_driving.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/converter/fdd_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.4/test_py/converter/handpose2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.4/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.4/test_py/converter/ua_detrac2voc.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.230835 pybaseutils-1.0.4/test_py/cython_build/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.4/test_py/cython_build/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.4/test_py/cython_build/build_cython.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.4/test_py/cython_build/build_pyarmor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.4/test_py/cython_build/cryptography_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.4/test_py/cython_build/fun_sum.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.4/test_py/cython_build/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.4/test_py/cython_build/model_des_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.4/test_py/cython_build/model_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2614 2024-02-21 01:59:28.000000 pybaseutils-1.0.4/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.4/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.4/test_py/demo3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.4/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.4/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.4/test_py/demo_coco_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.4/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.4/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.4/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.4/test_py/demo_for_pair_file.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.4/test_py/demo_for_polygon.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.4/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.4/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.4/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.4/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.4/test_py/demo_image_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.4/test_py/demo_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.4/test_py/demo_nii.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.4/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.4/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1001 2023-08-25 09:55:32.000000 pybaseutils-1.0.4/test_py/demo_rename.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.4/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.4/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.4/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.4/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.4/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.4/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.4/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.232912 pybaseutils-1.0.4/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.4/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.4/test_py/detector/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.4/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.4/test_py/detector/predet_labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.235553 pybaseutils-1.0.4/test_py/edit_distance/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.4/test_py/edit_distance/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.4/test_py/edit_distance/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.4/test_py/edit_distance/text_matching.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.4/test_py/edit_distance/text_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.237202 pybaseutils-1.0.4/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.4/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.4/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.4/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.239045 pybaseutils-1.0.4/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.4/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.4/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.4/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.4/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.4/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.4/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.4/test_py/performance.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.239930 pybaseutils-1.0.4/test_py/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.4/test_py/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.4/test_py/pose/human_pose.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-03-12 01:03:59.242741 pybaseutils-1.0.4/test_py/registry/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.4/test_py/registry/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.4/test_py/registry/base.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.4/test_py/registry/component.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.4/test_py/registry/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.4/test_py/registry/register.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.540737 pybaseutils-1.0.5/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.5/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-04-17 03:54:49.540398 pybaseutils-1.0.5/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.5/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.409094 pybaseutils-1.0.5/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-17 03:54:45.000000 pybaseutils-1.0.5/pybaseutils/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.414853 pybaseutils-1.0.5/pybaseutils/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.5/pybaseutils/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.5/pybaseutils/audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.5/pybaseutils/audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.5/pybaseutils/audio/vad_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.5/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.416692 pybaseutils-1.0.5/pybaseutils/build_utils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.5/pybaseutils/build_utils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.5/pybaseutils/build_utils/cython_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.5/pybaseutils/build_utils/pyarmor_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.419394 pybaseutils-1.0.5/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.5/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.5/pybaseutils/config_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.429336 pybaseutils-1.0.5/pybaseutils/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.5/pybaseutils/converter/build_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.5/pybaseutils/converter/build_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.5/pybaseutils/converter/build_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.5/pybaseutils/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_coco2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.5/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.432421 pybaseutils-1.0.5/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.5/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10572 2024-03-01 02:06:03.000000 pybaseutils-1.0.5/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.5/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.5/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.440160 pybaseutils-1.0.5/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.5/pybaseutils/dataloader/base_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7634 2024-03-18 07:07:15.000000 pybaseutils-1.0.5/pybaseutils/dataloader/base_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_det.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_ins.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_kps.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17642 2024-04-17 03:54:20.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17629 2024-03-18 07:11:47.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.5/pybaseutils/dataloader/voc_seg_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.5/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.444848 pybaseutils-1.0.5/pybaseutils/filter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/filter/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.5/pybaseutils/filter/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/filter/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.5/pybaseutils/filter/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.445546 pybaseutils-1.0.5/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.5/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.5/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103608 2024-03-27 03:34:35.000000 pybaseutils-1.0.5/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4480 2023-08-11 03:00:05.000000 pybaseutils-1.0.5/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.5/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.449630 pybaseutils-1.0.5/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.5/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.5/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.452516 pybaseutils-1.0.5/pybaseutils/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.5/pybaseutils/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.5/pybaseutils/pose/bones_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.5/pybaseutils/pose/human_pose.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.5/pybaseutils/pose/pose_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.454237 pybaseutils-1.0.5/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.5/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.5/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.455515 pybaseutils-1.0.5/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.5/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.5/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.5/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.5/pybaseutils/singleton_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.5/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.5/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.460516 pybaseutils-1.0.5/pybaseutils/tracking/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/tracking/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.463908 pybaseutils-1.0.5/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.5/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5104 2024-02-05 11:42:05.000000 pybaseutils-1.0.5/pybaseutils/transforms/face_alignment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5150 2024-02-21 06:07:01.000000 pybaseutils-1.0.5/pybaseutils/transforms/transform_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.5/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.5/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.5/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.412339 pybaseutils-1.0.5/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6937 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.5/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-17 03:54:49.540829 pybaseutils-1.0.5/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.5/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.487275 pybaseutils-1.0.5/test_py/
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.489146 pybaseutils-1.0.5/test_py/WebCrawler/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.5/test_py/WebCrawler/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.5/test_py/WebCrawler/search_image.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.5/test_py/WebCrawler/search_image_for_baidu.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.499144 pybaseutils-1.0.5/test_py/aije/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.5/test_py/aije/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.5/test_py/aije/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.5/test_py/aije/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.5/test_py/aije/copy_move.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.5/test_py/aije/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.5/test_py/aije/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.5/test_py/aije/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.5/test_py/aije/video_demo.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.503572 pybaseutils-1.0.5/test_py/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.5/test_py/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.5/test_py/audio/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.5/test_py/audio/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.5/test_py/audio/main_read.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.5/test_py/audio/segment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.5/test_py/audio/speechbrain_asr_indoor_prod.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.5/test_py/audio/speechbrain_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.5/test_py/class_attribute.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.5/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.519943 pybaseutils-1.0.5/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.5/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.5/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.5/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.5/test_py/converter/FreiHAND2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.5/test_py/converter/MTFL2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2718 2024-02-21 06:07:01.000000 pybaseutils-1.0.5/test_py/converter/WaterMeters.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.5/test_py/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.5/test_py/converter/convert_gesture2hand.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.5/test_py/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.5/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.5/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.5/test_py/converter/handpose2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.5/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.5/test_py/converter/voc_sbd2labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.525220 pybaseutils-1.0.5/test_py/cython_build/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.5/test_py/cython_build/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.5/test_py/cython_build/build_cython.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.5/test_py/cython_build/build_pyarmor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.5/test_py/cython_build/cryptography_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.5/test_py/cython_build/fun_sum.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.5/test_py/cython_build/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.5/test_py/cython_build/model_des_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.5/test_py/cython_build/model_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2614 2024-02-21 01:59:28.000000 pybaseutils-1.0.5/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.5/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.5/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.5/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.5/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.5/test_py/demo_coco_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.5/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.5/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.5/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.5/test_py/demo_for_pair_file.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.5/test_py/demo_for_polygon.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.5/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.5/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.5/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.5/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.5/test_py/demo_image_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.5/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.5/test_py/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.5/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1049 2024-04-15 12:43:54.000000 pybaseutils-1.0.5/test_py/demo_rename.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.5/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.5/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.5/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.5/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.5/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.5/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.527489 pybaseutils-1.0.5/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.5/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.5/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.5/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.530223 pybaseutils-1.0.5/test_py/edit_distance/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.5/test_py/edit_distance/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.5/test_py/edit_distance/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.5/test_py/edit_distance/text_matching.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.5/test_py/edit_distance/text_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.531903 pybaseutils-1.0.5/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.5/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.5/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.5/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.534708 pybaseutils-1.0.5/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.5/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.5/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.5/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.5/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.536208 pybaseutils-1.0.5/test_py/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.5/test_py/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.5/test_py/pose/human_pose.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.539663 pybaseutils-1.0.5/test_py/registry/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.5/test_py/registry/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.5/test_py/registry/base.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.5/test_py/registry/component.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.5/test_py/registry/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.5/test_py/registry/register.py
```

### Comparing `pybaseutils-1.0.4/LICENCE` & `pybaseutils-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/PKG-INFO` & `pybaseutils-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.4
+Version: 1.0.5
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.4/README.md` & `pybaseutils-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/audio/audio_utils.py` & `pybaseutils-1.0.5/pybaseutils/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/audio/pyaudio_utils.py` & `pybaseutils-1.0.5/pybaseutils/audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/audio/vad_utils.py` & `pybaseutils-1.0.5/pybaseutils/audio/vad_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/base64_utils.py` & `pybaseutils-1.0.5/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/batch_utils.py` & `pybaseutils-1.0.5/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/build_utils/cython_utils.py` & `pybaseutils-1.0.5/pybaseutils/build_utils/cython_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/build_utils/pyarmor_utils.py` & `pybaseutils-1.0.5/pybaseutils/build_utils/pyarmor_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cluster/kmean.py` & `pybaseutils-1.0.5/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-1.0.5/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cluster/similarity.py` & `pybaseutils-1.0.5/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/color_utils.py` & `pybaseutils-1.0.5/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/config_utils.py` & `pybaseutils-1.0.5/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/build_coco.py` & `pybaseutils-1.0.5/pybaseutils/converter/build_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/build_labelme.py` & `pybaseutils-1.0.5/pybaseutils/converter/build_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/build_voc.py` & `pybaseutils-1.0.5/pybaseutils/converter/build_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/concat_coco.py` & `pybaseutils-1.0.5/pybaseutils/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_coco2voc.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2coco.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2voc.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         out_xml_dir = os.path.join(out_root, "Annotations")
         out_image_dir = os.path.join(out_root, "JPEGImages") if out_img else None
         out_crop_dir = os.path.join(out_root, "crops")
         class_set = []
         for i in tqdm(range(len(self.dataset))):
             data = self.dataset.__getitem__(i)
             data = self.get_object_detection(data)
-            image, points, bboxes, labels = data["image"], data["point"], data["box"], data["label"]
+            image, points, bboxes, labels = data["image"], data["points"], data["boxes"], data["labels"]
             anno_file = data["anno_file"]
             image_file = data["image_file"]
             image_shape = image.shape
             if len(labels) == 0:
                 # file_utils.remove_file(anno_file)
                 # file_utils.remove_file(image_file)
                 print("empty dst_result:{}".format(image_file))
```

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_labelme2yolo.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_voc2coco.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_voc2voc.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_voc2yolo.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/converter/convert_yolo2voc.py` & `pybaseutils-1.0.5/pybaseutils/converter/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/coords_utils.py` & `pybaseutils-1.0.5/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-1.0.5/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cvutils/monitor.py` & `pybaseutils-1.0.5/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-1.0.5/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/cvutils/video_utils.py` & `pybaseutils-1.0.5/pybaseutils/cvutils/video_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/base_coco.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/base_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/base_dataset.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/base_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 class Dataset(object):
     """
     from torch.utils.data import Dataset,DataLoader, ConcatDataset
     """
 
     def __init__(self, **kwargs):
         self.image_ids = []
+        self.postfix = "jpg"
 
     def __getitem__(self, index):
         raise NotImplementedError
 
     def __add__(self, other):
         return ConcatDataset([self, other])
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_det.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_det.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         num_boxes = len(boxes)
         if self.target_transform:
             boxes, labels = self.target_transform(boxes, labels)
         target = self.convert_target(boxes, labels)
         if num_boxes == 0:
             index = int(random.uniform(0, len(self)))
             return self.__getitem__(index)
-        data = {"image": image, "target": target, "label": labels, "image_id": image_id,
+        data = {"image": image, "target": target, "labels": labels, "image_id": image_id,
                 "image_file": image_file, "size": [width, height], "class_name": self.class_name}
         return data
 
 
 def CocoDetections(anno_file=None,
                    image_dir="",
                    class_name=None,
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_ins.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_ins.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         :param vis:
         :return: 
         """
         image_id = self.image_ids[index]
         anns_info, file_info = self.get_object_annotations(image_id)
         image, width, height, image_file = self.get_object_image(file_info)
         boxes, labels, mask, segs = self.get_object_instance(anns_info, h=height, w=width, decode=self.decode)
-        data = {"segs": segs, "mask": mask, "image": image, "boxes": boxes, "label": labels,
+        data = {"segs": segs, "mask": mask, "image": image, "boxes": boxes, "labels": labels,
                 "image_id": image_id, "annotations": anns_info, "file_info": file_info,
                 "image_file": image_file, "size": [width, height], "class_name": self.class_name}
         return data
 
 
 def CocoInstances(anno_file=None,
                   image_dir="",
@@ -128,31 +128,31 @@
     class_name = ["BG", 'car', 'person']
     # class_name = {'bb': "bk", "person": "unique"}
     # 测试COCO数据集
     # anno_file2 = "/home/PKing/nasdata/dataset/face_person/COCO/val2017/instances_val2017.json"
 
     anno_file1 = "/media/PKing/新加卷1/SDK/base-utils/data/coco/coco_ins.json"
     anno_file2 = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v2/train_coco_instance.json"
+    anno_file2 = "/media/PKing/新加卷1/SDK/base-utils/data/coco/coco_ins.json"
     # anno_file2 = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v2/train_coco_instance.json"
     # class_name = ["BG", 'car,person,身穿工作服']
     # class_name = {"BG": 0, 'car': 1, 'person': 1, "身穿工作服": 1}
 
     class_name = {'手': 0, '护目镜': 1, '未穿工作服': 2, '身穿工作服': 2, '其他鞋': 3, '绝缘鞋': 3, '安全带': 4, '安全帽': 5,
                   '绝缘垫': 6, '绝缘手套': 7, '万用表': 8, '万用表线头': 9, '相序表': 10, '相序表线头': 11, '钳形电流表': 12,
                   '电能表': 13, '尖嘴钳': 14, '验电笔': 15, '螺丝刀': 16, '接线盒': 17, '电流互感器': 18, '表箱关': 19,
                   '表箱开': 19, '竹梯': 20, '准备区域': 21, '工作台': 22}
     #
     # anno_file = "/media/PKing/新加卷1/SDK/base-utils/data/coco/coco_ins.json"
     # anno_file = "/home/PKing/nasdata/dataset/tmp/hand-pose/FreiHAND/training/coco_kps.json"
     # image_dir = "/home/PKing/nasdata/dataset/tmp/hand-pose/FreiHAND/training/rgb"
-    # class_name = None
+    class_name = None
     # dataset = CocoInstance(anno_file=anno_file, image_dir="", class_name=class_name)
     dataset = CocoInstances(anno_file=[anno_file1, anno_file2], image_dir="",
                             class_name=class_name, use_rgb=False, shuffle=False)
     class_name = dataset.class_name
     for i in range(len(dataset)):
-        i = 2159
         data = dataset.__getitem__(i)
         image, boxes, labels, mask = data['image'], data["boxes"], data["label"], data["mask"]
         print("i={},image_id={}".format(i, data["image_id"]))
         # dataset.showAnns(image, data['annotations'])
         show_target_image(image, mask, boxes, labels, class_name=class_name)
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_coco_kps.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_kps.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         :param vis:
         :return: 
         """
         image_id = self.image_ids[index]
         anns_info, file_info = self.get_object_annotations(image_id)
         image, width, height, image_file = self.get_object_image(file_info)
         boxes, labels, keypoints = self.get_keypoint_info(anns_info, self.num_joints)
-        data = {"keypoints": keypoints, "image": image, "boxes": boxes, "label": labels, "image_id": image_id,
+        data = {"keypoints": keypoints, "image": image, "boxes": boxes, "labels": labels, "image_id": image_id,
                 "annotations": anns_info, "file_info": file_info, "image_file": image_file,
                 "size": [width, height], "class_name": self.class_name}
         return data
 
 
 def CocoKeypoints(anno_file=None,
                   image_dir="",
@@ -144,11 +144,11 @@
     anno_file = "/home/PKing/nasdata/dataset/tmp/hand-pose/HandPose-v2/train/train_anno.json"
     class_name = []
     dataset = CocoKeypoint(anno_file, image_dir, class_name=class_name)
     skeleton = dataset.skeleton
     for i in range(len(dataset)):
         data = dataset.__getitem__(i)
         # data = {"segs": segs, "image": image, "boxes": boxes, "label": labels, "image_id": image_id}
-        image, boxes, labels, keypoints = data['image'], data["boxes"], data["label"], data["keypoints"]
+        image, boxes, labels, keypoints = data['image'], data["boxes"], data["labels"], data["keypoints"]
         print("i={},image_id={}".format(i, data["image_id"]))
         # dataset.showAnns(image, data['annotations'])
         show_target_image(image, keypoints, boxes, skeleton=skeleton)
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,29 +185,29 @@
         image_file, anno_file, image_id = self.get_image_anno_file(image_id)
         annotation, width, height = self.load_annotations(anno_file)
         image = self.read_image(image_file, use_rgb=self.use_rgb)
         shape = image.shape
         boxes, labels, points, groups = self.parser_annotation(annotation, self.class_dict, shape,
                                                                min_points=self.min_points)
         data = {"image": image, "points": points, "boxes": boxes, "labels": labels, "groups": groups,
-                "image_file": image_file, "anno_file": anno_file, "size": [width, height]}
+                "image_file": image_file, "anno_file": anno_file, "size": [shape[1], shape[0]]}
         return data
 
     @staticmethod
     def parser_annotation(annotation: dict, class_dict={}, shape=None, min_points=-1):
         """
         :param annotation:  labelme标注的数据
         :param class_dict:  label映射
         :param shape: 图片shape(H,W,C),可进行坐标点的维度检查，避免越界
         :param min_points: 当标注的轮廓点的个数小于等于min_points，会被剔除；负数不剔除
         :return:
         """
         bboxes, labels, points, groups = [], [], [], []
         for anno in annotation:
-            label = anno["label"].lower()
+            label = anno["label"]
             if class_dict:
                 if not label in class_dict:
                     continue
                 if isinstance(class_dict, dict):
                     label = class_dict[label]
             pts = np.asarray(anno["points"], dtype=np.int32)
             if min_points > 0 and len(pts) <= min_points:
@@ -277,15 +277,15 @@
         :param w:
         :param h:
         :param class_name:
         :return:
         """
         objects = {}
         for i, anno in enumerate(annotation):
-            label = anno["label"].lower()
+            label = anno["label"]
             points = np.asarray(anno["points"], dtype=np.int32)
             group_id = anno["group_id"] if "group_id" in anno and anno["group_id"] else 0  # 通过group_id标记同一实例
             if file_utils.is_int(label):
                 keypoints: dict = json_utils.get_value(objects, [group_id, "keypoints"], default={})
                 keypoints.update({int(label): points.tolist()[0]})
                 objects = json_utils.set_value(objects, key=[group_id, "keypoints"], value=keypoints)
             elif label in class_name:
@@ -306,15 +306,15 @@
         :param w:
         :param h:
         :param class_name:
         :return:
         """
         objects = {}
         for i, anno in enumerate(annotation):
-            label = anno["label"].lower()
+            label = anno["label"]
             points = np.asarray(anno["points"], dtype=np.int32)
             group_id = i
             if file_utils.is_int(label):
                 continue
             elif class_name is None or len(class_name) == 0 or label in class_name:
                 segs = points
                 segs[:, 0] = np.clip(segs[:, 0], 0, w - 1)
@@ -324,18 +324,18 @@
                                                value={"labels": label, "boxes": box, "segs": segs})
         return objects
 
     @staticmethod
     def load_annotations(ann_file: str):
         try:
             with open(ann_file, "r") as f:
-                annotation = json.load(f)
-            annos = annotation["shapes"]
-            width = annotation['imageWidth']
-            height = annotation['imageHeight']
+                annotation: dict = json.load(f)
+            annos = annotation.get("shapes", [])
+            width = annotation.get('imageWidth', -1)
+            height = annotation.get('imageHeight', -1)
         except:
             print("illegal annotation:{}".format(ann_file))
             annos = []
             width = -1
             height = -1
         return annos, width, height
 
@@ -396,24 +396,27 @@
     """
     annotation, width, height = LabelMeDataset.load_annotations(anno_file)
     bboxes, labels, points, groups = LabelMeDataset.parser_annotation(annotation, class_dict, shape)
     return bboxes, labels, points, groups
 
 
 def show_target_image(image, bboxes, labels, points):
-    image = image_utils.draw_image_bboxes_text(image, bboxes, labels, color=(255, 0, 0))
+    image = image_utils.draw_image_bboxes_text(image, bboxes, labels, color=(255, 0, 0),
+                                               thickness=2, fontScale=1.2, drawType="chinese")
     # image = image_utils.draw_landmark(image, points, color=(0, 255, 0))
     image = image_utils.draw_key_point_in_image(image, points)
     image_utils.cv_show_image("det", image)
 
 
 if __name__ == "__main__":
     from pybaseutils.converter import build_labelme
 
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v1/json"
+    anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v7/json"
+    anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-outdoor-det/dataset-test/json"
     # anno_dir = [anno_dir, anno_dir]
     names = None
     dataset = LabelMeDatasets(filename=None,
                               data_root=None,
                               anno_dir=anno_dir,
                               image_dir=None,
                               class_name=names,
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,17 @@
             image_dir = os.path.join(data_root, "JPEGImages")
         if image_dir and not image_ids:
             image_ids = self.get_file_list(image_dir, postfix=file_utils.IMG_POSTFIX, basename=False)
             image_ids = [os.path.basename(f) for f in image_ids]
         elif anno_dir and not image_ids:
             image_ids = self.get_file_list(anno_dir, postfix=["*.xml"], basename=False)
             image_ids = [os.path.basename(f) for f in image_ids]
+
+        files = self.get_file_list(image_dir, postfix=file_utils.IMG_POSTFIX, basename=False)
+        self.postfix = os.path.basename(files[0]).split(".")[-1] if files else "jpg"
         return data_root, anno_dir, image_dir, image_ids
 
     def convert_target(self, boxes, labels):
         # （xmin,ymin,xmax,ymax,label）
         if len(boxes) == 0:
             target = np.empty(shape=(0, 5), dtype=np.float32)
         else:
@@ -203,15 +206,15 @@
         # boxes, labels = self.target_transform(boxes, labels)  # torch.Size([29952, 4]),torch.Size([29952])
         target = self.convert_target(boxes, labels)
         if num_boxes == 0 or len(labels) == 0:
             index = int(random.uniform(0, len(self)))
             return self.__getitem__(index)
         # return image, boxes, labels
         # return image, {"target": target, "image_id": image_id, "size": [width, height]}
-        data = {"image": image, "target": target, "image_id": image_id,
+        data = {"image": image, "target": target, "boxes": boxes, "labels": labels, "image_id": image_id,
                 "size": [width, height], "image_file": image_file}
         return data
 
     def get_image_anno_file(self, index):
         """
         :param index:
         :return:
@@ -224,15 +227,15 @@
         """
         :param index: int or str
         :return:
         """
         if isinstance(index, numbers.Number):
             image_id = self.image_ids[index]
         else:
-            image_id = index
+            image_id = index if "." in index else f"{index}.{self.postfix}"
         return image_id
 
     def __len__(self):
         return len(self.image_ids)
 
     def get_segment_info(self, filename, bbox):
         """
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/parser_yolo.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/parser_yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,16 +212,16 @@
         :return:rgb_image
         """
         image_id = self.index2id(index)
         image_file, anno_file, image_id = self.get_image_anno_file(image_id)
         image = self.read_image(image_file, use_rgb=self.use_rgb)
         shape = image.shape
         annotation = self.load_annotations(anno_file)
-        box, label, point = self.parser_annotation(annotation, shape, self.class_dict)
-        data = {"image": image, "box": box, "label": label, "point": point,
+        boxes, labels, points = self.parser_annotation(annotation, shape, self.class_dict)
+        data = {"image": image, "boxes": boxes, "labels": labels, "points": points,
                 "image_file": image_file, "anno_file": anno_file}
         return data
 
     @staticmethod
     def parser_annotation(annotation: dict, shape, class_dict):
         """
         :param annotation:  labelme标注的数据
```

### Comparing `pybaseutils-1.0.4/pybaseutils/dataloader/voc_seg_utils.py` & `pybaseutils-1.0.5/pybaseutils/dataloader/voc_seg_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/file_utils.py` & `pybaseutils-1.0.5/pybaseutils/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1229,11 +1229,38 @@
     if max_num:
         max_num = min(max_num, len(file_list))
         file_list = file_list[0:max_num]
     write_list_data(filename, file_list)
     print("num files:{},out_path:{}".format(len(file_list), filename))
 
 
+def copy_move_voc_dataset(data_file, data_root=None, out_root=None, file_map={}, move=False):
+    """
+    :param data_file: voc file.txt
+    :param data_root: voc dataset root path
+    :param out_root:  new output root path
+    :param file_map: {"Annotations": "xml", "json": "json", "JPEGImages": None}
+    :param move: move or copy
+    :return:
+    """
+    if not data_root: data_root = os.path.dirname(data_file)
+    files = read_data(data_file, split=None)
+    for name in tqdm(files):
+        idx, pos = name.split(".")
+        for sub, p in file_map.items():
+            n = name.replace(f".{pos}", f".{p}") if p else name
+            path = os.path.join(data_root, sub, n)
+            if out_root and os.path.exists(path):
+                dest = os.path.join(out_root, sub, n)
+                if move:
+                    move_file(path, dest)
+                else:
+                    copy_file(path, dest)
+            else:
+                print(f"no file:{path}")
+    return files
+
+
 if __name__ == '__main__':
     dir = "/home/dm/nasdata/dataset-dmai/handwriting/word-class/trainval/unknown"
     file_list, label_list = get_files_labels(dir)
     print(label_list)
```

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/QueueTable.py` & `pybaseutils-1.0.5/pybaseutils/filter/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/demo.py` & `pybaseutils-1.0.5/pybaseutils/filter/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/kalman_filter.py` & `pybaseutils-1.0.5/pybaseutils/filter/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/mean_filter.py` & `pybaseutils-1.0.5/pybaseutils/filter/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/motion_filter.py` & `pybaseutils-1.0.5/pybaseutils/filter/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/filter/pose_filter.py` & `pybaseutils-1.0.5/pybaseutils/filter/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/font_style/__init__.py` & `pybaseutils-1.0.5/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/font_utils.py` & `pybaseutils-1.0.5/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/geometry_tools.py` & `pybaseutils-1.0.5/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/heatmap_utils.py` & `pybaseutils-1.0.5/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/image_utils.py` & `pybaseutils-1.0.5/pybaseutils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1044,44 +1044,50 @@
     :return:
     """
     boxes = rects2bboxes(rects)
     image = draw_image_bboxes_labels_text(image, boxes, labels, boxes_name, color, drawType, top)
     return image
 
 
-def show_image_bboxes_text(title, image, boxes, boxes_name, color=None, drawType="custom", delay=0, top=True):
+def show_image_bboxes_text(title, image, boxes, boxes_name, color=None, thickness=-1, fontScale=-1.0,
+                           drawType="custom", delay=0, top=True):
     """
     :param boxes_name:
     :param bgr_image: bgr image
     :param color: BGR color:[B,G,R]
     :param boxes: [[x1,y1,x2,y2],[x1,y1,x2,y2]]
     :return:
     """
     bgr_image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
-    bgr_image = draw_image_bboxes_text(bgr_image, boxes, boxes_name, color, drawType, top)
+    bgr_image = draw_image_bboxes_text(bgr_image, boxes, boxes_name=boxes_name, color=color, thickness=thickness,
+                                       fontScale=fontScale, drawType=drawType, top=top)
     image = cv2.cvtColor(bgr_image, cv2.COLOR_BGR2RGB)
     cv_show_image(title, image, delay=delay)
     return image
 
 
-def draw_image_rects_text(image, rects, rects_name, color=None, drawType="custom", top=True):
+def draw_image_rects_text(image, rects, rects_name, color=None, thickness=-1, fontScale=-1.0,
+                          drawType="custom", top=True):
     boxes = rects2bboxes(rects)
-    image = draw_image_bboxes_text(image, boxes, rects_name, color, drawType, top)
+    image = draw_image_bboxes_text(image, boxes, boxes_name=rects_name, color=color, thickness=thickness,
+                                   fontScale=fontScale, drawType=drawType, top=top)
     return image
 
 
-def show_image_rects_text(title, image, rects, rects_name, color=None, drawType="custom", delay=0, top=True):
+def show_image_rects_text(title, image, rects, rects_name, color=None, thickness=-1, fontScale=-1.0, drawType="custom",
+                          delay=0, top=True):
     """
     :param rects_name:
     :param bgr_image: bgr image
     :param rects: [[x1,y1,w,h],[x1,y1,w,h]]
     :return:
     """
     boxes = rects2bboxes(rects)
-    image = show_image_bboxes_text(title, image, boxes, rects_name, color, drawType, delay, top)
+    image = show_image_bboxes_text(title, image, boxes, boxes_name=rects_name, color=color, thickness=thickness,
+                                   fontScale=fontScale, drawType=drawType, delay=delay, top=top)
     return image
 
 
 def draw_image_bboxes_labels(image, bboxes, labels, class_name=None, color=None,
                              thickness=-1, fontScale=-1.0, drawType="custom"):
     """
     :param image:
```

### Comparing `pybaseutils-1.0.4/pybaseutils/json_utils.py` & `pybaseutils-1.0.5/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/log.py` & `pybaseutils-1.0.5/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/logger.py` & `pybaseutils-1.0.5/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/metrics/accuracy.py` & `pybaseutils-1.0.5/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/metrics/average_meter.py` & `pybaseutils-1.0.5/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/metrics/class_report.py` & `pybaseutils-1.0.5/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/metrics/plot_pr.py` & `pybaseutils-1.0.5/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/metrics/plot_roc.py` & `pybaseutils-1.0.5/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/numpy_utils.py` & `pybaseutils-1.0.5/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pandas_utils.py` & `pybaseutils-1.0.5/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/plot_utils.py` & `pybaseutils-1.0.5/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pose/bones_utils.py` & `pybaseutils-1.0.5/pybaseutils/pose/bones_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pose/human_pose.py` & `pybaseutils-1.0.5/pybaseutils/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pose/pose_utils.py` & `pybaseutils-1.0.5/pybaseutils/pose/pose_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pycpp/demo.py` & `pybaseutils-1.0.5/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/pycpp/main.py` & `pybaseutils-1.0.5/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/server/apm_server.py` & `pybaseutils-1.0.5/pybaseutils/server/apm_server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/setup_config.py` & `pybaseutils-1.0.5/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/singleton_utils.py` & `pybaseutils-1.0.5/pybaseutils/singleton_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/thread_utils.py` & `pybaseutils-1.0.5/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/time_utils.py` & `pybaseutils-1.0.5/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracemalloc_utils.py` & `pybaseutils-1.0.5/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-1.0.5/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/QueueTable.py` & `pybaseutils-1.0.5/pybaseutils/tracking/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/demo.py` & `pybaseutils-1.0.5/pybaseutils/tracking/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/kalman_filter.py` & `pybaseutils-1.0.5/pybaseutils/tracking/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/mean_filter.py` & `pybaseutils-1.0.5/pybaseutils/tracking/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/motion_filter.py` & `pybaseutils-1.0.5/pybaseutils/tracking/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/tracking/pose_filter.py` & `pybaseutils-1.0.5/pybaseutils/tracking/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/transforms/affine_transform.py` & `pybaseutils-1.0.5/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/transforms/face_alignment.py` & `pybaseutils-1.0.5/pybaseutils/transforms/face_alignment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/transforms/transform_utils.py` & `pybaseutils-1.0.5/pybaseutils/transforms/transform_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/word_utils.py` & `pybaseutils-1.0.5/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/worker.py` & `pybaseutils-1.0.5/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils/yaml_utils.py` & `pybaseutils-1.0.5/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-1.0.5/pybaseutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.4
+Version: 1.0.5
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.4/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-1.0.5/pybaseutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,21 @@
 pybaseutils/cluster/maxmin_distance.py
 pybaseutils/cluster/similarity.py
 pybaseutils/converter/__init__.py
 pybaseutils/converter/build_coco.py
 pybaseutils/converter/build_labelme.py
 pybaseutils/converter/build_voc.py
 pybaseutils/converter/concat_coco.py
+pybaseutils/converter/convert_coco2labelme.py
 pybaseutils/converter/convert_coco2voc.py
 pybaseutils/converter/convert_labelme2coco.py
 pybaseutils/converter/convert_labelme2voc.py
 pybaseutils/converter/convert_labelme2yolo.py
 pybaseutils/converter/convert_voc2coco.py
+pybaseutils/converter/convert_voc2labelme.py
 pybaseutils/converter/convert_voc2voc.py
 pybaseutils/converter/convert_voc2yolo.py
 pybaseutils/converter/convert_yolo2voc.py
 pybaseutils/cvutils/__init__.py
 pybaseutils/cvutils/corner_utils.py
 pybaseutils/cvutils/monitor.py
 pybaseutils/cvutils/mouse_utils.py
@@ -145,15 +147,15 @@
 test_py/performance.py
 test_py/WebCrawler/__init__.py
 test_py/WebCrawler/search_image.py
 test_py/WebCrawler/search_image_for_baidu.py
 test_py/aije/__init__.py
 test_py/aije/convert_labelme2coco.py
 test_py/aije/convert_labelme2voc.py
-test_py/aije/demo2.py
+test_py/aije/copy_move.py
 test_py/aije/demo_video_aije.py
 test_py/aije/demo_voc_crop.py
 test_py/aije/demo_voc_vis.py
 test_py/aije/video_demo.py
 test_py/audio/__init__.py
 test_py/audio/demo.py
 test_py/audio/main.py
@@ -180,14 +182,15 @@
 test_py/converter/convert_labelme2voc.py
 test_py/converter/fatigue_driving.py
 test_py/converter/fdd_dataset.py
 test_py/converter/handpose2coco.py
 test_py/converter/insects_for_aichallenger.py
 test_py/converter/tt100k_utils.py
 test_py/converter/ua_detrac2voc.py
+test_py/converter/voc_sbd2labelme.py
 test_py/cython_build/__init__.py
 test_py/cython_build/build_cython.py
 test_py/cython_build/build_pyarmor.py
 test_py/cython_build/cryptography_demo.py
 test_py/cython_build/fun_sum.py
 test_py/cython_build/main.py
 test_py/cython_build/model_des_enctypt.py
```

### Comparing `pybaseutils-1.0.4/setup.py` & `pybaseutils-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/WebCrawler/search_image.py` & `pybaseutils-1.0.5/test_py/WebCrawler/search_image.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/WebCrawler/search_image_for_baidu.py` & `pybaseutils-1.0.5/test_py/WebCrawler/search_image_for_baidu.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/aije/convert_labelme2coco.py` & `pybaseutils-1.0.5/test_py/aije/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/aije/convert_labelme2voc.py` & `pybaseutils-1.0.5/test_py/aije/convert_labelme2voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 sys.path.insert(0, os.getcwd())
 import cv2
 from pybaseutils.converter.convert_labelme2voc import Labelme2VOC
 
 if __name__ == "__main__":
     # 将AIJE项目数据集，转换为VOC数据集
     # json_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-test/json"
-    json_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-outdoor-det/dataset-v2/json"
+    json_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v7/json"
     data_root = os.path.dirname(json_dir)
     image_dir = os.path.join(data_root, "JPEGImages")
 
     # class_dict = {"身穿工作服": "person", "未穿工作服": "person"}
     # out_root = os.path.join(data_root, "person")
     # out_image_dir = os.path.join(data_root, "person")
 
     class_dict = None
     lm = Labelme2VOC(image_dir, json_dir, class_name=class_dict, shuffle=False)
-    lm.build_dataset(data_root, class_dict={}, out_img=False, vis=False, crop=False)
+    lm.build_dataset(data_root, class_dict={}, out_img=False, vis=False, crop=True)
```

### Comparing `pybaseutils-1.0.4/test_py/aije/demo_video_aije.py` & `pybaseutils-1.0.5/test_py/aije/demo_video_aije.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,17 @@
     :param thresh: 相似度阈值
     :param vis: 是否可视化显示
     :return:
     """
     sm = monitor.StatusMonitor()
     # 室内
     name = os.path.basename(video_file).split(".")[0]
-    name = "{}_{}".format(os.path.basename(os.path.dirname(video_file)), name)
+    # name = "{}_{}".format(os.path.basename(os.path.dirname(video_file)), name)
     if prefix: name = f"{prefix}_{name}"
+    name = name.replace("-", "_")
     for k, v in name_table.items(): name = name.replace(k, v)
     # 室外
     # name = file_utils.get_time()
     video_cap = image_utils.get_video_capture(video_file)
     width, height, num_frames, fps = image_utils.get_video_info(video_cap)
     if not os.path.exists(out_dir): os.makedirs(out_dir)
     count = 0
@@ -68,28 +69,31 @@
         count += 1
     video_cap.release()
     cv2.destroyAllWindows()
 
 
 # thresh_dict = {"1号视角": 0.5, "2号视角": 0.15, "3号视角": 0.3, "4号视角": 0.3}
 # thresh_dict = {"一号位": 0.58, "平视": 0.35, "俯视": 0.35, "右视": 0.25, "左视": 0.3}
-thresh_dict = {"第一视角": 0.58, "主视角": 0.58, "平视": 0.30, "俯视": 0.30, "右视": 0.4, "左视": 0.4, "全景": 0.35}
+thresh_dict = {"第一视角": 0.50, "主视角": 0.50, "平视": 0.30, "俯视": 0.30, "右视": 0.35, "左视": 0.35, "全景": 0.30}
+
+
 # thresh_dict = {"1号位": 0.58, "平视": 0.35, "全景": 0.35, "俯视": 0.35, "右视": 0.25, "左视": 0.3}
 
 
 def video2frames_demo(root, out, prefix="", thresh=0.2):
     files = file_utils.get_files_lists(root, postfix=["*.avi", "*.mp4", "*.flv"])
     for video_file in tqdm(files):
         print(video_file)
         name = os.path.basename(video_file).split(".")[0]
         if name in thresh_dict:
             thresh = thresh_dict[name]
-        prefix_ = "{}_{}".format(prefix,os.path.basename(root))
+        prefix_ = "{}_{}".format(prefix, os.path.basename(os.path.dirname(video_file)))
         video2frames_similarity(video_file, out_dir=out, func=None, interval=100,
                                 thresh=thresh, prefix=prefix_, vis=True)
 
 
 if __name__ == "__main__":
-    root = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/南沙视频/室内"
-    prefix = "南沙"
+    image_utils.find_mask_contours()
+    root = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/使用钳形电流表测量低压线路电流/天河数据/2024-04-12-8"
+    prefix = "天河"
     out = root + "-train"
     video2frames_demo(root, out, prefix=prefix)
```

### Comparing `pybaseutils-1.0.4/test_py/aije/demo_voc_crop.py` & `pybaseutils-1.0.5/test_py/aije/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/aije/demo_voc_vis.py` & `pybaseutils-1.0.5/test_py/aije/demo_voc_vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pybaseutils.dataloader import parser_voc
 
 if __name__ == "__main__":
     class_name = {'手': 0, '护目镜': 1, '未穿工作服': 2, '身穿工作服': 2, '其他鞋': 3, '绝缘鞋': 3, '安全带': 4, '安全帽': 5,
                   '绝缘垫': 6, '绝缘手套': 7, '万用表': 8, '万用表线头': 9, '相序表': 10, '相序表线头': 11, '钳形电流表': 12,
                   '电能表': 13, '尖嘴钳': 14, '验电笔': 15, '螺丝刀': 16, '接线盒': 17, '电流互感器': 18, '表箱关': 19,
                   '表箱开': 19, '竹梯': 20, '准备区域': 21, '工作台': 22}
-    filename = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v5/train.txt"
+    filename = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v7/train.txt"
     dataset = parser_voc.VOCDataset(filename=filename,
                                     data_root=None,
                                     anno_dir=None,
                                     image_dir=None,
                                     class_name=class_name,
                                     transform=None,
                                     use_rgb=False,
```

### Comparing `pybaseutils-1.0.4/test_py/aije/video_demo.py` & `pybaseutils-1.0.5/test_py/aije/video_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/demo.py` & `pybaseutils-1.0.5/test_py/audio/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/main.py` & `pybaseutils-1.0.5/test_py/audio/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/main_read.py` & `pybaseutils-1.0.5/test_py/audio/main_read.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/segment.py` & `pybaseutils-1.0.5/test_py/audio/segment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/speechbrain_asr_indoor_prod.py` & `pybaseutils-1.0.5/test_py/audio/speechbrain_asr_indoor_prod.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/audio/speechbrain_demo.py` & `pybaseutils-1.0.5/test_py/audio/speechbrain_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/class_attribute.py` & `pybaseutils-1.0.5/test_py/class_attribute.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/class_names.py` & `pybaseutils-1.0.5/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/AffectNet.py` & `pybaseutils-1.0.5/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/AsianMovie.py` & `pybaseutils-1.0.5/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/BITVehicle2voc.py` & `pybaseutils-1.0.5/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/BSTLD2voc.py` & `pybaseutils-1.0.5/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/CCPD.py` & `pybaseutils-1.0.5/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/CCPD2voc.py` & `pybaseutils-1.0.5/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/FL3D_dataset.py` & `pybaseutils-1.0.5/test_py/converter/FL3D_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/MTFL2voc.py` & `pybaseutils-1.0.5/test_py/converter/MTFL2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/TT100K.py` & `pybaseutils-1.0.5/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/WaterMeters.py` & `pybaseutils-1.0.5/test_py/converter/WaterMeters.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/concat_coco.py` & `pybaseutils-1.0.5/test_py/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/convert_coco2voc.py` & `pybaseutils-1.0.5/test_py/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/convert_gesture2hand.py` & `pybaseutils-1.0.5/test_py/converter/convert_gesture2hand.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/convert_labelme2coco.py` & `pybaseutils-1.0.5/test_py/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/convert_labelme2voc.py` & `pybaseutils-1.0.5/test_py/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/fatigue_driving.py` & `pybaseutils-1.0.5/test_py/converter/fatigue_driving.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/fdd_dataset.py` & `pybaseutils-1.0.5/test_py/converter/fdd_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/handpose2coco.py` & `pybaseutils-1.0.5/test_py/converter/handpose2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-1.0.5/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/tt100k_utils.py` & `pybaseutils-1.0.5/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/converter/ua_detrac2voc.py` & `pybaseutils-1.0.5/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/cython_build/build_cython.py` & `pybaseutils-1.0.5/test_py/cython_build/build_cython.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/cython_build/build_pyarmor.py` & `pybaseutils-1.0.5/test_py/cython_build/build_pyarmor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/cython_build/cryptography_demo.py` & `pybaseutils-1.0.5/test_py/cython_build/cryptography_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/cython_build/model_des_enctypt.py` & `pybaseutils-1.0.5/test_py/cython_build/model_des_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/cython_build/model_enctypt.py` & `pybaseutils-1.0.5/test_py/cython_build/model_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo1.py` & `pybaseutils-1.0.5/test_py/demo1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo2.py` & `pybaseutils-1.0.5/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo3.py` & `pybaseutils-1.0.5/test_py/demo3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_async_await2.py` & `pybaseutils-1.0.5/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_coco_vis.py` & `pybaseutils-1.0.5/test_py/demo_coco_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_copy_files.py` & `pybaseutils-1.0.5/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_copy_files_for_voc.py` & `pybaseutils-1.0.5/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_ffmpy.py` & `pybaseutils-1.0.5/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_for_pair_file.py` & `pybaseutils-1.0.5/test_py/demo_for_pair_file.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_for_polygon.py` & `pybaseutils-1.0.5/test_py/demo_for_polygon.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_get_file_list.py` & `pybaseutils-1.0.5/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_gif.py` & `pybaseutils-1.0.5/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_gif_video.py` & `pybaseutils-1.0.5/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_image_crop.py` & `pybaseutils-1.0.5/test_py/demo_image_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_labelme.py` & `pybaseutils-1.0.5/test_py/demo_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_metrics.py` & `pybaseutils-1.0.5/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_mouse.py` & `pybaseutils-1.0.5/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_nii.py` & `pybaseutils-1.0.5/test_py/demo_nii.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_pandas.py` & `pybaseutils-1.0.5/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_plot.py` & `pybaseutils-1.0.5/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_rename.py` & `pybaseutils-1.0.5/test_py/demo_rename.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 """
 import os
 from tqdm import tqdm
 from pybaseutils import image_utils, file_utils
 
 
 def rename_image_file(image_dir, output, prefix=""):
-    file_list = file_utils.get_images_list(image_dir)
+    file_list = file_utils.get_files_lists(image_dir)
     time = file_utils.get_time()
     file_utils.create_dir(output)
     for i, old in tqdm(enumerate(file_list)):
         postfix = old.split(".")[-1]
         name = "{}_{}".format(prefix, time) if prefix else time
         name = "{}_{:0=4d}.{}".format(name, i, postfix)
         new = os.path.join(output, name)
         file_utils.copy_file(old, new)
 
 
 if __name__ == '__main__':
-    image_dir = "/home/PKing/nasdata/dataset/tmp/challenge/鸟类品种识别/鸟类品种识别挑战赛训练集/training_set/鹰"
-    output = "/home/PKing/nasdata/dataset/tmp/challenge/鸟类品种识别/鸟类品种识别挑战赛训练集/training_set/鹰-new"
-    rename_image_file(image_dir, output, prefix="")
+
+    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/使用钳形电流表测量低压线路电流/天河数据/2024-04-12-1-2-train"
+    output = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/使用钳形电流表测量低压线路电流/天河数据/2024-04-12-1-2-train2"
+    rename_image_file(image_dir, output, prefix="南沙")
```

### Comparing `pybaseutils-1.0.4/test_py/demo_standard_image .py` & `pybaseutils-1.0.5/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_standard_video .py` & `pybaseutils-1.0.5/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_taichi.py` & `pybaseutils-1.0.5/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_video.py` & `pybaseutils-1.0.5/test_py/demo_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_voc_crop.py` & `pybaseutils-1.0.5/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_voc_vis.py` & `pybaseutils-1.0.5/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_word_similar.py` & `pybaseutils-1.0.5/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_worker1.py` & `pybaseutils-1.0.5/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/demo_worker2.py` & `pybaseutils-1.0.5/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/detector/demo.py` & `pybaseutils-1.0.5/test_py/detector/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/detector/detect_face_person.py` & `pybaseutils-1.0.5/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/detector/predet_labelme.py` & `pybaseutils-1.0.5/test_py/detector/predet_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/edit_distance/demo.py` & `pybaseutils-1.0.5/test_py/edit_distance/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/edit_distance/text_matching.py` & `pybaseutils-1.0.5/test_py/edit_distance/text_matching.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/edit_distance/text_utils.py` & `pybaseutils-1.0.5/test_py/edit_distance/text_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/flask_demo/server.py` & `pybaseutils-1.0.5/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/kafka_worker.py` & `pybaseutils-1.0.5/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/men_tracemalloc.py` & `pybaseutils-1.0.5/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/performance.py` & `pybaseutils-1.0.5/test_py/performance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/pose/human_pose.py` & `pybaseutils-1.0.5/test_py/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/registry/base.py` & `pybaseutils-1.0.5/test_py/registry/base.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/registry/component.py` & `pybaseutils-1.0.5/test_py/registry/component.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/registry/main.py` & `pybaseutils-1.0.5/test_py/registry/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.4/test_py/registry/register.py` & `pybaseutils-1.0.5/test_py/registry/register.py`

 * *Files identical despite different names*

