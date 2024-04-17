# Comparing `tmp/rms-oops-0.0.2.tar.gz` & `tmp/rms_oops-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-oops-0.0.2.tar", last modified: Tue Jan 16 17:44:13 2024, max compression
+gzip compressed data, was "rms_oops-0.0.3.tar", last modified: Wed Apr 17 04:22:36 2024, max compression
```

## Comparing `rms-oops-0.0.2.tar` & `rms_oops-0.0.3.tar`

### file list

```diff
@@ -1,301 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.266928 rms-oops-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.218928 rms-oops-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.226928 rms-oops-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.github/workflows/run-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.github/workflows/run-windows-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-01-16 17:43:49.000000 rms-oops-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-01-16 17:43:49.000000 rms-oops-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-01-16 17:44:13.266928 rms-oops-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-16 17:43:49.000000 rms-oops-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.226928 rms-oops-0.0.2/ideas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.226928 rms-oops-0.0.2/ideas/cmodel_/
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3926 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/cmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2174 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/distance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1887 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/latitude.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2202 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/longitude.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/radius.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      652 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/cmodel_/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.226928 rms-oops-0.0.2/ideas/format_/
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/format_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1193 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/format_/format.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4732 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/format_/hms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1362 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/format_/pythonfmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/format_/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.226928 rms-oops-0.0.2/ideas/gll_ssi_masked/
--rwxr-xr-x   0 runner    (1001) docker     (127)    43215 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/gll_ssi_masked/backplane-__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45411 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/gll_ssi_masked/observation-__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14081 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/gll_ssi_masked/ssi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.230928 rms-oops-0.0.2/ideas/multipath/
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/multipath/multipath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.230928 rms-oops-0.0.2/ideas/nav_/
--rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6666 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/navigation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2149 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/nullnav.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6451 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/platescale.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10583 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/repointing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4459 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/timeshift.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      583 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/nav_/unittester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_frame_interpolation_using_matrix3.py.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.230928 rms-oops-0.0.2/ideas/old_observation_subclasses/
--rwxr-xr-x   0 runner    (1001) docker     (127)    21539 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_observation_subclasses/pushbroom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19409 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_observation_subclasses/pushframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28460 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_observation_subclasses/rasterscan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28080 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_observation_subclasses/rasterslit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22312 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/old_observation_subclasses/slit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.230928 rms-oops-0.0.2/ideas/packrat/
--rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/packrat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41206 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/packrat/packrat.py
--rw-r--r--   0 runner    (1001) docker     (127)    47188 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/packrat/packrat_arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/packrat/packrat_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/packrat/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16085 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/poleframe-with-tilt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8574 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.234928 rms-oops-0.0.2/ideas/shape2d/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10775 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/affine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7004 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/arc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15556 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/conic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32925 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    29842 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9657 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/point.py
--rw-r--r--   0 runner    (1001) docker     (127)    18016 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/shape2d/triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.234928 rms-oops-0.0.2/ideas/spice_starcat/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2011 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/make.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6395 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01.i
--rwxr-xr-x   0 runner    (1001) docker     (127)     2543 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4738 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01_interface.f
--rwxr-xr-x   0 runner    (1001) docker     (127)   118981 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01_wrap.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     3909 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/spice_starcat/strings.f
--rwxr-xr-x   0 runner    (1001) docker     (127)    17339 2024-01-16 17:43:49.000000 rms-oops-0.0.2/ideas/wobble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.238928 rms-oops-0.0.2/oops/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/.coveragerc
--rwxr-xr-x   0 runner    (1001) docker     (127)     2560 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-16 17:44:13.000000 rms-oops-0.0.2/oops/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.238928 rms-oops-0.0.2/oops/backplane/
--rwxr-xr-x   0 runner    (1001) docker     (127)    38796 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14163 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/ansa.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6927 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/border.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7763 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    99884 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/gold_master.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/lighting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11587 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/limb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3419 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/pole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/resolution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51688 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/ring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14140 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/sky.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24260 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/spheroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21353 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/backplane/where.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70794 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.242928 rms-oops-0.0.2/oops/cadence/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11134 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29573 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/dualcadence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/instant.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57751 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/metronome.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33319 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/reshapedcadence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12198 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/reversedcadence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18725 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/tdicadence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      847 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/cadence/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.242928 rms-oops-0.0.2/oops/calibration/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7969 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4360 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/extendedsource.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14220 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/flatcalib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4378 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/nullcalib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5029 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/pointsource.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13369 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/radiance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13101 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/rawcounts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/calibration/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21255 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      760 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   106278 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/event.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fittable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.246928 rms-oops-0.0.2/oops/fov/
--rw-r--r--   0 runner    (1001) docker     (127)    36798 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      898 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28001 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/barrelfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6323 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/flatfov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/gapfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12271 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/nullfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6558 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/offsetfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25290 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/polyfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26924 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/polynomialfov.py
--rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/radialfov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4379 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/slicefov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6518 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/subarray.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6898 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/subsampledfov.py
--rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/tdifov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/unittester.py
--rw-r--r--   0 runner    (1001) docker     (127)    28721 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/fov/wcsfov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.250928 rms-oops-0.0.2/oops/frame/
--rwxr-xr-x   0 runner    (1001) docker     (127)    53937 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1202 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13069 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/cmatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6173 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/inclinedframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9979 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/laplaceframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6010 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/navigation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19982 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/poleframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/postargframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11327 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/ringframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5977 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/rotation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32685 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/spiceframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8859 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/spicetype1frame.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8328 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/spinframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5278 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/synchronousframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7293 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/trackerframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5678 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/twovectorframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1239 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/frame/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.250928 rms-oops-0.0.2/oops/gravity/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5019 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/gravity/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/gravity/all.py
--rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/gravity/oblategravity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.250928 rms-oops-0.0.2/oops/hosts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.250928 rms-oops-0.0.2/oops/hosts/cassini/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/gold_master.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24834 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22276 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/iss_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/standard_obs.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21881 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/uvis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23388 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/uvis_test_suite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37906 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22140 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/cassini/vims_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/galileo/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12002 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/galileo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/galileo/ssi/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15506 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/galileo/ssi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/galileo/ssi/gold_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/galileo/ssi/standard_obs.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/galileo/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/hst/
--rwxr-xr-x   0 runner    (1001) docker     (127)    44796 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/hst/acs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3948 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/acs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/acs/hrc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3920 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/acs/sbc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7378 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/acs/wfc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/hst/nicmos/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6143 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/nicmos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/nicmos/nic1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/nicmos/nic2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2621 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/nicmos/nic3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/hst/wfc3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4953 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3/ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5224 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3/uvis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2501 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3/wfc3_pointing_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9572 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3/wfc3_test_suite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3_pointing_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12677 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfc3_test_suite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12280 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/hst/wfpc2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.254928 rms-oops-0.0.2/oops/hosts/juno/
--rw-r--r--   0 runner    (1001) docker     (127)    20306 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/juno/jiram/
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/jiram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/jiram/img.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/jiram/spe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/juno/junocam/
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/junocam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/junocam/gold_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/junocam/standard_obs.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/juno/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/jwst/
--rwxr-xr-x   0 runner    (1001) docker     (127)    21414 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/jwst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/jwst/nircam/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8235 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/jwst/nircam/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30553 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/jwst/nircam/uncal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/keck/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8715 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/keck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/keck/nirc2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7939 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/keck/nirc2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/keck/nirc2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/newhorizons/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5645 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/newhorizons/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26988 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/newhorizons/lorri.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/pds3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.258928 rms-oops-0.0.2/oops/hosts/voyager/
--rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/voyager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18998 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/hosts/voyager/iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14693 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/lightsource.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17836 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/meshgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.262928 rms-oops-0.0.2/oops/observation/
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/NOTES-ABOUT-OBSERVATION-CLASSES.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    49568 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/insitu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19395 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/pixel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21226 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/pushbroom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20422 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/pushframe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28362 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/rasterscan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29161 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/rasterslit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20723 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/rasterslit1d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22030 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/slit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15007 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/slit1d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32370 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/snapshot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70170 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/timedimage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1173 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/observation/unittester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.262928 rms-oops-0.0.2/oops/path/
--rwxr-xr-x   0 runner    (1001) docker     (127)    64953 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      839 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5711 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/circlepath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3428 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/coordpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3035 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/fixedpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43443 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/keplerpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3887 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/linearcoordpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3890 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/linearpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9284 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/multipath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37286 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/spicepath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/path/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/spice_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.266928 rms-oops-0.0.2/oops/surface/
--rwxr-xr-x   0 runner    (1001) docker     (127)    84590 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19898 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/ansa.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21862 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/centricellipsoid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19297 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/centricspheroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41671 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/ellipsoid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22354 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/graphicellipsoid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19326 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/graphicspheroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46515 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/limb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8942 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/nullsurface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28328 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/orbitplane.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9076 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/polarlimb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22063 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/ringplane.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25602 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/spheroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3250 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/spice_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/surface/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18045 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/transform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1014 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/unittester.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2744 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/unittester_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18859 2024-01-16 17:43:49.000000 rms-oops-0.0.2/oops/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-16 17:43:49.000000 rms-oops-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-16 17:43:49.000000 rms-oops-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.266928 rms-oops-0.0.2/rms_oops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-01-16 17:44:13.000000 rms-oops-0.0.2/rms_oops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-01-16 17:44:13.000000 rms-oops-0.0.2/rms_oops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 17:44:13.000000 rms-oops-0.0.2/rms_oops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-16 17:44:13.000000 rms-oops-0.0.2/rms_oops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-16 17:44:13.000000 rms-oops-0.0.2/rms_oops.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.222928 rms-oops-0.0.2/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.266928 rms-oops-0.0.2/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-01-16 17:43:49.000000 rms-oops-0.0.2/scripts/automated_tests/oops_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-16 17:44:13.270928 rms-oops-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:44:13.266928 rms-oops-0.0.2/spicedb/
--rwxr-xr-x   0 runner    (1001) docker     (127)   133536 2024-01-16 17:43:49.000000 rms-oops-0.0.2/spicedb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-01-16 17:43:49.000000 rms-oops-0.0.2/spicedb/sqlite_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.535551 rms_oops-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.487551 rms_oops-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.491551 rms_oops-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.github/workflows/run-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.github/workflows/run-windows-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-17 04:22:09.000000 rms_oops-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-17 04:22:09.000000 rms_oops-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-17 04:22:09.000000 rms_oops-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-17 04:22:09.000000 rms_oops-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-17 04:22:36.535551 rms_oops-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-17 04:22:09.000000 rms_oops-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 04:22:09.000000 rms_oops-0.0.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.491551 rms_oops-0.0.3/ideas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.495551 rms_oops-0.0.3/ideas/cmodel_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3926 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/cmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2174 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1887 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/latitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2202 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/longitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/radius.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      652 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/cmodel_/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.495551 rms_oops-0.0.3/ideas/format_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/format_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1193 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/format_/format.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4732 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/format_/hms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1362 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/format_/pythonfmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/format_/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.495551 rms_oops-0.0.3/ideas/gll_ssi_masked/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43215 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/gll_ssi_masked/backplane-__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45411 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/gll_ssi_masked/observation-__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14081 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/gll_ssi_masked/ssi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.495551 rms_oops-0.0.3/ideas/multipath/
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/multipath/multipath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.495551 rms_oops-0.0.3/ideas/nav_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6666 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/navigation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2149 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/nullnav.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6451 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/platescale.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10583 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/repointing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4459 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/timeshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      583 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/nav_/unittester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_frame_interpolation_using_matrix3.py.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.499551 rms_oops-0.0.3/ideas/old_observation_subclasses/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21539 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_observation_subclasses/pushbroom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19409 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_observation_subclasses/pushframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28460 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_observation_subclasses/rasterscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28080 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_observation_subclasses/rasterslit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22312 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/old_observation_subclasses/slit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.499551 rms_oops-0.0.3/ideas/packrat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/packrat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41206 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/packrat/packrat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47188 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/packrat/packrat_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/packrat/packrat_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/packrat/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16085 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/poleframe-with-tilt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8574 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.499551 rms_oops-0.0.3/ideas/shape2d/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10775 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/affine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7004 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/arc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15556 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/conic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32925 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29842 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9657 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18016 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/shape2d/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.503551 rms_oops-0.0.3/ideas/spice_starcat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2011 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/make.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6395 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01.i
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2543 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4738 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01_interface.f
+-rwxr-xr-x   0 runner    (1001) docker     (127)   118981 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01_wrap.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3909 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/spice_starcat/strings.f
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17339 2024-04-17 04:22:09.000000 rms_oops-0.0.3/ideas/wobble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.503551 rms_oops-0.0.3/oops/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/.coveragerc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2561 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 04:22:36.000000 rms_oops-0.0.3/oops/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.507551 rms_oops-0.0.3/oops/backplane/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38796 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14163 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/ansa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6927 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/border.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7763 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99884 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/gold_master.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/lighting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11587 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/limb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3419 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/pole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/resolution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51688 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/ring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14140 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/sky.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24260 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/spheroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21353 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/backplane/where.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70794 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.507551 rms_oops-0.0.3/oops/cadence/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11134 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29573 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/dualcadence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/instant.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57751 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/metronome.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33319 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/reshapedcadence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12198 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/reversedcadence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18725 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/tdicadence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      847 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/cadence/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.511551 rms_oops-0.0.3/oops/calibration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7969 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4360 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/extendedsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14220 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/flatcalib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4378 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/nullcalib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5029 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/pointsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13369 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/radiance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13101 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/rawcounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/calibration/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21255 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      760 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106278 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fittable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.511551 rms_oops-0.0.3/oops/fov/
+-rw-r--r--   0 runner    (1001) docker     (127)    36798 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      898 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28001 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/barrelfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6323 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/flatfov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/gapfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12271 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/nullfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6558 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/offsetfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25290 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/polyfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26924 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/polynomialfov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/radialfov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4379 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/slicefov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6518 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/subarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6898 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/subsampledfov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/tdifov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/unittester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28721 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/fov/wcsfov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.515551 rms_oops-0.0.3/oops/frame/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53937 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1202 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13069 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/cmatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6173 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/inclinedframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9979 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/laplaceframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6010 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/navigation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19982 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/poleframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/postargframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11327 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/ringframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5977 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/rotation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32685 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/spiceframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8859 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/spicetype1frame.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8328 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/spinframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5278 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/synchronousframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7293 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/trackerframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5678 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/twovectorframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1239 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/frame/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.515551 rms_oops-0.0.3/oops/gravity/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5019 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/gravity/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/gravity/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/gravity/oblategravity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.515551 rms_oops-0.0.3/oops/hosts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/cassini/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/gold_master.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24835 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22276 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/iss_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/standard_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21289 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/uvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23388 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/uvis_test_suite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38560 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22140 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/cassini/vims_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/galileo/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12002 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/galileo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/galileo/ssi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15506 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/galileo/ssi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/galileo/ssi/gold_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/galileo/ssi/standard_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/galileo/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/hst/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44796 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/hst/acs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3948 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/acs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/acs/hrc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3920 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/acs/sbc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7378 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/acs/wfc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.519551 rms_oops-0.0.3/oops/hosts/hst/nicmos/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6143 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/nicmos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/nicmos/nic1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/nicmos/nic2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2621 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/nicmos/nic3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/hst/wfc3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4953 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3/ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5224 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3/uvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2501 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3/wfc3_pointing_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9572 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3/wfc3_test_suite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3_pointing_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12677 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfc3_test_suite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12280 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/hst/wfpc2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/juno/
+-rw-r--r--   0 runner    (1001) docker     (127)    20306 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/juno/jiram/
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/jiram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/jiram/img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/jiram/spe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/juno/junocam/
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/junocam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/junocam/gold_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/junocam/standard_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/juno/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/jwst/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21414 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/jwst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/jwst/nircam/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8235 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/jwst/nircam/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30553 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/jwst/nircam/uncal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/keck/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8715 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/keck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/keck/nirc2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7939 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/keck/nirc2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/keck/nirc2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/newhorizons/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5645 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/newhorizons/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27031 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/newhorizons/lorri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/pds3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.523551 rms_oops-0.0.3/oops/hosts/voyager/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/voyager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18987 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/hosts/voyager/iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14693 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/lightsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17836 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/meshgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.527552 rms_oops-0.0.3/oops/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/NOTES-ABOUT-OBSERVATION-CLASSES.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49568 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/insitu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19395 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/pixel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21226 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/pushbroom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20422 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/pushframe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28362 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/rasterscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29161 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/rasterslit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20723 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/rasterslit1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22030 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/slit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15007 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/slit1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32370 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/snapshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70170 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/timedimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1173 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/observation/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.527552 rms_oops-0.0.3/oops/path/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64953 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      839 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5711 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/circlepath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3428 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/coordpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3035 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/fixedpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43443 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/keplerpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3887 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/linearcoordpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3890 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/linearpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9284 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/multipath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37286 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/spicepath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/path/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/spice_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.531551 rms_oops-0.0.3/oops/surface/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84590 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19898 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/ansa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21862 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/centricellipsoid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19297 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/centricspheroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41671 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/ellipsoid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22354 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/graphicellipsoid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19326 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/graphicspheroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46515 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/limb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8942 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/nullsurface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28328 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/orbitplane.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9076 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/polarlimb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22063 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/ringplane.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25602 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/spheroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3250 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/spice_shape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/surface/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18045 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1014 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/unittester.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2744 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/unittester_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18859 2024-04-17 04:22:09.000000 rms_oops-0.0.3/oops/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-17 04:22:09.000000 rms_oops-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 04:22:09.000000 rms_oops-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.531551 rms_oops-0.0.3/rms_oops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-17 04:22:36.000000 rms_oops-0.0.3/rms_oops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-17 04:22:36.000000 rms_oops-0.0.3/rms_oops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:22:36.000000 rms_oops-0.0.3/rms_oops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-17 04:22:36.000000 rms_oops-0.0.3/rms_oops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 04:22:36.000000 rms_oops-0.0.3/rms_oops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.491551 rms_oops-0.0.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.531551 rms_oops-0.0.3/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-04-17 04:22:09.000000 rms_oops-0.0.3/scripts/automated_tests/oops_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 04:22:36.535551 rms_oops-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:22:36.531551 rms_oops-0.0.3/spicedb/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   133536 2024-04-17 04:22:09.000000 rms_oops-0.0.3/spicedb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-04-17 04:22:09.000000 rms_oops-0.0.3/spicedb/sqlite_db.py
```

### Comparing `rms-oops-0.0.2/.github/workflows/publish_to_pypi.yml` & `rms_oops-0.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Publish to PyPI
-run-name: Publish to PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   release:
     types: [published]
 
 jobs:
   upload_pypi:
@@ -11,15 +11,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-oops-0.0.2/.github/workflows/publish_to_test_pypi.yml` & `rms_oops-0.0.3/.github/workflows/publish_to_test_pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-oops-0.0.2/.github/workflows/run-lint.yml` & `rms_oops-0.0.3/.github/workflows/run-lint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Lint
-run-name: Run Lint triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Lint: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   # pull_request:
   #   branches: [ master ]
   # push:
   #   branches: [ master ]
@@ -17,15 +17,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Run flake8 on oops
         run: |
           flake8 oops
```

### Comparing `rms-oops-0.0.2/.github/workflows/run-tests.yml` & `rms_oops-0.0.3/.github/workflows/run-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 name: Test oops
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
   push:
-    branches: [ master ]
+    branches: [ main ]
   schedule:
     - cron: "00 09 * * *"   # 1am PST, 2am PDT
 
 jobs:
   test:
     name: Test oops
     runs-on: ${{ matrix.os }}
@@ -46,15 +46,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Test with coverage
         run: |
           scripts/automated_tests/oops_main_test.sh
         shell: bash
```

### Comparing `rms-oops-0.0.2/.github/workflows/run-windows-tests.yml` & `rms_oops-0.0.3/.github/workflows/run-windows-tests.yml`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/.gitignore` & `rms_oops-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/LICENSE.md` & `rms_oops-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/__init__.py` & `rms_oops-0.0.3/ideas/cmodel_/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/cmodel.py` & `rms_oops-0.0.3/ideas/cmodel_/cmodel.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/distance.py` & `rms_oops-0.0.3/ideas/cmodel_/distance.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/latitude.py` & `rms_oops-0.0.3/ideas/cmodel_/latitude.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/longitude.py` & `rms_oops-0.0.3/ideas/cmodel_/longitude.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/radius.py` & `rms_oops-0.0.3/ideas/cmodel_/radius.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/cmodel_/unittester.py` & `rms_oops-0.0.3/ideas/cmodel_/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/format_/format.py` & `rms_oops-0.0.3/ideas/format_/format.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/format_/hms.py` & `rms_oops-0.0.3/ideas/format_/hms.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/format_/pythonfmt.py` & `rms_oops-0.0.3/ideas/format_/pythonfmt.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/format_/unittester.py` & `rms_oops-0.0.3/ideas/format_/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/gll_ssi_masked/backplane-__init__.py` & `rms_oops-0.0.3/ideas/gll_ssi_masked/backplane-__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/gll_ssi_masked/observation-__init__.py` & `rms_oops-0.0.3/ideas/gll_ssi_masked/observation-__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/gll_ssi_masked/ssi.py` & `rms_oops-0.0.3/ideas/gll_ssi_masked/ssi.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/multipath/multipath.py` & `rms_oops-0.0.3/ideas/multipath/multipath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/navigation.py` & `rms_oops-0.0.3/ideas/nav_/navigation.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/nullnav.py` & `rms_oops-0.0.3/ideas/nav_/nullnav.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/platescale.py` & `rms_oops-0.0.3/ideas/nav_/platescale.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/repointing.py` & `rms_oops-0.0.3/ideas/nav_/repointing.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/timeshift.py` & `rms_oops-0.0.3/ideas/nav_/timeshift.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/nav_/unittester.py` & `rms_oops-0.0.3/ideas/nav_/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_frame_interpolation_using_matrix3.py.txt` & `rms_oops-0.0.3/ideas/old_frame_interpolation_using_matrix3.py.txt`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_observation_subclasses/pushbroom.py` & `rms_oops-0.0.3/ideas/old_observation_subclasses/pushbroom.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_observation_subclasses/pushframe.py` & `rms_oops-0.0.3/ideas/old_observation_subclasses/pushframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_observation_subclasses/rasterscan.py` & `rms_oops-0.0.3/ideas/old_observation_subclasses/rasterscan.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_observation_subclasses/rasterslit.py` & `rms_oops-0.0.3/ideas/old_observation_subclasses/rasterslit.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/old_observation_subclasses/slit.py` & `rms_oops-0.0.3/ideas/old_observation_subclasses/slit.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/packrat/packrat.py` & `rms_oops-0.0.3/ideas/packrat/packrat.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/packrat/packrat_arrays.py` & `rms_oops-0.0.3/ideas/packrat/packrat_arrays.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/packrat/unittester.py` & `rms_oops-0.0.3/ideas/packrat/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/poleframe-with-tilt.py` & `rms_oops-0.0.3/ideas/poleframe-with-tilt.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/registry.py` & `rms_oops-0.0.3/ideas/registry.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/__init__.py` & `rms_oops-0.0.3/ideas/shape2d/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/affine.py` & `rms_oops-0.0.3/ideas/shape2d/affine.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/arc.py` & `rms_oops-0.0.3/ideas/shape2d/arc.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/circle.py` & `rms_oops-0.0.3/ideas/shape2d/circle.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/conic.py` & `rms_oops-0.0.3/ideas/shape2d/conic.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/ellipse.py` & `rms_oops-0.0.3/ideas/shape2d/ellipse.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/line.py` & `rms_oops-0.0.3/ideas/shape2d/line.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/point.py` & `rms_oops-0.0.3/ideas/shape2d/point.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/polygon.py` & `rms_oops-0.0.3/ideas/shape2d/polygon.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/shape2d/triangle.py` & `rms_oops-0.0.3/ideas/shape2d/triangle.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/__init__.py` & `rms_oops-0.0.3/ideas/spice_starcat/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/make.sh` & `rms_oops-0.0.3/ideas/spice_starcat/make.sh`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01.i` & `rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01.i`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01.py` & `rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01_interface.f` & `rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01_interface.f`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/spice_stcx01_wrap.c` & `rms_oops-0.0.3/ideas/spice_starcat/spice_stcx01_wrap.c`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/spice_starcat/strings.f` & `rms_oops-0.0.3/ideas/spice_starcat/strings.f`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/ideas/wobble.py` & `rms_oops-0.0.3/ideas/wobble.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/__init__.py` & `rms_oops-0.0.3/oops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from oops.constants import C, C_INVERSE, RPD, DPR, SPR, RPS, SPD, AU, \
                            PI, TWOPI, HALFPI
 
 from polymath import Boolean, Matrix, Matrix3, Pair, Quaternion, Qube, Scalar, \
                      Units, Vector, Vector3
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 ################################################################################
 # Class cross-references and other class attributes to be defined after startup
 ################################################################################
```

