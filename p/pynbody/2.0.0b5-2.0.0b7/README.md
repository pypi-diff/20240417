# Comparing `tmp/pynbody-2.0.0b5.tar.gz` & `tmp/pynbody-2.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynbody-2.0.0b5.tar", last modified: Sat Mar 16 14:52:24 2024, max compression
+gzip compressed data, was "pynbody-2.0.0b7.tar", last modified: Wed Apr 17 19:05:56 2024, max compression
```

## Comparing `pynbody-2.0.0b5.tar` & `pynbody-2.0.0b7.tar`

### file list

```diff
@@ -1,234 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.008578 pynbody-2.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-16 14:52:24.008578 pynbody-2.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.980578 pynbody-2.0.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/acknowledge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/pitfalls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.980578 pynbody-2.0.0b5/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/convenience.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/derived.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/essentials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/reference/plot.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.980578 pynbody-2.0.0b5/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/apigen.py
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/inheritance_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/ipython_console_highlighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/sphinxext/ipython_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.984578 pynbody-2.0.0b5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/bridge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/data_access.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.984578 pynbody-2.0.0b5/docs/tutorials/example_code/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/density_integrated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/density_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/do_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/do_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/do_pictures.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/do_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/do_preamble.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/rcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/rotcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/star_render.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/temperature_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/example_code/velocity_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/halos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/hmf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/pictures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/rotation_curve.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/snapshot_manipulation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/threads.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.988578 pynbody-2.0.0b5/pynbody/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/_util.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/CAMB_WMAP7
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/_com.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/_interpolate3d.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/angmom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/cambtemplate.ini
--rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/cmdlum.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/h1.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/halo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/hifrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/hmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/ionfrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/ionfracs.npz
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/pkdgrav_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/ramses_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/analysis/theoretical_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/array/
--rw-r--r--   0 runner    (1001) docker     (127)    29451 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/array/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/bc_modules/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/bc_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/bc_modules/capsulethunk.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/bridge/_bridge.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/chunk/
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/chunk/scan.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/dependencytracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/derived.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/extern/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/extern/_cython_fortran_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/extern/cython_fortran_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/family.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.992578 pynbody-2.0.0b5/pynbody/filt/
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/filt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/filt/geometry_selection.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.996578 pynbody-2.0.0b5/pynbody/gravity/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/_gravity.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/grav.c
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/ilc.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/ilp.h
--rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/kd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/main.c
--rw-r--r--   0 runner    (1001) docker     (127)    70165 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/moments.c
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/moments.h
--rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/serialtree.c
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/gravity/walk.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.996578 pynbody-2.0.0b5/pynbody/halo/
--rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/adaptahop.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/ahf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.000578 pynbody-2.0.0b5/pynbody/halo/details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/details/iord_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/details/number_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/details/particle_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/hbtplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/hop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/number_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/rockstar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/subfind.py
--rw-r--r--   0 runner    (1001) docker     (127)    25181 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/subfindhdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/subhalo_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/halo/velociraptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/iter_subclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.000578 pynbody-2.0.0b5/pynbody/kdtree/
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/kd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/kd.h
--rw-r--r--   0 runner    (1001) docker     (127)    21961 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/kdmain.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29947 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/smooth.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/kdtree/smooth.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.000578 pynbody-2.0.0b5/pynbody/openmp/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/openmp/openmp_null.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/openmp/openmp_real.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.000578 pynbody-2.0.0b5/pynbody/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19284 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/metals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/sph.py
--rw-r--r--   0 runner    (1001) docker     (127)    41579 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/stars.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/tollerud2008mw
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/plot/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/simdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.004578 pynbody-2.0.0b5/pynbody/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/copy_on_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    52745 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/gadget.py
--rw-r--r--   0 runner    (1001) docker     (127)    40970 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/gadgethdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/grafic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/namemapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/nchilada.py
--rw-r--r--   0 runner    (1001) docker     (127)    45792 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/ramses.py
--rw-r--r--   0 runner    (1001) docker     (127)    66474 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/simsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/subsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)    63862 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/tipsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/snapshot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.004578 pynbody-2.0.0b5/pynbody/sph/
--rw-r--r--   0 runner    (1001) docker     (127)    31333 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/sph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/sph/_render.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.004578 pynbody-2.0.0b5/pynbody/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/test_utils/gadget4_subfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/test_utils/pyread_gadget_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    24581 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    19033 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pynbody/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:23.988578 pynbody-2.0.0b5/pynbody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-16 14:52:23.000000 pynbody-2.0.0b5/pynbody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-16 14:52:23.000000 pynbody-2.0.0b5/pynbody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 14:52:23.000000 pynbody-2.0.0b5/pynbody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-16 14:52:23.000000 pynbody-2.0.0b5/pynbody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-16 14:52:23.000000 pynbody-2.0.0b5/pynbody.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 14:52:24.008578 pynbody-2.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:52:24.008578 pynbody-2.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/adaptahop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/ahf_halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/array_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/bridge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/copy_on_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/cosmology_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/derived_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/family_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/gadget_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/gadgethdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/grafic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/gravity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/halotools_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/hbtplus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/hop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/import_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/kdtree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/nchilada_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/partial_tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/performance_kdtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/ramses_new_ptcl_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/ramses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/rockstar_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/simsnap_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/sph_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/subarray_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/subfind_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/subfindhdf_gadget4_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/subfindhdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/swift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/theoretical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/transformation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-16 14:52:17.000000 pynbody-2.0.0b5/tests/velociraptor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/acknowledge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/pitfalls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/convenience.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/derived.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/essentials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/plot.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/apigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/inheritance_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/ipython_console_highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/ipython_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.361626 pynbody-2.0.0b7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/bridge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/data_access.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.361626 pynbody-2.0.0b7/docs/tutorials/example_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_integrated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_pictures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_preamble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/rcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/rotcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/star_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/temperature_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/velocity_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/halos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/hmf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/pictures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/rotation_curve.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/snapshot_manipulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.365626 pynbody-2.0.0b7/pynbody/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/CAMB_WMAP7
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/_com.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/_interpolate3d.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/angmom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cambtemplate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cmdlum.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/h1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/halo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/hifrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/hmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ionfrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ionfracs.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/pkdgrav_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ramses_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/theoretical_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/array/
+-rw-r--r--   0 runner    (1001) docker     (127)    29451 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/array/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/bc_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bc_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bc_modules/capsulethunk.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bridge/_bridge.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/chunk/
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/chunk/scan.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/dependencytracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/derived.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/_cython_fortran_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/cython_fortran_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/family.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.373626 pynbody-2.0.0b7/pynbody/filt/
+-rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/filt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/filt/geometry_selection.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.373626 pynbody-2.0.0b7/pynbody/gravity/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/_gravity.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/grav.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/ilc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/ilp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/kd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/main.c
+-rw-r--r--   0 runner    (1001) docker     (127)    70165 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/moments.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/moments.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/serialtree.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/walk.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/halo/
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/adaptahop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18094 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/ahf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/halo/details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/iord_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/number_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/particle_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/hbtplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/hop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/number_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/rockstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25211 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subfindhdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subhalo_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/velociraptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/iter_subclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/kdtree/
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kdmain.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/smooth.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28997 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/smooth.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/openmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/openmp/openmp_null.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/openmp/openmp_real.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19284 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/sph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41579 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/stars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/tollerud2008mw
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/simdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/copy_on_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52738 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41128 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/gadgethdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/grafic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/namemapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/nchilada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46971 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/ramses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68679 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/simsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/subsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63548 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/tipsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/sph/
+-rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/sph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/sph/_render.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/gadget4_subfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/pyread_gadget_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24581 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/_util.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/hdf_vds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.365626 pynbody-2.0.0b7/pynbody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/adaptahop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ahf_halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/array_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/bridge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/copy_on_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/cosmology_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/derived_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/family_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gadget_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gadgethdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/grafic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gravity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/halotools_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/hbtplus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/hop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/kdtree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/nchilada_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/partial_tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/performance_kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ramses_new_ptcl_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ramses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/rockstar_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/simsnap_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/sph_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subarray_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfind_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfindhdf_gadget4_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfindhdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/swift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/theoretical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19773 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/transformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/velociraptor_test.py
```

### Comparing `pynbody-2.0.0b5/PKG-INFO` & `pynbody-2.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b5
+Version: 2.0.0b7
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b5/README.md` & `pynbody-2.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/Makefile` & `pynbody-2.0.0b7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/bibliography.rst` & `pynbody-2.0.0b7/docs/bibliography.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/conf.py` & `pynbody-2.0.0b7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/index.rst` & `pynbody-2.0.0b7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/installation.rst` & `pynbody-2.0.0b7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/loaders.rst` & `pynbody-2.0.0b7/docs/loaders.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/pitfalls.rst` & `pynbody-2.0.0b7/docs/pitfalls.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/reference/analysis.rst` & `pynbody-2.0.0b7/docs/reference/analysis.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/reference/derived.rst` & `pynbody-2.0.0b7/docs/reference/derived.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/reference/index.rst` & `pynbody-2.0.0b7/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/apigen.py` & `pynbody-2.0.0b7/docs/sphinxext/apigen.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/docscrape.py` & `pynbody-2.0.0b7/docs/sphinxext/docscrape.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/docscrape_sphinx.py` & `pynbody-2.0.0b7/docs/sphinxext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/inheritance_diagram.py` & `pynbody-2.0.0b7/docs/sphinxext/inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/ipython_console_highlighting.py` & `pynbody-2.0.0b7/docs/sphinxext/ipython_console_highlighting.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/sphinxext/ipython_directive.py` & `pynbody-2.0.0b7/docs/sphinxext/ipython_directive.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/bridge.rst` & `pynbody-2.0.0b7/docs/tutorials/bridge.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/configuration.rst` & `pynbody-2.0.0b7/docs/tutorials/configuration.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/data_access.rst` & `pynbody-2.0.0b7/docs/tutorials/data_access.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/density_profile.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/density_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/do_data.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/do_data.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/do_images.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/do_images.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/do_pictures.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/do_pictures.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/do_plots.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/do_plots.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/do_preamble.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/do_preamble.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/rcs.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/rcs.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/rotcurve.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/rotcurve.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/example_code/velocity_vectors.py` & `pynbody-2.0.0b7/docs/tutorials/example_code/velocity_vectors.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/filters.rst` & `pynbody-2.0.0b7/docs/tutorials/filters.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/halos.rst` & `pynbody-2.0.0b7/docs/tutorials/halos.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/hmf.rst` & `pynbody-2.0.0b7/docs/tutorials/hmf.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/performance.rst` & `pynbody-2.0.0b7/docs/tutorials/performance.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/pictures.rst` & `pynbody-2.0.0b7/docs/tutorials/pictures.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/profile.rst` & `pynbody-2.0.0b7/docs/tutorials/profile.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/rotation_curve.rst` & `pynbody-2.0.0b7/docs/tutorials/rotation_curve.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/snapshot_manipulation.rst` & `pynbody-2.0.0b7/docs/tutorials/snapshot_manipulation.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/threads.rst` & `pynbody-2.0.0b7/docs/tutorials/threads.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/docs/tutorials/tutorials.rst` & `pynbody-2.0.0b7/docs/tutorials/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/__init__.py` & `pynbody-2.0.0b7/pynbody/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,10 +71,10 @@
 
 plot = PlotModuleProxy()
 
 from .snapshot import load, new
 
 derived_array = snapshot.simsnap.SimSnap.derived_quantity
 
-__version__ = '2.0.0-beta.5'
+__version__ = '2.0.0-beta.7'
 
 __all__ = ['load', 'new', 'derived_array']
```

### Comparing `pynbody-2.0.0b5/pynbody/_util.pyx` & `pynbody-2.0.0b7/pynbody/util/_util.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 cimport libc.math as cmath
 cimport numpy as np
 cimport openmp
 from cython.parallel cimport prange
 from libc.math cimport atan, pow
 from libc.stdlib cimport free, malloc
 
-from . import config
+from pynbody import config
 
 ctypedef fused fused_float:
     np.float32_t
     np.float64_t
 
 ctypedef fused fused_float_2:
     np.float32_t
@@ -116,18 +116,18 @@
     """Generate the x,y,z grid coordinates in the interval (0,1) for the
     specified indices (relative to the start of a GrafIC file) or slice of the
     file. nx,ny,nz are the number of particles in each dimension (presumably
     the same for all sane cases, but the file format allows for different
     values). If *pos* is not None, copy the results into the array; otherwise
     create a new array for the results and return it."""
 
-    from . import util
+    from . import indexing_length
 
     if pos is None:
-        pos = np.empty((util.indexing_length(indices_or_slice), 3),dtype=float)
+        pos = np.empty((indexing_length(indices_or_slice), 3),dtype=float)
 
     if isinstance(indices_or_slice, slice):
         _grid_gen_from_slice(indices_or_slice,nx,ny,nz,pos)
     else:
         _grid_gen_from_indices(np.asarray(indices_or_slice),nx,ny,nz,pos)
 
     return pos
```

### Comparing `pynbody-2.0.0b5/pynbody/analysis/CAMB_WMAP7` & `pynbody-2.0.0b7/pynbody/analysis/CAMB_WMAP7`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/_com.pyx` & `pynbody-2.0.0b7/pynbody/analysis/_com.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/_interpolate3d.pyx` & `pynbody-2.0.0b7/pynbody/analysis/_interpolate3d.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/angmom.py` & `pynbody-2.0.0b7/pynbody/analysis/angmom.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/cambtemplate.ini` & `pynbody-2.0.0b7/pynbody/analysis/cambtemplate.ini`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/cmdlum.npz` & `pynbody-2.0.0b7/pynbody/analysis/cmdlum.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/cosmology.py` & `pynbody-2.0.0b7/pynbody/analysis/cosmology.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/decomp.py` & `pynbody-2.0.0b7/pynbody/analysis/decomp.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/gravity.py` & `pynbody-2.0.0b7/pynbody/analysis/gravity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/h1.hdf5` & `pynbody-2.0.0b7/pynbody/analysis/h1.hdf5`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/halo.py` & `pynbody-2.0.0b7/pynbody/analysis/halo.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/hifrac.py` & `pynbody-2.0.0b7/pynbody/analysis/hifrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/hmf.py` & `pynbody-2.0.0b7/pynbody/analysis/hmf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/interpolate.py` & `pynbody-2.0.0b7/pynbody/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/ionfrac.py` & `pynbody-2.0.0b7/pynbody/analysis/ionfrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/ionfracs.npz` & `pynbody-2.0.0b7/pynbody/analysis/ionfracs.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/luminosity.py` & `pynbody-2.0.0b7/pynbody/analysis/luminosity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/pkdgrav_cosmo.py` & `pynbody-2.0.0b7/pynbody/analysis/pkdgrav_cosmo.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/profile.py` & `pynbody-2.0.0b7/pynbody/analysis/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/ramses_util.py` & `pynbody-2.0.0b7/pynbody/analysis/ramses_util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/analysis/theoretical_profiles.py` & `pynbody-2.0.0b7/pynbody/analysis/theoretical_profiles.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/array/__init__.py` & `pynbody-2.0.0b7/pynbody/array/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/bc_modules/capsulethunk.h` & `pynbody-2.0.0b7/pynbody/bc_modules/capsulethunk.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/bridge/__init__.py` & `pynbody-2.0.0b7/pynbody/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/bridge/_bridge.pyx` & `pynbody-2.0.0b7/pynbody/bridge/_bridge.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/chunk/__init__.py` & `pynbody-2.0.0b7/pynbody/chunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/chunk/scan.pyx` & `pynbody-2.0.0b7/pynbody/chunk/scan.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/configuration.py` & `pynbody-2.0.0b7/pynbody/configuration.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/default_config.ini` & `pynbody-2.0.0b7/pynbody/default_config.ini`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,17 @@
 birth_time: tform
 
 # map the names in the XXXX_file_descriptor.txt to pynbody names
 density: rho
 pressure: p
 metallicity: metal
 
+# for some reason sink particle masses are sometimes labelled msink
+msink: mass
+
 
 [ramses]
 # For RAMSES format post November 2017: map the raw particle family ID to the pynbody family type
 
 # families >0 in ascending order (1, 2,..)
 # the last family in the list is also assigned to all other positive families
 type-mapping-positive: dm, star, cloud, debris
```

### Comparing `pynbody-2.0.0b5/pynbody/dependencytracker.py` & `pynbody-2.0.0b7/pynbody/dependencytracker.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/derived.py` & `pynbody-2.0.0b7/pynbody/derived.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     self.kdtree.set_array_ref('rho', self['rho'])
     self.kdtree.set_array_ref('smooth', self['smooth'])
     self.kdtree.set_array_ref('mass', self['mass'])
     self.kdtree.set_array_ref('qty', self['vel'])
     self.kdtree.set_array_ref('qty_sm', sm)
 
     start = time.time()
-    self.kdtree.populate('qty_%s' % op, nsmooth, config['sph']['Kernel'])
+    self.kdtree.populate('qty_%s' % op, nsmooth)
     end = time.time()
 
     logger.info(f'{_op_dict[op]} done in {end - start:5.3g} s')
 
     return sm
