# Comparing `tmp/ansys_geometry_core-0.4.9.tar.gz` & `tmp/ansys_geometry_core-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_geometry_core-0.4.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_geometry_core-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_geometry_core-0.4.9.tar` & `ansys_geometry_core-0.5.0.tar`

### file list

```diff
@@ -1,103 +1,113 @@
--rw-r--r--   0        0        0     1089 2024-02-02 12:23:34.631900 ansys_geometry_core-0.4.9/LICENSE
--rw-r--r--   0        0        0     4881 2024-02-02 12:23:34.631900 ansys_geometry_core-0.4.9/README.rst
--rw-r--r--   0        0        0     3677 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/__init__.py
--rw-r--r--   0        0        0     2357 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/__init__.py
--rw-r--r--   0        0        0     1602 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/backend.py
--rw-r--r--   0        0        0    11484 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/client.py
--rw-r--r--   0        0        0    13467 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/conversions.py
--rw-r--r--   0        0        0     2483 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/defaults.py
--rw-r--r--   0        0        0    13771 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/docker_instance.py
--rw-r--r--   0        0        0    28232 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/launcher.py
--rw-r--r--   0        0        0      167 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/pim_configuration.json
--rw-r--r--   0        0        0    15601 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/product_instance.py
--rw-r--r--   0        0        0     1746 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/validate.py
--rw-r--r--   0        0        0     1762 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/__init__.py
--rw-r--r--   0        0        0     7898 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/beam.py
--rw-r--r--   0        0        0    39765 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/body.py
--rw-r--r--   0        0        0    42986 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/component.py
--rw-r--r--   0        0        0     6034 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/coordinate_system.py
--rw-r--r--   0        0        0    30616 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/design.py
--rw-r--r--   0        0        0     3697 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/designpoint.py
--rw-r--r--   0        0        0     4884 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/edge.py
--rw-r--r--   0        0        0    11027 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/face.py
--rw-r--r--   0        0        0     5448 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/part.py
--rw-r--r--   0        0        0     4686 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/selection.py
--rw-r--r--   0        0        0     4101 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/errors.py
--rw-r--r--   0        0        0    22524 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/logger.py
--rw-r--r--   0        0        0     1349 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/__init__.py
--rw-r--r--   0        0        0     3268 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/material.py
--rw-r--r--   0        0        0     4107 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/property.py
--rw-r--r--   0        0        0     1883 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/__init__.py
--rw-r--r--   0        0        0     6819 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/bbox.py
--rw-r--r--   0        0        0     3259 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/constants.py
--rw-r--r--   0        0        0     7035 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/frame.py
--rw-r--r--   0        0        0     4816 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/matrix.py
--rw-r--r--   0        0        0     4240 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/plane.py
--rw-r--r--   0        0        0    12120 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/point.py
--rw-r--r--   0        0        0    18024 2024-02-02 12:23:34.635900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/vector.py
--rw-r--r--   0        0        0     1786 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/__init__.py
--rw-r--r--   0        0        0     6766 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/accuracy.py
--rw-r--r--   0        0        0     9486 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/checks.py
--rw-r--r--   0        0        0     8253 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/measurements.py
--rw-r--r--   0        0        0     2291 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/options.py
--rw-r--r--   0        0        0     3684 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/units.py
--rw-r--r--   0        0        0    14849 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/modeler.py
--rw-r--r--   0        0        0     1417 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/__init__.py
--rw-r--r--   0        0        0    22177 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotter.py
--rw-r--r--   0        0        0    14013 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotter_helper.py
--rw-r--r--   0        0        0     5826 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotting_types.py
--rw-r--r--   0        0        0     2816 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/trame_gui.py
--rw-r--r--   0        0        0     1710 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     3058 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/button.py
--rw-r--r--   0        0        0     4239 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3626 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/measure.py
--rw-r--r--   0        0        0     3700 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/ruler.py
--rw-r--r--   0        0        0     3480 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/show_design_point.py
--rw-r--r--   0        0        0     3348 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/view_button.py
--rw-r--r--   0        0        0     2305 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/widget.py
--rw-r--r--   0        0        0     1911 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/__init__.py
--rw-r--r--   0        0        0    11271 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/circle.py
--rw-r--r--   0        0        0    14148 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/cone.py
--rw-r--r--   0        0        0     2767 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/curve_evaluation.py
--rw-r--r--   0        0        0    14563 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/cylinder.py
--rw-r--r--   0        0        0    13933 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/ellipse.py
--rw-r--r--   0        0        0     8529 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/line.py
--rw-r--r--   0        0        0     7332 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/parameterization.py
--rw-r--r--   0        0        0    13065 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/sphere.py
--rw-r--r--   0        0        0     4282 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/surface_evaluation.py
--rw-r--r--   0        0        0    15858 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/torus.py
--rw-r--r--   0        0        0     1909 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/__init__.py
--rw-r--r--   0        0        0    11643 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/arc.py
--rw-r--r--   0        0        0     6690 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/box.py
--rw-r--r--   0        0        0     5136 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/circle.py
--rw-r--r--   0        0        0     2971 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/edge.py
--rw-r--r--   0        0        0     7731 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/ellipse.py
--rw-r--r--   0        0        0     2998 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/face.py
--rw-r--r--   0        0        0    19590 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/gears.py
--rw-r--r--   0        0        0     6063 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/polygon.py
--rw-r--r--   0        0        0     6073 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/segment.py
--rw-r--r--   0        0        0    31342 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/sketch.py
--rw-r--r--   0        0        0     6878 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/slot.py
--rw-r--r--   0        0        0     8286 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/trapezoid.py
--rw-r--r--   0        0        0     3847 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/triangle.py
--rw-r--r--   0        0        0     1477 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/__init__.py
--rw-r--r--   0        0        0    11601 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/problem_areas.py
--rw-r--r--   0        0        0     2429 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/repair_tool_message.py
--rw-r--r--   0        0        0     9289 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/repair_tools.py
--rw-r--r--   0        0        0     1670 2024-02-02 12:23:34.639900 ansys_geometry_core-0.4.9/src/ansys/geometry/core/typing.py
--rw-r--r--   0        0        0     8857 1970-01-01 00:00:00.000000 ansys_geometry_core-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-17 07:07:51.897322 ansys_geometry_core-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5051 2024-04-17 07:07:51.897322 ansys_geometry_core-0.5.0/README.rst
+-rw-r--r--   0        0        0     4395 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/__init__.py
+-rw-r--r--   0        0        0     2477 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/backend.py
+-rw-r--r--   0        0        0    12286 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/client.py
+-rw-r--r--   0        0        0    18876 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/conversions.py
+-rw-r--r--   0        0        0     2483 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/defaults.py
+-rw-r--r--   0        0        0    13911 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/docker_instance.py
+-rw-r--r--   0        0        0    28218 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/launcher.py
+-rw-r--r--   0        0        0      167 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/pim_configuration.json
+-rw-r--r--   0        0        0    16343 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/product_instance.py
+-rw-r--r--   0        0        0     1776 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/validate.py
+-rw-r--r--   0        0        0     1782 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/__init__.py
+-rw-r--r--   0        0        0     7898 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/beam.py
+-rw-r--r--   0        0        0    46126 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/body.py
+-rw-r--r--   0        0        0    52507 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/component.py
+-rw-r--r--   0        0        0     6034 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/coordinate_system.py
+-rw-r--r--   0        0        0    33930 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/design.py
+-rw-r--r--   0        0        0     3697 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/designpoint.py
+-rw-r--r--   0        0        0     6069 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/edge.py
+-rw-r--r--   0        0        0    13956 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/face.py
+-rw-r--r--   0        0        0     5468 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/part.py
+-rw-r--r--   0        0        0     4686 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/selection.py
+-rw-r--r--   0        0        0     4101 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/errors.py
+-rw-r--r--   0        0        0    22524 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/logger.py
+-rw-r--r--   0        0        0     1349 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/material.py
+-rw-r--r--   0        0        0     4107 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/property.py
+-rw-r--r--   0        0        0     1883 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/bbox.py
+-rw-r--r--   0        0        0     3259 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/constants.py
+-rw-r--r--   0        0        0     7035 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/frame.py
+-rw-r--r--   0        0        0     4823 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/matrix.py
+-rw-r--r--   0        0        0     4240 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/plane.py
+-rw-r--r--   0        0        0    12120 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/point.py
+-rw-r--r--   0        0        0    18024 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/vector.py
+-rw-r--r--   0        0        0     2085 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/__init__.py
+-rw-r--r--   0        0        0     8033 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/accuracy.py
+-rw-r--r--   0        0        0     5215 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/auxiliary.py
+-rw-r--r--   0        0        0    12180 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/checks.py
+-rw-r--r--   0        0        0     8253 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/measurements.py
+-rw-r--r--   0        0        0     2291 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/options.py
+-rw-r--r--   0        0        0     3684 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/units.py
+-rw-r--r--   0        0        0    17075 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/modeler.py
+-rw-r--r--   0        0        0     1417 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/__init__.py
+-rw-r--r--   0        0        0    22179 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter.py
+-rw-r--r--   0        0        0    14013 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter_helper.py
+-rw-r--r--   0        0        0     5826 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotting_types.py
+-rw-r--r--   0        0        0     2816 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/trame_gui.py
+-rw-r--r--   0        0        0     1710 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     3058 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/button.py
+-rw-r--r--   0        0        0     4239 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3626 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/measure.py
+-rw-r--r--   0        0        0     3700 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/ruler.py
+-rw-r--r--   0        0        0     3480 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/show_design_point.py
+-rw-r--r--   0        0        0     3348 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/view_button.py
+-rw-r--r--   0        0        0     2305 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/widget.py
+-rw-r--r--   0        0        0     2176 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/__init__.py
+-rw-r--r--   0        0        0     5634 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/box_uv.py
+-rw-r--r--   0        0        0     1580 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/__init__.py
+-rw-r--r--   0        0        0    11617 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/circle.py
+-rw-r--r--   0        0        0     3539 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve.py
+-rw-r--r--   0        0        0     2767 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
+-rw-r--r--   0        0        0    14319 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/ellipse.py
+-rw-r--r--   0        0        0     8893 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/line.py
+-rw-r--r--   0        0        0     7428 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
+-rw-r--r--   0        0        0    13001 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/parameterization.py
+-rw-r--r--   0        0        0     1746 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/__init__.py
+-rw-r--r--   0        0        0    14274 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cone.py
+-rw-r--r--   0        0        0    14748 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cylinder.py
+-rw-r--r--   0        0        0     8067 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/plane.py
+-rw-r--r--   0        0        0    13257 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/sphere.py
+-rw-r--r--   0        0        0     3467 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface.py
+-rw-r--r--   0        0        0     4281 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
+-rw-r--r--   0        0        0    16027 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/torus.py
+-rw-r--r--   0        0        0     5694 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
+-rw-r--r--   0        0        0     1909 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/__init__.py
+-rw-r--r--   0        0        0    11643 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/arc.py
+-rw-r--r--   0        0        0     6690 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/box.py
+-rw-r--r--   0        0        0     5139 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/circle.py
+-rw-r--r--   0        0        0     2991 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/edge.py
+-rw-r--r--   0        0        0     7734 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/ellipse.py
+-rw-r--r--   0        0        0     3018 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/face.py
+-rw-r--r--   0        0        0    19590 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/gears.py
+-rw-r--r--   0        0        0     6063 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/polygon.py
+-rw-r--r--   0        0        0     6076 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/segment.py
+-rw-r--r--   0        0        0    31342 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/sketch.py
+-rw-r--r--   0        0        0     6878 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/slot.py
+-rw-r--r--   0        0        0     8286 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/trapezoid.py
+-rw-r--r--   0        0        0     3847 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/triangle.py
+-rw-r--r--   0        0        0     1550 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/__init__.py
+-rw-r--r--   0        0        0     3856 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/measurement_tools.py
+-rw-r--r--   0        0        0    14367 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/problem_areas.py
+-rw-r--r--   0        0        0     2429 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tool_message.py
+-rw-r--r--   0        0        0    10524 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tools.py
+-rw-r--r--   0        0        0     1670 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/typing.py
+-rw-r--r--   0        0        0     9057 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.0/PKG-INFO
```

### Comparing `ansys_geometry_core-0.4.9/LICENSE` & `ansys_geometry_core-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/README.rst` & `ansys_geometry_core-0.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/ansys/pyansys-geometry/actions/workflows/ci_cd.yml/badge.svg
    :target: https://github.com/ansys/pyansys-geometry/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
+   :target: https://opensource.org/blog/license/mit
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyansys-geometry/main.svg
@@ -68,14 +68,15 @@
 ^^^^^^^^^^^
 
 This code shows how to import PyAnsys Geometry and use some basic capabilities:
 
 .. code:: python
 
    from ansys.geometry.core import launch_modeler
+   from ansys.geometry.core.designer import DesignFileFormat
    from ansys.geometry.core.math import Plane, Point3D, Point2D
    from ansys.geometry.core.misc import UNITS, Distance
    from ansys.geometry.core.sketch import Sketch
 
    # Define a sketch
    origin = Point3D([0, 0, 10])
    plane = Plane(origin, direction_x=[1, 0, 0], direction_y=[0, 1, 0])
@@ -95,14 +96,17 @@
    body = design.extrude_sketch(
        name="CylinderBody", sketch=sketch, distance=Distance(80, unit=UNITS.m)
    )
 
    # Plot the body
    design.plot()
 
+   # Download the model
+   design.download(file_location="file.scdocx", format=DesignFileFormat.SCDOCX)
+
 For comprehensive usage information, see `Examples`_ in the `PyAnsys Geometry documentation`_.
 
 Documentation and issues
 ^^^^^^^^^^^^^^^^^^^^^^^^
 Documentation for the latest stable release of PyAnsys Geometry is hosted at `PyAnsys Geometry documentation`_.
 
 In the upper right corner of the documentation's title bar, there is an option for switching from
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,25 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """PyAnsys Geometry connection subpackage."""
 
 from ansys.geometry.core.connection.backend import ApiVersions, BackendType
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.conversions import (
+    curve_to_grpc_curve,
     frame_to_grpc_frame,
+    grpc_curve_to_curve,
     grpc_frame_to_frame,
     grpc_matrix_to_matrix,
+    grpc_surface_to_surface,
     plane_to_grpc_plane,
     point3d_to_grpc_point,
     sketch_shapes_to_grpc_geometries,
     tess_to_pd,
+    trimmed_curve_to_grpc_trimmed_curve,
     unit_vector_to_grpc_direction,
 )
 from ansys.geometry.core.connection.defaults import (
     DEFAULT_HOST,
     DEFAULT_PORT,
     GEOMETRY_SERVICE_DOCKER_IMAGE,
 )
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/backend.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 class ApiVersions(Enum):
     """Provides an enum for all the compatibles API versions."""
 
     V_21 = 21
     V_22 = 22
     V_231 = 231
     V_232 = 232
-    V_241 = LATEST = 241
+    V_241 = 241
+    V_242 = LATEST = 242
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/client.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,17 +165,20 @@
         if logging_file:
             if isinstance(logging_file, Path):
                 logging_file = str(logging_file)
             self._log.log_to_file(filename=logging_file, level=logging_level)
 
         self._admin_stub = AdminStub(self._channel)
 
+        # retrieve the backend information
+        grpc_backend_response = self._admin_stub.GetBackend(Empty())
+
         # if no backend type has been specified, ask the backend which type it is
         if backend_type == None:
-            grpc_backend_type = self._admin_stub.GetBackend(Empty()).type
+            grpc_backend_type = grpc_backend_response.type
             if grpc_backend_type == GRPCBackendType.DISCOVERY:
                 backend_type = BackendType.DISCOVERY
             elif grpc_backend_type == GRPCBackendType.SPACECLAIM:
                 backend_type = BackendType.SPACECLAIM
             elif grpc_backend_type == GRPCBackendType.WINDOWS_DMS:
                 backend_type = BackendType.WINDOWS_SERVICE
             elif grpc_backend_type == GRPCBackendType.LINUX_DMS:
@@ -183,14 +186,22 @@
 
         # Store the backend type
         self._backend_type = backend_type
         self._multiple_designs_allowed = (
             False if backend_type in (BackendType.DISCOVERY, BackendType.LINUX_SERVICE) else True
         )
 
+        # retrieve the backend version
+        if hasattr(grpc_backend_response, "version"):
+            ver = grpc_backend_response.version
+            self._backend_version = f"{ver.major_release}.{ver.minor_release}.{ver.service_pack}"
+        else:
+            logger.warning("The backend version is only available after 24.1 version.")
+            self._backend_version = "24.1.0"
+
     @property
     def backend_type(self) -> BackendType:
         """
         Backend type.
 
         Options are ``Windows Service``, ``Linux Service``, ``Discovery``,
         and ``SpaceClaim``.
@@ -199,14 +210,27 @@
         -----
         This method might return ``None`` because determining the backend type is
         not straightforward.
         """
         return self._backend_type
 
     @property
+    def backend_version(self) -> str:
+        """
+        Get the current backend version.
+
+        Returns
+        -------
+        str
+            Backend version in semantic versioning format (that is, Ansys 24R1 SP2
+            would be ``24.1.2``).
+        """
+        return self._backend_version
+
+    @property
     def multiple_designs_allowed(self) -> bool:
         """
         Flag indicating whether multiple designs are allowed.
 
         Notes
         -----
         This method will return ``False`` if the backend type is ``Discovery`` or
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/conversions.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/conversions.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,43 +19,59 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Module providing for conversions."""
 
 from ansys.api.geometry.v0.models_pb2 import Arc as GRPCArc
 from ansys.api.geometry.v0.models_pb2 import Circle as GRPCCircle
+from ansys.api.geometry.v0.models_pb2 import CurveGeometry as GRPCCurve
 from ansys.api.geometry.v0.models_pb2 import Direction as GRPCDirection
 from ansys.api.geometry.v0.models_pb2 import Ellipse as GRPCEllipse
 from ansys.api.geometry.v0.models_pb2 import Frame as GRPCFrame
 from ansys.api.geometry.v0.models_pb2 import Geometries as GRPCGeometries
 from ansys.api.geometry.v0.models_pb2 import Line as GRPCLine
 from ansys.api.geometry.v0.models_pb2 import Matrix as GRPCMatrix
 from ansys.api.geometry.v0.models_pb2 import Plane as GRPCPlane
 from ansys.api.geometry.v0.models_pb2 import Point as GRPCPoint
 from ansys.api.geometry.v0.models_pb2 import Polygon as GRPCPolygon