### Comparing `rms-oops-0.0.2/oops/backplane/__init__.py` & `rms_oops-0.0.3/oops/backplane/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/all.py` & `rms_oops-0.0.3/oops/backplane/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/ansa.py` & `rms_oops-0.0.3/oops/backplane/ansa.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/border.py` & `rms_oops-0.0.3/oops/backplane/border.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/distance.py` & `rms_oops-0.0.3/oops/backplane/distance.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/gold_master.py` & `rms_oops-0.0.3/oops/backplane/gold_master.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/lighting.py` & `rms_oops-0.0.3/oops/backplane/lighting.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/limb.py` & `rms_oops-0.0.3/oops/backplane/limb.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/orbit.py` & `rms_oops-0.0.3/oops/backplane/orbit.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/pole.py` & `rms_oops-0.0.3/oops/backplane/pole.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/resolution.py` & `rms_oops-0.0.3/oops/backplane/resolution.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/ring.py` & `rms_oops-0.0.3/oops/backplane/ring.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/sky.py` & `rms_oops-0.0.3/oops/backplane/sky.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/spheroid.py` & `rms_oops-0.0.3/oops/backplane/spheroid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/backplane/where.py` & `rms_oops-0.0.3/oops/backplane/where.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/body.py` & `rms_oops-0.0.3/oops/body.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/__init__.py` & `rms_oops-0.0.3/oops/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/all.py` & `rms_oops-0.0.3/oops/cadence/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/dualcadence.py` & `rms_oops-0.0.3/oops/cadence/dualcadence.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/instant.py` & `rms_oops-0.0.3/oops/cadence/instant.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/metronome.py` & `rms_oops-0.0.3/oops/cadence/metronome.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/reshapedcadence.py` & `rms_oops-0.0.3/oops/cadence/reshapedcadence.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/reversedcadence.py` & `rms_oops-0.0.3/oops/cadence/reversedcadence.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/sequence.py` & `rms_oops-0.0.3/oops/cadence/sequence.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/tdicadence.py` & `rms_oops-0.0.3/oops/cadence/tdicadence.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/cadence/unittester.py` & `rms_oops-0.0.3/oops/cadence/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/__init__.py` & `rms_oops-0.0.3/oops/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/all.py` & `rms_oops-0.0.3/oops/calibration/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/extendedsource.py` & `rms_oops-0.0.3/oops/calibration/extendedsource.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/flatcalib.py` & `rms_oops-0.0.3/oops/calibration/flatcalib.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/nullcalib.py` & `rms_oops-0.0.3/oops/calibration/nullcalib.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/pointsource.py` & `rms_oops-0.0.3/oops/calibration/pointsource.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/radiance.py` & `rms_oops-0.0.3/oops/calibration/radiance.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/rawcounts.py` & `rms_oops-0.0.3/oops/calibration/rawcounts.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/calibration/unittester.py` & `rms_oops-0.0.3/oops/calibration/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/config.py` & `rms_oops-0.0.3/oops/config.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/constants.py` & `rms_oops-0.0.3/oops/constants.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/event.py` & `rms_oops-0.0.3/oops/event.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fittable.py` & `rms_oops-0.0.3/oops/fittable.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/__init__.py` & `rms_oops-0.0.3/oops/fov/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/all.py` & `rms_oops-0.0.3/oops/fov/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/barrelfov.py` & `rms_oops-0.0.3/oops/fov/barrelfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/flatfov.py` & `rms_oops-0.0.3/oops/fov/flatfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/gapfov.py` & `rms_oops-0.0.3/oops/fov/gapfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/nullfov.py` & `rms_oops-0.0.3/oops/fov/nullfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/offsetfov.py` & `rms_oops-0.0.3/oops/fov/offsetfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/polyfov.py` & `rms_oops-0.0.3/oops/fov/polyfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/polynomialfov.py` & `rms_oops-0.0.3/oops/fov/polynomialfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/radialfov.py` & `rms_oops-0.0.3/oops/fov/radialfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/slicefov.py` & `rms_oops-0.0.3/oops/fov/slicefov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/subarray.py` & `rms_oops-0.0.3/oops/fov/subarray.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/subsampledfov.py` & `rms_oops-0.0.3/oops/fov/subsampledfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/tdifov.py` & `rms_oops-0.0.3/oops/fov/tdifov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/unittester.py` & `rms_oops-0.0.3/oops/fov/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/fov/wcsfov.py` & `rms_oops-0.0.3/oops/fov/wcsfov.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/__init__.py` & `rms_oops-0.0.3/oops/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/all.py` & `rms_oops-0.0.3/oops/frame/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/cmatrix.py` & `rms_oops-0.0.3/oops/frame/cmatrix.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/inclinedframe.py` & `rms_oops-0.0.3/oops/frame/inclinedframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/laplaceframe.py` & `rms_oops-0.0.3/oops/frame/laplaceframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/navigation.py` & `rms_oops-0.0.3/oops/frame/navigation.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/poleframe.py` & `rms_oops-0.0.3/oops/frame/poleframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/postargframe.py` & `rms_oops-0.0.3/oops/frame/postargframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/ringframe.py` & `rms_oops-0.0.3/oops/frame/ringframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/rotation.py` & `rms_oops-0.0.3/oops/frame/rotation.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/spiceframe.py` & `rms_oops-0.0.3/oops/frame/spiceframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/spicetype1frame.py` & `rms_oops-0.0.3/oops/frame/spicetype1frame.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/spinframe.py` & `rms_oops-0.0.3/oops/frame/spinframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/synchronousframe.py` & `rms_oops-0.0.3/oops/frame/synchronousframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/trackerframe.py` & `rms_oops-0.0.3/oops/frame/trackerframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/twovectorframe.py` & `rms_oops-0.0.3/oops/frame/twovectorframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/frame/unittester.py` & `rms_oops-0.0.3/oops/frame/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/gravity/__init__.py` & `rms_oops-0.0.3/oops/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/gravity/oblategravity.py` & `rms_oops-0.0.3/oops/gravity/oblategravity.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/__init__.py` & `rms_oops-0.0.3/oops/hosts/cassini/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/iss.py` & `rms_oops-0.0.3/oops/hosts/cassini/iss.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     Cassini.load_cks( tdb0, tdb1)
     Cassini.load_spks(tdb0, tdb1)
 
     return snapshots
 
 #===============================================================================