```

### Comparing `pynbody-2.0.0b5/pynbody/extern/_cython_fortran_utils.pyx` & `pynbody-2.0.0b7/pynbody/extern/_cython_fortran_utils.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/family.py` & `pynbody-2.0.0b7/pynbody/family.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/filt/__init__.py` & `pynbody-2.0.0b7/pynbody/filt/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/filt/geometry_selection.pyx` & `pynbody-2.0.0b7/pynbody/filt/geometry_selection.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/_gravity.pyx` & `pynbody-2.0.0b7/pynbody/gravity/_gravity.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/calc.py` & `pynbody-2.0.0b7/pynbody/gravity/calc.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/config.h` & `pynbody-2.0.0b7/pynbody/gravity/config.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/grav.c` & `pynbody-2.0.0b7/pynbody/gravity/grav.c`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/ilc.h` & `pynbody-2.0.0b7/pynbody/gravity/ilc.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/ilp.h` & `pynbody-2.0.0b7/pynbody/gravity/ilp.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/kd.h` & `pynbody-2.0.0b7/pynbody/gravity/kd.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/main.c` & `pynbody-2.0.0b7/pynbody/gravity/main.c`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/moments.c` & `pynbody-2.0.0b7/pynbody/gravity/moments.c`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/moments.h` & `pynbody-2.0.0b7/pynbody/gravity/moments.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/serialtree.c` & `pynbody-2.0.0b7/pynbody/gravity/serialtree.c`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/tree.py` & `pynbody-2.0.0b7/pynbody/gravity/tree.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/gravity/walk.c` & `pynbody-2.0.0b7/pynbody/gravity/walk.c`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/__init__.py` & `pynbody-2.0.0b7/pynbody/halo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import warnings
 import weakref
 from typing import TYPE_CHECKING, Iterable
 
 import numpy as np
 from numpy.typing import NDArray
 
-from .. import iter_subclasses, snapshot, util
+from .. import iter_subclasses, snapshot, units, util
 from .details.iord_mapping import make_iord_to_offset_mapper
 from .details.number_mapping import MonotonicHaloNumberMapper, create_halo_number_mapper
 from .details.particle_indices import HaloParticleIndices
 
 if TYPE_CHECKING:
     from .subhalo_catalogue import SubhaloCatalogue
 
@@ -144,23 +144,27 @@
     _init_iord_to_fpos, which creates a mapper as _iord_to_fpos. See details/iord_mapping.py for more information.
     """
 
     def __init__(self, sim, number_mapper):
         self._base: weakref[snapshot.SimSnap] = weakref.ref(sim)
         self.number_mapper: MonotonicHaloNumberMapper = number_mapper
         self._index_lists: HaloParticleIndices | None = None
+        self._properties: dict | None = None
         self._cached_halos: dict[int, Halo] = {}
 
     def load_all(self):
         """Loads all halos, which is normally more efficient if a large fraction of them will be accessed."""
         if not self._index_lists:
             index_lists = self._get_all_particle_indices()
+            properties = self.get_properties_all_halos(with_units=True)
             if isinstance(index_lists, tuple):
                 index_lists = HaloParticleIndices(*index_lists)
             self._index_lists = index_lists
+            if len(properties)>0:
+                self._properties = properties
 
     @util.deprecated("precalculate has been renamed to load_all")
     def precalculate(self):
         self.load_all()
 
     def _get_num_halos(self):
         return len(self.number_mapper)
@@ -199,35 +203,43 @@
 
         A generic implementation is provided that fetches index lists for all halos and then extracts the one"""
         self.load_all()
         return self._index_lists.get_particle_index_list_for_halo(
             self.number_mapper.number_to_index(halo_number)
         )
 
-    def _get_particle_indices_one_halo_using_list_if_available(self, halo_number) -> NDArray[int]:
+    def _get_particle_indices_one_halo_using_list_if_available(self, halo_number, halo_index) -> NDArray[int]:
         if self._index_lists:
-            return self._index_lists.get_particle_index_list_for_halo(
-                self.number_mapper.number_to_index(halo_number)
-            )
+            return self._index_lists.get_particle_index_list_for_halo(halo_index)
         else:
             if len(self._cached_halos) == 5:
                 warnings.warn("Accessing multiple halos may be more efficient if you call load_all() on the "
                               "halo catalogue", RuntimeWarning)
             return self._get_particle_indices_one_halo(halo_number)
             # NB subclasses may implement loading one halo direct from disk in the above
             # if not, the default implementation will populate _cached_index_lists
 
     def _get_halo_cached(self, halo_number) -> Halo:
         if halo_number not in self._cached_halos:
             self._cached_halos[halo_number] = self._get_halo(halo_number)
         return self._cached_halos[halo_number]
 
+    def _get_properties_one_halo_using_cache_if_available(self, halo_number, halo_index):
+        if self._properties is None:
+            return self.get_properties_one_halo(halo_number)
+        else:
+            return {k: units.get_item_with_unit(self._properties[k],halo_index)
+                    for k in self._properties}
+
     def _get_halo(self, halo_number) -> Halo:
-        return Halo(halo_number, self.get_properties_one_halo(halo_number), self, self.base,
-                    self._get_particle_indices_one_halo_using_list_if_available(halo_number))
+        halo_index = self.number_mapper.number_to_index(halo_number)
+        return Halo(halo_number,
+                    self._get_properties_one_halo_using_cache_if_available(halo_number, halo_index),
+                    self, self.base,
+                    self._get_particle_indices_one_halo_using_list_if_available(halo_number, halo_index))
 
     def get_dummy_halo(self, halo_number) -> DummyHalo:
         """Return a DummyHalo object containing only the halo properties, no particle information"""
         h = DummyHalo()
         h.properties.update(self.get_properties_one_halo(halo_number))
         return h
 
@@ -297,15 +309,17 @@
             return number_per_particle
 
     def load_copy(self, halo_number):
         """Load a fresh SimSnap with only the particles in specified halo
 
         This relies on the underlying SimSnap being capable of partial loading."""
         from .. import load
-        return load(self.base.filename, take=self._get_particle_indices_one_halo_using_list_if_available(halo_number))
+        halo_index = self.number_mapper.number_to_index(halo_number)
+        return load(self.base.filename,
+                    take=self._get_particle_indices_one_halo_using_list_if_available(halo_number, halo_index))
 
     def physical_units(self, distance='kpc', velocity='km s^-1', mass='Msol', persistent=True, convert_parent=False):
         """
         Converts all array's units to be consistent with the
         distance, velocity, mass basis units specified.
 
         Base units can be specified using keywords.
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/adaptahop.py` & `pynbody-2.0.0b7/pynbody/halo/adaptahop.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,17 @@
 
         # Initialize internal data
         self._base_dm = sim.dm
         self._iord_to_fpos = iord_mapping.make_iord_to_offset_mapper(self._base_dm["iord"])
 
         # dm needs to be at start of family map -- technically we will assume all particles are in dm
         # but then the parent class will use the position offsets as though they refer to the whole file
-        assert self.base._get_family_slice('dm') == slice(0, len(self._base_dm))
+        dm_offset = self.base._get_family_slice('dm').start
+        if dm_offset>0:
+            self._iord_to_fpos = iord_mapping.IordOffsetModifier(self._iord_to_fpos, dm_offset)
 
         self._halos = {}
 
         self._AdaptaHOP_fname = fname
 
 
         logger.debug("AdaptaHOPCatalogue loaded")
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/ahf.py` & `pynbody-2.0.0b7/pynbody/halo/ahf.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
         if halo_numbers == 'v1':
             number_mapper = SimpleHaloNumberMapper(1, self._num_halos)
         elif halo_numbers == 'file-order':
             number_mapper = SimpleHaloNumberMapper(0, self._num_halos)
         elif halo_numbers == 'length-order' or halo_numbers == 'length-order-v1':
             npart = self._halo_properties['npart']
-            osort = np.argsort(-npart)  # this is better than argsort(npart)[::-1], because it's stable
+            osort = np.argsort(-npart, kind='stable')  # this is better than argsort(npart)[::-1], because it's stable
             if halo_numbers.endswith('v1'):
                 number_mapper = NonMonotonicHaloNumberMapper(osort, ordering=True, start_index=1)
             else:
                 number_mapper = NonMonotonicHaloNumberMapper(osort, ordering=True, start_index=0)
         elif halo_numbers == 'ahf':
             number_mapper = self._ahf_own_number_mapper
         else:
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/details/iord_mapping.py` & `pynbody-2.0.0b7/pynbody/halo/details/iord_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 
 import numpy as np
 
-from pynbody._util import binary_search, is_sorted
+from pynbody.util import binary_search, is_sorted
 
 
 class IordToOffset(abc.ABC):
     @abc.abstractmethod
     def map_ignoring_order(self, i: np.ndarray | int) -> np.ndarray | int:
         """Given an array of iord values, return the corresponding fpos values.
 
@@ -51,14 +51,28 @@
         result = binary_search(np.asarray(iord_values), self._iord, self._iord_argsort)
 
         if singleton:
             return result[0]
         else:
             return result
 
+class IordOffsetModifier(IordToOffset):
+    """A wrapper around an IordToOffset which adds a constant offset to the result of the underlying mapping.
+
+    Useful if the iord values e.g. are only available for a single family; then the fpos_offset will correspond
+    to the first index of that family in the pynbody snapshot.
+    """
+    def __init__(self, iord_to_offset: IordToOffset, fpos_offset: int):
+        self._underlying = iord_to_offset
+        self._fpos_offset = fpos_offset
+
+    def map_ignoring_order(self, i: np.ndarray | int) -> np.ndarray | int:
+        result = self._underlying.map_ignoring_order(i)
+        result += self._fpos_offset
+        return result
 
 def make_iord_to_offset_mapper(iord: np.ndarray) -> IordToOffset:
     """Given an array of unique integers, iord, make an object which maps from an iord value to offset in the array.
 
     i.e. given an iord array and a subset of values my_iord_values,
 
      make_iord_to_offset_mapper(iord).map_ignoring_order(my_iord_values)
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/details/number_mapping.py` & `pynbody-2.0.0b7/pynbody/halo/details/number_mapping.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/details/particle_indices.py` & `pynbody-2.0.0b7/pynbody/halo/details/particle_indices.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/hbtplus.py` & `pynbody-2.0.0b7/pynbody/halo/hbtplus.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,22 +30,28 @@
         if hbt_filename is None:
             hbt_filename = self._infer_hbt_filename(sim)
 
         self._file = h5py.File(hbt_filename, 'r')
 
         num_halos = int(self._file["NumberOfSubhalosInAllFiles"][0])
         if int(self._file["NumberOfFiles"][0])>1:
-            raise ValueError("HBTPlusCatalogue does not support multi-file catalogues")
+            from ..util import hdf_vds
+            hbt_filename = str(hbt_filename)[:-7]
+            all_files = [f"{hbt_filename}.{num}.hdf5" for num in range(int(self._file["NumberOfFiles"][0]))]
+            maker = hdf_vds.HdfVdsMaker(all_files)
+            self._file = maker.get_temporary_hdf_vfile()
+
+        self._trackid_number_mapper = number_mapping.create_halo_number_mapper(self._file["Subhalos"]["TrackId"])
 
         if halo_numbers is None:
             number_mapper = number_mapping.SimpleHaloNumberMapper(0, num_halos)
         elif halo_numbers == 'track':
-            number_mapper = number_mapping.create_halo_number_mapper(self._file["Subhalos"]["TrackId"])
+            number_mapper = self._trackid_number_mapper
         elif halo_numbers == 'length-order':
-            osort = np.argsort(-self._file["Subhalos"]["Nbound"][:])
+            osort = np.argsort(-self._file["Subhalos"]["Nbound"][:], kind='stable')
             number_mapper = number_mapping.NonMonotonicHaloNumberMapper(osort, ordering=True, start_index=0)
         else:
             raise ValueError(f"Invalid value for halo_numbers: {halo_numbers}")
         super().__init__(sim, number_mapper)
 
         self._setup_parents()
 
@@ -67,24 +73,45 @@
 
         for candidate_path in candidate_paths:
             if candidate_path.exists():
                 return candidate_path
 
         raise FileNotFoundError(f'Could not find HBTPlus catalogue for {sim_filename}. Try passing hbt_filename explicitly.')
 
+    @classmethod
+    def _map_user_filename_to_file_0(cls, filename):
+        filename = pathlib.Path(filename)
+        if not filename.exists():
+            dot_hdf5 = filename.parent / (filename.name + '.hdf5')
+            dot_0_hdf5 = filename.parent / (filename.name + '.0.hdf5')
+            if dot_hdf5.exists():
+                filename = dot_hdf5
+            elif dot_0_hdf5.exists():
+                filename = dot_0_hdf5
+        return filename
 
     def _setup_parents(self):
         parents = np.empty(len(self), dtype=np.intp)
         parents.fill(-1)
         for i in range(len(self)):
-            for child in self._file["NestedSubhalos"][i]:
+            for child in self._trackid_number_mapper.number_to_index(self._file["NestedSubhalos"][i]):
                 parents[child] = self.number_mapper.index_to_number(i)
 
         self._parents = parents
 
+    def _map_trackid_to_pynbody_number(self, trackid: NDArray[int]) -> NDArray[int]:
+        if self.number_mapper is self._trackid_number_mapper:
+            return trackid
+        else:
+            return self.number_mapper.index_to_number(
+                self._trackid_number_mapper.number_to_index(
+                  trackid
+                )
+            )
+
     def _get_particle_indices_one_halo(self, halo_number) -> NDArray[int]:
         self._init_iord_to_fpos()
 
         iords = self._file["SubhaloParticles"][self.number_mapper.number_to_index(halo_number)]
         return np.sort(self._iord_to_fpos.map_ignoring_order(iords))
 
     def _get_all_particle_indices(self) -> HaloParticleIndices | tuple[np.ndarray, np.ndarray]:
@@ -129,15 +156,15 @@
         for k in self._file["Subhalos"].dtype.names:
             result[k] = np.asarray(self._file["Subhalos"][k])
         result['children'] = [self._get_children_one_halo(i) for i in range(len(self))]
         result['parent'] = self._parents
         return result
 
     def _get_children_one_halo(self, index) -> NDArray[int]:
-        return self.number_mapper.index_to_number(self._file["NestedSubhalos"][index])
+        return self._map_trackid_to_pynbody_number(self._file["NestedSubhalos"][index])
 
 
 
     @classmethod
     def _can_load(cls, sim, halo_numbers=None, hbt_filename=None):
         try:
             hbt_filename = hbt_filename or cls._infer_hbt_filename(sim)
@@ -161,16 +188,16 @@
 
         self._hbt_cat = hbt_cat
         self._group_cat = group_cat
         self._hbt_host_groups = np.asarray(hbt_cat._file["Subhalos"]["HostHaloId"])
         if self._hbt_host_groups.max() >= len(group_cat):
             raise ValueError("The HBT+ catalogue contains host groups that are not in the group catalogue")
         self._children = [[] for _ in range(len(group_cat))]
-        for p in range(len(hbt_cat)):
-            self._children[self._hbt_host_groups[p]].append(p)
+        for hbt_index, hbt_number in enumerate(hbt_cat.number_mapper):
+            self._children[self._hbt_host_groups[hbt_index]].append(hbt_number)
         self._children = [np.array(c) for c in self._children]
 
         super().__init__(group_cat.base, group_cat.number_mapper)
 
     def load_all(self):
         self._hbt_cat.load_all()
         self._group_cat.load_all()
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/hop.py` & `pynbody-2.0.0b7/pynbody/halo/hop.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/number_array.py` & `pynbody-2.0.0b7/pynbody/halo/number_array.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/rockstar.py` & `pynbody-2.0.0b7/pynbody/halo/rockstar.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/subfind.py` & `pynbody-2.0.0b7/pynbody/halo/subfind.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/subfindhdf.py` & `pynbody-2.0.0b7/pynbody/halo/subfindhdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
         if not subs:
             self._subhalo_catalogue = type(self)(sim, subs=True, _inherit_data_from=self)
 
     def __inherit_data(self, parent):
         attrs_to_share = ["_fof_properties", "_sub_properties", "_fof_group_offsets", "_fof_group_lengths",
                          "_subfind_halo_offsets", "_subfind_halo_lengths",
-                          "fof_ignore", "sub_ignore"]
+                          "fof_ignore", "sub_ignore","_subfind_halo_parent_groups"]
         for attr in attrs_to_share:
             setattr(self, attr, getattr(parent, attr))
 
 
     def _get_catalogue_multifile(self, sim):
         """Some variants of Subfind put all the particle data in the catalogue files, in which case the catalogue
         HDF files are already present in the base simulation. In other cases, notably Gadget4/Arepo, this must be
```

### Comparing `pynbody-2.0.0b5/pynbody/halo/subhalo_catalogue.py` & `pynbody-2.0.0b7/pynbody/halo/subhalo_catalogue.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/halo/velociraptor.py` & `pynbody-2.0.0b7/pynbody/halo/velociraptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,35 +69,35 @@
         else:
             self._path = Path(vr_basename)
 
         if self._path is None:
             raise OSError("Could not find velociraptor catalogue. Try specifying vr_basename='path/to/output', where the velociraptor outputs are output.properties.0 etc")
         self._grps = h5py.File(str(self._path.with_suffix('.catalog_groups.0')), 'r')
         self._part_ids = h5py.File(str(self._path.with_suffix('.catalog_particles.0')), 'r')
-        self._properties = h5py.File(str(self._path.with_suffix('.properties.0')), 'r')
+        self._properties_hdf_file = h5py.File(str(self._path.with_suffix('.properties.0')), 'r')
 
         if include_unbound:
             self._part_ids_unbound = h5py.File(str(self._path.with_suffix('.catalog_particles.unbound.0')), 'r')
         self._props = h5py.File(str(self._path.with_suffix('.properties.0')), 'r')
 
         assert self._grps['Num_of_files'][0] == 1, "Multi-file catalogues not supported at present"
 
         self._num_halos = self._grps['Num_of_groups'][0]
 
-        super().__init__(sim, number_mapping.create_halo_number_mapper(self._properties['ID']))
+        super().__init__(sim, number_mapping.create_halo_number_mapper(self._properties_hdf_file['ID']))
 
         self._setup_property_keys()
         self._setup_property_units()
         self._init_iord_to_fpos()
         self._calculate_children()
 
     def _setup_property_keys(self):
         self._property_keys = []
-        for k in self._properties.keys():
-            if len(self._properties[k]) == self._num_halos:
+        for k in self._properties_hdf_file.keys():
+            if len(self._properties_hdf_file[k]) == self._num_halos:
                 self._property_keys.append(k)
 
     def _setup_property_units(self):
         unitinfo = self._props['UnitInfo'].attrs
         comoving = int(unitinfo['Comoving_or_Physical'])!=0
         length = units.Unit("kpc")*float(unitinfo['Length_unit_to_kpc'])
         if comoving:
@@ -146,25 +146,25 @@
         parent = self._parents[i_zerobased]
         children = self._all_children_ordered_by_parent[self._children_start_index[i_zerobased]:self._children_stop_index[i_zerobased]]
         properties.update({'parent': parent, 'children': children})
         return properties
 
     def get_properties_all_halos(self, with_units=True) -> dict:
         if with_units:
-            all_properties = {k: array.SimArray(self._properties[k][:], u)
+            all_properties_hdf_file = {k: array.SimArray(self._properties_hdf_file[k][:], u)
                               for k, u in zip(self._property_keys, self._property_units)}
         else:
-            all_properties = {k: self._properties[k] for k in self._property_keys}
+            all_properties_hdf_file = {k: self._properties_hdf_file[k] for k in self._property_keys}
 
-        all_properties.update(
+        all_properties_hdf_file.update(
                {'parent': self._parents,
                 'children': [self._all_children_ordered_by_parent[start:end]
                              for start, end in zip(self._children_start_index, self._children_stop_index)]}
         )
-        return all_properties
+        return all_properties_hdf_file
 
 
     def _get_particle_indices_one_halo(self, halo_number) -> NDArray[int]:
         i_zerobased = self.number_mapper.number_to_index(halo_number)
         ptcl_fpos = self.__get_particle_indices_from_halo_index(i_zerobased, False)
 
         if self._include_unbound:
```

### Comparing `pynbody-2.0.0b5/pynbody/iter_subclasses.py` & `pynbody-2.0.0b7/pynbody/iter_subclasses.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/kdtree/__init__.py` & `pynbody-2.0.0b7/pynbody/kdtree/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """
-
-KDTree
-======
-
-Provides access to nearest neighbour lists and smoothing lengths.
+Efficient 3D KDTree implementation for fast geometrical calculations such as neighbour lists and smoothing lengths.
 
 """
 import logging
 import time
 import warnings
 
 import numpy as np
@@ -31,38 +27,64 @@
     ('pLower', np.intp),
     ('pUpper', np.intp)
 ])
 
 class KDTree:
     """KDTree can be used for smoothing, interpolating and geometrical queries.
 
-    Most users are unlikely to interact with the KDTree directly, instead using the higher-level
-    SPH functionality. To accelerate geometrical queries on a snapshot, try:
+
+    You are unlikely to need to interact with the KDTree directly, instead using the higher-level
+    SPH functionality such as
+
+    >>> f = pynbody.load("my_snapshot")
+    >>> f.gas['smooth'] # will build KDTree and calculate smoothing lengths for gas, if not available on disk
+    >>> f.gas['rho'] # will calculate densities for gas, if not available on disk
+    >>> f.dm['rho'] # will calculate densities for dark matter, if not available on disk
+
+    KDTree can also be used to accelerate geometrical queries on a snapshot, e.g.:
 
     >>> f = pynbody.load('my_snapshot')
     >>> f.build_kdtree()
-    >>> f[pynbody.filt.Sphere('10 kpc')] # this will automatically be a faster operation once the tree is built
+    >>> f[pynbody.filt.Sphere('10 kpc')]
 
-    Performance statistics can be tested using the performance_kdtree.py script in the tests folder
+    See :ref:`performance of filters <filters_tutorial_performance_implications>` for more information.
 
     Most KDTree operations proceed in parallel, using the number of threads specified in the
     pynbody configuration.
+
+    Performance statistics can be tested using the ``performance_kdtree.py`` script in the tests folder.
+
+    Note that the KDTree takes into account periodicity of cosmological volumes if it can. However, as soon as a
+    snapshot has been rotated, this may become impossible. In this case, the KDTree will issue a warning,
+    and will not use periodicity. This is to avoid incorrect results due to the periodicity assumption,
+    but it will lead to artefacts on the edge of the box. If you are working with a cosmological simulation,
+    it is best to perform any KDTree operations (such as smoothing) before rotating the snapshot, e.g.:
+
+    >>> f = pynbody.load('my_snapshot')
+    >>> f['rho']; f['smooth'] # force KDTree to be built and density estimations made
+    >>> pynbody.analysis.faceon(f) # rotate the snapshot
+    >>> pynbody.plot.image(f.g, qty='rho', width='10 kpc')
+
     """
 
     PROPID_HSM = 1
     PROPID_RHO = 2
     PROPID_QTYMEAN_1D = 3
     PROPID_QTYMEAN_ND = 4
     PROPID_QTYDISP_1D = 5
     PROPID_QTYDISP_ND = 6
     PROPID_QTYDIV  = 7
     PROPID_QTYCURL = 8
 
     def __init__(self, pos, mass, leafsize=32, boxsize=None, num_threads=None, shared_mem=False):
-        """
+        """Create a KDTree
+
+        Most users will not need to call this directly, but will instead use the higher-level functions, either
+        via accessing SPH properties on a snapshot, or calling :meth:`pynbody.snapshot.simsnap.SimSnap.build_tree`.
+
         Parameters
         ----------
         pos : pynbody.array.SimArray
             Particles positions.
         mass : pynbody.array.SimArray
             Particles mass.
         leafsize : int, optional
@@ -83,113 +105,120 @@
         num_threads_init = 2 ** int(np.log2(num_threads))
 
 
         self.leafsize = int(leafsize)
         self.kdtree = kdmain.init(pos, mass, self.leafsize)
         nodes = kdmain.get_node_count(self.kdtree)
 
+        # zeroing the KDNode elements below isn't strictly necessary but helps with testing/debugging since some
+        # of the memory won't be used
+
         if shared_mem:
             from ..array import shared
-            self.kdnodes = shared.make_shared_array(nodes, KDNode)
+            self.kdnodes = shared.make_shared_array(nodes, KDNode, zeros=True)
             self.particle_offsets = shared.make_shared_array(len(pos), np.intp)
         else:
-            self.kdnodes = np.empty(nodes, dtype=KDNode)
+            self.kdnodes = np.zeros(nodes, dtype=KDNode)
             self.particle_offsets = np.empty(len(pos), dtype=np.intp)
+
         kdmain.build(self.kdtree, self.kdnodes, self.particle_offsets, num_threads_init)
 
         self.boxsize = boxsize
         self._pos = pos
+        self.set_kernel(config['sph'].get('Kernel', 'CubicSpline'))
 
     def _set_num_threads(self, num_threads):
         if num_threads is None:
             num_threads = int(config["number_of_threads"])
         self.num_threads = num_threads
         return num_threads
 
     def serialize(self):
-        return self.leafsize, self.boxsize, self.kdnodes, self.particle_offsets
+        """Produce a serialized description of the tree"""
+        return self.leafsize, self.boxsize, self.kdnodes, self.particle_offsets, self._kernel_id
 
     @classmethod
     def deserialize(cls, pos, mass, serialized_state, num_threads = None, boxsize=None):
+        """Reconstruct a KDTree from a serialized state."""
         self = object.__new__(cls)
         self._set_num_threads(num_threads)
-        leafsize, boxsize_s, kdnodes, particle_offsets = serialized_state
+        leafsize, boxsize_s, kdnodes, particle_offsets, kernel_id = serialized_state
         if boxsize is not None and abs(boxsize-boxsize_s) > 1e-6:
             warnings.warn("Boxsize in serialized state does not match boxsize passed to deserialize")
         self.kdtree = kdmain.init(pos, mass, leafsize)
         self.leafsize = leafsize
         nodes = kdmain.get_node_count(self.kdtree)
         if len(kdnodes) != nodes:
             raise ValueError("Number of nodes in serialized state does not match number of nodes in kdtree")
         self.kdnodes = kdnodes
         if len(particle_offsets) != len(pos):
             raise ValueError("Number of particle offsets in serialized state does not match number of particles")
         self.particle_offsets = particle_offsets
         self.boxsize = boxsize
         self._pos = pos
+        self._kernel_id = kernel_id
 
         kdmain.import_prebuilt(self.kdtree, self.kdnodes, self.particle_offsets, 0)
 
         return self
 
 
 
     def particles_in_sphere(self, center, radius):
         """Find particles within a sphere.
 
+        Most users will not need to call this directly, but will instead use :class:`pynbody.filt.Sphere`.
+
         Parameters
         ----------
         center : array_like
             Center of the sphere.
         radius : float
             Radius of the sphere.
 
         Returns
         -------
         indices : array_like
             Indices of the particles within the sphere.
         """
-        smx = kdmain.nn_start(self.kdtree, 1, 1, self.boxsize)
+        smx = kdmain.nn_start(self.kdtree, 1, self.boxsize)
 
         particle_ids = kdmain.particles_in_sphere(self.kdtree, smx, center[0], center[1], center[2], radius)
 
         kdmain.nn_stop(self.kdtree, smx)
         return particle_ids
 
     def nn(self, nn=None):
         """Generator of neighbour list.
 
-        This method provides an interface to the neighbours search of the C-extension kdmain.
-
         Parameters
         ----------
         nn : int, None
             number of neighbours. If None, default to 64.
 
         Yields
         ------
         nbr_list : list[int, float, list[int], list[float]]
+
             Information about the neighbours of a particle.
+
             List with four elements:
-                nbr_list[0] : int
-                    the index of the particle in the snapshot's arrays.
-                nbr_list[1] : float
-                    the smoothing length of the particle (i.e. nbr_list[1] == snap['smooth'][nbr_list[0]]).
-                nbr_list[2] : list[int]
-                    list of the indexes of the `nn` neighbouring particles.
-                nbr_list[3] : list[float]
-                    list of distances squared of each neighbouring particles.
+
+            * ``nbr_list[0]`` (``int``): the index of the particle in the snapshot's arrays.
+            * ``nbr_list[1]`` (``float``): the smoothing length of the particle
+            * ``nbr_list[2]`` (``list[int]``): list of the indexes of the `nn` neighbouring particles.
+            * ``nbr_list[3]`` (``list[float]``): list of distances squared of each neighbouring particles.
 
             The lists of particle and of the relative distance squared are not sorted.
 
         """
         if nn is None:
             nn = 64
 
-        smx = kdmain.nn_start(self.kdtree, int(nn), 1, self.boxsize)
+        smx = kdmain.nn_start(self.kdtree, int(nn), self.boxsize)
         kdmain.domain_decomposition(self.kdtree, 1)
 
         while True:
             nbr_list = kdmain.nn_next(self.kdtree, smx)
             if nbr_list is None:
                 break
             yield nbr_list
@@ -198,41 +227,68 @@
 
     def all_nn(self, nn=None):
         """A list of neighbours information for all the particles in the snapshot."""
         return [x for x in self.nn(nn)]
 
     @staticmethod
     def array_name_to_id(name):
+        """Convert the pynbody name of an array to the corresponding integer ID in the C++ code."""
         if name == "smooth":
             return 0
         elif name == "rho":
             return 1
         elif name == "mass":
             return 2
         elif name == "qty":
             return 3
         elif name == "qty_sm":
             return 4
         else:
             raise ValueError("Unknown KDTree array")
 
     def set_array_ref(self, name, ar):