+from ansys.api.geometry.v0.models_pb2 import Surface as GRPCSurface
 from ansys.api.geometry.v0.models_pb2 import Tessellation
+from ansys.api.geometry.v0.models_pb2 import TrimmedCurve as GRPCTrimmedCurve
 from beartype.typing import TYPE_CHECKING, List, Optional, Tuple
 
 from ansys.geometry.core.math.frame import Frame
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point2D, Point3D
 from ansys.geometry.core.math.vector import UnitVector3D
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
+from ansys.geometry.core.shapes.curves.circle import Circle
+from ansys.geometry.core.shapes.curves.curve import Curve
+from ansys.geometry.core.shapes.curves.ellipse import Ellipse
+from ansys.geometry.core.shapes.curves.line import Line
+from ansys.geometry.core.shapes.surfaces.cone import Cone
+from ansys.geometry.core.shapes.surfaces.cylinder import Cylinder
+from ansys.geometry.core.shapes.surfaces.plane import PlaneSurface
+from ansys.geometry.core.shapes.surfaces.sphere import Sphere
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.torus import Torus
 from ansys.geometry.core.sketch.arc import Arc
 from ansys.geometry.core.sketch.circle import SketchCircle
 from ansys.geometry.core.sketch.edge import SketchEdge
 from ansys.geometry.core.sketch.ellipse import SketchEllipse
 from ansys.geometry.core.sketch.face import SketchFace
 from ansys.geometry.core.sketch.polygon import Polygon
 from ansys.geometry.core.sketch.segment import SketchSegment
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyvista import PolyData
 
+    from ansys.geometry.core.designer.face import SurfaceType
+    from ansys.geometry.core.shapes.curves.trimmed_curve import TrimmedCurve
+
 
 def unit_vector_to_grpc_direction(unit_vector: UnitVector3D) -> GRPCDirection:
     """
     Convert a ``UnitVector3D`` class to a unit vector Geometry service gRPC message.
 
     Parameters
     ----------
@@ -427,7 +443,151 @@
             [
                 frame.dir_y.x,
                 frame.dir_y.y,
                 frame.dir_y.z,
             ]
         ),
     )
+
+
+def grpc_surface_to_surface(surface: GRPCSurface, surface_type: "SurfaceType") -> Surface:
+    """
+    Convert an ``ansys.api.geometry.Surface`` gRPC message to a ``Surface`` class.
+
+    Parameters
+    ----------
+    surface : GRPCSurface
+        Geometry service gRPC surface message.
+
+    Returns
+    -------
+    Surface
+        Resulting converted surface.
+    """
+    from ansys.geometry.core.designer.face import SurfaceType
+
+    origin = Point3D(
+        [surface.origin.x, surface.origin.y, surface.origin.z], DEFAULT_UNITS.SERVER_LENGTH
+    )
+    axis = UnitVector3D([surface.axis.x, surface.axis.y, surface.axis.z])
+    reference = UnitVector3D([surface.reference.x, surface.reference.y, surface.reference.z])
+
+    if surface_type == SurfaceType.SURFACETYPE_CONE:
+        result = Cone(origin, surface.radius, surface.half_angle, reference, axis)
+    elif surface_type == SurfaceType.SURFACETYPE_CYLINDER:
+        result = Cylinder(origin, surface.radius, reference, axis)
+    elif surface_type == SurfaceType.SURFACETYPE_SPHERE:
+        result = Sphere(origin, surface.radius, reference, axis)
+    elif surface_type == SurfaceType.SURFACETYPE_TORUS:
+        result = Torus(origin, surface.major_radius, surface.minor_radius, reference, axis)
+    elif surface_type == SurfaceType.SURFACETYPE_PLANE:
+        result = PlaneSurface(origin, reference, axis)
+    else:
+        result = None
+    return result
+
+
+def grpc_curve_to_curve(curve: GRPCCurve) -> Curve:
+    """
+    Convert an ``ansys.api.geometry.CurveGeometry`` gRPC message to a ``Curve``.
+
+    Parameters
+    ----------
+    curve : GRPCCurve
+        Geometry service gRPC curve message.
+
+    Returns
+    -------
+    Curve
+        Resulting converted curve.
+    """
+    origin = Point3D([curve.origin.x, curve.origin.y, curve.origin.z])
+    try:
+        reference = UnitVector3D([curve.reference.x, curve.reference.y, curve.reference.z])
+        axis = UnitVector3D([curve.axis.x, curve.axis.y, curve.axis.z])
+    except ValueError:
+        # curve will be a line
+        pass
+    if curve.radius != 0:
+        result = Circle(origin, curve.radius, reference, axis)
+    elif curve.major_radius != 0 and curve.minor_radius != 0:
+        result = Ellipse(origin, curve.major_radius, curve.minor_radius, reference, axis)
+    elif curve.direction is not None:
+        result = Line(
+            origin,
+            UnitVector3D(
+                [
+                    curve.direction.x,
+                    curve.direction.y,
+                    curve.direction.z,
+                ]
+            ),
+        )
+    else:
+        result = None
+
+    return result
+
+
+def curve_to_grpc_curve(curve: Curve) -> GRPCCurve:
+    """
+    Convert a ``Curve`` to an ``ansys.api.geometry.CurveGeometry`` gRPC message.
+
+    Parameters
+    ----------
+    curve : Curve
+        Curve to convert.
+
+    Returns
+    -------
+    GRPCCurve
+        Return ``Curve`` as a ``ansys.api.geometry.CurveGeometry`` message.
+    """
+    grpc_curve = None
+    origin = point3d_to_grpc_point(curve.origin)
+
+    if isinstance(curve, Line):
+        direction = unit_vector_to_grpc_direction(curve.direction)
+        grpc_curve = GRPCCurve(origin=origin, direction=direction)
+    else:
+        reference = unit_vector_to_grpc_direction(curve.dir_x)
+        axis = unit_vector_to_grpc_direction(curve.dir_z)
+
+        if isinstance(curve, Circle):
+            grpc_curve = GRPCCurve(
+                origin=origin, reference=reference, axis=axis, radius=curve.radius.m
+            )
+        elif isinstance(curve, Ellipse):
+            grpc_curve = GRPCCurve(
+                origin=origin,
+                reference=reference,
+                axis=axis,
+                major_radius=curve.major_radius.m,
+                minor_radius=curve.minor_radius.m,
+            )
+
+    return grpc_curve
+
+
+def trimmed_curve_to_grpc_trimmed_curve(curve: "TrimmedCurve") -> GRPCTrimmedCurve:
+    """
+    Convert a ``TrimmedCurve``to an ``ansys.api.geometry.TrimmedCurve`` gRPC message.
+
+    Parameters
+    ----------
+    curve : TrimmedCurve
+        Curve to convert.
+
+    Returns
+    -------
+    GRPCTrimmedCurve
+        Geometry service gRPC ``TrimmedCurve`` message.
+    """
+    curve_geometry = curve_to_grpc_curve(curve.geometry)
+    i_start = curve.interval.start
+    i_end = curve.interval.end
+
+    return GRPCTrimmedCurve(
+        curve=curve_geometry,
+        interval_start=i_start,
+        interval_end=i_end,
+    )
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/defaults.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/docker_instance.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/docker_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 class GeometryContainers(Enum):
     """Provides an enum holding the available Geometry services."""
 
     WINDOWS_LATEST = 0, "windows", "windows-latest"
     LINUX_LATEST = 1, "linux", "linux-latest"
     WINDOWS_LATEST_UNSTABLE = 2, "windows", "windows-latest-unstable"
     LINUX_LATEST_UNSTABLE = 3, "linux", "linux-latest-unstable"
-    WINDOWS_24_1 = 4, "windows", "24.1"
+    WINDOWS_24_1 = 4, "windows", "windows-24.1"
+    LINUX_24_1 = 5, "linux", "linux-24.1"
+    WINDOWS_24_2 = 6, "windows", "windows-24.2"
+    LINUX_24_2 = 7, "linux", "linux-24.2"
 
 
 class LocalDockerInstance:
     """
     Instantiates a Geometry service as a local Docker container.
 
     By default, if a container with the Geometry service already exists at the given port,
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/launcher.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,26 +194,26 @@
             logger.warning(
                 "The Geometry service could not be started locally."
                 " Trying to start Ansys SpaceClaim locally."
             )
 
         try:
             logger.info("Starting Ansys SpaceClaim with Geometry Service locally.")
-            return launch_modeler_with_geometry_service(**kwargs)
+            return launch_modeler_with_spaceclaim(**kwargs)
         except Exception as err:
             logger.warning(
                 "Ansys SpaceClaim could not be started locally."
                 " Trying to start Ansys Discovery locally."
             )
 
         try:
             logger.info("Starting Ansys Discovery with Geometry Service locally.")
-            return launch_modeler_with_geometry_service(**kwargs)
+            return launch_modeler_with_discovery(**kwargs)
         except Exception as err:
-            logger.warning("Ansys SpaceClaim could not be started locally.")
+            logger.warning("Ansys Discovery could not be started locally.")
 
     # If we reached this point...
     raise NotImplementedError("Geometry service cannot be initialized.")
 
 
 def launch_remote_modeler(version: Optional[str] = None, **kwargs: Optional[Dict]) -> "Modeler":
     """
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/product_instance.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/product_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Module containing the ``ProductInstance`` class."""
 import os
 import signal
 import socket
-import subprocess
+
+# Subprocess is needed to start the backend. But
+# the input is controlled by the library. Excluding bandit check.
+import subprocess  # nosec B404
 
 from ansys.tools.path import get_available_ansys_installations, get_latest_ansys_installation
 from beartype.typing import TYPE_CHECKING, Dict, List
 
 from ansys.geometry.core.connection.backend import ApiVersions, BackendType
 from ansys.geometry.core.logger import LOG
 
@@ -105,14 +108,28 @@
 BACKEND_SPACECLAIM_HIDDEN = "/Headless=True"
 """
 The argument to hide SpaceClaim's UI on the backend.
 
 To be used only with Ansys SpaceClaim.
 """
 
+BACKEND_SPACECLAIM_HIDDEN_ENVVAR_KEY = "SPACECLAIM_MODE"
+"""
+SpaceClaim hidden backend's environment variable key.
+
+To be used only with Ansys SpaceClaim.
+"""
+
+BACKEND_SPACECLAIM_HIDDEN_ENVVAR_VALUE = "2"
+"""
+SpaceClaim hidden backend's environment variable value.
+
+To be used only with Ansys SpaceClaim.
+"""
+
 BACKEND_DISCOVERY_HIDDEN = "--hidden"
 """
 The argument to hide Discovery's UI on the backend.
 
 To be used only with Ansys Discovery.
 """
 
@@ -223,14 +240,17 @@
     Returns
     -------
     Modeler
         Instance of the Geometry service.
     """
     from ansys.geometry.core.modeler import Modeler
 
+    if os.name != "nt":  # pragma: no cover
+        raise RuntimeError("Method 'prepare_and_start_backend' is only available on Windows.")
+
     port = _check_port_or_get_one(port)
     installations = get_available_ansys_installations()
     if product_version != None:
         _check_version_is_available(product_version, installations)
     else:
         product_version = get_latest_ansys_installation()[0]
         _check_minimal_versions(product_version)
@@ -252,24 +272,27 @@
         # Here begins the spaceclaim arguments.
         args.append(BACKEND_SPACECLAIM_OPTIONS)
         args.append(
             BACKEND_ADDIN_MANIFEST_ARGUMENT
             + _manifest_path_provider(product_version, installations, manifest_path)
         )
         env_copy[BACKEND_API_VERSION_VARIABLE] = str(api_version)
+
     elif backend_type == BackendType.SPACECLAIM:
         args.append(os.path.join(installations[product_version], SPACECLAIM_FOLDER, SPACECLAIM_EXE))
         if hidden is True:
             args.append(BACKEND_SPACECLAIM_HIDDEN)
             args.append(BACKEND_SPLASH_OFF)
         args.append(
             BACKEND_ADDIN_MANIFEST_ARGUMENT
             + _manifest_path_provider(product_version, installations, manifest_path)
         )
         env_copy[BACKEND_API_VERSION_VARIABLE] = str(api_version)
+        env_copy[BACKEND_SPACECLAIM_HIDDEN_ENVVAR_KEY] = BACKEND_SPACECLAIM_HIDDEN_ENVVAR_VALUE
+
     elif backend_type == BackendType.WINDOWS_SERVICE:
         latest_version = get_latest_ansys_installation()[0]
         args.append(
             os.path.join(
                 installations[latest_version], WINDOWS_GEOMETRY_SERVICE_FOLDER, GEOMETRY_SERVICE_EXE
             )
         )
@@ -278,15 +301,15 @@
             f"Cannot connect to backend {backend_type.name} using ``prepare_and_start_backend()``"
         )
 
     LOG.info(f"Launching ProductInstance for {backend_type.name}")
     LOG.debug(f"Args: {args}")
     LOG.debug(f"Environment variables: {env_copy}")
 
-    instance = ProductInstance(_start_program(args, env_copy).pid)
+    instance = ProductInstance(__start_program(args, env_copy).pid)
 
     # Verify that the backend is ready to accept connections
     # before returning the Modeler instance.
     LOG.info("Waiting for backend to be ready...")
     _wait_for_backend(host, port, timeout)
 
     return Modeler(
@@ -379,15 +402,15 @@
             " Please specify a valid manifest."
             f" The ApiServer Add-In seems to be missing in {os.path.dirname(def_manifest_path)}"
         )
         LOG.error(msg)
         raise RuntimeError(msg)
 
 
-def _start_program(args: List[str], local_env: Dict[str, str]) -> subprocess.Popen:
+def __start_program(args: List[str], local_env: Dict[str, str]) -> subprocess.Popen:
     """
     Start the program where the path is the first item of the ``args`` array argument.
 
     Parameters
     ----------
     args : List[str]
         List of arguments to be passed to the program. The first list's item shall
@@ -396,17 +419,17 @@
         Environment variables to be passed to the program.
 
     Returns
     -------
     subprocess.Popen
         The subprocess object.
     """
-    return subprocess.Popen(
+    # private method and controlled input by library - excluding bandit check.
+    return subprocess.Popen(  # nosec B603
         args,
-        shell=os.name != "nt",
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
         env=local_env,
     )
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/connection/validate.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 .. code:: bash
 
    python -c "from ansys.geometry.core.connection import validate; validate()"
 """
 from ansys.geometry.core.connection.client import GrpcClient
 
 
-def validate():  # pragma: no cover
+def validate(*args, **kwargs):  # pragma: no cover
     """Create a client using the default settings and validate it."""
-    print(GrpcClient())
+    print(GrpcClient(*args, **kwargs))
     # TODO: consider adding additional server stat reporting
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """PyAnsys Geometry designer subpackage."""
 
 from ansys.geometry.core.designer.body import Body, MasterBody, MidSurfaceOffsetType
-from ansys.geometry.core.designer.component import Component, SharedTopologyType
+from ansys.geometry.core.designer.component import Component, ExtrusionDirection, SharedTopologyType
 from ansys.geometry.core.designer.design import Design, DesignFileFormat
 from ansys.geometry.core.designer.designpoint import DesignPoint
 from ansys.geometry.core.designer.edge import CurveType, Edge
 from ansys.geometry.core.designer.face import Face, SurfaceType
 from ansys.geometry.core.designer.part import MasterComponent, Part
 from ansys.geometry.core.designer.selection import NamedSelection
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/beam.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/beam.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/body.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/body.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 from enum import Enum, unique
 from functools import wraps
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.bodies_pb2 import (
     BooleanRequest,
     CopyRequest,
+    GetCollisionRequest,
+    MapRequest,
+    MirrorRequest,
+    RotateRequest,
+    ScaleRequest,
     SetAssignedMaterialRequest,
     TranslateRequest,
 )
 from ansys.api.geometry.v0.bodies_pb2_grpc import BodiesStub
 from ansys.api.geometry.v0.commands_pb2 import (
     AssignMidSurfaceOffsetTypeRequest,
     AssignMidSurfaceThicknessRequest,
@@ -41,27 +46,33 @@
 from ansys.api.geometry.v0.commands_pb2_grpc import CommandsStub
 from beartype import beartype as check_input_types
 from beartype.typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, Union
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.conversions import (
+    frame_to_grpc_frame,
+    plane_to_grpc_plane,
+    point3d_to_grpc_point,
     sketch_shapes_to_grpc_geometries,
     tess_to_pd,
     unit_vector_to_grpc_direction,
 )
 from ansys.geometry.core.designer.edge import CurveType, Edge
 from ansys.geometry.core.designer.face import Face, SurfaceType
 from ansys.geometry.core.errors import protect_grpc
 from ansys.geometry.core.materials.material import Material
 from ansys.geometry.core.math.constants import IDENTITY_MATRIX44
+from ansys.geometry.core.math.frame import Frame
 from ansys.geometry.core.math.matrix import Matrix44
+from ansys.geometry.core.math.plane import Plane
+from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D
-from ansys.geometry.core.misc.checks import check_type, ensure_design_is_active
-from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Distance
+from ansys.geometry.core.misc.checks import check_type, ensure_design_is_active, min_backend_version
+from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Angle, Distance
 from ansys.geometry.core.sketch.sketch import Sketch
 from ansys.geometry.core.typing import Real
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyvista import MultiBlock, PolyData
 
     from ansys.geometry.core.designer.component import Component
@@ -74,14 +85,25 @@
     MIDDLE = 0
     TOP = 1
     BOTTOM = 2
     VARIABLE = 3
     CUSTOM = 4
 
 
+@unique
+class CollisionType(Enum):
+    """Provides values for collision types between bodies."""
+
+    NONE = 0
+    TOUCH = 1
+    INTERSECT = 2
+    CONTAINED = 3
+    CONTAINEDTOUCH = 4
+
+
 class IBody(ABC):
     """
     Defines the common methods for a body, providing the abstract body interface.
 
     Both the ``MasterBody`` class and ``Body`` class both inherit from the ``IBody``
     class. All child classes must implement all abstract methods.
     """
@@ -316,14 +338,107 @@
         Returns
         -------
         None
         """
         return
 
     @abstractmethod
+    def rotate(
+        self,
+        axis_origin: Point3D,
+        axis_direction: UnitVector3D,
+        angle: Union[Quantity, Angle, Real],
+    ) -> None:
+        """
+        Rotate the geometry body around the specified axis by a given angle.
+
+        Parameters
+        ----------
+        axis_origin: Point3D
+            Origin of the rotational axis.
+        axis_direction: UnitVector3D
+            The axis of rotation.
+        angle: Union[~pint.Quantity, Angle, Real]
+            Angle (magnitude) of the rotation.
+
+        Returns
+        -------
+        None
+        """
+        return
+
+    @abstractmethod
+    def scale(self, value: Real) -> None:
+        """
+        Scale the geometry body by the given value.
+
+        Notes
+        -----
+        The calling object is directly modified when this method is called.
+        Thus, it is important to make copies if needed.
+
+        Parameters
+        ----------
+        value: Real
+            Value to scale the body by.
+        """
+        return
+
+    @abstractmethod
+    def map(self, frame: Frame) -> None:
+        """
+        Map the geometry body to the new specified frame.
+
+        Notes
+        -----
+        The calling object is directly modified when this method is called.
+        Thus, it is important to make copies if needed.
+
+        Parameters
+        ----------
+        frame: Frame
+            Structure defining the orientation of the body.
+        """
+        return
+
+    @abstractmethod
+    def mirror(self, plane: Plane) -> None:
+        """
+        Mirror the geometry body across the specified plane.
+
+        Notes
+        -----
+        The calling object is directly modified when this method is called.
+        Thus, it is important to make copies if needed.
+
+        Parameters
+        ----------
+        plane: Plane
+            Represents the mirror.
+        """
+        return
+
+    @abstractmethod
+    def get_collision(self, body: "Body") -> CollisionType:
+        """
+        Get the collision state between bodies.
+
+        Parameters
+        ----------
+        body: Body
+            Object that the collision state is checked with.
+
+        Returns
+        -------
+        CollisionType
+            Enum that defines the collision state between bodies.
+        """
+        return
+
+    @abstractmethod
     def copy(self, parent: "Component", name: str = None) -> "Body":
         """
         Create a copy of the body and place it under the specified parent component.
 
         Parameters
         ----------
         parent: Component
@@ -605,25 +720,37 @@
 
     @property
     @protect_grpc
     def faces(self) -> List[Face]:  # noqa: D102
         self._grpc_client.log.debug(f"Retrieving faces for body {self.id} from server.")
         grpc_faces = self._bodies_stub.GetFaces(self._grpc_id)
         return [
-            Face(grpc_face.id, SurfaceType(grpc_face.surface_type), self, self._grpc_client)
+            Face(
+                grpc_face.id,
+                SurfaceType(grpc_face.surface_type),
+                self,
+                self._grpc_client,
+                grpc_face.is_reversed,
+            )
             for grpc_face in grpc_faces.faces
         ]
 
     @property
     @protect_grpc
     def edges(self) -> List[Edge]:  # noqa: D102
         self._grpc_client.log.debug(f"Retrieving edges for body {self.id} from server.")
         grpc_edges = self._bodies_stub.GetEdges(self._grpc_id)
         return [
-            Edge(grpc_edge.id, CurveType(grpc_edge.curve_type), self, self._grpc_client)
+            Edge(
+                grpc_edge.id,
+                CurveType(grpc_edge.curve_type),
+                self,
+                self._grpc_client,
+                grpc_edge.is_reversed,
+            )
             for grpc_edge in grpc_edges.edges
         ]
 
     @property
     def is_alive(self) -> bool:  # noqa: D102
         return self._is_alive
 
@@ -737,14 +864,72 @@
                 ids=[self.id],
                 direction=unit_vector_to_grpc_direction(direction),
                 distance=translation_magnitude,
             )
         )
 
     @protect_grpc
