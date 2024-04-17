# Comparing `tmp/mahotas-1.4.8.tar.gz` & `tmp/mahotas-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mahotas-1.4.8.tar", last modified: Thu Oct 10 17:57:14 2019, max compression
+gzip compressed data, was "dist/mahotas-1.4.9.tar", last modified: Tue Nov 12 12:25:30 2019, max compression
```

## Comparing `mahotas-1.4.8.tar` & `mahotas-1.4.9.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15702 2019-10-10 17:57:14.000000 mahotas-1.4.8/PKG-INFO
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      183 2012-09-05 08:15:16.000000 mahotas-1.4.8/AUTHORS
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      362 2016-10-03 20:46:05.000000 mahotas-1.4.8/MANIFEST.in
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/docs/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2344 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/Makefile
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/docs/source/
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1127 2017-01-11 17:50:34.000000 mahotas-1.4.8/docs/source/lbp.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2938 2017-11-04 18:46:59.000000 mahotas-1.4.8/docs/source/features.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2217 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/edf.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    23054 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/LBP.svg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2546 2013-10-11 12:05:56.000000 mahotas-1.4.8/docs/source/distance.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3368 2016-07-29 10:52:31.000000 mahotas-1.4.8/docs/source/index.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     5567 2017-01-11 17:50:34.000000 mahotas-1.4.8/docs/source/labeled.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2169 2014-12-03 11:04:51.000000 mahotas-1.4.8/docs/source/principles.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2555 2013-10-11 12:13:23.000000 mahotas-1.4.8/docs/source/thresholding.rst
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/docs/source/figures/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      191 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/figures/distance.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1118 2017-01-11 17:50:34.000000 mahotas-1.4.8/docs/source/polygon.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2196 2017-01-11 17:50:34.000000 mahotas-1.4.8/docs/source/contributing.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1967 2016-10-07 07:16:29.000000 mahotas-1.4.8/docs/source/wally.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4660 2014-02-12 22:05:58.000000 mahotas-1.4.8/docs/source/internals.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)      203 2013-12-16 22:02:51.000000 mahotas-1.4.8/docs/source/api.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3017 2013-10-11 12:15:21.000000 mahotas-1.4.8/docs/source/morphology.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2841 2016-10-07 07:16:29.000000 mahotas-1.4.8/docs/source/install.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3465 2013-10-11 12:15:22.000000 mahotas-1.4.8/docs/source/wavelets.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6069 2016-10-07 07:28:33.000000 mahotas-1.4.8/docs/source/conf.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1429 2017-01-11 17:50:34.000000 mahotas-1.4.8/docs/source/color.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1988 2013-10-11 12:20:39.000000 mahotas-1.4.8/docs/source/tasks.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2197 2015-07-09 09:20:27.000000 mahotas-1.4.8/docs/source/mahotas-features.rst
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2149 2019-03-18 03:34:55.000000 mahotas-1.4.8/docs/source/surf.rst
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/docs/source/_templates/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1237 2014-07-04 11:12:44.000000 mahotas-1.4.8/docs/source/_templates/sidebar.html
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/docs/source/images/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5024 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/images/zmax.jpg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4386 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/images/zbest.jpg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6835 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/images/zedf.jpg
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1399 2016-06-26 15:22:28.000000 mahotas-1.4.8/docs/source/io.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4554 2016-06-26 15:50:57.000000 mahotas-1.4.8/docs/source/faq.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4124 2015-07-03 17:04:42.000000 mahotas-1.4.8/docs/source/surfref.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    12683 2019-10-10 17:53:29.000000 mahotas-1.4.8/docs/source/history.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2813 2013-10-09 16:20:32.000000 mahotas-1.4.8/docs/source/classification.rst
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2572 2013-04-27 22:26:54.000000 mahotas-1.4.8/COPYING
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)      686 2014-02-12 22:05:58.000000 mahotas-1.4.8/Makefile
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    12669 2019-10-10 17:52:55.000000 mahotas-1.4.8/ChangeLog
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1766 2016-01-24 15:22:12.000000 mahotas-1.4.8/INSTALL
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    11805 2019-10-10 17:52:56.000000 mahotas-1.4.8/README.md
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6959 2019-04-08 03:02:16.000000 mahotas-1.4.8/mahotas/thresholding.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    24554 2019-04-08 04:58:58.000000 mahotas-1.4.8/mahotas/_labeled.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    36002 2019-07-10 17:11:17.000000 mahotas-1.4.8/mahotas/_morph.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     7076 2015-03-07 20:36:53.000000 mahotas-1.4.8/mahotas/_filters.h
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5244 2019-03-22 07:39:07.000000 mahotas-1.4.8/mahotas/colors.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5871 2019-05-31 15:38:45.000000 mahotas-1.4.8/mahotas/internal.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6823 2019-04-08 03:02:16.000000 mahotas-1.4.8/mahotas/stretch.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/features/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2092 2018-10-20 05:30:33.000000 mahotas-1.4.8/mahotas/features/moments.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    32493 2015-04-06 18:58:37.000000 mahotas-1.4.8/mahotas/features/_surf.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      490 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/features/__init__.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3435 2012-12-27 23:52:48.000000 mahotas-1.4.8/mahotas/features/tas.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2896 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/features/zernike.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2559 2013-07-04 07:57:43.000000 mahotas-1.4.8/mahotas/features/_zernike.cpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6038 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/features/lbp.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1609 2013-12-16 22:02:51.000000 mahotas-1.4.8/mahotas/features/_lbp.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3776 2019-10-10 17:51:20.000000 mahotas-1.4.8/mahotas/features/_texture.cpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)    16206 2016-10-07 19:51:55.000000 mahotas-1.4.8/mahotas/features/texture.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2385 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/features/shape.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     9919 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/features/surf.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2299 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/histogram.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1848 2013-10-11 12:24:44.000000 mahotas-1.4.8/mahotas/distance.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/tests/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2776 2015-07-09 09:20:27.000000 mahotas-1.4.8/mahotas/tests/test_lbp.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      349 2012-05-09 19:38:14.000000 mahotas-1.4.8/mahotas/tests/test_filters.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3253 2017-01-11 17:50:34.000000 mahotas-1.4.8/mahotas/tests/test_thresholding.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       38 2011-12-05 15:56:40.000000 mahotas-1.4.8/mahotas/tests/test_mahotas.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6294 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/tests/test_morph.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      520 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_template_match.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3633 2015-11-16 10:46:36.000000 mahotas-1.4.8/mahotas/tests/test_watershed.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2961 2015-06-26 12:28:00.000000 mahotas-1.4.8/mahotas/tests/test_bbox.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     8192 2015-04-27 18:48:44.000000 mahotas-1.4.8/mahotas/tests/test_convolve.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1124 2012-10-16 21:25:47.000000 mahotas-1.4.8/mahotas/tests/test_euler.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1014 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/tests/test_surf_regression.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      697 2011-12-05 15:56:40.000000 mahotas-1.4.8/mahotas/tests/test_label.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1698 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_histogram.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      848 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_bwperim.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2718 2015-01-23 20:23:27.000000 mahotas-1.4.8/mahotas/tests/test_freeimage.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      950 2012-07-17 22:36:31.000000 mahotas-1.4.8/mahotas/tests/test_tas.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6916 2016-07-29 20:04:54.000000 mahotas-1.4.8/mahotas/tests/test_texture.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      796 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_gvoronoi.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      377 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/tests/test_mean_filter.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/tests/data/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      302 2011-12-05 15:56:40.000000 mahotas-1.4.8/mahotas/tests/data/1bpp.bmp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1983 2012-07-05 11:55:49.000000 mahotas-1.4.8/mahotas/tests/data/determinant_zero.png
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      706 2012-07-05 11:55:49.000000 mahotas-1.4.8/mahotas/tests/data/rgba.png
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   339380 2013-05-10 08:46:16.000000 mahotas-1.4.8/mahotas/tests/data/luispedro.npy
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2071 2012-09-02 20:30:17.000000 mahotas-1.4.8/mahotas/tests/test_center_of_mass.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3608 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/tests/test_zernike.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1272 2017-01-11 17:50:34.000000 mahotas-1.4.8/mahotas/tests/test_median_filter.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2284 2017-01-11 17:50:34.000000 mahotas-1.4.8/mahotas/tests/test_stretch.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      709 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/tests/test_find.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)      273 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/tests/__init__.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      399 2015-04-27 18:48:44.000000 mahotas-1.4.8/mahotas/tests/test_close_holes.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      345 2013-04-21 13:35:50.000000 mahotas-1.4.8/mahotas/tests/test_segmentation.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1100 2019-05-31 14:40:55.000000 mahotas-1.4.8/mahotas/tests/test_imresize.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1934 2012-10-18 00:53:47.000000 mahotas-1.4.8/mahotas/tests/pymorph_copy.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1520 2015-01-23 20:15:13.000000 mahotas-1.4.8/mahotas/tests/test_io.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      280 2015-06-01 11:21:34.000000 mahotas-1.4.8/mahotas/tests/test_citation.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      218 2013-05-03 19:15:50.000000 mahotas-1.4.8/mahotas/tests/test_demos.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1925 2015-02-08 14:39:42.000000 mahotas-1.4.8/mahotas/tests/test_moments.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      370 2013-05-10 08:46:16.000000 mahotas-1.4.8/mahotas/tests/utils.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4970 2018-10-20 05:30:33.000000 mahotas-1.4.8/mahotas/tests/test_internal.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1321 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/tests/test_features_shape.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1482 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_hitmiss.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2058 2013-12-16 22:03:44.000000 mahotas-1.4.8/mahotas/tests/test_interpolate.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1506 2013-09-27 15:46:18.000000 mahotas-1.4.8/mahotas/tests/test_distance.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2409 2013-05-20 13:07:07.000000 mahotas-1.4.8/mahotas/tests/test_polygon.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     9829 2015-11-16 10:46:36.000000 mahotas-1.4.8/mahotas/tests/test_labeled.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1151 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/tests/test_majority.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1466 2015-12-20 20:44:16.000000 mahotas-1.4.8/mahotas/tests/test_edge.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4233 2015-04-06 19:01:10.000000 mahotas-1.4.8/mahotas/tests/test_surf.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2258 2015-06-01 11:21:34.000000 mahotas-1.4.8/mahotas/tests/test_thin.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      958 2013-06-09 07:16:31.000000 mahotas-1.4.8/mahotas/tests/test_colors.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4492 2014-01-31 14:39:15.000000 mahotas-1.4.8/mahotas/tests/test_dilate_erode.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3920 2013-07-04 07:57:43.000000 mahotas-1.4.8/mahotas/_histogram.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       28 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/freeimage.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22007 2019-04-08 03:02:16.000000 mahotas-1.4.8/mahotas/convolve.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4321 2013-09-22 19:21:06.000000 mahotas-1.4.8/mahotas/_distance.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    25190 2019-04-08 03:02:16.000000 mahotas-1.4.8/mahotas/_convolve.cpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2860 2016-10-02 12:08:44.000000 mahotas-1.4.8/mahotas/resize.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/demos/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      534 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/demos/thresholding.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      494 2015-04-27 18:48:44.000000 mahotas-1.4.8/mahotas/demos/edge_demo.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      330 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/demos/distance.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      457 2019-07-19 22:53:49.000000 mahotas-1.4.8/mahotas/demos/surf_gaussians.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      439 2019-07-19 23:03:21.000000 mahotas-1.4.8/mahotas/demos/wally.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/demos/data/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    27428 2012-12-02 12:41:48.000000 mahotas-1.4.8/mahotas/demos/data/lena.jpg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   649215 2012-12-02 12:41:48.000000 mahotas-1.4.8/mahotas/demos/data/nuclear.png
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   377235 2012-12-02 12:41:48.000000 mahotas-1.4.8/mahotas/demos/data/DepartmentStore.jpg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22735 2011-12-05 15:56:40.000000 mahotas-1.4.8/mahotas/demos/data/luispedro.jpg
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1466 2014-07-04 11:12:44.000000 mahotas-1.4.8/mahotas/demos/__init__.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      986 2019-07-19 23:04:27.000000 mahotas-1.4.8/mahotas/demos/nuclear.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      341 2019-07-19 22:53:24.000000 mahotas-1.4.8/mahotas/demos/morphology.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      673 2019-07-19 22:51:44.000000 mahotas-1.4.8/mahotas/demos/surf_luispedro.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      556 2018-10-02 10:10:10.000000 mahotas-1.4.8/mahotas/demos/superpixels.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      723 2019-07-19 23:12:24.000000 mahotas-1.4.8/mahotas/demos/nuclear_distance_watershed.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1410 2012-08-28 21:28:30.000000 mahotas-1.4.8/mahotas/demos/wavelet_compress.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/moments.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       22 2019-10-10 17:53:04.000000 mahotas-1.4.8/mahotas/mahotas_version.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2200 2013-07-04 07:57:43.000000 mahotas-1.4.8/mahotas/utils.hpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    18309 2019-07-19 22:54:55.000000 mahotas-1.4.8/mahotas/labeled.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     5242 2016-10-02 12:08:44.000000 mahotas-1.4.8/mahotas/__init__.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      133 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/tas.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4822 2015-06-01 11:21:34.000000 mahotas-1.4.8/mahotas/_thin.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     7148 2015-06-03 10:11:44.000000 mahotas-1.4.8/mahotas/_bbox.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2502 2013-07-04 07:57:43.000000 mahotas-1.4.8/mahotas/_convex.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    11171 2019-05-31 14:41:30.000000 mahotas-1.4.8/mahotas/interpolate.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3733 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/polygon.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/zernike.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/numpypp/
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2726 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/numpypp/numpy.hpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2523 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/numpypp/dispatch.hpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)    21149 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/numpypp/array.hpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2984 2013-12-13 11:42:08.000000 mahotas-1.4.8/mahotas/segmentation.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      133 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/lbp.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5684 2015-07-03 17:01:14.000000 mahotas-1.4.8/mahotas/edge.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1073 2015-06-01 11:21:34.000000 mahotas-1.4.8/mahotas/thin.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22602 2019-07-09 14:31:34.000000 mahotas-1.4.8/mahotas/morph.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/texture.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1846 2016-10-07 07:16:29.000000 mahotas-1.4.8/mahotas/bbox.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1619 2015-11-16 15:51:12.000000 mahotas-1.4.8/mahotas/center_of_mass.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      283 2012-07-17 22:36:31.000000 mahotas-1.4.8/mahotas/bwperim.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3976 2013-09-27 15:46:18.000000 mahotas-1.4.8/mahotas/_center_of_mass.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1851 2019-04-08 03:02:16.000000 mahotas-1.4.8/mahotas/euler.py
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas/io/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    23535 2019-05-31 14:36:56.000000 mahotas-1.4.8/mahotas/io/freeimage.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1909 2019-07-19 22:58:04.000000 mahotas-1.4.8/mahotas/io/__init__.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      837 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/io/pil.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     7438 2013-12-21 12:02:05.000000 mahotas-1.4.8/mahotas/_filters.cpp
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15966 2019-05-31 14:41:30.000000 mahotas-1.4.8/mahotas/_interpolate.cpp
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4669 2016-10-04 10:27:07.000000 mahotas-1.4.8/mahotas/features_cli.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1211 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/debug.h
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      682 2014-12-03 11:04:51.000000 mahotas-1.4.8/mahotas/_filters.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      135 2012-04-05 18:15:06.000000 mahotas-1.4.8/mahotas/surf.py
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)       40 2016-10-07 07:28:33.000000 mahotas-1.4.8/readthedocs-requirements.txt
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       38 2019-10-10 17:57:14.000000 mahotas-1.4.8/setup.cfg
-drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15702 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/PKG-INFO
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        1 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/dependency_links.txt
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4543 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/SOURCES.txt
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)       64 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/entry_points.txt
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        6 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/requires.txt
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        8 2019-10-10 17:57:14.000000 mahotas-1.4.8/mahotas.egg-info/top_level.txt
--rw-r--r--   0 luispedro  (1001) luispedro  (1001)       18 2017-11-04 18:46:59.000000 mahotas-1.4.8/tests-requirements.txt
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5539 2019-07-19 22:54:22.000000 mahotas-1.4.8/setup.py
--rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        6 2012-04-05 18:15:06.000000 mahotas-1.4.8/requirements.txt
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15807 2019-11-12 12:25:30.000000 mahotas-1.4.9/PKG-INFO
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      183 2012-09-05 08:15:16.000000 mahotas-1.4.9/AUTHORS
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      362 2016-10-03 20:46:05.000000 mahotas-1.4.9/MANIFEST.in
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/docs/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2344 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/Makefile
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/docs/source/
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1127 2017-01-11 17:50:34.000000 mahotas-1.4.9/docs/source/lbp.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2938 2017-11-04 18:46:59.000000 mahotas-1.4.9/docs/source/features.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2217 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/edf.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    23054 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/LBP.svg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2546 2013-10-11 12:05:56.000000 mahotas-1.4.9/docs/source/distance.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3368 2016-07-29 10:52:31.000000 mahotas-1.4.9/docs/source/index.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     5567 2017-01-11 17:50:34.000000 mahotas-1.4.9/docs/source/labeled.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2169 2014-12-03 11:04:51.000000 mahotas-1.4.9/docs/source/principles.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2555 2013-10-11 12:13:23.000000 mahotas-1.4.9/docs/source/thresholding.rst
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/docs/source/figures/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      191 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/figures/distance.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1118 2017-01-11 17:50:34.000000 mahotas-1.4.9/docs/source/polygon.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2196 2017-01-11 17:50:34.000000 mahotas-1.4.9/docs/source/contributing.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1967 2016-10-07 07:16:29.000000 mahotas-1.4.9/docs/source/wally.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4660 2014-02-12 22:05:58.000000 mahotas-1.4.9/docs/source/internals.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)      203 2013-12-16 22:02:51.000000 mahotas-1.4.9/docs/source/api.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3017 2013-10-11 12:15:21.000000 mahotas-1.4.9/docs/source/morphology.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2841 2016-10-07 07:16:29.000000 mahotas-1.4.9/docs/source/install.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3465 2013-10-11 12:15:22.000000 mahotas-1.4.9/docs/source/wavelets.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6069 2016-10-07 07:28:33.000000 mahotas-1.4.9/docs/source/conf.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1429 2017-01-11 17:50:34.000000 mahotas-1.4.9/docs/source/color.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1988 2013-10-11 12:20:39.000000 mahotas-1.4.9/docs/source/tasks.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2197 2015-07-09 09:20:27.000000 mahotas-1.4.9/docs/source/mahotas-features.rst
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2149 2019-03-18 03:34:55.000000 mahotas-1.4.9/docs/source/surf.rst
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/docs/source/_templates/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1237 2014-07-04 11:12:44.000000 mahotas-1.4.9/docs/source/_templates/sidebar.html
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/docs/source/images/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5024 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/images/zmax.jpg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4386 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/images/zbest.jpg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6835 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/images/zedf.jpg
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1399 2016-06-26 15:22:28.000000 mahotas-1.4.9/docs/source/io.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4554 2016-06-26 15:50:57.000000 mahotas-1.4.9/docs/source/faq.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4124 2015-07-03 17:04:42.000000 mahotas-1.4.9/docs/source/surfref.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    12781 2019-11-12 11:52:15.000000 mahotas-1.4.9/docs/source/history.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2813 2013-10-09 16:20:32.000000 mahotas-1.4.9/docs/source/classification.rst
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2572 2013-04-27 22:26:54.000000 mahotas-1.4.9/COPYING
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)      686 2014-02-12 22:05:58.000000 mahotas-1.4.9/Makefile
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    12748 2019-11-12 11:52:15.000000 mahotas-1.4.9/ChangeLog
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1766 2016-01-24 15:22:12.000000 mahotas-1.4.9/INSTALL
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    11878 2019-11-12 11:52:15.000000 mahotas-1.4.9/README.md
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6959 2019-04-08 03:02:16.000000 mahotas-1.4.9/mahotas/thresholding.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    24554 2019-04-08 04:58:58.000000 mahotas-1.4.9/mahotas/_labeled.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    36002 2019-07-10 17:11:17.000000 mahotas-1.4.9/mahotas/_morph.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     7076 2015-03-07 20:36:53.000000 mahotas-1.4.9/mahotas/_filters.h
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5244 2019-03-22 07:39:07.000000 mahotas-1.4.9/mahotas/colors.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5871 2019-05-31 15:38:45.000000 mahotas-1.4.9/mahotas/internal.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6823 2019-04-08 03:02:16.000000 mahotas-1.4.9/mahotas/stretch.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/features/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2092 2018-10-20 05:30:33.000000 mahotas-1.4.9/mahotas/features/moments.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    32493 2015-04-06 18:58:37.000000 mahotas-1.4.9/mahotas/features/_surf.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      490 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/features/__init__.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3435 2012-12-27 23:52:48.000000 mahotas-1.4.9/mahotas/features/tas.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2896 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/features/zernike.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2559 2013-07-04 07:57:43.000000 mahotas-1.4.9/mahotas/features/_zernike.cpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6038 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/features/lbp.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1609 2013-12-16 22:02:51.000000 mahotas-1.4.9/mahotas/features/_lbp.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3776 2019-10-10 17:51:20.000000 mahotas-1.4.9/mahotas/features/_texture.cpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)    16206 2016-10-07 19:51:55.000000 mahotas-1.4.9/mahotas/features/texture.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2385 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/features/shape.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     9919 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/features/surf.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2299 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/histogram.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1848 2013-10-11 12:24:44.000000 mahotas-1.4.9/mahotas/distance.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/tests/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2776 2015-07-09 09:20:27.000000 mahotas-1.4.9/mahotas/tests/test_lbp.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      349 2012-05-09 19:38:14.000000 mahotas-1.4.9/mahotas/tests/test_filters.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3253 2017-01-11 17:50:34.000000 mahotas-1.4.9/mahotas/tests/test_thresholding.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       38 2011-12-05 15:56:40.000000 mahotas-1.4.9/mahotas/tests/test_mahotas.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     6294 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/tests/test_morph.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      520 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_template_match.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3633 2015-11-16 10:46:36.000000 mahotas-1.4.9/mahotas/tests/test_watershed.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2961 2015-06-26 12:28:00.000000 mahotas-1.4.9/mahotas/tests/test_bbox.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     8192 2015-04-27 18:48:44.000000 mahotas-1.4.9/mahotas/tests/test_convolve.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1124 2012-10-16 21:25:47.000000 mahotas-1.4.9/mahotas/tests/test_euler.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1014 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/tests/test_surf_regression.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      697 2011-12-05 15:56:40.000000 mahotas-1.4.9/mahotas/tests/test_label.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1698 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_histogram.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      848 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_bwperim.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2718 2015-01-23 20:23:27.000000 mahotas-1.4.9/mahotas/tests/test_freeimage.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      950 2012-07-17 22:36:31.000000 mahotas-1.4.9/mahotas/tests/test_tas.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     6916 2016-07-29 20:04:54.000000 mahotas-1.4.9/mahotas/tests/test_texture.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      796 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_gvoronoi.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      377 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/tests/test_mean_filter.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/tests/data/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      302 2011-12-05 15:56:40.000000 mahotas-1.4.9/mahotas/tests/data/1bpp.bmp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1983 2012-07-05 11:55:49.000000 mahotas-1.4.9/mahotas/tests/data/determinant_zero.png
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      706 2012-07-05 11:55:49.000000 mahotas-1.4.9/mahotas/tests/data/rgba.png
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   339380 2013-05-10 08:46:16.000000 mahotas-1.4.9/mahotas/tests/data/luispedro.npy
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2071 2012-09-02 20:30:17.000000 mahotas-1.4.9/mahotas/tests/test_center_of_mass.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3608 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/tests/test_zernike.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1272 2017-01-11 17:50:34.000000 mahotas-1.4.9/mahotas/tests/test_median_filter.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2284 2017-01-11 17:50:34.000000 mahotas-1.4.9/mahotas/tests/test_stretch.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      709 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/tests/test_find.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)      273 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/tests/__init__.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      399 2015-04-27 18:48:44.000000 mahotas-1.4.9/mahotas/tests/test_close_holes.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      345 2013-04-21 13:35:50.000000 mahotas-1.4.9/mahotas/tests/test_segmentation.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1100 2019-05-31 14:40:55.000000 mahotas-1.4.9/mahotas/tests/test_imresize.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1934 2012-10-18 00:53:47.000000 mahotas-1.4.9/mahotas/tests/pymorph_copy.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1520 2015-01-23 20:15:13.000000 mahotas-1.4.9/mahotas/tests/test_io.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      280 2015-06-01 11:21:34.000000 mahotas-1.4.9/mahotas/tests/test_citation.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      218 2013-05-03 19:15:50.000000 mahotas-1.4.9/mahotas/tests/test_demos.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1925 2015-02-08 14:39:42.000000 mahotas-1.4.9/mahotas/tests/test_moments.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      370 2013-05-10 08:46:16.000000 mahotas-1.4.9/mahotas/tests/utils.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4970 2018-10-20 05:30:33.000000 mahotas-1.4.9/mahotas/tests/test_internal.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1321 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/tests/test_features_shape.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1482 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_hitmiss.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2058 2013-12-16 22:03:44.000000 mahotas-1.4.9/mahotas/tests/test_interpolate.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1506 2013-09-27 15:46:18.000000 mahotas-1.4.9/mahotas/tests/test_distance.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2409 2013-05-20 13:07:07.000000 mahotas-1.4.9/mahotas/tests/test_polygon.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     9829 2015-11-16 10:46:36.000000 mahotas-1.4.9/mahotas/tests/test_labeled.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1151 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/tests/test_majority.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1466 2015-12-20 20:44:16.000000 mahotas-1.4.9/mahotas/tests/test_edge.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4233 2015-04-06 19:01:10.000000 mahotas-1.4.9/mahotas/tests/test_surf.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2258 2015-06-01 11:21:34.000000 mahotas-1.4.9/mahotas/tests/test_thin.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      958 2013-06-09 07:16:31.000000 mahotas-1.4.9/mahotas/tests/test_colors.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4492 2014-01-31 14:39:15.000000 mahotas-1.4.9/mahotas/tests/test_dilate_erode.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3920 2013-07-04 07:57:43.000000 mahotas-1.4.9/mahotas/_histogram.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       28 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/freeimage.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22007 2019-04-08 03:02:16.000000 mahotas-1.4.9/mahotas/convolve.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4321 2013-09-22 19:21:06.000000 mahotas-1.4.9/mahotas/_distance.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    25190 2019-04-08 03:02:16.000000 mahotas-1.4.9/mahotas/_convolve.cpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2860 2016-10-02 12:08:44.000000 mahotas-1.4.9/mahotas/resize.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/demos/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      534 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/demos/thresholding.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      494 2015-04-27 18:48:44.000000 mahotas-1.4.9/mahotas/demos/edge_demo.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      330 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/demos/distance.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      457 2019-07-19 22:53:49.000000 mahotas-1.4.9/mahotas/demos/surf_gaussians.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      439 2019-07-19 23:03:21.000000 mahotas-1.4.9/mahotas/demos/wally.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/demos/data/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    27428 2012-12-02 12:41:48.000000 mahotas-1.4.9/mahotas/demos/data/lena.jpg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   649215 2012-12-02 12:41:48.000000 mahotas-1.4.9/mahotas/demos/data/nuclear.png
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)   377235 2012-12-02 12:41:48.000000 mahotas-1.4.9/mahotas/demos/data/DepartmentStore.jpg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22735 2011-12-05 15:56:40.000000 mahotas-1.4.9/mahotas/demos/data/luispedro.jpg
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1466 2014-07-04 11:12:44.000000 mahotas-1.4.9/mahotas/demos/__init__.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      986 2019-07-19 23:04:27.000000 mahotas-1.4.9/mahotas/demos/nuclear.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      341 2019-07-19 22:53:24.000000 mahotas-1.4.9/mahotas/demos/morphology.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      673 2019-07-19 22:51:44.000000 mahotas-1.4.9/mahotas/demos/surf_luispedro.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      556 2018-10-02 10:10:10.000000 mahotas-1.4.9/mahotas/demos/superpixels.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      723 2019-07-19 23:12:24.000000 mahotas-1.4.9/mahotas/demos/nuclear_distance_watershed.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1410 2012-08-28 21:28:30.000000 mahotas-1.4.9/mahotas/demos/wavelet_compress.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/moments.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       22 2019-11-12 11:52:15.000000 mahotas-1.4.9/mahotas/mahotas_version.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2200 2013-07-04 07:57:43.000000 mahotas-1.4.9/mahotas/utils.hpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    18309 2019-07-19 22:54:55.000000 mahotas-1.4.9/mahotas/labeled.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     5242 2016-10-02 12:08:44.000000 mahotas-1.4.9/mahotas/__init__.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      133 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/tas.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4822 2015-06-01 11:21:34.000000 mahotas-1.4.9/mahotas/_thin.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     7148 2015-06-03 10:11:44.000000 mahotas-1.4.9/mahotas/_bbox.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2502 2013-07-04 07:57:43.000000 mahotas-1.4.9/mahotas/_convex.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    11171 2019-05-31 14:41:30.000000 mahotas-1.4.9/mahotas/interpolate.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     3733 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/polygon.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/zernike.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/numpypp/
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2726 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/numpypp/numpy.hpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2523 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/numpypp/dispatch.hpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)    21149 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/numpypp/array.hpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     2984 2013-12-13 11:42:08.000000 mahotas-1.4.9/mahotas/segmentation.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      133 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/lbp.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5684 2015-07-03 17:01:14.000000 mahotas-1.4.9/mahotas/edge.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1073 2015-06-01 11:21:34.000000 mahotas-1.4.9/mahotas/thin.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    22602 2019-07-09 14:31:34.000000 mahotas-1.4.9/mahotas/morph.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      141 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/texture.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     1846 2016-10-07 07:16:29.000000 mahotas-1.4.9/mahotas/bbox.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1619 2015-11-16 15:51:12.000000 mahotas-1.4.9/mahotas/center_of_mass.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      283 2012-07-17 22:36:31.000000 mahotas-1.4.9/mahotas/bwperim.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     3976 2013-09-27 15:46:18.000000 mahotas-1.4.9/mahotas/_center_of_mass.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1851 2019-04-08 03:02:16.000000 mahotas-1.4.9/mahotas/euler.py
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas/io/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    23535 2019-05-31 14:36:56.000000 mahotas-1.4.9/mahotas/io/freeimage.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     2000 2019-11-12 11:52:15.000000 mahotas-1.4.9/mahotas/io/__init__.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      837 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/io/pil.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     7438 2013-12-21 12:02:05.000000 mahotas-1.4.9/mahotas/_filters.cpp
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15966 2019-05-31 14:41:30.000000 mahotas-1.4.9/mahotas/_interpolate.cpp
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)     4669 2016-10-04 10:27:07.000000 mahotas-1.4.9/mahotas/features_cli.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     1211 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/debug.h
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      682 2014-12-03 11:04:51.000000 mahotas-1.4.9/mahotas/_filters.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)      135 2012-04-05 18:15:06.000000 mahotas-1.4.9/mahotas/surf.py
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)       40 2016-10-07 07:28:33.000000 mahotas-1.4.9/readthedocs-requirements.txt
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)       38 2019-11-12 12:25:30.000000 mahotas-1.4.9/setup.cfg
+drwxrwxr-x   0 luispedro  (1001) luispedro  (1001)        0 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)    15807 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/PKG-INFO
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        1 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/dependency_links.txt
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     4543 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/SOURCES.txt
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)       64 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/entry_points.txt
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        6 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/requires.txt
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        8 2019-11-12 12:25:30.000000 mahotas-1.4.9/mahotas.egg-info/top_level.txt
+-rw-r--r--   0 luispedro  (1001) luispedro  (1001)       18 2017-11-04 18:46:59.000000 mahotas-1.4.9/tests-requirements.txt
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)     5539 2019-07-19 22:54:22.000000 mahotas-1.4.9/setup.py
+-rw-rw-r--   0 luispedro  (1001) luispedro  (1001)        6 2012-04-05 18:15:06.000000 mahotas-1.4.9/requirements.txt
```

### Comparing `mahotas-1.4.8/PKG-INFO` & `mahotas-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahotas
-Version: 1.4.8
+Version: 1.4.9
 Summary: Mahotas: Computer Vision Library
 Home-page: http://luispedro.org/software/mahotas
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Description: # Mahotas
         