+        """Give the C++ code access to a given array.
+
+        Parameters
+        ----------
+
+        name : str
+            Name of the array to set (can be 'smooth', 'rho', 'mass', 'qty', 'qty_sm')
+        ar : pynbody.array.SimArray
+            Array that the C++ code will access. Note that INCREF is called on the array, so it will be kept
+            alive as long as the KDTree object is alive (or until another set_array_ref call replaces it.)
+        """
+
         if self.array_name_to_id(name) < 3:
             if not np.issubdtype(self._pos.dtype, ar.dtype):
                 raise TypeError(
                     "KDTree requires matching dtypes for %s (%s) and pos (%s) arrays"
                     % (name, ar.dtype, self._pos.dtype)
                 )
         kdmain.set_arrayref(self.kdtree, self.array_name_to_id(name), ar)
         assert self.get_array_ref(name) is ar
 
     def get_array_ref(self, name):
+        """Get the current array reference for a given name ('smooth', 'rho', 'mass', 'qty', or 'qty_sm')."""
         return kdmain.get_arrayref(self.kdtree, self.array_name_to_id(name))
 
     def smooth_operation_to_id(self, name):
+        """Convert the name of a smoothing operation to the corresponding integer ID in the C++ code.
+
+        Valid names are:
+
+        * 'hsm' : compute smoothing lengths
+        * 'rho' : compute density
+        * 'qty_mean' : compute SPH mean of the 'qty' array
+        * 'qty_disp' : compute SPH dispersion of the 'qty' array
+        * 'qty_div' : compute divergence of the 'qty' array
+        * 'qty_curl' : compute curl of the 'qty' array
+
+        """
+
         if name == "hsm":
             return self.PROPID_HSM
         elif name == "rho":
             return self.PROPID_RHO
         elif name == "qty_mean":
             input_array = self.get_array_ref("qty")
             if len(input_array.shape) == 1:
@@ -258,77 +314,97 @@
             input_array = self.get_array_ref("qty")
             if len(input_array.shape) != 2 and input_array.shape[1] != 3:
                 raise ValueError("Can only compute curl of 3D arrays")
             return self.PROPID_QTYCURL
         else:
             raise ValueError("Unknown smoothing request %s" % name)
 
-    def populate(self, mode, nn, kernel = 'CubicSpline'):
+
+    def set_kernel(self, kernel = 'CubicSpline'):
+        """Set the kernel for smoothing operations.
+
+        Parameters
+        ----------
+        kernel : str
+            Keyword to specify the smoothing kernel. Options: 'CubicSpline', 'WendlandC2'
+        """
+        if kernel == 'CubicSpline':
+            self._kernel_id = 0
+        elif kernel == 'WendlandC2':
+            self._kernel_id = 1
+        else:
+            raise ValueError("Kernel %r not recognised. Please choose either 'CubicSpline' or 'WendlandC2'." % kernel)
+
+
+    def populate(self, mode, nn):
         """Create the KDTree and perform the operation specified by `mode`.
 
         Parameters
         --------
         mode : str (see `kdtree.smooth_operation_to_id`)
             Specify operation to perform (compute smoothing lengths, density, SPH mean, or SPH dispersion).
         nn : int
             Number of neighbours to be considered when smoothing.
-        kernel : str
-            Keyword to specify the smoothing kernel. Options: 'CubicSpline', 'WendlandC2'
         """
 
 
         if nn is None:
             nn = 64
 
-        smx = kdmain.nn_start(self.kdtree, int(nn), self.num_threads, self.boxsize)
+        smx = kdmain.nn_start(self.kdtree, int(nn), self.boxsize)
 
         try:
             propid = self.smooth_operation_to_id(mode)
 
             if propid == self.PROPID_HSM:
                 kdmain.domain_decomposition(self.kdtree, self.num_threads)
 
-            if kernel == 'CubicSpline':
-                kernel = 0
-            elif kernel == 'WendlandC2':
-                kernel = 1
-            else:
-                raise ValueError(
-                    "Kernel keyword %s not recognised. Please choose either 'CubicSpline' or 'WendlandC2'." % kernel
-                )
 
             if self.num_threads == 1:
-                kdmain.populate(self.kdtree, smx, propid, 0, kernel)
+                NT = 8
+                util.thread_map(
+                    kdmain.populate,
+                    [self.kdtree] * NT,
+                    [smx] * NT,
+                    [propid] * NT,
+                    list(range(0, NT)),
+                    [self._kernel_id] * NT
+                )
             else:
                 util.thread_map(
                     kdmain.populate,
                     [self.kdtree] * self.num_threads,
                     [smx] * self.num_threads,
                     [propid] * self.num_threads,
                     list(range(0, self.num_threads)),
-                    [kernel] * self.num_threads
+                    [self._kernel_id] * self.num_threads
                 )
         finally:
             # Free C-structures memory
             kdmain.nn_stop(self.kdtree, smx)
 
-    def sph_mean(self, array, nsmooth=64, kernel = 'CubicSpline'):
+    def sph_mean(self, array, nsmooth=64):
         r"""Calculate the SPH mean of a simulation array.
 
-        It's the application of the SPH interpolation formula for computing the smoothed quantity at particles position.
-        It uses the cubic spline smoothing kernel W.
+        Given a kernel W, this calculates
+
+        .. math::
 
-            qty_sm[i] = \sum_{j=0}^{nsmooth}( mass[j]/rho[j] * qty[i] * W(|pos[i] - pos[j]|, smooth[i]) )
+          r_i = \sum_{j=0}^{N_{smooth}}\left( \frac{m_j}{\rho_j} q_i W(|x_i - x_j|, s_i) \right)
 
-        Actual computation is done in the C-extension functions smooth.cpp::smMeanQty[1,N]D.
+        where r is the result of the smoothing, m is the mass array, rho is the density array, q is the input array,
+        s_i is the smoothing length, and W is the kernel function.
+
+        The actual computation is done in the C++-extension function smooth.cpp::smMeanQty[1,N]D.
 
         Parameters
         ----------
         array : pynbody.array.SimArray
             Quantity to smooth (compute SPH interpolation at particles position).
+
         nsmooth:
             Number of neighbours to use when smoothing.
 
         Returns
         -------
         output : pynbody.array.SimArray
             The SPH mean of the input array.
@@ -340,41 +416,47 @@
             output.units = array.units
 
         self.set_array_ref("qty", array)
         self.set_array_ref("qty_sm", output)
 
         logger.info("Smoothing array with %d nearest neighbours" % nsmooth)
         start = time.time()
-        self.populate("qty_mean", nsmooth, kernel)
+        self.populate("qty_mean", nsmooth)
         end = time.time()
 
         logger.info("SPH smooth done in %5.3g s" % (end - start))
 
         return output
 
-    def sph_dispersion(self, array, nsmooth=64, kernel = 'CubicSpline'):
+    def sph_dispersion(self, array, nsmooth=64):
         r"""Calculate the SPH dispersion of a simulation array.
 
-        It uses the cubic spline smoothing kernel W.
+        Given a kernel W, this routine computes the smoothed quantity:
 
-        First it computes the smoothed quantity:
+        .. math::
 
-            qty_sm[i] = \sum_{j=0}^{nsmooth}( mass[j]/rho[j] * qty[i] * W(|pos[i] - pos[j]|, smooth[i]) )
+          r_i = \sum_{j=0}^{N_{smooth}}\left( \frac{m_j}{\rho_j} q_i W(|x_i - x_j|, s_i) \right)
 
         Then the squared root of the SPH smoothed variance:
 
-            qty_disp[i] = \sqrt( \sum_{j=0}^{nsmooth}( mass[j]/rho[j] * (qty_sm[i] - qty[j])^2 * W(|pos[i] - pos[j]|, smooth[i]) ) )
+        .. math::
+
+          d_i = \left\{ \sum_{j=0}^{N_{smooth}} \frac{m_j}{\rho_j} (q_i - r_i)^2 W(|x_i - x_j|, s_i) \right\}^{1/2}
 
-        Actual computation is done in the C-extension functions smooth.cpp::smDispQty[1,N]D.
+        where d_i is the calculated dispersion, m is the mass array, rho is the density array, q is the input array,
+        s_i is the smoothing length, and W is the kernel function.
+
+        Actual computation is done in the C++-extension functions smooth.cpp::smDispQty[1,N]D.
 
         Parameters
         ----------
         array : pynbody.array.SimArray
             Quantity to compute dispersion of.
