# Comparing `tmp/shapely-2.0rc2.tar.gz` & `tmp/shapely-2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapely-2.0rc2.tar", last modified: Sat Dec  3 14:44:26 2022, max compression
+gzip compressed data, was "shapely-2.0rc3.tar", last modified: Wed Dec  7 08:16:42 2022, max compression
```

## Comparing `shapely-2.0rc2.tar` & `shapely-2.0rc3.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.818128 shapely-2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2022-12-03 14:44:06.000000 shapely-2.0rc2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-03 14:44:06.000000 shapely-2.0rc2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2022-12-03 14:44:06.000000 shapely-2.0rc2/CREDITS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2022-12-03 14:44:06.000000 shapely-2.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-03 14:44:26.818128 shapely-2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2022-12-03 14:44:06.000000 shapely-2.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.798127 shapely-2.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/constructive.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/creation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/linear.rst
--rw-r--r--   0 runner    (1001) docker     (123)    90339 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/manual.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/measurement.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/migration_pygeos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/predicates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/set_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/strtree.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-03 14:44:06.000000 shapely-2.0rc2/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2022-12-03 14:44:06.000000 shapely-2.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2022-12-03 14:44:26.818128 shapely-2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2022-12-03 14:44:06.000000 shapely-2.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.818128 shapely-2.0rc2/shapely/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25204 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_geometry_helpers.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_geos.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_geos.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_pygeos_api.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/_ragged_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-03 14:44:26.818128 shapely-2.0rc2/shapely/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/affinity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.806127 shapely-2.0rc2/shapely/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/algorithms/cga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/algorithms/polylabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    37397 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/constructive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    20497 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.806127 shapely-2.0rc2/shapely/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33190 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/linestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/multilinestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/geos.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34289 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/set_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/speedups.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/strtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.810128 shapely-2.0rc2/shapely/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.810128 shapely-2.0rc2/shapely/tests/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_emptiness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_linestring.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_multilinestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    14675 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/geometry/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_constructive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_creation_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)    24505 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24783 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_ragged_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_set_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    76137 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_strtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.810128 shapely-2.0rc2/shapely/vectorized/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/vectorized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/wkb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-03 14:44:06.000000 shapely-2.0rc2/shapely/wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.806127 shapely-2.0rc2/shapely.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-03 14:44:26.000000 shapely-2.0rc2/shapely.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2022-12-03 14:44:26.000000 shapely-2.0rc2/shapely.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 14:44:26.000000 shapely-2.0rc2/shapely.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-03 14:44:26.000000 shapely-2.0rc2/shapely.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-03 14:44:26.000000 shapely-2.0rc2/shapely.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.814128 shapely-2.0rc2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/c_api.c
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/c_api.h
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/coords.c
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/coords.h
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/fast_loop_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    28126 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/geos.c
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/geos.h
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/kvec.h
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/lib.c
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/pygeom.c
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/pygeom.h
--rw-r--r--   0 runner    (1001) docker     (123)    38206 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/strtree.c
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/strtree.h
--rw-r--r--   0 runner    (1001) docker     (123)   119600 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/ufuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/ufuncs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/vector.c
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-03 14:44:06.000000 shapely-2.0rc2/src/vector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 14:44:26.818128 shapely-2.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_cga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_clip_by_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_create_inconsistent_dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_empty_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_geointerface.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_invalid_geometries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_linear_referencing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_linemerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_make_valid.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_minimum_clearance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_ndarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_orient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_parallel_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_polygonize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_polylabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_products_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_shared_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_substring.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_voronoi_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_wkb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/test_wkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-03 14:44:06.000000 shapely-2.0rc2/tests/threading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2022-12-03 14:44:06.000000 shapely-2.0rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.857154 shapely-2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2022-12-07 08:16:15.000000 shapely-2.0rc3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-07 08:16:15.000000 shapely-2.0rc3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2022-12-07 08:16:15.000000 shapely-2.0rc3/CREDITS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2022-12-07 08:16:15.000000 shapely-2.0rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-07 08:16:42.857154 shapely-2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2022-12-07 08:16:15.000000 shapely-2.0rc3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.825154 shapely-2.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/constructive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/creation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/linear.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    90339 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/measurement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/migration_pygeos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/predicates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/set_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/strtree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-07 08:16:15.000000 shapely-2.0rc3/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2022-12-07 08:16:15.000000 shapely-2.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-07 08:16:42.857154 shapely-2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2022-12-07 08:16:15.000000 shapely-2.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.857154 shapely-2.0rc3/shapely/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25204 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_geometry_helpers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_geos.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_geos.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_pygeos_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-07 08:16:42.857154 shapely-2.0rc3/shapely/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/affinity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.833154 shapely-2.0rc3/shapely/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/algorithms/cga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/algorithms/polylabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37397 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/constructive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20497 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.837154 shapely-2.0rc3/shapely/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33190 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/linestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/multilinestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/geos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34816 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/speedups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/strtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.841154 shapely-2.0rc3/shapely/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.841154 shapely-2.0rc3/shapely/tests/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_emptiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_linestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_multilinestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14675 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/geometry/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_constructive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_creation_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24505 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24783 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76137 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_strtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.841154 shapely-2.0rc3/shapely/vectorized/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/vectorized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/wkb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-07 08:16:15.000000 shapely-2.0rc3/shapely/wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.833154 shapely-2.0rc3/shapely.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-07 08:16:42.000000 shapely-2.0rc3/shapely.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2022-12-07 08:16:42.000000 shapely-2.0rc3/shapely.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 08:16:42.000000 shapely-2.0rc3/shapely.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-07 08:16:42.000000 shapely-2.0rc3/shapely.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-07 08:16:42.000000 shapely-2.0rc3/shapely.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.845154 shapely-2.0rc3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/c_api.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/coords.c
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/coords.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/fast_loop_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28126 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/geos.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/geos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/kvec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/pygeom.c
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/pygeom.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38206 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/strtree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/strtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119600 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/ufuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/ufuncs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/vector.c
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-07 08:16:15.000000 shapely-2.0rc3/src/vector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 08:16:42.857154 shapely-2.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_cga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_clip_by_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_create_inconsistent_dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_empty_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_geointerface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_invalid_geometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_linear_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_linemerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_make_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_minimum_clearance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_ndarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_orient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_parallel_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_polygonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_polylabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_products_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_shared_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_substring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_voronoi_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_wkb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/test_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-07 08:16:15.000000 shapely-2.0rc3/tests/threading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2022-12-07 08:16:15.000000 shapely-2.0rc3/versioneer.py
```

### Comparing `shapely-2.0rc2/CHANGES.txt` & `shapely-2.0rc3/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/CITATION.cff` & `shapely-2.0rc3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/CREDITS.txt` & `shapely-2.0rc3/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/LICENSE.txt` & `shapely-2.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/PKG-INFO` & `shapely-2.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapely
-Version: 2.0rc2
+Version: 2.0rc3
 Summary: Manipulation and analysis of geometric objects
 Author: Sean Gillies
 Maintainer: Shapely contributors
 License: BSD 3-Clause
 Project-URL: Documentation, https://shapely.readthedocs.io/
 Project-URL: Repository, https://github.com/shapely/shapely
 Keywords: geometry,topology,gis