+    @check_input_types
+    @reset_tessellation_cache
+    @min_backend_version(24, 2, 0)
+    def rotate(
+        self,
+        axis_origin: Point3D,
+        axis_direction: UnitVector3D,
+        angle: Union[Quantity, Angle, Real],
+    ) -> None:  # noqa: D102
+        angle = angle if isinstance(angle, Angle) else Angle(angle)
+        rotation_magnitude = angle.value.m_as(DEFAULT_UNITS.SERVER_ANGLE)
+        self._grpc_client.log.debug(f"Rotating body {self.id}.")
+        self._bodies_stub.Rotate(
+            RotateRequest(
+                id=self.id,
+                axis_origin=point3d_to_grpc_point(axis_origin),
+                axis_direction=unit_vector_to_grpc_direction(axis_direction),
+                angle=rotation_magnitude,
+            )
+        )
+
+    @protect_grpc
+    @check_input_types
+    @reset_tessellation_cache
+    @min_backend_version(24, 2, 0)
+    def scale(self, value: Real) -> None:  # noqa: D102
+        self._grpc_client.log.debug(f"Scaling body {self.id}.")
+        self._bodies_stub.Scale(ScaleRequest(id=self.id, scale=value))
+
+    @protect_grpc
+    @check_input_types
+    @reset_tessellation_cache
+    @min_backend_version(24, 2, 0)
+    def map(self, frame: Frame) -> None:  # noqa: D102
+        self._grpc_client.log.debug(f"Mapping body {self.id}.")
+        self._bodies_stub.Map(MapRequest(id=self.id, frame=frame_to_grpc_frame(frame)))
+
+    @protect_grpc
+    @check_input_types
+    @reset_tessellation_cache
+    @min_backend_version(24, 2, 0)
+    def mirror(self, plane: Plane) -> None:  # noqa: D102
+        self._grpc_client.log.debug(f"Mirroring body {self.id}.")
+        self._bodies_stub.Mirror(MirrorRequest(id=self.id, plane=plane_to_grpc_plane(plane)))
+
+    @protect_grpc
+    @min_backend_version(24, 2, 0)
+    def get_collision(self, body: "Body") -> CollisionType:  # noqa: D102
+        self._grpc_client.log.debug(f"Get collision between body {self.id} and body {body.id}.")
+        response = self._bodies_stub.GetCollision(
+            GetCollisionRequest(
+                body_1_id=self.id,
+                body_2_id=body.id,
+            )
+        )
+        return CollisionType(response.collision)
+
+    @protect_grpc
     def copy(self, parent: "Component", name: str = None) -> "Body":  # noqa: D102
         from ansys.geometry.core.designer.component import Component
 
         # Check input types
         check_type(parent, Component)
         check_type(name, (type(None), str))
         copy_name = self.name if name is None else name
@@ -899,26 +1084,33 @@
         grpc_faces = self._template._bodies_stub.GetFaces(EntityIdentifier(id=self.id))
         return [
             Face(
                 grpc_face.id,
                 SurfaceType(grpc_face.surface_type),
                 self,
                 self._template._grpc_client,
+                grpc_face.is_reversed,
             )
             for grpc_face in grpc_faces.faces
         ]
 
     @property
     @protect_grpc
     @ensure_design_is_active
     def edges(self) -> List[Edge]:  # noqa: D102
         self._template._grpc_client.log.debug(f"Retrieving edges for body {self.id} from server.")
         grpc_edges = self._template._bodies_stub.GetEdges(EntityIdentifier(id=self.id))
         return [
-            Edge(grpc_edge.id, CurveType(grpc_edge.curve_type), self, self._template._grpc_client)
+            Edge(
+                grpc_edge.id,
+                CurveType(grpc_edge.curve_type),
+                self,
+                self._template._grpc_client,
+                grpc_edge.is_reversed,
+            )
             for grpc_edge in grpc_edges.edges
         ]
 
     @property
     def _is_alive(self) -> bool:  # noqa: D102
         return self._template.is_alive
 
@@ -1001,20 +1193,22 @@
                 body=self._id,
                 curves=sketch_shapes_to_grpc_geometries(sketch._plane, sketch.edges, sketch.faces),
                 faces=[face._id for face in faces],
             )
         )
 
         new_edges = [
-            Edge(grpc_edge.id, grpc_edge.curve_type, self, self._template._grpc_client)
+            Edge(grpc_edge.id, CurveType(grpc_edge.curve_type), self, self._template._grpc_client)
             for grpc_edge in imprint_response.edges
         ]
 
         new_faces = [
-            Face(grpc_face.id, grpc_face.surface_type, self, self._template._grpc_client)
+            Face(
+                grpc_face.id, SurfaceType(grpc_face.surface_type), self, self._template._grpc_client
+            )
             for grpc_face in imprint_response.faces
         ]
 
         return (new_edges, new_faces)
 
     @protect_grpc
     @ensure_design_is_active
@@ -1036,15 +1230,17 @@
                 curves=curves,
                 direction=unit_vector_to_grpc_direction(direction),
                 closest_face=closest_face,
             )
         )
 
         projected_faces = [
-            Face(grpc_face.id, grpc_face.surface_type, self, self._template._grpc_client)
+            Face(
+                grpc_face.id, SurfaceType(grpc_face.surface_type), self, self._template._grpc_client
+            )
             for grpc_face in project_response.faces
         ]
 
         return projected_faces
 
     @check_input_types
     @protect_grpc
@@ -1067,27 +1263,54 @@
                 curves=curves,
                 direction=unit_vector_to_grpc_direction(direction),
                 closest_face=closest_face,
             )
         )
 
         imprinted_faces = [
-            Face(grpc_face.id, grpc_face.surface_type, self, self._template._grpc_client)
+            Face(
+                grpc_face.id, SurfaceType(grpc_face.surface_type), self, self._template._grpc_client
+            )
             for grpc_face in response.faces
         ]
 
         return imprinted_faces
 
     @ensure_design_is_active
     def translate(
         self, direction: UnitVector3D, distance: Union[Quantity, Distance, Real]
     ) -> None:  # noqa: D102
         return self._template.translate(direction, distance)
 
     @ensure_design_is_active
+    def rotate(
+        self,
+        axis_origin: Point3D,
+        axis_direction: UnitVector3D,
+        angle: Union[Quantity, Angle, Real],
+    ) -> None:  # noqa: D102
+        return self._template.rotate(axis_origin, axis_direction, angle)
+
+    @ensure_design_is_active
+    def scale(self, value: Real) -> None:  # noqa: D102
+        return self._template.scale(value)
+
+    @ensure_design_is_active
+    def map(self, frame: Frame) -> None:  # noqa: D102
+        return self._template.map(frame)
+
+    @ensure_design_is_active
+    def mirror(self, plane: Plane) -> None:  # noqa: D102
+        return self._template.mirror(plane)
+
+    @ensure_design_is_active
+    def get_collision(self, body: "Body") -> CollisionType:  # noqa: D102
+        return self._template.get_collision(body)
+
+    @ensure_design_is_active
     def copy(self, parent: "Component", name: str = None) -> "Body":  # noqa: D102
         return self._template.copy(parent, name)
 
     @ensure_design_is_active
     def tessellate(
         self, merge: Optional[bool] = False
     ) -> Union["PolyData", "MultiBlock"]:  # noqa: D102
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/component.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,54 +24,60 @@
 from enum import Enum, unique
 import uuid  # TODO: Is ID even needed? Maybe use from SC?
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.bodies_pb2 import (
     CreateBodyFromFaceRequest,
     CreateExtrudedBodyFromFaceProfileRequest,
+    CreateExtrudedBodyFromLoftProfilesRequest,
     CreateExtrudedBodyRequest,
     CreatePlanarBodyRequest,
+    CreateSphereBodyRequest,
+    CreateSweepingChainRequest,
+    CreateSweepingProfileRequest,
     TranslateRequest,
 )
 from ansys.api.geometry.v0.bodies_pb2_grpc import BodiesStub
 from ansys.api.geometry.v0.commands_pb2 import CreateBeamSegmentsRequest, CreateDesignPointsRequest
 from ansys.api.geometry.v0.commands_pb2_grpc import CommandsStub
 from ansys.api.geometry.v0.components_pb2 import (
     CreateRequest,
     SetPlacementRequest,
     SetSharedTopologyRequest,
 )
 from ansys.api.geometry.v0.components_pb2_grpc import ComponentsStub
-from ansys.api.geometry.v0.models_pb2 import Direction, Line
+from ansys.api.geometry.v0.models_pb2 import Direction, Line, TrimmedCurveList
 from beartype import beartype as check_input_types
 from beartype.typing import TYPE_CHECKING, List, Optional, Tuple, Union
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.conversions import (
     grpc_matrix_to_matrix,
     plane_to_grpc_plane,
     point3d_to_grpc_point,
     sketch_shapes_to_grpc_geometries,
+    trimmed_curve_to_grpc_trimmed_curve,
     unit_vector_to_grpc_direction,
 )
 from ansys.geometry.core.designer.beam import Beam, BeamProfile
 from ansys.geometry.core.designer.body import Body, MasterBody
 from ansys.geometry.core.designer.coordinate_system import CoordinateSystem
 from ansys.geometry.core.designer.designpoint import DesignPoint
 from ansys.geometry.core.designer.face import Face
 from ansys.geometry.core.designer.part import MasterComponent, Part
 from ansys.geometry.core.errors import protect_grpc
 from ansys.geometry.core.math.constants import IDENTITY_MATRIX44
 from ansys.geometry.core.math.frame import Frame
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
-from ansys.geometry.core.misc.checks import check_pint_unit_compatibility, ensure_design_is_active
+from ansys.geometry.core.misc.checks import ensure_design_is_active, min_backend_version
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Angle, Distance
+from ansys.geometry.core.shapes.curves.trimmed_curve import TrimmedCurve
 from ansys.geometry.core.sketch.sketch import Sketch
 from ansys.geometry.core.typing import Real
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyvista import MultiBlock, PolyData
 
 
@@ -81,14 +87,37 @@
 
     SHARETYPE_NONE = 0
     SHARETYPE_SHARE = 1
     SHARETYPE_MERGE = 2
     SHARETYPE_GROUPS = 3
 
 
+@unique
+class ExtrusionDirection(Enum):
+    """Enum for extrusion direction definition."""
+
+    POSITIVE = "+"
+    NEGATIVE = "-"
+
+    @classmethod
+    def from_string(cls, string: str, use_default_if_error: bool = False) -> "ExtrusionDirection":
+        """Convert a string to an ``ExtrusionDirection`` enum."""
+        if string == "+":
+            return cls.POSITIVE
+        elif string == "-":
+            return cls.NEGATIVE
+        elif use_default_if_error:
+            from ansys.geometry.core.logger import LOG
+
+            LOG.warning("Invalid extrusion direction. Using default value (+).")
+            return cls.POSITIVE
+        else:  # pragma: no cover
+            raise ValueError(f"Invalid extrusion direction: {string}.")
+
+
 class Component:
     """
     Provides for creating and managing a component.
 
     This class synchronizes to a design within a supporting Geometry service instance.
 
     Parameters
@@ -402,15 +431,19 @@
         # Store the SharedTopologyType set on the client
         self._shared_topology = share_type
 
     @protect_grpc
     @check_input_types
     @ensure_design_is_active
     def extrude_sketch(
-        self, name: str, sketch: Sketch, distance: Union[Quantity, Distance, Real]
+        self,
+        name: str,
+        sketch: Sketch,
+        distance: Union[Quantity, Distance, Real],
+        direction: Union[ExtrusionDirection, str] = ExtrusionDirection.POSITIVE,
     ) -> Body:
         """
         Create a solid body by extruding the sketch profile up by a given distance.
 
         Notes
         -----
         The newly created body is placed under this component within the design assembly.
@@ -419,42 +452,156 @@
         ----------
         name : str
             User-defined label for the new solid body.
         sketch : Sketch
             Two-dimensional sketch source for the extrusion.
         distance : Union[~pint.Quantity, Distance, Real]
             Distance to extrude the solid body.
+        direction : Union[ExtrusionDirection, str], default: "+"
+            Direction for extruding the solid body.
+            The default is to extrude in the positive normal direction of the sketch.
+            Options are "+" and "-" as a string, or the enum values.
 
         Returns
         -------
         Body
             Extruded body from the given sketch.
         """
         # Sanity checks on inputs
         distance = distance if isinstance(distance, Distance) else Distance(distance)
+        if isinstance(direction, str):
+            direction = ExtrusionDirection.from_string(direction, use_default_if_error=True)
 
         # Perform extrusion request
         request = CreateExtrudedBodyRequest(
             distance=distance.value.m_as(DEFAULT_UNITS.SERVER_LENGTH),
             parent=self.id,
             plane=plane_to_grpc_plane(sketch._plane),
             geometries=sketch_shapes_to_grpc_geometries(sketch._plane, sketch.edges, sketch.faces),
             name=name,
         )
 
+        # Check the direction - if it is -, flip the distance
+        if direction is ExtrusionDirection.NEGATIVE:
+            request.distance = -request.distance
+
         self._grpc_client.log.debug(f"Extruding sketch provided on {self.id}. Creating body...")
         response = self._bodies_stub.CreateExtrudedBody(request)
         tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=False)
         self._master_component.part.bodies.append(tb)
         return Body(response.id, response.name, self, tb)
 
+    @min_backend_version(24, 2, 0)
+    @protect_grpc
+    @check_input_types
+    @ensure_design_is_active
+    def sweep_sketch(
+        self,
+        name: str,
+        sketch: Sketch,
+        path: List[TrimmedCurve],
+    ) -> Body:
+        """
+        Create a body by sweeping a planar profile along a path.
+
+        Notes
+        -----
+        The newly created body is placed under this component within the design assembly.
+
+        Parameters
+        ----------
+        name : str
+            User-defined label for the new solid body.
+        sketch : Sketch
+            Two-dimensional sketch source for the extrusion.
+        path : List[TrimmedCurve]
+            The path to sweep the profile along.
+
+        Returns
+        -------
+        Body
+            Created body from the given sketch.
+        """
+        # Convert each ``TrimmedCurve`` in path to equivalent gRPC type
+        path_grpc = []
+        for tc in path:
+            path_grpc.append(trimmed_curve_to_grpc_trimmed_curve(tc))
+
+        request = CreateSweepingProfileRequest(
+            name=name,
+            parent=self.id,
+            plane=plane_to_grpc_plane(sketch._plane),
+            geometries=sketch_shapes_to_grpc_geometries(sketch._plane, sketch.edges, sketch.faces),
+            path=path_grpc,
+        )
+
+        self._grpc_client.log.debug(f"Creating a sweeping profile on {self.id}. Creating body...")
+        response = self._bodies_stub.CreateSweepingProfile(request)
+        tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=False)
+        self._master_component.part.bodies.append(tb)
+        return Body(response.id, response.name, self, tb)
+
+    @min_backend_version(24, 2, 0)
+    @protect_grpc
+    @check_input_types
+    @ensure_design_is_active
+    def sweep_chain(
+        self,
+        name: str,
+        path: List[TrimmedCurve],
+        chain: List[TrimmedCurve],
+    ) -> Body:
+        """
+        Create a body by sweeping a chain of curves along a path.
+
+        Notes
+        -----
+        The newly created body is placed under this component within the design assembly.
+
+        Parameters
+        ----------
+        name : str
+            User-defined label for the new solid body.
+        path : List[TrimmedCurve]
+            The path to sweep the chain along.
+        chain : List[TrimmedCurve]
+            A chain of trimmed curves.
+
+        Returns
+        -------
+        Body
+            Created body from the given sketch.
+        """
+        # Convert each ``TrimmedCurve`` in path and chain to equivalent gRPC types
+        path_grpc = [trimmed_curve_to_grpc_trimmed_curve(tc) for tc in path]
+        chain_grpc = [trimmed_curve_to_grpc_trimmed_curve(tc) for tc in chain]
+
+        request = CreateSweepingChainRequest(
+            name=name,
+            parent=self.id,
+            path=path_grpc,
+            chain=chain_grpc,
+        )
+
+        self._grpc_client.log.debug(f"Creating a sweeping chain on {self.id}. Creating body...")
+        response = self._bodies_stub.CreateSweepingChain(request)
+        tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=True)
+        self._master_component.part.bodies.append(tb)
+        return Body(response.id, response.name, self, tb)
+
     @protect_grpc
     @check_input_types
     @ensure_design_is_active
-    def extrude_face(self, name: str, face: Face, distance: Union[Quantity, Distance]) -> Body:
+    def extrude_face(
+        self,
+        name: str,
+        face: Face,
+        distance: Union[Quantity, Distance],
+        direction: Union[ExtrusionDirection, str] = ExtrusionDirection.POSITIVE,
+    ) -> Body:
         """
         Extrude the face profile by a given distance to create a solid body.
 
         There are no modifications against the body containing the source face.
 
         Notes
         -----