-        nsmooth:
+
+        nsmooth: int
             Number of neighbours to use when smoothing.
 
         Returns
         -------
         output : pynbody.array.SimArray
             The dispersion of the input array.
         """
@@ -384,22 +466,22 @@
             output.units = array.units
 
         self.set_array_ref("qty", array)
         self.set_array_ref("qty_sm", output)
 
         logger.info("Getting dispersion of array with %d nearest neighbours" % nsmooth)
         start = time.time()
-        self.populate("qty_disp", nsmooth, kernel)
+        self.populate("qty_disp", nsmooth)
         end = time.time()
 
         logger.info("SPH dispersion done in %5.3g s" % (end - start))
 
         return output
 
-    def _sph_differential_operator(self, array, op, nsmooth=64, kernel = 'CubicSpline'):
+    def _sph_differential_operator(self, array, op, nsmooth=64):
         if op == "div":
             op_label = "divergence"
             output = np.empty(len(array), dtype=array.dtype)
         elif op == "curl":
             op_label = "curl"
             output = np.empty_like(array)
         else:
@@ -410,23 +492,55 @@
             output.units = array.units/self._pos.units
 
         self.set_array_ref("qty", array)
         self.set_array_ref("qty_sm", output)
 
         logger.info("Getting %s of array with %d nearest neighbours" % (op_label, nsmooth))
         start = time.time()
-        self.populate("qty_%s" % op, nsmooth, kernel)
+        self.populate("qty_%s" % op, nsmooth)
         end = time.time()
 
         logger.info(f"SPH {op_label} done in {end - start:5.3g} s")
 
         return output
 
-    def sph_curl(self, array, nsmooth=64, kernel = 'CubicSpline'):
-        return self._sph_differential_operator(array, "curl", nsmooth, kernel)
+    def sph_curl(self, array, nsmooth=64):
+        """Calculate the curl of a given array using SPH smoothing.
+
+        Parameters
+        ----------
+
+        array : pynbody.array.SimArray
+            Quantity to compute curl of.
+
+        nsmooth : int
+            Number of neighbours to use when smoothing.
+
+        Returns
+        -------
+        pynbody.array.SimArray:
+            The curl of the input array.
+        """
+        return self._sph_differential_operator(array, "curl", nsmooth)
 
-    def sph_divergence(self, array, nsmooth=64, kernel = 'CubicSpline'):
-        return self._sph_differential_operator(array, "div", nsmooth, kernel)
+    def sph_divergence(self, array, nsmooth=64):
+        """Calculate the divergence of a given array using SPH smoothing.
+
+        Parameters
+        ----------
+
+        array : pynbody.array.SimArray
+            Quantity to compute curl of.
+
+        nsmooth : int
+            Number of neighbours to use when smoothing.
+
+        Returns
+        -------
+        pynbody.array.SimArray:
+            The curl of the input array.
+        """
+        return self._sph_differential_operator(array, "div", nsmooth)
 
     def __del__(self):
         if hasattr(self, "kdtree"):
             kdmain.free(self.kdtree)
```

### Comparing `pynbody-2.0.0b5/pynbody/kdtree/kd.cpp` & `pynbody-2.0.0b7/pynbody/kdtree/kd.cpp`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/kdtree/kd.h` & `pynbody-2.0.0b7/pynbody/kdtree/kd.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #ifndef KD_HINCLUDED
 #define KD_HINCLUDED
 
+#include <tuple>
+
 #include <Python.h>
 
 #define PY_ARRAY_UNIQUE_SYMBOL PYNBODY_ARRAY_API
 #include <numpy/arrayobject.h>
 
 #define ROOT 1
 #define LOWER(i) (i << 1)
@@ -36,15 +38,14 @@
   npy_intp pUpper;
 } KDNode;
 
 typedef struct KDContext {
   npy_intp nBucket;
   npy_intp nParticles;
   npy_intp nActive;
-  float fTime;
   int nLevels;
   npy_intp nNodes;
   npy_intp nSplit;
 
   npy_intp *particleOffsets; // length N array mapping from KDTree order to pynbody/file order
   PyObject *pNumpyParticleOffsets; // Numpy array from which the pointer stored in particleOffsets has been derived
 
@@ -162,14 +163,19 @@
   return *((T *)PyArray_GETPTR1(ar, i));
 }
 
 template <typename T> T GET2(PyObject *ar, npy_intp i, npy_intp j) {
   return *((T *)PyArray_GETPTR2(ar, i, j));
 }
 
+template <typename T> std::tuple<T, T, T> GET2(PyObject *ar, npy_intp i) {
+  T* ptr = (T *)PyArray_GETPTR1(ar, i);
+  return std::make_tuple(ptr[0], ptr[1], ptr[2]);
+}
+
 template <typename T> void SET(PyObject *ar, npy_intp i, T val) {
   *((T *)PyArray_GETPTR1(ar, i)) = val;
 }
 
 template <typename T> void SET2(PyObject *ar, npy_intp i, npy_intp j, T val) {
   *((T *)PyArray_GETPTR2(ar, i, j)) = val;
 }
@@ -178,11 +184,24 @@
   (*((T *)PyArray_GETPTR1(ar, i))) += val;
 }
 
 template <typename T> void ACCUM2(PyObject *ar, npy_intp i, npy_intp j, T val) {
   (*((T *)PyArray_GETPTR2(ar, i, j))) += val;
 }
 
+template <typename T>
+inline npy_intp kdFindLocalBucket(KDContext *kdtree, T *position) {
+  npy_intp cell = ROOT;
+  KDNode *c = kdtree->kdNodes;
+  while (cell < kdtree->nSplit) {
+    if (position[c[cell].iDim] < c[cell].fSplit)
+      cell = LOWER(cell);
+    else
+      cell = UPPER(cell);
+  }
+  return cell;
+}
+
 #define GETSMOOTH(T, pid) GET<T>(kd->pNumpySmooth, kd->particleOffsets[pid])
 #define SETSMOOTH(T, pid, val) SET<T>(kd->pNumpySmooth, kd->particleOffsets[pid], val)
 
 #endif
```

### Comparing `pynbody-2.0.0b5/pynbody/kdtree/kdmain.cpp` & `pynbody-2.0.0b7/pynbody/kdtree/kdmain.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -113,14 +113,21 @@
 
 template <> const char np_kind<float>() { return 'f'; }
 
 template <> const char np_kind<KDNode>() { return 'V'; }
 
 template <> const char np_kind<npy_intp>() { return 'i'; }
 
+template <typename T> const char py_kind() { return '?'; }
+
+template <> const char py_kind<double>() { return 'd'; }
+
+template <> const char py_kind<float>() { return 'f'; }
+
+
 template <typename T> int checkArray(PyObject *check, const char *name, npy_intp size=0, bool require_c_contiguous=false) {
   /* Checks that the passed object is a numpy array of the correct type, with the correct size (if specified), and is C-contiguous (if required)
   Returns 0 if the check passes, 1 if it fails (in which case an exception will have been set).
   */
 
   if (check == nullptr) {
     PyErr_Format(PyExc_ValueError, "An array must be passed for the '%s' argument", name);
@@ -307,153 +314,167 @@
 
   delete kd;
 
   Py_INCREF(Py_None);
   return Py_None;
 }
 
+
 /*==========================================================================*/
 /* nn_start                                                                 */
 /*==========================================================================*/
-PyObject *nn_start(PyObject *self, PyObject *args) {
-  KDContext* kd;
-  SMX smx;
+template<typename T> struct typed_nn_start {
+  static PyObject *call(PyObject *self, PyObject *args) {
+    KDContext* kd;
+    SmoothingContext<T> * smx;
 
-  PyObject *kdobj;
-  /* Nx1 Numpy arrays for smoothing length and density for calls that pass
-     in those values from existing arrays
-  */
+    PyObject *kdobj;
+    /* Nx1 Numpy arrays for smoothing length and density for calls that pass
+      in those values from existing arrays
+    */
 
-  int nSmooth, nProcs;
-  float period = std::numeric_limits<float>::max();
+    int nSmooth;
+    double period;
 
-  PyArg_ParseTuple(args, "Oii|f", &kdobj, &nSmooth, &nProcs, &period);
-  kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
+    PyArg_ParseTuple(args, "Oi|d", &kdobj, &nSmooth, &period);
+    kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
 
-  if (period <= 0)
-    period = std::numeric_limits<float>::max();
+    if (period <= 0)
+      period = std::numeric_limits<double>::max();
 
 
 
-  float fPeriod[3] = {period, period, period};
+    double fPeriod[3] = {period, period, period};
 
-  if (nSmooth > PyArray_DIM(kd->pNumpyPos, 0)) {
-    PyErr_SetString(
-        PyExc_ValueError,
-        "Number of smoothing particles exceeds number of particles in tree");
-    return NULL;
-  }
+    if (nSmooth > PyArray_DIM(kd->pNumpyPos, 0)) {
+      PyErr_SetString(
+          PyExc_ValueError,
+          "Number of smoothing particles exceeds number of particles in tree");
+      return NULL;
+    }
 
-  /*
-   ** Check to make sure that the bounds of the simulation agree
-   ** with the period specified, if not cause an error.
-   */
+    smCheckPeriodicityAndWarn(kd, fPeriod);
 
-  if (!smCheckFits(kd, fPeriod)) {
-    PyErr_SetString(
-        PyExc_ValueError,
-        "The particles span a region larger than the specified boxsize");
-    return NULL;
-  }
+    smx = smInit<T>(kd, nSmooth, period);
+    if (smx == nullptr) return nullptr; // smInit sets the error message
+    smSmoothInitStep(smx);
+    return PyCapsule_New(smx, NULL, NULL);
 
-  if (!smInit(&smx, kd, nSmooth, fPeriod)) {
-    PyErr_SetString(PyExc_RuntimeError, "Unable to create smoothing context");
-    return NULL;
   }
+};
+
 
-  smSmoothInitStep(smx, nProcs);
 
-  return PyCapsule_New(smx, NULL, NULL);
-}
 
 /*==========================================================================*/
 /* nn_next                                                                 */
 /*==========================================================================*/
-PyObject *nn_next(PyObject *self, PyObject *args) {
-  long nCnt, i, pj;
+template<typename T> struct typed_nn_next {
+  static PyObject *call(PyObject *self, PyObject *args) {
+    long nCnt, i, pj;
 
-  KDContext* kd;
-  SMX smx;
+    KDContext* kd;
+    SmoothingContext<T> * smx;
 
-  PyObject *kdobj, *smxobj;
-  PyObject *nnList;
-  PyObject *nnDist;
-  PyObject *retList;
+    PyObject *kdobj, *smxobj;
+    PyObject *nnList;
+    PyObject *nnDist;
+    PyObject *retList;
 
-  PyArg_ParseTuple(args, "OO", &kdobj, &smxobj);
-  kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
-  smx = (SMX)PyCapsule_GetPointer(smxobj, NULL);
+    PyArg_ParseTuple(args, "OO", &kdobj, &smxobj);
+    kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
+    smx = static_cast<SmoothingContext<T>*>(PyCapsule_GetPointer(smxobj, NULL));
 
-  Py_BEGIN_ALLOW_THREADS;
+    if(smx==nullptr) {
+      PyErr_SetString(PyExc_ValueError, "Invalid smoothing context object");
+      return nullptr;
+    }
 
-  if (kd->nBitDepth == 32) nCnt = smSmoothStep<float>(smx, 0);
-  else nCnt = smSmoothStep<double>(smx, 0);
+    Py_BEGIN_ALLOW_THREADS;
 
-  Py_END_ALLOW_THREADS;
+    nCnt = smSmoothStep<T>(smx, 0);
 
-  if (nCnt > 0) {
-    nnList = PyList_New(nCnt); // Py_INCREF(nnList);
-    nnDist = PyList_New(nCnt); // Py_INCREF(nnDist);
-    retList = PyList_New(4);
-    Py_INCREF(retList);
+    Py_END_ALLOW_THREADS;
 
-    for (i = 0; i < nCnt; i++) {
-      pj = smx->pList[i];
-      PyList_SetItem(nnList, i, PyLong_FromLong(smx->kd->particleOffsets[pj]));
-      PyList_SetItem(nnDist, i, PyFloat_FromDouble(smx->fList[i]));
-    }
+    if (nCnt > 0) {
+      nnList = PyList_New(nCnt); // Py_INCREF(nnList);
+      nnDist = PyList_New(nCnt); // Py_INCREF(nnDist);
+      retList = PyList_New(4);
+      Py_INCREF(retList);
+
+      for (i = 0; i < nCnt; i++) {
+        pj = smx->pList[i];
+        PyList_SetItem(nnList, i, PyLong_FromLong(smx->kd->particleOffsets[pj]));
+        PyList_SetItem(nnDist, i, PyFloat_FromDouble(smx->fList[i]));
+      }
 
-    PyList_SetItem(retList, 0, PyLong_FromLong(smx->kd->particleOffsets[smx->pi]));
-    if (kd->nBitDepth == 32)
-      PyList_SetItem(retList, 1, PyFloat_FromDouble(GETSMOOTH(float, smx->pi)));
-    else
-      PyList_SetItem(retList, 1,
-                     PyFloat_FromDouble(GETSMOOTH(double, smx->pi)));
-    PyList_SetItem(retList, 2, nnList);
-    PyList_SetItem(retList, 3, nnDist);
+      PyList_SetItem(retList, 0, PyLong_FromLong(smx->kd->particleOffsets[smx->pi]));
+      PyList_SetItem(retList, 1, PyFloat_FromDouble(GETSMOOTH(T, smx->pi)));
+      PyList_SetItem(retList, 2, nnList);
+      PyList_SetItem(retList, 3, nnDist);
+
+      return retList;
+    }
 
-    return retList;
+    Py_INCREF(Py_None);
+    return Py_None;
   }
+};
+
+
 
-  Py_INCREF(Py_None);
-  return Py_None;
-}
 
 /*==========================================================================*/
 /* nn_stop                                                                 */
 /*==========================================================================*/
-PyObject *nn_stop(PyObject *self, PyObject *args) {
-  KDContext* kd;
-  SMX smx;
+template<typename T> struct typed_nn_stop {
+  static PyObject *call(PyObject *self, PyObject *args) {
+    KDContext* kd;
+    SmoothingContext<T> * smx;
 
-  PyObject *kdobj, *smxobj;
+    PyObject *kdobj, *smxobj;
+
+    PyArg_ParseTuple(args, "OO", &kdobj, &smxobj);
+    kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
+    smx = static_cast<SmoothingContext<T>*>(PyCapsule_GetPointer(smxobj, NULL));
+    if(smx==nullptr) {
+      PyErr_SetString(PyExc_ValueError, "Invalid smoothing context object");
+      return nullptr;
+    }
+    delete smx;
+
+    Py_INCREF(Py_None);
+    return Py_None;
+  }
+};
 
-  PyArg_ParseTuple(args, "OO", &kdobj, &smxobj);
-  kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
-  smx = (SMX)PyCapsule_GetPointer(smxobj, NULL);
 
-  smFinish(smx);
 
-  Py_INCREF(Py_None);
-  return Py_None;
-}
 
 /*==========================================================================*/
 /* nn_rewind                                                                */
 /*==========================================================================*/
-PyObject *nn_rewind(PyObject *self, PyObject *args) {
-  SMX smx;
-  PyObject *smxobj;
+template<typename T> struct typed_nn_rewind {
+  static PyObject *call(PyObject *self, PyObject *args) {
+    SmoothingContext<T> * smx;
+    PyObject *smxobj;
+
+    PyArg_ParseTuple(args, "O", &smxobj);
+    smx = static_cast<SmoothingContext<T> * >(PyCapsule_GetPointer(smxobj, nullptr));
+    if(smx==nullptr) {
+      PyErr_SetString(PyExc_ValueError, "Invalid smoothing context object");
+      return nullptr;
+    }
+    smSmoothInitStep(smx);
+
+    return PyCapsule_New(smx, NULL, NULL);
+  }
+};
 
-  PyArg_ParseTuple(args, "O", &smxobj);
-  smx = (SMX)PyCapsule_GetPointer(smxobj, NULL);
-  smSmoothInitStep(smx, 1);
 
-  return PyCapsule_New(smx, NULL, NULL);
-}
 
 int getBitDepth(PyObject *check) {
 
   if (check == NULL) {
     return 0;
   }
 
@@ -608,59 +629,64 @@
 
   Py_INCREF(Py_None);
   return Py_None;
 }
 
 template <typename Tf, typename Tq> struct typed_particles_in_sphere {
   static PyObject *call(PyObject *self, PyObject *args) {
-    SMX smx;
+    SmoothingContext<Tf> * smx;
     KDContext* kd;
-    float r;
-    float ri[3];
+    Tf r;
+    Tf ri[3];
+
+    std::string pytype_s = "OO" + std::string(4, py_kind<Tf>());
+    const char* pytype = pytype_s.c_str();
 
     PyObject *kdobj = nullptr, *smxobj = nullptr;
 
-    PyArg_ParseTuple(args, "OOffff", &kdobj, &smxobj, &ri[0], &ri[1], &ri[2],
+
+    PyArg_ParseTuple(args, pytype, &kdobj, &smxobj, &ri[0], &ri[1], &ri[2],
                      &r);
 
     kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
-    smx = (SMX)PyCapsule_GetPointer(smxobj, NULL);
+    smx = (SmoothingContext<Tf> *)PyCapsule_GetPointer(smxobj, NULL);
 
     initParticleList(smx);
     smBallGather<Tf, smBallGatherStoreResultInList>(smx, r * r, ri);
 
     return getReturnParticleList(smx);
   }
 };
 
 template <typename Tf, typename Tq> struct typed_populate {
   static PyObject *call(PyObject *self, PyObject *args) {
 
     long i, nCnt;
     int procid;
     KDContext* kd;
-    SMX smx_global, smx_local;
+    SmoothingContext<Tf> *smx_global, *smx_local;
     int propid;
-    float ri[3];
-    float hsm;
+    Tf ri[3];
+    Tf hsm;
     int Wendland;
 
-    void (*pSmFn)(SMX, npy_intp, int, npy_intp *, float *, bool) = NULL;
+    void (*pSmFn)(SmoothingContext<Tf> *, npy_intp, int, bool) = NULL;
 
     PyObject *kdobj, *smxobj;
 
     PyArg_ParseTuple(args, "OOiii", &kdobj, &smxobj, &propid, &procid,
                      &Wendland);
     kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, NULL));
-    smx_global = (SMX)PyCapsule_GetPointer(smxobj, NULL);
+    smx_global = (SmoothingContext<Tf> *)PyCapsule_GetPointer(smxobj, NULL);
 
     long nbodies = PyArray_DIM(kd->pNumpyPos, 0);
 
     if (checkArray<Tf>(kd->pNumpySmooth, "smooth"))
       return NULL;
+
     if (propid > PROPID_HSM) {
       if (checkArray<Tf>(kd->pNumpyDen, "rho"))
         return NULL;
       if (checkArray<Tf>(kd->pNumpyMass, "mass"))
         return NULL;
     }
     if (propid > PROPID_RHO) {
@@ -722,29 +748,28 @@
         for (int j = 0; j < 3; ++j) {
           ri[j] = GET2<Tf>(kd->pNumpyPos, kd->particleOffsets[i], j);
         }
 
         // retrieve the existing smoothing length
         hsm = GETSMOOTH(Tf, i);
 
-        // use it to get nearest neighbours
-        nCnt = smBallGather<Tf, smBallGatherStoreResultInSmx>(
-            smx_local, 4 * hsm * hsm, ri);
+        // use it to get nearest neighbours - NB following should be Tf not double
+        nCnt = smBallGather<Tf, smBallGatherStoreResultInSmx>(smx_local, 4 * hsm * hsm, ri);
 
         // calculate the density
-        (*pSmFn)(smx_local, i, nCnt, smx_local->pList, smx_local->fList,
-                 Wendland);
+        (*pSmFn)(smx_local, i, nCnt, Wendland);
 
         // select next particle in coordination with other threads
         i = smGetNext(smx_local);
 
         if (smx_global->warnings)
           break;
       }
       Py_END_ALLOW_THREADS;
+
     }
 
     smFinishThreadLocalCopy(smx_local);
     if (smx_local->warnings) {
       PyErr_SetString(PyExc_RuntimeError,
                       "Buffer overflow in smoothing operation. This probably "
                       "means that your smoothing lengths are too large "
@@ -754,15 +779,15 @@
       Py_INCREF(Py_None);
       return Py_None;
     }
   }
 };
 
 template <template <typename, typename> class func>
-PyObject *type_dispatcher(PyObject *self, PyObject *args) {
+PyObject *type_dispatcher_2(PyObject *self, PyObject *args) {
   PyObject *kdobj = PyTuple_GetItem(args, 0);
   if (kdobj == nullptr) {
     PyErr_SetString(PyExc_ValueError, "First argument must be a kdtree object");
     return nullptr;
   }
   KDContext* kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, nullptr));
   int nF = kd->nBitDepth;
@@ -782,14 +807,53 @@
     return func<float, double>::call(self, args);
   else {
     PyErr_SetString(PyExc_ValueError, "Unsupported dtype combination");
     return nullptr;
   }
 }
 
+template <template <typename> class func>
+PyObject *type_dispatcher_1(PyObject *self, PyObject *args) {
+  PyObject *kdobj = PyTuple_GetItem(args, 0);
+  if (kdobj == nullptr) {
+    PyErr_SetString(PyExc_ValueError, "First argument must be a kdtree object");
+    return nullptr;
+  }
+  KDContext* kd = static_cast<KDContext*>(PyCapsule_GetPointer(kdobj, nullptr));
+  int nF = kd->nBitDepth;
+
+  if (nF == 64)
+    return func<double>::call(self, args);
+  else if (nF == 32)
+    return func<float>::call(self, args);
+  else {
+    PyErr_SetString(PyExc_ValueError, "Unsupported dtype combination");
+    return nullptr;
+  }
+}
+
+PyObject *nn_start(PyObject *self, PyObject *args) {
+  return type_dispatcher_1<typed_nn_start>(self, args);
+}
+
+PyObject *nn_next(PyObject *self, PyObject *args) {
+  return type_dispatcher_1<typed_nn_next>(self, args);
+}
+
+PyObject *nn_stop(PyObject *self, PyObject *args) {
+  return type_dispatcher_1<typed_nn_stop>(self, args);
+}
+
+
+PyObject *nn_rewind(PyObject *self, PyObject *args) {
+  return type_dispatcher_1<typed_nn_rewind>(self, args);
+}
+
+
+
 PyObject *populate(PyObject *self, PyObject *args) {
-  return type_dispatcher<typed_populate>(self, args);
+  return type_dispatcher_2<typed_populate>(self, args);
 }
 
 PyObject *particles_in_sphere(PyObject *self, PyObject *args) {
-  return type_dispatcher<typed_particles_in_sphere>(self, args);
+  return type_dispatcher_2<typed_particles_in_sphere>(self, args);
 }
```

### Comparing `pynbody-2.0.0b5/pynbody/kdtree/smooth.cpp` & `pynbody-2.0.0b7/pynbody/kdtree/smooth.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,72 @@
-#define NO_IMPORT_ARRAY
+#pragma once
 
-#include "smooth.h"
 #include "kd.h"
-#include <assert.h>
+#include "pq.h"
 #include <functional>
+#include <memory>
+#include <mutex>
+#include <stdbool.h>
+#include <vector>
 #include <iostream>
-#include <math.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
+#include <queue>
+#include <cmath>
 
-bool smCheckFits(KDContext* kd, float *fPeriod) {
+#define RESMOOTH_SAFE 500
+#define WORKUNIT 1000
+
+
+#define M_1_PI 0.31830988618379067154
+
+
+
+template<typename T>
+class SmoothingContext {
+public:
+  KDContext* kd;
+
+  npy_intp nSmooth;
+  T fPeriod[3];
+
+  npy_intp nListSize;
+  std::vector<T> fList;
+  std::vector<npy_intp> pList;
+
+  npy_intp pin = 0, pi = 0, pNext = 0; // particle indices for distributed loops (TODO: rationalise)
+  npy_intp nCurrent = 0; // particle indices for distributed loops (TODO: rationalise)
+
+  std::shared_ptr<std::mutex> pMutex;
+
+  SmoothingContext<T> * smx_global;
+
+
+  T ax = 0.0, ay = 0.0, az = 0.0;
+  bool warnings; //  keep track of whether a warning has been issued
+
+  std::unique_ptr<std::vector<npy_intp>> result;
+  std::unique_ptr<PriorityQueue<T>> priorityQueue;
+
+  SmoothingContext(KDContext* kd, npy_intp nSmooth, T fPeriod[3]) : kd(kd), nSmooth(nSmooth), fPeriod{fPeriod[0], fPeriod[1], fPeriod[2]},
+      nListSize(nSmooth + RESMOOTH_SAFE), fList(nListSize), pList(nListSize),
+      pMutex(std::make_shared<std::mutex>()),
+      priorityQueue(std::make_unique<PriorityQueue<T>>(nSmooth, kd->nActive)) {
+
+  }
+
+  SmoothingContext(const SmoothingContext<T> &copy) : kd(copy.kd), nSmooth(copy.nSmooth),
+      fPeriod{copy.fPeriod[0], copy.fPeriod[1], copy.fPeriod[2]},
+      nListSize(copy.nListSize), fList(nListSize), pList(nListSize), pMutex(copy.pMutex),
+      smx_global(const_cast<SmoothingContext<T>*>(&copy)),
+      priorityQueue(std::make_unique<PriorityQueue<T>>(nSmooth, kd->nActive)) { }
+      // copy constructor takes a pointer to the global context
+};
+
+
+template<typename T>
+bool smCheckFits(KDContext* kd, T *fPeriod) {
   KDNode *root;
   npy_intp j;
 
   assert(kd->kdNodes != nullptr);
   root = &kd->kdNodes[ROOT];
   assert(root != nullptr);
   /*
@@ -25,107 +77,63 @@
     if (root->bnd.fMax[j] - root->bnd.fMin[j] > fPeriod[j]) {
       return false;
     }
   }
   return true;
 }
 
-int smInit(SMX *psmx, KDContext* kd, int nSmooth, float *fPeriod) {
-  SMX smx;
-  KDNode *root;
-  int j;
-  int bError = 0;
 
-  root = &kd->kdNodes[ROOT];
-  assert(root != NULL);
-  /*
-   ** Check to make sure that the bounds of the simulation agree
-   ** with the period specified, if not cause an error.
-   */
-  for (j = 0; j < 3; ++j) {
-    if (root->bnd.fMax[j] - root->bnd.fMin[j] > fPeriod[j]) {
-      PyErr_SetString(
-          PyExc_ValueError,
-          "The particles span a region larger than the specified boxsize");
-      bError = 1;
-    }
+template<typename T>
+void smCheckPeriodicityAndWarn(KDContext* kd, T fPeriod[3]) {
+  if (!smCheckFits(kd, fPeriod)) {
+    PyErr_WarnEx(PyExc_RuntimeWarning,
+                 "\r\n\r\nThe particles span a region larger than the specified boxsize; disabling periodicity.\r\n\r\n"
+                 "For more information about this warning, see the module documentation for KDTree, \r\n"
+                 "https://pynbody.readthedocs.io/latest/reference/_autosummary/pynbody.kdtree.KDTree.html",
+                 1);
+    fPeriod[0] = fPeriod[1] = fPeriod[2] = std::numeric_limits<T>::max();
   }
+}
 
-  assert(nSmooth <= kd->nActive);
-  smx = new smContext;
-  smx->kd = kd;
-  smx->nSmooth = nSmooth;
-  smx->pq = (PQ *)malloc(nSmooth * sizeof(PQ));
-  assert(smx->pq != NULL);
-  PQ_INIT(smx->pq, nSmooth);
-  smx->iMark = (char *)malloc(kd->nActive * sizeof(char));
-  assert(smx->iMark != NULL);
-  smx->nListSize = smx->nSmooth + RESMOOTH_SAFE;
-  smx->fList = (float *)malloc(smx->nListSize * sizeof(float));
-  assert(smx->fList != NULL);
-  smx->pList = (npy_intp *)malloc(smx->nListSize * sizeof(npy_intp));
-  assert(smx->pList != NULL);
-  for (j = 0; j < 3; ++j)
-    smx->fPeriod[j] = fPeriod[j];
-
-  smx->nCurrent = 0;
-  smx->pMutex = std::make_shared<std::mutex>();
-  smx->smx_global = NULL;
+template<typename T>
+SmoothingContext<T> * smInit(KDContext* kd, int nSmooth, T fPeriod) {
+  T fPeriodArray[3] = {fPeriod, fPeriod, fPeriod};
 
-  *psmx = smx;
-  return (1);
-}
+  if(&(kd->kdNodes[ROOT]) == nullptr) {
+    PyErr_SetString(PyExc_ValueError, "Invalid KDTree");
+    return nullptr;
+  }
 
-SMX smInitThreadLocalCopy(SMX from) {
+  if(nSmooth > kd->nActive) {
+    PyErr_SetString(PyExc_ValueError, "nSmooth must be less than or equal to the number of particles");
+    return nullptr;
+  }
 
-  SMX smx;
-  KDNode *root;
-  npy_intp pi;
-  int j;
+  smCheckPeriodicityAndWarn(kd, fPeriodArray);
 
-  root = &from->kd->kdNodes[ROOT];
+  auto smx = new SmoothingContext<T>(kd, nSmooth, fPeriodArray); // not shared_ptr because python will memory manage it
 
-  smx = new smContext;
-  smx->kd = from->kd;
-  smx->nSmooth = from->nSmooth;
-  smx->pq = (PQ *)malloc(from->nSmooth * sizeof(PQ));
-  assert(smx->pq != NULL);
-  PQ_INIT(smx->pq, from->nSmooth);
-  smx->iMark = (char *)malloc(from->kd->nActive * sizeof(char));
-  assert(smx->iMark != NULL);
-  smx->nListSize = from->nListSize;
-  smx->fList = (float *)malloc(smx->nListSize * sizeof(float));
-  assert(smx->fList != NULL);
-  smx->pList = (npy_intp *)malloc(smx->nListSize * sizeof(npy_intp));
-  assert(smx->pList != NULL);
-  for (j = 0; j < 3; ++j)
-    smx->fPeriod[j] = from->fPeriod[j];
-  for (pi = 0; pi < smx->kd->nActive; ++pi) {
-    smx->iMark[pi] = 0;
-  }
-  smx->pMutex = from->pMutex;
+  return smx;
 
-  smx->smx_global = from;
-  smx->nCurrent = 0;
+}
+
+template<typename T>
+SmoothingContext<T> * smInitThreadLocalCopy(SmoothingContext<T> * from) {
+  auto smx = new SmoothingContext<T>(*from);
 
-  smInitPriorityQueue(smx);
   return smx;
 }
 
-void smFinishThreadLocalCopy(SMX smx) {
-  free(smx->pq);
-  free(smx->fList);
-  free(smx->pList);
-  free(smx->iMark);
+template<typename T>
+void smFinishThreadLocalCopy(SmoothingContext<T> * smx) {
   delete smx;
 }
 
-#define WORKUNIT 1000
-
-npy_intp smGetNext(SMX smx_local) {
+template<typename T>
+npy_intp smGetNext(SmoothingContext<T> * smx_local) {
 
   // synchronize warning state
   if (smx_local->warnings)
     smx_local->smx_global->warnings = true;
 
   npy_intp i = smx_local->nCurrent;
 
@@ -135,221 +143,204 @@
     smx_local->pMutex->lock();
     smx_local->nCurrent = smx_local->smx_global->nCurrent;
     i = smx_local->nCurrent;
     smx_local->smx_global->nCurrent += WORKUNIT;
     smx_local->pMutex->unlock();
   }
 
-  // i now has the next thing to be processed
-  // increment the local counter
 
-  smx_local->nCurrent += 1;
+  smx_local->nCurrent += 1; // increment the local counter, ready for next time we are called
 
   return i;
 }
 
-void smFinish(SMX smx) {
-  free(smx->iMark);
-  free(smx->pq);
-  free(smx->fList);
-  free(smx->pList);
 
-  delete smx;
-}
 
-template <typename T> void smBallSearch(SMX smx, float fBall2, float *ri) {
+
+
+template <typename T>
+void smBallSearch(SmoothingContext<T> *smx, T *ri) {
+  // Search for the nearest neighbors to the particle at ri[3].
+  // The priority queue must already be fully populated with some candidate particles. The better candidates the
+  // faster the search will perform.
   KDNode *c;
   npy_intp *p;
   KDContext* kd;
+
+  PriorityQueue<T> *priorityQueue = smx->priorityQueue.get();
+
   npy_intp cell, cp, ct, pj;
+
   T fDist2, dx, dy, dz, lx, ly, lz, sx, sy, sz, x, y, z;
-  PQ *pq;
 
   kd = smx->kd;
   c = smx->kd->kdNodes;
   p = smx->kd->particleOffsets;
-  pq = smx->pqHead;
+
   x = ri[0];
   y = ri[1];
   z = ri[2];
   lx = smx->fPeriod[0];
   ly = smx->fPeriod[1];
   lz = smx->fPeriod[2];
-  cell = ROOT;
-  /*
-   ** First find the "local" Bucket.
-   ** This could mearly be the closest bucket to ri[3].
-   */
-  while (cell < smx->kd->nSplit) {
-    if (ri[c[cell].iDim] < c[cell].fSplit)
-      cell = LOWER(cell);
-    else
-      cell = UPPER(cell);
-  }
-  /*
-   ** Now start the search from the bucket given by cell!
-   */
-  for (pj = c[cell].pLower; pj <= c[cell].pUpper; ++pj) {
-    dx = x - GET2<T>(kd->pNumpyPos, p[pj], 0);
-    dy = y - GET2<T>(kd->pNumpyPos, p[pj], 1);
-    dz = z - GET2<T>(kd->pNumpyPos, p[pj], 2);
+
+  cell = kdFindLocalBucket(kd, ri);
+
+  T fBall2 = priorityQueue->topDistanceSquaredOrMax();
+
+  npy_intp start_particle = c[cell].pLower;
+  npy_intp end_particle = c[cell].pUpper;
+
+  for (pj = start_particle; pj <= end_particle; ++pj) {
+    std::tie(dx, dy, dz) = GET2<T>(kd->pNumpyPos, p[pj]);
+    dx = x-dx;
+    dy = y-dy;
+    dz = z-dz;
+
     fDist2 = dx * dx + dy * dy + dz * dz;
-    if (fDist2 < fBall2) {
-      if (smx->iMark[pj])
-        continue;
-      smx->iMark[pq->p] = 0;
-      smx->iMark[pj] = 1;
-      pq->fKey = fDist2;
-      pq->p = pj;
-      pq->ax = 0.0;
-      pq->ay = 0.0;
-      pq->az = 0.0;
-      PQ_REPLACE(pq);
-      fBall2 = pq->fKey;
-    }
+    priorityQueue->push(fDist2, pj);
   }
   while (cell != ROOT) {
     cp = SIBLING(cell);
     ct = cp;
     SETNEXT(ct, ROOT);
     while (1) {
       INTERSECT(c, cp, fBall2, lx, ly, lz, x, y, z, sx, sy, sz);
       /*
        ** We have an intersection to test.
        */
       if (cp < smx->kd->nSplit) {
         cp = LOWER(cp);
         continue;
       } else {
-        for (pj = c[cp].pLower; pj <= c[cp].pUpper; ++pj) {
-          dx = sx - GET2<T>(kd->pNumpyPos, p[pj], 0);
-          dy = sy - GET2<T>(kd->pNumpyPos, p[pj], 1);
-          dz = sz - GET2<T>(kd->pNumpyPos, p[pj], 2);
+        start_particle = c[cp].pLower;
+        end_particle = c[cp].pUpper;
+
+        for (pj = start_particle; pj <= end_particle; ++pj) {
+          std::tie(dx, dy, dz) = GET2<T>(kd->pNumpyPos, p[pj]);
+          dx = sx-dx; dy = sy-dy; dz = sz-dz;
           fDist2 = dx * dx + dy * dy + dz * dz;
           if (fDist2 < fBall2) {
-            if (smx->iMark[pj])
-              continue;
-            smx->iMark[pq->p] = 0;
-            smx->iMark[pj] = 1;
-            pq->fKey = fDist2;
-            pq->p = pj;
-            pq->ax = sx - x;
-            pq->ay = sy - y;
-            pq->az = sz - z;
-            PQ_REPLACE(pq);
-            fBall2 = pq->fKey;
+            priorityQueue->push(fDist2, pj);
+            fBall2 = priorityQueue->topDistanceSquaredOrMax();
           }
         }
       }
     GetNextCell:
       SETNEXT(cp, ROOT);
       if (cp == ct)
         break;
     }
     cell = PARENT(cell);
   }
-  smx->pqHead = pq;
-}
-
-void initParticleList(SMX smx) {
-  smx->result = std::make_unique<std::vector<npy_intp>>();
-  smx->result->reserve(100000);
-  // not so large that it's expensive to reserve.
-  // Not so small that we constantly need to get more space.
 }
 
-PyObject *getReturnParticleList(SMX smx) {
-  // make a numpy array from smx->result
-  npy_intp dims[1] = {static_cast<npy_intp>(smx->result->size())};
-  PyObject *numpy_result = PyArray_SimpleNew(1, dims, NPY_INTP);
 
-  std::copy(smx->result->begin(), smx->result->end(),
-            static_cast<long *>(
-                PyArray_DATA(reinterpret_cast<PyArrayObject *>(numpy_result))));
-  smx->result.reset(nullptr);
-
-  return numpy_result;
+template<typename T>
+inline npy_intp smBallGatherStoreResultInList(SmoothingContext<T>* smx, T fDist2,
+                                              npy_intp particleIndex,
+                                              npy_intp foundIndex) {
+  smx->result->push_back(smx->kd->particleOffsets[particleIndex]);
+  return particleIndex + 1;
+}
+
+template<typename T>
+inline npy_intp smBallGatherStoreResultInSmx(SmoothingContext<T>* smx, T fDist2,
+                                             npy_intp particleIndex,
+                                             npy_intp foundIndex) {
+  if (foundIndex >= smx->nListSize) {
+    if (!smx->warnings)
+      fprintf(stderr, "Smooth - particle cache too small for local density - "
+                      "results will be incorrect\n");
+    smx->warnings = true;
+    return foundIndex;
+  }
+  smx->fList[foundIndex] = fDist2;
+  smx->pList[foundIndex] = particleIndex;
+  return foundIndex + 1;
 }
 
-void smSmoothInitStep(SMX smx, int nProcs_for_smooth) {
 
-  npy_intp pi;
+template <typename T,
+          npy_intp (*storeResultFunction)(SmoothingContext<T> *, T, npy_intp, npy_intp)>
+npy_intp smBallGather(SmoothingContext<T> * smx, T fBall2, T *ri) {
+  /* Gather all particles within the specified radius, using the storeResultFunction callback
+   * to store the results. */
+  KDNode *c;
+  npy_intp *p;
   KDContext* kd = smx->kd;
+  npy_intp pj, nCnt, cp, nSplit;
+  T dx, dy, dz, x, y, z, lx, ly, lz, sx, sy, sz, fDist2;
 
-  for (pi = 0; pi < kd->nActive; ++pi) {
-    smx->iMark[pi] = 0;
-  }
-
-  smInitPriorityQueue(smx);
-}
+  c = smx->kd->kdNodes;
+  p = smx->kd->particleOffsets;
+  nSplit = smx->kd->nSplit;
+  lx = smx->fPeriod[0];
+  ly = smx->fPeriod[1];
+  lz = smx->fPeriod[2];
+  x = ri[0];
+  y = ri[1];
+  z = ri[2];
 
-template <typename T> void smDomainDecomposition(KDContext* kd, int nprocs) {
+  // fBall2 = std::nextafter(fBall2, std::numeric_limits<T>::max());
 
-  // AP 31/8/2014 - Here is the domain decomposition for nProcs>1
-  // In principle one should do better by localizing the
-  // domains -- the current approach is a seriously naive decomposition.
-  // This will result in more snake collisions than necessary.
-  // However in practice, up to nCpu = 8, the scaling is looking
-  // pretty linear anyway so I'm leaving that for future.
-
-  npy_intp pi;
+  nCnt = 0;
+  cp = ROOT;
+  while (1) {
+    INTERSECT(c, cp, fBall2, lx, ly, lz, x, y, z, sx, sy, sz);
+    /*
+     ** We have an intersection to test.
+     */
 
-  if (nprocs > 0) {
-    for (pi = 0; pi < kd->nActive; ++pi) {
-      SETSMOOTH(T, pi, -(float)(1 + pi % nprocs));
+    if (cp < nSplit) {
+      cp = LOWER(cp);
+      continue;
+    } else {
+      for (pj = c[cp].pLower; pj <= c[cp].pUpper; ++pj) {
+        dx = sx - GET2<T>(kd->pNumpyPos, p[pj], 0);
+        dy = sy - GET2<T>(kd->pNumpyPos, p[pj], 1);
+        dz = sz - GET2<T>(kd->pNumpyPos, p[pj], 2);
+        fDist2 = dx * dx + dy * dy + dz * dz;
+        if (fDist2 <= fBall2) {
+          nCnt = storeResultFunction(smx, fDist2, pj, nCnt);
+        }
+      }
     }
+  GetNextCell:
+    // called by INTERSECT when a cell can be ignored, and finds the next cell
+    // to inspect
+    SETNEXT(cp, ROOT);
+    if (cp == ROOT)
+      break;
   }
+  assert(nCnt <= smx->nListSize);
+  return (nCnt);
 }
 
-void smInitPriorityQueue(SMX smx) {
-  /*
-   ** Initialize Priority Queue.
-   */
 
-  PQ *pq, *pqLast;
-  npy_intp pin, pj, pNext;
-  float ax, ay, az;
-
-  pqLast = &smx->pq[smx->nSmooth - 1];
-  pin = 0;
-  pNext = 1;
-  ax = 0.0;
-  ay = 0.0;
-  az = 0.0;
-
-  for (pq = smx->pq, pj = 0; pq <= pqLast; ++pq, ++pj) {
-    smx->iMark[pj] = 1;
-    pq->p = pj;
-    pq->ax = ax;
-    pq->ay = ay;
-    pq->az = az;
-  }
-  smx->pin = pin;
-  smx->pNext = pNext;
-  smx->ax = ax;
-  smx->ay = ay;
-  smx->az = az;
-}
+template <typename T>
+PyObject *getReturnParticleList(SmoothingContext<T> * smx);
+
 
-template <typename T> npy_intp smSmoothStep(SMX smx, int procid) {
+template <typename T>
+npy_intp smSmoothStep(SmoothingContext<T> * smx, int procid) {
   KDNode *c;
   npy_intp *p;
-  PQ *pq, *pqLast;
+
   KDContext* kd = smx->kd;
-  npy_intp cell;
   npy_intp pi, pin, pj, pNext, nCnt, nSmooth;
   npy_intp nScanned = 0;
 
-  float dx, dy, dz, x, y, z, h2, ax, ay, az;
-  float proc_signal = -(float)(procid)-1.0;
-  float ri[3];
+  T dx, dy, dz, x, y, z, h2, ax, ay, az;
+  T proc_signal = -static_cast<T>(procid)-1.0;
+  T ri[3];
 
   c = smx->kd->kdNodes;
   p = smx->kd->particleOffsets;
-  pqLast = &smx->pq[smx->nSmooth - 1];
+
   nSmooth = smx->nSmooth;
   pin = smx->pin;
   pNext = smx->pNext;
   ax = smx->ax;
   ay = smx->ay;
   az = smx->az;
 
@@ -369,278 +360,381 @@
         pNext = 0;
       if (nScanned == smx->kd->nActive) {
         // Nothing remains to be done.
         return -1;
       }
     }
 
+
+
     // mark the particle as 'processed' by assigning a dummy positive value
     // N.B. a race condition here doesn't matter since duplicating a bit of
     // work is more efficient than using a mutex (verified).
     SETSMOOTH(T, pNext, 10);
 
     pi = pNext;
     ++pNext;
-    x = GET2<T>(kd->pNumpyPos, p[pi], 0);
-    y = GET2<T>(kd->pNumpyPos, p[pi], 1);
-    z = GET2<T>(kd->pNumpyPos, p[pi], 2);
-    /*
-    ** First find the "local" Bucket.
-    ** This could merely be the closest bucket to ri[3].
-    */
-    cell = ROOT;
-    while (cell < smx->kd->nSplit) {
-      if (GET2<T>(kd->pNumpyPos, p[pi], c[cell].iDim) < c[cell].fSplit)
-        cell = LOWER(cell);
-      else
-        cell = UPPER(cell);
-    }
-    /*
-    ** Remove everything from the queue.
-    */
-    smx->pqHead = NULL;
-    for (pq = smx->pq; pq <= pqLast; ++pq)
-      smx->iMark[pq->p] = 0;
-    /*
-    ** Add everything from pj up to and including pj+nSmooth-1.
-    */
-    pj = c[cell].pLower;
-    if (pj > smx->kd->nActive - nSmooth)
-      pj = smx->kd->nActive - nSmooth;
-    for (pq = smx->pq; pq <= pqLast; ++pq) {
-      smx->iMark[pj] = 1;
-      dx = x - GET2<T>(kd->pNumpyPos, p[pj], 0);
-      dy = y - GET2<T>(kd->pNumpyPos, p[pj], 1);
-      dz = z - GET2<T>(kd->pNumpyPos, p[pj], 2);
-      pq->fKey = dx * dx + dy * dy + dz * dz;
-      pq->p = pj++;
-      pq->ax = 0.0;
-      pq->ay = 0.0;
-      pq->az = 0.0;
-    }
-    PQ_BUILD(smx->pq, nSmooth, smx->pqHead);
-  } else {
+
+    // Remove everything from the queue. Since the next particle may be
+    // far away from the one we previously processed, a better set of candidates
+    // is likely to be found by starting from the local cell, as smBallSearch will do
+    // when the priority queue is empty.
+    smx->priorityQueue->clear();
+
+
+  } else   {
     // Calculate priority queue using existing particles
     pi = pin;
 
     // Mark - see comment above
     SETSMOOTH(T, pi, 10);
 
     x = GET2<T>(kd->pNumpyPos, p[pi], 0);
     y = GET2<T>(kd->pNumpyPos, p[pi], 1);
     z = GET2<T>(kd->pNumpyPos, p[pi], 2);
 
-    smx->pqHead = NULL;
-    for (pq = smx->pq; pq <= pqLast; ++pq) {
-      pq->ax -= ax;
-      pq->ay -= ay;
-      pq->az -= az;
-      dx = x + pq->ax - GET2<T>(kd->pNumpyPos, p[pq->p], 0);
-      dy = y + pq->ay - GET2<T>(kd->pNumpyPos, p[pq->p], 1);
-      dz = z + pq->az - GET2<T>(kd->pNumpyPos, p[pq->p], 2);
-      pq->fKey = dx * dx + dy * dy + dz * dz;
-    }
-    PQ_BUILD(smx->pq, nSmooth, smx->pqHead);
+    auto priorityQueue = smx->priorityQueue.get();
+
+    priorityQueue->updateDistances([&](PQEntry<T> &entry) {
+      entry.ax -= ax;
+      entry.ay -= ay;
+      entry.az -= az;
+      dx = x + entry.ax - GET2<T>(kd->pNumpyPos, p[entry.getParticleIndex()], 0);
+      dy = y + entry.ay - GET2<T>(kd->pNumpyPos, p[entry.getParticleIndex()], 1);
+      dz = z + entry.az - GET2<T>(kd->pNumpyPos, p[entry.getParticleIndex()], 2);
+      entry.distanceSquared = dx * dx + dy * dy + dz * dz;
+    });
+
+    // Reset anchor coordinates
     ax = 0.0;
     ay = 0.0;
     az = 0.0;
+
+
   }
 
+  // We are now in a situation where the priority queue has a reasonable starting list of candidates for the nearest
+  // neighbours, and we can go ahead and perform a formal search
   for (int j = 0; j < 3; ++j) {
     ri[j] = GET2<T>(kd->pNumpyPos, p[pi], j);
   }
 
-  smBallSearch<T>(smx, smx->pqHead->fKey, ri);
-  SETSMOOTH(T, pi, 0.5 * sqrt(smx->pqHead->fKey));
+  smBallSearch<T>(smx, ri);
+  SETSMOOTH(T, pi, 0.5 * sqrt(smx->priorityQueue->topDistanceSquaredOrMax()));
 
   // p[pi].fSmooth = 0.5*sqrt(smx->pfBall2[pi]);
   /*
   ** Pick next particle, 'pin'.
-  ** Create fList and pList for function 'fncSmooth'.
+  ** Simultaneously create fList (distance info) and pList (particle indexes) for use when sending NN information
+  ** back to python
   */
   pin = pi;
   nCnt = 0;
-  h2 = smx->pqHead->fKey;
-  for (pq = smx->pq; pq <= pqLast; ++pq) {
+  h2 = smx->priorityQueue->topDistanceSquaredOrMax();
 
-    /* the next line is commented out because it results in the furthest
-    particle being excluded from the nearest-neighbor list - this means
-    that although the user requests 32 NN, she would get back 31. By
-    including the furthest particle, the neighbor list is always 32 long */
-
-    // if (pq == smx->pqHead) continue;
+  smx->priorityQueue->iterateHeapEntries([&pin, &h2, &ax, &ay, &az, &nCnt, smx, kd](const PQEntry<T> &entry) {
     if (nCnt >= smx->nListSize) {
       // no room left
       if (!smx->warnings)
         fprintf(stderr, "Smooth - particle cache too small for local density - "
                         "results will be incorrect\n");
       smx->warnings = true;
-      break;
+      return;
+    }
+
+    smx->pList[nCnt] = entry.getParticleIndex();
+    smx->fList[nCnt++] = entry.distanceSquared;
+
+    if (GETSMOOTH(T, entry.getParticleIndex()) >= 0)
+      return; // already done, don't re-do
+
+     // Here we are setting up the next particle to be processed. For best efficiency, choose one which is as close as possible
+    // to the one we just processed.
+    //
+    // One might imagine this would lead to attempting to proces a particle that we very recently processed already.
+    // However in practice checking here that the particle is not already processed seems more expensive than just
+    // processing it again. (It's not clear to me why this should be, it's just empirical.)
+    if (entry.distanceSquared < h2) {
+      pin = entry.getParticleIndex();
+      h2 = entry.distanceSquared;
+      ax = entry.ax;
+      ay = entry.ay;
+      az = entry.az;
+    }
+  });
+
+  smx->pi = pi; // = the particle just processed, for reflection back into python when using nn_next to expose NN info
+  smx->pin = pin; // = particle to be processed when smSmoothStep is next called
+  smx->pNext = pNext; // = particle to start scanning from, if it turns out the next particle doesn't need processing
+  smx->ax = ax; //
+  smx->ay = ay; // = anchor coordinates for wrapping (?)
+  smx->az = az; //
+
+  return nCnt;
+}
+
+
+template <typename T>
+void smSmoothInitStep(SmoothingContext<T> * smx);
+
+template <typename T>
+void smDensitySym(SmoothingContext<T> *, npy_intp, int, bool);
+
+template <typename T>
+void smDensity(SmoothingContext<T> *, npy_intp, int, bool);
+
+template <typename Tf, typename Tq>
+void smMeanQtyND(SmoothingContext<Tf> *, npy_intp, int, bool);
+template <typename Tf, typename Tq>
+void smDispQtyND(SmoothingContext<Tf> *, npy_intp, int, bool);
+template <typename Tf, typename Tq>
+void smMeanQty1D(SmoothingContext<Tf> *, npy_intp, int, bool);
+template <typename Tf, typename Tq>
+void smDispQty1D(SmoothingContext<Tf> *, npy_intp, int, bool);
+template <typename Tf, typename Tq>
+void smDivQty(SmoothingContext<Tf> *, npy_intp, int, bool);
+template <typename Tf, typename Tq>
+void smCurlQty(SmoothingContext<Tf> *, npy_intp, int, bool);
+
+
+template <typename T> T Wendland_kernel(SmoothingContext<T> *, T, int);
+
+template <typename T> T cubicSpline(SmoothingContext<T> *, T);
+
+template <typename Tf> Tf cubicSpline_gradient(Tf, Tf, Tf, Tf);
+
+template <typename Tf> Tf Wendland_gradient(Tf, Tf);
+
+template <typename T> void smDomainDecomposition(KDContext* kd, int nprocs);
+
+
+
+template<typename T>
+void initParticleList(SmoothingContext<T> * smx) {
+  smx->result = std::make_unique<std::vector<npy_intp>>();
+  smx->result->reserve(100000);
+  // not so large that it's expensive to reserve.
+  // Not so small that we constantly need to get more space.
+}
+
+template<typename T>
+PyObject *getReturnParticleList(SmoothingContext<T> * smx) {
+  // make a numpy array from smx->result
+  npy_intp dims[1] = {static_cast<npy_intp>(smx->result->size())};
+  PyObject *numpy_result = PyArray_SimpleNew(1, dims, NPY_INTP);
+
+  std::copy(smx->result->begin(), smx->result->end(),
+            static_cast<long *>(
+                PyArray_DATA(reinterpret_cast<PyArrayObject *>(numpy_result))));
+  smx->result.reset(nullptr);
+
+  return numpy_result;
+}
+
+template<typename T>
+void smSmoothInitStep(SmoothingContext<T>* smx) {
+}
+
+template <typename T> void smDomainDecomposition(KDContext* kd, int nprocs) {
+
+  // AP 31/8/2014 - Here is the domain decomposition for nProcs>1
+  // In principle one should do better by localizing the
+  // domains -- the current approach is a seriously naive decomposition.
+  // This will result in more snake collisions than necessary.
+  // However in practice, up to nCpu = 8, the scaling is looking
+  // pretty linear anyway so I'm leaving that for future.
+
+  // AP 6/4/2024 - revisited this while working on the improved KDTree/smoothing
+  // implementation. It would seem to be more efficient to assign particles to
+  // processors in 'blocks' given that the blocks are roughly spatially coherent.
+  // I have made this change but in practice (as per my comment in 2014!) it seems
+  // to make little difference to the performance. I also wondered whether having
+  // a simpler way for the individual processors to 'scan' for their next particle
+  // might be more efficient than using the smooth array in the way below. But
+  // in practice so little time is spent scanning that this doesn't seem to be
+  // an issue.
+
+  npy_intp pi;
+
+  if (nprocs > 0) {
+    for (pi = 0; pi < kd->nActive; ++pi) {
+      SETSMOOTH(T, pi, -static_cast<T>((pi * nprocs) / kd->nActive) - 1.0);
     }
+  }
+}
 
-    smx->pList[nCnt] = pq->p;
-    smx->fList[nCnt++] = pq->fKey;
+template<typename T>
+void smInitPriorityQueue(SmoothingContext<T> * smx) {
+  /*
+   ** Initialize Priority Queue.
+   */
 
-    if (GETSMOOTH(T, pq->p) >= 0)
-      continue; // already done, don't re-do
 
-    if (pq->fKey < h2) {
-      pin = pq->p;
-      h2 = pq->fKey;
-      ax = pq->ax;
-      ay = pq->ay;
-      az = pq->az;
+  std::cerr << "TEST of STL-based PQ" << std::endl;
+  PriorityQueue<double> myq(5, 20);
+  std::vector<int> particle_number_test =     {5,   0,   1,   10,  2,   3,    4,    6,   7,    8,   11};
+  std::vector<double> particle_distance_test = {0.1, 0.7, 0.3, 2.2, 0.5, 0.6,  0.05, 0.9, 10.2, 1.0, 1.1};
+
+  // iterate over the two lists simultaneously
+  for (auto i = 0; i < particle_number_test.size(); ++i) {
+    myq.push(particle_distance_test[i],particle_number_test[i]);
+    std::cerr << myq.top() << "; " << myq.size() << std::endl;
+    for(auto j = 0; j < 10; ++ j) {
+      std::cerr << (myq.contains(j) ?"*":"o");
     }
+    std::cerr << std::endl;
+  }
+
+  while(!myq.empty()) {
+    myq.pop();
+    std::cerr << myq.top() << "; " << myq.size() << std::endl;
+    for(auto j = 0; j < 10; ++ j) {
+      std::cerr << (myq.contains(j) ?"*":"o");
+    }
+    std::cerr << std::endl;
   }
 
-  smx->pi = pi;
-  smx->pin = pin;
-  smx->pNext = pNext;
-  smx->ax = ax;
-  smx->ay = ay;
-  smx->az = az;
 
-  return nCnt;
 }
 
-template <typename T> T cubicSpline(SMX smx, T r2) {
+
+template <typename T> T cubicSpline(SmoothingContext<T> * smx, T r2) {
   // Cubic Spline Kernel
   T rs;
   rs = 2.0 - sqrt(r2);
-  if (r2 < 1.0)
+  if NPY_UNLIKELY(rs < 0)
+    rs = 0;
+  else if (r2 < 1.0)
     rs = (1.0 - 0.75 * rs * r2);
   else
     rs = 0.25 * rs * rs * rs;
-  if (rs < 0)
-    rs = 0;
   return rs;
 }
 
-template <typename T> T Wendland_kernel(SMX smx, T r2, int nSmooth) {
+template <typename T> T Wendland_kernel(SmoothingContext<T> * smx, T r2, int nSmooth) {
   // Wendland Kernel
+
   T rs;
-  // Dehnen & Aly 2012 correction (1-0.0454684 at Ns=64) /
-  float Wzero = (21 / 16.) * (1 - 0.0294 * pow(nSmooth * 0.01, -0.977));
-  if (r2 <= 0)
-    rs = Wzero;
+
+  if NPY_UNLIKELY(r2 > 4.0)
+    rs = 0;
+  else if NPY_UNLIKELY(r2 == 0.0)
+    rs = (21 / 16.) * (1 - 0.0294 * pow(nSmooth * 0.01, -0.977));
   else {
     T au = sqrt(r2 * 0.25);
-    rs = 1 - au;
-    rs = rs * rs;
-    rs = rs * rs;
+    rs = pow(1 - au, 4);
     rs = (21 / 16.) * rs * (1 + 4 * au);
   }
-  if (rs < 0 && !smx->warnings) {
-    fprintf(stderr, "Internal consistency error\n");
-    smx->warnings = true;
-  }
+
   return rs;
 }
 
+
 template <typename T>
-void smDensitySym(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList,
-                  float *fList, bool Wendland) {
+void smDensitySym(SmoothingContext<T> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   T fNorm, ih2, r2, rs, ih;
   npy_intp i, pj;
   KDContext* kd = smx->kd;
 
   ih = 1.0 / GETSMOOTH(T, pi);
   ih2 = ih * ih;
   fNorm = 0.5 * M_1_PI * ih * ih2;
 
   for (i = 0; i < nSmooth; ++i) {
-    pj = pList[i];
-    r2 = fList[i] * ih2;
+    pj = smx->pList[i];
+    r2 = smx->fList[i] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     ACCUM<T>(kd->pNumpyDen, kd->particleOffsets[pi],
              rs * GET<T>(kd->pNumpyMass, kd->particleOffsets[pj]));
     ACCUM<T>(kd->pNumpyDen, kd->particleOffsets[pj],
              rs * GET<T>(kd->pNumpyMass, kd->particleOffsets[pi]));
   }
 }
 
+
+
+
 template <typename T>
-void smDensity(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList, float *fList,
-               bool Wendland) {
+void smDensity(SmoothingContext<T> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   T fNorm, ih2, r2, rs, ih;
   npy_intp j, pj, pi_iord;
   KDContext* kd = smx->kd;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<T>(kd->pNumpySmooth, pi_iord);
   ih2 = ih * ih;
   fNorm = M_1_PI * ih * ih2;
   SET<T>(kd->pNumpyDen, pi_iord, 0.0);
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     ACCUM<T>(kd->pNumpyDen, pi_iord,
              rs * GET<T>(kd->pNumpyMass, kd->particleOffsets[pj]));
   }
 }
 
+
+
 template <typename Tf, typename Tq>
-void smMeanQty1D(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList,
-                 float *fList, bool Wendland) {
+void smMeanQty1D(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   Tf fNorm, ih2, r2, rs, ih, mass, rho;
   npy_intp j, pj, pi_iord;
   KDContext* kd = smx->kd;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
   ih2 = ih * ih;
   fNorm = M_1_PI * ih * ih2;
 
   SET<Tq>(kd->pNumpyQtySmoothed, pi_iord, 0.0);
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     mass = GET<Tf>(kd->pNumpyMass, kd->particleOffsets[pj]);
     rho = GET<Tf>(kd->pNumpyDen, kd->particleOffsets[pj]);
     ACCUM<Tq>(kd->pNumpyQtySmoothed, pi_iord,
               rs * mass * GET<Tq>(kd->pNumpyQty, kd->particleOffsets[pj]) / rho);
   }
 }
 
 template <typename Tf, typename Tq>
-void smMeanQtyND(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList,
-                 float *fList, bool Wendland) {
+void smMeanQtyND(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   Tf fNorm, ih2, r2, rs, ih, mass, rho;
   npy_intp j, k, pj, pi_iord;
   KDContext* kd = smx->kd;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
   ih2 = ih * ih;
   fNorm = M_1_PI * ih * ih2;
 
   for (k = 0; k < 3; ++k)
     SET2<Tq>(kd->pNumpyQtySmoothed, pi_iord, k, 0.0);
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     mass = GET<Tf>(kd->pNumpyMass, kd->particleOffsets[pj]);
@@ -669,21 +763,22 @@
   Tf rs;
   if (r < 1e-24)
     r = 1e-24; // Fix to avoid dividing by zero in case r = 0.
   // For this case q = 0 and rs = 0 in any case, so we can savely set r to a
   // tiny value.
   if (q < 2.0)
     rs = -5.0 * q * (1.0 - 0.5 * q) * (1.0 - 0.5 * q) * (1.0 - 0.5 * q) / r;
+  else
+    rs = 0.0;
 
   return rs;
 }
 
 template <typename Tf, typename Tq>
-void smCurlQty(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList, float *fList,
-               bool Wendland) {
+void smCurlQty(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   Tf fNorm, ih2, r2, r, rs, q2, q, ih, mass, rho, dqty[3], qty_i[3];
   npy_intp j, k, pj, pi_iord, pj_iord;
   KDContext* kd = smx->kd;
   Tf curl[3], x, y, z, dx, dy, dz;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
@@ -696,21 +791,21 @@
   }
 
   x = GET2<Tf>(kd->pNumpyPos, pi_iord, 0);
   y = GET2<Tf>(kd->pNumpyPos, pi_iord, 1);
   z = GET2<Tf>(kd->pNumpyPos, pi_iord, 2);
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
+    pj = smx->pList[j];
     pj_iord = kd->particleOffsets[pj];
     dx = x - GET2<Tf>(kd->pNumpyPos, pj_iord, 0);
     dy = y - GET2<Tf>(kd->pNumpyPos, pj_iord, 1);
     dz = z - GET2<Tf>(kd->pNumpyPos, pj_iord, 2);
 
-    r2 = fList[j];
+    r2 = smx->fList[j];
     q2 = r2 * ih2;
     r = sqrt(r2);
     q = sqrt(q2);
 
     // Kernel gradient
     if (Wendland) {
       rs = Wendland_gradient(q, r);
@@ -733,16 +828,15 @@
     for (k = 0; k < 3; ++k) {
       ACCUM2<Tq>(kd->pNumpyQtySmoothed, pi_iord, k, rs * curl[k] * mass / rho);
     }
   }
 }
 
 template <typename Tf, typename Tq>
-void smDivQty(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList, float *fList,
-              bool Wendland) {
+void smDivQty(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
   Tf fNorm, ih2, r2, r, rs, q2, q, ih, mass, rho, div, dqty[3], qty_i[3];
   npy_intp j, k, pj, pi_iord, pj_iord;
   KDContext* kd = smx->kd;
   Tf x, y, z, dx, dy, dz;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
@@ -755,21 +849,21 @@
   y = GET2<Tf>(kd->pNumpyPos, pi_iord, 1);
   z = GET2<Tf>(kd->pNumpyPos, pi_iord, 2);
 
   for (k = 0; k < 3; ++k)
     qty_i[k] = GET2<Tq>(kd->pNumpyQty, pi_iord, k);
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
+    pj = smx->pList[j];
     pj_iord = kd->particleOffsets[pj];
     dx = x - GET2<Tf>(kd->pNumpyPos, pj_iord, 0);
     dy = y - GET2<Tf>(kd->pNumpyPos, pj_iord, 1);
     dz = z - GET2<Tf>(kd->pNumpyPos, pj_iord, 2);
 
-    r2 = fList[j];
+    r2 = smx->fList[j];
     q2 = r2 * ih2;
     r = sqrt(r2);
     q = sqrt(q2);
     // Kernel gradient
     if (Wendland) {
       rs = Wendland_gradient(q, r);
     } else {
@@ -787,20 +881,19 @@
     div = dx * dqty[0] + dy * dqty[1] + dz * dqty[2];
 
     ACCUM<Tq>(kd->pNumpyQtySmoothed, pi_iord, rs * div * mass / rho);
   }
 }
 
 template <typename Tf, typename Tq>
-void smDispQtyND(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList,
-                 float *fList, bool Wendland) {
-  float fNorm, ih2, r2, rs, ih, mass, rho;
+void smDispQtyND(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
+  Tf fNorm, ih2, r2, rs, ih, mass, rho;
   npy_intp j, k, pj, pi_iord;
   KDContext* kd = smx->kd;
-  float mean[3], tdiff;
+  Tq mean[3], tdiff;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
   ih2 = ih * ih;
   fNorm = M_1_PI * ih * ih2;
 
   SET<Tq>(kd->pNumpyQtySmoothed, pi_iord, 0.0);
@@ -809,16 +902,16 @@
 
     mean[k] = 0;
   }
 
   // pass 1: find mean
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     mass = GET<Tf>(kd->pNumpyMass, kd->particleOffsets[pj]);
@@ -826,16 +919,16 @@
     for (k = 0; k < 3; ++k)
       mean[k] += rs * mass * GET2<Tq>(kd->pNumpyQty, kd->particleOffsets[pj], k) / rho;
   }
 
   // pass 2: get variance
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     mass = GET<Tf>(kd->pNumpyMass, kd->particleOffsets[pj]);
@@ -850,17 +943,16 @@
   // finally: take square root to get dispersion
 
   SET<Tq>(kd->pNumpyQtySmoothed, pi_iord,
           sqrt(GET<Tq>(kd->pNumpyQtySmoothed, pi_iord)));
 }
 
 template <typename Tf, typename Tq>
-void smDispQty1D(SMX smx, npy_intp pi, int nSmooth, npy_intp *pList,
-                 float *fList, bool Wendland) {
-  float fNorm, ih2, r2, rs, ih, mass, rho;
+void smDispQty1D(SmoothingContext<Tf> * smx, npy_intp pi, int nSmooth, bool Wendland) {
+  Tf fNorm, ih2, r2, rs, ih, mass, rho;
   npy_intp j, pj, pi_iord;
   KDContext* kd = smx->kd;
   Tq mean, tdiff;
 
   pi_iord = kd->particleOffsets[pi];
   ih = 1.0 / GET<Tf>(kd->pNumpySmooth, pi_iord);
   ih2 = ih * ih;
@@ -869,16 +961,16 @@
   SET<Tq>(kd->pNumpyQtySmoothed, pi_iord, 0.0);
 
   mean = 0;
 
   // pass 1: find mean
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
 
     rs *= fNorm;
@@ -886,16 +978,16 @@
     rho = GET<Tf>(kd->pNumpyDen, kd->particleOffsets[pj]);
     mean += rs * mass * GET<Tq>(kd->pNumpyQty, kd->particleOffsets[pj]) / rho;
   }
 
   // pass 2: get variance
 
   for (j = 0; j < nSmooth; ++j) {
-    pj = pList[j];
-    r2 = fList[j] * ih2;
+    pj = smx->pList[j];
+    r2 = smx->fList[j] * ih2;
     if (Wendland) {
       rs = Wendland_kernel(smx, r2, nSmooth);
     } else {
       rs = cubicSpline(smx, r2);
     }
     rs *= fNorm;
     mass = GET<Tf>(kd->pNumpyMass, kd->particleOffsets[pj]);
@@ -905,130 +997,7 @@
   }
 
   // finally: take square root to get dispersion
 
   SET<Tq>(kd->pNumpyQtySmoothed, pi_iord,
           sqrt(GET<Tq>(kd->pNumpyQtySmoothed, pi_iord)));
 }
-
-// instantiate the actual functions that are available:
-
-template void smBallSearch<double>(SMX smx, float fBall2, float *ri);
-
-template void smDomainDecomposition<double>(KDContext* kd, int nprocs);
-
-template npy_intp smSmoothStep<double>(SMX smx, int procid);
-
-template void smDensitySym<double>(SMX smx, npy_intp pi, int nSmooth,
-                                   npy_intp *pList, float *fList,
-                                   bool Wendland);
-
-template void smDensity<double>(SMX smx, npy_intp pi, int nSmooth,
-                                npy_intp *pList, float *fList, bool Wendland);
-
-template void smBallSearch<float>(SMX smx, float fBall2, float *ri);
-
-template void smDomainDecomposition<float>(KDContext* kd, int nprocs);
-
-template npy_intp smSmoothStep<float>(SMX smx, int procid);
-
-template void smDensitySym<float>(SMX smx, npy_intp pi, int nSmooth,
-                                  npy_intp *pList, float *fList, bool Wendland);
-
-template void smDensity<float>(SMX smx, npy_intp pi, int nSmooth,
-                               npy_intp *pList, float *fList, bool Wendland);
-
-template void smMeanQty1D<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                          npy_intp *pList, float *fList,
-                                          bool Wendland);
-
-template void smMeanQtyND<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                          npy_intp *pList, float *fList,
-                                          bool Wendland);
-
-template void smDispQty1D<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                          npy_intp *pList, float *fList,
-                                          bool Wendland);
-
-template void smDispQtyND<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                          npy_intp *pList, float *fList,
-                                          bool Wendland);
-
-template void smCurlQty<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                        npy_intp *pList, float *fList,
-                                        bool Wendland);
-
-template void smDivQty<double, double>(SMX smx, npy_intp pi, int nSmooth,
-                                       npy_intp *pList, float *fList,
-                                       bool Wendland);
-
-template void smMeanQty1D<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smMeanQtyND<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smDispQty1D<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smDispQtyND<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smCurlQty<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                       npy_intp *pList, float *fList,
-                                       bool Wendland);
-
-template void smDivQty<double, float>(SMX smx, npy_intp pi, int nSmooth,
-                                      npy_intp *pList, float *fList,
-                                      bool Wendland);
-
-template void smMeanQty1D<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smMeanQtyND<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smDispQty1D<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smDispQtyND<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                         npy_intp *pList, float *fList,
-                                         bool Wendland);
-
-template void smCurlQty<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                       npy_intp *pList, float *fList,
-                                       bool Wendland);
-
-template void smDivQty<float, double>(SMX smx, npy_intp pi, int nSmooth,
-                                      npy_intp *pList, float *fList,
-                                      bool Wendland);
-
-template void smMeanQty1D<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                        npy_intp *pList, float *fList,
-                                        bool Wendland);
-
-template void smMeanQtyND<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                        npy_intp *pList, float *fList,
-                                        bool Wendland);
-
-template void smDispQty1D<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                        npy_intp *pList, float *fList,
-                                        bool Wendland);
-
-template void smDispQtyND<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                        npy_intp *pList, float *fList,
-                                        bool Wendland);
-
-template void smCurlQty<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                      npy_intp *pList, float *fList,
-                                      bool Wendland);
-
-template void smDivQty<float, float>(SMX smx, npy_intp pi, int nSmooth,
-                                     npy_intp *pList, float *fList,
-                                     bool Wendland);
```

### Comparing `pynbody-2.0.0b5/pynbody/plot/__init__.py` & `pynbody-2.0.0b7/pynbody/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/gas.py` & `pynbody-2.0.0b7/pynbody/plot/gas.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/generic.py` & `pynbody-2.0.0b7/pynbody/plot/generic.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/metals.py` & `pynbody-2.0.0b7/pynbody/plot/metals.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/profile.py` & `pynbody-2.0.0b7/pynbody/plot/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/sph.py` & `pynbody-2.0.0b7/pynbody/plot/sph.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/stars.py` & `pynbody-2.0.0b7/pynbody/plot/stars.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/plot/util.py` & `pynbody-2.0.0b7/pynbody/plot/util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/simdict.py` & `pynbody-2.0.0b7/pynbody/simdict.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/__init__.py` & `pynbody-2.0.0b7/pynbody/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/ascii.py` & `pynbody-2.0.0b7/pynbody/snapshot/ascii.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/copy_on_access.py` & `pynbody-2.0.0b7/pynbody/snapshot/copy_on_access.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/gadget.py` & `pynbody-2.0.0b7/pynbody/snapshot/gadget.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,17 +952,17 @@
 
     @classmethod
     def _can_load(cls, f: pathlib.Path):
         """Check whether we can load the file as Gadget format by reading
         the first 4 bytes"""
         fname = f
         if not f.exists():
-            if not f.with_suffix(".0").exists():
+            fname = f.parent / (f.name + ".0")
+            if not fname.exists():
                 return False
-            fname = f.with_suffix(".0")
 
         with open(fname, "br") as fd:
             r, = struct.unpack('=I', fd.read(4))
 
         # First int32 is 8 for a Gadget 2 file, or 256 for Gadget 1, or the
         # byte swapped equivalent.
         if r in (8, 134217728, 65536, 256):
```

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/gadgethdf.py` & `pynbody-2.0.0b7/pynbody/snapshot/gadgethdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,22 +83,25 @@
         filename = str(filename)
         self._mode = mode
         if h5py.is_hdf5(filename):
             self._filenames = [filename]
             self._numfiles = 1
         else:
             h1 = h5py.File(filename + ".0.hdf5", mode)
-            self._numfiles = h1[self._nfiles_groupname].attrs[self._nfiles_attrname]
+            self._numfiles = self._get_num_files(h1)
             if hasattr(self._numfiles, "__len__"):
                 assert len(self._numfiles) == 1
                 self._numfiles = self._numfiles[0]
             self._filenames = [filename+"."+str(i)+".hdf5" for i in range(self._numfiles)]
 
         self._open_files = {}
 
+    def _get_num_files(self, first_file):
+        return first_file[self._nfiles_groupname].attrs[self._nfiles_attrname]
+
     def __len__(self):
         return self._numfiles
 
     def __iter__(self) :
         for i in range(self._numfiles) :
             if i not in self._open_files:
                 self._open_files[i] = h5py.File(self._filenames[i], self._mode)
@@ -492,14 +495,16 @@
             else:
                 target[array_name].set_default_units()
 
             for loading_fam in all_fams_to_load:
                 i0 = 0
                 for hdf in self._all_hdf_groups_in_family(loading_fam):
                     npart = hdf['ParticleIDs'].size
+                    if npart == 0:
+                        continue
                     i1 = i0+npart
 
                     dataset = self._get_hdf_dataset(hdf, translated_name)
 
                     target_array = self[loading_fam][array_name][i0:i1]
                     assert target_array.size == dataset.size
```

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/grafic.py` & `pynbody-2.0.0b7/pynbody/snapshot/grafic.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/namemapper.py` & `pynbody-2.0.0b7/pynbody/snapshot/namemapper.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/nchilada.py` & `pynbody-2.0.0b7/pynbody/snapshot/nchilada.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/ramses.py` & `pynbody-2.0.0b7/pynbody/snapshot/ramses.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,16 @@
 
         self._timestep_id = _timestep_id(dirname)
         self._filename = dirname
         if os.path.isdir(dirname):
             self._dirname = dirname
         else:
             self._dirname = os.path.split(dirname)[0]
+        self._translate_array_name = namemapper.AdaptiveNameMapper('ramses-name-mapping')
+
         self._load_sink_data_to_temporary_store()
         self._load_infofile()
         self._load_namelistfile()
         self._setup_particle_descriptor()
 
         assert self._info['ndim'] <= 3
         if self._info['ndim'] < 3:
@@ -585,15 +587,14 @@
             self._guess_particle_descriptor()
         self._has_explicit_particle_families = 'family' in self._particle_blocks
 
     def _load_particle_descriptor(self):
         with open(os.path.join(self._filename, "part_file_descriptor.txt")) as f:
             self._particle_blocks = []
             self._particle_types = []
-            self._translate_array_name = namemapper.AdaptiveNameMapper('ramses-name-mapping')
             for line in f:
                 if not line.startswith("#"):
                     ivar, name, dtype = list(map(str.strip,line.split(",")))
                     self._particle_blocks.append(self._translate_array_name(name, reverse=True))
                     self._particle_types.append(dtype)
             self._particle_blocks_are_explictly_known = True
 
@@ -746,15 +747,16 @@
             return
 
         self._fix_fortran_missing_exponent(data)
 
         column_names[0] = column_names[0][1:].strip()
         dimensions[0] = dimensions[0][1:].strip()
 
-        self._sink_column_names = column_names
+        self._sink_column_names = [self._translate_array_name(c, reverse=True)
+                                   for c in column_names]
         self._sink_dimensions = dimensions
         self._sink_data = data
 
     def _after_load_sink_data_failure(self, warn=True):
         if warn:
             warnings.warn("Unexpected format in file %s -- sink data has not been loaded" % self._sink_filename())
 
@@ -1156,14 +1158,22 @@
             elif array_name in self._rt_blocks_3d:
                 warnings.warn("Loading RT data from disk. Photon densities are stored in flux units by Ramses and need "
                               "to be multiplied by the reduced speed of light of the run to obtain a physical number. "
                               "This is currently left to the user, see issue 542 for more discussion.")
                 self._load_gas_vars(_gv_load_rt)
                 for u_block in self._rt_blocks_3d:
                     self[fam][u_block].units = self._rt_unit
+            elif array_name == 'mass':
+                # Very special case. If 'mass' has been created already for particle blocks (or sink blocks), and the
+                # user requests it across the whole simulation, the SimSnap framework will issue this request rather
+                # than a request to load across all families (handled below). If we raise an exception, the user
+                # will see a confusing message about mass being unavailable for gas. So instead we redirect this to
+                # a derived array, which will result in a full mass array being returned (good) and a warning about
+                # conjoining derived and non-derived arrays (logical, at least).
+                self._derive_array('mass', fam)
             else:
                 raise OSError("No such array on disk")
         elif fam is None and array_name in ['pos', 'vel']:
             # synchronized loading of pos/vel information
             if 'pos' not in self:
                 self._create_array('pos', 3)
             if 'vel' not in self:
@@ -1176,17 +1186,23 @@
                 self._load_gas_vars()
 
             # the below triggers loading ALL particles, not just DM
             for name in 'x','y','z','vx','vy','vz':
                 self._load_particle_block(name)
 
         elif fam is None and array_name == 'mass':
+            # mass has to be handled separately because it is present as a particle block
+            # but not as a gas block -- there it will be derived. It is also present as a sink block,
+            # which is again handled differently. So somehow we need to bring all of this together in
+            # a way which doesn't baffle users.
+
             self._create_array('mass')
             self._load_particle_block('mass')
             self['mass'].set_default_units()
+
             if len(self.gas) > 0:
                 gasmass = mass(self.gas)
                 gasmass.convert_units(self['mass'].units)
                 self.gas['mass'] = gasmass
         else:
             raise OSError("No such array on disk")
```

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/simsnap.py` & `pynbody-2.0.0b7/pynbody/snapshot/simsnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,36 +335,50 @@
     def _get_subsnap_from_mask_array(self,mask_array):
         if len(mask_array.shape) > 1 or mask_array.shape[0] > len(self):
             raise ValueError("Incorrect shape for masking array")
         else:
             return self[np.where(mask_array)]
 
     def _get_array_with_lazy_actions(self, name):
-
+        """Get an array by the given name; if it's not available, attempt to load or derive it first"""
         if name in list(self.keys()):
             self._dependency_tracker.touching(name)
 
             # Ensure that any underlying dependencies on 1D positions and velocities
             # are forwarded to 3D dependencies as well
             nd_name = self._array_name_1D_to_ND(name)
             if nd_name is not None:
                 self._dependency_tracker.touching(nd_name)
 