-def initialize(ck='reconstructed', planets=None, offset_wac=True, asof=None,
+def initialize(ck='reconstructed', planets=None, offset_wac=False, asof=None,
                spk='reconstructed', gapfill=True,
                mst_pck=True, irregulars=True):
     """Initialize key information about the ISS instrument.
 
     Must be called first. After the first call, later calls to this function
     are ignored.
```

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/iss_test_suite.py` & `rms_oops-0.0.3/oops/hosts/cassini/iss_test_suite.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/standard_obs.py` & `rms_oops-0.0.3/oops/hosts/cassini/standard_obs.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/uvis.py` & `rms_oops-0.0.3/oops/hosts/cassini/uvis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-################################################################################
+##########################################################################################
 # oops/hosts/cassini/uvis.py
-################################################################################
+##########################################################################################
 
-import oops
 import numpy as np
 import numbers
 import os
+
 import julian
+import oops
 import pdsparser
 
 from oops.hosts.cassini import Cassini
+from oops.hosts         import pds3
 
 DEBUG = False       # True to assert that the data array must have null
                     # values outside the active windows
 
-################################################################################
+##########################################################################################
 # Standard class methods
-################################################################################
+##########################################################################################
 
 def from_file(filespec, data=True, enclose=False, **parameters):
     """A general, static method to return one or more Observation subclass
     objects based on a label for a given Cassini UVIS file.
 
     Input:
         filespec        the full path to the PDS label of a UVIS data file.
         data            True to include the data array.
-        enclose         True to return a single observation, regardless of how
-                        many windows are defined. If multiple windows are used,
-                        then the observation (and the optional data array) are
-                        are defined by the enclosing limits in line and band,
-                        and the binning is assumed to be 1. If False and
-                        multiple windows are used, the function returns a tuple
-                        of observations rather than a single observation.
+        enclose         True to return a single observation, regardless of how many
+                        windows are defined. If multiple windows are used, then the
+                        observation (and the optional data array) are are defined by the
+                        enclosing limits in line and band, and the binning is assumed to
+                        be 1. If False and multiple windows are used, the function returns
+                        a tuple of observations rather than a single observation.
     """
-    UVIS.initialize()   # Define everything the first time through; use defaults
-                        # unless initialize() is called explicitly.
 
-    # Load the PDS label
-    recs = pdsparser.PdsLabel.load_file(filespec)
-
-    # Deal with corrupt syntax
-    for i in range(len(recs)):
-        rec = recs[i]
-        if 'CORE_UNIT' in rec:
-            if '"COUNTS/BIN"' not in rec:
-                recs[i] = rec.replace('COUNTS/BIN', '"COUNTS/BIN"')
-        if rec.startswith('ODC_ID'):
-            recs[i] = rec.replace(',', '')
+    UVIS.initialize()   # Define everything the first time through; use defaults unless
+                        # initialize() is called explicitly.
 
     # Get the label dictionary and data array dimensions
-    label = pdsparser.PdsLabel.from_string(recs).as_dict()
+    label = pds3.fast_dict(filespec)
 
     # Load any needed SPICE kernels
     tstart = julian.tdb_from_tai(julian.tai_from_iso(label['START_TIME']))
     tstop  = julian.tdb_from_tai(julian.tai_from_iso(label['STOP_TIME']))
     Cassini.load_cks( tstart, tstop)
     Cassini.load_spks(tstart, tstop)
 
@@ -61,15 +51,15 @@
     if 'QUBE' in label:
         return get_qube(filespec, tstart, label, data, enclose)
     elif 'TIME_SERIES' in label:
         return get_time_series(filespec, tstart, label, data)
     else:
         return get_spectrum(filespec, tstart, label, data)
 
-#===============================================================================
+#=========================================================================================
 def get_qube(filespec, tstart, label, data, enclose):
     """The observation object given that it is a QUBE."""
 
     global DEBUG
 
     # Determine the detector and mode
     detector = label['PRODUCT_ID'][:3]
@@ -79,15 +69,15 @@
 
     # Define the instrument frame
     frame_id = UVIS.frame_ids[detector]
 
     # Get array shape
     info = label['QUBE']
     (bands,lines,samples) = info['CORE_ITEMS']
-    assert lines in (1,64)
+    assert lines in (1,64), f'invalid lines = {lines}'
 
     if lines == 1:
         shape = (samples, bands)
     else:
         shape = (lines, samples, bands)
 
     # Define the cadence
@@ -169,15 +159,15 @@
                                lines, line0[w], line1[w]+1, line_bin[w],
                                bands, band0[w], band1[w]+1, band_bin[w],
                                rebin=True)
             obslist.append(obs)
 
         return tuple(obslist)
 
-#===============================================================================
+#=========================================================================================
 def get_one_qube(label, detector, resolution,
                  fov, cadence, frame_id,
                  shape, array, samples,
                  lines, line0, line1, line_bin,
                  bands, band0, band1, band_bin,
                  rebin):
     """A single Observation object for the identified window of the UVIS qube."""
@@ -201,43 +191,42 @@
         if array is not None:
             array = array[..., band0:band1]
 
     # Bin the lines
     if rebin and line_bin > 1:
         assert dline % line_bin == 0
         fov = oops.fov.SubsampledFOV(fov, (1,line_bin))
-        dline_binned = dline / line_bin
+        dline_binned = dline // line_bin
         shape = (dline_binned,) + shape[1:]
 
         if array is not None:
             if DEBUG:
                 assert np.all(array[dline_binned:, ...] == array_null)
 
             array = array[:dline_binned]
 
     # Bin the bands
     if rebin and band_bin > 1:
         if DEBUG:
             assert dband % band_bin == 0    # seen to fail occasionally
 
-        dband_binned = dband / band_bin
+        dband_binned = dband // band_bin
         shape = shape[:-1] + (dband_binned,)
 
         if array is not None:
             if DEBUG:
                 assert np.all(array[..., dband_binned:] == array_null)
 
             array = array[..., :dband_binned]
 
     # Create the Observation
     if lines == 1:
         obs = oops.obs.Pixel(('t','b'), cadence, fov, 'CASSINI', frame_id)
     else:
-        obs = oops.obs.TimedImage(('v','ut','b'), 1, cadence, fov,
-                                  'CASSINI', frame_id)
+        obs = oops.obs.TimedImage(('v','ut','b'), cadence, fov, 'CASSINI', frame_id)
 
     obs.insert_subfield('dict', label)
     obs.insert_subfield('instrument', 'UVIS')
     obs.insert_subfield('detector', detector)
     obs.insert_subfield('sampling', resolution)
     obs.insert_subfield('product_type', 'QUBE')
 
@@ -253,15 +242,15 @@
         obs.insert_subfield('data', array)
 
     # Update the observation shape
     obs.shape = shape
 
     return obs
 
-#===============================================================================
+#=========================================================================================
 def get_time_series(filespec, tstart, label, data):
     """The observation object given that it is a TIME_SERIES."""
 
     # Determine the detector
     product_id = label['PRODUCT_ID']
     if product_id.startswith('HSP'):
         detector = 'HSP'
@@ -312,15 +301,15 @@
         obs.insert_subfield('data', array)
 
     # Update the observation shape
     obs.shape = (samples,)
 
     return obs
 
-#===============================================================================
+#=========================================================================================
 def get_spectrum(filespec, tstart, label, data):
     """The observation object given that it is a SPECTRUM."""
 
     # Determine the detector
     detector = label['PRODUCT_ID'][:3]
     assert detector in ('EUV', 'FUV')
 
@@ -377,35 +366,34 @@
         obs.insert_subfield('data', array)
 
     # Update the observation shape
     obs.shape = (bands,)
 
     return obs
 
-#===============================================================================
+#=========================================================================================
 def load_data(filespec, body, dtype):
 
     head = os.path.split(filespec)[0]
 
     data_filespec = os.path.join(head, body)
     if not os.path.exists(data_filespec):
         data_filespec = os.path.join(head, body.lower())
     if not os.path.exists(data_filespec):
         f = open(data_filespec,'r')     # raise IOError
 
     return np.fromfile(data_filespec, sep='', dtype=dtype)
 
-#===============================================================================
+#=========================================================================================
 def initialize(ck='reconstructed', planets=None, asof=None,
                spk='reconstructed', gapfill=True,
                mst_pck=True, irregulars=True):
     """Initialize key information about the VIMS instrument.
 
-    Must be called first. After the first call, later calls to this function
-    are ignored.
+    Must be called first. After the first call, later calls to this function are ignored.
 
     Input:
         ck,spk      'predicted', 'reconstructed', or 'none', depending on
                     which kernels are to be used. Defaults are 'reconstructed'.
                     Use 'none' if the kernels are to be managed manually.
         planets     A list of planets to pass to define_solar_system. None or
                     0 means all.
@@ -413,18 +401,18 @@
                     None to ignore.
         gapfill     True to include gapfill CKs. False otherwise.
         mst_pck     True to include MST PCKs, which update the rotation models
                     for some of the small moons.
         irregulars  True to include the irregular satellites;
                     False otherwise.
     """
-    UVIS.initialize(ck=ck, planets=planets, asof=asof, spk=spk,
-                    gapfill=gapfill, mst_pck=mst_pck, irregulars=irregulars)
+    UVIS.initialize(ck=ck, planets=planets, asof=asof, spk=spk, gapfill=gapfill,
+                    mst_pck=mst_pck, irregulars=irregulars)
 
-#===============================================================================
+#=========================================================================================
 class UVIS(object):
     """An instance-free class to hold Cassini UVIS instrument parameters."""
 
     instrument_kernel = None
     fovs = {}
     initialized = False
 
@@ -444,46 +432,42 @@
     frame_ids = {'FUV'    : 'CASSINI_UVIS_FUV',
                  'EUV'    : 'CASSINI_UVIS_EUV',
                  'SOLAR'  : 'CASSINI_UVIS_SOLAR',
                  'SOL_OFF': 'CASSINI_UVIS_SOL_OFF',
                  'HSP'    : 'CASSINI_UVIS_HSP',
                  'HDAC'   : 'CASSINI_UVIS_HDAC'}
 
-    #===========================================================================
+    #=====================================================================================
     @staticmethod
-    def initialize(ck='reconstructed', planets=None, asof=None,
-                   spk='reconstructed', gapfill=True,
-                   mst_pck=True, irregulars=True):
+    def initialize(ck='reconstructed', planets=None, asof=None, spk='reconstructed',
+                   gapfill=True, mst_pck=True, irregulars=True):
         """Fill in key information about the UVIS channels.
 
-        Must be called first. After the first call, later calls to this function
-        are ignored.
+        Must be called first. After the first call, later calls to this function are
+        ignored.
 
         Input:
-            ck,spk      'predicted', 'reconstructed', or 'none', depending on
-                        which kernels are to be used. Defaults are
-                        'reconstructed'. Use 'none' if the kernels are to be
-                        managed manually.
-            planets     A list of planets to pass to define_solar_system. None
-                        or 0 means all.
-            asof        Only use SPICE kernels that existed before this date;
-                        None to ignore.
+            ck,spk      'predicted', 'reconstructed', or 'none', depending on which
+                        kernels are to be used. Defaults are 'reconstructed'. Use 'none'
+                        if the kernels are to be managed manually.
+            planets     A list of planets to pass to define_solar_system. None or 0 means
+                        all.
+            asof        Only use SPICE kernels that existed before this date; None to
+                        ignore.
             gapfill     True to include gapfill CKs. False otherwise.
-            mst_pck     True to include MST PCKs, which update the rotation
-                        models for some of the small moons.
-            irregulars  True to include the irregular satellites;
-                        False otherwise.
+            mst_pck     True to include MST PCKs, which update the rotation models for
+                        some of the small moons.
+            irregulars  True to include the irregular satellites; False otherwise.
         """
 
         # Quick exit after first call
         if UVIS.initialized:
             return
 
-        Cassini.initialize(ck=ck, planets=planets, asof=asof, spk=spk,
-                           gapfill=gapfill,
+        Cassini.initialize(ck=ck, planets=planets, asof=asof, spk=spk, gapfill=gapfill,
                            mst_pck=mst_pck, irregulars=irregulars)
         Cassini.load_instruments(asof=asof)
 
         # Load the instrument kernel
         UVIS.instrument_kernel = Cassini.spice_instrument_kernel('UVIS')[0]
 
         # TEMPORARY FIX to a loader problem
@@ -522,43 +506,35 @@
             # Not every combination is really used but that doesn't matter
             for lines in {1, 64}:
                 fov = oops.fov.FlatFOV((u_angle, v_angle/lines), (1,lines))
                 UVIS.fovs[(detector, resolution, lines)] = fov
 
         UVIS.initialized = True
 
-    #===========================================================================
+    #=====================================================================================
     @staticmethod
     def reset():
         """Resets the internal Cassini UVIS parameters. Can be useful for
         debugging.
         """
 
         UVIS.instrument_kernel = None
         UVIS.fovs = {}
         UVIS.initialized = False
 
         Cassini.reset()
 
-################################################################################
+##########################################################################################
 # UNIT TESTS
-################################################################################
+##########################################################################################
 import unittest
 import os.path
 import oops.backplane.gold_master as gm
 
-from oops.unittester_support    import TESTDATA_PARENT_DIRECTORY
-
-
-#===============================================================================
-class Test_Cassini_UVIS(unittest.TestCase):
-
-    #===========================================================================
-    def runTest(self):
-        pass
+from oops.unittester_support import TESTDATA_PARENT_DIRECTORY
 
 
 #===============================================================================
 class Test_Cassini_UVIS_GoldMaster_HSP2014_197_21_29(unittest.TestCase):
 
     #===========================================================================
     def runTest(self):
@@ -578,14 +554,15 @@
             python gold_master.py \
                 ~/Dropbox-SETI/OOPS-Resources/test_data/cassini/UVIS/HSP2014_197_21_29.DAT \
                 --module hosts.cassini.uvis \
                 --ring SATURN_MAIN_RINGS \
                 --no-inventory \
                 --adopt
         """
+
         gm.execute_as_unittest(self,
                 obspath = os.path.join(TESTDATA_PARENT_DIRECTORY,
                                        'cassini/UVIS/HSP2014_197_21_29.DAT'),
                 index   = None,
                 module  = 'oops.hosts.cassini.uvis',
                 planet  = '',
                 moon    = '',
```

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/uvis_test_suite.py` & `rms_oops-0.0.3/oops/hosts/cassini/uvis_test_suite.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/vims.py` & `rms_oops-0.0.3/oops/hosts/cassini/vims.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-################################################################################
+##########################################################################################
 # oops/hosts/cassini/vims.py
 #
 # Known shortcomings:
 #
-# For SAMPLING_MODE_ID == "UNDER" (aka Nyquist sampling), the FOV boundary will
-# be slightly off because an FOV object cannot handle overlapping, double-sized
-# pixels. The proper boundary is 1/64th larger along the line direction to
-# account for the larger pixel.
-################################################################################
+# For SAMPLING_MODE_ID == "UNDER" (aka Nyquist sampling), the FOV boundary will be
+# be slightly off because an FOV object cannot handle overlapping, double-sized pixels.
+# The proper boundary is 1/64th larger along the line direction to account for the larger
+# pixel.
+##########################################################################################
 
 import numpy as np
-import numpy.lib.stride_tricks
+from numpy.lib import stride_tricks
 
 import julian
 import pdsparser
 import cspyce
 import oops
 
 from oops.hosts.cassini import Cassini
+from oops.hosts.pds3    import pds3
 
 # Timing correction as of 1/9/15 -- MRS
 # EXTRA_INTERSAMPLE_DELAY =  0.000363     # observed empirically in V1555349441
 # TIME_CORRECTION         = -0.337505
 
 TIME_FACTOR = 1.01725
 
@@ -68,336 +69,434 @@
                              VIS_NORMAL_PIXEL/VIS_HIRES_FACTOR))
 
 IR_OVER_VIS = IR_NORMAL_PIXEL / VIS_NORMAL_PIXEL
 
 IR_FULL_FOV  = oops.fov.FlatFOV(IR_NORMAL_SCALE,  oops.Pair((64,64)))
 VIS_FULL_FOV = oops.fov.FlatFOV(VIS_NORMAL_SCALE, oops.Pair((64,64)))
 
-################################################################################
+##########################################################################################
+# FMT files have fixed values
+##########################################################################################
+
+CORE_DESCRIPTION_FMT = pds3.fast_dict("""\
+  CORE_ITEM_BYTES                = 2
+  CORE_ITEM_TYPE                 = SUN_INTEGER
+  CORE_BASE                      = 0.0
+  CORE_MULTIPLIER                = 1.0
+  CORE_VALID_MINIMUM             = -4095
+  CORE_NULL                      = -8192
+  CORE_LOW_REPR_SATURATION       = -32767
+  CORE_LOW_INSTR_SATURATION      = -32766
+  CORE_HIGH_REPR_SATURATION      = -32764
+  CORE_HIGH_INSTR_SATURATION     = -32765
+  CORE_MINIMUM_DN                = -122
+  CORE_NAME                      = "RAW DATA NUMBER"
+  CORE_UNIT                      = DIMENSIONLESS
+""")
+
+SUFFIX_DESCRIPTION_FMT = pds3.fast_dict("""\
+  GROUP                          = SAMPLE_SUFFIX
+    SUFFIX_NAME                  = BACKGROUND
+    SUFFIX_UNIT                  = DIMENSIONLESS
+    SUFFIX_ITEM_BYTES            = 4
+    SUFFIX_ITEM_TYPE             = SUN_INTEGER
+    SUFFIX_BASE                  = 0.0
+    SUFFIX_MULTIPLIER            = 1.0
+    SUFFIX_VALID_MINIMUM         = 0
+    SUFFIX_NULL                  = -8192
+    SUFFIX_LOW_REPR_SAT          = -32767
+    SUFFIX_LOW_INSTR_SAT         = -32766
+    SUFFIX_HIGH_REPR_SAT         = -32764
+    SUFFIX_HIGH_INSTR_SAT        = -32765
+  END_GROUP                      = SAMPLE_SUFFIX
+
+  GROUP                          = BAND_SUFFIX
+    SUFFIX_NAME                  = (X_SCAN_DRIVE_CURRENT,
+                                    Z_SCAN_DRIVE_CURRENT,
+                                    X_SCAN_MIRROR_POSITION,
+                                    Z_SCAN_MIRROR_POSITION)
+    SUFFIX_UNIT                  = (DIMENSIONLESS,DIMENSIONLESS,
+                                    DIMENSIONLESS,DIMENSIONLESS)
+    SUFFIX_ITEM_TYPE             = (SUN_INTEGER,SUN_INTEGER,
+                                    SUN_INTEGER,SUN_INTEGER)
+    SUFFIX_ITEM_BYTES            = (4,4,4,4)
+    SUFFIX_BASE                  = (0.0,0.0,0.0,0.0)
+    SUFFIX_MULTIPLIER            = (1.0,1.0,1.0,1.0)
+    SUFFIX_VALID_MINIMUM         = (0,0,0,0)
+    SUFFIX_NULL                  = (-8192,-8192,-8192,-8192)
+    SUFFIX_LOW_REPR_SAT          = (-32767,-32767,-32767,-32767)
+    SUFFIX_LOW_INSTR_SAT         = (-32766,-32766,-32766,-32766)
+    SUFFIX_HIGH_INSTR_SAT        = (-32765,-32765,-32765,-32765)
+    SUFFIX_HIGH_REPR_SAT         = (-32764,-32764,-32764,-32764)
+  END_GROUP                      = BAND_SUFFIX
+""")
+
+BAND_BIN_CENTER_FMT = pds3.fast_dict("""\
+  GROUP                          = BAND_BIN
+    BAND_BIN_CENTER = (0.35,0.36,0.37,0.37,0.38,0.39,0.40,0.40,0.41,0.42,
+      0.42,0.43,0.44,0.45,0.45,0.46,0.47,0.48,0.49,0.49,0.50,0.51,0.51,0.52,
+      0.53,0.53,0.54,0.55,0.56,0.56,0.57,0.58,0.59,0.59,0.60,0.61,0.62,0.62,
+      0.63,0.64,0.64,0.65,0.66,0.67,0.67,0.68,0.69,0.70,0.70,0.71,0.72,0.72,
+      0.73,0.74,0.75,0.75,0.76,0.77,0.78,0.78,0.79,0.80,0.81,0.81,0.82,0.83,
+      0.83,0.84,0.85,0.86,0.86,0.87,0.88,0.89,0.89,0.90,0.91,0.92,0.92,0.93,
+      0.94,0.94,0.95,0.96,0.97,0.97,0.98,0.99,1.00,1.00,1.01,1.02,1.02,1.03,
+      1.04,1.05,0.863,0.879,0.896,0.912,0.928,0.945,0.961,0.977,0.994,1.010,
+      1.026,1.043,1.060,1.077,1.093,1.109,1.125,1.142,1.159,1.175,1.191,1.207,
+      1.224,1.240,1.257,1.273,1.290,1.306,1.322,1.338,1.355,1.372,1.388,1.404,
+      1.421,1.437,1.453,1.470,1.487,1.503,1.519,1.535,1.552,1.569,1.585,1.597,
+      1.620,1.637,1.651,1.667,1.684,1.700,1.717,1.733,1.749,1.766,1.783,1.799,
+      1.815,1.831,1.848,1.864,1.882,1.898,1.914,1.930,1.947,1.964,1.980,1.997,
+      2.013,2.029,2.046,2.063,2.079,2.095,2.112,2.128,2.145,2.162,2.178,2.194,
+      2.211,2.228,2.245,2.261,2.277,2.294,2.311,2.328,2.345,2.363,2.380,2.397,
+      2.413,2.430,2.446,2.462,2.479,2.495,2.512,2.528,2.544,2.559,2.577,2.593,
+      2.610,2.625,2.642,2.656,2.676,2.691,2.707,2.728,2.743,2.758,2.776,2.794,
+      2.811,2.827,2.845,2.861,2.877,2.894,2.910,2.926,2.942,2.958,2.972,2.996,
+      3.009,3.025,3.043,3.059,3.075,3.092,3.107,3.125,3.142,3.158,3.175,3.192,
+      3.209,3.227,3.243,3.261,3.278,3.294,3.311,3.328,3.345,3.361,3.377,3.394,
+      3.410,3.427,3.444,3.460,3.476,3.493,3.508,3.525,3.542,3.558,3.575,3.591,
+      3.609,3.626,3.644,3.660,3.678,3.695,3.712,3.729,3.746,3.763,3.779,3.796,
+      3.812,3.830,3.846,3.857,3.877,3.894,3.910,3.926,3.943,3.959,3.975,3.992,
+      4.008,4.024,4.042,4.058,4.076,4.092,4.110,4.127,4.144,4.161,4.178,4.193,
+      4.206,4.219,4.237,4.255,4.273,4.292,4.310,4.328,4.346,4.361,4.378,4.393,
+      4.410,4.427,4.443,4.461,4.477,4.495,4.511,4.529,4.547,4.563,4.581,4.598,
+      4.615,4.631,4.649,4.665,4.682,4.698,4.715,4.732,4.749,4.765,4.782,4.798,
+      4.815,4.831,4.848,4.864,4.881,4.898,4.915,4.932,4.949,4.967,4.984,5.001,
+      5.017,5.036,5.052,5.069,5.086,5.102)
+    BAND_BIN_UNIT                = MICROMETER
+    BAND_BIN_ORIGINAL_BAND = (1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,
+      19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,
+      43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,
+      67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,
+      91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,
+      111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127,128,
+      129,130,131,132,133,134,135,136,137,138,139,140,141,142,143,144,145,146,
+      147,148,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,
+      165,166,167,168,169,170,171,172,173,174,175,176,177,178,179,180,181,182,
+      183,184,185,186,187,188,189,190,191,192,193,194,195,196,197,198,199,200,
+      201,202,203,204,205,206,207,208,209,210,211,212,213,214,215,216,217,218,
+      219,220,221,222,223,224,225,226,227,228,229,230,231,232,233,234,235,236,
+      237,238,239,240,241,242,243,244,245,246,247,248,249,250,251,252,253,254,
+      255,256,257,258,259,260,261,262,263,264,265,266,267,268,269,270,271,272,
+      273,274,275,276,277,278,279,280,281,282,283,284,285,286,287,288,289,290,
+      291,292,293,294,295,296,297,298,299,300,301,302,303,304,305,306,307,308,
+      309,310,311,312,313,314,315,316,317,318,319,320,321,322,323,324,325,326,
+      327,328,329,330,331,332,333,334,335,336,337,338,339,340,341,342,343,344,
+      345,346,347,348,349,350,351)
+  END_GROUP                      = BAND_BIN
+""")
+
+##########################################################################################
 # Standard class methods
-################################################################################
+##########################################################################################
 
-def from_file(filespec, fast=False, **parameters):
-    """A general, static method to return a pair of Observation objects based on
-    a given Cassini VIMS data file or label file.
+def from_file(filespec, data=True):
+    """A general, static method to return a pair of Observation objects based on a given
+    Cassini VIMS data file or label file.
 
     Input:
         filespec        the full path to a VIMS cube file or its PDS label.
-        fast            True to perform a fast load of a label file. A fast load
-                        bypasses the PDS label parser and pulls the minimum
-                        required information out of the label using a much
-                        faster procedure. It works only when the filespec is a
-                        PDS label.
-
-    Return:             (vis,ir)
-        vis             the VIS observation, or None if the VIS channel was
-                        inactive.
-        ir              the IR observation, or None if the IR channel was
-                        inactive.
+        data            if True, data arrays are included in the returned observation
+                        objects. Use a tuple of two booleans to specify whether to include
+                        the VIS and IR data independently.
+
+    Return:             (vis, ir)
+        vis             the VIS observation, or None if the VIS channel was inactive.
+        ir              the IR observation, or None if the IR channel was inactive.
     """
 
     VIMS.initialize()   # Define everything the first time through; use defaults
                         # unless initialize() is called explicitly.
 
-    # Load a label via the fast procedure if specified
-    if fast:
-        assert filespec.lower().endswith('.lbl')
-        f = open(filespec)
-        lines = f.readlines()
-        f.close()
+    if not isinstance(data, (tuple, list)):
+        data = (data, data)
+
+    label = pds3.fast_dict(filespec)
+
+    # Insert "data_file" and "header_recs"
+    # Convert ISIS .qub info to a standard PDS3 label dictionary
+    if 'QUBE' in label:
+
+        # PDS3 labels use "SPECTRAL_QUBE" in place of "QUBE"
+        label['SPECTRAL_QUBE'] = label['QUBE']
+
+        # Copy the non-structural issue to the top-level dictionary
+        for key, value in label['QUBE'].items():
+            if (key in {'AXES', 'AXIS_NAME'}
+                or key[:5] == 'CORE_'
+                or key[:7] in {'SUFFIX_', 'SAMPLE_', 'BAND_SU'}):
+                    continue
+            label[key] = value
 
-        label = fast_dict(lines)
+        # Rename "PACKING" to "PACKING_FLAG"
+        label['PACKING_FLAG'] = label['PACKING']
 
-        # Allow label['SPECTRAL_QUBE'] to work properly below
-        label['SPECTRAL_QUBE'] = label
+        # Add these items
+        label['data_file'] = filespec
+        label['header_recs'] = label['^QUBE'] - 1
 
-    # Otherwise, use the standard parser
+    # Otherwise, convert PDS3 label info to a standard ISIS dictionary
     else:
-        # Load the VIMS file or the PDS label
-        lines = pdsparser.PdsLabel.load_file(filespec)
 
-        # Fix known syntax errors
-        for i in range(len(lines)):
-            line = lines[i]
-
-            # In GAIN_MODE_ID and BACKGROUND_SAMPLING_MODE_ID, sometimes N/A is
-            # not properly quoted
-            if line[:4] in ('GAIN', 'BACK'):
-                lines[i] = line.replace('(N/A',  '("N/A"')
-                lines[i] = line.replace('N/A)',  '"N/A")')
-
-            # Sometimes a comment begins on one line and and ends on the next
-            if line.strip().endswith('*/') and '/*' not in line:
-                lines[i] = '\n'
-
-        label = pdsparser.PdsLabel.from_string(lines).as_dict()
-
-    is_isis_file = 'QUBE' in label.keys()
-    if is_isis_file:                # If this is an ISIS file...
-        info = label['QUBE']        # ... the info is in the QUBE object
-    else:                           # Otherwise, this is a .LBL file
-        info = label                # ... and the info is at the top level
-        info['CORE_ITEMS'] = label['SPECTRAL_QUBE']['CORE_ITEMS']
-        info['BAND_SUFFIX_NAME'] = label['SPECTRAL_QUBE']['BAND_SUFFIX_NAME']
-        info['PACKING'] = info['PACKING_FLAG']
+        # Insert the needed info from the .FMT files
+        label['SPECTRAL_QUBE'].update(CORE_DESCRIPTION_FMT)
+        label['SPECTRAL_QUBE'].update(SUFFIX_DESCRIPTION_FMT)
+        label.update(BAND_BIN_CENTER_FMT)
+
+        # ISIS labels use "QUBE" in place of "SPECTRAL_QUBE"
+        label['QUBE'] = label['SPECTRAL_QUBE']
+
+        # Add these items
+        parent = os.path.split(filespec)[0]
+        label['data_file'] = os.path.join(parent, label['^QUBE'][0])
+        label['header_recs'] = label['^QUBE'][1] - 1
+
+    qube_dict = label['SPECTRAL_QUBE']
 
     # Load any needed SPICE kernels
-    tstart = julian.tdb_from_tai(julian.tai_from_iso(info['START_TIME']))
+    tstart = julian.tdb_from_tai(julian.tai_from_iso(label['START_TIME']))
     Cassini.load_cks( tstart, tstart + 3600.)
     Cassini.load_spks(tstart, tstart + 3600.)
 
     # Check power state of each channel: [0] is IR; [1] is VIS
-    ir_is_off  = info['POWER_STATE_FLAG'][0] == 'OFF'
-    vis_is_off = info['POWER_STATE_FLAG'][1] == 'OFF'
+    ir_is_off  = label['POWER_STATE_FLAG'][0] == 'OFF'
+    vis_is_off = label['POWER_STATE_FLAG'][1] == 'OFF'
 
     ########################################
-    # Load the data array
+    # Load the data arrays
     ########################################
 
-    (samples, bands, lines) = info['CORE_ITEMS']
+    (samples, bands, lines) = qube_dict['CORE_ITEMS']
     assert bands in (352, 256, 96)
 
-    if is_isis_file:
-        (data, times) = _load_data_and_times(filespec, label)
-        assert data.shape == (lines, samples, bands)
+    vis_data = None
+    ir_data = None
+    times = None
+
+    if data[0] or data[1]:
+        qub_file = filespec.replace('.lbl', '.qub')
+        (array, times) = _load_data_and_times(qub_file, label)
+        assert array.shape == (lines, samples, bands), 'incorrect array shape'
 
         if bands == 352:
-            vis_data = data[:,:,:96]    # index order is [line, sample, band]
-            ir_data  = data[:,:,96:]
+            vis_data = array[:,:,:96]   # index order is [line, sample, band]
+            ir_data  = array[:,:,96:]
         elif bands == 256:              # only happens in a few early cubes
             vis_data = None
-            ir_data = data
+            ir_data = array
         else:
-            vis_data = data
+            vis_data = array
             ir_data = None
 
-    else:
-        vis_data = None
-        ir_data = None
-        times = None
-
     ########################################
     # Define the FOVs
     ########################################
 
-    swath_width = info['SWATH_WIDTH']
-    swath_length = info['SWATH_LENGTH']
+    swath_width = label['SWATH_WIDTH']
+    swath_length = label['SWATH_LENGTH']
 
     frame_size = swath_width * swath_length
     frames = (samples * lines) // frame_size
     assert samples * lines == frames * frame_size
 
     # Replace multiple one-line frames by one frame, multiple lines
     if frames > 1 and frame_size != 1:
         assert swath_length == 1
         swath_length = frames
         lines = frames
         frame_size = swath_width * swath_length
 
     uv_shape = (swath_width, swath_length)
 
-    x_offset = info['X_OFFSET']
-    z_offset = info['Z_OFFSET']
+    x_offset = label['X_OFFSET']
+    z_offset = label['Z_OFFSET']
     uv_los = (33. - x_offset, 33. - z_offset)
 
-    vis_sampling = info['SAMPLING_MODE_ID'][1].strip()  # handle ' NORMAL'
-    ir_sampling  = info['SAMPLING_MODE_ID'][0].strip()
+    vis_sampling = label['SAMPLING_MODE_ID'][1].strip()  # handle ' NORMAL'
+    ir_sampling  = label['SAMPLING_MODE_ID'][0].strip()
 
     # VIS FOV
     if vis_sampling == 'HI-RES':
         vis_fov = oops.fov.FlatFOV(VIS_HIRES_SCALE, uv_shape,
-                    (VIS_HIRES_FACTOR * uv_los[0] - uv_shape[0],
-                     VIS_HIRES_FACTOR * uv_los[1] - uv_shape[1]))
+                                   (VIS_HIRES_FACTOR * uv_los[0] - uv_shape[0],
+                                    VIS_HIRES_FACTOR * uv_los[1] - uv_shape[1]))
 
     elif uv_shape == (64,64):
         vis_fov = VIS_FULL_FOV
 
     else:
         vis_fov = oops.fov.FlatFOV(VIS_NORMAL_SCALE, uv_shape,
-                    (IR_OVER_VIS * uv_los[0], IR_OVER_VIS * uv_los[1]))
+                                   (IR_OVER_VIS * uv_los[0], IR_OVER_VIS * uv_los[1]))
 
     # IR FOV
-    if info['INSTRUMENT_MODE_ID'] == 'OCCULTATION':
+    if label['INSTRUMENT_MODE_ID'] == 'OCCULTATION':
         if ir_sampling == 'NORMAL':
             ir_fov = oops.fov.FlatFOV(IR_NORMAL_SCALE, uv_shape, uv_los)
         else:
             ir_fov = oops.fov.FlatFOV(IR_HIRES_SCALE, uv_shape, uv_los)
 
     elif ir_sampling in ('HI-RES','UNDER'):
         ir_fov = oops.fov.FlatFOV(IR_HIRES_SCALE, uv_shape,
-                    (IR_HIRES_FACTOR * uv_los[0] - uv_shape[0]/2., uv_los[1]))
+                                  (IR_HIRES_FACTOR * uv_los[0] - uv_shape[0]/2.,
+                                   uv_los[1]))
 
     elif uv_shape == (64,64):
         ir_fov = IR_FULL_FOV
 
     else:
         ir_fov = oops.fov.FlatFOV(IR_NORMAL_SCALE, uv_shape, uv_los)
 
     # Nyquist sampling
     if ir_sampling == 'UNDER':
-        ### VIMS IR sampling mode UNDER is untested!!
+        ### TBD: VIMS IR sampling mode UNDER is untested!!
         # Use ir_det_size = 2 for RasterSlit1D and RasterSlit observations
         # Use (1., ir_det_size) for RasterScan observations
         ir_fov = oops.fov.GapFOV(IR_NORMAL_SCALE, uv_shape, uv_los)
 
     else:
         ir_fov = oops.fov.FlatFOV(IR_NORMAL_SCALE, uv_shape, uv_los)
 
     ########################################
     # Define the cadences
     ########################################
 
     # Define cadences based on header parameters
-    ir_texp  = info['EXPOSURE_DURATION'][0] * 0.001 * TIME_FACTOR
-    vis_texp = info['EXPOSURE_DURATION'][1] * 0.001 * TIME_FACTOR
+    ir_texp  = label['EXPOSURE_DURATION'][0] * 0.001 * TIME_FACTOR
+    vis_texp = label['EXPOSURE_DURATION'][1] * 0.001 * TIME_FACTOR
     vis_texp_nonzero = max(vis_texp, 1.e-8) # avoids divide-by-zero in cadences
 
-    interframe_delay = info['INTERFRAME_DELAY_DURATION'] * 0.001 * TIME_FACTOR
-    interline_delay  = info['INTERLINE_DELAY_DURATION']  * 0.001 * TIME_FACTOR
+    interframe_delay = label['INTERFRAME_DELAY_DURATION'] * 0.001 * TIME_FACTOR
+    interline_delay  = label['INTERLINE_DELAY_DURATION']  * 0.001 * TIME_FACTOR
 
     # Adjust the timing of one line, multiple frames
     if frames > 1 and frame_size != 1:
         interline_delay = interframe_delay
 
     length_stride = max(ir_texp * swath_width, vis_texp) + interline_delay
 
     backplane_cadence = None
 
     # Define a cadence based on the time backplane, if it is present
     if times is None:
         pass
 
-    elif info['OVERWRITTEN_CHANNEL_FLAG'] == 'ON':
+    elif label['OVERWRITTEN_CHANNEL_FLAG'] == 'ON':
         times = times.ravel()
         assert times[0] < times[1]
         assert vis_is_off
         backplane_cadence = oops.cadence.Sequence(times, ir_texp)
 
-    elif info['PACKING'] == 'ON':
+    elif label['PACKING_FLAG'] == 'ON':
         times = times.ravel()
         assert times[0] == times[1]
         tstart = times[0]
         frame_cadence = oops.cadence.Sequence(times[::frame_size], texp=0.)
 
     else:       # No packing plus no embedded timing just means a better tstart
         times = times.ravel()
         assert times[0] == times[1]
         tstart = times[0]
 
-    vis_header_cadence = oops.cadence.Metronome(tstart,
-                                length_stride, vis_texp_nonzero, swath_length)
-    ir_fast_cadence = oops.cadence.Metronome(tstart,
-                                ir_texp, ir_texp, swath_width)
-    ir_header_cadence = oops.cadence.DualCadence(vis_header_cadence,
-                                ir_fast_cadence)
+    vis_header_cadence = oops.cadence.Metronome(tstart, length_stride, vis_texp_nonzero,
+                                                swath_length)
+    ir_fast_cadence = oops.cadence.Metronome(tstart, ir_texp, ir_texp, swath_width)
+    ir_header_cadence = oops.cadence.DualCadence(vis_header_cadence, ir_fast_cadence)
 
     # At this point...
     #   vis_header_cadence  always defined, always 1-D.
     #   ir_fast_cadence     always defined, always 1-D.
     #   ir_header_cadence   always defined, always 2-D.
     #   backplane_cadence   defined if timing was recorded, always 1-D.
 
     ########################################
     # Define the coordinate frames
     ########################################
 
     vis_frame_id = 'CASSINI_VIMS_V'
     ir_frame_id  = 'CASSINI_VIMS_IR'
 
-    if (info['TARGET_NAME'] == 'SUN' or '_SOL' in info['OBSERVATION_ID']):
+    if (label['TARGET_NAME'] == 'SUN' or '_SOL' in label['OBSERVATION_ID']):
         ir_frame_id = 'CASSINI_VIMS_IR_SOL'
 
     ########################################
     # Construct the Observation objects
     ########################################
 
     vis_obs = None
     ir_obs  = None
 
     # POINT/OCCULTATION case
     if swath_width == 1 and swath_length == 1:
         assert vis_is_off
         if backplane_cadence is None:
             fast_stride = ir_texp   # + EXTRA_INTERSAMPLE_DELAY
-            fastcad = oops.cadence.Metronome(tstart, fast_stride, ir_texp,
-                                             samples)
+            fastcad = oops.cadence.Metronome(tstart, fast_stride, ir_texp, samples)
 
             slow_stride = ir_texp * samples + interline_delay
-            slowcad = oops.cadence.Metronome(tstart, slow_stride, slow_stride,
-                                             lines)
+            slowcad = oops.cadence.Metronome(tstart, slow_stride, slow_stride, lines)
             fullcad = oops.cadence.DualCadence(slowcad, fastcad)
             ir_cadence = oops.cadence.ReshapedCadence(fullcad, (samples*lines,))
 
         else:
             ir_cadence = backplane_cadence
 
         if ir_data is not None:
             ir_data = ir_data.reshape((frames, 256))
 
-        ir_obs = oops.obs.Pixel(('t','b'),
-                                ir_cadence, ir_fov,
-                                'CASSINI', ir_frame_id)
+        ir_obs = oops.obs.Pixel(('t','b'), ir_cadence, ir_fov, 'CASSINI', ir_frame_id)
 
     # Single LINE case
     elif swath_length == 1:
         if not vis_is_off:
             if vis_data is not None:
                 vis_data = vis_data.reshape((samples, 96))
 
-            vis_obs = oops.obs.Slit1D(('u','b'),
-                                       tstart, vis_texp_nonzero, vis_fov,
+            vis_obs = oops.obs.Slit1D(('u','b'), tstart, vis_texp_nonzero, vis_fov,
                                        'CASSINI', vis_frame_id)
 
         if not ir_is_off:
             if ir_data is not None:
                 ir_data = ir_data.reshape((samples, 256))
 
             if backplane_cadence is not None:
                 ir_fast_cadence = backplane_cadence
 
-            ir_obs = oops.obs.RasterSlit1D(('ut','b'),
-                                           ir_fast_cadence, ir_fov,
+            ir_obs = oops.obs.RasterSlit1D(('ut','b'), ir_fast_cadence, ir_fov,
                                            'CASSINI', ir_frame_id)
 
     # Single 2-D IMAGE case
     elif samples == swath_width and lines == swath_length:
         if not vis_is_off:
-            vis_obs = oops.obs.TimedImage(('vt','u','b'),
-                                          vis_header_cadence, vis_fov,
+            vis_obs = oops.obs.TimedImage(('vt','u','b'), vis_header_cadence, vis_fov,
                                           'CASSINI', vis_frame_id)
 
         if not ir_is_off:
             if backplane_cadence is None:
                 ir_cadence = oops.cadence.DualCadence(vis_header_cadence,
                                                       ir_fast_cadence)
             else:
                 ir_cadence = oops.cadence.ReshapedCadence(backplane_cadence,
                                                          (lines,samples))
 
-            ir_obs = oops.obs.TimedImage(('vslow','ufast','b'),
-                                         ir_cadence, ir_fov,
+            ir_obs = oops.obs.TimedImage(('vslow','ufast','b'), ir_cadence, ir_fov,
                                          'CASSINI', ir_frame_id)
 
     # Multiple LINE case
     elif swath_length == 1 and swath_length == lines:
         if not vis_is_off:
-            vis_obs = oops.obs.TimedImage(('vt','u','b'),
-                                          frame_cadence, vis_fov,
+            vis_obs = oops.obs.TimedImage(('vt','u','b'), frame_cadence, vis_fov,
                                           'CASSINI', vis_frame_id)
 
         if not ir_is_off:
             if backplane_cadence is None:
-                ir_cadence = oops.cadence.DualCadence(frame_cadence,
-                                                      ir_fast_cadence)
+                ir_cadence = oops.cadence.DualCadence(frame_cadence, ir_fast_cadence)
             else:
                 ir_cadence = oops.cadence.ReshapedCadence(backplane_cadence,
                                                          (lines,samples))
 
-            ir_obs = oops.obs.TimedImage(('vslow','ufast','b'),
-                                         ir_cadence, ir_fov,
+            ir_obs = oops.obs.TimedImage(('vslow','ufast','b'), ir_cadence, ir_fov,
                                          'CASSINI', ir_frame_id)
 
 # 1/9/15 broken code no longer needed
 #     # Multiple 2-D IMAGE case
 #
 #     elif lines == frames and samples == swath_width * swath_length:
 #         if not vis_is_off:
@@ -480,80 +579,75 @@
     if vis_obs is not None:
         vis_obs.insert_subfield('instrument', 'VIMS')
         vis_obs.insert_subfield('detector', 'VIS')
         vis_obs.insert_subfield('sampling', vis_sampling)
         vis_obs.insert_subfield('dict', label)
         vis_obs.insert_subfield('index_dict', label)# for backward compatibility
 
-        if vis_data is not None:
+        if vis_data is not None and data[0]:
             vis_obs.insert_subfield('data', vis_data)
 
     if ir_obs is not None:
         ir_obs.insert_subfield('instrument', 'VIMS')
         ir_obs.insert_subfield('detector', 'IR')
         ir_obs.insert_subfield('sampling', ir_sampling)
         ir_obs.insert_subfield('dict', label)
         ir_obs.insert_subfield('index_dict', label)# for backward compatibility
 
-        if ir_data is not None:
+        if ir_data is not None and data[1]:
             ir_obs.insert_subfield('data', ir_data)
 
     return (vis_obs, ir_obs)
 
-#===============================================================================
+#=========================================================================================
 def _load_data_and_times(filespec, label):
     """Load the data array from the file.
 
-    If time backplanes are present, also return an array of times in seconds
-    TDB as derived from these backplanes.
+    If time backplanes are present, also return an array of times in seconds TDB as
+    derived from these backplanes.
 
     Input:
         filespec        full path to the data file.
         label           the label dictionary.
 
     Return:             (data, times)
-        data            a Numpy array containing the data in axis order
-                        (line, sample, band).
-        times           the time sampling array in (line, sample) axis order, or
-                        None if no time backplane is found in the file.
+        data            a Numpy array containing the data in axis order (line, sample,
+                        band).
+        times           the time sampling array in (line, sample) axis order, or None if
+                        no time backplane is found in the file.
 
-    Note: This procedure is absurdly complicated but it has been rather
-    carefully debugged. --MRS 7/4/12.
+    Note: This procedure is absurdly complicated but it has been rather carefully
+    debugged. --MRS 7/4/12.
     """
-    info = label['QUBE']
 
-    # Extract key parameters fro the file header
-    core_items   = info['CORE_ITEMS']
+    qube_dict = label['SPECTRAL_QUBE']
+
+    # Extract key parameters from the file header
+    core_items   = qube_dict['CORE_ITEMS']
     core_samples = core_items[0]
     core_bands   = core_items[1]
     core_lines   = core_items[2]
-    core_item_bytes = info['CORE_ITEM_BYTES']
-    core_item_type  = info['CORE_ITEM_TYPE']
+    core_item_bytes = qube_dict.get('CORE_ITEM_BYTES', 2)
+    core_item_type  = qube_dict.get('CORE_ITEM_TYPE', 'SUN_INTEGER')
 
-    sample_suffix_items = info['SUFFIX_ITEMS'][0]
-    band_suffix_items   = info['SUFFIX_ITEMS'][1]
+    sample_suffix_items = qube_dict['SUFFIX_ITEMS'][0]
+    band_suffix_items   = qube_dict['SUFFIX_ITEMS'][1]
 
     suffix_item_bytes = 4
 
-    if sample_suffix_items == 1:
-        suffix_item_type = info['SAMPLE_SUFFIX_ITEM_TYPE']
-    elif sample_suffix_items > 1:
-        suffix_item_type = info['SAMPLE_SUFFIX_ITEM_TYPE'][0]
-    elif band_suffix_items == 1:
-        suffix_item_type = info['BAND_SUFFIX_ITEM_TYPE']
-    elif band_suffix_items > 1:
-        suffix_item_type = info['BAND_SUFFIX_ITEM_TYPE'][0]
-    else:
-        suffix_item_type = ''
+    key = 'SAMPLE_SUFFIX_ITEM_TYPE' if sample_suffix_items else 'BAND_SUFFIX_ITEM_TYPE'
+    suffix_item_type = qube_dict.get(key, 'SUN_INTEGER')
+    if isinstance(suffix_item_type, (list, tuple)):
+        suffix_item_type = suffix_item_type[0]  # all backplanes/sideplanes are same type
 
     record_bytes = label['RECORD_BYTES']
-    header_bytes = record_bytes * (label['^QUBE'][1] - 1)
+    header_bytes = record_bytes * label['header_recs']
 
     # Make sure we have byte-aligned values
-    assert (core_samples * core_item_bytes) % suffix_item_bytes == 0
+    assert (core_samples * core_item_bytes) % suffix_item_bytes == 0, 'misaligned items'
 
     ############################
 
     # Determine the dtype and strides for the core item array
     band_stride = (core_samples * core_item_bytes +
                    sample_suffix_items * suffix_item_bytes)
 
@@ -593,23 +687,23 @@
     # Read the file as core dtypes
     array = np.fromfile(filespec, dtype=core_dtype)
 
     # Slice away the core lines, leaving off the line suffix
     array = array[offset:offset+size]
 
     # Create a data array using new strides in (line, sample, band) order
-    data = numpy.lib.stride_tricks.as_strided(array,
-                    strides = (line_stride, core_item_bytes, band_stride),
-                    shape   = (core_lines,  core_samples,    core_bands))
+    data = stride_tricks.as_strided(array,
+                                    strides = (line_stride, core_item_bytes, band_stride),
+                                    shape   = (core_lines,  core_samples,    core_bands))
 
     # Convert core to a native 3-D array
     data = data.astype(native_dtype)
 
     # If there are no time backplanes, we're done
-    band_suffix_name = info['BAND_SUFFIX_NAME']
+    band_suffix_name = qube_dict['BAND_SUFFIX_NAME']
     if 'SLICE_TIME_SECONDS' not in band_suffix_name:
         return (data, None)
 
     ############################
 
     # Determine the dtype for the file core
     if 'SUN_' in core_item_type or 'MSB_' in suffix_item_type:
@@ -639,17 +733,17 @@
                 offset = core_bands * (core_samples * core_item_bytes +
                                        sample_suffix_items * suffix_item_bytes),
                 dtype = suffix_item_dtype)
 
     # Extract the band suffix array using new strides in
     # (backplane, line, sample) order
     backplane_stride = suffix_item_bytes * (core_samples + sample_suffix_items)
-    backplane = numpy.lib.stride_tricks.as_strided(offset_array,
-                strides = (backplane_stride,  line_stride, suffix_item_bytes),
-                shape   = (band_suffix_items, core_lines,  core_samples))
+    backplane = stride_tricks.as_strided(offset_array,
+                            strides = (backplane_stride,  line_stride, suffix_item_bytes),
+                            shape   = (band_suffix_items, core_lines,  core_samples))
 
     # Convert to spacecraft clock
     seconds = backplane[band_suffix_name.index('SLICE_TIME_SECONDS')]
     ticks = backplane[band_suffix_name.index('SLICE_TIME_TICKS')]
     sclock = seconds + ticks/15959.
 
     # Convert to TDB
@@ -670,141 +764,30 @@
         tdb_max = cspyce.scs2e(-82, formatted) + (sclock_max - float(formatted))
 
         times = tdb_min + (sclock - sclock_min) * ((tdb_max - tdb_min) /
                                                    (sclock_max - sclock_min))
 
     return (data, times)
 
-#===============================================================================
-def pds_value_from_constants(string_value):
-    """A value or tuple from a string that does not contain quotes and therefore
-    expects a pre-defined constant.
-
-    Input:
-        string_value    a string that is either a pre-defined constant OR a
-                        tuple of pre-defined constants
-
-    Return:             a string of that constant or a tuple of strings of those
-                        constants.
-    """
-    if string_value[0] == '(' and string_value[-1] == ')':
-        words = string_value[1:-1].split(',')
-        return words
-        """string_list = []
-        for word in words:
-            string_list.append('"' + word + '"')
-        string_tuple = tuple(string_list)
-        return string_tuple
-        """
-
-    #if add_quotes:
-    #    return '"' + string_value + '"'
-    return string_value
-
-#===============================================================================
-def fast_dict(lines):
-    """A dictionary extracted from the PDS label of a VIMS file, containing the
-    minimum required set of entries for the observation to be generated and
-    analyzed.
-
-    This routine is much faster than a call to PdsLabel.from_file() because
-    it does not use the pyparsing module.
-
-    Input:
-        lines           a list containing all the lines of the file, as read by
-                        file.readlines().
-
-    Return:             a dictionary containing, at minimum, these elements:
-                            "BAND_SUFFIX_NAME" = unparsed string
-                            "CORE_ITEMS" = three ints
-                            "EXPOSURE_DURATION" = two floats
-                            "INSTRUMENT_MODE_ID" = unquoted string
-                            "INTERFRAME_DELAY_DURATION" = float
-                            "INTERLINE_DELAY_DURATION" = float
-                            "MISSION_PHASE_NAME" = string
-                            "OVERWRITTEN_CHANNEL_FLAG" = string
-                            "PACKING_FLAG" = string
-                            "POWER_STATE_FLAG" = pair of strings
-                            "SAMPLING_MODE_ID" = pair of strings
-                            "START_TIME" = string
-                            "SWATH_LENGTH" = int
-                            "SWATH_WIDTH" = int
-                            "TARGET_NAME" = string
-                            "X_OFFSET" = int
-                            "Z_OFFSET" = int
-    """
-    def three_ints(string):
-        string = string.strip()
-        assert string[0] == '(' and string[1] == ')'
-        (a,b,c) = string[1:-1].split(',')
-        return (int(a), int(b), int(c))
-
-    def two_floats(string):
-        string = string.strip()
-        assert string[0] == '(' and string[1] == ')'
-        (a,b) = string[1:-1].split(',')
-        return (float(a), float(b))
-
-    def two_strings(string):
-        string = string.strip()
-        assert string[0] == '(' and string[1] == ')'
-        (a,b) = string[1:-1].split(',')
-        return (unquote(a), unquote(b))
-
-    def unquote(string):
-        string = string.strip()
-        if len(string) >= 2 and string[0] == '"' and string[-1] == '"':
-            return string[1:-1]
-        else:
-            return string
-
-    # Create a quick dictionary using the PDS keyword, equal to the string value
-    dict = {}
-    for line in lines:
-        pair = line.split('=')
-        if len(pair) == 2:
-            dict[pair[0].strip()] = pair[1]
-
-    # Re-define the required keywords
-
-    dict['BAND_SUFFIX_NAME']          = dict['BAND_SUFFIX_NAME'].strip()
-    dict['CORE_ITEMS']                = three_ints(dict['CORE_ITEMS'])
-    dict['EXPOSURE_DURATION']         = two_floats(dict['EXPOSURE_DURATION'])
-    dict['INSTRUMENT_MODE_ID']        = unquote(dict['INSTRUMENT_MODE_ID'])
-    dict['INTERFRAME_DELAY_DURATION'] = float(dict['INTERFRAME_DELAY_DURATION'])
-    dict['INTERLINE_DELAY_DURATION']  = float(dict['INTERLINE_DELAY_DURATION'])
-    dict['MISSION_PHASE_NAME']        = unquote(['MISSION_PHASE_NAME'])
-    dict['OVERWRITTEN_CHANNEL_FLAG']  = unquote(['OVERWRITTEN_CHANNEL_FLAG'])
-    dict['PACKING_FLAG']              = unquote(dict['PACKING_FLAG'])
-    dict['POWER_STATE_FLAG']          = two_strings(dict['POWER_STATE_FLAG'])
-    dict['SAMPLING_MODE_ID']          = two_strings(dict['SAMPLING_MODE_ID'])
-    dict['START_TIME']                = dict['START_TIME'].strip()
-    dict['SWATH_LENGTH']              = int(dict['SWATH_LENGTH'])
-    dict['SWATH_WIDTH']               = int(dict['SWATH_WIDTH'])
-    dict['TARGET_NAME']               = unquote(dict['TARGET_NAME'])
-    dict['X_OFFSET']                  = int(dict['X_OFFSET'])
-    dict['Z_OFFSET']                  = int(dict['Z_OFFSET'])
-
-    return dict
-
-#===============================================================================
+#=========================================================================================
 def meshgrid_and_times(obs, oversample=6, extend=1.5):
-    """A meshgrid object and time array that oversamples and extends the
-    dimensions of the field of view of a VIMS observation.
+    """A meshgrid object and time array that oversamples and extends the dimensions of the
+    field of view of a VIMS observation.
 
     Input:
-        obs             the VIMS observation object to for which to generate a
-                        meshgrid and a time array.
-        oversample      the factor by which to oversample the field of view, in
-                        units of the full-resolution VIMS pixel size.
-        extend          the number of pixels by which to extend the field of
-                        view, in units of the oversampled pixel.
+        obs             the VIMS observation object to for which to generate a meshgrid
+                        and a time array.
+        oversample      the factor by which to oversample the field of view, in units of
+                        the full-resolution VIMS pixel size.
+        extend          the number of pixels by which to extend the field of view, in
+                        units of the oversampled pixel.
 
     Return:             (mesgrid, time)
     """
+
     shrinkage = {('IR',  'NORMAL'): (1,1),
                  ('IR',  'HI-RES'): (2,1),
                  ('IR',  'UNDER' ): (2,1),
                  ('VIS', 'NORMAL'): (1,1),
                  ('VIS', 'HI-RES'): (3,3)}
 
     assert obs.instrument == 'VIMS'
@@ -818,136 +801,119 @@
     vstep = vshrink / oversample
 
     origin = (-extend * ustep, -extend * vstep)
 
     limit = (obs.fov.uv_shape.vals[0] + extend * ustep,
              obs.fov.uv_shape.vals[1] + extend * vstep)
 
-    meshgrid = oops.Meshgrid.for_fov(obs.fov, origin, undersample, oversample,
-                                     limit, swap=True)
+    meshgrid = oops.Meshgrid.for_fov(obs.fov, origin, undersample, oversample, limit,
+                                     swap=True)
 
     time = obs.uvt(obs.fov.nearest_uv(meshgrid.uv).swapxy())[1]
 
     return (meshgrid, time)
 
-#===============================================================================
-def initialize(ck='reconstructed', planets=None, asof=None,
-               spk='reconstructed', gapfill=True,
-               mst_pck=True, irregulars=True):
+#=========================================================================================
+def initialize(ck='reconstructed', planets=None, asof=None, spk='reconstructed',
+               gapfill=True, mst_pck=True, irregulars=True):
     """Initialize key information about the VIMS instrument.
 
     Must be called first. After the first call, later calls to this function
     are ignored.
 
     Input:
-        ck,spk      'predicted', 'reconstructed', or 'none', depending on
-                    which kernels are to be used. Defaults are 'reconstructed'.
-                    Use 'none' if the kernels are to be managed manually.
-        planets     A list of planets to pass to define_solar_system. None or
-                    0 means all.
+        ck,spk      'predicted', 'reconstructed', or 'none', depending on which kernels
+                    are to be used. Defaults are 'reconstructed'. Use 'none' if the
+                    kernels are to be managed manually.
+        planets     A list of planets to pass to define_solar_system. None or 0 means all.
         asof        Only use SPICE kernels that existed before this date;
                     None to ignore.
         gapfill     True to include gapfill CKs. False otherwise.
-        mst_pck     True to include MST PCKs, which update the rotation models
-                    for some of the small moons.
-        irregulars  True to include the irregular satellites;
-                    False otherwise.
+        mst_pck     True to include MST PCKs, which update the rotation models for some of
+                    of the small moons.
+        irregulars  True to include the irregular satellites; False otherwise.
     """
-    VIMS.initialize(ck=ck, planets=planets, asof=asof, spk=spk,
-                    gapfill=gapfill, mst_pck=mst_pck, irregulars=irregulars)
 
-################################################################################
+    VIMS.initialize(ck=ck, planets=planets, asof=asof, spk=spk, gapfill=gapfill,
+                    mst_pck=mst_pck, irregulars=irregulars)
+
+##########################################################################################
 
 class VIMS(object):
     """An instance-free class to hold Cassini VIMS instrument parameters."""
 
     initialized = False
     instrument_kernel = None
 
-    #===========================================================================
     @staticmethod
-    def initialize(ck='reconstructed', planets=None, asof=None,
-                   spk='reconstructed', gapfill=True,
-                   mst_pck=True, irregulars=True):
+    def initialize(ck='reconstructed', planets=None, asof=None, spk='reconstructed',
+                   gapfill=True, mst_pck=True, irregulars=True):
         """Fill in key information about the VIS and IR channels.
 
-        Must be called first. After the first call, later calls to this function
-        are ignored.
+        Must be called first. After the first call, later calls to this function are
+        ignored.
 
         Input:
-            ck,spk      'predicted', 'reconstructed', or 'none', depending on
-                        which kernels are to be used. Defaults are
-                        'reconstructed'. Use 'none' if the kernels are to be
-                        managed manually.
-            planets     A list of planets to pass to define_solar_system. None
-                        or 0 means all.
-            asof        Only use SPICE kernels that existed before this date;
-                        None to ignore.
+            ck,spk      'predicted', 'reconstructed', or 'none', depending on which
+                        kernels are to be used. Defaults are 'reconstructed'. Use 'none'
+                        if the kernels are to be managed manually.
+            planets     A list of planets to pass to define_solar_system. None or 0 means
+                        all.
+            asof        Only use SPICE kernels that existed before this date; None to
+                        ignore.
             gapfill     True to include gapfill CKs. False otherwise.
-            mst_pck     True to include MST PCKs, which update the rotation
-                        models for some of the small moons.
-            irregulars  True to include the irregular satellites;
-                        False otherwise.
+            mst_pck     True to include MST PCKs, which update the rotation models for
+                        some of the small moons.
+            irregulars  True to include the irregular satellites; False otherwise.
         """
 
         # Quick exit after first call
         if VIMS.initialized:
             return
 
-        Cassini.initialize(ck=ck, planets=planets, asof=asof, spk=spk,
-                           gapfill=gapfill,
+        Cassini.initialize(ck=ck, planets=planets, asof=asof, spk=spk, gapfill=gapfill,
                            mst_pck=mst_pck, irregulars=irregulars)
         Cassini.load_instruments(asof=asof)
 
         # Load the instrument kernel
         VIMS.instrument_kernel = Cassini.spice_instrument_kernel('VIMS')[0]
 
         # Construct a SpiceFrame for each detector
         ignore = oops.frame.SpiceFrame('CASSINI_VIMS_V')
         ignore = oops.frame.SpiceFrame('CASSINI_VIMS_IR')
         ignore = oops.frame.SpiceFrame('CASSINI_VIMS_IR_SOL')
 
         VIMS.initialized = True
 
-    #===========================================================================
+    #=====================================================================================
     @staticmethod
     def reset():
         """Reset the internal Cassini VIMS parameters.
 
         Can be useful for debugging.
         """
 
         VIMS.instrument_kernel = None
         VIMS.fovs = {}
         VIMS.initialized = False
 
         Cassini.reset()
 
-################################################################################
+##########################################################################################
 # UNIT TESTS
-################################################################################
+##########################################################################################
 import unittest
 import os.path
 import oops.backplane.gold_master as gm
 
-from oops.unittester_support    import TESTDATA_PARENT_DIRECTORY
-
+from oops.unittester_support import TESTDATA_PARENT_DIRECTORY
 
-#===============================================================================
-class Test_Cassini_VIMS(unittest.TestCase):
 
-    #===========================================================================
-    def runTest(self):
-        pass
-
-
-#===============================================================================
 class Test_Cassini_VIMS_GoldMaster_v1690952775(unittest.TestCase):
 
-    #===========================================================================
     def runTest(self):
         """
         *** fails because vims needs updating ***
 
         v1690952775 Compare w Gold Masters
 
         To preview and regenerate gold masters (from pds-oops/oops/backplane/):
@@ -961,22 +927,22 @@
             python gold_master.py \
                 ~/Dropbox-SETI/OOPS-Resources/test_data/cassini/VIMS/v1793917030_1.qub \
                 --module hosts.cassini.vims \
                 --planet SATURN \
                 --no-inventory \
                 --adopt
         """
+
         gm.execute_as_unittest(self,
                 obspath = os.path.join(TESTDATA_PARENT_DIRECTORY,
                                        'cassini/VIMS/v1793917030_1.qub'),
                 index   = None,
                 module  = 'oops.hosts.cassini.vims',
                 planet  = 'SATURN',
                 moon    = '',
                 ring    = '',
                 inventory=False, border=10)
 
-
 ############################################
 if __name__ == '__main__':
     unittest.main(verbosity=2)
-################################################################################
+##########################################################################################
```

### Comparing `rms-oops-0.0.2/oops/hosts/cassini/vims_test_suite.py` & `rms_oops-0.0.3/oops/hosts/cassini/vims_test_suite.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/galileo/__init__.py` & `rms_oops-0.0.3/oops/hosts/galileo/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/galileo/ssi/__init__.py` & `rms_oops-0.0.3/oops/hosts/galileo/ssi/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/galileo/ssi/standard_obs.py` & `rms_oops-0.0.3/oops/hosts/galileo/ssi/standard_obs.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/__init__.py` & `rms_oops-0.0.3/oops/hosts/hst/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/acs/__init__.py` & `rms_oops-0.0.3/oops/hosts/hst/acs/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/acs/hrc.py` & `rms_oops-0.0.3/oops/hosts/hst/acs/hrc.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/acs/sbc.py` & `rms_oops-0.0.3/oops/hosts/hst/acs/sbc.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/acs/wfc.py` & `rms_oops-0.0.3/oops/hosts/hst/acs/wfc.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/nicmos/__init__.py` & `rms_oops-0.0.3/oops/hosts/hst/nicmos/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/nicmos/nic1.py` & `rms_oops-0.0.3/oops/hosts/hst/nicmos/nic1.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/nicmos/nic2.py` & `rms_oops-0.0.3/oops/hosts/hst/nicmos/nic2.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/nicmos/nic3.py` & `rms_oops-0.0.3/oops/hosts/hst/nicmos/nic3.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3/__init__.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3/ir.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3/ir.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3/uvis.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3/uvis.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3/wfc3_pointing_test.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3/wfc3_pointing_test.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3/wfc3_test_suite.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3/wfc3_test_suite.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3_pointing_test.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3_pointing_test.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfc3_test_suite.py` & `rms_oops-0.0.3/oops/hosts/hst/wfc3_test_suite.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/hst/wfpc2.py` & `rms_oops-0.0.3/oops/hosts/hst/wfpc2.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/__init__.py` & `rms_oops-0.0.3/oops/hosts/juno/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/jiram/__init__.py` & `rms_oops-0.0.3/oops/hosts/juno/jiram/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/jiram/img.py` & `rms_oops-0.0.3/oops/hosts/juno/jiram/img.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/jiram/spe.py` & `rms_oops-0.0.3/oops/hosts/juno/jiram/spe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/junocam/__init__.py` & `rms_oops-0.0.3/oops/hosts/juno/junocam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,40 +116,38 @@
         item.insert_subfield('filespec', filespec)
         item.insert_subfield('basename', os.path.basename(filespec))
         obs.append(item)
 
     return obs
 
 #===============================================================================
-def initialize(ck='reconstructed', planets=None, offset_wac=True, asof=None,
+def initialize(ck='reconstructed', planets=None, asof=None,
                spk='reconstructed', gapfill=True,
                mst_pck=True, irregulars=True):
     """Initialize key information about the JUNOCAM instrument.
 
     Must be called first. After the first call, later calls to this function
     are ignored.
 
     Input:
         ck,spk      'predicted', 'reconstructed', or 'none', depending on which
                     kernels are to be used. Defaults are 'reconstructed'. Use
                     'none' if the kernels are to be managed manually.
         planets     A list of planets to pass to define_solar_system. None or
                     0 means all.
-        offset_wac  True to offset the WAC frame relative to the NAC frame as
-                    determined by star positions.
         asof        Only use SPICE kernels that existed before this date; None
                     to ignore.
         gapfill     True to include gapfill CKs. False otherwise.
         mst_pck     True to include MST PCKs, which update the rotation models
                     for some of the small moons.
         irregulars  True to include the irregular satellites;
                     False otherwise.
     """
 
-    JUNOCAM.initialize(ck=ck, planets=planets, offset_wac=offset_wac, asof=asof,
+    JUNOCAM.initialize(ck=ck, planets=planets, asof=asof,
                    spk=spk, gapfill=gapfill,
                    mst_pck=mst_pck, irregulars=irregulars)
 
 ### mst_pck has no relevance here as an option; it's specific to Saturn.
 ### unless JunoCam ever targeted a Jupiter irregular, you can also omit that option.
 ### Really, I think you only need to ck and spk options, and only so we can be
 ### ready for some future date when/if this info is regenerated.
```

### Comparing `rms-oops-0.0.2/oops/hosts/juno/junocam/standard_obs.py` & `rms_oops-0.0.3/oops/hosts/juno/junocam/standard_obs.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/juno/unittester.py` & `rms_oops-0.0.3/oops/hosts/juno/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/jwst/__init__.py` & `rms_oops-0.0.3/oops/hosts/jwst/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/jwst/nircam/__init__.py` & `rms_oops-0.0.3/oops/hosts/jwst/nircam/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/jwst/nircam/uncal.py` & `rms_oops-0.0.3/oops/hosts/jwst/nircam/uncal.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/keck/__init__.py` & `rms_oops-0.0.3/oops/hosts/keck/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/keck/nirc2/__init__.py` & `rms_oops-0.0.3/oops/hosts/keck/nirc2/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/keck/nirc2.py` & `rms_oops-0.0.3/oops/hosts/keck/nirc2.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/newhorizons/__init__.py` & `rms_oops-0.0.3/oops/hosts/newhorizons/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/newhorizons/lorri.py` & `rms_oops-0.0.3/oops/hosts/newhorizons/lorri.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,38 +172,38 @@
 
     try:
         target_body = oops.Body.lookup(target_name)
     except:
         target_body = None
 
     if geom == 'spice':
-        path = oops.Path.as_waypoint('NEW HORIZONS')
+        path = oops.path.Path.as_waypoint('NEW HORIZONS')
     else:
 
         # First construct a path from the Sun to NH
         posx = -header['SPCSSCX']
         posy = -header['SPCSSCY']
         posz = -header['SPCSSCZ']
 
         velx = -header['SPCSSCVX']
         vely = -header['SPCSSCVY']
         velz = -header['SPCSSCVZ']
 
         # The path_id has to be unique to this observation
-        sun_path = oops.Path.as_waypoint('SUN')
+        sun_path = oops.path.Path.as_waypoint('SUN')
         path_id = '.NH_PATH_' + filename
         sc_path = oops.path.LinearPath((oops.Vector3([posx, posy, posz]),
                                         oops.Vector3([velx, vely, velz])),
                                        tdb_midtime, sun_path,
-                                       oops.Frame.J2000,
+                                       oops.frame.FrameFrame.J2000,
                                        path_id=path_id)
-        path = oops.Path.as_waypoint(sc_path)
+        path = oops.path.Path.as_waypoint(sc_path)
 
     if pointing == 'spice':
-        frame = oops.Frame.as_wayframe('NH_LORRI')
+        frame = oops.frame.Frame.as_wayframe('NH_LORRI')
     else:
 
         # Create a frame based on the boresight
         u_center = shape[1]/2. + 0.5    # offset to put [1,1] at center of pixel
         v_center = shape[0]/2. + 0.5
         (ra_deg, dec_deg) = radec_from_uv(u_center, v_center, header)
         north_clock_deg = header['SPCEMEN']
@@ -231,15 +231,15 @@
         scet = header['SPCSCET']
 
         frame_id = '.NH_FRAME_' + filename
         lorri_frame = oops.frame.Cmatrix.from_ra_dec(ra_deg, dec_deg,
                                                      north_clock_deg,
                                                      oops.Frame.J2000,
                                                      frame_id=frame_id)
-        frame = oops.Frame.as_wayframe(lorri_frame)
+        frame = oops.frame.Frame.as_wayframe(lorri_frame)
 
         event = oops.Event(tdb_midtime, oops.Vector3.ZERO, path, frame)
         event.neg_arr_ap = oops.Vector3.ZAXIS
         los = event.neg_arr_ap_j2000
 
     # Create a Snapshot
     snapshot = oops.obs.Snapshot(('v','u'), tstart, texp, fov, path, frame,
@@ -282,15 +282,15 @@
         try:
             solar_range = parameters['solar_range']
         except KeyError:
             solar_range = None
 
         # If necessary, get the solar range from the target name
         if solar_range is None and target_body is not None:
-            target_sun_path = oops.Path.as_waypoint(target_name).wrt('SUN')
+            target_sun_path = oops.path.Path.as_waypoint(target_name).wrt('SUN')
             # Paths of the relevant bodies need to be defined in advance!
 
             sun_event = target_sun_path.event_at_time(tdb_midtime)
             solar_range = sun_event.pos.norm().vals / solar.AU
 
         if solar_range is None:
             raise IOError("Calibration can't figure out range from Sun to " +
```

### Comparing `rms-oops-0.0.2/oops/hosts/unittester.py` & `rms_oops-0.0.3/oops/hosts/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/hosts/voyager/iss.py` & `rms_oops-0.0.3/oops/hosts/voyager/iss.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         target = vicar_dict['LAB05'][31:43].rstrip()
         target = target.replace('_', ' ')
 
         filter = lab03[37:43].rstrip()
         factor = None
 
     # Interpret the GEOMED parameter
-    if 'GEOMA' in vic.get_values('TASK'):
+    if 'GEOMA' in vic['TASK']:
         assert vic.data_2d.shape == (1000,1000)
         fovs = {
             'NAC': ISS.fovs['NAC_GEOMED'],
             'WAC': ISS.fovs['WAC_GEOMED'],
         }
     else:
         fovs = ISS.fovs
```

### Comparing `rms-oops-0.0.2/oops/lightsource.py` & `rms_oops-0.0.3/oops/lightsource.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/meshgrid.py` & `rms_oops-0.0.3/oops/meshgrid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/NOTES-ABOUT-OBSERVATION-CLASSES.txt` & `rms_oops-0.0.3/oops/observation/NOTES-ABOUT-OBSERVATION-CLASSES.txt`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/__init__.py` & `rms_oops-0.0.3/oops/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/all.py` & `rms_oops-0.0.3/oops/observation/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/insitu.py` & `rms_oops-0.0.3/oops/observation/insitu.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/pixel.py` & `rms_oops-0.0.3/oops/observation/pixel.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/pushbroom.py` & `rms_oops-0.0.3/oops/observation/pushbroom.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/pushframe.py` & `rms_oops-0.0.3/oops/observation/pushframe.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/rasterscan.py` & `rms_oops-0.0.3/oops/observation/rasterscan.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/rasterslit.py` & `rms_oops-0.0.3/oops/observation/rasterslit.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/rasterslit1d.py` & `rms_oops-0.0.3/oops/observation/rasterslit1d.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/slit.py` & `rms_oops-0.0.3/oops/observation/slit.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/slit1d.py` & `rms_oops-0.0.3/oops/observation/slit1d.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/snapshot.py` & `rms_oops-0.0.3/oops/observation/snapshot.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/timedimage.py` & `rms_oops-0.0.3/oops/observation/timedimage.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/observation/unittester.py` & `rms_oops-0.0.3/oops/observation/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/__init__.py` & `rms_oops-0.0.3/oops/path/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/all.py` & `rms_oops-0.0.3/oops/path/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/circlepath.py` & `rms_oops-0.0.3/oops/path/circlepath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/coordpath.py` & `rms_oops-0.0.3/oops/path/coordpath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/fixedpath.py` & `rms_oops-0.0.3/oops/path/fixedpath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/keplerpath.py` & `rms_oops-0.0.3/oops/path/keplerpath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/linearcoordpath.py` & `rms_oops-0.0.3/oops/path/linearcoordpath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/linearpath.py` & `rms_oops-0.0.3/oops/path/linearpath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/multipath.py` & `rms_oops-0.0.3/oops/path/multipath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/spicepath.py` & `rms_oops-0.0.3/oops/path/spicepath.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/path/unittester.py` & `rms_oops-0.0.3/oops/path/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/spice_support.py` & `rms_oops-0.0.3/oops/spice_support.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/__init__.py` & `rms_oops-0.0.3/oops/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/all.py` & `rms_oops-0.0.3/oops/surface/all.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/ansa.py` & `rms_oops-0.0.3/oops/surface/ansa.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/centricellipsoid.py` & `rms_oops-0.0.3/oops/surface/centricellipsoid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/centricspheroid.py` & `rms_oops-0.0.3/oops/surface/centricspheroid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/ellipsoid.py` & `rms_oops-0.0.3/oops/surface/ellipsoid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/graphicellipsoid.py` & `rms_oops-0.0.3/oops/surface/graphicellipsoid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/graphicspheroid.py` & `rms_oops-0.0.3/oops/surface/graphicspheroid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/limb.py` & `rms_oops-0.0.3/oops/surface/limb.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/nullsurface.py` & `rms_oops-0.0.3/oops/surface/nullsurface.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/orbitplane.py` & `rms_oops-0.0.3/oops/surface/orbitplane.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/polarlimb.py` & `rms_oops-0.0.3/oops/surface/polarlimb.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/ringplane.py` & `rms_oops-0.0.3/oops/surface/ringplane.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/spheroid.py` & `rms_oops-0.0.3/oops/surface/spheroid.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/spice_shape.py` & `rms_oops-0.0.3/oops/surface/spice_shape.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/surface/unittester.py` & `rms_oops-0.0.3/oops/surface/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/transform.py` & `rms_oops-0.0.3/oops/transform.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/unittester.py` & `rms_oops-0.0.3/oops/unittester.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/unittester_support.py` & `rms_oops-0.0.3/oops/unittester_support.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/oops/utils.py` & `rms_oops-0.0.3/oops/utils.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/pyproject.toml` & `rms_oops-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/rms_oops.egg-info/SOURCES.txt` & `rms_oops-0.0.3/rms_oops.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 .coveragerc
 .flake8
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE.md
 README.md
+codecov.yml
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
 .github/workflows/run-lint.yml
 .github/workflows/run-tests.yml
```

### Comparing `rms-oops-0.0.2/scripts/automated_tests/oops_main_test.sh` & `rms_oops-0.0.3/scripts/automated_tests/oops_main_test.sh`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/spicedb/__init__.py` & `rms_oops-0.0.3/spicedb/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-oops-0.0.2/spicedb/sqlite_db.py` & `rms_oops-0.0.3/spicedb/sqlite_db.py`

 * *Files identical despite different names*