@@ -464,44 +611,154 @@
 
         Parameters
         ----------
         name : str
             User-defined label for the new solid body.
         face : Face
             Target face to use as the source for the new surface.
-        distance : Union[~pint.Quantity, Distance]
+        distance : Union[~pint.Quantity, Distance, Real]
             Distance to extrude the solid body.
+        direction : Union[ExtrusionDirection, str], default: "+"
+            Direction for extruding the solid body's face.
+            The default is to extrude in the positive normal direction of the face.
+            Options are "+" and "-" as a string, or the enum values.
 
         Returns
         -------
         Body
             Extruded solid body.
         """
         # Sanity checks on inputs
-        extrude_distance = distance if isinstance(distance, Quantity) else distance.value
-        check_pint_unit_compatibility(extrude_distance.units, DEFAULT_UNITS.SERVER_LENGTH)
+        distance = distance if isinstance(distance, Distance) else Distance(distance)
+        if isinstance(direction, str):
+            direction = ExtrusionDirection.from_string(direction, use_default_if_error=True)
 
         # Take the face source directly. No need to verify the source of the face.
         request = CreateExtrudedBodyFromFaceProfileRequest(
-            distance=extrude_distance.m_as(DEFAULT_UNITS.SERVER_LENGTH),
+            distance=distance.value.m_as(DEFAULT_UNITS.SERVER_LENGTH),
             parent=self.id,
             face=face.id,
             name=name,
         )
 
+        # Check the direction - if it is -, flip the distance
+        if direction is ExtrusionDirection.NEGATIVE:
+            request.distance = -request.distance
+
         self._grpc_client.log.debug(f"Extruding from face provided on {self.id}. Creating body...")
         response = self._bodies_stub.CreateExtrudedBodyFromFaceProfile(request)
 
         tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=False)
         self._master_component.part.bodies.append(tb)
         return Body(response.id, response.name, self, tb)
 
     @protect_grpc
     @check_input_types
     @ensure_design_is_active
+    @min_backend_version(24, 2, 0)
+    def create_sphere(self, name: str, center: Point3D, radius: Distance) -> Body:
+        """
+        Create a sphere body defined by the center point and the radius.
+
+        Parameters
+        ----------
+        name : str
+            Body name.
+        center : Point3D
+            Center point of the sphere.
+        radius : Distance
+            Radius of the sphere.
+
+        Returns
+        -------
+        Body
+            Sphere body object.
+        """
+        request = CreateSphereBodyRequest(
+            name=name,
+            parent=self.id,
+            center=point3d_to_grpc_point(center),
+            radius=radius.value.m_as(DEFAULT_UNITS.SERVER_LENGTH),
+        )
+        self._grpc_client.log.debug(f"Creating a sphere body on {self.id} .")
+        response = self._bodies_stub.CreateSphereBody(request)
+        tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=False)
+        self._master_component.part.bodies.append(tb)
+        return Body(response.id, response.name, self, tb)
+
+    @protect_grpc
+    @check_input_types
+    @ensure_design_is_active
+    @min_backend_version(24, 2, 0)
+    def create_body_from_loft_profile(
+        self,
+        name: str,
+        profiles: List[List[TrimmedCurve]],
+        periodic: bool = False,
+        ruled: bool = False,
+    ) -> Body:
+        """
+        Create a lofted body from a collection of trimmed curves.
+
+        Parameters
+        ----------
+        name : str
+            Name of the lofted body.
+        profiles : List[List[TrimmedCurve]]
+            Collection of lists of trimmed curves (profiles) defining the lofted body's shape.
+        periodic : bool, default: False
+            Whether the lofted body should have periodic continuity.
+        ruled : bool
+            Whether the lofted body should be ruled.
+
+        Returns
+        -------
+        Body
+            Created lofted body object.
+
+        Notes
+        -----
+        Surfaces produced have a U parameter in the direction of the profile curves,
+        and a V parameter in the direction of lofting.
+        Profiles can have different numbers of segments. A minimum twist solution is
+        produced.
+        Profiles should be all closed or all open. Closed profiles cannot contain inner
+        loops. If closed profiles are supplied, a closed (solid) body is produced, if
+        possible. Otherwise, an open (sheet) body is produced.
+        The periodic argument applies when the profiles are closed. It is ignored if
+        the profiles are open.
+
+        If ``periodic=True``, at least three profiles must be supplied. The loft continues
+        from the last profile back to the first profile to produce surfaces that are
+        periodic in V.
+
+        If ``periodic=False``, at least two profiles must be supplied. If the first
+        and last profiles are planar, end capping faces are created. Otherwise, an open
+        (sheet) body is produced.
+        If ``ruled=True``, separate ruled surfaces are produced between each pair of profiles.
+        If ``periodic=True``, the loft continues from the last profile back to the first
+        profile, but the surfaces are not periodic.
+        """
+        profiles_grpc = [
+            TrimmedCurveList(curves=[trimmed_curve_to_grpc_trimmed_curve(tc) for tc in profile])
+            for profile in profiles
+        ]
+
+        request = CreateExtrudedBodyFromLoftProfilesRequest(
+            name=name, parent=self.id, profiles=profiles_grpc, periodic=periodic, ruled=ruled
+        )
+        self._grpc_client.log.debug(f"Creating a loft profile body on {self.id} .")
+        response = self._bodies_stub.CreateExtrudedBodyFromLoftProfiles(request)
+        tb = MasterBody(response.master_id, name, self._grpc_client, is_surface=False)
+        self._master_component.part.bodies.append(tb)
+        return Body(response.id, response.name, self, tb)
+
+    @protect_grpc
+    @check_input_types
+    @ensure_design_is_active
     def create_surface(self, name: str, sketch: Sketch) -> Body:
         """
         Create a surface body with a sketch profile.
 
         The newly created body is placed under this component within the design assembly.
 
         Parameters
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/coordinate_system.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/design.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/design.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 """Provides for managing designs."""
 
 from enum import Enum, unique
 from pathlib import Path
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier, PartExportFormat
-from ansys.api.dbu.v0.designs_pb2 import NewRequest, SaveAsRequest
+from ansys.api.dbu.v0.designs_pb2 import InsertRequest, NewRequest, SaveAsRequest
 from ansys.api.dbu.v0.designs_pb2_grpc import DesignsStub
 from ansys.api.geometry.v0.commands_pb2 import (
     AssignMidSurfaceOffsetTypeRequest,
     AssignMidSurfaceThicknessRequest,
     CreateBeamCircularProfileRequest,
 )
 from ansys.api.geometry.v0.commands_pb2_grpc import CommandsStub
@@ -64,15 +64,15 @@
 from ansys.geometry.core.errors import protect_grpc
 from ansys.geometry.core.materials.material import Material
 from ansys.geometry.core.materials.property import MaterialProperty, MaterialPropertyType
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Y, ZERO_POINT3D
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
-from ansys.geometry.core.misc.checks import ensure_design_is_active
+from ansys.geometry.core.misc.checks import ensure_design_is_active, min_backend_version
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Distance
 from ansys.geometry.core.modeler import Modeler
 from ansys.geometry.core.typing import RealSequence
 
 
 @unique
 class DesignFileFormat(Enum):
@@ -577,14 +577,66 @@
             self._grpc_client.log.debug(f"Beam profile {removal_name} successfully deleted.")
         else:
             self._grpc_client.log.warning(
                 f"Attempted beam profile deletion failed, with name {removal_name}."
                 + " Ignoring request."
             )
 
+    @protect_grpc
+    @check_input_types
+    @ensure_design_is_active
+    @min_backend_version(24, 2, 0)
+    def insert_file(self, file_location: Union[Path, str]) -> Component:
+        """
+        Insert a file into the design.
+
+        Parameters
+        ----------
+        file_location : Union[~pathlib.Path, str]
+            Location on disk where the file is located.
+
+        Returns
+        -------
+        Component
+            The newly inserted component.
+        """
+        # Upload the file to the server
+        filepath_server = self._modeler._upload_file(file_location)
+
+        # Insert the file into the design
+        self._design_stub.Insert(InsertRequest(filepath=filepath_server))
+        self._grpc_client.log.debug(f"File {file_location} successfully inserted into design.")
+
+        # Get a temporal design object to update the current one
+        tmp_design = Design("", self._modeler, read_existing_design=True)
+
+        # Update the reference to the design
+        for component in tmp_design.components:
+            component._parent_component = self
+
+        # Update the design's components - add the new one
+        #
+        # If the list is empty, add the components from the new design
+        if not self._components:
+            self._components.extend(tmp_design.components)
+        else:
+            # Insert operation adds the inserted file as a component to the design.
+            for tmp_component in tmp_design.components:
+                # Otherwise, check which is the new component added
+                for component in self._components:
+                    if component.id == tmp_component.id:
+                        break
+                    # If not equal, add the component - since it has not been found
+                    self._components.append(tmp_component)
+
+        self._grpc_client.log.debug(f"Design {self.name} is successfully updated.")
+
+        # Return the newly inserted component
+        return self._components[-1]
+
     def __repr__(self) -> str:
         """Represent the ``Design`` as a string."""
         alive_bodies = [1 if body.is_alive else 0 for body in self.bodies]
         alive_comps = [1 if comp.is_alive else 0 for comp in self.components]
         lines = [f"ansys.geometry.core.designer.Design {hex(id(self))}"]
         lines.append(f"  Name                 : {self.name}")
         lines.append(f"  Is active?           : {self._is_active}")
@@ -596,14 +648,17 @@
         lines.append(f"  N Beam Profiles      : {len(self.beam_profiles)}")
         lines.append(f"  N Design Points      : {len(self.design_points)}")
         return "\n".join(lines)
 
     def __read_existing_design(self) -> None:
         """Read an existing ``Design`` located on the server."""
         #
+        # TODO: This might go out of sync with the _update_design_inplace method.
+        #       Ensure that the two methods are in sync. Especially regarding cleanup.
+        #
         # TODO: Not all features implemented yet. Status is as follows
         #
         # Windows:
         #
         # - [X] Components
         # - [X] Bodies
         # - [X] Materials
@@ -755,7 +810,39 @@
         self._grpc_client.log.debug(f"Bodies created: {len(created_bodies)}")
         self._grpc_client.log.debug(f"Materials created: {len(self.materials)}")
         self._grpc_client.log.debug(f"NamedSelections created: {len(self.named_selections)}")
         self._grpc_client.log.debug(f"CoordinateSystems created: {num_created_coord_systems}")
         self._grpc_client.log.debug(f"SharedTopologyTypes set: {num_created_shared_topologies}")
 
         self._grpc_client.log.debug(f"\nSuccessfully read design in: {end - start} s")
+
+    def _update_design_inplace(self) -> None:
+        """
+        Update the design to align with the server side.
+
+        Notes
+        -----
+        This method is used to update the design inside repair tools.
+        Its usage is not recommended for other purposes.
+        """
+        # Clear all the existing information
+        #
+        # TODO: This might go out of sync with the __read_existing_design method
+        #       if the latter is updated and this method is not. Ensure that
+        #       the two methods are in sync.
+        #
+        self._components = []
+        self._bodies = []
+        self._materials = []
+        self._named_selections = {}
+        self._coordinate_systems = {}
+
+        # Get the previous design id
+        previous_design_id = self._design_id
+
+        # Read the existing design
+        self.__read_existing_design()
+
+        # If the design id has changed, update the design id in the Modeler
+        if previous_design_id != self._design_id:
+            self._modeler._designs[self._design_id] = self
+            self._modeler._designs.pop(previous_design_id)
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/designpoint.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/designpoint.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/edge.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/edge.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,18 +25,21 @@
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.edges_pb2_grpc import EdgesStub
 from beartype.typing import TYPE_CHECKING, List
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
+from ansys.geometry.core.connection.conversions import grpc_curve_to_curve
 from ansys.geometry.core.errors import protect_grpc
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.misc.checks import ensure_design_is_active
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
+from ansys.geometry.core.shapes.curves.trimmed_curve import ReversedTrimmedCurve, TrimmedCurve
+from ansys.geometry.core.shapes.parameterization import Interval
 
 if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.designer.body import Body
     from ansys.geometry.core.designer.face import Face
 
 
 @unique
@@ -63,42 +66,87 @@
         Server-defined ID for the body.
     curve_type : CurveType
         Type of curve that the edge forms.
     body : Body
         Parent body that the edge constructs.
     grpc_client : GrpcClient
         Active supporting Geometry service instance for design modeling.
+    is_reversed : bool
+        Direction of the edge.
     """
 
-    def __init__(self, id: str, curve_type: CurveType, body: "Body", grpc_client: GrpcClient):
-        """Initialize ``Edge`` class."""
+    def __init__(
+        self,
+        id: str,
+        curve_type: CurveType,
+        body: "Body",
+        grpc_client: GrpcClient,
+        is_reversed: bool = False,
+    ):
+        """Initialize the ``Edge`` class."""
         self._id = id
         self._curve_type = curve_type
         self._body = body
         self._grpc_client = grpc_client
         self._edges_stub = EdgesStub(grpc_client.channel)
+        self._is_reversed = is_reversed
+        self._shape = None
 
     @property
     def id(self) -> str:
         """ID of the edge."""
         return self._id
 
     @property
     def _grpc_id(self) -> EntityIdentifier:
-        """Entity identifier of this edge on the server side."""
+        """Entity ID of this edge on the server side."""
         return EntityIdentifier(id=self._id)
 
     @property
+    def is_reversed(self) -> bool:
+        """Flag indicating if the edge is reversed."""
+        return self._is_reversed
+
+    @property
+    def shape(self) -> TrimmedCurve:
+        """
+        Underlying trimmed curve of the edge.
+
+        If the edge is reversed, its shape is the ``ReversedTrimmedCurve`` type, which swaps the
+        start and end points of the curve and handles parameters to allow evaluation as if the
+        curve is not reversed.
+        """
+        if self._shape is None:
+            self._grpc_client.log.debug("Requesting edge properties from server.")
+            response = self._edges_stub.GetCurve(self._grpc_id)
+            geometry = grpc_curve_to_curve(response)
+
+            response = self._edges_stub.GetStartAndEndPoints(self._grpc_id)
+            start = Point3D([response.start.x, response.start.y, response.start.z])
+            end = Point3D([response.end.x, response.end.y, response.end.z])
+
+            response = self._edges_stub.GetLength(self._grpc_id)
+            length = Quantity(response.length, DEFAULT_UNITS.SERVER_LENGTH)
+
+            response = self._edges_stub.GetInterval(self._grpc_id)
+            interval = Interval(response.start, response.end)
+
+            self._shape = (
+                ReversedTrimmedCurve(geometry, start, end, interval, length)
+                if self.is_reversed
+                else TrimmedCurve(geometry, start, end, interval, length)
+            )
+        return self._shape
+
+    @property
     @protect_grpc
     @ensure_design_is_active
     def length(self) -> Quantity:
         """Calculated length of the edge."""
-        self._grpc_client.log.debug("Requesting edge length from server.")
-        length_response = self._edges_stub.GetLength(self._grpc_id)
-        return Quantity(length_response.length, DEFAULT_UNITS.SERVER_LENGTH)
+        return self.shape.length
 
     @property
     def curve_type(self) -> CurveType:
         """Curve type of the edge."""
         return self._curve_type
 
     @property
@@ -107,28 +155,16 @@
     def faces(self) -> List["Face"]:
         """Faces that contain the edge."""
         from ansys.geometry.core.designer.face import Face, SurfaceType
 
         self._grpc_client.log.debug("Requesting edge faces from server.")
         grpc_faces = self._edges_stub.GetFaces(self._grpc_id).faces
         return [
-            Face(grpc_face.id, SurfaceType(grpc_face.surface_type), self._body, self._grpc_client)
+            Face(
+                grpc_face.id,
+                SurfaceType(grpc_face.surface_type),
+                self._body,
+                self._grpc_client,
+                grpc_face.is_reversed,
+            )
             for grpc_face in grpc_faces
         ]
-
-    @property
-    @protect_grpc
-    @ensure_design_is_active
-    def start_point(self) -> Point3D:
-        """Edge start point."""
-        self._grpc_client.log.debug("Requesting edge points from server.")
-        point = self._edges_stub.GetStartAndEndPoints(self._grpc_id).start
-        return Point3D([point.x, point.y, point.z])
-
-    @property
-    @protect_grpc
-    @ensure_design_is_active
-    def end_point(self) -> Point3D:
-        """Edge end point."""
-        self._grpc_client.log.debug("Requesting edge points from server.")
-        point = self._edges_stub.GetStartAndEndPoints(self._grpc_id).end
-        return Point3D([point.x, point.y, point.z])
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/face.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/face.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,27 +21,35 @@
 # SOFTWARE.
 """Module for managing a face."""
 
 from enum import Enum, unique
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.edges_pb2_grpc import EdgesStub
-from ansys.api.geometry.v0.faces_pb2 import EvaluateRequest, GetNormalRequest
+from ansys.api.geometry.v0.faces_pb2 import CreateIsoParamCurvesRequest
 from ansys.api.geometry.v0.faces_pb2_grpc import FacesStub
 from ansys.api.geometry.v0.models_pb2 import Edge as GRPCEdge
 from beartype.typing import TYPE_CHECKING, List
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
-from ansys.geometry.core.designer.edge import CurveType, Edge
+from ansys.geometry.core.connection.conversions import grpc_curve_to_curve, grpc_surface_to_surface
+from ansys.geometry.core.designer.edge import Edge
 from ansys.geometry.core.errors import protect_grpc
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D
 from ansys.geometry.core.misc.checks import ensure_design_is_active
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
+from ansys.geometry.core.shapes.box_uv import BoxUV
+from ansys.geometry.core.shapes.curves.trimmed_curve import TrimmedCurve
+from ansys.geometry.core.shapes.parameterization import Interval
+from ansys.geometry.core.shapes.surfaces.trimmed_surface import (
+    ReversedTrimmedSurface,
+    TrimmedSurface,
+)
 
 if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.designer.body import Body
 
 
 @unique
 class SurfaceType(Enum):
@@ -143,53 +151,92 @@
         Type of surface that the face forms.
     body : Body
         Parent body that the face constructs.
     grpc_client : GrpcClient
         Active supporting Geometry service instance for design modeling.
     """
 