-            return self._get_array(name)
-
-        with self._dependency_tracker.calculating(name):
+        elif not self.lazy_off:
+            # The array is not currently in memory at the level we need it, and there is a possibility
+            # of getting it into memory using lazy derivation or loading. First, if there is a family level
+            # array by the same name, dispose of it. (Note if this is being called on a FamilySubSnap, the below
+            # has no effect, and anyway we wouldn't reach this point in the code if the family array were available.)
             self.__resolve_obscuring_family_array(name)
 
-            if not self.lazy_off:
-                if not self.lazy_load_off:
-                    self.__load_if_required(name)
-                if not self.lazy_derive_off:
+            # Now, we'll try to load the array...
+            did_load = False
+            if not self.lazy_load_off:
+                # Note that we don't want this to be inside _dependency_tracker.calculating(name), because there is a
+                # small possibility the load will be mapped into a derivation by the loader class. Specifically this
+                # happens in ramses snapshots for the mass array (which is derived from the density array for gas cells).
+                self.__load_if_required(name)
+
+            if name in self:
+                # We managed to load it. Note the dependency.
+                self._dependency_tracker.touching(name)
+            elif not self.lazy_derive_off:
+                # Try deriving instead
+                with self._dependency_tracker.calculating(name):
                     self.__derive_if_required(name)
 
