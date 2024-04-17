# Comparing `tmp/janim-0.4.0.tar.gz` & `tmp/janim-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-0.4.0.tar` & `janim-0.5.0.tar`

### file list

```diff
@@ -1,93 +1,97 @@
--rw-r--r--   0        0        0      164 2024-03-08 02:47:13.175046 janim-0.4.0/.gitignore
--rw-r--r--   0        0        0      961 2024-03-06 02:38:15.419027 janim-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0      398 2024-03-07 03:42:49.399574 janim-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-0.4.0/.vscode/tasks.json
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-0.4.0/LICENSE
--rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-0.4.0/README.md
--rw-r--r--   0        0        0       71 2024-03-26 15:04:45.600346 janim-0.4.0/janim/__init__.py
--rw-r--r--   0        0        0     8328 2024-03-14 06:39:26.694306 janim-0.4.0/janim/__main__.py
--rw-r--r--   0        0        0     4105 2024-03-26 14:54:35.892709 janim-0.4.0/janim/anims/animation.py
--rw-r--r--   0        0        0     5209 2024-03-08 02:47:13.199067 janim-0.4.0/janim/anims/composition.py
--rw-r--r--   0        0        0     5816 2024-03-14 08:41:07.949118 janim-0.4.0/janim/anims/creation.py
--rw-r--r--   0        0        0      855 2024-02-20 13:10:29.944561 janim-0.4.0/janim/anims/display.py
--rw-r--r--   0        0        0     3293 2024-03-14 06:39:26.710299 janim-0.4.0/janim/anims/fading.py
--rw-r--r--   0        0        0     1464 2024-03-14 06:39:26.710299 janim-0.4.0/janim/anims/rotation.py
--rw-r--r--   0        0        0    19250 2024-03-26 14:54:35.897697 janim-0.4.0/janim/anims/timeline.py
--rw-r--r--   0        0        0     8568 2024-03-26 14:54:35.902683 janim-0.4.0/janim/anims/transform.py
--rw-r--r--   0        0        0     9432 2024-03-14 08:01:57.787600 janim-0.4.0/janim/anims/updater.py
--rw-r--r--   0        0        0     4495 2024-02-20 13:10:29.952576 janim-0.4.0/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-0.4.0/janim/camera/camera_info.py
--rw-r--r--   0        0        0     8226 2024-03-26 14:54:35.906672 janim-0.4.0/janim/components/component.py
--rw-r--r--   0        0        0     2326 2024-03-14 06:39:26.718305 janim-0.4.0/janim/components/data.py
--rw-r--r--   0        0        0     2517 2024-03-26 14:54:35.911658 janim-0.4.0/janim/components/depth.py
--rw-r--r--   0        0        0     1279 2024-03-05 11:28:56.434384 janim-0.4.0/janim/components/image.py
--rw-r--r--   0        0        0    31519 2024-03-26 14:54:35.911658 janim-0.4.0/janim/components/points.py
--rw-r--r--   0        0        0     3024 2024-03-14 12:12:39.400689 janim-0.4.0/janim/components/radius.py
--rw-r--r--   0        0        0     8633 2024-03-26 14:54:35.912656 janim-0.4.0/janim/components/rgbas.py
--rw-r--r--   0        0        0    23584 2024-03-26 14:54:35.916644 janim-0.4.0/janim/components/vpoints.py
--rw-r--r--   0        0        0      171 2024-02-20 13:10:29.968656 janim-0.4.0/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-0.4.0/janim/constants/alignment.py
--rw-r--r--   0        0        0     1333 2024-02-20 13:10:29.970716 janim-0.4.0/janim/constants/colors.py
--rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-0.4.0/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-0.4.0/janim/constants/degrees.py
--rw-r--r--   0        0        0     5157 2024-03-28 08:26:28.364109 janim-0.4.0/janim/examples.py
--rw-r--r--   0        0        0     1721 2024-03-14 06:39:26.734309 janim-0.4.0/janim/exception.py
--rw-r--r--   0        0        0    27913 2024-03-26 14:54:35.921631 janim-0.4.0/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-0.4.0/janim/gui/application.py
--rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-0.4.0/janim/gui/export.png
--rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-0.4.0/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0      881 2024-02-20 13:10:29.978729 janim-0.4.0/janim/gui/glwidget.py
--rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-0.4.0/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8892 2024-03-14 06:39:26.742300 janim-0.4.0/janim/gui/selector.py
--rw-r--r--   0        0        0     1531 2024-03-26 14:54:35.929610 janim-0.4.0/janim/imports.py
--rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-0.4.0/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8823 2024-03-26 14:54:35.934597 janim-0.4.0/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-03-26 14:54:35.938586 janim-0.4.0/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-0.4.0/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8792 2024-03-23 03:08:17.235541 janim-0.4.0/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6497 2024-03-26 14:54:35.947562 janim-0.4.0/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     8130 2024-03-14 06:39:26.759952 janim-0.4.0/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5379 2024-03-14 06:39:26.922045 janim-0.4.0/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5315 2024-03-05 11:28:56.482378 janim-0.4.0/janim/items/image_item.py
--rw-r--r--   0        0        0    19385 2024-03-24 09:07:24.006701 janim-0.4.0/janim/items/item.py
--rw-r--r--   0        0        0     3397 2024-03-14 06:39:26.922045 janim-0.4.0/janim/items/points.py
--rw-r--r--   0        0        0     7379 2024-03-26 14:54:35.952548 janim-0.4.0/janim/items/relation.py
--rw-r--r--   0        0        0     6290 2024-03-14 06:39:26.922045 janim-0.4.0/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-0.4.0/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4077 2024-03-26 14:54:35.956538 janim-0.4.0/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     2629 2024-03-08 02:47:13.295042 janim-0.4.0/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-03-05 11:28:56.482378 janim-0.4.0/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    15525 2024-03-26 14:54:35.957535 janim-0.4.0/janim/items/text/text.py
--rw-r--r--   0        0        0     1064 2024-03-14 06:39:26.938042 janim-0.4.0/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5487 2024-03-26 14:54:35.961526 janim-0.4.0/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-0.4.0/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-03-06 03:25:06.445058 janim-0.4.0/janim/render/base.py
--rw-r--r--   0        0        0     4376 2024-03-08 02:47:13.303044 janim-0.4.0/janim/render/file_writer.py
--rw-r--r--   0        0        0     8944 2024-03-06 03:27:12.375792 janim-0.4.0/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-0.4.0/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-02-20 13:10:30.006723 janim-0.4.0/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-0.4.0/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-0.4.0/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-0.4.0/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-03-23 12:55:11.430379 janim-0.4.0/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-0.4.0/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0      857 2024-03-05 11:28:56.514381 janim-0.4.0/janim/render/texture.py
--rw-r--r--   0        0        0      950 2024-03-14 06:39:26.962043 janim-0.4.0/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-0.4.0/janim/utils/bezier.py
--rw-r--r--   0        0        0     3899 2024-03-23 12:41:22.536500 janim-0.4.0/janim/utils/config.py
--rw-r--r--   0        0        0      215 2024-02-20 13:10:30.018725 janim-0.4.0/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-0.4.0/janim/utils/dict_ops.py
--rw-r--r--   0        0        0      655 2024-03-08 02:47:13.303044 janim-0.4.0/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2402 2024-03-12 10:38:58.590837 janim-0.4.0/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-0.4.0/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-0.4.0/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-0.4.0/janim/utils/paths.py
--rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-0.4.0/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2008 2024-02-20 13:10:30.022729 janim-0.4.0/janim/utils/refresh.py
--rw-r--r--   0        0        0     8918 2024-03-07 06:40:50.078686 janim-0.4.0/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-0.4.0/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-0.4.0/janim/utils/space_ops.py
--rw-r--r--   0        0        0     1055 2024-03-26 14:54:35.973493 janim-0.4.0/janim/utils/unique_nparray.py
--rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-0.4.0/logo.png
--rw-r--r--   0        0        0      976 2024-03-26 14:54:35.974490 janim-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 janim-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      164 2024-03-08 02:47:13.175046 janim-0.5.0/.gitignore
+-rw-r--r--   0        0        0      961 2024-03-06 02:38:15.419027 janim-0.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      398 2024-03-07 03:42:49.399574 janim-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-0.5.0/.vscode/tasks.json
+-rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-0.5.0/LICENSE
+-rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-0.5.0/README.md
+-rw-r--r--   0        0        0       71 2024-04-17 04:01:00.033666 janim-0.5.0/janim/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-0.5.0/janim/__main__.py
+-rw-r--r--   0        0        0     4095 2024-04-17 03:59:08.847168 janim-0.5.0/janim/anims/animation.py
+-rw-r--r--   0        0        0     5417 2024-04-17 03:59:08.848161 janim-0.5.0/janim/anims/composition.py
+-rw-r--r--   0        0        0     5922 2024-04-17 03:59:08.848161 janim-0.5.0/janim/anims/creation.py
+-rw-r--r--   0        0        0      855 2024-02-20 13:10:29.944561 janim-0.5.0/janim/anims/display.py
+-rw-r--r--   0        0        0     3293 2024-03-14 06:39:26.710299 janim-0.5.0/janim/anims/fading.py
+-rw-r--r--   0        0        0     1484 2024-04-17 03:59:08.849160 janim-0.5.0/janim/anims/rotation.py
+-rw-r--r--   0        0        0    26747 2024-04-17 03:59:08.849160 janim-0.5.0/janim/anims/timeline.py
+-rw-r--r--   0        0        0     8590 2024-04-17 03:59:08.850373 janim-0.5.0/janim/anims/transform.py
+-rw-r--r--   0        0        0     9432 2024-03-14 08:01:57.787600 janim-0.5.0/janim/anims/updater.py
+-rw-r--r--   0        0        0     4495 2024-04-16 10:46:40.397643 janim-0.5.0/janim/camera/camera.py
+-rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-0.5.0/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6703 2024-04-17 03:59:08.851151 janim-0.5.0/janim/cli.py
+-rw-r--r--   0        0        0     8265 2024-04-17 03:59:08.851151 janim-0.5.0/janim/components/component.py
+-rw-r--r--   0        0        0     2326 2024-03-14 06:39:26.718305 janim-0.5.0/janim/components/data.py
+-rw-r--r--   0        0        0     2517 2024-03-26 14:54:35.911658 janim-0.5.0/janim/components/depth.py
+-rw-r--r--   0        0        0     1279 2024-03-05 11:28:56.434384 janim-0.5.0/janim/components/image.py
+-rw-r--r--   0        0        0    31519 2024-03-26 14:54:35.911658 janim-0.5.0/janim/components/points.py
+-rw-r--r--   0        0        0     3024 2024-03-14 12:12:39.400689 janim-0.5.0/janim/components/radius.py
+-rw-r--r--   0        0        0     8633 2024-03-26 14:54:35.912656 janim-0.5.0/janim/components/rgbas.py
+-rw-r--r--   0        0        0    23584 2024-03-26 14:54:35.916644 janim-0.5.0/janim/components/vpoints.py
+-rw-r--r--   0        0        0      171 2024-02-20 13:10:29.968656 janim-0.5.0/janim/constants/__init__.py
+-rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-0.5.0/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1333 2024-02-20 13:10:29.970716 janim-0.5.0/janim/constants/colors.py
+-rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-0.5.0/janim/constants/coord.py
+-rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-0.5.0/janim/constants/degrees.py
+-rw-r--r--   0        0        0     4806 2024-04-17 03:59:08.852148 janim-0.5.0/janim/examples.py
+-rw-r--r--   0        0        0     1721 2024-03-14 06:39:26.734309 janim-0.5.0/janim/exception.py
+-rw-r--r--   0        0        0    39434 2024-04-17 03:59:08.853145 janim-0.5.0/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-0.5.0/janim/gui/application.py
+-rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-0.5.0/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-0.5.0/janim/gui/export.png
+-rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-0.5.0/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0      845 2024-04-17 03:59:08.854142 janim-0.5.0/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      903 2024-04-17 03:59:08.854142 janim-0.5.0/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-0.5.0/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8892 2024-03-14 06:39:26.742300 janim-0.5.0/janim/gui/selector.py
+-rw-r--r--   0        0        0     1564 2024-04-17 03:59:08.854142 janim-0.5.0/janim/imports.py
+-rw-r--r--   0        0        0     4744 2024-04-17 03:59:08.855140 janim-0.5.0/janim/items/audio.py
+-rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-0.5.0/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8823 2024-03-26 14:54:35.934597 janim-0.5.0/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2165 2024-03-26 14:54:35.938586 janim-0.5.0/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-0.5.0/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8792 2024-03-23 03:08:17.235541 janim-0.5.0/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6497 2024-03-26 14:54:35.947562 janim-0.5.0/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     8130 2024-04-12 02:55:45.180361 janim-0.5.0/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5379 2024-03-14 06:39:26.922045 janim-0.5.0/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5315 2024-03-05 11:28:56.482378 janim-0.5.0/janim/items/image_item.py
+-rw-r--r--   0        0        0    19385 2024-03-24 09:07:24.006701 janim-0.5.0/janim/items/item.py
+-rw-r--r--   0        0        0     3397 2024-03-14 06:39:26.922045 janim-0.5.0/janim/items/points.py
+-rw-r--r--   0        0        0     7379 2024-03-26 14:54:35.952548 janim-0.5.0/janim/items/relation.py
+-rw-r--r--   0        0        0     6290 2024-03-14 06:39:26.922045 janim-0.5.0/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-0.5.0/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4072 2024-04-17 03:59:08.855140 janim-0.5.0/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-0.5.0/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       40 2024-03-05 11:28:56.482378 janim-0.5.0/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    15651 2024-04-17 03:59:08.856138 janim-0.5.0/janim/items/text/text.py
+-rw-r--r--   0        0        0     1064 2024-03-14 06:39:26.938042 janim-0.5.0/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5487 2024-03-26 14:54:35.961526 janim-0.5.0/janim/items/vitem.py
+-rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-0.5.0/janim/logger.py
+-rw-r--r--   0        0        0     3054 2024-03-06 03:25:06.445058 janim-0.5.0/janim/render/base.py
+-rw-r--r--   0        0        0     8944 2024-03-06 03:27:12.375792 janim-0.5.0/janim/render/impl.py
+-rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-0.5.0/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-0.5.0/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-0.5.0/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-0.5.0/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-0.5.0/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-0.5.0/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-0.5.0/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0      857 2024-03-05 11:28:56.514381 janim-0.5.0/janim/render/texture.py
+-rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-0.5.0/janim/render/writer.py
+-rw-r--r--   0        0        0      950 2024-03-14 06:39:26.962043 janim-0.5.0/janim/typing.py
+-rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-0.5.0/janim/utils/bezier.py
+-rw-r--r--   0        0        0     4156 2024-04-17 03:59:08.858135 janim-0.5.0/janim/utils/config.py
+-rw-r--r--   0        0        0      215 2024-02-20 13:10:30.018725 janim-0.5.0/janim/utils/data.py
+-rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-0.5.0/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0      657 2024-04-17 03:59:08.858135 janim-0.5.0/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2406 2024-04-17 03:59:08.859133 janim-0.5.0/janim/utils/font.py
+-rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-0.5.0/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-0.5.0/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-0.5.0/janim/utils/paths.py
+-rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-0.5.0/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2008 2024-02-20 13:10:30.022729 janim-0.5.0/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8918 2024-03-07 06:40:50.078686 janim-0.5.0/janim/utils/signal.py
+-rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-0.5.0/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-0.5.0/janim/utils/space_ops.py
+-rw-r--r--   0        0        0     1108 2024-04-17 03:59:08.859133 janim-0.5.0/janim/utils/unique_nparray.py
+-rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-0.5.0/logo.png
+-rw-r--r--   0        0        0     1018 2024-04-17 03:59:08.860128 janim-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-0.5.0/PKG-INFO
```

### Comparing `janim-0.4.0/.readthedocs.yaml` & `janim-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/LICENSE` & `janim-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/README.md` & `janim-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/__main__.py` & `janim-0.5.0/janim/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,19 @@
 import importlib.machinery
 import os
 import platform
 import subprocess as sp
 import time
-from argparse import ArgumentParser, Namespace
+from argparse import Namespace
 
 from janim.anims.timeline import Timeline
 from janim.exception import (EXITCODE_MODULE_NOT_FOUND, EXITCODE_NOT_FILE,
                              ExitException)
 from janim.logger import log
-from janim.utils.config import Config, default_config
-from janim.utils.file_ops import get_janim_dir
-
-
-def main() -> None:
-    parser = ArgumentParser(description='A library for simple animation effects')
-    parser.set_defaults(func=None)
-
-    sp = parser.add_subparsers()
-    run_parser(sp.add_parser('run', help='Run timeline(s) from specific namespace'))
-    write_parser(sp.add_parser('write', help='Generate video file(s) of timeline(s) from specific namesapce'))
-    examples_parser(sp.add_parser('examples', help='Show examples of janim'))
-
-    args = parser.parse_args()
-    if args.func is None:
-        parser.print_help()
-    else:
-        args.func(args)
-
-
-def render_args(parser: ArgumentParser) -> None:
-    parser.add_argument(
-        'filepath',
-        help='Path to file holding the python code for the timeline'
-    )
-    parser.add_argument(
-        'timeline_names',
-        nargs='*',
-        help='Name of the Timeline class you want to see'
-    )
-    parser.add_argument(
-        '-a', '--all',
-        action='store_true',
-        help='Render all timelines from a file'
-    )
-    parser.add_argument(
-        '-c', '--config',
-        nargs=2,
-        metavar=('key', 'value'),
-        action='append',
-        help='Override config'
-    )
-
-
-def run_parser(parser: ArgumentParser) -> None:
-    render_args(parser)
-    parser.add_argument(
-        '-i', '--interact',
-        action='store_true',
-        help='Enable the network socket for interacting'
-    )
-    parser.set_defaults(func=run)
-
-
-def write_parser(parser: ArgumentParser) -> None:
-    render_args(parser)
-    parser.add_argument(
-        '-o', '--open',
-        action='store_true',
-        help='Open the file after writing'
-    )
-    parser.add_argument(
-        '--format',
-        choices=['mp4', 'mov'],
-        default='mp4',
-        help='Format of the output file'
-    )
-    parser.set_defaults(func=write)
-
-
-def examples_parser(parser: ArgumentParser) -> None:
-    parser.set_defaults(filepath=os.path.join(get_janim_dir(), 'examples.py'))
-    parser.add_argument(
-        'timeline_names',
-        nargs='*',
-        help='Name of the example you want to see'
-    )
-    parser.set_defaults(all=None)
-    parser.set_defaults(config=None)
-    parser.set_defaults(func=run)
-    parser.set_defaults(interact=False)
+from janim.utils.config import default_config
 
 
 def run(args: Namespace) -> None:
     module = get_module(args.filepath)
     if module is None:
         return
     modify_default_config(args)
@@ -143,41 +63,57 @@
         return
     modify_default_config(args)
 
     timelines = extract_timelines_from_module(args, module)
     if not timelines:
         return
 
-    from janim.render.file_writer import FileWriter
+    from janim.render.writer import AudioWriter, VideoWriter
 
     log.info('======')
 
     built = [timeline().build() for timeline in timelines]
 
     log.info('======')
 
-    output_dir = os.path.normpath(Config.get.output_dir)
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
-
-    log.info(f'fps={Config.get.fps}')
-    log.info(f'resolution="{Config.get.pixel_width}x{Config.get.pixel_height}"')
-    log.info(f'output_dir="{output_dir}"')
-    log.info(f'format="{args.format}"')
+    both = not args.video and not args.audio
 
     log.info('======')
 
     for anim in built:
-        writer = FileWriter(anim)
-        writer.write_all(
-            os.path.join(Config.get.output_dir,
-                         f'{anim.timeline.__class__.__name__}.{args.format}')
-        )
-        if args.open and anim is built[-1]:
-            open_file(writer.final_file_path)
+        name = anim.timeline.__class__.__name__
+
+        output_dir = os.path.normpath(anim.cfg.output_dir)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+
+        if both or args.video:
+            log.info(f'fps={anim.cfg.fps}')
+            log.info(f'resolution="{anim.cfg.pixel_width}x{anim.cfg.pixel_height}"')
+            log.info(f'format="{args.format}"')
+        if both or args.audio:
+            log.info(f'audio_format="{args.audio_format}"')
+            log.info(f'audio_framerate="{anim.cfg.audio_framerate}"')
+        log.info(f'output_dir="{output_dir}"')
+
+        if both or args.video:
+            writer = VideoWriter(anim)
+            writer.write_all(
+                os.path.join(anim.cfg.output_dir,
+                             f'{name}.{args.format}')
+            )
+            if args.open and anim is built[-1]:
+                open_file(writer.final_file_path)
+
+        if (both or args.audio) and anim.timeline.has_audio():
+            writer = AudioWriter(anim)
+            writer.write_all(
+                os.path.join(anim.cfg.output_dir,
+                             f'{name}.{args.audio_format}')
+            )
 
     log.info('======')
 
 
 def modify_default_config(args: Namespace) -> None:
     if args.config:
         for key, value in args.config:
@@ -196,15 +132,17 @@
 
     module_name = file_name.replace(os.sep, ".").replace(".py", "")
     loader = importlib.machinery.SourceFileLoader(module_name, file_name)
     module = loader.load_module()
     return module
 
 
-def extract_timelines_from_module(args: Namespace, module) -> list[type[Timeline]]:
+def extract_timelines_from_module(args: Namespace, module) -> list[type['Timeline']]:
+    from janim.anims.timeline import Timeline
+
     timelines = []
     err = False
 
     if not args.all and args.timeline_names:
         for name in args.timeline_names:
             try:
                 timelines.append(module.__dict__[name])
@@ -229,19 +167,23 @@
 
         name_to_class = {}
         for idx, timeline_class in enumerate(classes, start=1):
             name = timeline_class.__name__
             print(f"{str(idx).zfill(max_digits)}: {name}")
             name_to_class[name] = timeline_class
 
-        user_input = input(
-            "\nThat module has multiple timelines, "
-            "which ones would you like to render?"
-            "\nTimeline Name or Number: "
-        )
+        try:
+            user_input = input(
+                "\nThat module has multiple timelines, "
+                "which ones would you like to render?"
+                "\nTimeline Name or Number: "
+            )
+        except KeyboardInterrupt:
+            user_input = ''
+
         for split_str in user_input.replace(' ', '').split(','):
             if not split_str:
                 continue
             if split_str.isnumeric():
                 idx = int(split_str) - 1
                 if 0 <= idx < len(classes):
                     timelines.append(classes[idx])