-    def __init__(self, id: str, surface_type: SurfaceType, body: "Body", grpc_client: GrpcClient):
-        """Initialize ``Face`` class."""
+    def __init__(
+        self,
+        id: str,
+        surface_type: SurfaceType,
+        body: "Body",
+        grpc_client: GrpcClient,
+        is_reversed: bool = False,
+    ):
+        """Initialize the ``Face`` class."""
         self._id = id
         self._surface_type = surface_type
         self._body = body
         self._grpc_client = grpc_client
         self._faces_stub = FacesStub(grpc_client.channel)
         self._edges_stub = EdgesStub(grpc_client.channel)
+        self._is_reversed = is_reversed
+        self._shape = None
+
+        self._grpc_client.log.debug("Requesting surface properties from server.")
 
     @property
     def id(self) -> str:
         """Face ID."""
         return self._id
 
     @property
     def _grpc_id(self) -> EntityIdentifier:
-        """Entity identifier of this face on the server side."""
+        """Entity ID of this face on the server side."""
         return EntityIdentifier(id=self._id)
 
     @property
+    def is_reversed(self) -> bool:
+        """Flag indicating if the face is reversed."""
+        return self._is_reversed
+
+    @property
     def body(self) -> "Body":
         """Body that the face belongs to."""
         return self._body
 
     @property
+    def shape(self) -> TrimmedSurface:
+        """
+        Underlying trimmed surface of the face.
+
+        If the face is reversed, its shape is a ``ReversedTrimmedSurface`` type, which handles the
+        direction of the normal vector to ensure it is always facing outward.
+        """
+        if self._shape is None:
+            self._grpc_client.log.debug("Requesting face properties from server.")
+
+            surface_response = self._faces_stub.GetSurface(self._grpc_id)
+            geometry = grpc_surface_to_surface(surface_response, self._surface_type)
+            box = self._faces_stub.GetBoxUV(self._grpc_id)
+            box_uv = BoxUV(Interval(box.start_u, box.end_u), Interval(box.start_v, box.end_v))
+
+            self._shape = (
+                ReversedTrimmedSurface(geometry, box_uv)
+                if self.is_reversed
+                else TrimmedSurface(geometry, box_uv)
+            )
+        return self._shape
+
+    @property
+    def surface_type(self) -> SurfaceType:
+        """Surface type of the face."""
+        return self._surface_type
+
+    @property
     @protect_grpc
     @ensure_design_is_active
     def area(self) -> Quantity:
         """Calculated area of the face."""
         self._grpc_client.log.debug("Requesting face area from server.")
         area_response = self._faces_stub.GetArea(self._grpc_id)
         return Quantity(area_response.area, DEFAULT_UNITS.SERVER_AREA)
 
     @property
-    def surface_type(self) -> SurfaceType:
-        """Surface type of the face."""
-        return self._surface_type
-
-    @property
     @protect_grpc
     @ensure_design_is_active
     def edges(self) -> List[Edge]:
         """List of all edges of the face."""
         self._grpc_client.log.debug("Requesting face edges from server.")
         edges_response = self._faces_stub.GetEdges(self._grpc_id)
         return self.__grpc_edges_to_edges(edges_response.edges)
@@ -228,18 +275,17 @@
             loops.append(
                 FaceLoop(type=type, length=length, min_bbox=min, max_bbox=max, edges=edges)
             )
 
         return loops
 
     @protect_grpc
-    @ensure_design_is_active
-    def face_normal(self, u: float = 0.5, v: float = 0.5) -> UnitVector3D:
+    def normal(self, u: float = 0.5, v: float = 0.5) -> UnitVector3D:
         """
-        Get the normal direction to the face evaluated at certain UV coordinates.
+        Get the normal direction to the face at certain proportional UV coordinates.
 
         Notes
         -----
         To properly use this method, you must handle UV coordinates. Thus, you must
         know how these relate to the underlying Geometry service. It is an advanced
         method for Geometry experts only.
 
@@ -255,23 +301,20 @@
         Returns
         -------
         UnitVector3D
             :class:`UnitVector3D` object evaluated at the given U and V coordinates.
             This :class:`UnitVector3D` object is perpendicular to the surface at the
             given UV coordinates.
         """
-        self._grpc_client.log.debug(f"Requesting face normal from server with (u,v)=({u},{v}).")
-        response = self._faces_stub.GetNormal(GetNormalRequest(id=self.id, u=u, v=v)).direction
-        return UnitVector3D([response.x, response.y, response.z])
+        return self.shape.normal(u, v)
 
     @protect_grpc
-    @ensure_design_is_active
-    def face_point(self, u: float = 0.5, v: float = 0.5) -> Point3D:
+    def point(self, u: float = 0.5, v: float = 0.5) -> Point3D:
         """
-        Get a point of the face evaluated at certain UV coordinates.
+        Get a point of the face evaluated at certain proportional UV coordinates.
 
         Notes
         -----
         To properly use this method, you must handle UV coordinates. Thus, you must
         know how these relate to the underlying Geometry service. It is an advanced
         method for Geometry experts only.
 
@@ -286,17 +329,15 @@
 
         Returns
         -------
         Point3D
             :class:`Point3D`
             object evaluated at the given UV coordinates.
         """
-        self._grpc_client.log.debug(f"Requesting face point from server with (u,v)=({u},{v}).")
-        response = self._faces_stub.Evaluate(EvaluateRequest(id=self.id, u=u, v=v)).point
-        return Point3D([response.x, response.y, response.z], DEFAULT_UNITS.SERVER_LENGTH)
+        return self.shape.evaluate_proportion(u, v).position
 
     def __grpc_edges_to_edges(self, edges_grpc: List[GRPCEdge]) -> List[Edge]:
         """
         Transform a list of gRPC edge messages into actual ``Edge`` objects.
 
         Parameters
         ----------
@@ -304,13 +345,61 @@
             List of gRPC messages of type ``Edge``.
 
         Returns
         -------
         List[Edge]
             ``Edge`` objects to obtain from gRPC messages.
         """
+        from ansys.geometry.core.designer.edge import CurveType, Edge
+
         edges = []
         for edge_grpc in edges_grpc:
             edges.append(
-                Edge(edge_grpc.id, CurveType(edge_grpc.curve_type), self._body, self._grpc_client)
+                Edge(
+                    edge_grpc.id,
+                    CurveType(edge_grpc.curve_type),
+                    self._body,
+                    self._grpc_client,
+                    edge_grpc.is_reversed,
+                )
             )
         return edges
+
+    def create_isoparametric_curves(
+        self, use_u_param: bool, parameter: float
+    ) -> List[TrimmedCurve]:
+        """
+        Create isoparametic curves at the given proportional parameter.
+
+        Typically, only one curve is created, but if the face has a hole, it is possible that
+        more than one curve is created.
+
+        Parameters
+        ----------
+        use_u_param : bool
+            Whether the parameter is the ``u`` coordinate or ``v`` coordinate. If ``True``,
+            it is the ``u`` coordinate. If ``False``, it is the ``v`` coordinate.
+        parameter : float
+            Proportional [0-1] parameter to create the one or more curves at.
+
+        Returns
+        -------
+        List[TrimmedCurve]
+            List of curves that were created.
+        """
+        curves = self._faces_stub.CreateIsoParamCurves(
+            CreateIsoParamCurvesRequest(id=self.id, u_dir_curve=use_u_param, proportion=parameter)
+        ).curves
+
+        trimmed_curves = []
+        for c in curves:
+            geometry = grpc_curve_to_curve(c.curve)
+            start = Point3D([c.start.x, c.start.y, c.start.z])
+            end = Point3D([c.end.x, c.end.y, c.end.z])
+            interval = Interval(c.interval_start, c.interval_end)
+            length = Quantity(c.length, DEFAULT_UNITS.SERVER_LENGTH)
+
+            trimmed_curves.append(
+                TrimmedCurve(geometry, start, end, interval, length, self._grpc_client)
+            )
+
+        return trimmed_curves
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/part.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/part.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """Module providing fundamental data of an assembly."""
 from beartype.typing import TYPE_CHECKING, List
 
 from ansys.geometry.core.designer.body import MasterBody
 from ansys.geometry.core.math.constants import IDENTITY_MATRIX44
 from ansys.geometry.core.math.matrix import Matrix44
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.designer.component import Component
 
 
 class Part:
     """
     Represents a part master.
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/designer/selection.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/selection.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/errors.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/logger.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/material.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/material.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/materials/property.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/property.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/bbox.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/bbox.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/constants.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/frame.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/frame.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/matrix.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides matrix primitive representations."""
 from beartype import beartype as check_input_types
 from beartype.typing import Optional, Union
 import numpy as np
 
-from ansys.geometry.core.misc import check_ndarray_is_float_int
+from ansys.geometry.core.misc.checks import check_ndarray_is_float_int
 from ansys.geometry.core.typing import Real, RealSequence
 
 DEFAULT_MATRIX33 = np.identity(3)
 """Default value of the 3x3 identity matrix for the ``Matrix33`` class."""
 
 DEFAULT_MATRIX44 = np.identity(4)
 """Default value of the 4x4 identity matrix for the ``Matrix44`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/plane.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/point.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/math/vector.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,20 +18,31 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides the PyAnsys Geometry miscellaneous subpackage."""
 
 from ansys.geometry.core.misc.accuracy import ANGLE_ACCURACY, LENGTH_ACCURACY, Accuracy
+from ansys.geometry.core.misc.auxiliary import (
+    get_bodies_from_ids,
+    get_design_from_body,
+    get_design_from_component,
+    get_design_from_edge,
+    get_design_from_face,
+    get_edges_from_ids,
+    get_faces_from_ids,
+)
 from ansys.geometry.core.misc.checks import (
     check_is_float_int,
     check_ndarray_is_all_nan,
     check_ndarray_is_float_int,
     check_ndarray_is_non_zero,
     check_ndarray_is_not_none,
     check_pint_unit_compatibility,
     check_type,
+    check_type_all_elements_in_iterable,
     check_type_equivalence,
+    min_backend_version,
 )
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Angle, Distance
 from ansys.geometry.core.misc.options import ImportOptions
 from ansys.geometry.core.misc.units import UNITS, PhysicalQuantity
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/accuracy.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/accuracy.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,24 +22,43 @@
 """Provides for evaluating decimal precision."""
 
 
 import math
 
 from ansys.geometry.core.typing import Real
 
-LENGTH_ACCURACY = 1e-8
+LENGTH_ACCURACY: Real = 1e-8
 """Constant for decimal accuracy in length comparisons."""
 
-ANGLE_ACCURACY = 1e-6
+ANGLE_ACCURACY: Real = 1e-6
 """Constant for decimal accuracy in angle comparisons."""
 
+DOUBLE_ACCURACY: Real = 1e-13
+"""Constant for double accuracy."""
+
 
 class Accuracy:
     """Provides decimal precision evaluations for actions such as equivalency."""
 
+    @staticmethod
+    def length_accuracy() -> Real:
+        """Return the ``LENGTH_ACCURACY`` constant."""
+        return LENGTH_ACCURACY
+
+    @staticmethod
+    def angle_accuracy() -> Real:
+        """Return the ``ANGLE_ACCURACY`` constant."""
+        return ANGLE_ACCURACY
+
+    @staticmethod
+    def double_accuracy() -> Real:
+        """Return the ``DOUBLE_ACCURACY`` constant."""
+        return DOUBLE_ACCURACY
+
+    @staticmethod
     def length_is_equal(comparison_length: Real, reference_length: Real) -> bool:
         """
         Check if the comparison length is equal to the reference length.
 
         Notes
         -----
         The check is done up to the constant value specified for ``LENGTH_ACCURACY``.
@@ -50,14 +69,32 @@
             ``True`` if the comparison length is equal to the reference length
             within the length accuracy, ``False`` otherwise.
         """
         return Accuracy.is_within_tolerance(
             comparison_length, reference_length, LENGTH_ACCURACY, LENGTH_ACCURACY
         )
 
+    @staticmethod
+    def equal_doubles(a: Real, b: Real):
+        """Compare two double values."""
+        return Accuracy.is_within_tolerance(a, b, DOUBLE_ACCURACY, DOUBLE_ACCURACY)
+
+    @staticmethod
+    def compare_with_tolerance(
+        a: Real, b: Real, relative_tolerance: Real, absolute_tolerance: Real
+    ) -> Real:
+        """Compare two doubles given the relative and absolute tolerances."""
+        if Accuracy.is_within_tolerance(a, b, relative_tolerance, absolute_tolerance):
+            return 0
+        elif a < b:
+            return -1
+        else:
+            return 1
+
+    @staticmethod
     def length_is_greater_than_or_equal(comparison_length: Real, reference_length: Real) -> bool:
         """
         Check if the comparison length is greater than the reference length.
 
         Notes
         -----
         The check is done up to the constant value specified for ``LENGTH_ACCURACY``.
@@ -69,14 +106,15 @@
             the length accuracy, ``False`` otherwise.
         """
         return bool(
             comparison_length > reference_length
             or Accuracy.length_is_equal(comparison_length, reference_length)
         )
 
+    @staticmethod
     def length_is_less_than_or_equal(comparison_length: Real, reference_length: Real) -> bool:
         """
         Check if the comparison length is less than or equal to the reference length.
 
         Notes
         -----
         The check is done up to the constant value specified for ``LENGTH_ACCURACY``.
@@ -88,86 +126,93 @@
             within the length accuracy, ``False`` otherwise.
         """
         return bool(
             comparison_length < reference_length
             or Accuracy.length_is_equal(comparison_length, reference_length)
         )
 
+    @staticmethod
     def length_is_zero(length: Real) -> bool:
         """
         Check if the length is within the length accuracy of exact zero.
 
         Returns
         -------
         bool
             ``True`` if the length is within the length accuracy of exact zero,
             ``False`` otherwise.
         """
         return bool(length <= LENGTH_ACCURACY and length >= -LENGTH_ACCURACY)
 
+    @staticmethod
     def length_is_negative(length: Real) -> bool:
         """
         Check if the length is below a negative length accuracy.
 
         Returns
         -------
         bool
             ``True`` if the length is below a negative length accuracy,
              ``False`` otherwise.
         """
         return bool(length < -LENGTH_ACCURACY)
 
+    @staticmethod
     def length_is_positive(length: Real) -> bool:
         """
         Check if the length is above a positive length accuracy.
 
         Returns
         -------
         bool
             ``True`` if the length is above a positive length accuracy,
              ``False`` otherwise.
         """
         return bool(length > LENGTH_ACCURACY)
 
+    @staticmethod
     def angle_is_zero(angle: Real) -> bool:
         """
         Check if the length is within the angle accuracy of exact zero.
 
         Returns
         -------
         bool
             ``True`` if the length is within the angle accuracy of exact zero,
              ``False`` otherwise.
         """
         return bool(abs(angle) < ANGLE_ACCURACY)
 
+    @staticmethod
     def angle_is_negative(angle: Real) -> bool:
         """
         Check if the angle is below a negative angle accuracy.
 
         Returns
         -------
         bool
             ``True`` if the angle is below a negative angle accuracy,
              ``False`` otherwise.
         """
         return bool(angle <= -ANGLE_ACCURACY)
 
+    @staticmethod
     def angle_is_positive(angle: Real) -> bool:
         """
         Check if the angle is above a positive angle accuracy.
 
         Returns
         -------
         bool
            ``True`` if the angle is above a positive angle accuracy,
             ``False`` otherwise.
         """
         return bool(angle >= ANGLE_ACCURACY)
 
+    @staticmethod
     def is_within_tolerance(
         a: Real, b: Real, relative_tolerance: Real, absolute_tolerance: Real
     ) -> bool:
         """
         Check if two values (a and b) are inside a relative and absolute tolerance.
 
         Parameters
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/measurements.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/measurements.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/options.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/options.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/misc/units.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/units.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/modeler.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/modeler.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 from grpc import Channel
 
 from ansys.geometry.core.connection.backend import BackendType
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.defaults import DEFAULT_HOST, DEFAULT_PORT
 from ansys.geometry.core.errors import GeometryRuntimeError, protect_grpc
 from ansys.geometry.core.logger import LOG as logger
-from ansys.geometry.core.misc.checks import check_type
+from ansys.geometry.core.misc.checks import check_type, min_backend_version
 from ansys.geometry.core.misc.options import ImportOptions
+from ansys.geometry.core.tools.measurement_tools import MeasurementTools
 from ansys.geometry.core.tools.repair_tools import RepairTools
 from ansys.geometry.core.typing import Real
 
 if TYPE_CHECKING:  # pragma: no cover
     from ansys.platform.instancemanagement import Instance
 
     from ansys.geometry.core.connection.docker_instance import LocalDockerInstance
@@ -99,15 +100,15 @@
         product_instance: Optional["ProductInstance"] = None,
         timeout: Optional[Real] = 120,
         logging_level: Optional[int] = logging.INFO,
         logging_file: Optional[Union[Path, str]] = None,
         backend_type: Optional[BackendType] = None,
     ):
         """Initialize the ``Modeler`` class."""
-        self._client = GrpcClient(
+        self._grpc_client = GrpcClient(
             host=host,
             port=port,
             channel=channel,
             remote_instance=remote_instance,
             docker_instance=docker_instance,
             product_instance=product_instance,
             timeout=timeout,
@@ -116,17 +117,19 @@
             backend_type=backend_type,
         )
 
         # Initialize the RepairTools - Not available on Linux
         # TODO: delete "if" when Linux service is able to use repair tools
         if self.client.backend_type == BackendType.LINUX_SERVICE:
             self._repair_tools = None
+            self._measurement_tools = None
             logger.warning("Linux backend does not support repair tools.")
         else:
-            self._repair_tools = RepairTools(self._client)
+            self._repair_tools = RepairTools(self._grpc_client)
+            self._measurement_tools = MeasurementTools(self._grpc_client)
 
         # Maintaining references to all designs within the modeler workspace
         self._designs: Dict[str, "Design"] = {}
 
         # Check if the backend allows for multiple designs and throw warning if needed
         if not self.client.multiple_designs_allowed:
             logger.warning(
@@ -134,15 +137,15 @@
                 "designs open in the same session. Only the last design created "
                 "will be available to perform modeling operations."
             )
 
     @property
     def client(self) -> GrpcClient:
         """``Modeler`` instance client."""
-        return self._client
+        return self._grpc_client
 
     def create_design(self, name: str) -> "Design":
         """
         Initialize a new design with the connected client.
 
         Parameters
         ----------