@@ -224,14 +224,18 @@
         list](http://groups.google.com/group/pythonvision?pli=1) is a much
         better venue and generates a public discussion log for others in the
         future. You can use it for mahotas or general computer vision in Python
         questions.
         
         ## Recent Changes
         
+        ### Version 1.4.9 (Nov 12 2019)
+        
+        - Fix FreeImage detection (issue #108)
+        
         ### Version 1.4.8 (Oct 11 2019)
         
         - Fix co-occurrence matrix computation (patch by @databaaz)
         
         ### Version 1.4.7 (Jul 10 2019)
         
         - Fix compilation on Windows
```

### Comparing `mahotas-1.4.8/docs/Makefile` & `mahotas-1.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/lbp.rst` & `mahotas-1.4.9/docs/source/lbp.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/features.rst` & `mahotas-1.4.9/docs/source/features.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/edf.rst` & `mahotas-1.4.9/docs/source/edf.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/LBP.svg` & `mahotas-1.4.9/docs/source/LBP.svg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/distance.rst` & `mahotas-1.4.9/docs/source/distance.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/index.rst` & `mahotas-1.4.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/labeled.rst` & `mahotas-1.4.9/docs/source/labeled.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/principles.rst` & `mahotas-1.4.9/docs/source/principles.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/thresholding.rst` & `mahotas-1.4.9/docs/source/thresholding.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/polygon.rst` & `mahotas-1.4.9/docs/source/polygon.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/contributing.rst` & `mahotas-1.4.9/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/wally.rst` & `mahotas-1.4.9/docs/source/wally.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/internals.rst` & `mahotas-1.4.9/docs/source/internals.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/morphology.rst` & `mahotas-1.4.9/docs/source/morphology.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/install.rst` & `mahotas-1.4.9/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/wavelets.rst` & `mahotas-1.4.9/docs/source/wavelets.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/conf.py` & `mahotas-1.4.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/color.rst` & `mahotas-1.4.9/docs/source/color.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/tasks.rst` & `mahotas-1.4.9/docs/source/tasks.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/mahotas-features.rst` & `mahotas-1.4.9/docs/source/mahotas-features.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/surf.rst` & `mahotas-1.4.9/docs/source/surf.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/_templates/sidebar.html` & `mahotas-1.4.9/docs/source/_templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/images/zmax.jpg` & `mahotas-1.4.9/docs/source/images/zmax.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/images/zbest.jpg` & `mahotas-1.4.9/docs/source/images/zbest.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/images/zedf.jpg` & `mahotas-1.4.9/docs/source/images/zedf.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/io.rst` & `mahotas-1.4.9/docs/source/io.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/faq.rst` & `mahotas-1.4.9/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/surfref.rst` & `mahotas-1.4.9/docs/source/surfref.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/docs/source/history.rst` & `mahotas-1.4.9/docs/source/history.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+Version 1.4.9 (Nov 12 2019)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Fix FreeImage detection (issue #108)
+
+
 Version 1.4.8 (Oct 11 2019)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 - Fix co-occurrence matrix computation (patch by @databaaz)
 
 Version 1.4.7 (Jul 10 2019)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `mahotas-1.4.8/docs/source/classification.rst` & `mahotas-1.4.9/docs/source/classification.rst`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/COPYING` & `mahotas-1.4.9/COPYING`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/Makefile` & `mahotas-1.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/ChangeLog` & `mahotas-1.4.9/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Version 1.4.9 2019-11-12 by luispedro
+	* Fix FreeImage detection (issue #108)
+
 Version 1.4.8 2019-10-11 by luispedro
 	* Fix co-occurrence matrix computation (patch by @databaaz)
 
 Version 1.4.7 2019-07-10 by luispedro
 	* Fix compilation on Windows
 
 Version 1.4.6 2019-07-10 by luispedro
```

### Comparing `mahotas-1.4.8/INSTALL` & `mahotas-1.4.9/INSTALL`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/README.md` & `mahotas-1.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,18 @@
 list](http://groups.google.com/group/pythonvision?pli=1) is a much
 better venue and generates a public discussion log for others in the
 future. You can use it for mahotas or general computer vision in Python
 questions.
 
 ## Recent Changes
 
+### Version 1.4.9 (Nov 12 2019)
+
+- Fix FreeImage detection (issue #108)
+
 ### Version 1.4.8 (Oct 11 2019)
 
 - Fix co-occurrence matrix computation (patch by @databaaz)
 
 ### Version 1.4.7 (Jul 10 2019)
 
 - Fix compilation on Windows
```

### Comparing `mahotas-1.4.8/mahotas/thresholding.py` & `mahotas-1.4.9/mahotas/thresholding.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_labeled.cpp` & `mahotas-1.4.9/mahotas/_labeled.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_morph.cpp` & `mahotas-1.4.9/mahotas/_morph.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_filters.h` & `mahotas-1.4.9/mahotas/_filters.h`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/colors.py` & `mahotas-1.4.9/mahotas/colors.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/internal.py` & `mahotas-1.4.9/mahotas/internal.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/stretch.py` & `mahotas-1.4.9/mahotas/stretch.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/moments.py` & `mahotas-1.4.9/mahotas/features/moments.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/_surf.cpp` & `mahotas-1.4.9/mahotas/features/_surf.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/tas.py` & `mahotas-1.4.9/mahotas/features/tas.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/zernike.py` & `mahotas-1.4.9/mahotas/features/zernike.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/_zernike.cpp` & `mahotas-1.4.9/mahotas/features/_zernike.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/lbp.py` & `mahotas-1.4.9/mahotas/features/lbp.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/_lbp.cpp` & `mahotas-1.4.9/mahotas/features/_lbp.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/_texture.cpp` & `mahotas-1.4.9/mahotas/features/_texture.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/texture.py` & `mahotas-1.4.9/mahotas/features/texture.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/shape.py` & `mahotas-1.4.9/mahotas/features/shape.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features/surf.py` & `mahotas-1.4.9/mahotas/features/surf.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/histogram.py` & `mahotas-1.4.9/mahotas/histogram.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/distance.py` & `mahotas-1.4.9/mahotas/distance.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_lbp.py` & `mahotas-1.4.9/mahotas/tests/test_lbp.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_thresholding.py` & `mahotas-1.4.9/mahotas/tests/test_thresholding.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_morph.py` & `mahotas-1.4.9/mahotas/tests/test_morph.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_template_match.py` & `mahotas-1.4.9/mahotas/tests/test_template_match.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_watershed.py` & `mahotas-1.4.9/mahotas/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_bbox.py` & `mahotas-1.4.9/mahotas/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_convolve.py` & `mahotas-1.4.9/mahotas/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_euler.py` & `mahotas-1.4.9/mahotas/tests/test_euler.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_surf_regression.py` & `mahotas-1.4.9/mahotas/tests/test_surf_regression.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_label.py` & `mahotas-1.4.9/mahotas/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_histogram.py` & `mahotas-1.4.9/mahotas/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_bwperim.py` & `mahotas-1.4.9/mahotas/tests/test_bwperim.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_freeimage.py` & `mahotas-1.4.9/mahotas/tests/test_freeimage.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_tas.py` & `mahotas-1.4.9/mahotas/tests/test_tas.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_texture.py` & `mahotas-1.4.9/mahotas/tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_gvoronoi.py` & `mahotas-1.4.9/mahotas/tests/test_gvoronoi.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/data/determinant_zero.png` & `mahotas-1.4.9/mahotas/tests/data/determinant_zero.png`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/data/rgba.png` & `mahotas-1.4.9/mahotas/tests/data/rgba.png`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/data/luispedro.npy` & `mahotas-1.4.9/mahotas/tests/data/luispedro.npy`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_center_of_mass.py` & `mahotas-1.4.9/mahotas/tests/test_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_zernike.py` & `mahotas-1.4.9/mahotas/tests/test_zernike.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_median_filter.py` & `mahotas-1.4.9/mahotas/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_stretch.py` & `mahotas-1.4.9/mahotas/tests/test_stretch.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_find.py` & `mahotas-1.4.9/mahotas/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_imresize.py` & `mahotas-1.4.9/mahotas/tests/test_imresize.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/pymorph_copy.py` & `mahotas-1.4.9/mahotas/tests/pymorph_copy.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_io.py` & `mahotas-1.4.9/mahotas/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_moments.py` & `mahotas-1.4.9/mahotas/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_internal.py` & `mahotas-1.4.9/mahotas/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_features_shape.py` & `mahotas-1.4.9/mahotas/tests/test_features_shape.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_hitmiss.py` & `mahotas-1.4.9/mahotas/tests/test_hitmiss.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_interpolate.py` & `mahotas-1.4.9/mahotas/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_distance.py` & `mahotas-1.4.9/mahotas/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_polygon.py` & `mahotas-1.4.9/mahotas/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_labeled.py` & `mahotas-1.4.9/mahotas/tests/test_labeled.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_majority.py` & `mahotas-1.4.9/mahotas/tests/test_majority.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_edge.py` & `mahotas-1.4.9/mahotas/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_surf.py` & `mahotas-1.4.9/mahotas/tests/test_surf.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_thin.py` & `mahotas-1.4.9/mahotas/tests/test_thin.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_colors.py` & `mahotas-1.4.9/mahotas/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/tests/test_dilate_erode.py` & `mahotas-1.4.9/mahotas/tests/test_dilate_erode.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_histogram.cpp` & `mahotas-1.4.9/mahotas/_histogram.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/convolve.py` & `mahotas-1.4.9/mahotas/convolve.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_distance.cpp` & `mahotas-1.4.9/mahotas/_distance.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_convolve.cpp` & `mahotas-1.4.9/mahotas/_convolve.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/resize.py` & `mahotas-1.4.9/mahotas/resize.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/thresholding.py` & `mahotas-1.4.9/mahotas/demos/thresholding.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/data/lena.jpg` & `mahotas-1.4.9/mahotas/demos/data/lena.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/data/nuclear.png` & `mahotas-1.4.9/mahotas/demos/data/nuclear.png`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/data/DepartmentStore.jpg` & `mahotas-1.4.9/mahotas/demos/data/DepartmentStore.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/data/luispedro.jpg` & `mahotas-1.4.9/mahotas/demos/data/luispedro.jpg`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/__init__.py` & `mahotas-1.4.9/mahotas/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/nuclear.py` & `mahotas-1.4.9/mahotas/demos/nuclear.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/surf_luispedro.py` & `mahotas-1.4.9/mahotas/demos/surf_luispedro.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/superpixels.py` & `mahotas-1.4.9/mahotas/demos/superpixels.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/nuclear_distance_watershed.py` & `mahotas-1.4.9/mahotas/demos/nuclear_distance_watershed.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/demos/wavelet_compress.py` & `mahotas-1.4.9/mahotas/demos/wavelet_compress.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/utils.hpp` & `mahotas-1.4.9/mahotas/utils.hpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/labeled.py` & `mahotas-1.4.9/mahotas/labeled.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/__init__.py` & `mahotas-1.4.9/mahotas/__init__.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_thin.cpp` & `mahotas-1.4.9/mahotas/_thin.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_bbox.cpp` & `mahotas-1.4.9/mahotas/_bbox.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_convex.cpp` & `mahotas-1.4.9/mahotas/_convex.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/interpolate.py` & `mahotas-1.4.9/mahotas/interpolate.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/polygon.py` & `mahotas-1.4.9/mahotas/polygon.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/numpypp/numpy.hpp` & `mahotas-1.4.9/mahotas/numpypp/numpy.hpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/numpypp/dispatch.hpp` & `mahotas-1.4.9/mahotas/numpypp/dispatch.hpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/numpypp/array.hpp` & `mahotas-1.4.9/mahotas/numpypp/array.hpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/segmentation.py` & `mahotas-1.4.9/mahotas/segmentation.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/edge.py` & `mahotas-1.4.9/mahotas/edge.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/thin.py` & `mahotas-1.4.9/mahotas/thin.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/morph.py` & `mahotas-1.4.9/mahotas/morph.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/bbox.py` & `mahotas-1.4.9/mahotas/bbox.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/center_of_mass.py` & `mahotas-1.4.9/mahotas/center_of_mass.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_center_of_mass.cpp` & `mahotas-1.4.9/mahotas/_center_of_mass.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/euler.py` & `mahotas-1.4.9/mahotas/euler.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/io/freeimage.py` & `mahotas-1.4.9/mahotas/io/freeimage.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/io/__init__.py` & `mahotas-1.4.9/mahotas/io/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     try:
         from imread import imread, imsave
     except ImportError: # pragma: no cover
         try:
             from .pil import imread, imsave
         except ImportError:
             from .freeimage import imread, imsave
-except ImportError: # pragma: no cover
+# Importing freeimage can throw both ImportError and OSError, so check for both
+except (OSError, ImportError): # pragma: no cover
     import sys
     _,e,_ = sys.exc_info()
     _error_message %= e
     imread = error_imread
     imsave = error_imsave
```

### Comparing `mahotas-1.4.8/mahotas/io/pil.py` & `mahotas-1.4.9/mahotas/io/pil.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_filters.cpp` & `mahotas-1.4.9/mahotas/_filters.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_interpolate.cpp` & `mahotas-1.4.9/mahotas/_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/features_cli.py` & `mahotas-1.4.9/mahotas/features_cli.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/debug.h` & `mahotas-1.4.9/mahotas/debug.h`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas/_filters.py` & `mahotas-1.4.9/mahotas/_filters.py`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/mahotas.egg-info/PKG-INFO` & `mahotas-1.4.9/mahotas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahotas
-Version: 1.4.8
+Version: 1.4.9
 Summary: Mahotas: Computer Vision Library
 Home-page: http://luispedro.org/software/mahotas
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Description: # Mahotas
         
@@ -224,14 +224,18 @@
         list](http://groups.google.com/group/pythonvision?pli=1) is a much
         better venue and generates a public discussion log for others in the
         future. You can use it for mahotas or general computer vision in Python
         questions.
         
         ## Recent Changes
         
+        ### Version 1.4.9 (Nov 12 2019)
+        
+        - Fix FreeImage detection (issue #108)
+        
         ### Version 1.4.8 (Oct 11 2019)
         
         - Fix co-occurrence matrix computation (patch by @databaaz)
         
         ### Version 1.4.7 (Jul 10 2019)
         
         - Fix compilation on Windows
```

### Comparing `mahotas-1.4.8/mahotas.egg-info/SOURCES.txt` & `mahotas-1.4.9/mahotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mahotas-1.4.8/setup.py` & `mahotas-1.4.9/setup.py`

 * *Files identical despite different names*