```

### Comparing `shapely-2.0rc2/README.rst` & `shapely-2.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/design.rst` & `shapely-2.0rc3/docs/design.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/geometry.rst` & `shapely-2.0rc3/docs/geometry.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/index.rst` & `shapely-2.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/installation.rst` & `shapely-2.0rc3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/manual.rst` & `shapely-2.0rc3/docs/manual.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/migration.rst` & `shapely-2.0rc3/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/docs/migration_pygeos.rst` & `shapely-2.0rc3/docs/migration_pygeos.rst`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/pyproject.toml` & `shapely-2.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/setup.py` & `shapely-2.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/__init__.py` & `shapely-2.0rc3/shapely/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,13 +22,12 @@
     MultiPoint,
     MultiLineString,
     MultiPolygon,
     GeometryCollection,
     LinearRing,
 )
 
-from ._version import get_versions
+from . import _version
 
-__version__ = get_versions()["version"]
-del get_versions
+__version__ = _version.get_versions()["version"]
 
 setup_signal_checks()
```

### Comparing `shapely-2.0rc2/shapely/_geometry.py` & `shapely-2.0rc3/shapely/_geometry.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/_geometry_helpers.pyx` & `shapely-2.0rc3/shapely/_geometry_helpers.pyx`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/_geos.pxd` & `shapely-2.0rc3/shapely/_geos.pxd`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/_geos.pyx` & `shapely-2.0rc3/shapely/_geos.pyx`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/_pygeos_api.pxd` & `shapely-2.0rc3/shapely/_pygeos_api.pxd`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/_ragged_array.py` & `shapely-2.0rc3/shapely/_ragged_array.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/affinity.py` & `shapely-2.0rc3/shapely/affinity.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/algorithms/cga.py` & `shapely-2.0rc3/shapely/algorithms/cga.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/algorithms/polylabel.py` & `shapely-2.0rc3/shapely/algorithms/polylabel.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/constructive.py` & `shapely-2.0rc3/shapely/constructive.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/coordinates.py` & `shapely-2.0rc3/shapely/coordinates.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/coords.py` & `shapely-2.0rc3/shapely/coords.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/creation.py` & `shapely-2.0rc3/shapely/creation.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/decorators.py` & `shapely-2.0rc3/shapely/decorators.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/enum.py` & `shapely-2.0rc3/shapely/enum.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/errors.py` & `shapely-2.0rc3/shapely/errors.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/__init__.py` & `shapely-2.0rc3/shapely/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/base.py` & `shapely-2.0rc3/shapely/geometry/base.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/collection.py` & `shapely-2.0rc3/shapely/geometry/collection.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/geo.py` & `shapely-2.0rc3/shapely/geometry/geo.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/linestring.py` & `shapely-2.0rc3/shapely/geometry/linestring.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/multilinestring.py` & `shapely-2.0rc3/shapely/geometry/multilinestring.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/multipoint.py` & `shapely-2.0rc3/shapely/geometry/multipoint.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/multipolygon.py` & `shapely-2.0rc3/shapely/geometry/multipolygon.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/point.py` & `shapely-2.0rc3/shapely/geometry/point.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/geometry/polygon.py` & `shapely-2.0rc3/shapely/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/io.py` & `shapely-2.0rc3/shapely/io.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/linear.py` & `shapely-2.0rc3/shapely/linear.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/measurement.py` & `shapely-2.0rc3/shapely/measurement.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/ops.py` & `shapely-2.0rc3/shapely/ops.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/plotting.py` & `shapely-2.0rc3/shapely/plotting.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/predicates.py` & `shapely-2.0rc3/shapely/predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1110,14 +1110,20 @@
         For other keyword-only arguments, see the
         `NumPy ufunc docs <https://numpy.org/doc/stable/reference/ufuncs.html#ufuncs-kwargs>`_.
 
     See also
     --------
     contains : variant taking two geometries as input
 