@@ -162,25 +165,38 @@
         if len(self._designs) > 1:
             logger.warning(
                 "Some backends only support one design. "
                 + "Previous designs may be deleted (on the service) when creating a new one."
             )
         return self._designs[design.design_id]
 
-    def get_active_design(self) -> "Design":
+    def get_active_design(self, sync_with_backend: bool = True) -> "Design":
         """
         Get the active design on the modeler object.
 
+        Parameters
+        ----------
+        sync_with_backend : bool, default: True
+            Whether to sync the active design with the remote service. If set to False,
+            the active design may be out-of-sync with the remote service. This is useful
+            when the active design is known to be up-to-date.
+
         Returns
         -------
         Design
             Design object already existing on the modeler.
         """
         for _, design in self._designs.items():
             if design._is_active:
+
+                # Check if sync_with_backend is requested
+                if sync_with_backend:
+                    design._update_design_inplace()
+
+                # Return the active design
                 return design
 
         return None
 
     def read_existing_design(self) -> "Design":
         """
         Read the existing design on the service with the connected client.
@@ -241,15 +257,15 @@
             raise ValueError("File path must lead to a file, not a directory.")
 
         file_name = os.path.split(file_path)[1]
 
         with open(file_path, "rb") as file:
             data = file.read()
 
-        c_stub = CommandsStub(self._client.channel)
+        c_stub = CommandsStub(self._grpc_client.channel)
 
         response = c_stub.UploadFile(
             UploadFileRequest(
                 data=data,
                 file_name=file_name,
                 open=open_file,
                 import_options=import_options.to_dict(),
@@ -299,35 +315,55 @@
                 files = os.listdir(dir)
                 for file in files:
                     full_path = os.path.join(dir, file)
                     if full_path != file_path:
                         self._upload_file(full_path)
             self._upload_file(file_path, True, import_options)
         else:
-            DesignsStub(self._client.channel).Open(
+            DesignsStub(self._grpc_client.channel).Open(
                 OpenRequest(filepath=file_path, import_options=import_options.to_dict())
             )
 
         return self.read_existing_design()
 
     def __repr__(self) -> str:
         """Represent the modeler as a string."""
         lines = []
         lines.append(f"Ansys Geometry Modeler ({hex(id(self))})")
         lines.append("")
-        lines.append(str(self._client))
+        lines.append(str(self._grpc_client))
         return "\n".join(lines)
 
     @protect_grpc
     def run_discovery_script_file(
         self, file_path: str, script_args: Optional[Dict[str, str]] = None, import_design=False
     ) -> Tuple[Dict[str, str], Optional["Design"]]:
         """
         Run a Discovery script file.
 
+        .. note::
+
+            If arguments are passed to the script, they must be in the form of a dictionary.
+            On the server side, the script will receive the arguments as a dictionary of strings,
+            under the variable name ``argsDict``. For example, if the script is called with the
+            arguments ``run_discovery_script_file(..., script_args = {"length": "20"}, ...)``,
+            the script will receive the dictionary ``argsDict`` with the key-value pair
+            ``{"length": "20"}``.
+
+        .. note::
+
+            If an output is expected from the script, it will be returned as a dictionary of
+            strings. The keys and values of the dictionary are the variables and their values
+            that the script returns. However, it is necessary that the script creates a
+            dictionary called ``result`` with the variables and their values that are expected
+            to be returned. For example, if the script is expected to return the number of bodies
+            in the design, the script should create a dictionary called ``result`` with the
+            key-value pair ``{"numBodies": numBodies}``, where ``numBodies`` is the number of
+            bodies in the design.
+
         The implied API version of the script should match the API version of the running
         Geometry Service. DMS API versions 23.2.1 and later are supported. DMS is a
         Windows-based modeling service that has been containerized to ease distribution,
         execution, and remotability operations.
 
         Parameters
         ----------
@@ -352,30 +388,36 @@
         Raises
         ------
         GeometryRuntimeError
             If the Discovery script fails to run. Otherwise, assume that the script
             ran successfully.
         """
         serv_path = self._upload_file(file_path)
-        ga_stub = DbuApplicationStub(self._client.channel)
+        ga_stub = DbuApplicationStub(self._grpc_client.channel)
         request = RunScriptFileRequest(
             script_path=serv_path,
             script_args=script_args,
         )
 
         self.client.log.debug(f"Running Discovery script file at {file_path}...")
         response = ga_stub.RunScriptFile(request)
 
         if not response.success:
             raise GeometryRuntimeError(response.message)
 
         self.client.log.debug(f"Script result message: {response.message}")
 
         if import_design:
-            return (response.values, self.read_existing_design())
+            return (dict(response.values), self.read_existing_design())
         else:
-            return response.values
+            return dict(response.values)
 
     @property
     def repair_tools(self) -> RepairTools:
         """Access to repair tools."""
         return self._repair_tools
+
+    @property
+    @min_backend_version(24, 2, 0)
+    def measurement_tools(self) -> MeasurementTools:
+        """Access to measurement tools."""
+        return self._measurement_tools
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotter.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             Body of which to add the edges.
         **plotting_options : dict, default: None
             Keyword arguments. For allowable keyword arguments, see the
             :meth:`Plotter.add_mesh <pyvista.Plotter.add_mesh>` method.
         """
         edge_plot_list = []
         for edge in body_plot.object.edges:
-            line = pv.Line(edge.start_point, edge.end_point)
+            line = pv.Line(edge.shape.start, edge.shape.start)
             edge_actor = self.scene.add_mesh(
                 line, line_width=10, color=EDGE_COLOR, **plotting_options
             )
             edge_actor.SetVisibility(False)
             edge_plot = EdgePlot(edge_actor, edge, body_plot)
             edge_plot_list.append(edge_plot)
         body_plot.edges = edge_plot_list
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotter_helper.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/plotting_types.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotting_types.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/trame_gui.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/_images/isometric.png` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/button.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/displace_arrows.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/measure.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/ruler.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/show_design_point.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/show_design_point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/view_button.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/plotting/widgets/widget.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""PyAnsys Geometry primitives subpackage."""
+"""Provides the PyAnsys Geometry ``geometry`` subpackage."""
 
-from ansys.geometry.core.primitives.circle import Circle, CircleEvaluation
-from ansys.geometry.core.primitives.cone import Cone, ConeEvaluation
-from ansys.geometry.core.primitives.cylinder import Cylinder, CylinderEvaluation
-from ansys.geometry.core.primitives.ellipse import Ellipse, EllipseEvaluation
-from ansys.geometry.core.primitives.line import Line, LineEvaluation
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.circle import Circle, CircleEvaluation
+from ansys.geometry.core.shapes.curves.curve import Curve
+from ansys.geometry.core.shapes.curves.ellipse import Ellipse, EllipseEvaluation
+from ansys.geometry.core.shapes.curves.line import Line, LineEvaluation
+from ansys.geometry.core.shapes.parameterization import (
+    Interval,
     Parameterization,
     ParamForm,
     ParamType,
     ParamUV,
 )
-from ansys.geometry.core.primitives.sphere import Sphere, SphereEvaluation
-from ansys.geometry.core.primitives.surface_evaluation import SurfaceEvaluation
-from ansys.geometry.core.primitives.torus import Torus
+from ansys.geometry.core.shapes.surfaces.cone import Cone, ConeEvaluation
+from ansys.geometry.core.shapes.surfaces.cylinder import Cylinder, CylinderEvaluation
+from ansys.geometry.core.shapes.surfaces.plane import PlaneEvaluation, PlaneSurface
+from ansys.geometry.core.shapes.surfaces.sphere import Sphere, SphereEvaluation
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.surface_evaluation import SurfaceEvaluation
+from ansys.geometry.core.shapes.surfaces.torus import Torus
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/circle.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/circle.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.accuracy import Accuracy
 from ansys.geometry.core.misc.measurements import Distance
-from ansys.geometry.core.primitives.curve_evaluation import CurveEvaluation
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.curve import Curve
+from ansys.geometry.core.shapes.curves.curve_evaluation import CurveEvaluation
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
 )
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Circle:
+class Circle(Curve):
     """
     Provides 3D circle representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the circle.
@@ -223,37 +224,43 @@
         """
         return (
             Accuracy.length_is_equal(self.radius.m, other.radius.m)
             and self.origin == other.origin
             and self.dir_z == other.dir_z
         )
 
-    def get_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Parameterization:
         """
         Get the parametrization of the circle.
 
         The parameter of a circle specifies the clockwise angle around the axis
         (right-hand corkscrew law), with a zero parameter at ``dir_x`` and a
         period of 2*pi.
 
         Returns
         -------
         Parameterization
             Information about how the circle is parameterized.
         """
         return Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
 
+    def contains_param(self, param: Real) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
+
 
 class CircleEvaluation(CurveEvaluation):
     """
     Provides evaluation of a circle at a given parameter.
 
     Parameters
     ----------
-    circle: ~ansys.geometry.core.primitives.circle.Circle
+    circle: ~ansys.geometry.core.shapes.curves.circle.Circle
         Circle to evaluate.
     parameter: Real
         Parameter to evaluate the circle at.
     """
 
     def __init__(self, circle: Circle, parameter: Real) -> None:
         """``CircleEvaluation`` class constructor."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/cone.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cone.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,36 +20,37 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides for creating and managing a cone."""
 
 from functools import cached_property
 
 from beartype import beartype as check_input_types
-from beartype.typing import Union
+from beartype.typing import Tuple, Union
 import numpy as np
 from pint import Quantity
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.measurements import Angle, Distance
-from ansys.geometry.core.primitives.line import Line
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.line import Line
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
     ParamUV,
 )
-from ansys.geometry.core.primitives.surface_evaluation import SurfaceEvaluation
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.surface_evaluation import SurfaceEvaluation
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Cone:
+class Cone(Surface):
     """
     Provides 3D cone representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the cone.
@@ -231,54 +232,52 @@
         cone_radius = self.radius.m + v * np.tan(self.half_angle.m)
         point_radius = np.linalg.norm(point - line_eval.position)
         dist_to_cone = (point_radius - cone_radius) * np.cos(self.half_angle.m)
         v += dist_to_cone * np.sin(self.half_angle.m)
 
         return ConeEvaluation(self, ParamUV(u, v))
 
-    def get_u_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Tuple[Parameterization, Parameterization]:
         """
-        Get the parametrization conditions for the U parameter.
+        Parameterize the cone surface as a tuple (U and V respectively).
 
         The U parameter specifies the clockwise angle around the axis (right-hand
         corkscrew law), with a zero parameter at ``dir_x`` and a period of 2*pi.
 
-        Returns
-        -------
-        Parameterization
-            Information about how a cone's U parameter is parameterized.
-        """
-        return Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
-
-    def get_v_parameterization(self) -> Parameterization:
-        """
-        Get the parametrization conditions for the V parameter.
-
         The V parameter specifies the distance along the axis, with a zero parameter at
         the XY plane of the cone.
 
         Returns
         -------
-        Parameterization
-            Information about how a cone's V parameter is parameterized.
+        Tuple[Parameterization, Parameterization]
+            Information about how a cone's u and v parameters are parameterized, respectively.
         """
-        # V parameter interval depends on which way the cone opens
+        u = Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
+
         start, end = (
             (self.apex_param, np.inf) if self.apex_param < 0 else (np.NINF, self.apex_param)
         )
-        return Parameterization(ParamForm.OPEN, ParamType.LINEAR, Interval(start, end))
+        v = Parameterization(ParamForm.OPEN, ParamType.LINEAR, Interval(start, end))
+
+        return (u, v)
+
+    def contains_param(self, param_uv: ParamUV) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
 
 
 class ConeEvaluation(SurfaceEvaluation):
     """
     Evaluate the cone at given parameters.
 
     Parameters
     ----------
-    cone: ~ansys.geometry.core.primitives.cone.Cone
+    cone: ~ansys.geometry.core.shapes.surfaces.cone.Cone
         Cone to evaluate.
     parameter: ParamUV
         Pparameters (u, v) to evaluate the cone at.
     """
 
     def __init__(self, cone: Cone, parameter: ParamUV) -> None:
         """Initialize the ``ConeEvaluation`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/curve_evaluation.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/cylinder.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cylinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,57 +20,58 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides for creating and managing a cylinder."""
 
 from functools import cached_property
 
 from beartype import beartype as check_input_types
-from beartype.typing import Union
+from beartype.typing import Tuple, Union
 import numpy as np
-import pint
+from pint import Quantity
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.measurements import Distance
-from ansys.geometry.core.primitives.circle import Circle
-from ansys.geometry.core.primitives.line import Line
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.circle import Circle
+from ansys.geometry.core.shapes.curves.line import Line
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
     ParamUV,
 )
-from ansys.geometry.core.primitives.surface_evaluation import SurfaceEvaluation
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.surface_evaluation import SurfaceEvaluation
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Cylinder:
+class Cylinder(Surface):
     """
     Provides 3D cylinder representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the cylinder.
-    radius : Union[~pint.Quantity, Distance, Real]
+    radius : Union[Quantity, Distance, Real]
         Radius of the cylinder.
     reference : Union[~numpy.ndarray, RealSequence, UnitVector3D, Vector3D]
         X-axis direction.
     axis : Union[~numpy.ndarray, RealSequence, UnitVector3D, Vector3D]
         Z-axis direction.
     """
 
     @check_input_types
     def __init__(
         self,
         origin: Union[np.ndarray, RealSequence, Point3D],
-        radius: Union[pint.Quantity, Distance, Real],
+        radius: Union[Quantity, Distance, Real],
         reference: Union[np.ndarray, RealSequence, UnitVector3D, Vector3D] = UNITVECTOR3D_X,
         axis: Union[np.ndarray, RealSequence, UnitVector3D, Vector3D] = UNITVECTOR3D_Z,
     ):
         """Initialize the ``Cylinder`` class."""
         self._origin = Point3D(origin) if not isinstance(origin, Point3D) else origin
         self._reference = (
             UnitVector3D(reference) if not isinstance(reference, UnitVector3D) else reference
@@ -86,15 +87,15 @@
 
     @property
     def origin(self) -> Point3D:
         """Origin of the cylinder."""
         return self._origin
 
     @property
-    def radius(self) -> pint.Quantity:
+    def radius(self) -> Quantity:
         """Radius of the cylinder."""
         return self._radius.value
 
     @property
     def dir_x(self) -> UnitVector3D:
         """X-direction of the cylinder."""
         return self._reference
@@ -105,60 +106,60 @@
         return self.dir_z.cross(self.dir_x)
 
     @property
     def dir_z(self) -> UnitVector3D:
         """Z-direction of the cylinder."""
         return self._axis
 
-    def surface_area(self, height: Union[pint.Quantity, Distance, Real]) -> pint.Quantity:
+    def surface_area(self, height: Union[Quantity, Distance, Real]) -> Quantity:
         """
         Get the surface area of the cylinder.
 
         Notes
         -----
            By nature, a cylinder is infinite. If you want to get the surface area,
            you must bound it by a height. Normally a cylinder surface is not closed
            (does not have "caps" on the ends). This method assumes that the cylinder
            is closed for the purpose of getting the surface area.
 
         Parameters
         ----------
-        height : Union[~pint.Quantity, Distance, Real]
+        height : Union[Quantity, Distance, Real]
             Height to bound the cylinder at.
 
         Returns
         -------
-        ~pint.Quantity
+        Quantity
             Surface area of the temporarily bounded cylinder.
         """
         height = height if isinstance(height, Distance) else Distance(height)
         if height.value <= 0:
             raise ValueError("Height must be a real positive value.")
 
         return 2 * np.pi * self.radius * height.value + 2 * np.pi * self.radius**2
 
-    def volume(self, height: Union[pint.Quantity, Distance, Real]) -> pint.Quantity:
+    def volume(self, height: Union[Quantity, Distance, Real]) -> Quantity:
         """
         Get the volume of the cylinder.
 
         Notes
         -----
            By nature, a cylinder is infinite. If you want to get the surface area,
            you must bound it by a height. Normally a cylinder surface is not closed
            (does not have "caps" on the ends). This method assumes that the cylinder
            is closed for the purpose of getting the surface area.
 
         Parameters
         ----------
-        height : Union[~pint.Quantity, Distance, Real]
+        height : Union[Quantity, Distance, Real]
             Height to bound the cylinder at.
 
         Returns
         -------
-        ~pint.Quantity
+        Quantity
             Volume of the temporarily bounded cylinder.
         """
         height = height if isinstance(height, Distance) else Distance(height)
         if height.value <= 0:
             raise ValueError("Height must be a real positive value.")
 
         return np.pi * self.radius**2 * height.value
@@ -242,50 +243,48 @@
         u = circle.project_point(point).parameter
 
         line = Line(self.origin, self.dir_z)
         v = line.project_point(point).parameter
 
         return CylinderEvaluation(self, ParamUV(u, v))
 
-    def get_u_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Tuple[Parameterization, Parameterization]:
         """
-        Get the parametrization conditions for the U parameter.
+        Parameterize the cylinder surface as a tuple (U and V respectively).
 
         The U parameter specifies the clockwise angle around the axis (right-hand
         corkscrew law), with a zero parameter at ``dir_x`` and a period of 2*pi.
 