@@ -272,11 +214,7 @@
             commands.append("open")
 
         commands.append(file_path)
 
         FNULL = open(os.devnull, 'w')
         sp.call(commands, stdout=FNULL, stderr=sp.STDOUT)
         FNULL.close()
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `janim-0.4.0/janim/anims/animation.py` & `janim-0.5.0/janim/anims/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable
 
 from janim.components.depth import Cmpt_Depth
 from janim.utils.rate_functions import RateFunc, smooth
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:   # pragma: no cover
     from janim.anims.composition import AnimGroup
 
 
 @dataclass
 class TimeRange:
     at: float
     duration: float
 
     @property
     def end(self) -> float:
         return self.at + self.duration
 
+    def copy(self) -> TimeRange:
+        return TimeRange(self.at, self.duration)
+
 
 class Animation:
     '''
     动画基类
 
     - 创建一个从 ``at`` 持续至 ``at + duration`` 的动画
     - 指定 ``rate_func`` 可以设定插值函数，默认为 :meth:`janim.utils.rate_functions.smooth` 即平滑插值
@@ -44,22 +47,20 @@
 
         self.local_range = TimeRange(at, duration)
         self.global_range = None
         self.rate_func = rate_func
 
         self.render_call_list: list[RenderCall] = []
 
-    def set_global_range(self, at: float, duration: float | None = None) -> None:
+    def compute_global_range(self, at: float, duration: float) -> None:
         '''
-        设置在 :class:`~.Timeline` 上的时间范围
+        计算 :class:`~.Timeline` 上的时间范围
 
-        不需要手动设置，该方法是被 :meth:`~.AnimGroup.set_global_range` 调用以计算的
+        该方法是被 :meth:`~.AnimGroup.set_global_range` 调用以计算的
         '''
-        if duration is None:
-            duration = self.local_range.duration
         self.global_range = TimeRange(at, duration)
 
     def set_render_call_list(self, lst: list[RenderCall]) -> None:
         '''
         设置绘制调用，具体参考 :class:`RenderCall`
         '''
         self.render_call_list = sorted(lst, key=lambda x: x.depth, reverse=True)
```

### Comparing `janim-0.4.0/janim/anims/composition.py` & `janim-0.5.0/janim/anims/composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,217 +110,230 @@
 000006d0: 6578 7465 6e64 2861 6e69 6d2e 666c 6174  extend(anim.flat
 000006e0: 7465 6e28 2929 0d0a 2020 2020 2020 2020  ten())..        
 000006f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
 00000700: 2020 2020 2020 2020 2020 2072 6573 756c             resul
 00000710: 742e 6170 7065 6e64 2861 6e69 6d29 0d0a  t.append(anim)..
 00000720: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
 00000730: 2072 6573 756c 740d 0a0d 0a20 2020 2064   result....    d