-            return self._get_array(name)
+        # At this point we've done everything we can to get the array into memory. If it's still not there, we'll
+        # get a KeyError from the below.
+        return self._get_array(name)
 
 
 
     def __load_if_required(self, name):
         if name not in list(self.keys()):
             try:
                 self.__load_array_and_perform_postprocessing(name)
@@ -372,14 +386,20 @@
                 pass
 
     def __derive_if_required(self, name):
         if name not in list(self.keys()):
             self._derive_array(name)
 
     def __resolve_obscuring_family_array(self, name):
+        """When a lazy derive or lazy load is about to happen for array given by name, deal with family arrays by the same name
+
+        Note that if this is being called from a family subview, family_keys() returns an empty set by definition, so
+        nothing bad happens. It is when a derivation/lazy-load is attempted across the snapshot that having family arrays
+        of the same name might get in the way.
+        """
         if name in self.family_keys():
             self.__remove_family_array_if_derived(name)
 
         if name in self.family_keys():
             self.__load_remaining_families_if_loadable(name)
 
         if name in self.family_keys():
@@ -403,15 +423,16 @@
             del self.ancestor[name]
 
 
     def __load_remaining_families_if_loadable(self, name):
         in_fam, out_fam = self.__get_included_and_excluded_families_for_array(name)
         try:
             for fam in out_fam:
-                self.__load_array_and_perform_postprocessing(name, fam=fam)
+                if name not in self[fam]: # (check again, in case it was created in the meantime)
+                    self.__load_array_and_perform_postprocessing(name, fam=fam)
         except OSError:
             pass
 
 
 
     def _get_persist(self, hash, name):
         try:
@@ -481,15 +502,15 @@
     ############################################
     def keys(self):
         """Return the directly accessible array names (in memory)"""
         return list(self._arrays.keys())
 
     def has_key(self, name):
         """Returns True if the array name is accessible (in memory)"""
-        return name in list(self.keys())
+        return name in self.keys()
 
     def values(self):
         """Returns a list of the actual arrays in memory"""
         x = []
         for k in list(self.keys()):
             x.append(self[k])
         return x
@@ -873,25 +894,26 @@
 
             # Find out what was loaded
             new_keys = set(anc.keys()) - pre_keys
             new_fam_keys = fk()
             for fami in new_fam_keys:
                 new_fam_keys[fami] = new_fam_keys[fami] - pre_fam_keys[fami]
 
-            # If the loader hasn't given units already, try to determine the defaults
-            # Then, attempt to convert what was loaded into friendly units
-            for v in new_keys:
-                if not units.has_units(anc[v]):
-                    anc[v].units = anc._default_units_for(v)
-                anc._autoconvert_array_unit(anc[v])
-            for f, vals in new_fam_keys.items():
-                for v in vals:
-                    if not units.has_units(anc[f][v]):
-                        anc[f][v].units = anc._default_units_for(v)
-                    anc._autoconvert_array_unit(anc[f][v])
+            with self.lazy_off:
+                # If the loader hasn't given units already, try to determine the defaults
+                # Then, attempt to convert what was loaded into friendly units
+                for v in new_keys:
+                    if not units.has_units(anc[v]):
+                        anc[v].units = anc._default_units_for(v)
+                    anc._autoconvert_array_unit(anc[v])
+                for f, vals in new_fam_keys.items():
+                    for v in vals:
+                        if not units.has_units(anc[f][v]):
+                            anc[f][v].units = anc._default_units_for(v)
+                        anc._autoconvert_array_unit(anc[f][v])
 
 
 
     ############################################
     # VECTOR TRANSFORMATIONS OF THE SNAPSHOT
     ############################################
     def transform(self, matrix):