+    Notes
+    -----
+    If you compare a small number of polygons or lines with many points,
+    it can be beneficial to prepare the geometries in advance using
+    :func:`shapely.prepare`.
+
     Examples
     --------
     >>> from shapely import Point, Polygon
     >>> area = Polygon([(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)])
     >>> contains(area, Point(0.5, 0.5))
     True
     >>> contains_xy(area, 0.5, 0.5)
@@ -1150,14 +1156,23 @@
         For other keyword-only arguments, see the
         `NumPy ufunc docs <https://numpy.org/doc/stable/reference/ufuncs.html#ufuncs-kwargs>`_.
 
     See also
     --------
     intersects : variant taking two geometries as input
 
+    Notes
+    -----
+    If you compare a single or few geometries with many points, it can be
+    beneficial to prepare the geometries in advance using
+    :func:`shapely.prepare`.
+
+    The `touches` predicate can be determined with this function by getting
+    the boundary of the geometries: ``intersects_xy(boundary(geom), x, y)``.
+
     Examples
     --------
     >>> from shapely import LineString, Point
     >>> line = LineString([(0, 0), (1, 1)])
     >>> intersects(line, Point(0, 0))
     True
     >>> intersects_xy(line, 0, 0)
```

### Comparing `shapely-2.0rc2/shapely/prepared.py` & `shapely-2.0rc3/shapely/prepared.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/set_operations.py` & `shapely-2.0rc3/shapely/set_operations.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/speedups.py` & `shapely-2.0rc3/shapely/speedups.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/strtree.py` & `shapely-2.0rc3/shapely/strtree.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,38 @@
 
 
 class STRtree:
     """
     A query-only R-tree spatial index created using the
     Sort-Tile-Recursive (STR) [1]_ algorithm.
 
-    For two-dimensional spatial data. The tree is constructed directly
-    at initialization. The tree is immutable and query-only, meaning that
-    once created nodes cannot be added or removed.
+    The tree indexes the bounding boxes of each geometry.  The tree is
+    constructed directly at initialization and nodes cannot be added or
+    removed after it has been created.
 
     All operations return indices of the input geometries.  These indices
     can be used to index into anything associated with the input geometries,
     including the input geometries themselves, or custom items stored in
     another object of the same length as the geometries.
 
+    Bounding boxes limited to two dimensions and are axis-aligned (equivalent to
+    the ``bounds`` property of a geometry); any Z values present in geometries
+    are ignored for purposes of indexing within the tree.
+
     Any mixture of geometry types may be stored in the tree.
 
+    Note: the tree is more efficient for querying when there are fewer
+    geometries that have overlapping bounding boxes and where there is greater
+    similarity between the outer boundary of a geometry and its bounding box.
+    For example, a MultiPolygon composed of widely-spaced individual Polygons
+    will have a large overall bounding box compared to the boundaries of its
+    individual Polygons, and the bounding box may also potentially overlap many
+    other geometries within the tree.  This means that the resulting tree may be
+    less efficient to query than a tree constructed from individual Polygons.
+
     Parameters
     ----------
     geoms : sequence
         A sequence of geometry objects.
     node_capacity : int, default 10
         The maximum number of child nodes per parent node in the tree.
 
@@ -90,44 +103,49 @@
         ndarray of Geometry objects
         """
         return self._geometries
 
     def query(self, geometry, predicate=None, distance=None):
         """
         Return the integer indices of all combinations of each input geometry
-        and tree geometries where the extent of each input geometry intersects
-        the extent of a tree geometry.
+        and tree geometries where the bounding box of each input geometry
+        intersects the bounding box of a tree geometry.
 
         If the input geometry is a scalar, this returns an array of shape (n, ) with
         the indices of the matching tree geometries.  If the input geometry is an
         array_like, this returns an array with shape (2,n) where the subarrays
         correspond to the indices of the input geometries and indices of the
         tree geometries associated with each.  To generate an array of pairs of
         input geometry index and tree geometry index, simply transpose the
         result.
 
-        If a predicate is provided, the tree geometries are further filtered to
-        those that meet the predicate when comparing the input geometry to the
-        tree geometry:
-        predicate(geom, tree_geometry)
+        If a predicate is provided, the tree geometries are first queried based
+        on the bounding box of the input geometry and then are further filtered
+        to those that meet the predicate when comparing the input geometry to
+        the tree geometry:
+        predicate(geometry, tree_geometry)
 
         The 'dwithin' predicate requires GEOS >= 3.10.
 
-        Any input geometry that is None or empty will never match geometries
-        in the tree.
+        Bounding boxes are limited to two dimensions and are axis-aligned
+        (equivalent to the ``bounds`` property of a geometry); any Z values
+        present in input geometries are ignored when querying the tree.
+
+        Any input geometry that is None or empty will never match geometries in
+        the tree.
 
         Parameters
         ----------
         geometry : Geometry or array_like
             Input geometries to query the tree and filter results using the
             optional predicate.
         predicate : {None, 'intersects', 'within', 'contains', 'overlaps', 'crosses',\
 'touches', 'covers', 'covered_by', 'contains_properly', 'dwithin'}, optional
             The predicate to use for testing geometries from the tree
-            that are within the input geometry's extent.
+            that are within the input geometry's bounding box.
         distance : number or array_like, optional
             Distances around each input geometry within which to query the tree
             for the 'dwithin' predicate.  If array_like, shape must be
             broadcastable to shape of geometry.  Required if predicate='dwithin'.
 
         Returns
         -------
@@ -206,18 +224,18 @@
         ['A']
 
 
         Notes
         -----
         In the context of a spatial join, input geometries are the "left"
         geometries that determine the order of the results, and tree geometries
-        are "right" geometries that are joined against the left geometries.
-        This effectively performs an inner join, where only those combinations
-        of geometries that can be joined based on overlapping extents or optional
-        predicate are returned.
+        are "right" geometries that are joined against the left geometries. This
+        effectively performs an inner join, where only those combinations of
+        geometries that can be joined based on overlapping bounding boxes or
+        optional predicate are returned.
         """
 
         geometry = np.asarray(geometry)
         is_scalar = False
         if geometry.ndim == 0:
             geometry = np.expand_dims(geometry, 0)
             is_scalar = True