-        Returns
-        -------
-        Parameterization
-            Information about how the cylinder's U parameter is parameterized.
-        """
-        return Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
-
-    def get_v_parameterization(self) -> Parameterization:
-        """
-        Get the parametrization conditions for the V parameter.
-
         The V parameter specifies the distance along the axis, with a zero parameter at
         the XY plane of the cylinder.
 
         Returns
         -------
-        Parameterization
-            Information about how the cylinders's V parameter is parameterized.
+        Tuple[Parameterization, Parameterization]
+            Information about how a cylinder's u and v parameters are parameterized, respectively.
         """
-        return Parameterization(ParamForm.OPEN, ParamType.LINEAR, Interval(np.NINF, np.inf))
+        u = Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
+        v = Parameterization(ParamForm.OPEN, ParamType.LINEAR, Interval(np.NINF, np.inf))
+
+        return (u, v)
+
+    def contains_param(self, param_uv: ParamUV) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
 
 
 class CylinderEvaluation(SurfaceEvaluation):
     """
     Provides evaluation of a cylinder at given parameters.
 
     Parameters
     ----------
-    cylinder: Cylinder
+    cylinder: ~ansys.geometry.core.shapes.surfaces.cylinder.Cylinder
         Cylinder to evaluate.
     parameter: ParamUV
         Parameters (u, v) to evaluate the cylinder at.
     """
 
     def __init__(self, cylinder: Cylinder, parameter: ParamUV) -> None:
         """Initialize the ``CylinderEvaluation`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/ellipse.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/ellipse.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.accuracy import Accuracy
 from ansys.geometry.core.misc.measurements import Distance
-from ansys.geometry.core.primitives.curve_evaluation import CurveEvaluation
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.curve import Curve
+from ansys.geometry.core.shapes.curves.curve_evaluation import CurveEvaluation
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
 )
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Ellipse:
+class Ellipse(Curve):
     """
     Provides 3D ellipse representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the ellipse.
@@ -285,36 +286,42 @@
             new_point,
             self.major_radius,
             self.minor_radius,
             UnitVector3D(new_reference[0:3]),
             UnitVector3D(new_axis[0:3]),
         )
 
-    def get_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Parameterization:
         """
         Get the parametrization of the ellipse.
 
         The parameter of an ellipse specifies the clockwise angle around the axis
         (right-hand corkscrew law), with a zero parameter at ``dir_x`` and a period of 2*pi.
 
         Returns
         -------
         Parameterization
             Information about how the ellipse is parameterized.
         """
         return Parameterization(ParamForm.PERIODIC, ParamType.OTHER, Interval(0, 2 * np.pi))
 
+    def contains_param(self, param: Real) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
+
 
 class EllipseEvaluation(CurveEvaluation):
     """
     Evaluate an ellipse at a given parameter.
 
     Parameters
     ----------
-    ellipse: Ellipse
+    ellipse: ~ansys.geometry.core.shapes.curves.ellipse.Ellipse
         Ellipse to evaluate.
     parameter: float, int
         Parameter to evaluate the ellipse at.
     """
 
     def __init__(self, ellipse: Ellipse, parameter: Real) -> None:
         """``Initialize the ``EllipseEvaluation`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/line.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,26 @@
 from beartype.typing import Union
 import numpy as np
 
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.accuracy import LENGTH_ACCURACY
-from ansys.geometry.core.primitives.curve_evaluation import CurveEvaluation
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.curves.curve import Curve
+from ansys.geometry.core.shapes.curves.curve_evaluation import CurveEvaluation
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
 )
-from ansys.geometry.core.typing import RealSequence
+from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Line:
+class Line(Curve):
     """
     Provides 3D line representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the line.
@@ -175,31 +176,37 @@
         bool
             ``True`` if the line is opposite to another line.
         """
         if self.is_coincident_line(other):
             return self.direction.is_opposite(other.direction)
         return False
 
-    def get_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Parameterization:
         """
         Get the parametrization of the line.
 
         The parameter of a line specifies the distance from the `origin` in the
         direction of `direction`.
 
         Returns
         -------
         Parameterization
             Information about how the line is parameterized.
         """
         return Parameterization(ParamForm.OPEN, ParamType.LINEAR, Interval(np.NINF, np.inf))
 
+    def contains_param(self, param: Real) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
+
 
 class LineEvaluation(CurveEvaluation):
-    """Evaluate a line."""
+    """Provides for evaluating a line."""
 
     def __init__(self, line: Line, parameter: float = None) -> None:
         """Initialize the ``LineEvaluation`` class."""
         self._line = line
         self._parameter = parameter
 
     @property
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/sphere.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/sphere.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,35 +20,36 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides for creating and managing a sphere."""
 
 from functools import cached_property
 
 from beartype import beartype as check_input_types
-from beartype.typing import Union
+from beartype.typing import Tuple, Union
 import numpy as np
 from pint import Quantity
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.measurements import Distance
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
     ParamUV,
 )
-from ansys.geometry.core.primitives.surface_evaluation import SurfaceEvaluation
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.surface_evaluation import SurfaceEvaluation
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Sphere:
+class Sphere(Surface):
     """
     Provides 3D sphere representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D]
         Origin of the sphere.
@@ -199,51 +200,49 @@
         if np.allclose((x * x + y * y + z * z), Point3D([0, 0, 0])):
             return SphereEvaluation(self, ParamUV(0, np.pi / 2))
 
         u = np.arctan2(y, x)
         v = np.arctan2(z, np.sqrt(x * x + y * y))
         return SphereEvaluation(self, ParamUV(u, v))
 
-    def get_u_parameterization(self) -> Parameterization:
+    def parameterization(self) -> Tuple[Parameterization, Parameterization]:
         """
-        Get the parametrization conditions for the U parameter.
+        Parameterization of the sphere surface as a tuple (U and V respectively).
 
         The U parameter specifies the longitude angle, increasing clockwise (east) about
         ``dir_z`` (right-hand corkscrew law). It has a zero parameter at ``dir_x`` and a
         period of ``2*pi``.
 
+        The V parameter specifies the latitude, increasing north, with a zero parameter
+        at the equator and a range of [-pi/2, pi/2].
+
         Returns
         -------
-        Parameterization
-            Information about how a sphere's U parameter is parameterized.
+        Tuple[Parameterization, Parameterization]
+            Information about how a sphere's u and v parameters are parameterized, respectively.
         """
-        return Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
+        u = Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
+        v = Parameterization(ParamForm.CLOSED, ParamType.OTHER, Interval(-np.pi / 2, np.pi / 2))
 
-    def get_v_parameterization(self) -> Parameterization:
-        """
-        Get the parametrization conditions for the V parameter.
+        return (u, v)
 
-        The V parameter specifies the latitude, increasing north, with a zero parameter
-        at the equator and a range of ``[-pi/2, pi/2]``.
+    def contains_param(self, param_uv: ParamUV) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
 
-        Returns
-        -------
-        Parameterization
-            Information about how a sphere's V parameter is parameterized.
-        """
-        return Parameterization(ParamForm.CLOSED, ParamType.OTHER, Interval(-np.pi / 2, np.pi / 2))
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
 
 
 class SphereEvaluation(SurfaceEvaluation):
     """
     Evaluate a sphere at given parameters.
 
     Parameters
     ----------
-    sphere: ~ansys.geometry.core.primitives.sphere.Sphere
+    sphere: ~ansys.geometry.core.shapes.surfaces.sphere.Sphere
         Sphere to evaluate.
     parameter: ParamUV
         Parameters (u, v) to evaluate the sphere at.
     """
 
     def __init__(self, sphere: Sphere, parameter: ParamUV) -> None:
         """Initialize the ``SphereEvaluation`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/surface_evaluation.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 # SOFTWARE.
 """Provides for evaluating a surface."""
 
 from functools import cached_property
 
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
-from ansys.geometry.core.primitives.parameterization import ParamUV
+from ansys.geometry.core.shapes.parameterization import ParamUV
 from ansys.geometry.core.typing import Real
 
 
 class SurfaceEvaluation:
     """Provides for evaluating a surface."""
 
     def __init__(self, parameter: ParamUV) -> None:
         """Initialize the ``SurfaceEvaluation`` class."""
         self._parameter = parameter
 
     @property
-    def parameter(self) -> Real:
+    def parameter(self) -> ParamUV:
         """Parameter that the evaluation is based upon."""
         raise NotImplementedError("Each evaluation must provide the parameter definition.")
 
     @cached_property
     def position(self) -> Point3D:
         """Point on the surface, based on the evaluation."""
         raise NotImplementedError("Each evaluation must provide the position definition.")
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/primitives/torus.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/torus.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,36 @@
 # SOFTWARE.
 """Provides for creating and managing a torus."""
 
 from functools import cached_property
 from typing import Tuple
 
 from beartype import beartype as check_input_types
-from beartype.typing import Union
+from beartype.typing import Tuple, Union
 import numpy as np
 from pint import Quantity
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
 from ansys.geometry.core.math.matrix import Matrix44
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D, Vector3D
 from ansys.geometry.core.misc.measurements import Distance
-from ansys.geometry.core.primitives.parameterization import (
+from ansys.geometry.core.shapes.parameterization import (
     Interval,
     Parameterization,
     ParamForm,
     ParamType,
     ParamUV,
 )
-from ansys.geometry.core.primitives.surface_evaluation import SurfaceEvaluation
+from ansys.geometry.core.shapes.surfaces.surface import Surface
+from ansys.geometry.core.shapes.surfaces.surface_evaluation import SurfaceEvaluation
 from ansys.geometry.core.typing import Real, RealSequence
 
 
-class Torus:
+class Torus(Surface):
     """
     Provides 3D torus representation.
 
     Parameters
     ----------
     origin : Union[~numpy.ndarray, RealSequence, Point3D],
         Centered origin of the torus.
@@ -190,48 +191,40 @@
         Returns
         -------
         TorusEvaluation
             Resulting evaluation.
         """
         return TorusEvaluation(self, parameter)
 
-    def get_u_parameterization(self):
+    def parameterization(self) -> Tuple[Parameterization, Parameterization]:
         """
-        Get the parametrization conditions for the U parameter.
+        Parameterize the torus surface as a tuple (U and V respectively).
 
         The U parameter specifies the longitude angle, increasing clockwise (east) about
         the axis (right-hand corkscrew law). It has a zero parameter at
         ``Geometry.Frame.DirX`` and a period of ``2*pi``.
 
-        Returns
-        -------
-        Parameterization
-            Information about how a sphere's U parameter is parameterized.
-        """
-        return Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
-
-    def get_v_parameterization(self) -> Parameterization:
-        """
-        Get the parametrization conditions of the V parameter.
-
         The V parameter specifies the latitude, increasing north, with a zero parameter
-        at the equator. For the donut, where the ``Geometry.Torus.MajorRadius`` is greater
-        than the ``Geometry.Torus.MinorRadius``, the range is ``[-pi, pi]`` and the
+        at the equator. For the donut, where the major radius is greater
+        than the minor radius, the range is [-pi, pi] and the
         parameterization is periodic. For a degenerate torus, the range is restricted
         accordingly and the parameterization is non-periodic.
 
         Returns
         -------
-        Parameterization
-            Information about how a torus's V parameter is parameterized.
+        Tuple[Parameterization, Parameterization]
+            Information about how a torus's u and v parameters are parameterized, respectively.
         """
-        return Parameterization(
+        u = Parameterization(ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(0, 2 * np.pi))
+        v = Parameterization(
             ParamForm.PERIODIC, ParamType.CIRCULAR, Interval(-np.pi / 2, np.pi / 2)
         )
 
+        return (u, v)
+
     def project_point(self, point: Point3D) -> "TorusEvaluation":
         """
         Project a point onto the torus and evaluate the torus.
 
         Parameters
         ----------
         point : Point3D
@@ -258,22 +251,28 @@
         ) < np.power(
             np.linalg.norm((TorusEvaluation(self, ParamUV(u + np.pi, v2)).position() - point)), 2
         ):
             return TorusEvaluation(self, ParamUV(u, v1))
         else:
             return TorusEvaluation(self, ParamUV(u + np.pi, v2))
 
+    def contains_param(self, param_uv: ParamUV) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_param() is not implemented.")
+
+    def contains_point(self, point: Point3D) -> bool:  # noqa: D102
+        raise NotImplementedError("contains_point() is not implemented.")
+
 
 class TorusEvaluation(SurfaceEvaluation):
     """
     Evaluate the torus`` at given parameters.
 
     Parameters
     ----------
-    Torus: ~ansys.geometry.core.primitives.torus.Torus
+    Torus: ~ansys.geometry.core.shapes.surfaces.torus.Torus
         Torust to evaluate.
     parameter: ParamUV
         Parameters (u, v) to evaluate the torus at.
     """
 
     def __init__(self, torus: Torus, parameter: ParamUV) -> None:
         """Initiate the ``TorusEvaluation`` class."""
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/arc.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/arc.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/box.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/box.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/circle.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from beartype.typing import Optional, Union
 from pint import Quantity
 import pyvista as pv
 
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point2D, Point3D
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Distance
-from ansys.geometry.core.primitives.circle import Circle
+from ansys.geometry.core.shapes.curves.circle import Circle
 from ansys.geometry.core.sketch.face import SketchFace
 from ansys.geometry.core.typing import Real
 
 
 class SketchCircle(SketchFace, Circle):
     """
     Provides for modeling a circle.
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/edge.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/edge.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from beartype.typing import TYPE_CHECKING
 from pint import Quantity
 import pyvista as pv
 
 from ansys.geometry.core.math.point import Point2D
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.math.plane import Plane
 
 
 class SketchEdge:
     """Provides for modeling edges forming sketched shapes."""
 
     @property
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/ellipse.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 from ansys.geometry.core.math.matrix import Matrix33, Matrix44
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point2D, Point3D
 from ansys.geometry.core.math.vector import Vector3D
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Angle, Distance
 from ansys.geometry.core.misc.units import UNITS
-from ansys.geometry.core.primitives.ellipse import Ellipse
+from ansys.geometry.core.shapes.curves.ellipse import Ellipse
 from ansys.geometry.core.sketch.face import SketchFace
 from ansys.geometry.core.typing import Real
 
 
 class SketchEllipse(SketchFace, Ellipse):
     """
     Provides for modeling an ellipse.
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/face.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/face.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from beartype.typing import TYPE_CHECKING, List
 from pint import Quantity
 import pyvista as pv
 
 from ansys.geometry.core.sketch.edge import SketchEdge
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.math.plane import Plane
 
 
 class SketchFace:
     """Provides for modeling a face."""
 
     def __init__(self):
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/gears.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/gears.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/polygon.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/polygon.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/segment.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import pyvista as pv
 
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point2D, Point3D
 from ansys.geometry.core.math.vector import UnitVector3D
 from ansys.geometry.core.misc.checks import check_ndarray_is_all_nan
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
-from ansys.geometry.core.primitives.line import Line
+from ansys.geometry.core.shapes.curves.line import Line
 from ansys.geometry.core.sketch.edge import SketchEdge
 
 
 class SketchSegment(SketchEdge, Line):
     """
     Provides segment representation of a line.
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/sketch.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/sketch.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/slot.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/slot.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/trapezoid.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/trapezoid.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/sketch/triangle.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/triangle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/__init__.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """PyAnsys Geometry tools subpackage."""
 
+from ansys.geometry.core.tools.measurement_tools import MeasurementTools
 from ansys.geometry.core.tools.problem_areas import (
     DuplicateFaceProblemAreas,
     ExtraEdgeProblemAreas,
     InexactEdgeProblemAreas,
 )
 from ansys.geometry.core.tools.repair_tool_message import RepairToolMessage
 from ansys.geometry.core.tools.repair_tools import RepairTools
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/problem_areas.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/problem_areas.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,20 +27,31 @@
     FixInexactEdgesRequest,
     FixMissingFacesRequest,
     FixSmallFacesRequest,
     FixSplitEdgesRequest,
     FixStitchFacesRequest,
 )
 from ansys.api.geometry.v0.repairtools_pb2_grpc import RepairToolsStub
-from beartype.typing import List
+from beartype.typing import TYPE_CHECKING, List
 from google.protobuf.wrappers_pb2 import Int32Value
 
 from ansys.geometry.core.connection import GrpcClient
+from ansys.geometry.core.misc.auxiliary import (
+    get_design_from_body,
+    get_design_from_edge,
+    get_design_from_face,
+)
+from ansys.geometry.core.misc.checks import check_type_all_elements_in_iterable
 from ansys.geometry.core.tools.repair_tool_message import RepairToolMessage
 
+if TYPE_CHECKING:  # pragma: no cover
+    from ansys.geometry.core.designer.body import Body
+    from ansys.geometry.core.designer.edge import Edge
+    from ansys.geometry.core.designer.face import Face
+
 
 class ProblemArea:
     """
     Represents problem areas.
 
     Parameters
     ----------
@@ -75,88 +86,107 @@
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    faces : List[str]
+    faces : List[Face]
         List of faces associated with the design.
     """
 
-    def __init__(self, id: str, faces: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, faces: List["Face"]):
         """Initialize a new instance of the duplicate face problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.face import Face
+
+        # Verify that all elements in the list are of type Face
+        check_type_all_elements_in_iterable(faces, Face)
+
         self._faces = faces
 
     @property