@@ -1230,20 +1252,22 @@
             hx = hash(name)
             if hx not in cache:
                 cache[hx] = fn()
 
         return cache[hx]
 
     def _get_array(self, name, index=None, always_writable=False):
-        """Get the array of the specified *name*, optionally
-        for only the particles specified by *index*.
+        """Get the array of the specified *name*, optionally for only the particles specified by *index*.
 
-        If *always_writable* is True, the returned array is
-        writable. Otherwise, it is still normally writable, but
-        not if the array is flagged as derived by the framework."""
+        If *always_writable* is True, the returned array is writable. Otherwise, it is still normally writable, but
+        not if the array is flagged as derived by the framework.
+
+        Note that this routine never calls any lazy loading/derivation routines, for which one needs to call
+        _get_array_with_lazy_actions.
+        """
 
         x = self._arrays[name]
         if x.derived and not always_writable:
             x = x.view()
             x.flags['WRITEABLE'] = False
 
         if index is not None:
@@ -1262,14 +1286,17 @@
         """Get the family-level array with specified *name* for the family *fam*,
         optionally for only the particles specified by *index* (relative to the
         family slice).
 
         If *always_writable* is True, the returned array is writable. Otherwise
         it is still normally writable, but not if the array is flagged as derived
         by the framework.
+
+        Note that this routine never calls any lazy loading/derivation routines, for which one needs to call
+        _get_array_with_lazy_actions on the FamilySubSnap returned by self[fam].
         """
 
         try:
             x = self._family_arrays[name][fam]
         except KeyError:
             raise KeyError("No array " + name + " for family " + fam.name) from None
```

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/subsnap.py` & `pynbody-2.0.0b7/pynbody/snapshot/subsnap.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/swift.py` & `pynbody-2.0.0b7/pynbody/snapshot/swift.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/tipsy.py` & `pynbody-2.0.0b7/pynbody/snapshot/tipsy.py`

 * *Files 2% similar despite different names*

```diff
@@ -779,21 +779,21 @@
                          'xform', 'yform', 'zform', 'vxform', 'vyform', 'vzform',
                          'posform', 'velform','h2form']
         # if massform available as auxiliary array, faster to load it instead
         if array_name == 'massform' and 'massform' not in self.loadable_keys():
             starlog_keys += ['massform']
 
         if filename is None and array_name in starlog_keys:
-
             try:
                 self.read_starlog()
-                if fam is not None:
-                    return self[fam][array_name]
-                else:
-                    return self[array_name]
+                with self.lazy_off:
+                    if fam is not None:
+                        return self[fam][array_name]
+                    else:
+                        return self[array_name]
             except OSError:
                 pass
 
         # N.B. this code is a bit inefficient for loading
         # family-specific arrays, because it reads in the whole array
         # then slices it.  But of course the memory is only wasted
         # while still inside this routine, so it's only really the
@@ -903,39 +903,40 @@
         done = False
         filename = None
         x = os.path.dirname(x)
         # Attempt the loading of information
         l = glob.glob(os.path.join(x, "*.starlog"))
         if (len(l)):
             for filename in l:
-                sl = StarLog(filename)
+                starlog = StarLog(filename)
         else:
             l = glob.glob(os.path.join(x, "../*.starlog"))
             if (len(l) == 0):
                 raise OSError("Couldn't find starlog file")
             for filename in l:
-                sl = StarLog(filename)
+                starlog = StarLog(filename)
 
         logger.info("Bridging starlog into SimSnap")
-        b = pynbody.bridge.OrderBridge(self, sl)
-        b(b(b(sl))).star['iorderGas'] = b(b(sl)).star['iorderGas']
-        b(b(b(sl))).star['massform'] = b(b(sl)).star['massform']
-        b(b(b(sl))).star['rhoform'] = b(b(sl)).star['rhoform']
-        b(b(b(sl))).star['tempform'] = b(b(sl)).star['tempform']
-        b(b(b(sl)))['posform'] = b(b(sl))['pos']
-        b(b(b(sl)))['velform'] = b(b(sl))['vel']
-        #b(sl).star['iorderGas'] = sl.star['iorderGas'][:len(self.star)]
-        #b(sl).star['massform'] = sl.star['massform'][:len(self.star)]
-        #b(sl).star['rhoform'] = sl.star['rhoform'][:len(self.star)]
-        #b(sl).star['tempform'] = sl.star['tempform'][:len(self.star)]
-        #b(sl)['posform'] = sl['pos'][:len(self.star), :]
-        #b(sl)['velform'] = sl['vel'][:len(self.star), :]
-        if 'h2form' in list(sl.star.keys()):
-            b(b(b(sl))).star['h2form'] = b(b(sl)).star['h2form']
-        else: print("No H2 data found in StarLog file")
+        b = pynbody.bridge.OrderBridge(self, starlog)
+
+        source = b(b(starlog))
+        dest = b(source)
+
+        dest.star['iorderGas'] = source.star['iorderGas']
+        dest.star['massform'] = source.star['massform']
+        dest.star['rhoform'] = source.star['rhoform']
+        dest.star['tempform'] = source.star['tempform']
+        dest['posform'] = source['pos']
+        dest['velform'] = source['vel']
+
+        if 'h2form' in list(starlog.star.keys()):
+            dest.star['h2form'] = source.star['h2form']
+        else:
+            logger.info("No H2 data found in StarLog file")
+
         for i, x in enumerate(['x', 'y', 'z']):
             self._arrays[x + 'form'] = self['posform'][:, i]
         for i, x in enumerate(['vx', 'vy', 'vz']):
             self._arrays[x + 'form'] = self['velform'][:, i]
 
     @classmethod
     def _can_load(cls, f):
```

### Comparing `pynbody-2.0.0b5/pynbody/snapshot/util.py` & `pynbody-2.0.0b7/pynbody/snapshot/util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/sph/__init__.py` & `pynbody-2.0.0b7/pynbody/sph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     logger.info('Smoothing with %d nearest neighbours' %
                 config['sph']['smooth-particles'])
 
     sm = array.SimArray(np.empty(len(self['pos']), dtype=self['pos'].dtype), self['pos'].units)
 
     start = time.time()
     self.kdtree.set_array_ref('smooth',sm)
-    self.kdtree.populate('hsm', config['sph']['smooth-particles'], config['sph']['Kernel'])
+    self.kdtree.populate('hsm', config['sph']['smooth-particles'])
     end = time.time()
 
     logger.info('Smoothing done in %5.3gs' % (end - start))
     self._kdtree_derived_smoothing = True
     return sm
 
 def _get_smooth_array_ensuring_compatibility(self):
@@ -101,15 +101,15 @@
     start = time.time()
 
 
     self.kdtree.set_array_ref('smooth',_get_smooth_array_ensuring_compatibility(self))
     self.kdtree.set_array_ref('mass',self['mass'])
     self.kdtree.set_array_ref('rho',rho)
 
-    self.kdtree.populate('rho', config['sph']['smooth-particles'], config['sph']['Kernel'])
+    self.kdtree.populate('rho', config['sph']['smooth-particles'])
 
     end = time.time()
     logger.info('Density calculation done in %5.3g s' % (end - start))
 
     return rho
```

### Comparing `pynbody-2.0.0b5/pynbody/sph/_render.pyx` & `pynbody-2.0.0b7/pynbody/sph/_render.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/test_utils/gadget4_subfind_reader.py` & `pynbody-2.0.0b7/pynbody/test_utils/gadget4_subfind_reader.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/test_utils/pyread_gadget_hdf5.py` & `pynbody-2.0.0b7/pynbody/test_utils/pyread_gadget_hdf5.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/transformation.py` & `pynbody-2.0.0b7/pynbody/transformation.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/units.py` & `pynbody-2.0.0b7/pynbody/units.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/pynbody/util.py` & `pynbody-2.0.0b7/pynbody/util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import threading
 import time
 import warnings
 from typing import Union
 
 import numpy as np
 
-from . import units
-from .array import SimArray
+from .. import units
+from ..array import SimArray
 
 logger = logging.getLogger('pynbody.util')
 from ._util import *
 
 
 def open_(filename: str | pathlib.Path, *args):
     """Open a file, determining from the filename whether to use
```

### Comparing `pynbody-2.0.0b5/pynbody.egg-info/PKG-INFO` & `pynbody-2.0.0b7/pynbody.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b5
+Version: 2.0.0b7
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b5/pynbody.egg-info/SOURCES.txt` & `pynbody-2.0.0b7/pynbody.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,25 +45,23 @@
 docs/tutorials/example_code/do_preamble.py
 docs/tutorials/example_code/rcs.py
 docs/tutorials/example_code/rotcurve.py
 docs/tutorials/example_code/star_render.py
 docs/tutorials/example_code/temperature_slice.py
 docs/tutorials/example_code/velocity_vectors.py
 pynbody/__init__.py
-pynbody/_util.pyx
 pynbody/configuration.py
 pynbody/default_config.ini
 pynbody/dependencytracker.py
 pynbody/derived.py
 pynbody/family.py
 pynbody/iter_subclasses.py
 pynbody/simdict.py
 pynbody/transformation.py
 pynbody/units.py
-pynbody/util.py
 pynbody.egg-info/PKG-INFO
 pynbody.egg-info/SOURCES.txt
 pynbody.egg-info/dependency_links.txt
 pynbody.egg-info/requires.txt
 pynbody.egg-info/top_level.txt
 pynbody/analysis/CAMB_WMAP7
 pynbody/analysis/__init__.py
@@ -129,14 +127,15 @@
 pynbody/halo/details/iord_mapping.py
 pynbody/halo/details/number_mapping.py
 pynbody/halo/details/particle_indices.py
 pynbody/kdtree/__init__.py
 pynbody/kdtree/kd.cpp
 pynbody/kdtree/kd.h
 pynbody/kdtree/kdmain.cpp
+pynbody/kdtree/pq.h
 pynbody/kdtree/smooth.cpp
 pynbody/kdtree/smooth.h
 pynbody/openmp/openmp_null.pyx
 pynbody/openmp/openmp_real.pyx
 pynbody/plot/__init__.py
 pynbody/plot/gas.py
 pynbody/plot/generic.py
@@ -161,14 +160,17 @@
 pynbody/snapshot/tipsy.py
 pynbody/snapshot/util.py
 pynbody/sph/__init__.py
 pynbody/sph/_render.pyx
 pynbody/test_utils/__init__.py
 pynbody/test_utils/gadget4_subfind_reader.py
 pynbody/test_utils/pyread_gadget_hdf5.py
+pynbody/util/__init__.py
+pynbody/util/_util.pyx
+pynbody/util/hdf_vds.py
 tests/adaptahop_test.py
 tests/ahf_halos_test.py
 tests/array_test.py
 tests/bridge_test.py
 tests/copy_on_access_test.py
 tests/cosmology_test.py
 tests/derived_arrays_test.py
```

### Comparing `pynbody-2.0.0b5/pyproject.toml` & `pynbody-2.0.0b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/setup.py` & `pynbody-2.0.0b7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,24 @@
 ext_modules = []
 libraries=[ ]
 extra_compile_args = ['-ftree-vectorize',
                       '-fno-omit-frame-pointer',
                       '-funroll-loops',
                       '-fprefetch-loop-arrays',
                       '-fstrict-aliasing',
+                      '-fno-expensive-optimizations', #<-- for arm64 gcc
                       '-g', '-std=c++14']
 
+# note on -fno-expensive-optimizations:
+# This is needed for arm64 gcc, which otherwise gets wrong results for a small number of particles
+# in the kdtree_test.py::test_smooth_wendlandC2 test. It's unclear why; quite possibly there is
+# a subtle bug in the code exposed by these optimizations, but it is such a vague optimization
+# that it's hard to know what it is. The actual routine affected is smBallGather, but for some reason
+# its impact only shows up with the Wendland kernel.
+
 extra_link_args = openmp_args + ['-std=c++14']
 
 if xcode_fix_needed():
     # workaround for XCode bug FB13097713
     # https://developer.apple.com/documentation/xcode-release-notes/xcode-15-release-notes#Linking
     extra_link_args += ['-Wl,-ld_classic']
 
@@ -104,16 +112,16 @@
                      extra_compile_args=openmp_args,
                      extra_link_args=extra_link_args)
 
 bridge_pyx = Extension('pynbody.bridge._bridge',
                      sources=['pynbody/bridge/_bridge.pyx'],
                      include_dirs=incdir)
 
-util_pyx = Extension('pynbody._util',
-                     sources=['pynbody/_util.pyx'],
+util_pyx = Extension('pynbody.util._util',
+                     sources=['pynbody/util/_util.pyx'],
                      include_dirs=incdir,
                      extra_compile_args=openmp_args,
                      extra_link_args=extra_link_args)
 
 filt_geom_pyx = Extension('pynbody.filt.geometry_selection',
                      sources=['pynbody/filt/geometry_selection.pyx'],
                      include_dirs=incdir,
@@ -137,15 +145,16 @@
                 cython_fortran_file, interpolate3d_pyx, omp_commands]
 
 install_requires = [
     'cython>=0.20',
     'h5py>=3.0.0',
     'matplotlib>=3.0.0',
     'numpy>=1.21.6',
-    'scipy>=1.0.0'
+    'scipy>=1.0.0',
+    'posix-ipc>=1.1.0'
 ]
 
 tests_require = [
     'pytest','pandas'
 ]
 
 docs_require = [
@@ -176,15 +185,15 @@
       version = get_version("pynbody/__init__.py"),
       description = 'Light-weight astronomical N-body/SPH analysis for python',
       url = 'https://github.com/pynbody/pynbody/releases',
       package_dir = {'pynbody/': ''},
       packages = ['pynbody', 'pynbody/analysis', 'pynbody/bc_modules', 'pynbody/array',
                   'pynbody/plot', 'pynbody/gravity', 'pynbody/chunk', 'pynbody/filt', 'pynbody/sph',
                   'pynbody/snapshot', 'pynbody/bridge', 'pynbody/halo', 'pynbody/halo/details',
-                  'pynbody/extern', 'pynbody/kdtree', 'pynbody/test_utils'],
+                  'pynbody/extern', 'pynbody/kdtree', 'pynbody/test_utils', 'pynbody/util'],
       package_data={'pynbody': ['default_config.ini'],
                     'pynbody/analysis': ['cmdlum.npz',
                                          'h1.hdf5',
                                          'ionfracs.npz',
                                          'CAMB_WMAP7',
                                          'cambtemplate.ini'],
                     'pynbody/plot': ['tollerud2008mw']},
```

### Comparing `pynbody-2.0.0b5/tests/adaptahop_test.py` & `pynbody-2.0.0b7/tests/adaptahop_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,7 +228,24 @@
 
 def test_halo_iteration(halos):
     h = list(halos)
 
     assert len(h) == len(halos)
     assert h[0] is halos[1]
     assert h[-1] is halos[len(halos)]
+
+def test_dm_not_first_family(f):
+    # AdaptaHOP files only refer to DM particles, but we can't assume that DM is the first family
+    # e.g. tracer particles come first
+
+    f = pynbody.load("testdata/new_adaptahop_output_00080")
+    f_with_tracers = pynbody.new(gas_tracer=100, dm=len(f.dm), star=len(f.star), gas=len(f.gas))
+    f_with_tracers.dm['iord'] = f.dm['iord']
+    f_with_tracers.properties.update(f.properties)
+
+    halos = f.halos()
+
+    halos2 = pynbody.halo.adaptahop.NewAdaptaHOPCatalogue(f_with_tracers,
+                                 fname = "testdata/new_adaptahop_output_00080/Halos/tree_bricks080")
+
+    assert (halos2[1].dm['iord'] == halos[1].dm['iord']).all()
+    assert (halos2[2].dm['iord'] == halos[2].dm['iord']).all()
```

### Comparing `pynbody-2.0.0b5/tests/ahf_halos_test.py` & `pynbody-2.0.0b7/tests/ahf_halos_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,32 +21,41 @@
 
 
 def test_load_ahf_catalogue():
     f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
     h = pynbody.halo.ahf.AHFCatalogue(f)
     assert len(h)==1411
 
+h0_sample_iords = [57, 27875, 54094, 82969, 112002, 140143, 173567, 205840, 264606,
+           301694, 333383, 358730, 374767, 402300, 430180, 456015, 479885, 496606,
+           519824, 539971, 555195, 575204, 596047, 617669, 652724, 1533992, 1544021,
+           1554045, 1564080, 1574107, 1584130, 1594158, 1604204, 1614257, 1624308, 1634376,
+           1644485, 1654580, 1664698, 1674831, 1685054, 1695252, 1705513, 1715722, 1725900,
+           1736070, 1746235, 1756400, 1766584, 1776754, 1786886]
+
 @pytest.mark.parametrize("do_load_all", [True, False])
 def test_ahf_particles(do_load_all, cleanup_fpos_file):
     f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
     h = pynbody.halo.ahf.AHFCatalogue(f)
 
     if do_load_all:
         h.load_all()
 
     assert len(h[0])==502300
-    assert (h[0]['iord'][::10000]==[57, 27875, 54094, 82969, 112002, 140143, 173567, 205840, 264606,
-           301694, 333383, 358730, 374767, 402300, 430180, 456015, 479885, 496606,
-           519824, 539971, 555195, 575204, 596047, 617669, 652724, 1533992, 1544021,
-           1554045, 1564080, 1574107, 1584130, 1594158, 1604204, 1614257, 1624308, 1634376,
-           1644485, 1654580, 1664698, 1674831, 1685054, 1695252, 1705513, 1715722, 1725900,
-           1736070, 1746235, 1756400, 1766584, 1776754, 1786886]).all()
+    assert h[0].ancestor is f
+    assert (h[0]['iord'][::10000]==h0_sample_iords).all()
     assert len(h[19])==3272
     assert(h[19]['iord'][::1000] == [232964, 341019, 752354, 793468]).all()
 
+def test_load_copy():
+    f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
+    h = pynbody.halo.ahf.AHFCatalogue(f)
+    hcopy = h.load_copy(0)
+    assert (hcopy['iord'][::10000] == h0_sample_iords).all()
+    assert hcopy.ancestor is not f
 
 @pytest.mark.parametrize("do_load_all", [True, False])
 def test_load_ahf_catalogue_non_gzipped(do_load_all):
     for extension in ["halos", "particles", "substructure"]:
         subprocess.call(["gunzip",f"testdata/gasoline_ahf/g15784.lr.01024.z0.000.AHF_{extension}.gz"])
     try:
         f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
```

### Comparing `pynbody-2.0.0b5/tests/array_test.py` & `pynbody-2.0.0b7/tests/array_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,84 +197,91 @@
 
 def test_shared_arrays():
     import gc
 
     import pynbody.array as pyn_array
 
     gc.collect() # this is to start with a clean slate, get rid of any shared arrays that might be hanging around
-    baseline_num_shared_arrays = pyn_array.shared.get_num_shared_arrays() # hopefully zero, but we can't guarantee that
+    baseline_num_shared_arrays = pyn_array.shared.get_num_shared_arrays_owned() # hopefully zero, but we can't guarantee that
 
     ar = pyn_array._array_factory((3,5), dtype=np.float32, zeros=True, shared=True)
 
     assert ar.shape == (3,5)
     assert (ar == 0.0).all()
 
     ar[:] = np.arange(3)[: , np.newaxis] * np.arange(5)[np.newaxis, :]
 
     # now let's see if we can transfer it to another process:
 
     import multiprocessing as mp
-    p = mp.Process(target=_test_and_alter_shared_value, args=(pyn_array.shared._shared_array_deconstruct(ar),))
+    context = mp.get_context('spawn')
+    p = context.Process(target=_test_and_alter_shared_value, args=(pyn_array.shared._shared_array_deconstruct(ar),))
     p.start()
     p.join()
 
     # check that the other process has successfully changed our value:
     assert (ar[:] ==  np.arange(3)[:, np.newaxis] ).all()
 
-    assert pyn_array.shared.get_num_shared_arrays() == 1 + baseline_num_shared_arrays
+    assert pyn_array.shared.get_num_shared_arrays_owned() == 1 + baseline_num_shared_arrays
 
     ar2 = pyn_array._array_factory((3,5), dtype=np.float32, zeros=True, shared=True)
-    assert pyn_array.shared.get_num_shared_arrays() == 2 + baseline_num_shared_arrays
+    assert pyn_array.shared.get_num_shared_arrays_owned() == 2 + baseline_num_shared_arrays
 
     del ar, ar2
     gc.collect()
 
-    assert pyn_array.shared.get_num_shared_arrays() == baseline_num_shared_arrays
+    assert pyn_array.shared.get_num_shared_arrays_owned() == baseline_num_shared_arrays
 
+@pytest.fixture
+def clean_up_test_protection():
+    import posix_ipc
+    try:
+        posix_ipc.unlink_shared_memory("pynbody-test-cleanup")
+    except posix_ipc.ExistentialError:
+        pass
+    yield
+    try:
+        posix_ipc.unlink_shared_memory("pynbody-test-cleanup")
+    except posix_ipc.ExistentialError:
+        pass
 
 def _test_shared_arrays_cleaned_on_exit():
     global ar
     ar = shared.make_shared_array((10,), dtype=np.int32, zeros=True, fname="pynbody-test-cleanup")
     # intentionally don't delete it, to see if it gets cleaned up on exit
 
-def test_shared_arrays_cleaned_on_exit():
-    stderr = _run_function_externally("_test_shared_arrays_cleaned_on_exit")
-
-    assert "leaked shared_memory" not in stderr  # should have cleaned up without fuss
+def test_shared_arrays_cleaned_on_exit(clean_up_test_protection):
+    _run_function_externally("_test_shared_arrays_cleaned_on_exit")
 
     _assert_shared_memory_cleaned_up()
 
 
-def _test_shared_arrays_cleaned_on_kill():
+def _test_shared_arrays_cleaned_on_terminate():
     # designed to run in a completely separate python process (i.e. not a subprocess of the test process)
     ar = shared.make_shared_array((10,), dtype=np.int32, zeros=True, fname="pynbody-test-cleanup")
 
-    # send SIGKILL to ourselves:
-    os.kill(os.getpid(), signal.SIGKILL)
+    # send SIGTERM to ourselves:
+    os.kill(os.getpid(), signal.SIGTERM)
 
     # wait to die...
     time.sleep(2.0)
 
 
-def test_shared_arrays_cleaned_on_kill():
-    stderr = _run_function_externally("_test_shared_arrays_cleaned_on_kill")
-
-    assert "leaked shared_memory" in stderr # this tells us the resource tracker has claimed to clean it up
-
+def test_shared_arrays_cleaned_on_kill(clean_up_test_protection):
+    stderr = _run_function_externally("_test_shared_arrays_cleaned_on_terminate")
     _assert_shared_memory_cleaned_up()
 
 
 def _assert_shared_memory_cleaned_up():
-    with pytest.raises(FileNotFoundError):
+    with pytest.raises(pynbody.array.shared.SharedArrayNotFound):
         _ = shared.make_shared_array((10,), dtype=np.int32, zeros=False,
                                      fname="pynbody-test-cleanup", create=False)
 
 
 def _run_function_externally(function_name):
     pwd = os.path.dirname(__file__)
     python = sys.executable
     import subprocess
     process = subprocess.Popen([python, "-c",
                                 f"from array_test import {function_name}; {function_name}()"]
-                               , cwd=pwd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    stdout, stderr = process.communicate()
-    return stderr.decode("utf-8")
+                               , cwd=pwd)
+    process.wait()
```

### Comparing `pynbody-2.0.0b5/tests/bridge_test.py` & `pynbody-2.0.0b7/tests/bridge_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/copy_on_access_test.py` & `pynbody-2.0.0b7/tests/copy_on_access_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/cosmology_test.py` & `pynbody-2.0.0b7/tests/cosmology_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/derived_arrays_test.py` & `pynbody-2.0.0b7/tests/derived_arrays_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/family_test.py` & `pynbody-2.0.0b7/tests/family_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/filter_test.py` & `pynbody-2.0.0b7/tests/filter_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/gadget_test.py` & `pynbody-2.0.0b7/tests/gadget_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/gadgethdf_test.py` & `pynbody-2.0.0b7/tests/gadgethdf_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/grafic_test.py` & `pynbody-2.0.0b7/tests/grafic_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/gravity_test.py` & `pynbody-2.0.0b7/tests/gravity_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/halos_test.py` & `pynbody-2.0.0b7/tests/halos_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/halotools_test.py` & `pynbody-2.0.0b7/tests/halotools_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/hop_test.py` & `pynbody-2.0.0b7/tests/hop_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/kdtree_test.py` & `pynbody-2.0.0b7/tests/kdtree_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,49 +61,48 @@
     np.save('test_smooth.npy', f.dm['smooth'][::100])
     np.save('test_rho.npy', f.dm['rho'][::100])
     np.save('test_v_mean.npy',f.dm['v_mean'][::100])
     np.save('test_v_disp.npy',f.dm['v_disp'][::100])
     """
 
     npt.assert_allclose(f.dm['smooth'][::100],
-                        smooth,rtol=1e-5)
+                        smooth,rtol=1e-8)
 
     npt.assert_allclose(f.dm['rho'][::100],
-                        rho,rtol=1e-5)
+                        rho,rtol=1e-8)
 
 
 