@@ -252,22 +270,26 @@
         indices = self._tree.query(geometry, predicate)
         return indices[1] if is_scalar else indices
 
     @requires_geos("3.6.0")
     def nearest(self, geometry) -> Union[Any, None]:
         """
         Return the index of the nearest geometry in the tree for each input
-        geometry.
+        geometry based on distance within two-dimensional Cartesian space.
+
+        This distance will be 0 when input geometries intersect tree geometries.
 
         If there are multiple equidistant or intersected geometries in the tree,
         only a single result is returned for each input geometry, based on the
         order that tree geometries are visited; this order may be
         nondeterministic.
 
-        If any input geometry is None or empty, an error is raised.
+        If any input geometry is None or empty, an error is raised.  Any Z
+        values present in input geometries are ignored when finding nearest
+        tree geometries.
 
         Parameters
         ----------
         geometry : Geometry or array_like
             Input geometries to query the tree.
 
         Returns
@@ -334,16 +356,18 @@
         self,
         geometry,
         max_distance=None,
         return_distance=False,
         exclusive=False,
         all_matches=True,
     ):
-        """Returns the index of the nearest geometries in the tree for each input
-        geometry.
+        """Return the index of the nearest geometries in the tree for each input
+        geometry based on distance within two-dimensional Cartesian space.
+
+        This distance will be 0 when input geometries intersect tree geometries.
 
         If there are multiple equidistant or intersected geometries in tree and
         `all_matches` is True (the default), all matching tree geometries are
         returned; otherwise only the first matching tree geometry is returned.
         Tree indices are returned in the order they are visited for each input
         geometry and may not be in ascending index order; no meaningful order is
         implied.
@@ -356,15 +380,16 @@
         max_distance may have a negative performance impact because many tree
         geometries will be queried for each input geometry.
 
         The distance, if returned, will be 0 for any intersected geometries in
         the tree.
 
         Any geometry that is None or empty in the input geometries is omitted
-        from the output.
+        from the output.  Any Z values present in input geometries are ignored
+        when finding nearest tree geometries.
 
         Parameters
         ----------
         geometry : Geometry or array_like
             Input geometries to query the tree.
         max_distance : float, optional
             Maximum distance within which to query for nearest items in tree.
```

### Comparing `shapely-2.0rc2/shapely/testing.py` & `shapely-2.0rc3/shapely/testing.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/common.py` & `shapely-2.0rc3/shapely/tests/common.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_collection.py` & `shapely-2.0rc3/shapely/tests/geometry/test_collection.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_coords.py` & `shapely-2.0rc3/shapely/tests/geometry/test_coords.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_emptiness.py` & `shapely-2.0rc3/shapely/tests/geometry/test_emptiness.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_format.py` & `shapely-2.0rc3/shapely/tests/geometry/test_format.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_geometry_base.py` & `shapely-2.0rc3/shapely/tests/geometry/test_geometry_base.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_hash.py` & `shapely-2.0rc3/shapely/tests/geometry/test_hash.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_linestring.py` & `shapely-2.0rc3/shapely/tests/geometry/test_linestring.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_multilinestring.py` & `shapely-2.0rc3/shapely/tests/geometry/test_multilinestring.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_multipoint.py` & `shapely-2.0rc3/shapely/tests/geometry/test_multipoint.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_multipolygon.py` & `shapely-2.0rc3/shapely/tests/geometry/test_multipolygon.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_point.py` & `shapely-2.0rc3/shapely/tests/geometry/test_point.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/geometry/test_polygon.py` & `shapely-2.0rc3/shapely/tests/geometry/test_polygon.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_constructive.py` & `shapely-2.0rc3/shapely/tests/test_constructive.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_coordinates.py` & `shapely-2.0rc3/shapely/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_creation.py` & `shapely-2.0rc3/shapely/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_creation_indices.py` & `shapely-2.0rc3/shapely/tests/test_creation_indices.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_geometry.py` & `shapely-2.0rc3/shapely/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_io.py` & `shapely-2.0rc3/shapely/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_linear.py` & `shapely-2.0rc3/shapely/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_measurement.py` & `shapely-2.0rc3/shapely/tests/test_measurement.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_misc.py` & `shapely-2.0rc3/shapely/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_plotting.py` & `shapely-2.0rc3/shapely/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_predicates.py` & `shapely-2.0rc3/shapely/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_ragged_array.py` & `shapely-2.0rc3/shapely/tests/test_ragged_array.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_set_operations.py` & `shapely-2.0rc3/shapely/tests/test_set_operations.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_strtree.py` & `shapely-2.0rc3/shapely/tests/test_strtree.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/tests/test_testing.py` & `shapely-2.0rc3/shapely/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/validation.py` & `shapely-2.0rc3/shapely/validation.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/vectorized/__init__.py` & `shapely-2.0rc3/shapely/vectorized/__init__.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/wkb.py` & `shapely-2.0rc3/shapely/wkb.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely/wkt.py` & `shapely-2.0rc3/shapely/wkt.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/shapely.egg-info/PKG-INFO` & `shapely-2.0rc3/shapely.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapely
-Version: 2.0rc2
+Version: 2.0rc3
 Summary: Manipulation and analysis of geometric objects
 Author: Sean Gillies
 Maintainer: Shapely contributors
 License: BSD 3-Clause
 Project-URL: Documentation, https://shapely.readthedocs.io/
 Project-URL: Repository, https://github.com/shapely/shapely
 Keywords: geometry,topology,gis
```

### Comparing `shapely-2.0rc2/shapely.egg-info/SOURCES.txt` & `shapely-2.0rc3/shapely.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/c_api.c` & `shapely-2.0rc3/src/c_api.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/c_api.h` & `shapely-2.0rc3/src/c_api.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/coords.c` & `shapely-2.0rc3/src/coords.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/fast_loop_macros.h` & `shapely-2.0rc3/src/fast_loop_macros.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/geos.c` & `shapely-2.0rc3/src/geos.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/geos.h` & `shapely-2.0rc3/src/geos.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/kvec.h` & `shapely-2.0rc3/src/kvec.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/lib.c` & `shapely-2.0rc3/src/lib.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/pygeom.c` & `shapely-2.0rc3/src/pygeom.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/pygeom.h` & `shapely-2.0rc3/src/pygeom.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/strtree.c` & `shapely-2.0rc3/src/strtree.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/strtree.h` & `shapely-2.0rc3/src/strtree.h`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/ufuncs.c` & `shapely-2.0rc3/src/ufuncs.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/src/vector.c` & `shapely-2.0rc3/src/vector.c`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/__init__.py` & `shapely-2.0rc3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/conftest.py` & `shapely-2.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_affinity.py` & `shapely-2.0rc3/tests/test_affinity.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_box.py` & `shapely-2.0rc3/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_buffer.py` & `shapely-2.0rc3/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_cga.py` & `shapely-2.0rc3/tests/test_cga.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_clip_by_rect.py` & `shapely-2.0rc3/tests/test_clip_by_rect.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_create_inconsistent_dimensionality.py` & `shapely-2.0rc3/tests/test_create_inconsistent_dimensionality.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_delaunay.py` & `shapely-2.0rc3/tests/test_delaunay.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_empty_polygons.py` & `shapely-2.0rc3/tests/test_empty_polygons.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_equality.py` & `shapely-2.0rc3/tests/test_equality.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_geointerface.py` & `shapely-2.0rc3/tests/test_geointerface.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_invalid_geometries.py` & `shapely-2.0rc3/tests/test_invalid_geometries.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_linear_referencing.py` & `shapely-2.0rc3/tests/test_linear_referencing.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_linemerge.py` & `shapely-2.0rc3/tests/test_linemerge.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_locale.py` & `shapely-2.0rc3/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_make_valid.py` & `shapely-2.0rc3/tests/test_make_valid.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_minimum_clearance.py` & `shapely-2.0rc3/tests/test_minimum_clearance.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_ndarrays.py` & `shapely-2.0rc3/tests/test_ndarrays.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_operations.py` & `shapely-2.0rc3/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_operators.py` & `shapely-2.0rc3/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_orient.py` & `shapely-2.0rc3/tests/test_orient.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_parallel_offset.py` & `shapely-2.0rc3/tests/test_parallel_offset.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_persist.py` & `shapely-2.0rc3/tests/test_persist.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_pickle.py` & `shapely-2.0rc3/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_polygonize.py` & `shapely-2.0rc3/tests/test_polygonize.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_polylabel.py` & `shapely-2.0rc3/tests/test_polylabel.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_predicates.py` & `shapely-2.0rc3/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_prepared.py` & `shapely-2.0rc3/tests/test_prepared.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_shape.py` & `shapely-2.0rc3/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_shared_paths.py` & `shapely-2.0rc3/tests/test_shared_paths.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_snap.py` & `shapely-2.0rc3/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_split.py` & `shapely-2.0rc3/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_substring.py` & `shapely-2.0rc3/tests/test_substring.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_svg.py` & `shapely-2.0rc3/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_transform.py` & `shapely-2.0rc3/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_union.py` & `shapely-2.0rc3/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_vectorized.py` & `shapely-2.0rc3/tests/test_vectorized.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_voronoi_diagram.py` & `shapely-2.0rc3/tests/test_voronoi_diagram.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_wkb.py` & `shapely-2.0rc3/tests/test_wkb.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/test_wkt.py` & `shapely-2.0rc3/tests/test_wkt.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/tests/threading_test.py` & `shapely-2.0rc3/tests/threading_test.py`

 * *Files identical despite different names*

### Comparing `shapely-2.0rc2/versioneer.py` & `shapely-2.0rc3/versioneer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 
-# Version: 0.18
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +187,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,36 +275,62 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable, Dict
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -317,128 +357,144 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Callable, Dict
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -468,84 +524,89 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
@@ -554,75 +615,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -630,52 +699,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -684,15 +793,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -709,21 +818,22 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
@@ -753,27 +863,75 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -796,20 +954,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -872,18 +1059,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -911,15 +1102,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -946,75 +1137,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1022,52 +1221,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1076,15 +1315,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1101,91 +1340,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1199,15 +1438,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1254,27 +1493,75 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -1297,20 +1584,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1373,18 +1689,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1476,35 +1796,39 @@
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1519,50 +1843,89 @@
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
@@ -1589,17 +1952,17 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1615,19 +1978,56 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -1683,29 +2083,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
 def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1721,62 +2126,36 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -1809,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