-    def faces(self) -> List[str]:
-        """
-        The list of the problem area ids.
-
-        This method returns the list of problem area ids with duplicate faces.
-        """
+    def faces(self) -> List["Face"]:
+        """The list of the edges connected to this problem area."""
         return self._faces
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.faces:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_face(self.faces[0])
         response = self._repair_stub.FixDuplicateFaces(
             FixDuplicateFacesRequest(duplicate_face_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
+
         return message
 
 
 class MissingFaceProblemAreas(ProblemArea):
     """
     Provides missing face problem area definition.
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    edges : List[str]
+    edges : List[Edge]
         List of edges associated with the design.
     """
 
-    def __init__(self, id: str, edges: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, edges: List["Edge"]):
         """Initialize a new instance of the missing face problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.edge import Edge
+
+        # Verify that all elements in the list are of type Edge
+        check_type_all_elements_in_iterable(edges, Edge)
+
         self._edges = edges
 
     @property
-    def edges(self) -> List[str]:
-        """The list of the ids of the edges connected to this problem area."""
+    def edges(self) -> List["Edge"]:
+        """The list of the edges connected to this problem area."""
         return self._edges
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.edges:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_edge(self.edges[0])
         response = self._repair_stub.FixMissingFaces(
             FixMissingFacesRequest(missing_face_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
         return message
 
@@ -167,40 +197,51 @@
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    edges : List[str]
+    edges : List[Edge]
         List of edges associated with the design.
     """
 
-    def __init__(self, id: str, edges: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, edges: List["Edge"]):
         """Initialize a new instance of the inexact edge problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.edge import Edge
+
+        # Verify that all elements in the list are of type Edge
+        check_type_all_elements_in_iterable(edges, Edge)
+
         self._edges = edges
 
     @property
-    def edges(self) -> List[str]:
-        """The list of the ids of the edges connected to this problem area."""
+    def edges(self) -> List["Edge"]:
+        """The list of the edges connected to this problem area."""
         return self._edges
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.edges:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_edge(self.edges[0])
         response = self._repair_stub.FixInexactEdges(
             FixInexactEdgesRequest(inexact_edge_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
         return message
 
@@ -211,65 +252,82 @@
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    edges : List[str]
+    edges : List[Edge]
         List of edges associated with the design.
     """
 
-    def __init__(self, id: str, edges: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, edges: List["Edge"]):
         """Initialize a new instance of the extra edge problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.edge import Edge
+
+        # Verify that all elements in the list are of type Edge
+        check_type_all_elements_in_iterable(edges, Edge)
+
         self._edges = edges
 
     @property
-    def edges(self) -> List[str]:
+    def edges(self) -> List["Edge"]:
         """The list of the ids of the edges connected to this problem area."""
         return self._edges
 
 
 class SmallFaceProblemAreas(ProblemArea):
     """
     Represents a small face problem area with unique identifier and associated faces.
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    faces : List[str]
+    faces : List[Face]
         List of edges associated with the design.
     """
 
-    def __init__(self, id: str, faces: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, faces: List["Face"]):
         """Initialize a new instance of the small face problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.face import Face
+
+        # Verify that all elements in the list are of type Face
+        check_type_all_elements_in_iterable(faces, Face)
+
         self._faces = faces
 
     @property
-    def faces(self) -> List[str]:
+    def faces(self) -> List["Face"]:
         """The list of the ids of the edges connected to this problem area."""
         return self._faces
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.faces:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_face(self.faces[0])
         response = self._repair_stub.FixSmallFaces(
             FixSmallFacesRequest(small_face_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
         return message
 
@@ -280,40 +338,51 @@
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    edges : List[str]
+    edges : List[Edge]
         List of edges associated with the design.
     """
 
-    def __init__(self, id: str, edges: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, edges: List["Edge"]):
         """Initialize a new instance of the split edge problem area class."""
         super().__init__(id, grpc_client)
+
+        from ansys.geometry.core.designer.edge import Edge
+
+        # Verify that all elements in the list are of type Edge
+        check_type_all_elements_in_iterable(edges, Edge)
+
         self._edges = edges
 
     @property
-    def edges(self) -> List[str]:
-        """The list of the ids of the edges connected to this problem area."""
+    def edges(self) -> List["Edge"]:
+        """The list of edges connected to this problem area."""
         return self._edges
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.edges:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_edge(self.edges[0])
         response = self._repair_stub.FixSplitEdges(
             FixSplitEdgesRequest(split_edge_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
         return message
 
@@ -324,39 +393,50 @@
 
     Parameters
     ----------
     id : str
         Server-defined ID for the body.
     grpc_client : GrpcClient
         Active supporting geometry service instance for design modeling.
-    faces : List[str]
-        List of faces associated with the design.
+    bodies : List[Body]
+        List of bodies associated with the design.
     """
 
-    def __init__(self, id: str, faces: List[str], grpc_client: GrpcClient):
+    def __init__(self, id: str, grpc_client: GrpcClient, bodies: List["Body"]):
         """Initialize a new instance of the stitch face problem area class."""
         super().__init__(id, grpc_client)
-        self._faces = faces
+
+        from ansys.geometry.core.designer.body import Body
+
+        # Verify that all elements in the list are of type Body
+        check_type_all_elements_in_iterable(bodies, Body)
+
+        self._bodies = bodies
 
     @property
-    def faces(self) -> List[str]:
-        """The list of the ids of the faces connected to this problem area."""
-        return self._faces
+    def bodies(self) -> List["Body"]:
+        """The list of the bodies connected to this problem area."""
+        return self._bodies
 
     def fix(self) -> RepairToolMessage:
         """
         Fix the problem area.
 
         Returns
         -------
         message: RepairToolMessage
             Message containing created and/or modified bodies.
         """
+        if not self.bodies:
+            return RepairToolMessage(False, [], [])
+
+        parent_design = get_design_from_body(self.bodies[0])
         response = self._repair_stub.FixStitchFaces(
             FixStitchFacesRequest(stitch_face_problem_area_id=self._id_grpc)
         )
+        parent_design._update_design_inplace()
         message = RepairToolMessage(
             response.result.success,
             response.result.created_bodies_monikers,
             response.result.modified_bodies_monikers,
         )
         return message
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/repair_tool_message.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tool_message.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/tools/repair_tools.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,32 +28,37 @@
     FindMissingFacesRequest,
     FindSmallFacesRequest,
     FindSplitEdgesRequest,
     FindStitchFacesRequest,
 )
 from ansys.api.geometry.v0.repairtools_pb2_grpc import RepairToolsStub
 from beartype.typing import TYPE_CHECKING, List
-
-if TYPE_CHECKING:  # pragma: no cover
-    from ansys.geometry.core.designer.body import Body
-
 from google.protobuf.wrappers_pb2 import DoubleValue
 
 from ansys.geometry.core.connection import GrpcClient
+from ansys.geometry.core.misc.auxiliary import (
+    get_bodies_from_ids,
+    get_design_from_body,
+    get_edges_from_ids,
+    get_faces_from_ids,
+)
 from ansys.geometry.core.tools.problem_areas import (
     DuplicateFaceProblemAreas,
     ExtraEdgeProblemAreas,
     InexactEdgeProblemAreas,
     MissingFaceProblemAreas,
     SmallFaceProblemAreas,
     SplitEdgeProblemAreas,
     StitchFaceProblemAreas,
 )
 from ansys.geometry.core.typing import Real
 
+if TYPE_CHECKING:  # pragma: no cover
+    from ansys.geometry.core.designer.body import Body
+
 
 class RepairTools:
     """Repair tools for PyAnsys Geometry."""
 
     def __init__(self, grpc_client: GrpcClient):
         """Initialize Repair Tools class."""
         self._grpc_client = grpc_client
@@ -78,29 +83,35 @@
             The maximum length of the edges.
 
         Returns
         -------
         List[SplitEdgeProblemAreas]
             List of objects representing split edge problem areas.
         """
+        if not bodies:
+            return []
+
         angle_value = DoubleValue(value=float(angle))
         length_value = DoubleValue(value=float(length))
         body_ids = [body.id for body in bodies]
 
         problem_areas_response = self._repair_stub.FindSplitEdges(
             FindSplitEdgesRequest(
                 bodies_or_faces=body_ids, angle=angle_value, distance=length_value
             )
         )
-
-        problem_areas = [
-            SplitEdgeProblemAreas(res.id, list(res.edge_monikers), self._grpc_client)
+        parent_design = get_design_from_body(bodies[0])
+        return [
+            SplitEdgeProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_edges_from_ids(parent_design, res.edge_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_extra_edges(self, bodies: List["Body"]) -> List[ExtraEdgeProblemAreas]:
         """
         Find the extra edges in the given list of bodies.
 
         This method find the extra edge problem areas and returns a list of extra edge
         problem areas objects.
@@ -111,23 +122,31 @@
             List of bodies that extra edges are investigated on.
 
         Returns
         -------
         List[ExtraEdgeProblemArea]
             List of objects representing extra edge problem areas.
         """
+        if not bodies:
+            return []
+
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindExtraEdges(
             FindExtraEdgesRequest(selection=body_ids)
         )
-        problem_areas = [
-            ExtraEdgeProblemAreas(res.id, list(res.edge_monikers), self._grpc_client)
+        parent_design = get_design_from_body(bodies[0])
+
+        return [
+            ExtraEdgeProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_edges_from_ids(parent_design, res.edge_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_inexact_edges(self, bodies: List["Body"]) -> List[InexactEdgeProblemAreas]:
         """
         Find inexact edges in the given list of bodies.
 
         This method find the inexact edge problem areas and returns a list of inexact
         edge problem areas objects.
@@ -138,23 +157,32 @@
             List of bodies that inexact edges are investigated on.
 
         Returns
         -------
         List[InExactEdgeProblemArea]
             List of objects representing inexact edge problem areas.
         """
+        if not bodies:
+            return []
+
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindInexactEdges(
             FindInexactEdgesRequest(selection=body_ids)
         )
-        problem_areas = [
-            InexactEdgeProblemAreas(res.id, list(res.edge_monikers), self._grpc_client)
+
+        parent_design = get_design_from_body(bodies[0])
+
+        return [
+            InexactEdgeProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_edges_from_ids(parent_design, res.edge_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_duplicate_faces(self, bodies: List["Body"]) -> List[DuplicateFaceProblemAreas]:
         """
         Find the duplicate face problem areas.
 
         This method finds the duplicate face problem areas and returns a list of
         duplicate face problem areas objects.
@@ -165,23 +193,31 @@
             List of bodies that duplicate faces are investigated on.
 
         Returns
         -------
         List[DuplicateFaceProblemAreas]
             List of objects representing duplicate face problem areas.
         """
+        if not bodies:
+            return []
+
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindDuplicateFaces(
             FindDuplicateFacesRequest(faces=body_ids)
         )
-        problem_areas = [
-            DuplicateFaceProblemAreas(res.id, list(res.face_monikers), self._grpc_client)
+
+        parent_design = get_design_from_body(bodies[0])
+        return [
+            DuplicateFaceProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_faces_from_ids(parent_design, res.face_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_missing_faces(self, bodies: List["Body"]) -> List[MissingFaceProblemAreas]:
         """
         Find the missing faces.
 
         This method find the missing face problem areas and returns a list of missing
         face problem areas objects.
@@ -192,23 +228,30 @@
             List of bodies that missing faces are investigated on.
 
         Returns
         -------
         List[MissingFaceProblemAreas]
             List of objects representing missing face problem areas.
         """
+        if not bodies:
+            return []
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindMissingFaces(
             FindMissingFacesRequest(faces=body_ids)
         )
-        problem_areas = [
-            MissingFaceProblemAreas(res.id, list(res.edge_monikers), self._grpc_client)
+        parent_design = get_design_from_body(bodies[0])
+
+        return [
+            MissingFaceProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_edges_from_ids(parent_design, res.edge_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_small_faces(self, bodies: List["Body"]) -> List[SmallFaceProblemAreas]:
         """
         Find the small face problem areas.
 
         This method finds and returns a list of ids of small face problem areas
         objects.
@@ -219,23 +262,31 @@
             List of bodies that small faces are investigated on.
 
         Returns
         -------
         List[SmallFaceProblemAreas]
             List of objects representing small face problem areas.
         """
+        if not bodies:
+            return []
+
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindSmallFaces(
             FindSmallFacesRequest(selection=body_ids)
         )
-        problem_areas = [
-            SmallFaceProblemAreas(res.id, list(res.face_monikers), self._grpc_client)
+        parent_design = get_design_from_body(bodies[0])
+
+        return [
+            SmallFaceProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_faces_from_ids(parent_design, res.face_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
 
     def find_stitch_faces(self, bodies: List["Body"]) -> List[StitchFaceProblemAreas]:
         """
         Return the list of stitch face problem areas.
 
         This method find the stitch face problem areas and returns a list of ids of stitch face
         problem areas objects.
@@ -250,12 +301,16 @@
         List[StitchFaceProblemAreas]
             List of objects representing stitch face problem areas.
         """
         body_ids = [body.id for body in bodies]
         problem_areas_response = self._repair_stub.FindStitchFaces(
             FindStitchFacesRequest(faces=body_ids)
         )
-        problem_areas = [
-            StitchFaceProblemAreas(res.id, list(res.body_monikers), self._grpc_client)
+        parent_design = get_design_from_body(bodies[0])
+        return [
+            StitchFaceProblemAreas(
+                str(res.id),
+                self._grpc_client,
+                get_bodies_from_ids(parent_design, res.body_monikers),
+            )
             for res in problem_areas_response.result
         ]
-        return problem_areas
```

### Comparing `ansys_geometry_core-0.4.9/src/ansys/geometry/core/typing.py` & `ansys_geometry_core-0.5.0/src/ansys/geometry/core/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.4.9/PKG-INFO` & `ansys_geometry_core-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 Metadata-Version: 2.1
 Name: ansys-geometry-core
-Version: 0.4.9
+Version: 0.5.0
 Summary: A python wrapper for Ansys Geometry service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ansys-api-geometry==0.3.5
+Requires-Dist: ansys-api-geometry==0.4.1
 Requires-Dist: ansys-tools-path>=0.3,<1
-Requires-Dist: beartype>=0.11.0,<1
+Requires-Dist: beartype>=0.11.0,<0.19
 Requires-Dist: google-api-python-client>=1.7.11,<3
 Requires-Dist: googleapis-common-protos>=1.52.0,<2
 Requires-Dist: grpcio>=1.35.0,<2
 Requires-Dist: grpcio-health-checking>=1.45.0,<2
 Requires-Dist: numpy>=1.20.3,<2
 Requires-Dist: Pint>=0.18,<1
 Requires-Dist: protobuf>=3.20.2,<5
 Requires-Dist: pyvista>=0.37.0,<1
 Requires-Dist: scipy>=1.7.3,<2
 Requires-Dist: six>=1.16.0,<2
 Requires-Dist: vtk>=9,<10
+Requires-Dist: semver>=3,<4
 Requires-Dist: ansys-platform-instancemanagement>=1.0.3,<2 ; extra == "all"
 Requires-Dist: docker>=6.0.1,<8 ; extra == "all"
 Requires-Dist: pyvista[jupyter]>=0.38.1,<0.42 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.13.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
+Requires-Dist: beartype==0.18.2 ; extra == "doc"
 Requires-Dist: docker==7.0.0 ; extra == "doc"
 Requires-Dist: ipyvtklink==0.2.3 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: jupytext==1.16.1 ; extra == "doc"
 Requires-Dist: myst-parser==2.0.0 ; extra == "doc"
-Requires-Dist: nbconvert==7.14.2 ; extra == "doc"
+Requires-Dist: nbconvert==7.16.3 ; extra == "doc"
 Requires-Dist: nbsphinx==0.9.3 ; extra == "doc"
-Requires-Dist: notebook==7.0.7 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
-Requires-Dist: panel==1.3.8 ; extra == "doc"
-Requires-Dist: pyvista[jupyter]==0.43.2 ; extra == "doc"
+Requires-Dist: notebook==7.1.2 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
+Requires-Dist: panel==1.4.1 ; extra == "doc"
+Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "doc"
 Requires-Dist: requests==2.31.0 ; extra == "doc"
 Requires-Dist: sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: sphinx-autoapi==3.0.0 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: sphinx_design==0.5.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: vtk==9.3.0 ; extra == "doc"
 Requires-Dist: ansys-platform-instancemanagement==1.1.2 ; extra == "tests"
-Requires-Dist: ansys-tools-path==0.4.1 ; extra == "tests"
-Requires-Dist: beartype==0.17.0 ; extra == "tests"
+Requires-Dist: ansys-tools-path==0.5.1 ; extra == "tests"
+Requires-Dist: beartype==0.18.2 ; extra == "tests"
 Requires-Dist: docker==7.0.0 ; extra == "tests"
-Requires-Dist: google-api-python-client==2.116.0 ; extra == "tests"
-Requires-Dist: googleapis-common-protos==1.62.0 ; extra == "tests"
-Requires-Dist: grpcio==1.60.0 ; extra == "tests"
+Requires-Dist: google-api-python-client==2.122.0 ; extra == "tests"
+Requires-Dist: googleapis-common-protos==1.63.0 ; extra == "tests"
+Requires-Dist: grpcio==1.62.1 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.60.0 ; extra == "tests"
-Requires-Dist: numpy==1.26.3 ; extra == "tests"
+Requires-Dist: numpy==1.26.4 ; extra == "tests"
 Requires-Dist: Pint==0.23 ; extra == "tests"
 Requires-Dist: protobuf==4.25.1 ; extra == "tests"
-Requires-Dist: pytest==8.0.0 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests"
-Requires-Dist: pyvista[jupyter]==0.43.2 ; extra == "tests"
+Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "tests"
 Requires-Dist: requests==2.31.0 ; extra == "tests"
-Requires-Dist: scipy==1.12.0 ; extra == "tests"
+Requires-Dist: scipy==1.13.0 ; extra == "tests"
+Requires-Dist: semver==3.0.2 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: vtk==9.3.0 ; extra == "tests"
 Project-URL: Discussions, https://github.com/ansys/pyansys-geometry/discussions
 Project-URL: Documentation, https://geometry.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyansys-geometry/issues
 Project-URL: Releases, https://github.com/ansys/pyansys-geometry/releases
 Project-URL: Source, https://github.com/ansys/pyansys-geometry
@@ -106,15 +107,15 @@
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/ansys/pyansys-geometry/actions/workflows/ci_cd.yml/badge.svg
    :target: https://github.com/ansys/pyansys-geometry/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
+   :target: https://opensource.org/blog/license/mit
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyansys-geometry/main.svg
@@ -151,14 +152,15 @@
 ^^^^^^^^^^^
 
 This code shows how to import PyAnsys Geometry and use some basic capabilities:
 
 .. code:: python
 
    from ansys.geometry.core import launch_modeler
+   from ansys.geometry.core.designer import DesignFileFormat
    from ansys.geometry.core.math import Plane, Point3D, Point2D
    from ansys.geometry.core.misc import UNITS, Distance
    from ansys.geometry.core.sketch import Sketch
 
    # Define a sketch
    origin = Point3D([0, 0, 10])
    plane = Plane(origin, direction_x=[1, 0, 0], direction_y=[0, 1, 0])
@@ -178,14 +180,17 @@
    body = design.extrude_sketch(
        name="CylinderBody", sketch=sketch, distance=Distance(80, unit=UNITS.m)
    )
 
    # Plot the body
    design.plot()
 
+   # Download the model
+   design.download(file_location="file.scdocx", format=DesignFileFormat.SCDOCX)
+
 For comprehensive usage information, see `Examples`_ in the `PyAnsys Geometry documentation`_.
 
 Documentation and issues
 ^^^^^^^^^^^^^^^^^^^^^^^^
 Documentation for the latest stable release of PyAnsys Geometry is hosted at `PyAnsys Geometry documentation`_.
 
 In the upper right corner of the documentation's title bar, there is an option for switching from
```