-00000740: 6566 2073 6574 5f67 6c6f 6261 6c5f 7261  ef set_global_ra
-00000750: 6e67 6528 7365 6c66 2c20 6174 3a20 666c  nge(self, at: fl
-00000760: 6f61 742c 2064 7572 6174 696f 6e3a 2066  oat, duration: f
-00000770: 6c6f 6174 207c 204e 6f6e 6520 3d20 4e6f  loat | None = No
-00000780: 6e65 2920 2d3e 204e 6f6e 653a 0d0a 2020  ne) -> None:..  
-00000790: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-000007a0: 2020 20e8 aebe e7bd aee5 b9b6 e8ae a1e7     .............
-000007b0: ae97 e5ad 90e5 8aa8 e794 bbe7 9a84 e697  ................
-000007c0: b6e9 97b4 e88c 83e5 9bb4 0d0a 0d0a 2020  ..............  
-000007d0: 2020 2020 2020 e4b8 8de9 9c80 e8a6 81e6        ..........
-000007e0: 898b e58a a8e8 aebe e7bd aeef bc8c e8af  ................
-000007f0: a5e6 96b9 e6b3 95e6 98af e8a2 ab20 3a6d  ............. :m
-00000800: 6574 683a 607e 2e54 696d 656c 696e 652e  eth:`~.Timeline.
-00000810: 7072 6570 6172 6560 20e8 b083 e794 a8e4  prepare` .......
-00000820: bba5 e8ae a1e7 ae97 e79a 840d 0a20 2020  .............   
-00000830: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-00000840: 2020 7375 7065 7228 292e 7365 745f 676c    super().set_gl
-00000850: 6f62 616c 5f72 616e 6765 2861 742c 2064  obal_range(at, d
-00000860: 7572 6174 696f 6e29 0d0a 0d0a 2020 2020  uration)....    
-00000870: 2020 2020 6966 2064 7572 6174 696f 6e20      if duration 
-00000880: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00000890: 2020 2020 2020 6475 7261 7469 6f6e 203d        duration =
-000008a0: 2073 656c 662e 6c6f 6361 6c5f 7261 6e67   self.local_rang
-000008b0: 652e 6475 7261 7469 6f6e 0d0a 0d0a 2020  e.duration....  
-000008c0: 2020 2020 2020 6661 6374 6f72 203d 2064        factor = d
-000008d0: 7572 6174 696f 6e20 2f20 7365 6c66 2e6d  uration / self.m
-000008e0: 6178 740d 0a0d 0a20 2020 2020 2020 2066  axt....        f
-000008f0: 6f72 2061 6e69 6d20 696e 2073 656c 662e  or anim in self.
-00000900: 616e 696d 733a 0d0a 2020 2020 2020 2020  anims:..        
-00000910: 2020 2020 616e 696d 2e73 6574 5f67 6c6f      anim.set_glo
-00000920: 6261 6c5f 7261 6e67 6528 0d0a 2020 2020  bal_range(..    
-00000930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000940: 2e67 6c6f 6261 6c5f 7261 6e67 652e 6174  .global_range.at
-00000950: 202b 2061 6e69 6d2e 6c6f 6361 6c5f 7261   + anim.local_ra
-00000960: 6e67 652e 6174 202a 2066 6163 746f 722c  nge.at * factor,
-00000970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000980: 2020 616e 696d 2e6c 6f63 616c 5f72 616e    anim.local_ran
-00000990: 6765 2e64 7572 6174 696f 6e20 2a20 6661  ge.duration * fa
-000009a0: 6374 6f72 0d0a 2020 2020 2020 2020 2020  ctor..          
-000009b0: 2020 290d 0a0d 0a20 2020 2064 6566 2061    )....    def a
-000009c0: 6e69 6d5f 7072 655f 696e 6974 2873 656c  nim_pre_init(sel
-000009d0: 6629 202d 3e20 4e6f 6e65 3a0d 0a20 2020  f) -> None:..   
-000009e0: 2020 2020 2066 6f72 2061 6e69 6d20 696e       for anim in
-000009f0: 2073 656c 662e 616e 696d 733a 0d0a 2020   self.anims:..  
-00000a00: 2020 2020 2020 2020 2020 616e 696d 2e61            anim.a
-00000a10: 6e69 6d5f 7072 655f 696e 6974 2829 0d0a  nim_pre_init()..
-00000a20: 0d0a 2020 2020 6465 6620 616e 696d 5f69  ..    def anim_i
-00000a30: 6e69 7428 7365 6c66 2920 2d3e 204e 6f6e  nit(self) -> Non
-00000a40: 653a 0d0a 2020 2020 2020 2020 666f 7220  e:..        for 
-00000a50: 616e 696d 2069 6e20 7365 6c66 2e61 6e69  anim in self.ani
-00000a60: 6d73 3a0d 0a20 2020 2020 2020 2020 2020  ms:..           
-00000a70: 2061 6e69 6d2e 616e 696d 5f69 6e69 7428   anim.anim_init(
-00000a80: 290d 0a0d 0a20 2020 2064 6566 2067 6574  )....    def get
-00000a90: 5f61 6e69 6d5f 7428 7365 6c66 2c20 616c  _anim_t(self, al
-00000aa0: 7068 613a 2066 6c6f 6174 2c20 616e 696d  pha: float, anim
-00000ab0: 3a20 416e 696d 6174 696f 6e29 202d 3e20  : Animation) -> 
-00000ac0: 666c 6f61 743a 0d0a 2020 2020 2020 2020  float:..        
-00000ad0: 7265 7475 726e 2061 6c70 6861 202a 2073  return alpha * s
-00000ae0: 656c 662e 6d61 7874 202d 2061 6e69 6d2e  elf.maxt - anim.
-00000af0: 6c6f 6361 6c5f 7261 6e67 652e 6174 0d0a  local_range.at..
-00000b00: 0d0a 2020 2020 6465 6620 616e 696d 5f6f  ..    def anim_o
-00000b10: 6e5f 616c 7068 6128 7365 6c66 2c20 616c  n_alpha(self, al
-00000b20: 7068 613a 2066 6c6f 6174 2920 2d3e 204e  pha: float) -> N
-00000b30: 6f6e 653a 0d0a 2020 2020 2020 2020 2727  one:..        ''
-00000b40: 270d 0a20 2020 2020 2020 20e5 9ca8 e8af  '..        .....
-00000b50: a5e6 96b9 e6b3 95e4 b8ad efbc 8c3a 636c  .............:cl
-00000b60: 6173 733a 6041 6e69 6d47 726f 7570 6020  ass:`AnimGroup` 
-00000b70: e980 9ae8 bf87 2060 6061 6c70 6861 6060  ...... ``alpha``
-00000b80: 0d0a 2020 2020 2020 2020 e68d a2e7 ae97  ..        ......
-00000b90: e587 bae5 ad90 e58a a8e7 94bb e79a 8420  ............... 
-00000ba0: 6060 6c6f 6361 6c5f 7460 6020 e5b9 b6e8  ``local_t`` ....
-00000bb0: b083 e794 a8e5 ad90 e58a a8e7 94bb e79a  ................
-00000bc0: 8420 3a6d 6574 683a 607e 2e41 6e69 6d61  . :meth:`~.Anima
-00000bd0: 7469 6f6e 2e61 6e69 6d5f 6f6e 6020 e696  tion.anim_on` ..
-00000be0: b9e6 b395 0d0a 2020 2020 2020 2020 2727  ......        ''
-00000bf0: 270d 0a20 2020 2020 2020 2067 6c6f 6261  '..        globa
-00000c00: 6c5f 7420 3d20 7365 6c66 2e67 6c6f 6261  l_t = self.globa
-00000c10: 6c5f 745f 6374 782e 6765 7428 290d 0a0d  l_t_ctx.get()...
-00000c20: 0a20 2020 2020 2020 2066 6f72 2061 6e69  .        for ani
-00000c30: 6d20 696e 2073 656c 662e 616e 696d 733a  m in self.anims:
-00000c40: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-00000c50: 696d 5f74 203d 2073 656c 662e 6765 745f  im_t = self.get_
-00000c60: 616e 696d 5f74 2861 6c70 6861 2c20 616e  anim_t(alpha, an
-00000c70: 696d 290d 0a20 2020 2020 2020 2020 2020  im)..           
-00000c80: 2069 6620 616e 696d 2e67 6c6f 6261 6c5f   if anim.global_
-00000c90: 7261 6e67 652e 6174 203c 3d20 676c 6f62  range.at <= glob
-00000ca0: 616c 5f74 203c 2061 6e69 6d2e 676c 6f62  al_t < anim.glob
-00000cb0: 616c 5f72 616e 6765 2e65 6e64 3a0d 0a20  al_range.end:.. 
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00000cd0: 6e69 6d2e 616e 696d 5f6f 6e28 616e 696d  nim.anim_on(anim
-00000ce0: 5f74 290d 0a0d 0a0d 0a63 6c61 7373 2053  _t)......class S
-00000cf0: 7563 6365 7373 696f 6e28 416e 696d 4772  uccession(AnimGr
-00000d00: 6f75 7029 3a0d 0a20 2020 2027 2727 0d0a  oup):..    '''..
-00000d10: 2020 2020 e58a a8e7 94bb e99b 86e5 9088      ............
-00000d20: efbc 88e9 a1ba e5ba 8fe6 89a7 e8a1 8cef  ................
-00000d30: bc89 0d0a 0d0a 2020 2020 2d20 e4bc 9ae5  ......    - ....
-00000d40: b086 e4bc a0e5 85a5 e79a 84e5 8aa8 e794  ................
-00000d50: bbe4 be9d e6ac a1e6 89a7 e8a1 8cef bc8c  ................
-00000d60: e4b8 8de5 b9b6 e8a1 8c0d 0a20 2020 202d  ...........    -
-00000d70: 20e5 8faf e4bb a5e4 bca0 e585 a520 6062   ............ `b
-00000d80: 7566 6660 20e6 8c87 e5ae 9ae5 898d e590  uff` ...........
-00000d90: 8ee5 8aa8 e794 bbe4 b8ad e997 b4e7 9a84  ................
-00000da0: e7a9 bae7 99bd e697 b6e9 97b4 0d0a 2020  ..............  
-00000db0: 2020 2d20 e585 b6e4 bd99 e4b8 8e20 6041    - ......... `A
-00000dc0: 6e69 6d47 726f 7570 6020 e79b b8e5 908c  nimGroup` ......
-00000dd0: 0d0a 0d0a 2020 2020 e697 b6e9 97b4 e7a4  ....    ........
-00000de0: bae4 be8b efbc 9a0d 0a0d 0a20 2020 202e  ...........    .
-00000df0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00000e00: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-00000e10: 2053 7563 6365 7373 696f 6e28 0d0a 2020   Succession(..  
-00000e20: 2020 2020 2020 2020 2020 416e 696d 3128            Anim1(
-00000e30: 6475 7261 7469 6f6e 3d33 292c 0d0a 2020  duration=3),..  
-00000e40: 2020 2020 2020 2020 2020 416e 696d 3228            Anim2(
-00000e50: 6475 7261 7469 6f6e 3d34 290d 0a20 2020  duration=4)..   
-00000e60: 2020 2020 2029 2023 2041 6e69 6d31 20e5       ) # Anim1 .
-00000e70: 9ca8 2030 7e33 7320 e689 a7e8 a18c efbc  .. 0~3s ........
-00000e80: 8c41 6e69 6d32 20e5 9ca8 2033 7e37 7320  .Anim2 ... 3~7s 
-00000e90: e689 a7e8 a18c 0d0a 0d0a 2020 2020 2020  ..........      
-00000ea0: 2020 5375 6363 6573 7369 6f6e 280d 0a20    Succession(.. 
-00000eb0: 2020 2020 2020 2020 2020 2041 6e69 6d31             Anim1
-00000ec0: 2864 7572 6174 696f 6e3d 3229 2c0d 0a20  (duration=2),.. 
-00000ed0: 2020 2020 2020 2020 2020 2041 6e69 6d32             Anim2
-00000ee0: 2861 743d 312c 2064 7572 6174 696f 6e3d  (at=1, duration=
-00000ef0: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
-00000f00: 2041 6e69 6d33 2861 743d 302e 352c 2064   Anim3(at=0.5, d
-00000f10: 7572 6174 696f 6e3d 3229 0d0a 2020 2020  uration=2)..    
-00000f20: 2020 2020 2920 2320 416e 696d 3120 e59c      ) # Anim1 ..
-00000f30: a820 307e 3273 20e6 89a7 e8a1 8cef bc8c  . 0~2s .........
-00000f40: 416e 696d 3220 e59c a820 337e 3573 20e6  Anim2 ... 3~5s .
-00000f50: 89a7 e8a1 8cef bc8c 416e 696d 3320 e59c  ........Anim3 ..
-00000f60: a820 352e 357e 372e 3573 20e6 89a7 e8a1  . 5.5~7.5s .....
-00000f70: 8c0d 0a0d 0a20 2020 2020 2020 2053 7563  .....        Suc
-00000f80: 6365 7373 696f 6e28 0d0a 2020 2020 2020  cession(..      
-00000f90: 2020 2020 2020 416e 696d 3128 6475 7261        Anim1(dura
-00000fa0: 7469 6f6e 3d32 292c 0d0a 2020 2020 2020  tion=2),..      
-00000fb0: 2020 2020 2020 416e 696d 3228 6475 7261        Anim2(dura
-00000fc0: 7469 6f6e 3d32 292c 0d0a 2020 2020 2020  tion=2),..      
-00000fd0: 2020 2020 2020 416e 696d 3328 6475 7261        Anim3(dura
-00000fe0: 7469 6f6e 3d32 292c 0d0a 2020 2020 2020  tion=2),..      
-00000ff0: 2020 2020 2020 6275 6666 3d30 2e35 0d0a        buff=0.5..
-00001000: 2020 2020 2020 2020 2920 2320 416e 696d          ) # Anim
-00001010: 3120 e59c a820 307e 3273 20e6 89a7 e8a1  1 ... 0~2s .....
-00001020: 8cef bc8c 416e 696d 3220 e59c a820 322e  ....Anim2 ... 2.
-00001030: 357e 342e 3573 20e6 89a7 e8a1 8cef bc8c  5~4.5s .........
-00001040: 416e 696d 3320 e59c a820 357e 3773 20e6  Anim3 ... 5~7s .
-00001050: 89a7 e8a1 8c0d 0a20 2020 2027 2727 0d0a  .......    '''..
-00001060: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001070: 2873 656c 662c 202a 616e 696d 733a 2041  (self, *anims: A
-00001080: 6e69 6d61 7469 6f6e 2c20 6275 6666 3a20  nimation, buff: 
-00001090: 666c 6f61 7420 3d20 302c 202a 2a6b 7761  float = 0, **kwa
-000010a0: 7267 7329 3a0d 0a20 2020 2020 2020 2065  rgs):..        e
-000010b0: 6e64 5f74 696d 6520 3d20 300d 0a20 2020  nd_time = 0..   
-000010c0: 2020 2020 2066 6f72 2061 6e69 6d20 696e       for anim in
-000010d0: 2061 6e69 6d73 3a0d 0a20 2020 2020 2020   anims:..       
-000010e0: 2020 2020 2061 6e69 6d2e 6c6f 6361 6c5f       anim.local_
-000010f0: 7261 6e67 652e 6174 202b 3d20 656e 645f  range.at += end_
-00001100: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-00001110: 2020 656e 645f 7469 6d65 203d 2061 6e69    end_time = ani
-00001120: 6d2e 6c6f 6361 6c5f 7261 6e67 652e 656e  m.local_range.en
-00001130: 6420 2b20 6275 6666 0d0a 2020 2020 2020  d + buff..      
-00001140: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00001150: 5f5f 282a 616e 696d 732c 202a 2a6b 7761  __(*anims, **kwa
-00001160: 7267 7329 0d0a 0d0a 0d0a 636c 6173 7320  rgs)......class 
-00001170: 416c 6967 6e65 6428 416e 696d 4772 6f75  Aligned(AnimGrou
-00001180: 7029 3a0d 0a20 2020 2027 2727 0d0a 2020  p):..    '''..  
-00001190: 2020 e58a a8e7 94bb e99b 86e5 9088 efbc    ..............
-000011a0: 88e5 b9b6 e588 97e5 afb9 e9bd 90e6 89a7  ................
-000011b0: e8a1 8cef bc89 0d0a 0d0a 2020 2020 e697  ..........    ..
-000011c0: b6e9 97b4 e7a4 bae4 be8b efbc 9a0d 0a0d  ................
-000011d0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-000011e0: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
-000011f0: 2020 2020 2020 2041 6c69 676e 6564 280d         Aligned(.
-00001200: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-00001210: 6d31 2864 7572 6174 696f 6e3d 3129 2c0d  m1(duration=1),.
-00001220: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-00001230: 6d32 2864 7572 6174 696f 6e3d 3229 0d0a  m2(duration=2)..
-00001240: 2020 2020 2020 2020 2920 2320 416e 696d          ) # Anim
-00001250: 3120 e592 8c20 416e 696d 3220 e983 bde5  1 ... Anim2 ....
-00001260: 9ca8 2030 7e32 7320 e689 a7e8 a18c 0d0a  .. 0~2s ........
-00001270: 0d0a 2020 2020 2020 2020 416c 6967 6e65  ..        Aligne
-00001280: 6428 0d0a 2020 2020 2020 2020 2020 2020  d(..            
-00001290: 416e 696d 3128 6475 7261 7469 6f6e 3d31  Anim1(duration=1
-000012a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000012b0: 416e 696d 3228 6475 7261 7469 6f6e 3d32  Anim2(duration=2
-000012c0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000012d0: 6475 7261 7469 6f6e 3d34 0d0a 2020 2020  duration=4..    
-000012e0: 2020 2020 2920 2320 416e 696d 3120 e592      ) # Anim1 ..
-000012f0: 8c20 416e 696d 3220 e983 bde5 9ca8 2030  . Anim2 ...... 0
-00001300: 7e34 7320 e689 a7e8 a18c 0d0a 2020 2020  ~4s ........    
-00001310: 2727 270d 0a20 2020 2064 6566 205f 5f69  '''..    def __i
-00001320: 6e69 745f 5f28 2a61 6e69 6d73 3a20 416e  nit__(*anims: An
-00001330: 696d 6174 696f 6e2c 202a 2a6b 7761 7267  imation, **kwarg
-00001340: 7329 3a0d 0a20 2020 2020 2020 206d 6178  s):..        max
-00001350: 7420 3d20 6d61 7828 616e 696d 2e6c 6f63  t = max(anim.loc
-00001360: 616c 5f72 616e 6765 2e65 6e64 2066 6f72  al_range.end for
-00001370: 2061 6e69 6d20 696e 2061 6e69 6d73 290d   anim in anims).
-00001380: 0a20 2020 2020 2020 2066 6f72 2061 6e69  .        for ani
-00001390: 6d20 696e 2061 6e69 6d73 3a0d 0a20 2020  m in anims:..   
-000013a0: 2020 2020 2020 2020 2066 6163 746f 7220           factor 
-000013b0: 3d20 616e 696d 2e6c 6f63 616c 5f72 616e  = anim.local_ran
-000013c0: 6765 2e65 6e64 202f 206d 6178 740d 0a20  ge.end / maxt.. 
-000013d0: 2020 2020 2020 2020 2020 2061 6e69 6d2e             anim.
-000013e0: 6c6f 6361 6c5f 7261 6e67 652e 6174 202a  local_range.at *
-000013f0: 3d20 6661 6374 6f72 0d0a 2020 2020 2020  = factor..      
-00001400: 2020 2020 2020 616e 696d 2e6c 6f63 616c        anim.local
-00001410: 5f72 616e 6765 2e64 7572 6174 696f 6e20  _range.duration 
-00001420: 2a3d 2066 6163 746f 720d 0a0d 0a20 2020  *= factor....   
-00001430: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001440: 6e69 745f 5f28 2a61 6e69 6d73 2c20 2a2a  nit__(*anims, **
-00001450: 6b77 6172 6773 290d 0a                   kwargs)..
+00000740: 6566 2063 6f6d 7075 7465 5f67 6c6f 6261  ef compute_globa
+00000750: 6c5f 7261 6e67 6528 7365 6c66 2c20 6174  l_range(self, at
+00000760: 3a20 666c 6f61 742c 2064 7572 6174 696f  : float, duratio
+00000770: 6e3a 2066 6c6f 6174 2920 2d3e 204e 6f6e  n: float) -> Non
+00000780: 653a 0d0a 2020 2020 2020 2020 2727 270d  e:..        '''.
+00000790: 0a20 2020 2020 2020 20e8 aea1 e7ae 97e5  .        .......
+000007a0: ad90 e58a a8e7 94bb e79a 84e6 97b6 e997  ................
+000007b0: b4e8 8c83 e59b b40d 0a0d 0a20 2020 2020  ...........     
+000007c0: 2020 20e8 afa5 e696 b9e6 b395 e698 afe8     .............
+000007d0: a2ab 203a 6d65 7468 3a60 7e2e 5469 6d65  .. :meth:`~.Time
+000007e0: 6c69 6e65 2e70 7265 7061 7265 6020 e8b0  line.prepare` ..
+000007f0: 83e7 94a8 e4bb a5e8 aea1 e7ae 97e7 9a84  ................
+00000800: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00000810: 2020 2020 2020 2073 7570 6572 2829 2e63         super().c
+00000820: 6f6d 7075 7465 5f67 6c6f 6261 6c5f 7261  ompute_global_ra
+00000830: 6e67 6528 6174 2c20 6475 7261 7469 6f6e  nge(at, duration
+00000840: 290d 0a0d 0a20 2020 2020 2020 2066 6163  )....        fac
+00000850: 746f 7220 3d20 6475 7261 7469 6f6e 202f  tor = duration /
+00000860: 2073 656c 662e 6d61 7874 0d0a 0d0a 2020   self.maxt....  
+00000870: 2020 2020 2020 666f 7220 616e 696d 2069        for anim i
+00000880: 6e20 7365 6c66 2e61 6e69 6d73 3a0d 0a20  n self.anims:.. 
+00000890: 2020 2020 2020 2020 2020 2061 6e69 6d2e             anim.
+000008a0: 636f 6d70 7574 655f 676c 6f62 616c 5f72  compute_global_r
+000008b0: 616e 6765 280d 0a20 2020 2020 2020 2020  ange(..         
+000008c0: 2020 2020 2020 2073 656c 662e 676c 6f62         self.glob
+000008d0: 616c 5f72 616e 6765 2e61 7420 2b20 616e  al_range.at + an
+000008e0: 696d 2e6c 6f63 616c 5f72 616e 6765 2e61  im.local_range.a
+000008f0: 7420 2a20 6661 6374 6f72 2c0d 0a20 2020  t * factor,..   
+00000900: 2020 2020 2020 2020 2020 2020 2061 6e69               ani
+00000910: 6d2e 6c6f 6361 6c5f 7261 6e67 652e 6475  m.local_range.du
+00000920: 7261 7469 6f6e 202a 2066 6163 746f 720d  ration * factor.
+00000930: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00000940: 0d0a 2020 2020 6465 6620 616e 696d 5f70  ..    def anim_p
+00000950: 7265 5f69 6e69 7428 7365 6c66 2920 2d3e  re_init(self) ->
+00000960: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00000970: 666f 7220 616e 696d 2069 6e20 7365 6c66  for anim in self
+00000980: 2e61 6e69 6d73 3a0d 0a20 2020 2020 2020  .anims:..       
+00000990: 2020 2020 2061 6e69 6d2e 616e 696d 5f70       anim.anim_p
+000009a0: 7265 5f69 6e69 7428 290d 0a0d 0a20 2020  re_init()....   
+000009b0: 2064 6566 2061 6e69 6d5f 696e 6974 2873   def anim_init(s
+000009c0: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
+000009d0: 2020 2020 2020 2066 6f72 2061 6e69 6d20         for anim 
+000009e0: 696e 2073 656c 662e 616e 696d 733a 0d0a  in self.anims:..
+000009f0: 2020 2020 2020 2020 2020 2020 616e 696d              anim
+00000a00: 2e61 6e69 6d5f 696e 6974 2829 0d0a 0d0a  .anim_init()....
+00000a10: 2020 2020 6465 6620 6765 745f 616e 696d      def get_anim
+00000a20: 5f74 2873 656c 662c 2061 6c70 6861 3a20  _t(self, alpha: 
+00000a30: 666c 6f61 742c 2061 6e69 6d3a 2041 6e69  float, anim: Ani
+00000a40: 6d61 7469 6f6e 2920 2d3e 2066 6c6f 6174  mation) -> float
+00000a50: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00000a60: 6e20 616c 7068 6120 2a20 7365 6c66 2e6d  n alpha * self.m
+00000a70: 6178 7420 2d20 616e 696d 2e6c 6f63 616c  axt - anim.local
+00000a80: 5f72 616e 6765 2e61 740d 0a0d 0a20 2020  _range.at....   
+00000a90: 2064 6566 2061 6e69 6d5f 6f6e 5f61 6c70   def anim_on_alp
+00000aa0: 6861 2873 656c 662c 2061 6c70 6861 3a20  ha(self, alpha: 
+00000ab0: 666c 6f61 7429 202d 3e20 4e6f 6e65 3a0d  float) -> None:.
+00000ac0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
+00000ad0: 2020 2020 2020 e59c a8e8 afa5 e696 b9e6        ..........
+00000ae0: b395 e4b8 adef bc8c 3a63 6c61 7373 3a60  ........:class:`
+00000af0: 416e 696d 4772 6f75 7060 20e9 809a e8bf  AnimGroup` .....
+00000b00: 8720 6060 616c 7068 6160 600d 0a20 2020  . ``alpha``..   
+00000b10: 2020 2020 20e6 8da2 e7ae 97e5 87ba e5ad       ...........
+00000b20: 90e5 8aa8 e794 bbe7 9a84 2060 606c 6f63  .......... ``loc
+00000b30: 616c 5f74 6060 20e5 b9b6 e8b0 83e7 94a8  al_t`` .........
+00000b40: e5ad 90e5 8aa8 e794 bbe7 9a84 203a 6d65  ............ :me
+00000b50: 7468 3a60 7e2e 416e 696d 6174 696f 6e2e  th:`~.Animation.
+00000b60: 616e 696d 5f6f 6e60 20e6 96b9 e6b3 950d  anim_on` .......
+00000b70: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
+00000b80: 2020 2020 2020 676c 6f62 616c 5f74 203d        global_t =
+00000b90: 2073 656c 662e 676c 6f62 616c 5f74 5f63   self.global_t_c
+00000ba0: 7478 2e67 6574 2829 0d0a 0d0a 2020 2020  tx.get()....    
+00000bb0: 2020 2020 666f 7220 616e 696d 2069 6e20      for anim in 
+00000bc0: 7365 6c66 2e61 6e69 6d73 3a0d 0a20 2020  self.anims:..   
+00000bd0: 2020 2020 2020 2020 2061 6e69 6d5f 7420           anim_t 
+00000be0: 3d20 7365 6c66 2e67 6574 5f61 6e69 6d5f  = self.get_anim_
+00000bf0: 7428 616c 7068 612c 2061 6e69 6d29 0d0a  t(alpha, anim)..
+00000c00: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00000c10: 6e69 6d2e 676c 6f62 616c 5f72 616e 6765  nim.global_range
+00000c20: 2e61 7420 3c3d 2067 6c6f 6261 6c5f 7420  .at <= global_t 
+00000c30: 3c20 616e 696d 2e67 6c6f 6261 6c5f 7261  < anim.global_ra
+00000c40: 6e67 652e 656e 643a 0d0a 2020 2020 2020  nge.end:..      
+00000c50: 2020 2020 2020 2020 2020 616e 696d 2e61            anim.a
+00000c60: 6e69 6d5f 6f6e 2861 6e69 6d5f 7429 0d0a  nim_on(anim_t)..
+00000c70: 0d0a 0d0a 636c 6173 7320 5375 6363 6573  ....class Succes
+00000c80: 7369 6f6e 2841 6e69 6d47 726f 7570 293a  sion(AnimGroup):
+00000c90: 0d0a 2020 2020 2727 270d 0a20 2020 20e5  ..    '''..    .
+00000ca0: 8aa8 e794 bbe9 9b86 e590 88ef bc88 e9a1  ................
+00000cb0: bae5 ba8f e689 a7e8 a18c efbc 890d 0a0d  ................
+00000cc0: 0a20 2020 202d 20e4 bc9a e5b0 86e4 bca0  .    - .........
+00000cd0: e585 a5e7 9a84 e58a a8e7 94bb e4be 9de6  ................
+00000ce0: aca1 e689 a7e8 a18c efbc 8ce4 b88d e5b9  ................
+00000cf0: b6e8 a18c 0d0a 2020 2020 2d20 e58f afe4  ......    - ....
+00000d00: bba5 e4bc a0e5 85a5 2060 6275 6666 6020  ........ `buff` 
+00000d10: e68c 87e5 ae9a e589 8de5 908e e58a a8e7  ................
+00000d20: 94bb e4b8 ade9 97b4 e79a 84e7 a9ba e799  ................
+00000d30: bde6 97b6 e997 b40d 0a20 2020 202d 20e5  .........    - .
+00000d40: 85b6 e4bd 99e4 b88e 2060 416e 696d 4772  ........ `AnimGr
+00000d50: 6f75 7060 20e7 9bb8 e590 8c0d 0a0d 0a20  oup` .......... 
+00000d60: 2020 20e6 97b6 e997 b4e7 a4ba e4be 8bef     .............
+00000d70: bc9a 0d0a 0d0a 2020 2020 2e2e 2063 6f64  ......    .. cod
+00000d80: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+00000d90: 0d0a 0d0a 2020 2020 2020 2020 5375 6363  ....        Succ
+00000da0: 6573 7369 6f6e 280d 0a20 2020 2020 2020  ession(..       
+00000db0: 2020 2020 2041 6e69 6d31 2864 7572 6174       Anim1(durat
+00000dc0: 696f 6e3d 3329 2c0d 0a20 2020 2020 2020  ion=3),..       
+00000dd0: 2020 2020 2041 6e69 6d32 2864 7572 6174       Anim2(durat
+00000de0: 696f 6e3d 3429 0d0a 2020 2020 2020 2020  ion=4)..        
+00000df0: 2920 2320 416e 696d 3120 e59c a820 307e  ) # Anim1 ... 0~
+00000e00: 3373 20e6 89a7 e8a1 8cef bc8c 416e 696d  3s .........Anim
+00000e10: 3220 e59c a820 337e 3773 20e6 89a7 e8a1  2 ... 3~7s .....
+00000e20: 8c0d 0a0d 0a20 2020 2020 2020 2053 7563  .....        Suc
+00000e30: 6365 7373 696f 6e28 0d0a 2020 2020 2020  cession(..      
+00000e40: 2020 2020 2020 416e 696d 3128 6475 7261        Anim1(dura
+00000e50: 7469 6f6e 3d32 292c 0d0a 2020 2020 2020  tion=2),..      
+00000e60: 2020 2020 2020 416e 696d 3228 6174 3d31        Anim2(at=1
+00000e70: 2c20 6475 7261 7469 6f6e 3d32 292c 0d0a  , duration=2),..
+00000e80: 2020 2020 2020 2020 2020 2020 416e 696d              Anim
+00000e90: 3328 6174 3d30 2e35 2c20 6475 7261 7469  3(at=0.5, durati
+00000ea0: 6f6e 3d32 290d 0a20 2020 2020 2020 2029  on=2)..        )
+00000eb0: 2023 2041 6e69 6d31 20e5 9ca8 2030 7e32   # Anim1 ... 0~2
+00000ec0: 7320 e689 a7e8 a18c efbc 8c41 6e69 6d32  s .........Anim2
+00000ed0: 20e5 9ca8 2033 7e35 7320 e689 a7e8 a18c   ... 3~5s ......
+00000ee0: efbc 8c41 6e69 6d33 20e5 9ca8 2035 2e35  ...Anim3 ... 5.5
+00000ef0: 7e37 2e35 7320 e689 a7e8 a18c 0d0a 0d0a  ~7.5s ..........
+00000f00: 2020 2020 2020 2020 5375 6363 6573 7369          Successi
+00000f10: 6f6e 280d 0a20 2020 2020 2020 2020 2020  on(..           
+00000f20: 2041 6e69 6d31 2864 7572 6174 696f 6e3d   Anim1(duration=
+00000f30: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
+00000f40: 2041 6e69 6d32 2864 7572 6174 696f 6e3d   Anim2(duration=
+00000f50: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
+00000f60: 2041 6e69 6d33 2864 7572 6174 696f 6e3d   Anim3(duration=
+00000f70: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
+00000f80: 2062 7566 663d 302e 350d 0a20 2020 2020   buff=0.5..     
+00000f90: 2020 2029 2023 2041 6e69 6d31 20e5 9ca8     ) # Anim1 ...
+00000fa0: 2030 7e32 7320 e689 a7e8 a18c efbc 8c41   0~2s .........A
+00000fb0: 6e69 6d32 20e5 9ca8 2032 2e35 7e34 2e35  nim2 ... 2.5~4.5
+00000fc0: 7320 e689 a7e8 a18c efbc 8c41 6e69 6d33  s .........Anim3
+00000fd0: 20e5 9ca8 2035 7e37 7320 e689 a7e8 a18c   ... 5~7s ......
+00000fe0: 0d0a 2020 2020 2727 270d 0a20 2020 2064  ..    '''..    d
+00000ff0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001000: 2c20 2a61 6e69 6d73 3a20 416e 696d 6174  , *anims: Animat
+00001010: 696f 6e2c 2062 7566 663a 2066 6c6f 6174  ion, buff: float
+00001020: 203d 2030 2c20 2a2a 6b77 6172 6773 293a   = 0, **kwargs):
+00001030: 0d0a 2020 2020 2020 2020 656e 645f 7469  ..        end_ti
+00001040: 6d65 203d 2030 0d0a 2020 2020 2020 2020  me = 0..        
+00001050: 666f 7220 616e 696d 2069 6e20 616e 696d  for anim in anim
+00001060: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001070: 616e 696d 2e6c 6f63 616c 5f72 616e 6765  anim.local_range
+00001080: 2e61 7420 2b3d 2065 6e64 5f74 696d 650d  .at += end_time.
+00001090: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+000010a0: 5f74 696d 6520 3d20 616e 696d 2e6c 6f63  _time = anim.loc
+000010b0: 616c 5f72 616e 6765 2e65 6e64 202b 2062  al_range.end + b
+000010c0: 7566 660d 0a20 2020 2020 2020 2073 7570  uff..        sup
+000010d0: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a61  er().__init__(*a
+000010e0: 6e69 6d73 2c20 2a2a 6b77 6172 6773 290d  nims, **kwargs).
+000010f0: 0a0d 0a0d 0a63 6c61 7373 2041 6c69 676e  .....class Align
+00001100: 6564 2841 6e69 6d47 726f 7570 293a 0d0a  ed(AnimGroup):..
+00001110: 2020 2020 2727 270d 0a20 2020 20e5 8aa8      '''..    ...
+00001120: e794 bbe9 9b86 e590 88ef bc88 e5b9 b6e5  ................
+00001130: 8897 e5af b9e9 bd90 e689 a7e8 a18c efbc  ................
+00001140: 890d 0a0d 0a20 2020 20e6 97b6 e997 b4e7  .....    .......
+00001150: a4ba e4be 8bef bc9a 0d0a 0d0a 2020 2020  ............    
+00001160: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00001170: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
+00001180: 2020 416c 6967 6e65 6428 0d0a 2020 2020    Aligned(..    
+00001190: 2020 2020 2020 2020 416e 696d 3128 6475          Anim1(du
+000011a0: 7261 7469 6f6e 3d31 292c 0d0a 2020 2020  ration=1),..    
+000011b0: 2020 2020 2020 2020 416e 696d 3228 6475          Anim2(du
+000011c0: 7261 7469 6f6e 3d32 290d 0a20 2020 2020  ration=2)..     
+000011d0: 2020 2029 2023 2041 6e69 6d31 20e5 928c     ) # Anim1 ...
+000011e0: 2041 6e69 6d32 20e9 83bd e59c a820 307e   Anim2 ...... 0~
+000011f0: 3273 20e6 89a7 e8a1 8c0d 0a0d 0a20 2020  2s ..........   
+00001200: 2020 2020 2041 6c69 676e 6564 280d 0a20       Aligned(.. 
+00001210: 2020 2020 2020 2020 2020 2041 6e69 6d31             Anim1
+00001220: 2864 7572 6174 696f 6e3d 3129 2c0d 0a20  (duration=1),.. 
+00001230: 2020 2020 2020 2020 2020 2041 6e69 6d32             Anim2
+00001240: 2864 7572 6174 696f 6e3d 3229 2c0d 0a20  (duration=2),.. 
+00001250: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+00001260: 696f 6e3d 340d 0a20 2020 2020 2020 2029  ion=4..        )
+00001270: 2023 2041 6e69 6d31 20e5 928c 2041 6e69   # Anim1 ... Ani
+00001280: 6d32 20e9 83bd e59c a820 307e 3473 20e6  m2 ...... 0~4s .
+00001290: 89a7 e8a1 8c0d 0a20 2020 2027 2727 0d0a  .......    '''..
+000012a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000012b0: 2873 656c 662c 202a 616e 696d 733a 2041  (self, *anims: A
+000012c0: 6e69 6d61 7469 6f6e 2c20 6475 7261 7469  nimation, durati
+000012d0: 6f6e 3a20 666c 6f61 7420 7c20 4e6f 6e65  on: float | None
+000012e0: 203d 204e 6f6e 652c 202a 2a6b 7761 7267   = None, **kwarg
+000012f0: 7329 3a0d 0a20 2020 2020 2020 2069 6620  s):..        if 
+00001300: 6475 7261 7469 6f6e 2069 7320 4e6f 6e65  duration is None
+00001310: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+00001320: 7572 6174 696f 6e20 3d20 6d61 7828 616e  uration = max(an
+00001330: 696d 2e6c 6f63 616c 5f72 616e 6765 2e65  im.local_range.e
+00001340: 6e64 2066 6f72 2061 6e69 6d20 696e 2061  nd for anim in a
+00001350: 6e69 6d73 290d 0a0d 0a20 2020 2020 2020  nims)....       
+00001360: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00001370: 5f28 2a61 6e69 6d73 2c20 6475 7261 7469  _(*anims, durati
+00001380: 6f6e 3d64 7572 6174 696f 6e2c 202a 2a6b  on=duration, **k
+00001390: 7761 7267 7329 0d0a 0d0a 2020 2020 6465  wargs)....    de
+000013a0: 6620 636f 6d70 7574 655f 676c 6f62 616c  f compute_global
+000013b0: 5f72 616e 6765 2873 656c 662c 2061 743a  _range(self, at:
+000013c0: 2066 6c6f 6174 2c20 6475 7261 7469 6f6e   float, duration
+000013d0: 3a20 666c 6f61 7429 202d 3e20 4e6f 6e65  : float) -> None
+000013e0: 3a0d 0a20 2020 2020 2020 2041 6e69 6d61  :..        Anima
+000013f0: 7469 6f6e 2e63 6f6d 7075 7465 5f67 6c6f  tion.compute_glo
+00001400: 6261 6c5f 7261 6e67 6528 7365 6c66 2c20  bal_range(self, 
+00001410: 6174 2c20 6475 7261 7469 6f6e 290d 0a0d  at, duration)...
+00001420: 0a20 2020 2020 2020 2066 6f72 2061 6e69  .        for ani
+00001430: 6d20 696e 2073 656c 662e 616e 696d 733a  m in self.anims:
+00001440: 0d0a 2020 2020 2020 2020 2020 2020 6661  ..            fa
+00001450: 6374 6f72 203d 2064 7572 6174 696f 6e20  ctor = duration 
+00001460: 2f20 616e 696d 2e6c 6f63 616c 5f72 616e  / anim.local_ran
+00001470: 6765 2e65 6e64 0d0a 2020 2020 2020 2020  ge.end..        
+00001480: 2020 2020 616e 696d 2e63 6f6d 7075 7465      anim.compute
+00001490: 5f67 6c6f 6261 6c5f 7261 6e67 6528 0d0a  _global_range(..
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 7365 6c66 2e67 6c6f 6261 6c5f 7261 6e67  self.global_rang
+000014c0: 652e 6174 202b 2061 6e69 6d2e 6c6f 6361  e.at + anim.loca
+000014d0: 6c5f 7261 6e67 652e 6174 202a 2066 6163  l_range.at * fac
+000014e0: 746f 722c 0d0a 2020 2020 2020 2020 2020  tor,..          
+000014f0: 2020 2020 2020 616e 696d 2e6c 6f63 616c        anim.local
+00001500: 5f72 616e 6765 2e64 7572 6174 696f 6e20  _range.duration 
+00001510: 2a20 6661 6374 6f72 0d0a 2020 2020 2020  * factor..      
+00001520: 2020 2020 2020 290d 0a                         )..
```

### Comparing `janim-0.4.0/janim/anims/creation.py` & `janim-0.5.0/janim/anims/creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         become_at_end: bool = False,
         root_only: bool = False,
         **kwargs
     ):
         def func(data: Item.Data, p: UpdaterParams) -> None:
             cmpt = data.components.get('points', None)
             if cmpt is None or not isinstance(cmpt, Cmpt_VPoints):
-                return
+                return  # pragma: no cover
             if not cmpt.has():
-                return
+                return  # pragma: no cover
 
             if not auto_close_path:
-                cmpt.pointwise_become_partial(cmpt, *bound_func(p))
+                cmpt.pointwise_become_partial(cmpt, *bound_func(p))     # pragma: no cover
             else:
                 end_indices = np.array(cmpt.get_subpath_end_indices())
                 begin_indices = np.array([0, *[indice + 2 for indice in end_indices[:-1]]])
 
                 points = cmpt.get()
                 cond1 = np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
 
@@ -123,24 +123,24 @@
             **kwargs
         )
         self.stroke_radius = stroke_radius
         self.stroke_color = stroke_color
 
     def create_extra_data(self, data: Item.Data[VItem]) -> tuple | None:
         if not isinstance(data.item, VItem):
-            return None
+            return None     # pragma: no cover
         data_copy = data._copy(data)
         data_copy.cmpt.radius.set(self.stroke_radius)
         data_copy.cmpt.stroke.set(self.stroke_color, 1)
         data_copy.cmpt.fill.set(alpha=0)
         return (data_copy, )
 
     def updater(self, data: Item.Data[VItem], p: UpdaterParams) -> None:
         if p.extra_data is None:
-            return
+            return  # pragma: no cover
         outline, = p.extra_data
         index, subalpha = integer_interpolate(0, 2, p.alpha)
 
         if index == 0:
             data._restore(outline)
             data.cmpt.points.pointwise_become_partial(data.cmpt.points, 0, subalpha)
         else:
```

### Comparing `janim-0.4.0/janim/anims/display.py` & `janim-0.5.0/janim/anims/display.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/anims/fading.py` & `janim-0.5.0/janim/anims/fading.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/anims/rotation.py` & `janim-0.5.0/janim/anims/rotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if about_point is None:
             box = item.astype(Points).points.self_box if root_only else item.astype(Points).points.box
             about_point = box.get(about_edge)
 
         def func(data: Item.Data, p: UpdaterParams) -> None:
             points = data.components.get('points', None)
             if points is None or not isinstance(points, Cmpt_Points):
-                return
+                return  # pragma: no cover
             points.rotate(p.alpha * angle, about_point=about_point, root_only=True)
 
         super().__init__(item, func, root_only=root_only, **kwargs)
 
 
 class Rotating(Rotate):
     '''
```

### Comparing `janim-0.4.0/janim/anims/timeline.py` & `janim-0.5.0/janim/anims/timeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,49 +6,97 @@
 import time
 import traceback
 from abc import ABCMeta, abstractmethod
 from bisect import bisect, insort
 from collections import defaultdict
 from contextvars import ContextVar
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Iterable, Self
+from typing import Callable, Iterable, Self
 
 import moderngl as mgl
 import numpy as np
 
 from janim.anims.animation import Animation, TimeRange
 from janim.anims.composition import AnimGroup
 from janim.anims.display import Display
-from janim.anims.transform import MethodTransform
 from janim.camera.camera import Camera
+from janim.constants import DOWN, UP
 from janim.exception import (NotAnimationError, StoreFailedError,
                              StoreNotFoundError, TimelineLookupError)
+from janim.items.audio import Audio
 from janim.items.item import Item
+from janim.items.svg.typst import TypstText
+from janim.items.text.text import Text
 from janim.logger import log
 from janim.render.base import RenderData, Renderer, set_global_uniforms
-from janim.utils.config import Config
+from janim.utils.config import Config, ConfigGetter, config_ctx_var
+from janim.utils.iterables import resize_preserving_order
 from janim.utils.simple_functions import clip
 
-if TYPE_CHECKING:   # pragma: no cover
-    from janim.items.item import Item
-
 GET_DATA_DELTA = 1e-5
 ANIM_END_DELTA = 1e-5 * 2
 DEFAULT_DURATION = 1
 
 type DynamicData = Callable[[float], Item.Data]
 
 
 class Timeline(metaclass=ABCMeta):
     '''
     继承该类并实现 :meth:`construct` 方法，以实现动画的构建逻辑
 
     调用 :meth:`build` 可以得到构建完成的动画对象
     '''
 
+    # region config
+
+    CONFIG: Config | None = None
+    '''
+    在子类中定义该变量可以起到设置配置的作用，例如：
+
+    .. code-block::
+
+        class Example(Timeline):
+            CONFIG = Config(
+                font=['Consolas', 'LXGW WenKai Lite']
+            )
+
+            def construct(self) -> None:
+                ...
+    '''
+
+    class _WithConfig:
+        def __init__(self, cls: type[Timeline]):
+            self.cls = cls
+
+            self.lst: list[Config] = []
+            for sup in self.cls.mro():
+                config: Config | None = getattr(sup, 'CONFIG', None)
+                if config is None or config in self.lst:
+                    continue
+                self.lst.append(config)
+
+            self.lst.reverse()
+
+        def __enter__(self) -> Self:
+            lst = [*config_ctx_var.get(), *self.lst]
+            self.token = config_ctx_var.set(lst)
+            return self
+
+        def __exit__(self, exc_type, exc_value, tb) -> None:
+            config_ctx_var.reset(self.token)
+
+    @classmethod
+    def with_config(cls) -> _WithConfig:
+        '''
+        使用定义在 :class:`Timeline` 子类中的 config
+        '''
+        return cls._WithConfig(cls)
+
+    # endregion
+
     # region context
 
     ctx_var: ContextVar[Timeline | None] = ContextVar('Timeline.ctx_var', default=None)
 
     @staticmethod
     def get_context(raise_exc=True) -> Timeline | None:
         '''
@@ -102,63 +150,85 @@
         time: float
         data: Item.Data | DynamicData
         '''
         - 当 ``data`` 的类型为 ``Item.Data`` 时，为静态数据
         - 否则，对于 ``DynamicData`` ，会在获取时调用以得到对应数据
         '''
 
+    @dataclass
+    class PlayAudioInfo:
+        '''
+        调用 :meth:`~.Timeline.play_audio` 的参数信息
+        '''
+        audio: Audio
+        range: TimeRange
+        clip_range: TimeRange
+
+    @dataclass
+    class SubtitleInfo:
+        '''
+        调用 :meth:`~.Timeline.subtitle` 的参数信息
+        '''
+        text: str
+        range: TimeRange
+        kwargs: dict
+        subtitle: Text
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.current_time: float = 0
         self.times_of_code: list[Timeline.TimeOfCode] = []
 
         self.scheduled_tasks: list[Timeline.ScheduledTask] = []
         self.anims: list[AnimGroup] = []
         self.display_anims: list[Display] = []
+        self.audio_infos: list[Timeline.PlayAudioInfo] = []
+        self.subtitle_infos: list[Timeline.SubtitleInfo] = []   # helpful for extracting subtitles
 
         self.item_stored_datas: defaultdict[Item, list[Timeline.TimedItemData]] = defaultdict(list)
         self.item_display_times: dict[Item, int] = {}
 
-        self.camera = Camera()
-        self.register(self.camera)
-
     @abstractmethod
     def construct(self) -> None:
         '''
         继承该方法以实现动画的构建逻辑
         '''
-        pass
+        pass    # pragma: no cover
 
     def build(self, *, quiet=False) -> TimelineAnim:
         '''
         构建动画并返回
         '''
-        token = self.ctx_var.set(self)
-        try:
-            self._build_frame = inspect.currentframe()
-
-            if not quiet:
-                log.info(f'Building "{self.__class__.__name__}"')
-                start_time = time.time()
-
-            self.construct()
-
-            if self.current_time == 0:
-                self.forward(DEFAULT_DURATION)  # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
-                log.info(f'"{self.__class__.__name__}" 构建后没有产生时长，自动产生了 {DEFAULT_DURATION}s 的时长')
-            self.cleanup_display()
-            global_anim = TimelineAnim(self)
-
-            if not quiet:
-                elapsed = time.time() - start_time
-                log.info(f'Finished building "{self.__class__.__name__}" in {elapsed:.2f} s')
+        with self.with_config():
+            token = self.ctx_var.set(self)
+            self.config_getter = ConfigGetter(config_ctx_var.get())
+            self.camera = Camera()
+            try:
+                self._build_frame = inspect.currentframe()
+
+                if not quiet:   # pragma: no cover
+                    log.info(f'Building "{self.__class__.__name__}"')
+                    start_time = time.time()
+
+                self.construct()
+
+                if self.current_time == 0:
+                    self.forward(DEFAULT_DURATION)  # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
+                    if not quiet:   # pragma: no cover
+                        log.info(f'"{self.__class__.__name__}" 构建后没有产生时长，自动产生了 {DEFAULT_DURATION}s 的时长')
+                self.cleanup_display()
+                global_anim = TimelineAnim(self)
+
+                if not quiet:   # pragma: no cover
+                    elapsed = time.time() - start_time
+                    log.info(f'Finished building "{self.__class__.__name__}" in {elapsed:.2f} s')
 
-        finally:
-            self.ctx_var.reset(token)
+            finally:
+                self.ctx_var.reset(token)
 
         return global_anim
 
     def schedule(self, at: float, func: Callable, *args, **kwargs) -> None:
         '''
         计划执行
 
@@ -218,15 +288,15 @@
         ]
         for anim in anims:
             if not isinstance(anim, Animation):
                 raise NotAnimationError('传入了非动画对象，可能是你忘记使用 .anim 了')
 
         anim = AnimGroup(*anims, **kwargs)
         anim.local_range.at += self.current_time
-        anim.set_global_range(anim.local_range.at, anim.local_range.duration)
+        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
 
         anim.anim_pre_init()
         self.detect_changes_of_all()
         anim.anim_init()
 
         self.anims.append(anim)
 
@@ -264,15 +334,15 @@
         if time is None:
             return
 
         duration = self.current_time - time
 
         anim = Display(item, duration=duration, root_only=True)
         anim.local_range.at += time
-        anim.set_global_range(anim.local_range.at, anim.local_range.duration)
+        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
         self.display_anims.append(anim)
         return anim
 
     def hide(self, *roots: Item, root_only=False) -> None:
         '''
         隐藏物件
         '''
@@ -287,14 +357,143 @@
         对目前显示中的所有物件调用隐藏，使得正确产生 :class:`~.Display` 对象
         '''
         for item in list(self.item_display_times.keys()):
             self._hide(item)
 
     # endregion
 
+    # region audio
+
+    def play_audio(
+        self,
+        audio: Audio,
+        *,
+        delay: float = 0,
+        begin: float = 0,
+        end: float = -1,
+    ) -> TimeRange:
+        '''
+        在当前位置播放音频
+
+        - 可以指定 ``begin`` 和 ``end`` 表示裁剪区段
+        - 可以指定在当前位置往后 ``delay`` 秒才开始播放
+
+        返回值表示播放的时间段
+        '''
+        if end == -1:
+            end = audio.duration()
+        duration = end - begin
+
+        info = Timeline.PlayAudioInfo(audio,
+                                      TimeRange(self.current_time + delay, duration),
+                                      TimeRange(begin, duration))
+        self.audio_infos.append(info)
+
+        return info.range.copy()
+
+    def has_audio(self) -> bool:
+        return len(self.audio_infos) != 0
+
+    def get_audio_samples_of_frame(
+        self,
+        fps: float,
+        framerate: int,
+        frame: int
+    ) -> np.ndarray:
+        begin = frame / fps
+        end = (frame + 1) / fps
+
+        output_sample_count = math.floor(end * framerate) - math.floor(begin * framerate)
+        result = np.zeros(output_sample_count, dtype=np.int16)
+
+        for info in self.audio_infos:
+            if end < info.range.at or begin > info.range.end:
+                continue
+
+            audio = info.audio
+
+            frame_begin = int((begin - info.range.at + info.clip_range.at) * audio.framerate)
+            frame_end = int((end - info.range.at + info.clip_range.at) * audio.framerate)
+
+            clip_begin = max(0, int(audio.framerate * info.clip_range.at))
+            clip_end = min(audio.sample_count(), int(audio.framerate * info.clip_range.end))
+
+            left_blank = max(0, clip_begin - frame_begin)
+            right_blank = max(0, frame_end - clip_end)
+
+            data = audio._samples._data[max(clip_begin, frame_begin): min(clip_end, frame_end)]
+
+            if left_blank != 0 or right_blank != 0:
+                data = np.concatenate([
+                    np.zeros(left_blank, dtype=np.int16),
+                    data,
+                    np.zeros(right_blank, dtype=np.int16)
+                ])
+
+            result += resize_preserving_order(data, output_sample_count)
+
+        return result
+
+    # endregion
+
+    # region subtitle
+
+    def subtitle(
+        self,
+        text: str | Iterable[str],
+        delay: float = 0,
+        duration: float = 1,
+        scale: float | Iterable[float] = 0.8,
+        use_typst_text: bool | Iterable[bool] = False,
+        **kwargs
+    ) -> TimeRange:
+        '''
+        添加字幕
+
+        - 文字可以传入一个列表，纵向排列显示
+        - 可以指定在当前位置往后 ``delay`` 秒才显示
+        - ``duration`` 表示持续时间
+        - ``scale`` 表示对文字的缩放，默认为 ``0.8``，可以传入列表表示对各个文字的缩放
+        - ``use_typst_text`` 表示是否使用 :class:`TypstText`，可以传入列表表示各个文字是否使用
+
+        返回值表示显示的时间段
+        '''
+        text_lst = [text] if isinstance(text, str) else text
+        scale_lst = [scale] if not isinstance(scale, Iterable) else scale
+        use_typst_lst = [use_typst_text] if not isinstance(use_typst_text, Iterable) else use_typst_text
+
+        range = TimeRange(self.current_time + delay, duration)
+        for text, scale, use_typst_text in zip(reversed(text_lst),
+                                               reversed(resize_preserving_order(scale_lst, len(text_lst))),
+                                               reversed(resize_preserving_order(use_typst_lst, len(text_lst)))):
+            subtitle = (TypstText if use_typst_text else Text)(text, **kwargs)
+            subtitle.points.scale(scale)
+            self.place_subtitle(subtitle, range)
+            self.subtitle_infos.append(Timeline.SubtitleInfo(text,
+                                                             range,
+                                                             kwargs,
+                                                             subtitle))
+            self.schedule(range.at, subtitle.show)
+            self.schedule(range.end, subtitle.hide)
+
+        return range.copy()
+
+    def place_subtitle(self, subtitle: Text, range: TimeRange) -> None:
+        for other in reversed(self.subtitle_infos):
+            # 根据 TimelineView 中排列显示标签的经验
+            # 这里加了一个 np.isclose 的判断
+            # 如果不加可能导致前一个字幕消失但是后一个字幕凭空出现在更上面
+            # （但是我没有测试过是否会出现这个bug，只是根据写 TimelineView 时的经验加了 np.isclose）
+            if other.range.at <= range.at < other.range.end and not np.isclose(range.at, other.range.end):
+                subtitle.points.next_to(other.subtitle, UP)
+                return
+        subtitle.points.to_border(DOWN)
+
+    # endregion
+
     # region stored_data
 
     # region register
 
     def register(self, item: Item) -> None:
         '''
         在 :meth:`construct` 中创建的物件会自动调用该方法
@@ -386,15 +585,15 @@
                 if isinstance(timed_data.data, Item.Data):
                     return timed_data.data
                 else:
                     if skip_dynamic_data:
                         continue
                     return timed_data.data(t)
 
-        assert False
+        assert False    # pragma: no cover
 
     def get_stored_data_at_right[T](self, item: T, t: float, *, skip_dynamic_data=False) -> Item.Data[T]:
         '''
         得到在指定时间之后的瞬间，物件的数据
         '''
         return self.get_stored_data_at_time(item, t + GET_DATA_DELTA, skip_dynamic_data=skip_dynamic_data)
 
@@ -483,15 +682,15 @@
         time = self.fmt_time(self.current_time)
 
         log.debug(f't={time}  {ext_msg}at construct.{self.get_construct_lineno()}')
 
     # endregion
 
 
-class SourceTimeline(Timeline):
+class SourceTimeline(Timeline):     # pragma: no cover
     '''
     与 :class:`Timeline` 相比，会在背景显示源代码
     '''
     def build(self, *, quiet=False) -> TimelineAnim:
         from janim.items.text.text import SourceDisplayer
         token = self.ctx_var.set(self)
         SourceDisplayer(self.__class__).show()
@@ -518,18 +717,22 @@
         self.display_anim.global_range = self.display_anim.local_range
         self.user_anim.global_range = self.user_anim.local_range
         self.global_range = self.local_range
 
         self.flattened = self.flatten()
         self._time: float | None = None
 
+    @property
+    def cfg(self) -> Config | ConfigGetter:
+        return self.timeline.config_getter
+
     def anim_on(self, local_t: float) -> None:
         # 使最后一帧不空屏
         if np.isclose(local_t, self.global_range.duration):
-            local_t -= 1 / Config.get.fps
+            local_t -= 1 / self.cfg.fps
 
         self._time = local_t
         token = self.global_t_ctx.set(local_t)
         try:
             super().anim_on(local_t)
         finally:
             self.global_t_ctx.reset(token)
@@ -540,15 +743,15 @@
         '''
         if self._time is None:
             return
 
         timeline = self.timeline
         camera_data = timeline.get_stored_data_at_right(timeline.camera, self._time)
         camera_info = camera_data.cmpt.points.info
-        anti_alias_radius = Config.get.anti_alias_width / 2 * camera_info.scaled_factor
+        anti_alias_radius = self.cfg.anti_alias_width / 2 * camera_info.scaled_factor
 
         set_global_uniforms(
             ctx,
             ('JA_VIEW_MATRIX', camera_info.view_matrix.T.flatten()),
             ('JA_PROJ_MATRIX', camera_info.proj_matrix.T.flatten()),
             ('JA_FRAME_RADIUS', camera_info.frame_radius),
             ('JA_ANTI_ALIAS_RADIUS', anti_alias_radius)
```

### Comparing `janim-0.4.0/janim/anims/transform.py` & `janim-0.5.0/janim/anims/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from janim.items.item import Item
 from janim.logger import log
 from janim.typing import Vect
 from janim.utils.data import AlignedData
 from janim.utils.paths import PathFunc, path_along_arc, straight_path
 
 if TYPE_CHECKING:
-    from janim.anims.timeline import DynamicData
+    from janim.anims.timeline import DynamicData    # pragma: no cover
 
 
 class Transform(Animation):
     label_color = (208, 171, 67)
 
     def __init__(
         self,
```

### Comparing `janim-0.4.0/janim/anims/updater.py` & `janim-0.5.0/janim/anims/updater.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/camera/camera.py` & `janim-0.5.0/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/camera/camera_info.py` & `janim-0.5.0/janim/camera/camera_info.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/component.py` & `janim-0.5.0/janim/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,16 @@
         cmpt_copy.objects = {
             key: new_cmpts[key]
             for key in cmpt_copy.objects.keys()
         }
 
         return cmpt_copy
 
-    def become(self, other) -> None: ...
+    def become(self, other) -> Self:    # pragma: no cover
+        return self
 
     def __eq__(self, other: _CmptGroup) -> bool:
         for key in self.objects.keys():
             if self.objects[key] != other.objects[key]:
                 return False
 
         return True
```

### Comparing `janim-0.4.0/janim/components/data.py` & `janim-0.5.0/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/depth.py` & `janim-0.5.0/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/image.py` & `janim-0.5.0/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/points.py` & `janim-0.5.0/janim/components/points.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/radius.py` & `janim-0.5.0/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/rgbas.py` & `janim-0.5.0/janim/components/rgbas.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/components/vpoints.py` & `janim-0.5.0/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/constants/colors.py` & `janim-0.5.0/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/examples.py` & `janim-0.5.0/janim/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,14 @@
         self.forward()
         self.play(Create(circle))
         self.play(Transform(circle, square))
         self.play(Uncreate(square))
         self.forward()
 
 
-class CmptAnimExample(Timeline):
-    def construct(self) -> None:
-        circle = Circle(color=BLUE, fill_alpha=0.5)
-
-        self.show(circle)
-        self.forward()
-        self.play(circle.anim.color.set(GREEN))
-        self.play(circle.anim.fill.set(alpha=0.2))
-        self.play(circle.anim.points.scale(2))
-        self.forward()
-
-
 class SimpleCurveExample(Timeline):
     def construct(self) -> None:
         item1 = VItem(
             LEFT * 2, DR, UR * 3 + UP, RIGHT * 4, DR * 2, DOWN * 2, LEFT * 2,
             NAN_POINT,
             DL * 3, DL * 2, DOWN * 3, DL * 4, DL * 3,
         )
```

### Comparing `janim-0.4.0/janim/exception.py` & `janim-0.5.0/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/gui/anim_viewer.py` & `janim-0.5.0/janim/gui/anim_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-import importlib.machinery
-import inspect
-import json
-import os
-import sys
-import time
-import traceback
-from bisect import bisect
-from dataclasses import dataclass
-
 try:
-    # flake8: noqa
     import PySide6
 except ImportError:
     print('使用 GUI 界面时需要安装额外模块，但是未安装')
     print('你可以使用 pip install janim[gui] 进行安装，并确保你安装在了正确的 Python 版本中')
 
     from janim.exception import EXITCODE_PYSIDE6_NOT_FOUND, ExitException
     raise ExitException(EXITCODE_PYSIDE6_NOT_FOUND)
 
+import importlib.machinery
+import inspect
+import json
+import os
+import sys
+import time
+import traceback
+from bisect import bisect
+from dataclasses import dataclass
 
-from PySide6.QtCore import QByteArray, QRectF, Qt, QTimer, Signal
-from PySide6.QtGui import (QCloseEvent, QColor, QHideEvent, QIcon, QKeyEvent,
-                           QMouseEvent, QPainter, QPaintEvent, QPen,
+import numpy as np
+from PySide6.QtCore import (QByteArray, QPoint, QRect, QRectF, Qt, QTimer,
+                            Signal)
+from PySide6.QtGui import (QBrush, QCloseEvent, QColor, QHideEvent, QIcon,
+                           QKeyEvent, QMouseEvent, QPainter, QPaintEvent, QPen,
                            QWheelEvent)
 from PySide6.QtWidgets import (QApplication, QFileDialog, QLabel, QMainWindow,
                                QMessageBox, QPushButton, QSizePolicy,
-                               QSplitter, QStackedLayout, QWidget)
+                               QSplitter, QStackedLayout, QVBoxLayout, QWidget)
 
 from janim.anims.animation import Animation, TimeRange
 from janim.anims.timeline import Timeline, TimelineAnim
 from janim.exception import ExitException
 from janim.gui.application import Application
+from janim.gui.audio_player import AudioPlayer
 from janim.gui.fixed_ratio_widget import FixedRatioWidget
 from janim.gui.glwidget import GLWidget
+from janim.gui.precise_timer import PreciseTimer
 from janim.gui.richtext_editor import RichTextEditor
 from janim.gui.selector import Selector
 from janim.logger import log
-from janim.render.file_writer import FileWriter
-from janim.utils.config import Config
+from janim.render.writer import VideoWriter
 from janim.utils.file_ops import get_janim_dir
 from janim.utils.simple_functions import clip
 
 TIMELINE_VIEW_MIN_DURATION = 0.5
 
-# TODO: 鼠标悬停在时间轴的动画上时，显示动画信息
-
 
 class AnimViewer(QMainWindow):
     '''
     用于显示构建完成的时间轴动画
 
     可以使用 ``AnimViewer.views(MyTimeline().build())`` 进行直接显示
     '''
+    play_finished = Signal()
+
     def __init__(
         self,
         anim: TimelineAnim,
         auto_play: bool = True,
         interact: bool = False,
         parent: QWidget | None = None
     ) -> None:
@@ -72,20 +73,24 @@
         self.timeline_view.value_changed.connect(self.on_value_changed)
         self.timeline_view.dragged.connect(lambda: self.set_play_state(False))
         self.timeline_view.space_pressed.connect(lambda: self.switch_play_state())
         self.timeline_view.value_changed.emit(0)
 
         self.btn_export.clicked.connect(self.on_export_clicked)
 
-        self.play_timer = QTimer(self)
-        self.play_timer.setTimerType(Qt.TimerType.PreciseTimer)
+        self.play_timer = PreciseTimer(1 / self.anim.cfg.preview_fps, self)
         self.play_timer.timeout.connect(self.on_play_timer_timeout)
         if auto_play:
             self.switch_play_state()
 
+        if self.anim.timeline.has_audio():
+            self.audio_player = AudioPlayer(self.anim.cfg.audio_framerate)
+        else:
+            self.audio_player = None
+
         self.fps_counter = 0
         self.fps_record_start = time.time()
 
         self.glw.rendered.connect(self.on_glw_rendered)
 
     # region setup_ui
 
@@ -94,36 +99,36 @@
         self.setup_status_bar()
         self.setup_central_widget()
 
     def setup_menu_bar(self) -> None:
         menu_bar = self.menuBar()
         menu_functions = menu_bar.addMenu('功能')
 
-        action_stay_on_top = menu_functions.addAction('窗口置前')
-        action_stay_on_top.setCheckable(True)
-        action_stay_on_top.setShortcut('Ctrl+T')
-        action_stay_on_top.toggled.connect(self.on_stay_on_top_toggled)
-        action_stay_on_top.setChecked(True)
+        self.action_stay_on_top = menu_functions.addAction('窗口置前')
+        self.action_stay_on_top.setCheckable(True)
+        self.action_stay_on_top.setShortcut('Ctrl+T')
+        self.action_stay_on_top.toggled.connect(self.on_stay_on_top_toggled)
+        self.action_stay_on_top.setChecked(True)
 
         menu_functions.addSeparator()
 
-        action_reload = menu_functions.addAction('重新构建')
-        action_reload.setShortcut('Ctrl+L')
-        action_reload.triggered.connect(self.on_rebuild_triggered)
+        self.action_reload = menu_functions.addAction('重新构建')
+        self.action_reload.setShortcut('Ctrl+L')
+        self.action_reload.triggered.connect(self.on_rebuild_triggered)
 
         menu_functions.addSeparator()
 
-        action_select = menu_functions.addAction('子物件选择')
-        action_select.setShortcut('Ctrl+S')
-        action_select.triggered.connect(self.on_select_triggered)
+        self.action_select = menu_functions.addAction('子物件选择')
+        self.action_select.setShortcut('Ctrl+S')
+        self.action_select.triggered.connect(self.on_select_triggered)
         self.selector: Selector | None = None
 
-        action_richtext_edit = menu_functions.addAction('富文本编辑')
-        action_richtext_edit.setShortcut('Ctrl+R')
-        action_richtext_edit.triggered.connect(self.on_richtext_edit_triggered)
+        self.action_richtext_edit = menu_functions.addAction('富文本编辑')
+        self.action_richtext_edit.setShortcut('Ctrl+R')
+        self.action_richtext_edit.triggered.connect(self.on_richtext_edit_triggered)
         self.richtext_editor: RichTextEditor | None = None
 
     def setup_status_bar(self) -> None:
         self.fps_label = QLabel()
         self.time_label = QLabel()
         self.btn_export = QPushButton()
         self.btn_export.setIcon(QIcon(os.path.join(get_janim_dir(), 'gui', 'export.png')))
@@ -147,15 +152,15 @@
         self.stkLayout.addWidget(self.overlay)
 
         self.stkWidget = QWidget(self)
         self.stkWidget.setLayout(self.stkLayout)
 
         self.fixed_ratio_widget = FixedRatioWidget(
             self.stkWidget,
-            (Config.get.pixel_width, Config.get.pixel_height)
+            (self.anim.cfg.pixel_width, self.anim.cfg.pixel_height)
         )
 
         self.timeline_view = TimelineView(self.anim)
         self.timeline_view.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
 
         self.vsplitter = QSplitter()
         self.vsplitter.setOrientation(Qt.Orientation.Vertical)
@@ -166,16 +171,16 @@
 
         self.setCentralWidget(self.vsplitter)
         self.setMinimumSize(200, 160)
         self.resize(800, 608)
         self.setWindowTitle('JAnim Graphics')
 
     def move_to_position(self) -> None:
-        window_position = Config.get.wnd_pos
-        window_monitor = Config.get.wnd_monitor
+        window_position = self.anim.cfg.wnd_pos
+        window_monitor = self.anim.cfg.wnd_monitor
 
         if len(window_position) != 2 or window_position[0] not in 'UOD' or window_position[1] not in 'LOR':
             log.warning(f'wnd_pos has wrong argument "{window_position}".')
             window_position = 'UR'
 
         screens = QApplication.screens()
         if window_monitor < len(screens):
@@ -338,16 +343,23 @@
 
                 self.send_lineno(line)
 
         self.glw.set_time(time)
         self.time_label.setText(f'{time:.1f}/{self.anim.global_range.duration:.1f} s')
 
     def on_play_timer_timeout(self) -> None:
+        if self.anim.timeline.has_audio():
+            samples = self.anim.timeline.get_audio_samples_of_frame(self.anim.cfg.preview_fps,
+                                                                    self.anim.cfg.audio_framerate,
+                                                                    self.timeline_view.progress())
+            self.audio_player.write(samples.tobytes())
+
         self.timeline_view.set_progress(self.timeline_view.progress() + 1)
         if self.timeline_view.at_end():
+            self.play_finished.emit()
             self.play_timer.stop()
 
     def on_stay_on_top_toggled(self, flag: bool) -> None:
         visible = self.isVisible()
         self.setWindowFlag(Qt.WindowType.WindowStaysOnTopHint, flag)
         if visible:
             self.setVisible(True)
@@ -414,22 +426,22 @@
     def on_richtext_editor_destroyed(self) -> None:
         self.richtext_editor = None
 
     def on_glw_rendered(self) -> None:
         cur = time.time()
         self.fps_counter += 1
         if cur - self.fps_record_start >= 1:
-            self.fps_label.setText(f'Preview FPS: {self.fps_counter}/{Config.get.preview_fps}')
+            self.fps_label.setText(f'Preview FPS: {self.fps_counter}/{self.anim.cfg.preview_fps}')
             self.fps_counter = 0
             self.fps_record_start = cur
 
     def on_export_clicked(self) -> None:
         self.play_timer.stop()
 
-        output_dir = Config.get.output_dir
+        output_dir = self.anim.cfg.output_dir
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         file_path = QFileDialog.getSaveFileName(
             self,
             '',
             os.path.join(output_dir, f'{self.anim.timeline.__class__.__name__}.mp4'),
@@ -437,15 +449,15 @@
         )
         file_path = file_path[0]
         if not file_path:
             return
 
         QMessageBox.information(self, '提示', '即将进行输出，请留意控制台信息')
         try:
-            FileWriter.writes(self.anim.timeline.__class__().build(), file_path)
+            VideoWriter.writes(self.anim.timeline.__class__().build(), file_path)
         except Exception as e:
             if not isinstance(e, ExitException):
                 traceback.print_exc()
         else:
             QMessageBox.information(self, '提示', f'已完成输出至 {file_path}')
 
     # endregion
@@ -460,15 +472,15 @@
         if self.play_timer.isActive():
             self.play_timer.stop()
         else:
             if self.timeline_view.at_end():
                 self.timeline_view.set_progress(0)
             self.fps_record_start = time.time()
             self.fps_counter = 0
-            self.play_timer.start(1000 // Config.get.preview_fps)
+            self.play_timer.start_precise_timer()
 
     # endregion
 
     @classmethod
     def views(cls, anim: TimelineAnim) -> None:
         '''
         直接显示一个浏览构建完成的时间轴动画的窗口
@@ -519,35 +531,45 @@
         d: bool = False
 
     value_changed = Signal(float)
     dragged = Signal()
 
     space_pressed = Signal()
 
-    label_height = 24   # px
-    play_space = 20     # px
+    # px
+    audio_height = 20
+    label_height = 24
+    range_tip_height = 4
+    play_space = 20
 
     def __init__(self, anim: TimelineAnim, parent: QWidget | None = None):
         super().__init__(parent)
 
         self.set_anim(anim)
 
+        self.hover_timer = QTimer(self)
+        self.hover_timer.setSingleShot(True)
+        self.hover_timer.timeout.connect(self.on_hover_timer_timeout)
+
+        self.tooltip: QWidget | None = None
+
         self.key_timer = QTimer(self)
         self.key_timer.timeout.connect(self.on_key_timer_timeout)
         self.key_timer.start(1000 // 60)
 
         self.setFocusPolicy(Qt.FocusPolicy.StrongFocus)
         self.setMouseTracking(True)
+        self.setMinimumHeight(self.label_height + self.range_tip_height + 10)
 
     def set_anim(self, anim: TimelineAnim) -> None:
         self.range = TimeRange(0, min(20, anim.global_range.duration))
         self.y_offset = 0
         self.anim = anim
         self._progress = 0
-        self._maximum = round(anim.global_range.end * Config.get.preview_fps)
+        self._maximum = round(anim.global_range.end * self.anim.cfg.preview_fps)
 
         self.is_pressing = TimelineView.Pressing()
 
         self.init_label_info()
         self.update()
 
     def init_label_info(self) -> None:
@@ -558,15 +580,16 @@
         self.max_row = 0
 
         self.flatten = self.anim.user_anim.flatten()[1:]
         self._sorted_anims = None
 
         stack: list[Animation] = []
         for anim in self.flatten:
-            while stack and stack[-1].global_range.end <= anim.global_range.at:
+            # 可能会因为浮点误差导致 <= 中的相等判断错误，所以 +1e-5
+            while stack and stack[-1].global_range.end <= anim.global_range.at + 1e-5:
                 stack.pop()
 
             self.labels_info.append(TimelineView.LabelInfo(anim, len(stack)))
             self.max_row = max(self.max_row, len(stack))
             stack.append(anim)
 
     def get_sorted_anims(self) -> list[Animation]:
@@ -576,14 +599,200 @@
 
     def set_range(self, at: float, duration: float) -> None:
         duration = min(duration, self.anim.global_range.duration)
         at = clip(at, 0, self.anim.global_range.duration - duration)
         self.range = TimeRange(at, duration)
         self.update()
 
+    def hover_at(self, pos: QPoint) -> None:
+        audio_rect = self.audio_rect
+        bottom_rect = self.bottom_rect
+
+        # 因为后出现的音频在绘制时会覆盖前面的音频，所以这里用 reversed，就会得到最上层的
+        for info in reversed(self.anim.timeline.audio_infos):
+            range = self.time_range_to_pixel_range(info.range)
+            if QRectF(range.left, audio_rect.y(), range.width, self.audio_height).contains(pos):
+                self.hover_at_audio(pos, info)
+                return
+
+        for info in self.labels_info:
+            range = self.time_range_to_pixel_range(info.anim.global_range)
+            if QRectF(range.left,
+                      bottom_rect.y() + self.label_y(info.row),
+                      range.width,
+                      self.label_height).contains(pos):
+                self.hover_at_anim(pos, info.anim)
+
+    def hover_at_audio(self, pos: QPoint, info: Timeline.PlayAudioInfo) -> None:
+        msg_lst = [
+            f'{round(info.range.at, 2)}s ~ {round(info.range.end, 2)}s',
+            info.audio.filepath
+        ]
+        if info.clip_range != TimeRange(0, info.audio.duration()):
+            msg_lst.append(f'Clip: {round(info.clip_range.at, 2)}s ~ {round(info.clip_range.end, 2)}s')
+
+        label = QLabel('\n'.join(msg_lst))
+        chart_view = self.create_audio_chart(info, near=round(self.pixel_to_time(pos.x())))
+
+        layout = QVBoxLayout()
+        layout.addWidget(label)
+        layout.addWidget(chart_view)
+
+        self.tooltip = QWidget()
+        self.tooltip.setWindowFlag(Qt.WindowType.ToolTip)
+        self.tooltip.setLayout(layout)
+        self.tooltip.adjustSize()
+
+        self.place_tooltip(self.tooltip, pos)
+        self.tooltip.show()
+
+    def create_audio_chart(self, info: Timeline.PlayAudioInfo, near: float | None = None) -> None:
+        from PySide6.QtCharts import (QChart, QChartView, QLineSeries,
+                                      QValueAxis)
+
+        audio = info.audio
+
+        clip_begin = info.clip_range.at
+        clip_end = info.clip_range.end
+        if near is not None:
+            clip_begin = max(clip_begin, near - info.range.at - 4)
+            clip_end = min(clip_end, near - info.range.at + 4)
+
+        range_begin = clip_begin + info.range.at
+        range_end = clip_end + info.range.at
+
+        begin = int(clip_begin * audio.framerate)
+        end = int(clip_end * audio.framerate)
+
+        left_blank = max(0, -begin)
+        right_blank = max(0, end - audio.sample_count())
+
+        data = audio._samples._data[max(0, begin): min(end, audio.sample_count())]
+
+        if left_blank != 0 or right_blank != 0:
+            data = np.concatenate([
+                np.zeros(left_blank, dtype=np.int16),
+                data,
+                np.zeros(right_blank, dtype=np.int16)
+            ])
+
+        unit = audio.framerate // self.anim.cfg.fps
+
+        data = np.max(
+            np.abs(
+                data[:len(data) // unit * unit].reshape(-1, unit)
+            ),
+            axis=1
+        ) / np.iinfo(np.int16).max
+
+        times = np.linspace(range_begin,
+                            range_end,
+                            len(data))
+
+        series = QLineSeries()
+        for t, y in zip(times, data):
+            series.append(t, y)
+
+        x_axis = QValueAxis()
+        x_axis.setRange(range_begin, range_end)
+        x_axis.setTickCount(max(2, 1 + int(range_end - range_begin)))
+
+        y_axis = QValueAxis()
+        y_axis.setRange(0, 1)
+
+        chart = QChart()
+        chart.addSeries(series)
+        chart.addAxis(x_axis, Qt.AlignmentFlag.AlignBottom)
+        chart.addAxis(y_axis, Qt.AlignmentFlag.AlignLeft)
+        series.attachAxis(x_axis)
+        series.attachAxis(y_axis)
+        chart.legend().setVisible(False)
+
+        chart_view = QChartView(chart)
+        chart_view.setRenderHint(QPainter.RenderHint.Antialiasing)
+        chart_view.setMinimumSize(250, 200)
+
+        return chart_view
+
+    def hover_at_anim(self, pos: QPoint, anim: Animation) -> None:
+        parents = [anim]
+        while True:
+            last = parents[-1]
+            if last.parent is None or last.parent is self.anim.user_anim:
+                break
+            parents.append(last.parent)
+
+        label1 = QLabel(f'{anim.__class__.__name__} '
+                        f'{round(anim.global_range.at, 2)}s ~ {round(anim.global_range.end, 2)}s')
+        chart_view = self.create_anim_chart(anim)
+        label2 = QLabel(
+            '\n↑\n'.join(
+                f'{anim.rate_func.__name__} ({anim.__class__.__name__})'
+                for anim in parents
+            )
+        )
+
+        layout = QVBoxLayout()
+        layout.addWidget(label1)
+        layout.addWidget(chart_view)
+        layout.addWidget(label2)
+
+        self.tooltip = QWidget()
+        self.tooltip.setWindowFlag(Qt.WindowType.ToolTip)
+        self.tooltip.setLayout(layout)
+        self.tooltip.adjustSize()
+
+        self.place_tooltip(self.tooltip, pos)
+        self.tooltip.show()
+
+    def create_anim_chart(self, anim: Animation) -> None:
+        from PySide6.QtCharts import QChart, QChartView, QScatterSeries
+
+        count = int(anim.global_range.duration * self.anim.cfg.fps)
+        times = np.linspace(anim.global_range.at,
+                            anim.global_range.end,
+                            count)
+
+        series = QScatterSeries()
+        series.setMarkerSize(3)
+        series.setPen(Qt.PenStyle.NoPen)
+        for t in times:
+            series.append(t, anim.get_alpha_on_global_t(t))
+
+        chart = QChart()
+        chart.addSeries(series)
+        chart.createDefaultAxes()
+        chart.legend().setVisible(False)
+
+        chart_view = QChartView(chart)
+        chart_view.setRenderHint(QPainter.RenderHint.Antialiasing)
+        chart_view.setMinimumSize(250, 200)
+
+        return chart_view
+
+    def place_tooltip(self, tooltip: QWidget, pos: QPoint) -> None:
+        rect = tooltip.screen().availableGeometry()
+        global_pos = self.mapToGlobal(pos)
+        to = QPoint(global_pos) + QPoint(2, 2)
+        if to.x() + tooltip.width() > rect.right():
+            to.setX(global_pos.x() - tooltip.width() - 2)
+        if to.y() + tooltip.height() > rect.bottom():
+            to.setY(global_pos.y() - tooltip.height() - 2)
+
+        tooltip.move(to)
+
+    def hide_tooltip(self) -> None:
+        if self.tooltip is not None:
+            self.tooltip = None
+
+    def on_hover_timer_timeout(self) -> None:
+        pos = self.mapFromGlobal(self.cursor().pos())
+        if self.rect().contains(pos):
+            self.hover_at(pos)
+
     def on_key_timer_timeout(self) -> None:
         if self.is_pressing.w:
             cursor_time = self.pixel_to_time(self.mapFromGlobal(self.cursor().pos()).x())
 
             factor = max(TIMELINE_VIEW_MIN_DURATION / self.range.duration, 0.97)
             self.set_range(
                 factor * (self.range.at - cursor_time) + cursor_time,
@@ -633,18 +842,18 @@
     def progress(self) -> int:
         return self._progress
 
     def at_end(self) -> bool:
         return self._progress == self._maximum
 
     def progress_to_time(self, progress: int) -> float:
-        return progress / Config.get.preview_fps
+        return progress / self.anim.cfg.preview_fps
 
     def time_to_progress(self, time: float) -> int:
-        return round(time * Config.get.preview_fps)
+        return round(time * self.anim.cfg.preview_fps)
 
     def time_to_pixel(self, time: float) -> float:
         return (time - self.range.at) / self.range.duration * self.width()
 
     def pixel_to_time(self, pixel: float) -> float:
         return pixel / self.width() * self.range.duration + self.range.at
 
@@ -661,18 +870,24 @@
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         if event.button() == Qt.MouseButton.LeftButton:
             self.set_progress(self.pixel_to_progress(event.position().x()))
             self.dragged.emit()
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
+        self.hover_timer.start(500)
+        self.hide_tooltip()
+
         if event.buttons() & Qt.MouseButton.LeftButton:
             self.set_progress(self.pixel_to_progress(event.position().x()))
             self.dragged.emit()
 
+    def leaveEvent(self, _) -> None:
+        self.hide_tooltip()
+
     def keyPressEvent(self, event: QKeyEvent) -> None:
         key = event.key()
 
         if key == Qt.Key.Key_Space:
             self.space_pressed.emit()
 
         elif key == Qt.Key.Key_W:
@@ -683,27 +898,27 @@
             self.is_pressing.s = True
         elif key == Qt.Key.Key_D:
             self.is_pressing.d = True
 
         elif key == Qt.Key.Key_Z:
             anims = self.get_sorted_anims()
             time = self.progress_to_time(self._progress)
-            idx = bisect(anims, time - 1e-5, key=lambda x: x.global_range.at)
+            idx = bisect(anims, time - 1e-2, key=lambda x: x.global_range.at)
             idx -= 1
             if idx < 0:
                 self.set_progress(0)
             else:
                 self.set_progress(self.time_to_progress(anims[idx].global_range.at))
 
             self.dragged.emit()
 
         elif key == Qt.Key.Key_C:
             anims = self.get_sorted_anims()
             time = self.progress_to_time(self._progress)
-            idx = bisect(anims, time + 1e-5, key=lambda x: x.global_range.at)
+            idx = bisect(anims, time + 1e-2, key=lambda x: x.global_range.at)
             if idx < len(anims):
                 self.set_progress(self.time_to_progress(anims[idx].global_range.at))
             else:
                 self.set_progress(self.time_to_progress(self.anim.global_range.end))
 
             self.dragged.emit()
 
@@ -723,52 +938,151 @@
         self.y_offset = clip(self.y_offset - event.angleDelta().y() / 240 * self.label_height,
                              0,
                              self.max_row * self.label_height)
         self.update()
 
     def paintEvent(self, _: QPaintEvent) -> None:
         p = QPainter(self)
+        orig_font = p.font()
+
+        # 绘制每次 forward 或 play 的时刻
+        times_of_code = self.anim.timeline.times_of_code
+        left = bisect(times_of_code, self.range.at - 1e-5, key=lambda x: x.time)
+        right = bisect(times_of_code, self.range.end + 1e-5, key=lambda x: x.time)
+
+        p.setPen(QPen(QColor(74, 48, 80), 2))
+        p.setRenderHint(QPainter.RenderHint.Antialiasing, True)
+        for time_of_code in times_of_code[left:right]:
+            self.paint_line(p, time_of_code.time)
+        p.setRenderHint(QPainter.RenderHint.Antialiasing, False)
+
+        # 绘制音频区段
+        if self.anim.timeline.has_audio():
+            audio_rect = self.audio_rect
+
+            font = p.font()
+            font.setPointSize(8)
+            p.setFont(font)
+
+            for info in self.anim.timeline.audio_infos:
+                if info.range.end <= self.range.at or info.range.at >= self.range.end:
+                    continue
+
+                self.paint_label(p,
+                                 info.range,
+                                 audio_rect.y(),
+                                 self.audio_height,
+                                 info.audio.filename,
+                                 QColor(152, 255, 191),
+                                 QColor(152, 255, 191, 128))
+
+            p.setFont(orig_font)
 
         # 绘制动画区段
+        bottom_rect = self.bottom_rect
+        p.setClipRect(bottom_rect)
+
         for info in self.labels_info:
             if info.anim.global_range.end <= self.range.at or info.anim.global_range.at >= self.range.end:
                 continue
 
-            range = self.time_range_to_pixel_range(info.anim.global_range)
-            rect = QRectF(range.left, -self.y_offset + info.row * self.label_height, range.width, self.label_height)
-            if rect.x() < 0:
-                rect.setX(0)
-
-            # 这里的判断使得区段过窄时也能看得见
-            if rect.width() > 5:
-                x_adjust = 2
-            elif rect.width() > 1:
-                x_adjust = (rect.width() - 1) / 2
-            else:
-                x_adjust = 0
+            self.paint_label(p,
+                             info.anim.global_range,
+                             bottom_rect.y() + self.label_y(info.row),
+                             self.label_height,
+                             info.anim.__class__.__name__,
+                             Qt.PenStyle.NoPen,
+                             QColor(*info.anim.label_color).lighter())
 
-            # 绘制背景部分
-            rect.adjust(x_adjust, 2, -x_adjust, -2)
-            p.setPen(Qt.PenStyle.NoPen)
-            p.setBrush(QColor(*info.anim.label_color).lighter())
-            p.drawRect(rect)
-
-            # 绘制动画类名
-            rect.adjust(1, 1, -1, -1)
-            p.setPen(Qt.GlobalColor.black)
-            p.drawText(
-                rect,
-                Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
-                f'{info.anim.__class__.__name__}'
-            )
+        p.setClipping(False)
 
         # 绘制当前进度指示
-        pixel_at = self.progress_to_pixel(self._progress)
         p.setPen(QPen(Qt.GlobalColor.white, 2))
-        p.drawLine(pixel_at, 0, pixel_at, self.height())
+        p.setRenderHint(QPainter.RenderHint.Antialiasing, True)
+        self.paint_line(p, self.progress_to_time(self._progress))
+        p.setRenderHint(QPainter.RenderHint.Antialiasing, False)
 
         # 绘制视野区域指示（底部的长条）
         left = self.range.at / self.anim.global_range.duration * self.width()
         width = self.range.duration / self.anim.global_range.duration * self.width()
         p.setPen(Qt.PenStyle.NoPen)
         p.setBrush(QColor(77, 102, 132))
-        p.drawRoundedRect(left, self.height() - 4, width, 4, 2, 2)
+        p.drawRoundedRect(
+            left,
+            self.height() - self.range_tip_height,
+            width,
+            self.range_tip_height,
+            self.range_tip_height / 2,
+            self.range_tip_height / 2
+        )
+
+    @property
+    def audio_rect(self) -> QRect:
+        if not self.anim.timeline.has_audio():
+            return QRect(0, 0, self.width(), 0)
+        return QRect(0, 0, self.width(), self.audio_height)
+
+    @property
+    def bottom_rect(self) -> QRect:
+        return self.rect().adjusted(0,
+                                    self.audio_height if self.anim.timeline.has_audio() else 0,
+                                    0,
+                                    -self.range_tip_height)
+
+    def label_y(self, row: int) -> float:
+        return -self.y_offset + row * self.label_height
+
+    def paint_label(
+        self,
+        p: QPainter,
+        time_range: TimeRange,
+        y: float,
+        height: float,
+        txt: str,
+        stroke: QPen | QColor,
+        fill: QBrush | QColor,
+    ) -> None:
+        range = self.time_range_to_pixel_range(time_range)
+        rect = QRectF(range.left, y, range.width, height)
+
+        # 标记是否应当绘制文字
+        draw_txt = True
+
+        # 使得超出底端的区段也能看到一条边
+        max_y = self.height() - self.range_tip_height - 4
+        if rect.y() > max_y:
+            rect.setY(max_y)
+            rect.setBottom(self.height() + 2)
+            draw_txt = False
+
+        # 这里的判断使得区段过窄时也能看得见
+        if rect.width() > 5:
+            x_adjust = 2
+        elif rect.width() > 1:
+            x_adjust = (rect.width() - 1) / 2
+        else:
+            x_adjust = 0
+
+        # 绘制背景部分
+        rect.adjust(x_adjust, 2, -x_adjust, -2)
+        p.setPen(stroke)
+        p.setBrush(fill)
+        p.drawRect(rect)
+
+        # 使得在区段的左侧有一部分在显示区域外时，
+        # 文字仍然对齐到屏幕的左端，而不是跑到屏幕外面去
+        if rect.x() < 0:
+            rect.setX(0)
+
+        # 绘制文字
+        if draw_txt:
+            rect.adjust(1, 1, -1, -1)
+            p.setPen(Qt.GlobalColor.black)
+            p.drawText(
+                rect,
+                Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
+                txt
+            )
+
+    def paint_line(self, p: QPainter, time: float) -> None:
+        pixel_at = self.time_to_pixel(time)
+        p.drawLine(pixel_at, 0, pixel_at, self.height())
```

### Comparing `janim-0.4.0/janim/gui/export.png` & `janim-0.5.0/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/gui/fixed_ratio_widget.py` & `janim-0.5.0/janim/gui/fixed_ratio_widget.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/gui/glwidget.py` & `janim-0.5.0/janim/gui/glwidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 import moderngl as mgl
 from PySide6.QtCore import Signal
 from PySide6.QtOpenGLWidgets import QOpenGLWidget
 from PySide6.QtWidgets import QWidget
 
 from janim.anims.timeline import TimelineAnim
-from janim.utils.config import Config
 
 
 class GLWidget(QOpenGLWidget):
     '''
     窗口中央的渲染界面
     '''
     rendered = Signal()
@@ -22,12 +21,12 @@
         self.anim.anim_on(time)
         self.update()
 
     def initializeGL(self) -> None:
         self.ctx = mgl.create_context()
         self.ctx.enable(mgl.BLEND)
 
-        self.ctx.clear(*Config.get.background_color.rgb)
+        self.ctx.clear(*self.anim.cfg.background_color.rgb)
 
     def paintGL(self) -> None:
         self.anim.render_all(self.ctx)
         self.rendered.emit()
```

### Comparing `janim-0.4.0/janim/gui/richtext_editor.py` & `janim-0.5.0/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/gui/selector.py` & `janim-0.5.0/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/imports.py` & `janim-0.5.0/janim/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from janim.anims.rotation import *
 from janim.anims.timeline import *
 from janim.anims.transform import *
 from janim.anims.updater import *
 from janim.camera.camera import *
 from janim.camera.camera_info import *
 from janim.components.rgbas import apart_alpha, merge_alpha
+from janim.items.audio import *
 from janim.items.coordinate.coordinate_systems import *
 from janim.items.coordinate.functions import *
 from janim.items.coordinate.number_line import *
 from janim.items.geometry.arc import *
 from janim.items.geometry.arrow import *
 from janim.items.geometry.line import *
 from janim.items.geometry.polygon import *
```

### Comparing `janim-0.4.0/janim/items/boolean_ops.py` & `janim-0.5.0/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/coordinate/coordinate_systems.py` & `janim-0.5.0/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/coordinate/functions.py` & `janim-0.5.0/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/coordinate/number_line.py` & `janim-0.5.0/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/geometry/arc.py` & `janim-0.5.0/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/geometry/arrow.py` & `janim-0.5.0/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/geometry/line.py` & `janim-0.5.0/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/geometry/polygon.py` & `janim-0.5.0/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/image_item.py` & `janim-0.5.0/janim/items/image_item.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/item.py` & `janim-0.5.0/janim/items/item.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/points.py` & `janim-0.5.0/janim/items/points.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/relation.py` & `janim-0.5.0/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/svg/brace.py` & `janim-0.5.0/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/svg/brace.svg` & `janim-0.5.0/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/svg/svg_item.py` & `janim-0.5.0/janim/items/svg/svg_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,239 +17,239 @@
 00000100: 6c6f 6767 6572 2069 6d70 6f72 7420 6c6f  logger import lo
 00000110: 670d 0a66 726f 6d20 6a61 6e69 6d2e 7574  g..from janim.ut
 00000120: 696c 732e 6265 7a69 6572 2069 6d70 6f72  ils.bezier impor
 00000130: 7420 5061 7468 4275 696c 6465 720d 0a66  t PathBuilder..f
 00000140: 726f 6d20 6a61 6e69 6d2e 7574 696c 732e  rom janim.utils.
 00000150: 636f 6e66 6967 2069 6d70 6f72 7420 436f  config import Co
 00000160: 6e66 6967 0d0a 0d0a 2320 e8bf 99e9 878c  nfig....# ......
-00000170: e79a 8420 332e 3331 3336 20e6 98af e688  ... 3.3136 .....
-00000180: 91e6 898b e58a a8e8 af95 e587 bae6 9da5  ................
-00000190: e79a 840d 0a44 4546 4155 4c54 5f53 5647  .....DEFAULT_SVG
-000001a0: 4954 454d 5f53 4341 4c45 5f46 4143 544f  ITEM_SCALE_FACTO
-000001b0: 5220 3d20 332e 3331 3336 0d0a 5354 524f  R = 3.3136..STRO
-000001c0: 4b45 5f57 4944 5448 5f43 4f4e 5645 5253  KE_WIDTH_CONVERS
-000001d0: 494f 4e20 3d20 302e 3031 0d0a 0d0a 7479  ION = 0.01....ty
-000001e0: 7065 2056 4974 656d 4275 696c 6465 7220  pe VItemBuilder 
-000001f0: 3d20 4361 6c6c 6162 6c65 5b5b 5d2c 2056  = Callable[[], V
-00000200: 4974 656d 5d0d 0a0d 0a0d 0a64 6566 205f  Item]......def _
-00000210: 636f 6e76 6572 745f 706f 696e 745f 746f  convert_point_to
-00000220: 5f33 6428 783a 2066 6c6f 6174 2c20 793a  _3d(x: float, y:
-00000230: 2066 6c6f 6174 2920 2d3e 206e 702e 6e64   float) -> np.nd
-00000240: 6172 7261 793a 0d0a 2020 2020 7265 7475  array:..    retu
-00000250: 726e 206e 702e 6172 7261 7928 5b78 2c20  rn np.array([x, 
-00000260: 792c 2030 5d29 0d0a 0d0a 0d0a 6465 6620  y, 0])......def 
-00000270: 5f63 6f6e 7665 7274 5f61 6c70 6861 5f74  _convert_alpha_t
-00000280: 6f5f 666c 6f61 7428 783a 2069 6e74 207c  o_float(x: int |
-00000290: 204e 6f6e 6529 202d 3e20 666c 6f61 743a   None) -> float:
-000002a0: 0d0a 2020 2020 7265 7475 726e 204e 6f6e  ..    return Non
-000002b0: 6520 6966 2078 2069 7320 4e6f 6e65 2065  e if x is None e
-000002c0: 6c73 6520 7820 2f20 3235 350d 0a0d 0a0d  lse x / 255.....
-000002d0: 0a63 6c61 7373 2053 5647 4974 656d 2847  .class SVGItem(G
-000002e0: 726f 7570 5b56 4974 656d 5d29 3a0d 0a20  roup[VItem]):.. 
-000002f0: 2020 2027 2727 0d0a 2020 2020 e4bc a0e5     '''..    ....
-00000300: 85a5 2053 5647 20e6 9687 e4bb b6e8 b7af  .. SVG .........
-00000310: e5be 84ef bc8c e8a7 a3e6 9e90 e4b8 bae7  ................
-00000320: 89a9 e4bb b60d 0a20 2020 2027 2727 0d0a  .......    '''..
-00000330: 2020 2020 7376 675f 7061 7274 5f64 6566      svg_part_def
-00000340: 6175 6c74 5f6b 7761 7267 7320 3d20 6469  ault_kwargs = di
-00000350: 6374 280d 0a20 2020 2020 2020 2073 7472  ct(..        str
-00000360: 6f6b 655f 7261 6469 7573 3d31 2e30 202a  oke_radius=1.0 *
-00000370: 2053 5452 4f4b 455f 5749 4454 485f 434f   STROKE_WIDTH_CO
-00000380: 4e56 4552 5349 4f4e 202f 2032 2c0d 0a20  NVERSION / 2,.. 
-00000390: 2020 2020 2020 2073 7472 6f6b 655f 636f         stroke_co
-000003a0: 6c6f 723d 4e6f 6e65 2c0d 0a20 2020 2020  lor=None,..     
-000003b0: 2020 2073 7472 6f6b 655f 616c 7068 613d     stroke_alpha=
-000003c0: 302c 0d0a 2020 2020 2020 2020 6669 6c6c  0,..        fill
-000003d0: 5f63 6f6c 6f72 3d4e 6f6e 652c 0d0a 2020  _color=None,..  
-000003e0: 2020 2020 2020 6669 6c6c 5f61 6c70 6861        fill_alpha
-000003f0: 3d30 0d0a 2020 2020 290d 0a20 2020 2076  =0..    )..    v
-00000400: 6974 656d 5f62 7569 6c64 6572 735f 6d61  item_builders_ma
-00000410: 703a 2064 6963 745b 7475 706c 652c 206c  p: dict[tuple, l
-00000420: 6973 745b 5649 7465 6d42 7569 6c64 6572  ist[VItemBuilder
-00000430: 5d5d 203d 207b 7d0d 0a0d 0a20 2020 2064  ]] = {}....    d
-00000440: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00000450: 2c20 6669 6c65 5f70 6174 683a 2073 7472  , file_path: str
-00000460: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-00000470: 2020 2020 2020 6974 656d 7320 3d20 7365        items = se
-00000480: 6c66 2e67 6574 5f69 7465 6d73 5f66 726f  lf.get_items_fro
-00000490: 6d5f 6669 6c65 2866 696c 655f 7061 7468  m_file(file_path
-000004a0: 290d 0a0d 0a20 2020 2020 2020 2073 7570  )....        sup
-000004b0: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a69  er().__init__(*i
-000004c0: 7465 6d73 2c20 2a2a 6b77 6172 6773 290d  tems, **kwargs).
-000004d0: 0a0d 0a20 2020 2020 2020 2073 656c 6628  ...        self(
-000004e0: 5649 7465 6d29 2e70 6f69 6e74 732e 7363  VItem).points.sc
-000004f0: 616c 6528 0d0a 2020 2020 2020 2020 2020  ale(..          
-00000500: 2020 436f 6e66 6967 2e67 6574 2e70 6978    Config.get.pix
-00000510: 656c 5f74 6f5f 6672 616d 655f 7261 7469  el_to_frame_rati
-00000520: 6f20 2a20 4445 4641 554c 545f 5356 4749  o * DEFAULT_SVGI
-00000530: 5445 4d5f 5343 414c 455f 4641 4354 4f52  TEM_SCALE_FACTOR
-00000540: 2c0d 0a20 2020 2020 2020 2020 2020 2061  ,..            a
-00000550: 626f 7574 5f70 6f69 6e74 3d4f 5249 4749  bout_point=ORIGI
-00000560: 4e0d 0a20 2020 2020 2020 2029 2e66 6c69  N..        ).fli
-00000570: 7028 5249 4748 5429 0d0a 0d0a 2020 2020  p(RIGHT)....    
-00000580: 2020 2020 7365 6c66 2e6d 6f76 655f 696e      self.move_in
-00000590: 746f 5f70 6f73 6974 696f 6e28 290d 0a0d  to_position()...
-000005a0: 0a20 2020 2064 6566 206d 6f76 655f 696e  .    def move_in
-000005b0: 746f 5f70 6f73 6974 696f 6e28 7365 6c66  to_position(self
-000005c0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-000005d0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-000005e0: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-000005f0: 2020 2064 6566 2067 6574 5f69 7465 6d73     def get_items
-00000600: 5f66 726f 6d5f 6669 6c65 2866 696c 655f  _from_file(file_
-00000610: 7061 7468 3a20 7374 7229 202d 3e20 6c69  path: str) -> li
-00000620: 7374 5b49 7465 6d5d 3a0d 0a20 2020 2020  st[Item]:..     
-00000630: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-00000640: e8a7 a3e6 9e90 e696 87e4 bbb6 e5b9 b6e5  ................
-00000650: be97 e588 b0e7 89a9 e4bb b6e5 8897 e8a1  ................
-00000660: a80d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
-00000670: 2020 2020 2020 2020 6d74 696d 6520 3d20          mtime = 
-00000680: 6f73 2e70 6174 682e 6765 746d 7469 6d65  os.path.getmtime
-00000690: 2866 696c 655f 7061 7468 290d 0a20 2020  (file_path)..   
-000006a0: 2020 2020 206e 616d 6520 3d20 6f73 2e70       name = os.p
-000006b0: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
-000006c0: 7061 7468 2e62 6173 656e 616d 6528 6669  path.basename(fi
-000006d0: 6c65 5f70 6174 6829 295b 305d 0d0a 2020  le_path))[0]..  
-000006e0: 2020 2020 2020 6b65 7920 3d20 286e 616d        key = (nam
-000006f0: 652c 206d 7469 6d65 290d 0a0d 0a20 2020  e, mtime)....   
-00000700: 2020 2020 2063 6163 6865 6420 3d20 5356       cached = SV
-00000710: 4749 7465 6d2e 7669 7465 6d5f 6275 696c  GItem.vitem_buil
-00000720: 6465 7273 5f6d 6170 2e67 6574 286b 6579  ders_map.get(key
-00000730: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
-00000740: 2069 6620 6361 6368 6564 2069 7320 6e6f   if cached is no
-00000750: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00000760: 2020 2020 2072 6574 7572 6e20 5b62 7569       return [bui
-00000770: 6c64 6572 2829 2066 6f72 2062 7569 6c64  lder() for build
-00000780: 6572 2069 6e20 6361 6368 6564 5d0d 0a0d  er in cached]...
-00000790: 0a20 2020 2020 2020 2073 7667 3a20 7365  .        svg: se
-000007a0: 2e53 5647 203d 2073 652e 5356 472e 7061  .SVG = se.SVG.pa
-000007b0: 7273 6528 6669 6c65 5f70 6174 6829 0d0a  rse(file_path)..
-000007c0: 0d0a 2020 2020 2020 2020 6f66 6673 6574  ..        offset
-000007d0: 203d 206e 702e 6172 7261 7928 5b73 7667   = np.array([svg
-000007e0: 2e77 6964 7468 202f 202d 322c 2073 7667  .width / -2, svg
-000007f0: 2e68 6569 6768 7420 2f20 2d32 5d29 0d0a  .height / -2])..
-00000800: 0d0a 2020 2020 2020 2020 6275 696c 6465  ..        builde
-00000810: 7273 3a20 6c69 7374 5b56 4974 656d 4275  rs: list[VItemBu
-00000820: 696c 6465 725d 203d 205b 5d0d 0a20 2020  ilder] = []..   
-00000830: 2020 2020 2066 6f72 2073 6861 7065 2069       for shape i
-00000840: 6e20 7376 672e 656c 656d 656e 7473 2829  n svg.elements()
-00000850: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000860: 6620 6973 696e 7374 616e 6365 2873 6861  f isinstance(sha
-00000870: 7065 2c20 2873 652e 4772 6f75 702c 2073  pe, (se.Group, s
-00000880: 652e 5573 6529 293a 0d0a 2020 2020 2020  e.Use)):..      
-00000890: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-000008a0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-000008b0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-000008c0: 7368 6170 652c 2073 652e 5061 7468 293a  shape, se.Path):
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008e0: 2020 6275 696c 6465 7273 2e61 7070 656e    builders.appen
-000008f0: 6428 5356 4749 7465 6d2e 636f 6e76 6572  d(SVGItem.conver
-00000900: 745f 7061 7468 2873 6861 7065 2c20 6f66  t_path(shape, of
-00000910: 6673 6574 2929 0d0a 2020 2020 2020 2020  fset))..        
-00000920: 2020 2020 656c 6966 2074 7970 6528 7368      elif type(sh
-00000930: 6170 6529 2069 7320 7365 2e53 5647 456c  ape) is se.SVGEl
-00000940: 656d 656e 743a 0d0a 2020 2020 2020 2020  ement:..        
-00000950: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00000960: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00000970: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000980: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
-00000990: 2866 2755 6e73 7570 706f 7274 6564 2065  (f'Unsupported e
-000009a0: 6c65 6d65 6e74 2074 7970 653a 207b 7479  lement type: {ty
-000009b0: 7065 2873 6861 7065 297d 2729 0d0a 0d0a  pe(shape)}')....
-000009c0: 2020 2020 2020 2020 5356 4749 7465 6d2e          SVGItem.
-000009d0: 7669 7465 6d5f 6275 696c 6465 7273 5f6d  vitem_builders_m
-000009e0: 6170 5b6b 6579 5d20 3d20 6275 696c 6465  ap[key] = builde
-000009f0: 7273 0d0a 2020 2020 2020 2020 7265 7475  rs..        retu
-00000a00: 726e 205b 6275 696c 6465 7228 2920 666f  rn [builder() fo
-00000a10: 7220 6275 696c 6465 7220 696e 2062 7569  r builder in bui
-00000a20: 6c64 6572 735d 0d0a 0d0a 2020 2020 4073  lders]....    @s
-00000a30: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
-00000a40: 2064 6566 2063 6f6e 7665 7274 5f70 6174   def convert_pat
-00000a50: 6828 7061 7468 3a20 7365 2e50 6174 682c  h(path: se.Path,
-00000a60: 206f 6666 7365 743a 206e 702e 6e64 6172   offset: np.ndar
-00000a70: 7261 7929 202d 3e20 5649 7465 6d42 7569  ray) -> VItemBui
-00000a80: 6c64 6572 3a0d 0a20 2020 2020 2020 2062  lder:..        b
-00000a90: 7569 6c64 6572 203d 2050 6174 6842 7569  uilder = PathBui
-00000aa0: 6c64 6572 2829 0d0a 2020 2020 2020 2020  lder()..        
-00000ab0: 7365 676d 656e 745f 636c 6173 735f 746f  segment_class_to
-00000ac0: 5f66 756e 635f 6d61 7020 3d20 7b0d 0a20  _func_map = {.. 
-00000ad0: 2020 2020 2020 2020 2020 2073 652e 4d6f             se.Mo
-00000ae0: 7665 3a20 2862 7569 6c64 6572 2e6d 6f76  ve: (builder.mov
-00000af0: 655f 746f 2c20 2827 656e 6427 2c29 292c  e_to, ('end',)),
-00000b00: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000b10: 2e43 6c6f 7365 3a20 2862 7569 6c64 6572  .Close: (builder
-00000b20: 2e63 6c6f 7365 5f70 6174 682c 2028 2929  .close_path, ())
-00000b30: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00000b40: 652e 4c69 6e65 3a20 2862 7569 6c64 6572  e.Line: (builder
-00000b50: 2e6c 696e 655f 746f 2c20 2827 656e 6427  .line_to, ('end'
-00000b60: 2c29 292c 0d0a 2020 2020 2020 2020 2020  ,)),..          
-00000b70: 2020 7365 2e51 7561 6472 6174 6963 4265    se.QuadraticBe
-00000b80: 7a69 6572 3a20 2862 7569 6c64 6572 2e63  zier: (builder.c
-00000b90: 6f6e 6963 5f74 6f2c 2028 2763 6f6e 7472  onic_to, ('contr
-00000ba0: 6f6c 272c 2027 656e 6427 2929 2c0d 0a20  ol', 'end')),.. 
-00000bb0: 2020 2020 2020 2020 2020 2073 652e 4375             se.Cu
-00000bc0: 6269 6342 657a 6965 723a 2028 6275 696c  bicBezier: (buil
-00000bd0: 6465 722e 6375 6269 635f 746f 2c20 2827  der.cubic_to, ('
-00000be0: 636f 6e74 726f 6c31 272c 2027 636f 6e74  control1', 'cont
-00000bf0: 726f 6c32 272c 2027 656e 6427 2929 0d0a  rol2', 'end'))..
-00000c00: 2020 2020 2020 2020 7d0d 0a0d 0a20 2020          }....   
-00000c10: 2020 2020 2066 6f72 2073 6567 6d65 6e74       for segment
-00000c20: 2069 6e20 7061 7468 3a0d 0a20 2020 2020   in path:..     
-00000c30: 2020 2020 2020 2073 6567 6d65 6e74 5f63         segment_c
-00000c40: 6c61 7373 203d 2073 6567 6d65 6e74 2e5f  lass = segment._
-00000c50: 5f63 6c61 7373 5f5f 0d0a 2020 2020 2020  _class__..      
-00000c60: 2020 2020 2020 6675 6e63 2c20 6174 7472        func, attr
-00000c70: 5f6e 616d 6573 203d 2073 6567 6d65 6e74  _names = segment
-00000c80: 5f63 6c61 7373 5f74 6f5f 6675 6e63 5f6d  _class_to_func_m
-00000c90: 6170 5b73 6567 6d65 6e74 5f63 6c61 7373  ap[segment_class
-00000ca0: 5d0d 0a20 2020 2020 2020 2020 2020 2070  ]..            p
-00000cb0: 6f69 6e74 7320 3d20 5b0d 0a20 2020 2020  oints = [..     
-00000cc0: 2020 2020 2020 2020 2020 205f 636f 6e76             _conv
-00000cd0: 6572 745f 706f 696e 745f 746f 5f33 6428  ert_point_to_3d(
-00000ce0: 2a67 6574 6174 7472 2873 6567 6d65 6e74  *getattr(segment
-00000cf0: 2c20 6174 7472 5f6e 616d 6529 290d 0a20  , attr_name)).. 
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000d10: 6f72 2061 7474 725f 6e61 6d65 2069 6e20  or attr_name in 
-00000d20: 6174 7472 5f6e 616d 6573 0d0a 2020 2020  attr_names..    
-00000d30: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00000d40: 2020 2020 2020 2066 756e 6328 2a70 6f69         func(*poi
-00000d50: 6e74 7329 0d0a 0d0a 2020 2020 2020 2020  nts)....        
-00000d60: 7669 7465 6d5f 7374 796c 6573 203d 2064  vitem_styles = d
-00000d70: 6963 7428 0d0a 2020 2020 2020 2020 2020  ict(..          
-00000d80: 2020 7374 726f 6b65 5f72 6164 6975 733d    stroke_radius=
-00000d90: 7061 7468 2e73 7472 6f6b 655f 7769 6474  path.stroke_widt
-00000da0: 6820 2a20 5354 524f 4b45 5f57 4944 5448  h * STROKE_WIDTH
-00000db0: 5f43 4f4e 5645 5253 494f 4e20 2f20 322c  _CONVERSION / 2,
-00000dc0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00000dd0: 726f 6b65 5f63 6f6c 6f72 3d70 6174 682e  roke_color=path.
-00000de0: 7374 726f 6b65 2e68 6578 2c0d 0a20 2020  stroke.hex,..   
-00000df0: 2020 2020 2020 2020 2073 7472 6f6b 655f           stroke_
-00000e00: 616c 7068 613d 5f63 6f6e 7665 7274 5f61  alpha=_convert_a
-00000e10: 6c70 6861 5f74 6f5f 666c 6f61 7428 7061  lpha_to_float(pa
-00000e20: 7468 2e73 7472 6f6b 652e 616c 7068 6129  th.stroke.alpha)
-00000e30: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
-00000e40: 696c 6c5f 636f 6c6f 723d 7061 7468 2e66  ill_color=path.f
-00000e50: 696c 6c2e 6865 782c 0d0a 2020 2020 2020  ill.hex,..      
-00000e60: 2020 2020 2020 6669 6c6c 5f61 6c70 6861        fill_alpha
-00000e70: 3d5f 636f 6e76 6572 745f 616c 7068 615f  =_convert_alpha_
-00000e80: 746f 5f66 6c6f 6174 2870 6174 682e 6669  to_float(path.fi
-00000e90: 6c6c 2e61 6c70 6861 290d 0a20 2020 2020  ll.alpha)..     
-00000ea0: 2020 2029 0d0a 2020 2020 2020 2020 7669     )..        vi
-00000eb0: 7465 6d5f 706f 696e 7473 203d 2062 7569  tem_points = bui
-00000ec0: 6c64 6572 2e67 6574 2829 0d0a 2020 2020  lder.get()..    
-00000ed0: 2020 2020 7669 7465 6d5f 706f 696e 7473      vitem_points
-00000ee0: 5b3a 2c20 3a32 5d20 2b3d 206f 6666 7365  [:, :2] += offse
-00000ef0: 740d 0a0d 0a20 2020 2020 2020 2064 6566  t....        def
-00000f00: 2076 6974 656d 5f62 7569 6c64 6572 2829   vitem_builder()
-00000f10: 202d 3e20 5649 7465 6d3a 0d0a 2020 2020   -> VItem:..    
-00000f20: 2020 2020 2020 2020 7669 7465 6d20 3d20          vitem = 
-00000f30: 5649 7465 6d28 2a2a 5356 4749 7465 6d2e  VItem(**SVGItem.
-00000f40: 7376 675f 7061 7274 5f64 6566 6175 6c74  svg_part_default
-00000f50: 5f6b 7761 7267 7329 0d0a 2020 2020 2020  _kwargs)..      
-00000f60: 2020 2020 2020 7669 7465 6d2e 7365 745f        vitem.set_
-00000f70: 7374 796c 6528 2a2a 7669 7465 6d5f 7374  style(**vitem_st
-00000f80: 796c 6573 290d 0a20 2020 2020 2020 2020  yles)..         
-00000f90: 2020 2076 6974 656d 2e70 6f69 6e74 732e     vitem.points.
-00000fa0: 7365 7428 7669 7465 6d5f 706f 696e 7473  set(vitem_points
-00000fb0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00000fc0: 6574 7572 6e20 7669 7465 6d0d 0a0d 0a20  eturn vitem.... 
-00000fd0: 2020 2020 2020 2072 6574 7572 6e20 7669         return vi
-00000fe0: 7465 6d5f 6275 696c 6465 720d 0a         tem_builder..
+00000170: e79a 8420 332e 3237 3220 e698 afe6 898b  ... 3.272 ......
+00000180: e58a a8e8 af95 e587 bae6 9da5 e79a 840d  ................
+00000190: 0a44 4546 4155 4c54 5f53 5647 4954 454d  .DEFAULT_SVGITEM
+000001a0: 5f53 4341 4c45 5f46 4143 544f 5220 3d20  _SCALE_FACTOR = 
+000001b0: 332e 3237 320d 0a53 5452 4f4b 455f 5749  3.272..STROKE_WI
+000001c0: 4454 485f 434f 4e56 4552 5349 4f4e 203d  DTH_CONVERSION =
+000001d0: 2030 2e30 310d 0a0d 0a74 7970 6520 5649   0.01....type VI
+000001e0: 7465 6d42 7569 6c64 6572 203d 2043 616c  temBuilder = Cal
+000001f0: 6c61 626c 655b 5b5d 2c20 5649 7465 6d5d  lable[[], VItem]
+00000200: 0d0a 0d0a 0d0a 6465 6620 5f63 6f6e 7665  ......def _conve
+00000210: 7274 5f70 6f69 6e74 5f74 6f5f 3364 2878  rt_point_to_3d(x
+00000220: 3a20 666c 6f61 742c 2079 3a20 666c 6f61  : float, y: floa
+00000230: 7429 202d 3e20 6e70 2e6e 6461 7272 6179  t) -> np.ndarray
+00000240: 3a0d 0a20 2020 2072 6574 7572 6e20 6e70  :..    return np
+00000250: 2e61 7272 6179 285b 782c 2079 2c20 305d  .array([x, y, 0]
+00000260: 290d 0a0d 0a0d 0a64 6566 205f 636f 6e76  )......def _conv
+00000270: 6572 745f 616c 7068 615f 746f 5f66 6c6f  ert_alpha_to_flo
+00000280: 6174 2878 3a20 696e 7420 7c20 4e6f 6e65  at(x: int | None
+00000290: 2920 2d3e 2066 6c6f 6174 3a0d 0a20 2020  ) -> float:..   
+000002a0: 2072 6574 7572 6e20 4e6f 6e65 2069 6620   return None if 
+000002b0: 7820 6973 204e 6f6e 6520 656c 7365 2078  x is None else x
+000002c0: 202f 2032 3535 0d0a 0d0a 0d0a 636c 6173   / 255......clas
+000002d0: 7320 5356 4749 7465 6d28 4772 6f75 705b  s SVGItem(Group[
+000002e0: 5649 7465 6d5d 293a 0d0a 2020 2020 2727  VItem]):..    ''
+000002f0: 270d 0a20 2020 20e4 bca0 e585 a520 5356  '..    ...... SV
+00000300: 4720 e696 87e4 bbb6 e8b7 afe5 be84 efbc  G ..............
+00000310: 8ce8 a7a3 e69e 90e4 b8ba e789 a9e4 bbb6  ................
+00000320: 0d0a 2020 2020 2727 270d 0a20 2020 2073  ..    '''..    s
+00000330: 7667 5f70 6172 745f 6465 6661 756c 745f  vg_part_default_
+00000340: 6b77 6172 6773 203d 2064 6963 7428 0d0a  kwargs = dict(..
+00000350: 2020 2020 2020 2020 7374 726f 6b65 5f72          stroke_r
+00000360: 6164 6975 733d 312e 3020 2a20 5354 524f  adius=1.0 * STRO
+00000370: 4b45 5f57 4944 5448 5f43 4f4e 5645 5253  KE_WIDTH_CONVERS
+00000380: 494f 4e20 2f20 322c 0d0a 2020 2020 2020  ION / 2,..      
+00000390: 2020 7374 726f 6b65 5f63 6f6c 6f72 3d4e    stroke_color=N
+000003a0: 6f6e 652c 0d0a 2020 2020 2020 2020 7374  one,..        st
+000003b0: 726f 6b65 5f61 6c70 6861 3d30 2c0d 0a20  roke_alpha=0,.. 
+000003c0: 2020 2020 2020 2066 696c 6c5f 636f 6c6f         fill_colo
+000003d0: 723d 4e6f 6e65 2c0d 0a20 2020 2020 2020  r=None,..       
+000003e0: 2066 696c 6c5f 616c 7068 613d 300d 0a20   fill_alpha=0.. 
+000003f0: 2020 2029 0d0a 2020 2020 7669 7465 6d5f     )..    vitem_
+00000400: 6275 696c 6465 7273 5f6d 6170 3a20 6469  builders_map: di
+00000410: 6374 5b74 7570 6c65 2c20 6c69 7374 5b56  ct[tuple, list[V
+00000420: 4974 656d 4275 696c 6465 725d 5d20 3d20  ItemBuilder]] = 
+00000430: 7b7d 0d0a 0d0a 2020 2020 6465 6620 5f5f  {}....    def __
+00000440: 696e 6974 5f5f 2873 656c 662c 2066 696c  init__(self, fil
+00000450: 655f 7061 7468 3a20 7374 722c 202a 2a6b  e_path: str, **k
+00000460: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00000470: 2069 7465 6d73 203d 2073 656c 662e 6765   items = self.ge
+00000480: 745f 6974 656d 735f 6672 6f6d 5f66 696c  t_items_from_fil
+00000490: 6528 6669 6c65 5f70 6174 6829 0d0a 0d0a  e(file_path)....
+000004a0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+000004b0: 5f5f 696e 6974 5f5f 282a 6974 656d 732c  __init__(*items,
+000004c0: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
+000004d0: 2020 2020 2020 7365 6c66 2856 4974 656d        self(VItem
+000004e0: 292e 706f 696e 7473 2e73 6361 6c65 280d  ).points.scale(.
+000004f0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
+00000500: 6669 672e 6765 742e 7069 7865 6c5f 746f  fig.get.pixel_to
+00000510: 5f66 7261 6d65 5f72 6174 696f 202a 2044  _frame_ratio * D
+00000520: 4546 4155 4c54 5f53 5647 4954 454d 5f53  EFAULT_SVGITEM_S
+00000530: 4341 4c45 5f46 4143 544f 522c 0d0a 2020  CALE_FACTOR,..  
+00000540: 2020 2020 2020 2020 2020 6162 6f75 745f            about_
+00000550: 706f 696e 743d 4f52 4947 494e 0d0a 2020  point=ORIGIN..  
+00000560: 2020 2020 2020 292e 666c 6970 2852 4947        ).flip(RIG
+00000570: 4854 290d 0a0d 0a20 2020 2020 2020 2073  HT)....        s
+00000580: 656c 662e 6d6f 7665 5f69 6e74 6f5f 706f  elf.move_into_po
+00000590: 7369 7469 6f6e 2829 0d0a 0d0a 2020 2020  sition()....    
+000005a0: 6465 6620 6d6f 7665 5f69 6e74 6f5f 706f  def move_into_po
+000005b0: 7369 7469 6f6e 2873 656c 6629 202d 3e20  sition(self) -> 
+000005c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2070  None:..        p
+000005d0: 6173 730d 0a0d 0a20 2020 2040 7374 6174  ass....    @stat
+000005e0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
+000005f0: 6620 6765 745f 6974 656d 735f 6672 6f6d  f get_items_from
+00000600: 5f66 696c 6528 6669 6c65 5f70 6174 683a  _file(file_path:
+00000610: 2073 7472 2920 2d3e 206c 6973 745b 4974   str) -> list[It
+00000620: 656d 5d3a 0d0a 2020 2020 2020 2020 2727  em]:..        ''
+00000630: 270d 0a20 2020 2020 2020 20e8 a7a3 e69e  '..        .....
+00000640: 90e6 9687 e4bb b6e5 b9b6 e5be 97e5 88b0  ................
+00000650: e789 a9e4 bbb6 e588 97e8 a1a8 0d0a 2020  ..............  
+00000660: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+00000670: 2020 206d 7469 6d65 203d 206f 732e 7061     mtime = os.pa
+00000680: 7468 2e67 6574 6d74 696d 6528 6669 6c65  th.getmtime(file
+00000690: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+000006a0: 6e61 6d65 203d 206f 732e 7061 7468 2e73  name = os.path.s
+000006b0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+000006c0: 6261 7365 6e61 6d65 2866 696c 655f 7061  basename(file_pa
+000006d0: 7468 2929 5b30 5d0d 0a20 2020 2020 2020  th))[0]..       
+000006e0: 206b 6579 203d 2028 6e61 6d65 2c20 6d74   key = (name, mt
+000006f0: 696d 6529 0d0a 0d0a 2020 2020 2020 2020  ime)....        
+00000700: 6361 6368 6564 203d 2053 5647 4974 656d  cached = SVGItem
+00000710: 2e76 6974 656d 5f62 7569 6c64 6572 735f  .vitem_builders_
+00000720: 6d61 702e 6765 7428 6b65 792c 204e 6f6e  map.get(key, Non
+00000730: 6529 0d0a 2020 2020 2020 2020 6966 2063  e)..        if c
+00000740: 6163 6865 6420 6973 206e 6f74 204e 6f6e  ached is not Non
+00000750: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000760: 7265 7475 726e 205b 6275 696c 6465 7228  return [builder(
+00000770: 2920 666f 7220 6275 696c 6465 7220 696e  ) for builder in
+00000780: 2063 6163 6865 645d 0d0a 0d0a 2020 2020   cached]....    
+00000790: 2020 2020 7376 673a 2073 652e 5356 4720      svg: se.SVG 
+000007a0: 3d20 7365 2e53 5647 2e70 6172 7365 2866  = se.SVG.parse(f
+000007b0: 696c 655f 7061 7468 290d 0a0d 0a20 2020  ile_path)....   
+000007c0: 2020 2020 206f 6666 7365 7420 3d20 6e70       offset = np
+000007d0: 2e61 7272 6179 285b 7376 672e 7769 6474  .array([svg.widt
+000007e0: 6820 2f20 2d32 2c20 7376 672e 6865 6967  h / -2, svg.heig
+000007f0: 6874 202f 202d 325d 290d 0a0d 0a20 2020  ht / -2])....   
+00000800: 2020 2020 2062 7569 6c64 6572 733a 206c       builders: l
+00000810: 6973 745b 5649 7465 6d42 7569 6c64 6572  ist[VItemBuilder
+00000820: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
+00000830: 666f 7220 7368 6170 6520 696e 2073 7667  for shape in svg
+00000840: 2e65 6c65 6d65 6e74 7328 293a 0d0a 2020  .elements():..  
+00000850: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00000860: 6e73 7461 6e63 6528 7368 6170 652c 2028  nstance(shape, (
+00000870: 7365 2e47 726f 7570 2c20 7365 2e55 7365  se.Group, se.Use
+00000880: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00000890: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+000008a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000008b0: 6973 696e 7374 616e 6365 2873 6861 7065  isinstance(shape
+000008c0: 2c20 7365 2e50 6174 6829 3a0d 0a20 2020  , se.Path):..   
+000008d0: 2020 2020 2020 2020 2020 2020 2062 7569               bui
+000008e0: 6c64 6572 732e 6170 7065 6e64 2853 5647  lders.append(SVG
+000008f0: 4974 656d 2e63 6f6e 7665 7274 5f70 6174  Item.convert_pat
+00000900: 6828 7368 6170 652c 206f 6666 7365 7429  h(shape, offset)
+00000910: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00000920: 6c69 6620 7479 7065 2873 6861 7065 2920  lif type(shape) 
+00000930: 6973 2073 652e 5356 4745 6c65 6d65 6e74  is se.SVGElement
+00000940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000950: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+00000960: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 6c6f 672e 7761 726e 696e 6728 6627 556e  log.warning(f'Un
+00000990: 7375 7070 6f72 7465 6420 656c 656d 656e  supported elemen
+000009a0: 7420 7479 7065 3a20 7b74 7970 6528 7368  t type: {type(sh
+000009b0: 6170 6529 7d27 290d 0a0d 0a20 2020 2020  ape)}')....     
+000009c0: 2020 2053 5647 4974 656d 2e76 6974 656d     SVGItem.vitem
+000009d0: 5f62 7569 6c64 6572 735f 6d61 705b 6b65  _builders_map[ke
+000009e0: 795d 203d 2062 7569 6c64 6572 730d 0a20  y] = builders.. 
+000009f0: 2020 2020 2020 2072 6574 7572 6e20 5b62         return [b
+00000a00: 7569 6c64 6572 2829 2066 6f72 2062 7569  uilder() for bui
+00000a10: 6c64 6572 2069 6e20 6275 696c 6465 7273  lder in builders
+00000a20: 5d0d 0a0d 0a20 2020 2040 7374 6174 6963  ]....    @static
+00000a30: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+00000a40: 636f 6e76 6572 745f 7061 7468 2870 6174  convert_path(pat
+00000a50: 683a 2073 652e 5061 7468 2c20 6f66 6673  h: se.Path, offs
+00000a60: 6574 3a20 6e70 2e6e 6461 7272 6179 2920  et: np.ndarray) 
+00000a70: 2d3e 2056 4974 656d 4275 696c 6465 723a  -> VItemBuilder:
+00000a80: 0d0a 2020 2020 2020 2020 6275 696c 6465  ..        builde
+00000a90: 7220 3d20 5061 7468 4275 696c 6465 7228  r = PathBuilder(
+00000aa0: 290d 0a20 2020 2020 2020 2073 6567 6d65  )..        segme
+00000ab0: 6e74 5f63 6c61 7373 5f74 6f5f 6675 6e63  nt_class_to_func
+00000ac0: 5f6d 6170 203d 207b 0d0a 2020 2020 2020  _map = {..      
+00000ad0: 2020 2020 2020 7365 2e4d 6f76 653a 2028        se.Move: (
+00000ae0: 6275 696c 6465 722e 6d6f 7665 5f74 6f2c  builder.move_to,
+00000af0: 2028 2765 6e64 272c 2929 2c0d 0a20 2020   ('end',)),..   
+00000b00: 2020 2020 2020 2020 2073 652e 436c 6f73           se.Clos
+00000b10: 653a 2028 6275 696c 6465 722e 636c 6f73  e: (builder.clos
+00000b20: 655f 7061 7468 2c20 2829 292c 0d0a 2020  e_path, ()),..  
+00000b30: 2020 2020 2020 2020 2020 7365 2e4c 696e            se.Lin
+00000b40: 653a 2028 6275 696c 6465 722e 6c69 6e65  e: (builder.line
+00000b50: 5f74 6f2c 2028 2765 6e64 272c 2929 2c0d  _to, ('end',)),.
+00000b60: 0a20 2020 2020 2020 2020 2020 2073 652e  .            se.
+00000b70: 5175 6164 7261 7469 6342 657a 6965 723a  QuadraticBezier:
+00000b80: 2028 6275 696c 6465 722e 636f 6e69 635f   (builder.conic_
+00000b90: 746f 2c20 2827 636f 6e74 726f 6c27 2c20  to, ('control', 
+00000ba0: 2765 6e64 2729 292c 0d0a 2020 2020 2020  'end')),..      
+00000bb0: 2020 2020 2020 7365 2e43 7562 6963 4265        se.CubicBe
+00000bc0: 7a69 6572 3a20 2862 7569 6c64 6572 2e63  zier: (builder.c
+00000bd0: 7562 6963 5f74 6f2c 2028 2763 6f6e 7472  ubic_to, ('contr
+00000be0: 6f6c 3127 2c20 2763 6f6e 7472 6f6c 3227  ol1', 'control2'
+00000bf0: 2c20 2765 6e64 2729 290d 0a20 2020 2020  , 'end'))..     
+00000c00: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
+00000c10: 666f 7220 7365 676d 656e 7420 696e 2070  for segment in p
+00000c20: 6174 683a 0d0a 2020 2020 2020 2020 2020  ath:..          
+00000c30: 2020 7365 676d 656e 745f 636c 6173 7320    segment_class 
+00000c40: 3d20 7365 676d 656e 742e 5f5f 636c 6173  = segment.__clas
+00000c50: 735f 5f0d 0a20 2020 2020 2020 2020 2020  s__..           
+00000c60: 2066 756e 632c 2061 7474 725f 6e61 6d65   func, attr_name
+00000c70: 7320 3d20 7365 676d 656e 745f 636c 6173  s = segment_clas
+00000c80: 735f 746f 5f66 756e 635f 6d61 705b 7365  s_to_func_map[se
+00000c90: 676d 656e 745f 636c 6173 735d 0d0a 2020  gment_class]..  
+00000ca0: 2020 2020 2020 2020 2020 706f 696e 7473            points
+00000cb0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
+00000cc0: 2020 2020 2020 5f63 6f6e 7665 7274 5f70        _convert_p
+00000cd0: 6f69 6e74 5f74 6f5f 3364 282a 6765 7461  oint_to_3d(*geta
+00000ce0: 7474 7228 7365 676d 656e 742c 2061 7474  ttr(segment, att
+00000cf0: 725f 6e61 6d65 2929 0d0a 2020 2020 2020  r_name))..      
+00000d00: 2020 2020 2020 2020 2020 666f 7220 6174            for at
+00000d10: 7472 5f6e 616d 6520 696e 2061 7474 725f  tr_name in attr_
+00000d20: 6e61 6d65 730d 0a20 2020 2020 2020 2020  names..         
+00000d30: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00000d40: 2020 6675 6e63 282a 706f 696e 7473 290d    func(*points).
+00000d50: 0a0d 0a20 2020 2020 2020 2076 6974 656d  ...        vitem
+00000d60: 5f73 7479 6c65 7320 3d20 6469 6374 280d  _styles = dict(.
+00000d70: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00000d80: 6f6b 655f 7261 6469 7573 3d70 6174 682e  oke_radius=path.
+00000d90: 7374 726f 6b65 5f77 6964 7468 202a 2053  stroke_width * S
+00000da0: 5452 4f4b 455f 5749 4454 485f 434f 4e56  TROKE_WIDTH_CONV
+00000db0: 4552 5349 4f4e 202f 2032 2c0d 0a20 2020  ERSION / 2,..   
+00000dc0: 2020 2020 2020 2020 2073 7472 6f6b 655f           stroke_
+00000dd0: 636f 6c6f 723d 7061 7468 2e73 7472 6f6b  color=path.strok
+00000de0: 652e 6865 782c 0d0a 2020 2020 2020 2020  e.hex,..        
+00000df0: 2020 2020 7374 726f 6b65 5f61 6c70 6861      stroke_alpha
+00000e00: 3d5f 636f 6e76 6572 745f 616c 7068 615f  =_convert_alpha_
+00000e10: 746f 5f66 6c6f 6174 2870 6174 682e 7374  to_float(path.st
+00000e20: 726f 6b65 2e61 6c70 6861 292c 0d0a 2020  roke.alpha),..  
+00000e30: 2020 2020 2020 2020 2020 6669 6c6c 5f63            fill_c
+00000e40: 6f6c 6f72 3d70 6174 682e 6669 6c6c 2e68  olor=path.fill.h
+00000e50: 6578 2c0d 0a20 2020 2020 2020 2020 2020  ex,..           
+00000e60: 2066 696c 6c5f 616c 7068 613d 5f63 6f6e   fill_alpha=_con
+00000e70: 7665 7274 5f61 6c70 6861 5f74 6f5f 666c  vert_alpha_to_fl
+00000e80: 6f61 7428 7061 7468 2e66 696c 6c2e 616c  oat(path.fill.al
+00000e90: 7068 6129 0d0a 2020 2020 2020 2020 290d  pha)..        ).
+00000ea0: 0a20 2020 2020 2020 2076 6974 656d 5f70  .        vitem_p
+00000eb0: 6f69 6e74 7320 3d20 6275 696c 6465 722e  oints = builder.
+00000ec0: 6765 7428 290d 0a20 2020 2020 2020 2076  get()..        v
+00000ed0: 6974 656d 5f70 6f69 6e74 735b 3a2c 203a  item_points[:, :
+00000ee0: 325d 202b 3d20 6f66 6673 6574 0d0a 0d0a  2] += offset....
+00000ef0: 2020 2020 2020 2020 6465 6620 7669 7465          def vite
+00000f00: 6d5f 6275 696c 6465 7228 2920 2d3e 2056  m_builder() -> V
+00000f10: 4974 656d 3a0d 0a20 2020 2020 2020 2020  Item:..         
+00000f20: 2020 2076 6974 656d 203d 2056 4974 656d     vitem = VItem
+00000f30: 282a 2a53 5647 4974 656d 2e73 7667 5f70  (**SVGItem.svg_p
+00000f40: 6172 745f 6465 6661 756c 745f 6b77 6172  art_default_kwar
+00000f50: 6773 290d 0a20 2020 2020 2020 2020 2020  gs)..           
+00000f60: 2076 6974 656d 2e73 6574 5f73 7479 6c65   vitem.set_style
+00000f70: 282a 2a76 6974 656d 5f73 7479 6c65 7329  (**vitem_styles)
+00000f80: 0d0a 2020 2020 2020 2020 2020 2020 7669  ..            vi
+00000f90: 7465 6d2e 706f 696e 7473 2e73 6574 2876  tem.points.set(v
+00000fa0: 6974 656d 5f70 6f69 6e74 7329 0d0a 2020  item_points)..  
+00000fb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000fc0: 2076 6974 656d 0d0a 0d0a 2020 2020 2020   vitem....      
+00000fd0: 2020 7265 7475 726e 2076 6974 656d 5f62    return vitem_b
+00000fe0: 7569 6c64 6572 0d0a                      uilder..
```

### Comparing `janim-0.4.0/janim/items/svg/typst.py` & `janim-0.5.0/janim/items/svg/typst.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,40 +126,69 @@
 000007d0: 7572 6e20 7376 675f 6669 6c65 5f70 6174  urn svg_file_pat
 000007e0: 680d 0a0d 0a0d 0a63 6c61 7373 2054 7970  h......class Typ
 000007f0: 7374 2854 7970 7374 446f 6329 3a0d 0a20  st(TypstDoc):.. 
 00000800: 2020 2027 2727 0d0a 2020 2020 5479 7073     '''..    Typs
 00000810: 7420 e585 ace5 bc8f 0d0a 2020 2020 2727  t ........    ''
 00000820: 270d 0a20 2020 2064 6566 205f 5f69 6e69  '..    def __ini
 00000830: 745f 5f28 7365 6c66 2c20 7465 7874 3a20  t__(self, text: 
-00000840: 7374 722c 202a 2a6b 7761 7267 7329 3a0d  str, **kwargs):.
-00000850: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00000860: 2e5f 5f69 6e69 745f 5f28 6627 2420 7b74  .__init__(f'$ {t
-00000870: 6578 747d 2024 272c 202a 2a6b 7761 7267  ext} $', **kwarg
-00000880: 7329 0d0a 0d0a 2020 2020 6465 6620 6d6f  s)....    def mo
-00000890: 7665 5f69 6e74 6f5f 706f 7369 7469 6f6e  ve_into_position
-000008a0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
-000008b0: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-000008c0: 696e 7473 2e74 6f5f 6365 6e74 6572 2829  ints.to_center()
-000008d0: 0d0a 0d0a 0d0a 6361 6368 6564 5f74 7970  ......cached_typ
-000008e0: 7374 5f74 656d 706c 6174 653a 2073 7472  st_template: str
-000008f0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 0d0a   | None = None..
-00000900: 0d0a 0d0a 6465 6620 6765 745f 7479 7073  ....def get_typs
-00000910: 745f 7465 6d70 6c61 7465 2829 202d 3e20  t_template() -> 
-00000920: 7374 723a 0d0a 2020 2020 676c 6f62 616c  str:..    global
-00000930: 2063 6163 6865 645f 7479 7073 745f 7465   cached_typst_te
-00000940: 6d70 6c61 7465 0d0a 0d0a 2020 2020 6966  mplate....    if
-00000950: 2063 6163 6865 645f 7479 7073 745f 7465   cached_typst_te
-00000960: 6d70 6c61 7465 2069 7320 6e6f 7420 4e6f  mplate is not No
-00000970: 6e65 3a0d 0a20 2020 2020 2020 2072 6574  ne:..        ret
-00000980: 7572 6e20 6361 6368 6564 5f74 7970 7374  urn cached_typst
-00000990: 5f74 656d 706c 6174 650d 0a0d 0a20 2020  _template....   
-000009a0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
-000009b0: 7468 2e6a 6f69 6e28 6765 745f 6a61 6e69  th.join(get_jani
-000009c0: 6d5f 6469 7228 292c 2027 6974 656d 7327  m_dir(), 'items'
-000009d0: 2c20 2773 7667 272c 2027 7479 7073 745f  , 'svg', 'typst_
-000009e0: 7465 6d70 6c61 7465 2e74 7970 2729 2920  template.typ')) 
-000009f0: 6173 2066 3a0d 0a20 2020 2020 2020 2074  as f:..        t
-00000a00: 6578 7420 3d20 662e 7265 6164 2829 0d0a  ext = f.read()..
-00000a10: 0d0a 2020 2020 6361 6368 6564 5f74 7970  ..    cached_typ
-00000a20: 7374 5f74 656d 706c 6174 6520 3d20 7465  st_template = te
-00000a30: 7874 0d0a 2020 2020 7265 7475 726e 2074  xt..    return t
-00000a40: 6578 740d 0a                             ext..
+00000840: 7374 722c 202a 2c20 7573 655f 6d61 7468  str, *, use_math
+00000850: 5f65 6e76 6972 6f6e 6d65 6e74 3a20 626f  _environment: bo
+00000860: 6f6c 203d 2054 7275 652c 202a 2a6b 7761  ol = True, **kwa
+00000870: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
+00000880: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00000890: 0d0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+000008a0: 2420 7b74 6578 747d 2024 2720 6966 2075  $ {text} $' if u
+000008b0: 7365 5f6d 6174 685f 656e 7669 726f 6e6d  se_math_environm
+000008c0: 656e 7420 656c 7365 2074 6578 742c 0d0a  ent else text,..
+000008d0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+000008e0: 6172 6773 0d0a 2020 2020 2020 2020 290d  args..        ).
+000008f0: 0a0d 0a20 2020 2064 6566 206d 6f76 655f  ...    def move_
+00000900: 696e 746f 5f70 6f73 6974 696f 6e28 7365  into_position(se
+00000910: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
+00000920: 2020 2020 2020 7365 6c66 2e70 6f69 6e74        self.point
+00000930: 732e 746f 5f63 656e 7465 7228 290d 0a0d  s.to_center()...
+00000940: 0a0d 0a63 6c61 7373 2054 7970 7374 5465  ...class TypstTe
+00000950: 7874 2854 7970 7374 293a 0d0a 2020 2020  xt(Typst):..    
+00000960: 2727 270d 0a20 2020 2054 7970 7374 20e6  '''..    Typst .
+00000970: 9687 e69c ac0d 0a0d 0a20 2020 20e7 9bb8  .........    ...
+00000980: e5bd 93e4 ba8e 203a 636c 6173 733a 6054  ...... :class:`T
+00000990: 7970 7374 6020 e4bc a0e5 85a5 2060 6075  ypst` ...... ``u
+000009a0: 7365 5f6d 6174 685f 656e 7669 726f 6e6d  se_math_environm
+000009b0: 656e 743d 4661 6c73 6560 600d 0a20 2020  ent=False``..   
+000009c0: 2027 2727 0d0a 2020 2020 6465 6620 5f5f   '''..    def __
+000009d0: 696e 6974 5f5f 2873 656c 662c 2074 6578  init__(self, tex
+000009e0: 743a 2073 7472 2c20 7573 655f 6d61 7468  t: str, use_math
+000009f0: 5f65 6e76 6972 6f6e 6d65 6e74 3a20 626f  _environment: bo
+00000a00: 6f6c 203d 2046 616c 7365 2c20 2a2a 6b77  ol = False, **kw
+00000a10: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00000a20: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00000a30: 280d 0a20 2020 2020 2020 2020 2020 2074  (..            t
+00000a40: 6578 742c 0d0a 2020 2020 2020 2020 2020  ext,..          
+00000a50: 2020 7573 655f 6d61 7468 5f65 6e76 6972    use_math_envir
+00000a60: 6f6e 6d65 6e74 3d75 7365 5f6d 6174 685f  onment=use_math_
+00000a70: 656e 7669 726f 6e6d 656e 742c 0d0a 2020  environment,..  
+00000a80: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+00000a90: 6773 0d0a 2020 2020 2020 2020 290d 0a0d  gs..        )...
+00000aa0: 0a0d 0a63 6163 6865 645f 7479 7073 745f  ...cached_typst_
+00000ab0: 7465 6d70 6c61 7465 3a20 7374 7220 7c20  template: str | 
+00000ac0: 4e6f 6e65 203d 204e 6f6e 650d 0a0d 0a0d  None = None.....
+00000ad0: 0a64 6566 2067 6574 5f74 7970 7374 5f74  .def get_typst_t
+00000ae0: 656d 706c 6174 6528 2920 2d3e 2073 7472  emplate() -> str
+00000af0: 3a0d 0a20 2020 2067 6c6f 6261 6c20 6361  :..    global ca
+00000b00: 6368 6564 5f74 7970 7374 5f74 656d 706c  ched_typst_templ
+00000b10: 6174 650d 0a0d 0a20 2020 2069 6620 6361  ate....    if ca
+00000b20: 6368 6564 5f74 7970 7374 5f74 656d 706c  ched_typst_templ
+00000b30: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
+00000b40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b50: 2063 6163 6865 645f 7479 7073 745f 7465   cached_typst_te
+00000b60: 6d70 6c61 7465 0d0a 0d0a 2020 2020 7769  mplate....    wi
+00000b70: 7468 206f 7065 6e28 6f73 2e70 6174 682e  th open(os.path.
+00000b80: 6a6f 696e 2867 6574 5f6a 616e 696d 5f64  join(get_janim_d
+00000b90: 6972 2829 2c20 2769 7465 6d73 272c 2027  ir(), 'items', '
+00000ba0: 7376 6727 2c20 2774 7970 7374 5f74 656d  svg', 'typst_tem
+00000bb0: 706c 6174 652e 7479 7027 2929 2061 7320  plate.typ')) as 
+00000bc0: 663a 0d0a 2020 2020 2020 2020 7465 7874  f:..        text
+00000bd0: 203d 2066 2e72 6561 6428 290d 0a0d 0a20   = f.read().... 
+00000be0: 2020 2063 6163 6865 645f 7479 7073 745f     cached_typst_
+00000bf0: 7465 6d70 6c61 7465 203d 2074 6578 740d  template = text.
+00000c00: 0a20 2020 2072 6574 7572 6e20 7465 7874  .    return text
+00000c10: 0d0a                                     ..
```

### Comparing `janim-0.4.0/janim/items/text/text.py` & `janim-0.5.0/janim/items/text/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,15 +263,21 @@
         stroke_alpha: float = 0,
         fill_alpha: float = 1,
         **kwargs
     ) -> None:
         # 获取字体
         if isinstance(font, str):
             font = [font]
-        font.append(Config.get.font)
+
+        cfg_font = Config.get.font
+        if isinstance(cfg_font, str):
+            font.append(cfg_font)
+        else:
+            font.extend(cfg_font)
+
         fonts = [
             Font.get(get_fontpath_by_name(name))
             for name in font
         ]
 
         if format is not Text.Format.RichText:
             self.text = text
```

### Comparing `janim-0.4.0/janim/items/value_tracker.py` & `janim-0.5.0/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/items/vitem.py` & `janim-0.5.0/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/render/base.py` & `janim-0.5.0/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/render/impl.py` & `janim-0.5.0/janim/render/impl.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/render/shaders/dotcloud.geom.glsl` & `janim-0.5.0/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/render/shaders/vitem.frag.glsl` & `janim-0.5.0/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/render/texture.py` & `janim-0.5.0/janim/render/texture.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/typing.py` & `janim-0.5.0/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/bezier.py` & `janim-0.5.0/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/config.py` & `janim-0.5.0/janim/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 import tempfile
 from contextvars import ContextVar
 from dataclasses import dataclass
-from typing import Self
+from typing import Iterable, Self
 
 import psutil
 from colour import Color
 
 from janim.constants import DOWN, LEFT, RIGHT, UP
 from janim.typing import Vect
 
@@ -40,21 +40,23 @@
 
     其中没有设置的属性则采用默认设置 :py:obj:`~.default_config`
     '''
     fps: int = None
     preview_fps: int = None
     anti_alias_width: float = None
 
-    aspect_ratio: float = None
     frame_height: float = None
+    frame_width: float = None
 
     pixel_height: int = None
     pixel_width: int = None
     background_color: Color = None
-    font: str = None
+    font: str | Iterable[str] = None
+
+    audio_framerate: int = None
 
     wnd_pos: str = None
     wnd_monitor: int = None
 
     typst_bin: str = None
 
     ffmpeg_bin: str = None
@@ -76,22 +78,24 @@
 
 
 default_config = Config(
     fps=60,
     preview_fps=60 if is_power_plugged() else 30,
     anti_alias_width=0.015,
 
-    aspect_ratio=16.0 / 9.0,
     frame_height=8.0,
+    frame_width=16.0 / 9.0 * 8.0,   # aspect_ratio(16/9) * frame_height
 
     pixel_height=1080,
     pixel_width=1920,
     background_color=Color('#000000'),
     font='Consolas',
 
+    audio_framerate=44100,
+
     wnd_pos='OR',
     wnd_monitor=0,
 
     typst_bin='typst',
 
     ffmpeg_bin='ffmpeg',
     output_dir='videos',
@@ -111,26 +115,29 @@
 
 class ConfigGetter:
     '''
     与配置数据相关联的数据的获取
 
     请仍然使用 ``Config.get.xxx`` 来获取定义在该类中的内容
     '''
+    def __init__(self, config_ctx: list[Config] | None = None):
+        self.config_ctx = config_ctx
+
     def __getattr__(self, name: str) -> None:
-        lst = config_ctx_var.get()
+        lst = self.config_ctx or config_ctx_var.get()
         for config in reversed(lst):
             value = getattr(config, name)
             if value is not None:
                 return value
 
         return None
 
     @property
-    def frame_width(self) -> float:
-        return Config.get.aspect_ratio * Config.get.frame_height
+    def aspect_ratio(self) -> float:
+        return Config.get.frame_width / Config.get.frame_height
 
     @property
     def frame_x_radius(self) -> float:
         return Config.get.frame_width / 2
 
     @property
     def frame_y_radius(self) -> float:
```

### Comparing `janim-0.4.0/janim/utils/dict_ops.py` & `janim-0.5.0/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/file_ops.py` & `janim-0.5.0/janim/utils/file_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import importlib.util
 import os
 
-from janim.utils.config import Config
-
 
 def guarantee_existence(path: str) -> str:
     if not os.path.exists(path):
         os.makedirs(path)
     return os.path.abspath(path)
 
 
@@ -14,14 +12,15 @@
     '''
     得到 janim 的路径
     '''
     return os.path.dirname(importlib.util.find_spec('janim').origin)
 
 
 def get_typst_temp_dir() -> str:
+    from janim.utils.config import Config
     return guarantee_existence(os.path.join(Config.get.temp_dir, 'Typst'))
 
 
 def readall(filepath: str) -> str:
     '''
     从文件中读取所有字符
     '''
```

### Comparing `janim-0.4.0/janim/utils/font.py` & `janim-0.5.0/janim/utils/font.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 @lru_cache()
 def get_fontpath_by_name(font_name: str) -> str:
     '''
     通过字体名得到字体文件路径
 
-    例：通过 `Consolas` 得到 `C:\\Windows\\Fonts\\consola.ttf`
+    例：通过 ``Consolas`` 得到 ``C:\\Windows\\Fonts\\consola.ttf``
     '''
     global fontpaths
 
     if fontpaths is None:
         from janim.utils.font_manager import findSystemFonts
         fontpaths = findSystemFonts()
```

### Comparing `janim-0.4.0/janim/utils/font_manager.py` & `janim-0.5.0/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/iterables.py` & `janim-0.5.0/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/paths.py` & `janim-0.5.0/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/rate_functions.py` & `janim-0.5.0/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/refresh.py` & `janim-0.5.0/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/signal.py` & `janim-0.5.0/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/simple_functions.py` & `janim-0.5.0/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/space_ops.py` & `janim-0.5.0/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/janim/utils/unique_nparray.py` & `janim-0.5.0/janim/utils/unique_nparray.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         self._dtype = dtype
 
     def len(self) -> int:
         return len(self._data)
 
     @property
     def data(self) -> np.ndarray:
+        # TODO: Optimize by setting WRITEABLE=False
         return self._data.copy()
 
     @data.setter
     def data(self, data: np.ndarray | Iterable) -> None:
         if not isinstance(data, np.ndarray):
             self._data = np.array(data, dtype=self._dtype)
         else:
```

### Comparing `janim-0.4.0/logo.png` & `janim-0.5.0/logo.png`

 * *Files identical despite different names*

### Comparing `janim-0.4.0/pyproject.toml` & `janim-0.5.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 ]
 
 [project.optional-dependencies]
 gui = [
     "pyside6",
     "qdarkstyle",
     "beautifulsoup4",
+    "pyaudio",
 ]
 doc = [
     "sphinx",
+    "sphinx-copybutton",
     "furo",
     "jinja2",
     "docutils",
 ]
 
 [tool.flit.sdist]
 exclude = ["doc/", "test/"]
```

### Comparing `janim-0.4.0/PKG-INFO` & `janim-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 0.4.0
+Version: 0.5.0
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -15,20 +15,22 @@
 Requires-Dist: psutil
 Requires-Dist: skia-pathops
 Requires-Dist: fontTools
 Requires-Dist: freetype-py
 Requires-Dist: pillow
 Requires-Dist: svgelements
 Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: jinja2 ; extra == "doc"
 Requires-Dist: docutils ; extra == "doc"
 Requires-Dist: pyside6 ; extra == "gui"
 Requires-Dist: qdarkstyle ; extra == "gui"
 Requires-Dist: beautifulsoup4 ; extra == "gui"
+Requires-Dist: pyaudio ; extra == "gui"
 Project-URL: Documentation, https://janim.rtfd.io
 Project-URL: Home, https://github.com/jkjkil4/JAnim
 Project-URL: Source, https://github.com/jkjkil4/JAnim
 Provides-Extra: doc
 Provides-Extra: gui
 
 ![logo](logo.png)
```