-    npt.assert_allclose(v_mean,f.dm['v_mean'][::100],rtol=1e-3)
-    npt.assert_allclose(v_disp,f.dm['v_disp'][::100],rtol=1e-3)
+    npt.assert_allclose(v_mean,f.dm['v_mean'][::100],rtol=1e-8)
+    npt.assert_allclose(v_disp,f.dm['v_disp'][::100],rtol=1e-8)
 
     # check 1D smooth works too
     vz_mean = f.dm.kdtree.sph_mean(f.dm['vz'],32)
-    npt.assert_allclose(v_mean[:,2],vz_mean[::100],rtol=1e-3)
+    npt.assert_allclose(v_mean[:,2],vz_mean[::100],rtol=1e-8)
 
     # check 1D dispersions
     v_disp_squared = (
         f.dm.kdtree.sph_dispersion(f.dm['vx'], 32)**2+
         f.dm.kdtree.sph_dispersion(f.dm['vy'], 32)**2+
         f.dm.kdtree.sph_dispersion(f.dm['vz'], 32)**2
     )
 
-    npt.assert_allclose(v_disp**2, v_disp_squared[::100], rtol=1e-3)
+    npt.assert_allclose(v_disp**2, v_disp_squared[::100], rtol=1e-8)
 
 
 def test_smooth_WendlandC2(rho_W):
+    pynbody.config['sph']['Kernel'] = 'WendlandC2'
 
-    """
-        np.save('test_rho_W.npy', f.g['rho'][::100])
-    """
-    pynbody.config['Kernel'] = 'WendlandC2'
-
-    f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
-
-    npt.assert_allclose(f.g['rho'][::100],
-                        rho_W,rtol=1e-5)
+    try:
+        f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
+        del f.properties['boxsize']
+        np.save('test_rho_W2.npy', f.dm['rho'][::100])
+        npt.assert_allclose(f.d['rho'][::100], rho_W, rtol=1e-6)
+    finally:
+        pynbody.config['sph']['Kernel'] = 'CubicSpline'
 
 def test_kd_delete():
     global f
     f.dm['smooth']
 
     assert hasattr(f.dm,'kdtree')
 
@@ -179,27 +178,33 @@
 
     generator_nn = t.nn(n_neigh)
     n = next(generator_nn)
     # print(n)
 
     p_idx = n[0]       # particle index in snapshot arrays
     hsml = n[1]        # smoothing length
-    neigh_list = n[2]  # neighbours list
-    dist2 = n[3]       # squared distances from neighbours
+    neigh_list = np.array(n[2])  # neighbours list
+    dist2 = np.array(n[3])       # squared distances from neighbours
     assert p_idx == 9
     assert hsml == f.g['smooth'][p_idx]
     npt.assert_allclose(hsml,np.sqrt(np.max(dist2))/2, rtol=1e-6)
-    assert hsml == 128.19053649902344
-    assert neigh_list == [9, 11, 35, 1998, 7, 12, 22, 36, 5, 20, 34, 31, 8, 19, 37, 10, 2018,
-                          2017, 38, 52, 39, 41, 42, 33, 23, 1997, 43, 1996, 24, 40, 25, 21]
-    npt.assert_allclose(dist2, [0.0, 39369.51953125, 24460.677734375, 31658.59375, 58536.9765625, 57026.3984375, 51718.3515625,
-                         47861.25390625, 59311.27734375, 34860.97265625, 36082.15234375, 65731.2578125, 16879.42578125,
-                         52811.79296875, 16521.751953125, 17574.501953125, 24489.19140625, 29066.84765625, 36883.796875,
-                         41815.23046875, 60706.04296875, 31192.068359375, 58157.92578125, 60277.04296875, 61944.99609375,
-                         45676.2578125, 54654.58984375, 59870.70703125, 20319.2890625, 35900.76953125, 30422.66796875, 56239.8828125],
+    assert np.allclose(hsml, 128.19053649902344)
+
+    ordering = np.argsort(dist2)
+    assert (neigh_list[ordering] == [   9,   37,    8,   10,   24,   35, 2018, 2017,   25,   41, 1998,
+         20,   40,   34,   38,   11,   52, 1997,   36,   22,   19,   43,
+         21,   12,   42,    7,    5, 1996,   33,   39,   23,   31]).all()
+    npt.assert_allclose(dist2[ordering], [    0.        , 16521.75195312, 16879.42578125, 17574.50195312,
+       20319.2890625 , 24460.67773438, 24489.19140625, 29066.84765625,
+       30422.66796875, 31192.06835938, 31658.59375   , 34860.97265625,
+       35900.76953125, 36082.15234375, 36883.796875  , 39369.51953125,
+       41815.23046875, 45676.2578125 , 47861.25390625, 51718.3515625 ,
+       52811.79296875, 54654.58984375, 56239.8828125 , 57026.3984375 ,
+       58157.92578125, 58536.9765625 , 59311.27734375, 59870.70703125,
+       60277.04296875, 60706.04296875, 61944.99609375, 65731.2578125 ],
                         rtol=1e-6)
 
     neighbour_list_all = t.all_nn(n_neigh)
     assert n == neighbour_list_all[0]
     for nl in neighbour_list_all:
         assert len(nl[2]) == n_neigh   # always find n_neigh neighbours
         idx_self = nl[2].index(nl[0])  # index of self in the neighbour list (not necessarily the first element)
@@ -215,14 +220,44 @@
     # print(f.g['v_curl'][::100], f.g['v_div'][::100])
     curl, div = arr['curl'], arr['div']
     npt.assert_allclose(f.g['v_curl'][::100], curl, rtol=2e-4)
     npt.assert_allclose(f.g['v_div'][::100],  div,  rtol=2e-4)
     npt.assert_equal(f.g['vorticity'], f.g['v_curl'])
     assert f.g['vorticity'].units == f.g['vel'].units/f.g['pos'].units
 
+def test_kdtree_parallel_build():
+    """Check that parallel tree build results in identical tree to serial build."""
+    f = pynbody.new(dm=5000)
+    f['pos'] = np.random.uniform(size=(5000,3))
+    f['mass'] = np.random.uniform(size=5000)
+
+    f.build_tree(1)
+    result_one_thread = f.kdtree.serialize()
+
+    _, _, kdn1, poff1, _ = result_one_thread
+
+    del f.kdtree
+
+    f.build_tree(4)
+    result_four_threads = f.kdtree.serialize()
+    _, _, kdn4, poff4, _ = result_four_threads
+
+    assert (kdn1['pLower'] == kdn4['pLower']).all()
+    assert (kdn1['pUpper'] == kdn4['pUpper']).all()
+    assert (kdn1['iDim'] == kdn4['iDim']).all()
+    npt.assert_allclose(kdn1['bnd']['fMin'], kdn4['bnd']['fMin'])
+    npt.assert_allclose(kdn1['bnd']['fMax'], kdn4['bnd']['fMax'])
+    npt.assert_allclose(kdn1['fSplit'], kdn4['fSplit'])
+    assert (poff1 == poff4).all()
+
+
+
+
+
+
 @pytest.mark.parametrize("npart", [1, 10, 100, 1000, 100000])
 @pytest.mark.parametrize("offset", [0.0, 0.2, 0.5]) # checks wrapping
 @pytest.mark.parametrize("radius", [0.1, 0.3, 1.0])
 @pytest.mark.parametrize("dtype", [np.float32, np.float64])
 def test_particles_in_sphere(npart, offset, radius, dtype):
     f = pynbody.new(dm=npart)
 
@@ -264,21 +299,29 @@
     f['pos'] = np.random.normal(1.0, size=(npart, 3))
     f['mass'] = np.random.uniform(size=npart)
     return f
 
 
 def test_kdtree_shared_mem(npart=1000):
     f = _make_test_gaussian(npart)
-    n = shared.get_num_shared_arrays()
+    n = shared.get_num_shared_arrays_owned()
     f.build_tree(shared_mem=False)
-    assert shared.get_num_shared_arrays() == n
+    assert shared.get_num_shared_arrays_owned() == n
     del f
 
     f = _make_test_gaussian(npart)
     f.build_tree(shared_mem=True)
-    assert shared.get_num_shared_arrays() == 2+n
+    assert shared.get_num_shared_arrays_owned() == 2 + n
     assert f.kdtree.kdnodes._shared_fname.startswith('pynbody')
     assert f.kdtree.particle_offsets._shared_fname.startswith('pynbody')
     del f
     gc.collect()
-    shared._ensure_shared_memory_clean()
-    assert shared.get_num_shared_arrays() == n
+    assert shared.get_num_shared_arrays_owned() == n
+
+def test_boxsize_too_small():
+    f = pynbody.new(dm=1000)
+    f['pos'] = np.random.normal(scale=1.0, size=f['pos'].shape)
+    f['vel'] = np.random.normal(scale=1.0, size=f['vel'].shape)
+    f['mass'] = np.random.uniform(1.0, 10.0, size=f['mass'].shape)
+    f.properties['boxsize'] = 0.1
+    with pytest.warns(RuntimeWarning, match = "span a region larger than the specified boxsize"):
+        _ = f['smooth']
```

### Comparing `pynbody-2.0.0b5/tests/nchilada_test.py` & `pynbody-2.0.0b7/tests/nchilada_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/partial_tipsy_test.py` & `pynbody-2.0.0b7/tests/partial_tipsy_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/performance_kdtree.py` & `pynbody-2.0.0b7/tests/performance_kdtree.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,26 +29,33 @@
 except Exception:
     num_threads = None
 
 np.random.seed(1337)
 
 Npart = 10000000
 Ntrials = 20
+dtype = np.float32
 
-centres = np.random.uniform(size=(Ntrials,3)) - 0.5
-radii = 10.**np.random.uniform(low=-3.0,high=-1.0,size=Ntrials)
+centres = (np.random.uniform(size=(Ntrials,3)) - 0.5).astype(dtype)
+radii = 10.**np.random.uniform(low=-3.0,high=-1.0,size=Ntrials).astype(dtype)
 
-xcs = np.random.uniform(-0.5, 0.5, size=Ntrials)
-ycs = np.random.uniform(-0.5, 0.5, size=Ntrials)
-zcs = np.random.uniform(-0.5, 0.5, size=Ntrials)
+xcs = np.random.uniform(-0.5, 0.5, size=Ntrials).astype(dtype)
+ycs = np.random.uniform(-0.5, 0.5, size=Ntrials).astype(dtype)
+zcs = np.random.uniform(-0.5, 0.5, size=Ntrials).astype(dtype)
 
 f = pynbody.new(dm=Npart)
+f._create_array('pos', 3, dtype=dtype)
+f._create_array('mass', 1, dtype=dtype)
 
-f['pos'] = np.random.uniform(size=(Npart,3))
+f['pos'] = np.random.uniform(size=(Npart,3)).astype(dtype)
 f['pos'] -= 0.5
+f['mass'] = np.ones(Npart, dtype=dtype)
+f.properties['boxsize'] = 1.0
+
+print("Using data type = ",f['pos'].dtype)
 
 with timer("sphere queries without tree"):
     for cen, rad in zip(centres, radii):
         print(".",end="")
         sys.stdout.flush()
         _ = f[pynbody.filt.Sphere(rad, cen)]
 
@@ -66,19 +73,19 @@
 
 with timer("sphere queries from tree"):
     for cen,rad in zip(centres,radii):
         print(".", end="")
         sys.stdout.flush()
         _ = f[pynbody.filt.Sphere(rad, cen)]
 
-with timer("cube queries from tree"):
-    for xc, yc, zc, s in zip(xcs, ycs, zcs, radii):
-        print(".", end="")
-        sys.stdout.flush()
-        _ = f[pynbody.filt.Cuboid(xc - s, yc - s, zc - s, xc + s, yc + s, zc + s)]
+# with timer("cube queries from tree"):
+#     for xc, yc, zc, s in zip(xcs, ycs, zcs, radii):
+#         print(".", end="")
+#         sys.stdout.flush()
+#         _ = f[pynbody.filt.Cuboid(xc - s, yc - s, zc - s, xc + s, yc + s, zc + s)]
 
 
 
 with timer("get smooth"):
     _ = f['smooth']
 
 with timer("get rho"):
```

### Comparing `pynbody-2.0.0b5/tests/ramses_test.py` & `pynbody-2.0.0b7/tests/ramses_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/rockstar_test.py` & `pynbody-2.0.0b7/tests/rockstar_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/snapshot_test.py` & `pynbody-2.0.0b7/tests/snapshot_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/sph_image_test.py` & `pynbody-2.0.0b7/tests/sph_image_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/subarray_test.py` & `pynbody-2.0.0b7/tests/subarray_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/subfind_test.py` & `pynbody-2.0.0b7/tests/subfind_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/subfindhdf_gadget4_test.py` & `pynbody-2.0.0b7/tests/subfindhdf_gadget4_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/subfindhdf_test.py` & `pynbody-2.0.0b7/tests/subfindhdf_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
           2042696, 1992905, 2092106, 2074698, 2026952, 1944013,   10185,
           1960656, 1912012, 2090949]).all()
     assert (h[10]['iord'][::100] == [ 782722,  865539,  865923,  784260,  849150,  750470,  898950,
            866689,  882560, 2913154, 2865029, 2880647, 2896644, 2995974,
           2913929, 2881289, 2896517, 2995969,  832898,  865671,  832639]).all()
 
     assert h[0].properties['NsubPerHalo'] == 6
-    assert (h[0].properties['children'] == [0, 1, 2, 3, 4, 5]).all()
+    assert np.all(h[0].properties['children'] == [0, 1, 2, 3, 4, 5])
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=RuntimeWarning, message="Accessing multiple halos")
         for i, halo in enumerate(h[0:10]):
             halo['mass'].sum()
             for fam in [halo.g, halo.d, halo.s]:
                 assert (len(fam['iord']) ==
@@ -121,17 +121,17 @@
 
     if with_units:
         npt.assert_allclose(properties['Mass'].units.ratio(snap.infer_original_units("g")), 1.0)
         npt.assert_allclose(properties['CenterOfMass'].units.ratio(snap.infer_original_units("cm")), 1.0)
     else:
         assert not hasattr(properties['Mass'], 'units')
 
-
-
-def test_halo_values(snap) :
+@pytest.mark.filterwarnings("ignore:Accessing multiple halos")
+@pytest.mark.parametrize('load_all', (True, False))
+def test_halo_values(snap, load_all) :
     """ Check that halo values (and sizes) agree with pyread_gadget_hdf5 """
 
     filesub = 'testdata/gadget3/data/subhalos_103/subhalo_103'
 
 
 
     FoF_Mass = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'Mass', sub_dir='fof', nopanda=True, silent=True)
@@ -139,15 +139,16 @@
     Sub_Mass = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'Mass', sub_dir='subfind', nopanda=True, silent=True)
     Sub_MassType = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'MassType', sub_dir='subfind', nopanda=True, silent=True)
     NsubPerHalo = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'NsubPerHalo', sub_dir='subfind', nopanda=True, silent=True)
     OffsetHalo = np.roll(NsubPerHalo.cumsum(), 1)
     OffsetHalo[0]=0 ## To start counter
 
     h = snap.halos()
-    h.load_all()
+    if load_all:
+        h.load_all()
 
     FoF_CoM = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'CenterOfMass', sub_dir='fof', nopanda=True, silent=True)
     Sub_CoM = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'CenterOfMass', sub_dir='subfind', nopanda=True, silent=True)
 
     # Check the Halo Array values
     for i,halo in enumerate(h[0:10]) :
         assert(np.allclose(halo.properties['CenterOfMass'], FoF_CoM[i], rtol=1e-3))
@@ -181,12 +182,14 @@
     # Test the Particle Temperature and implicitly the particle ordering
     for i,halo in enumerate(h[0:10]) :
         npt.assert_allclose(
             halo.g['temp'],
             FoF_Temp[FoF_Offset[i]:FoF_Offset[i]+FoF_Length[i]],
         )
 
-def test_halo_properties_physical_units(snap):
+@pytest.mark.parametrize('load_all', (True, False))
+def test_halo_properties_physical_units(snap, load_all):
     h = snap.halos()
-    h.load_all()
+    if load_all:
+        h.load_all()
     h.physical_units()
     npt.assert_allclose(h[0].properties['CenterOfMass'], [1242.67381894, 1571.45917479, 2232.62036159])
```

### Comparing `pynbody-2.0.0b5/tests/swift_test.py` & `pynbody-2.0.0b7/tests/swift_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,14 @@
     assert not f._hdf_files.is_virtual()
     _assert_multifile_contents_is_sensible(f)
 
 def test_swift_singlefile_is_not_vds():
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
     assert not f._hdf_files.is_virtual()
 
-
-
-# TODO: test partial loading where the region wraps around the periodic box
-
 def test_swift_singlefile_partial_loading():
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5",
                      take_swift_cells=[5,15,20,25])
     assert len(f.dm) == 1849
     assert len(f.gas) == 1882
     assert (f.dm['iord'][::100] == [ 16468,   9172,  41176,  49874,   9342,  10234,  33908,  25852,
                                      42628,  34566,  26566,  10818, 502992,  67776,  34896,  68286,
@@ -148,15 +144,15 @@
 def test_swift_dtypes():
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
     assert np.issubdtype(f['iord'].dtype, np.integer)
     assert np.issubdtype(f['pos'].dtype, np.floating)
 
 @pytest.mark.parametrize('test_region',
                          [pynbody.filt.Sphere(50., (50., 50., 50.)),
-                         pynbody.filt.Cuboid(-20.0)])
+                         pynbody.filt.Cuboid(-20.0)]) # note the cuboid test region wraps around the box
 def test_swift_take_geometric_region(test_region):
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5",
                      take_region = test_region)
 
     f_full = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
 
     assert len(f) < len(f_full)
```

### Comparing `pynbody-2.0.0b5/tests/test_profile.py` & `pynbody-2.0.0b7/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/theoretical_profile.py` & `pynbody-2.0.0b7/tests/theoretical_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/tipsy_test.py` & `pynbody-2.0.0b7/tests/tipsy_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
     rhoform = snap.s['rhoform'].in_units('Msol kpc**-3')[:1000:100]
     correct = np.array([ 2472533.42024787,  5336799.91228041, 64992197.77874849,
             16312128.27530325,  2514281.61028265, 14384682.79060703,
              3334026.53876033, 30041215.63578063, 24977741.02041524,
             10758492.68887316])
     assert np.all(np.abs(rhoform - correct) < 1e-7)
     # h2form should not be in the available starlog keys
-    with pytest.raises(DependencyError):
+    with pytest.raises(KeyError):
         h2form = snap.s['h2form']
 
 def test_read_starlog_with_log(snap):
     # the last key is incorrectly labeled in order to ensure
     # that the log file is being read
     with open('testdata/gasoline_ahf/g15784.lr.log', 'w') as logf:
         logf.write('# ilbDumpIteration: 0\n# bDoSimulateLB: 0\n# starlog data:\n'
```

### Comparing `pynbody-2.0.0b5/tests/transformation_test.py` & `pynbody-2.0.0b7/tests/transformation_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/units_test.py` & `pynbody-2.0.0b7/tests/units_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/utils_test.py` & `pynbody-2.0.0b7/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b5/tests/velociraptor_test.py` & `pynbody-2.0.0b7/tests/velociraptor_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,19 @@
           394930, 395314, 411440, 411308, 386736, 402994, 419634, 411306,
           386860, 411434, 395188, 403118, 395180, 394798, 419506, 411184,
           403378, 402986]
 
     assert (np.sort(h[20]['iord']) == np.sort(testvals)).all()
 
 
+@pytest.mark.filterwarnings("ignore:Accessing multiple halos")
 @pytest.mark.parametrize("use_all", [True, False])
 def test_swift_velociraptor_parents_and_children(use_all):
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
     h = pynbody.halo.velociraptor.VelociraptorCatalogue(f)
-    h.load_all()
 
     if use_all:
         properties = h.get_properties_all_halos()
         getter = lambda k, i: properties[k][h.number_mapper.number_to_index(i)]
     else:
         getter = lambda k, i: h[i].properties[k]
 
@@ -67,18 +67,21 @@
     # the above were from the genuine velociraptor output. But since these were the only subhalos, the test was
     # a bit too trivial. The following are some faked subhalos to test a more complex scenario
 
     assert (getter('children', 1) == [203, 204, 206]).all()
     assert (getter('children', 4) == [205, 207]).all()
     assert getter('parent', 203) == 1
 
-def test_swift_velociraptor_properties():
+@pytest.mark.filterwarnings("ignore:Accessing multiple halos")
+@pytest.mark.parametrize("load_all", [True, False])
+def test_swift_velociraptor_properties(load_all):
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
     h = pynbody.halo.velociraptor.VelociraptorCatalogue(f)
-    h.load_all()
+    if load_all:
+        h.load_all()
 
     assert np.allclose(float(h[1].properties['Lx']), -90787.3983020414e13)
     assert np.allclose(float(h[10].properties['Lx']), -73881.83861892551e13)
 
     assert np.allclose(h[1].properties['Lx'].ratio("1e13 kpc Msol km s**-1"), -90787.3983020414)
 
 @pytest.mark.parametrize("with_units", [True, False])
```

