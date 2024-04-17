# Comparing `tmp/manim_physics-0.3.0.tar.gz` & `tmp/manim_physics-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_physics-0.3.0.tar", max compression
+gzip compressed data, was "manim_physics-0.4.0.tar", max compression
```

## Comparing `manim_physics-0.3.0.tar` & `manim_physics-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      301 2023-06-12 03:32:54.254775 manim_physics-0.3.0/manim_physics/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 03:32:54.255761 manim_physics-0.3.0/manim_physics/electromagnetism/__init__.py
--rw-r--r--   0        0        0     4496 2023-06-12 03:32:54.256759 manim_physics-0.3.0/manim_physics/electromagnetism/electrostatics.py
--rw-r--r--   0        0        0     3043 2023-06-12 03:32:54.257756 manim_physics-0.3.0/manim_physics/electromagnetism/magnetostatics.py
--rw-r--r--   0        0        0      108 2023-06-12 03:32:54.258762 manim_physics-0.3.0/manim_physics/optics/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-12 03:32:54.259756 manim_physics-0.3.0/manim_physics/optics/lenses.py
--rw-r--r--   0        0        0     5026 2023-06-12 03:32:54.260751 manim_physics-0.3.0/manim_physics/optics/rays.py
--rw-r--r--   0        0        0        0 2023-06-12 03:32:54.260751 manim_physics-0.3.0/manim_physics/rigid_mechanics/__init__.py
--rw-r--r--   0        0        0     5267 2023-06-12 03:32:54.261771 manim_physics-0.3.0/manim_physics/rigid_mechanics/pendulum.py
--rw-r--r--   0        0        0     7977 2023-06-12 03:32:54.262758 manim_physics-0.3.0/manim_physics/rigid_mechanics/rigid_mechanics.py
--rw-r--r--   0        0        0     7381 2023-06-12 03:32:54.263759 manim_physics-0.3.0/manim_physics/wave.py
--rw-r--r--   0        0        0      760 2023-06-12 03:33:16.999818 manim_physics-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      711 2023-06-12 03:32:54.237754 manim_physics-0.3.0/README.md
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 manim_physics-0.3.0/setup.py
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 manim_physics-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      301 2024-04-11 15:06:41.506324 manim_physics-0.4.0/manim_physics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:06:41.507325 manim_physics-0.4.0/manim_physics/electromagnetism/__init__.py
+-rw-r--r--   0        0        0     4496 2024-04-11 15:06:41.507325 manim_physics-0.4.0/manim_physics/electromagnetism/electrostatics.py
+-rw-r--r--   0        0        0     3043 2024-04-11 15:06:41.508497 manim_physics-0.4.0/manim_physics/electromagnetism/magnetostatics.py
+-rw-r--r--   0        0        0      108 2024-04-11 15:06:41.509494 manim_physics-0.4.0/manim_physics/optics/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-11 15:06:41.510495 manim_physics-0.4.0/manim_physics/optics/lenses.py
+-rw-r--r--   0        0        0     5026 2024-04-11 15:06:41.510495 manim_physics-0.4.0/manim_physics/optics/rays.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:06:41.512495 manim_physics-0.4.0/manim_physics/rigid_mechanics/__init__.py
+-rw-r--r--   0        0        0     5267 2024-04-11 15:06:41.513496 manim_physics-0.4.0/manim_physics/rigid_mechanics/pendulum.py
+-rw-r--r--   0        0        0     7977 2024-04-11 15:06:41.513496 manim_physics-0.4.0/manim_physics/rigid_mechanics/rigid_mechanics.py
+-rw-r--r--   0        0        0     7381 2024-04-11 15:06:41.514496 manim_physics-0.4.0/manim_physics/wave.py
+-rw-r--r--   0        0        0      805 2024-04-17 16:29:46.729929 manim_physics-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      711 2024-04-11 15:06:41.491490 manim_physics-0.4.0/README.md
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 manim_physics-0.4.0/PKG-INFO
```

### Comparing `manim_physics-0.3.0/manim_physics/electromagnetism/electrostatics.py` & `manim_physics-0.4.0/manim_physics/electromagnetism/electrostatics.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/electromagnetism/magnetostatics.py` & `manim_physics-0.4.0/manim_physics/electromagnetism/magnetostatics.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/optics/lenses.py` & `manim_physics-0.4.0/manim_physics/optics/lenses.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/optics/rays.py` & `manim_physics-0.4.0/manim_physics/optics/rays.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/rigid_mechanics/pendulum.py` & `manim_physics-0.4.0/manim_physics/rigid_mechanics/pendulum.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/rigid_mechanics/rigid_mechanics.py` & `manim_physics-0.4.0/manim_physics/rigid_mechanics/rigid_mechanics.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/manim_physics/wave.py` & `manim_physics-0.4.0/manim_physics/wave.py`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/pyproject.toml` & `manim_physics-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "manim-physics"
-version = "0.3.0"
+version = "0.4.0"
 description = "Support physics simulation"
 authors = ["Matheart <waautomationwong@gmail.com>"]
 repository = "https://github.com/Matheart/manim-physics"
 readme="README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-manim = "^0.17.3"
-pymunk = "^6.0.0"
-Shapely = "^1.8.0"
+python = ">=3.9,<3.13"
+manim = "~0.18.0"
+pymunk = "^6.6.0"
+shapely = "^2.0.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-black = "^23.3.0"
-pre-commit = "^3.3.2"
-furo = "^2022.06.21"
-sphinx = "^4"
-sphinx-copybutton = "^0.4.0"
+pytest = "^7.4.3"
+black = ">=23.11,<25.0"
+pre-commit = "^3.5.0"
+furo = "^2023.09.10"
+Sphinx = "^7.2.6"
+sphinx-copybutton = "^0.5.2"
 sphinxcontrib-programoutput = "^0.17"
-myst-parser = "^0.17.2"
+myst-parser = "^2.0.0"
+matplotlib = "^3.8.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."manim.plugins"]
 "manim_physics" = "manim_physics"
```

### Comparing `manim_physics-0.3.0/README.md` & `manim_physics-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `manim_physics-0.3.0/PKG-INFO` & `manim_physics-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: manim-physics
-Version: 0.3.0
+Version: 0.4.0
 Summary: Support physics simulation
 Home-page: https://github.com/Matheart/manim-physics
 Author: Matheart
 Author-email: waautomationwong@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Shapely (>=1.8.0,<2.0.0)
-Requires-Dist: manim (>=0.17.3,<0.18.0)
-Requires-Dist: pymunk (>=6.0.0,<7.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: manim (>=0.18.0,<0.19.0)
+Requires-Dist: pymunk (>=6.6.0,<7.0.0)
+Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/Matheart/manim-physics
 Description-Content-Type: text/markdown
 
 # manim-physics 
 ## Introduction
 This is a 2D physics simulation plugin that allows you to generate complicated
 scenes in various branches of Physics such as rigid mechanics,
```

