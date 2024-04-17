# Comparing `tmp/pilgram2-2.0.4.tar.gz` & `tmp/pilgram2-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilgram2-2.0.4.tar", max compression
+gzip compressed data, was "pilgram2-2.0.5.tar", last modified: Wed Apr 17 18:26:50 2024, max compression
```

## Comparing `pilgram2-2.0.4.tar` & `pilgram2-2.0.5.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11558 2023-04-19 04:50:10.095416 pilgram2-2.0.4/LICENSE
--rw-r--r--   0        0        0     1021 2023-05-31 18:38:25.638514 pilgram2-2.0.4/pilgram2/_1977.py
--rw-r--r--   0        0        0     2634 2023-05-31 18:38:25.638514 pilgram2-2.0.4/pilgram2/__init__.py
--rw-r--r--   0        0        0      617 2023-06-01 17:46:56.534914 pilgram2-2.0.4/pilgram2/_version.py
--rw-r--r--   0        0        0     1141 2023-05-31 18:38:25.639516 pilgram2-2.0.4/pilgram2/aden.py
--rw-r--r--   0        0        0     1005 2023-05-31 18:38:25.639516 pilgram2-2.0.4/pilgram2/amaro.py
--rw-r--r--   0        0        0     1002 2023-05-31 18:38:25.639516 pilgram2-2.0.4/pilgram2/ashby.py
--rw-r--r--   0        0        0      988 2023-05-31 18:38:25.640515 pilgram2-2.0.4/pilgram2/brannan.py
--rw-r--r--   0        0        0     1236 2023-05-31 18:38:25.640515 pilgram2-2.0.4/pilgram2/brooklyn.py
--rw-r--r--   0        0        0     1074 2023-05-31 18:38:25.640515 pilgram2-2.0.4/pilgram2/charmes.py
--rw-r--r--   0        0        0      998 2023-05-31 18:38:25.640515 pilgram2-2.0.4/pilgram2/clarendon.py
--rw-r--r--   0        0        0     1070 2023-05-31 18:38:25.641514 pilgram2-2.0.4/pilgram2/crema.py
--rw-r--r--   0        0        0      993 2023-05-31 18:38:25.641514 pilgram2-2.0.4/pilgram2/css/__init__.py
--rw-r--r--   0        0        0     1580 2023-05-31 18:38:25.641514 pilgram2-2.0.4/pilgram2/css/blending/__init__.py
--rw-r--r--   0        0        0     3696 2023-05-31 18:38:25.642514 pilgram2-2.0.4/pilgram2/css/blending/alpha.py
--rw-r--r--   0        0        0     2235 2023-05-31 18:38:25.642514 pilgram2-2.0.4/pilgram2/css/blending/color.py
--rw-r--r--   0        0        0     1989 2023-05-31 18:38:25.642514 pilgram2-2.0.4/pilgram2/css/blending/color_burn.py
--rw-r--r--   0        0        0     2137 2023-05-31 18:38:25.643510 pilgram2-2.0.4/pilgram2/css/blending/color_dodge.py
--rw-r--r--   0        0        0     1378 2023-05-31 18:38:25.643510 pilgram2-2.0.4/pilgram2/css/blending/darken.py
--rw-r--r--   0        0        0     1432 2023-05-31 18:38:25.643510 pilgram2-2.0.4/pilgram2/css/blending/difference.py
--rw-r--r--   0        0        0     1558 2023-05-31 18:38:25.643510 pilgram2-2.0.4/pilgram2/css/blending/exclusion.py
--rw-r--r--   0        0        0     1956 2023-05-31 18:38:25.644511 pilgram2-2.0.4/pilgram2/css/blending/hard_light.py
--rw-r--r--   0        0        0     2285 2023-05-31 18:38:25.644511 pilgram2-2.0.4/pilgram2/css/blending/hue.py
--rw-r--r--   0        0        0     1386 2023-05-31 18:38:25.644511 pilgram2-2.0.4/pilgram2/css/blending/lighten.py
--rw-r--r--   0        0        0     1424 2023-05-31 18:38:25.645510 pilgram2-2.0.4/pilgram2/css/blending/multiply.py
--rw-r--r--   0        0        0     6124 2023-05-31 18:38:25.645510 pilgram2-2.0.4/pilgram2/css/blending/nonseparable.py
--rw-r--r--   0        0        0     1315 2023-05-31 18:38:25.645510 pilgram2-2.0.4/pilgram2/css/blending/normal.py
--rw-r--r--   0        0        0     1113 2023-05-31 18:38:25.646512 pilgram2-2.0.4/pilgram2/css/blending/overlay.py
--rw-r--r--   0        0        0     1481 2023-05-31 18:38:25.646512 pilgram2-2.0.4/pilgram2/css/blending/screen.py
--rw-r--r--   0        0        0     2606 2023-05-31 18:38:25.646512 pilgram2-2.0.4/pilgram2/css/blending/soft_light.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.647512 pilgram2-2.0.4/pilgram2/css/blending/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-05-31 18:38:25.647512 pilgram2-2.0.4/pilgram2/css/blending/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-31 18:38:25.647512 pilgram2-2.0.4/pilgram2/css/blending/tests/helpers/alpha_support.py
--rw-r--r--   0        0        0     4250 2023-05-31 18:38:25.648511 pilgram2-2.0.4/pilgram2/css/blending/tests/test_alpha.py
--rw-r--r--   0        0        0     1384 2023-05-31 18:38:25.648511 pilgram2-2.0.4/pilgram2/css/blending/tests/test_color.py
--rw-r--r--   0        0        0     1408 2023-05-31 18:38:25.648511 pilgram2-2.0.4/pilgram2/css/blending/tests/test_color_burn.py
--rw-r--r--   0        0        0     1419 2023-05-31 18:38:25.649515 pilgram2-2.0.4/pilgram2/css/blending/tests/test_color_dodge.py
--rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.649515 pilgram2-2.0.4/pilgram2/css/blending/tests/test_darken.py
--rw-r--r--   0        0        0     1061 2023-05-31 18:38:25.649515 pilgram2-2.0.4/pilgram2/css/blending/tests/test_difference.py
--rw-r--r--   0        0        0     1412 2023-05-31 18:38:25.650510 pilgram2-2.0.4/pilgram2/css/blending/tests/test_exclusion.py
--rw-r--r--   0        0        0     1434 2023-05-31 18:38:25.650510 pilgram2-2.0.4/pilgram2/css/blending/tests/test_hard_light.py
--rw-r--r--   0        0        0     1863 2023-05-31 18:38:25.650510 pilgram2-2.0.4/pilgram2/css/blending/tests/test_hue.py
--rw-r--r--   0        0        0     1049 2023-05-31 18:38:25.650510 pilgram2-2.0.4/pilgram2/css/blending/tests/test_lighten.py
--rw-r--r--   0        0        0     1053 2023-05-31 18:38:25.651513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_multiply.py
--rw-r--r--   0        0        0     5166 2023-05-31 18:38:25.651513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_nonseparable.py
--rw-r--r--   0        0        0     1529 2023-05-31 18:38:25.651513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_normal.py
--rw-r--r--   0        0        0     1654 2023-05-31 18:38:25.652513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_overlay.py
--rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.652513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_screen.py
--rw-r--r--   0        0        0     1413 2023-05-31 18:38:25.652513 pilgram2-2.0.4/pilgram2/css/blending/tests/test_soft_light.py
--rw-r--r--   0        0        0     1304 2023-05-31 18:38:25.653514 pilgram2-2.0.4/pilgram2/css/brightness.py
--rw-r--r--   0        0        0     1473 2023-05-31 18:38:25.653514 pilgram2-2.0.4/pilgram2/css/contrast.py
--rw-r--r--   0        0        0     2036 2023-05-31 18:38:25.653514 pilgram2-2.0.4/pilgram2/css/grayscale.py
--rw-r--r--   0        0        0     2578 2023-05-31 18:38:25.653514 pilgram2-2.0.4/pilgram2/css/hue_rotate.py
--rw-r--r--   0        0        0     2019 2023-05-31 18:38:25.654512 pilgram2-2.0.4/pilgram2/css/saturate.py
--rw-r--r--   0        0        0     2024 2023-05-31 18:38:25.654512 pilgram2-2.0.4/pilgram2/css/sepia.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.654512 pilgram2-2.0.4/pilgram2/css/tests/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-31 18:38:25.654512 pilgram2-2.0.4/pilgram2/css/tests/test_brightness.py
--rw-r--r--   0        0        0     2401 2023-05-31 18:38:25.655512 pilgram2-2.0.4/pilgram2/css/tests/test_contrast.py
--rw-r--r--   0        0        0     2313 2023-05-31 18:38:25.655512 pilgram2-2.0.4/pilgram2/css/tests/test_grayscale.py
--rw-r--r--   0        0        0     2741 2023-05-31 18:38:25.655512 pilgram2-2.0.4/pilgram2/css/tests/test_hue_rotate.py
--rw-r--r--   0        0        0     2321 2023-05-31 18:38:25.655512 pilgram2-2.0.4/pilgram2/css/tests/test_saturate.py
--rw-r--r--   0        0        0     2170 2023-05-31 18:38:25.656514 pilgram2-2.0.4/pilgram2/css/tests/test_sepia.py
--rw-r--r--   0        0        0      920 2023-05-31 18:38:25.656514 pilgram2-2.0.4/pilgram2/dogpatch.py
--rw-r--r--   0        0        0     1043 2023-05-31 18:38:25.656514 pilgram2-2.0.4/pilgram2/earlybird.py
--rw-r--r--   0        0        0      996 2023-05-31 18:38:25.657513 pilgram2-2.0.4/pilgram2/gingham.py
--rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.657513 pilgram2-2.0.4/pilgram2/ginza.py
--rw-r--r--   0        0        0     1157 2023-05-31 18:38:25.657513 pilgram2-2.0.4/pilgram2/hefe.py
--rw-r--r--   0        0        0     1040 2023-05-31 18:38:25.657513 pilgram2-2.0.4/pilgram2/helena.py
--rw-r--r--   0        0        0     1129 2023-05-31 18:38:25.658513 pilgram2-2.0.4/pilgram2/hudson.py
--rw-r--r--   0        0        0      960 2023-05-31 18:38:25.658513 pilgram2-2.0.4/pilgram2/inkwell.py
--rw-r--r--   0        0        0     1036 2023-05-31 18:38:25.658513 pilgram2-2.0.4/pilgram2/juno.py
--rw-r--r--   0        0        0     1011 2023-05-31 18:38:25.659513 pilgram2-2.0.4/pilgram2/kelvin.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.659513 pilgram2-2.0.4/pilgram2/lark.py
--rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.659513 pilgram2-2.0.4/pilgram2/lofi.py
--rw-r--r--   0        0        0     1037 2023-05-31 18:38:25.659513 pilgram2-2.0.4/pilgram2/ludwig.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.660513 pilgram2-2.0.4/pilgram2/maven.py
--rw-r--r--   0        0        0     1519 2023-05-31 18:38:25.660513 pilgram2-2.0.4/pilgram2/mayfair.py
--rw-r--r--   0        0        0     1103 2023-05-31 18:38:25.660513 pilgram2-2.0.4/pilgram2/moon.py
--rw-r--r--   0        0        0     1156 2023-05-31 18:38:25.661513 pilgram2-2.0.4/pilgram2/nashville.py
--rw-r--r--   0        0        0     1029 2023-05-31 18:38:25.661513 pilgram2-2.0.4/pilgram2/perpetua.py
--rw-r--r--   0        0        0     1047 2023-05-31 18:38:25.661513 pilgram2-2.0.4/pilgram2/poprocket.py
--rw-r--r--   0        0        0     1124 2023-05-31 18:38:25.661513 pilgram2-2.0.4/pilgram2/reyes.py
--rw-r--r--   0        0        0     1561 2023-05-31 18:38:25.662514 pilgram2-2.0.4/pilgram2/rise.py
--rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.662514 pilgram2-2.0.4/pilgram2/sierra.py
--rw-r--r--   0        0        0      953 2023-05-31 18:38:25.662514 pilgram2-2.0.4/pilgram2/skyline.py
--rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.662514 pilgram2-2.0.4/pilgram2/slumber.py
--rw-r--r--   0        0        0     1033 2023-05-31 18:38:25.663513 pilgram2-2.0.4/pilgram2/stinson.py
--rw-r--r--   0        0        0     1127 2023-05-31 18:38:25.663513 pilgram2-2.0.4/pilgram2/sutro.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.664526 pilgram2-2.0.4/pilgram2/tests/__init__.py
--rw-r--r--   0        0        0    63895 2023-05-31 18:38:25.664526 pilgram2-2.0.4/pilgram2/tests/assets/mtjimba.jpg
--rw-r--r--   0        0        0      840 2023-05-31 18:38:25.665525 pilgram2-2.0.4/pilgram2/tests/test_1977.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.4/pilgram2/tests/test_aden.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.4/pilgram2/tests/test_amaro.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.666524 pilgram2-2.0.4/pilgram2/tests/test_ashby.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.666524 pilgram2-2.0.4/pilgram2/tests/test_brannan.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.666524 pilgram2-2.0.4/pilgram2/tests/test_brooklyn.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.667523 pilgram2-2.0.4/pilgram2/tests/test_charmes.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.667523 pilgram2-2.0.4/pilgram2/tests/test_clarendon.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.668521 pilgram2-2.0.4/pilgram2/tests/test_crema.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.4/pilgram2/tests/test_dogpatch.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.668521 pilgram2-2.0.4/pilgram2/tests/test_earlybird.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.4/pilgram2/tests/test_gingham.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.669524 pilgram2-2.0.4/pilgram2/tests/test_ginza.py
--rw-r--r--   0        0        0      832 2023-05-31 18:38:25.669524 pilgram2-2.0.4/pilgram2/tests/test_hefe.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.669524 pilgram2-2.0.4/pilgram2/tests/test_helena.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.4/pilgram2/tests/test_hudson.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.670522 pilgram2-2.0.4/pilgram2/tests/test_inkwell.py
--rw-r--r--   0        0        0      832 2023-05-31 18:38:25.670522 pilgram2-2.0.4/pilgram2/tests/test_juno.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.4/pilgram2/tests/test_kelvin.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.4/pilgram2/tests/test_lark.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.4/pilgram2/tests/test_lofi.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.671522 pilgram2-2.0.4/pilgram2/tests/test_ludwig.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.672523 pilgram2-2.0.4/pilgram2/tests/test_maven.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.672523 pilgram2-2.0.4/pilgram2/tests/test_mayfair.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.672523 pilgram2-2.0.4/pilgram2/tests/test_moon.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.672523 pilgram2-2.0.4/pilgram2/tests/test_nashville.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.4/pilgram2/tests/test_perpetua.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.4/pilgram2/tests/test_poprocket.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.673522 pilgram2-2.0.4/pilgram2/tests/test_reyes.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.673522 pilgram2-2.0.4/pilgram2/tests/test_rise.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.674524 pilgram2-2.0.4/pilgram2/tests/test_sierra.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.674524 pilgram2-2.0.4/pilgram2/tests/test_skyline.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.674524 pilgram2-2.0.4/pilgram2/tests/test_slumber.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.4/pilgram2/tests/test_stinson.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.675526 pilgram2-2.0.4/pilgram2/tests/test_sutro.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.4/pilgram2/tests/test_toaster.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.676521 pilgram2-2.0.4/pilgram2/tests/test_valencia.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.4/pilgram2/tests/test_walden.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.4/pilgram2/tests/test_willow.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.677524 pilgram2-2.0.4/pilgram2/tests/test_xpro2.py
--rw-r--r--   0        0        0     1013 2023-05-31 18:38:25.677524 pilgram2-2.0.4/pilgram2/toaster.py
--rw-r--r--   0        0        0     1278 2023-05-31 18:38:25.677524 pilgram2-2.0.4/pilgram2/util/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.677524 pilgram2-2.0.4/pilgram2/util/add.py
--rw-r--r--   0        0        0     1010 2023-05-31 18:38:25.678524 pilgram2-2.0.4/pilgram2/util/apply_lut.py
--rw-r--r--   0        0        0      972 2023-05-31 18:38:25.679038 pilgram2-2.0.4/pilgram2/util/clip.py
--rw-r--r--   0        0        0     1439 2023-05-31 18:38:25.679038 pilgram2-2.0.4/pilgram2/util/fill.py
--rw-r--r--   0        0        0      899 2023-05-31 18:38:25.679038 pilgram2-2.0.4/pilgram2/util/invert.py
--rw-r--r--   0        0        0     2832 2023-05-31 18:38:25.679038 pilgram2-2.0.4/pilgram2/util/linear_gradient.py
--rw-r--r--   0        0        0      869 2023-05-31 18:38:25.680050 pilgram2-2.0.4/pilgram2/util/or_convert.py
--rw-r--r--   0        0        0     3801 2023-05-31 18:38:25.680050 pilgram2-2.0.4/pilgram2/util/radial_gradient.py
--rw-r--r--   0        0        0     1098 2023-05-31 18:38:25.680050 pilgram2-2.0.4/pilgram2/util/subtract.py
--rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.681046 pilgram2-2.0.4/pilgram2/util/tests/test_add.py
--rw-r--r--   0        0        0     1226 2023-05-31 18:38:25.681046 pilgram2-2.0.4/pilgram2/util/tests/test_apply_lut.py
--rw-r--r--   0        0        0     1122 2023-05-31 18:38:25.681046 pilgram2-2.0.4/pilgram2/util/tests/test_clip.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.682048 pilgram2-2.0.4/pilgram2/util/tests/test_fill.py
--rw-r--r--   0        0        0     1020 2023-05-31 18:38:25.682048 pilgram2-2.0.4/pilgram2/util/tests/test_invert.py
--rw-r--r--   0        0        0     2603 2023-05-31 18:38:25.682048 pilgram2-2.0.4/pilgram2/util/tests/test_linear_gradient.py
--rw-r--r--   0        0        0     1097 2023-05-31 18:38:25.683048 pilgram2-2.0.4/pilgram2/util/tests/test_or_convert.py
--rw-r--r--   0        0        0     4730 2023-05-31 18:38:25.683048 pilgram2-2.0.4/pilgram2/util/tests/test_radial_gradient.py
--rw-r--r--   0        0        0     1115 2023-05-31 18:38:25.683048 pilgram2-2.0.4/pilgram2/util/tests/test_subtract.py
--rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.683048 pilgram2-2.0.4/pilgram2/valencia.py
--rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.684047 pilgram2-2.0.4/pilgram2/walden.py
--rw-r--r--   0        0        0     1150 2023-05-31 18:38:25.684047 pilgram2-2.0.4/pilgram2/willow.py
--rw-r--r--   0        0        0     1344 2023-05-31 18:38:25.684047 pilgram2-2.0.4/pilgram2/xpro2.py
--rw-r--r--   0        0        0     2762 2023-12-17 18:11:21.288881 pilgram2-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2993 2023-06-01 18:14:18.605151 pilgram2-2.0.4/README.md
--rw-r--r--   0        0        0     3902 1970-01-01 00:00:00.000000 pilgram2-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 18:26:37.967493 pilgram2-2.0.5/LICENSE
+-rw-r--r--   0        0        0     3018 2024-04-17 18:26:37.967493 pilgram2-2.0.5/README.md
+-rw-r--r--   0        0        0     1021 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/_1977.py
+-rw-r--r--   0        0        0     2634 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/_version.py
+-rw-r--r--   0        0        0     1141 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/aden.py
+-rw-r--r--   0        0        0     1005 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/amaro.py
+-rw-r--r--   0        0        0     1002 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/ashby.py
+-rw-r--r--   0        0        0      988 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/brannan.py
+-rw-r--r--   0        0        0     1236 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/brooklyn.py
+-rw-r--r--   0        0        0     1074 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/charmes.py
+-rw-r--r--   0        0        0      998 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/clarendon.py
+-rw-r--r--   0        0        0     1070 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/crema.py
+-rw-r--r--   0        0        0      993 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/__init__.py
+-rw-r--r--   0        0        0     3696 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/alpha.py
+-rw-r--r--   0        0        0     2242 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/color.py
+-rw-r--r--   0        0        0     2080 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/color_burn.py
+-rw-r--r--   0        0        0     2228 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/color_dodge.py
+-rw-r--r--   0        0        0     1378 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/darken.py
+-rw-r--r--   0        0        0     1432 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/difference.py
+-rw-r--r--   0        0        0     1558 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/exclusion.py
+-rw-r--r--   0        0        0     1956 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/hard_light.py
+-rw-r--r--   0        0        0     2292 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/hue.py
+-rw-r--r--   0        0        0     1386 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/lighten.py
+-rw-r--r--   0        0        0     1424 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/multiply.py
+-rw-r--r--   0        0        0     6124 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/nonseparable.py
+-rw-r--r--   0        0        0     1315 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/normal.py
+-rw-r--r--   0        0        0     1113 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/overlay.py
+-rw-r--r--   0        0        0     1481 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/screen.py
+-rw-r--r--   0        0        0     2606 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/soft_light.py
+-rw-r--r--   0        0        0      592 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1126 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/helpers/alpha_support.py
+-rw-r--r--   0        0        0     4250 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_alpha.py
+-rw-r--r--   0        0        0     1384 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_color.py
+-rw-r--r--   0        0        0     1408 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_color_burn.py
+-rw-r--r--   0        0        0     1419 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_color_dodge.py
+-rw-r--r--   0        0        0     1045 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_darken.py
+-rw-r--r--   0        0        0     1061 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_difference.py
+-rw-r--r--   0        0        0     1412 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_exclusion.py
+-rw-r--r--   0        0        0     1434 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_hard_light.py
+-rw-r--r--   0        0        0     1863 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_hue.py
+-rw-r--r--   0        0        0     1049 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_lighten.py
+-rw-r--r--   0        0        0     1053 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_multiply.py
+-rw-r--r--   0        0        0     5441 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_nonseparable.py
+-rw-r--r--   0        0        0     1529 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_normal.py
+-rw-r--r--   0        0        0     1654 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_overlay.py
+-rw-r--r--   0        0        0     1045 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_screen.py
+-rw-r--r--   0        0        0     1413 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/blending/tests/test_soft_light.py
+-rw-r--r--   0        0        0     1304 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/brightness.py
+-rw-r--r--   0        0        0     1473 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/contrast.py
+-rw-r--r--   0        0        0     2036 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/grayscale.py
+-rw-r--r--   0        0        0     2578 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/hue_rotate.py
+-rw-r--r--   0        0        0     2019 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/saturate.py
+-rw-r--r--   0        0        0     2024 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/sepia.py
+-rw-r--r--   0        0        0      592 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_brightness.py
+-rw-r--r--   0        0        0     2401 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_contrast.py
+-rw-r--r--   0        0        0     2313 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_grayscale.py
+-rw-r--r--   0        0        0     2741 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_hue_rotate.py
+-rw-r--r--   0        0        0     2321 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_saturate.py
+-rw-r--r--   0        0        0     2170 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/css/tests/test_sepia.py
+-rw-r--r--   0        0        0      920 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/dogpatch.py
+-rw-r--r--   0        0        0     1043 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/earlybird.py
+-rw-r--r--   0        0        0      996 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/gingham.py
+-rw-r--r--   0        0        0     1069 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/ginza.py
+-rw-r--r--   0        0        0     1157 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/hefe.py
+-rw-r--r--   0        0        0     1040 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/helena.py
+-rw-r--r--   0        0        0     1129 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/hudson.py
+-rw-r--r--   0        0        0      960 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/inkwell.py
+-rw-r--r--   0        0        0     1036 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/juno.py
+-rw-r--r--   0        0        0     1011 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/kelvin.py
+-rw-r--r--   0        0        0     1048 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/lark.py
+-rw-r--r--   0        0        0     1118 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/lofi.py
+-rw-r--r--   0        0        0     1037 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/ludwig.py
+-rw-r--r--   0        0        0     1048 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/maven.py
+-rw-r--r--   0        0        0     1519 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/mayfair.py
+-rw-r--r--   0        0        0     1103 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/moon.py
+-rw-r--r--   0        0        0     1156 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/nashville.py
+-rw-r--r--   0        0        0     1029 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/perpetua.py
+-rw-r--r--   0        0        0     1047 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/poprocket.py
+-rw-r--r--   0        0        0     1124 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/reyes.py
+-rw-r--r--   0        0        0     1561 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/rise.py
+-rw-r--r--   0        0        0     1093 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/sierra.py
+-rw-r--r--   0        0        0      953 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/skyline.py
+-rw-r--r--   0        0        0     1092 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/slumber.py
+-rw-r--r--   0        0        0     1033 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/stinson.py
+-rw-r--r--   0        0        0     1127 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/sutro.py
+-rw-r--r--   0        0        0      592 2024-04-17 18:26:37.967493 pilgram2-2.0.5/pilgram2/tests/__init__.py
+-rw-r--r--   0        0        0    63895 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/assets/mtjimba.jpg
+-rw-r--r--   0        0        0      840 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_1977.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_aden.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_amaro.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_ashby.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_brannan.py
+-rw-r--r--   0        0        0      857 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_brooklyn.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_charmes.py
+-rw-r--r--   0        0        0      862 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_clarendon.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_crema.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_dogpatch.py
+-rw-r--r--   0        0        0      862 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_earlybird.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_gingham.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_ginza.py
+-rw-r--r--   0        0        0      832 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_hefe.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_helena.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_hudson.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_inkwell.py
+-rw-r--r--   0        0        0      832 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_juno.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_kelvin.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_lark.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_lofi.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_ludwig.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_maven.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_mayfair.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_moon.py
+-rw-r--r--   0        0        0      862 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_nashville.py
+-rw-r--r--   0        0        0      857 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_perpetua.py
+-rw-r--r--   0        0        0      857 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_poprocket.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_reyes.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_rise.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_sierra.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_skyline.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_slumber.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_stinson.py
+-rw-r--r--   0        0        0      837 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_sutro.py
+-rw-r--r--   0        0        0      852 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_toaster.py
+-rw-r--r--   0        0        0      857 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_valencia.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_walden.py
+-rw-r--r--   0        0        0      847 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_willow.py
+-rw-r--r--   0        0        0      842 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/tests/test_xpro2.py
+-rw-r--r--   0        0        0     1013 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/toaster.py
+-rw-r--r--   0        0        0     1278 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/add.py
+-rw-r--r--   0        0        0     1010 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/apply_lut.py
+-rw-r--r--   0        0        0      972 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/clip.py
+-rw-r--r--   0        0        0     1439 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/fill.py
+-rw-r--r--   0        0        0      899 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/invert.py
+-rw-r--r--   0        0        0     2832 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/linear_gradient.py
+-rw-r--r--   0        0        0      869 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/or_convert.py
+-rw-r--r--   0        0        0     3801 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/radial_gradient.py
+-rw-r--r--   0        0        0     1098 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/subtract.py
+-rw-r--r--   0        0        0     1092 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_add.py
+-rw-r--r--   0        0        0     1226 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_apply_lut.py
+-rw-r--r--   0        0        0     1122 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_clip.py
+-rw-r--r--   0        0        0     1048 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_fill.py
+-rw-r--r--   0        0        0     1020 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_invert.py
+-rw-r--r--   0        0        0     2603 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_linear_gradient.py
+-rw-r--r--   0        0        0     1097 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_or_convert.py
+-rw-r--r--   0        0        0     4730 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_radial_gradient.py
+-rw-r--r--   0        0        0     1115 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/util/tests/test_subtract.py
+-rw-r--r--   0        0        0     1093 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/valencia.py
+-rw-r--r--   0        0        0     1118 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/walden.py
+-rw-r--r--   0        0        0     1150 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/willow.py
+-rw-r--r--   0        0        0     1344 2024-04-17 18:26:37.971493 pilgram2-2.0.5/pilgram2/xpro2.py
+-rw-r--r--   0        0        0     2126 2024-04-17 18:26:50.755657 pilgram2-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0    16949 1970-01-01 00:00:00.000000 pilgram2-2.0.5/PKG-INFO
```

### Comparing `pilgram2-2.0.4/LICENSE` & `pilgram2-2.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `pilgram2-2.0.4/pilgram2/_1977.py` & `pilgram2-2.0.5/pilgram2/_1977.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/__init__.py` & `pilgram2-2.0.5/pilgram2/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/_version.py` & `pilgram2-2.0.5/pilgram2/_version.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/aden.py` & `pilgram2-2.0.5/pilgram2/aden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/amaro.py` & `pilgram2-2.0.5/pilgram2/amaro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/ashby.py` & `pilgram2-2.0.5/pilgram2/ashby.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/brannan.py` & `pilgram2-2.0.5/pilgram2/brannan.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/brooklyn.py` & `pilgram2-2.0.5/pilgram2/brooklyn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/charmes.py` & `pilgram2-2.0.5/pilgram2/charmes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/clarendon.py` & `pilgram2-2.0.5/pilgram2/clarendon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/crema.py` & `pilgram2-2.0.5/pilgram2/crema.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/__init__.py` & `pilgram2-2.0.5/pilgram2/css/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/__init__.py` & `pilgram2-2.0.5/pilgram2/css/blending/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/alpha.py` & `pilgram2-2.0.5/pilgram2/css/blending/alpha.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/color.py` & `pilgram2-2.0.5/pilgram2/css/blending/color.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         The output image.
     """
 
     r, g, b = im2.split()  # Cs
     lum_cb = lum_im(im1)  # Lum(Cb)
     lum_cs = lum_im(im2)  # Lum(C) in SetLum
 
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "f((r, g, b), lum_cb, lum_cs)",
         f=_color_image_math,
         r=r,
         g=g,
         b=b,
         lum_cb=lum_cb,
         lum_cs=lum_cs,
```

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/color_burn.py` & `pilgram2-2.0.5/pilgram2/css/blending/color_burn.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,20 @@
     Returns:
         The output image.
     """
 
     return Image.merge(
         "RGB",
         [
-            ImageMath.eval("f(cb, cs)", f=_color_burn_image_math, cb=cb, cs=cs)
+            ImageMath.unsafe_eval(
+                "f(cb, cs)",
+                f=_color_burn_image_math,
+                cb=cb,
+                cs=cs,
+            )
             for cb, cs in zip(im1.split(), im2.split())
         ],
     )
 
 
 def color_burn(im1, im2):
     """Darkens the backdrop color to reflect the source color.
```

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/color_dodge.py` & `pilgram2-2.0.5/pilgram2/css/blending/color_dodge.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,20 @@
     Returns:
         The output image.
     """
 
     return Image.merge(
         "RGB",
         [
-            ImageMath.eval("f(cb, cs_inv)", f=_color_dodge_image_math, cb=cb, cs_inv=cs_inv)
+            ImageMath.unsafe_eval(
+                "f(cb, cs_inv)",
+                f=_color_dodge_image_math,
+                cb=cb,
+                cs_inv=cs_inv,
+            )
             for cb, cs_inv in zip(im1.split(), invert(im2).split())
         ],
     )
 
 
 def color_dodge(im1, im2):
     """Brightens the backdrop color to reflect the source color.
```

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/darken.py` & `pilgram2-2.0.5/pilgram2/css/blending/darken.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/difference.py` & `pilgram2-2.0.5/pilgram2/css/blending/difference.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/exclusion.py` & `pilgram2-2.0.5/pilgram2/css/blending/exclusion.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/hard_light.py` & `pilgram2-2.0.5/pilgram2/css/blending/hard_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/hue.py` & `pilgram2-2.0.5/pilgram2/css/blending/hue.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         The output image.
     """
 
     r1, g1, b1 = im1.split()  # Cb
     r2, g2, b2 = im2.split()  # Cs
     lum_cb = lum_im(im1)  # Lum(Cb)
 
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "f((r1, g1, b1), (r2, g2, b2), lum_cb)",
         f=_hue_image_math,
         r1=r1,
         g1=g1,
         b1=b1,
         r2=r2,
         g2=g2,
```

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/lighten.py` & `pilgram2-2.0.5/pilgram2/css/blending/lighten.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/multiply.py` & `pilgram2-2.0.5/pilgram2/css/blending/multiply.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/nonseparable.py` & `pilgram2-2.0.5/pilgram2/css/blending/nonseparable.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/normal.py` & `pilgram2-2.0.5/pilgram2/css/blending/normal.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/overlay.py` & `pilgram2-2.0.5/pilgram2/css/blending/overlay.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/screen.py` & `pilgram2-2.0.5/pilgram2/css/blending/screen.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/soft_light.py` & `pilgram2-2.0.5/pilgram2/css/blending/soft_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/__init__.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/helpers/__init__.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/helpers/alpha_support.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/helpers/alpha_support.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_alpha.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_color.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_color_burn.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_color_burn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_color_dodge.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_color_dodge.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_darken.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_darken.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_difference.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_exclusion.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_hard_light.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_hard_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_hue.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_lighten.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_lighten.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_multiply.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_multiply.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_nonseparable.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_nonseparable.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,31 +30,43 @@
     set_sat,
 )
 
 
 def test_min3():
     im = util.fill((1, 1), [0, 128, 255])
     r, g, b = im.split()
-    im_min = ImageMath.eval('convert(min3((r, g, b)), "L")', min3=_min3, r=r, g=g, b=b)
+    im_min = ImageMath.unsafe_eval(
+        'convert(min3((r, g, b)), "L")',
+        min3=_min3,
+        r=r,
+        g=g,
+        b=b,
+    )
 
     assert list(im_min.getdata()) == [0]
 
 
 def test_max3():
     im = util.fill((1, 1), [0, 128, 255])
     r, g, b = im.split()
-    im_max = ImageMath.eval('convert(max3((r, g, b)), "L")', max3=_max3, r=r, g=g, b=b)
+    im_max = ImageMath.unsafe_eval(
+        'convert(max3((r, g, b)), "L")',
+        max3=_max3,
+        r=r,
+        g=g,
+        b=b,
+    )
 
     assert list(im_max.getdata()) == [255]
 
 
 def test_clip_color():
     im = util.fill((1, 1), [0, 128, 255])
     r, g, b = im.split()
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "clip_color((float(r - 64), float(g), float(b + 64)))",
         clip_color=_clip_color,
         r=r,
         g=g,
         b=b,
     )
 
@@ -65,15 +77,21 @@
     ]
     assert [list(band.im.getdata()) for band in bands] == expected
 
 
 def test_lum():
     im = util.fill((1, 1), [0, 128, 255])
     r, g, b = im.split()
-    im_f = ImageMath.eval("lum((float(r), float(g), float(b)))", lum=lum, r=r, g=g, b=b)
+    im_f = ImageMath.unsafe_eval(
+        "lum((float(r), float(g), float(b)))",
+        lum=lum,
+        r=r,
+        g=g,
+        b=b,
+    )
     im_l = im_f.convert("L")
 
     assert list(im_f.getdata()) == [pytest.approx(103.57, 1e-6)]
     assert list(im_l.getdata()) == [floor(103.57)]
 
 
 def test_lum_im():
@@ -86,15 +104,15 @@
 def test_set_lum():
     im1 = util.fill((1, 1), [0, 128, 255])
     im2 = util.fill((1, 1), [128, 128, 128])
     r1, g1, b1 = im1.split()
     r2, g2, b2 = im2.split()
     c1 = "(float(r1), float(g1), float(b1))"
     c2 = "(float(r2), float(g2), float(b2))"
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         f"set_lum({c1}, lum({c2}))",
         set_lum=set_lum,
         lum=lum,
         r1=r1,
         g1=g1,
         b1=b1,
         r2=r2,
@@ -113,25 +131,31 @@
     expected2 = [(floor(41.13881001122631), floor(148.48874067225782), 255)]
     assert list(im_set_lum.getdata()) == expected2
 
 
 def test_sat():
     im = util.fill((1, 1), [80, 128, 200])
     r, g, b = im.split()
-    im_sat = ImageMath.eval('convert(sat((r, g, b)), "L")', sat=sat, r=r, g=g, b=b)
+    im_sat = ImageMath.unsafe_eval(
+        'convert(sat((r, g, b)), "L")',
+        sat=sat,
+        r=r,
+        g=g,
+        b=b,
+    )
 
     assert list(im_sat.getdata()) == [120]
 
 
 def test_set_sat_cmax_gt_cmin():
     im1 = util.fill((1, 1), [0, 128, 255])
     im2 = util.fill((1, 1), [64, 96, 128])  # sat = 64
     r1, g1, b1 = im1.split()
     r2, g2, b2 = im2.split()
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "set_sat((r1, g1, b1), sat((r2, g2, b2)))",
         set_sat=set_sat,
         sat=sat,
         r1=r1,
         g1=g1,
         b1=b1,
         r2=r2,
@@ -148,15 +172,15 @@
 
 
 def test_set_sat_cmax_eq_cmid_gt_cmin():
     im1 = util.fill((1, 1), [0, 128, 128])
     im2 = util.fill((1, 1), [64, 96, 128])  # sat = 64
     r1, g1, b1 = im1.split()
     r2, g2, b2 = im2.split()
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "set_sat((r1, g1, b1), sat((r2, g2, b2)))",
         set_sat=set_sat,
         sat=sat,
         r1=r1,
         g1=g1,
         b1=b1,
         r2=r2,
@@ -169,15 +193,15 @@
 
 
 def test_set_sat_cmax_eq_cmin():
     im1 = util.fill((1, 1), [128, 128, 128])
     im2 = util.fill((1, 1), [64, 96, 128])  # sat = 64
     r1, g1, b1 = im1.split()
     r2, g2, b2 = im2.split()
-    bands = ImageMath.eval(
+    bands = ImageMath.unsafe_eval(
         "set_sat((r1, g1, b1), sat((r2, g2, b2)))",
         set_sat=set_sat,
         sat=sat,
         r1=r1,
         g1=g1,
         b1=b1,
         r2=r2,
```

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_normal.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_overlay.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_screen.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/blending/tests/test_soft_light.py` & `pilgram2-2.0.5/pilgram2/css/blending/tests/test_soft_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/brightness.py` & `pilgram2-2.0.5/pilgram2/css/brightness.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/contrast.py` & `pilgram2-2.0.5/pilgram2/css/contrast.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/grayscale.py` & `pilgram2-2.0.5/pilgram2/css/grayscale.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/hue_rotate.py` & `pilgram2-2.0.5/pilgram2/css/hue_rotate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/saturate.py` & `pilgram2-2.0.5/pilgram2/css/saturate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/sepia.py` & `pilgram2-2.0.5/pilgram2/css/sepia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/__init__.py` & `pilgram2-2.0.5/pilgram2/css/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_brightness.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_brightness.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_contrast.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_contrast.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_grayscale.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_hue_rotate.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_hue_rotate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_saturate.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_saturate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/css/tests/test_sepia.py` & `pilgram2-2.0.5/pilgram2/css/tests/test_sepia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/dogpatch.py` & `pilgram2-2.0.5/pilgram2/dogpatch.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/earlybird.py` & `pilgram2-2.0.5/pilgram2/earlybird.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/gingham.py` & `pilgram2-2.0.5/pilgram2/gingham.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/ginza.py` & `pilgram2-2.0.5/pilgram2/ginza.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/hefe.py` & `pilgram2-2.0.5/pilgram2/hefe.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/helena.py` & `pilgram2-2.0.5/pilgram2/helena.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/hudson.py` & `pilgram2-2.0.5/pilgram2/hudson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/inkwell.py` & `pilgram2-2.0.5/pilgram2/inkwell.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/juno.py` & `pilgram2-2.0.5/pilgram2/juno.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/kelvin.py` & `pilgram2-2.0.5/pilgram2/kelvin.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/lark.py` & `pilgram2-2.0.5/pilgram2/lark.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/lofi.py` & `pilgram2-2.0.5/pilgram2/lofi.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/ludwig.py` & `pilgram2-2.0.5/pilgram2/ludwig.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/maven.py` & `pilgram2-2.0.5/pilgram2/maven.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/mayfair.py` & `pilgram2-2.0.5/pilgram2/mayfair.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/moon.py` & `pilgram2-2.0.5/pilgram2/moon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/nashville.py` & `pilgram2-2.0.5/pilgram2/nashville.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/perpetua.py` & `pilgram2-2.0.5/pilgram2/perpetua.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/poprocket.py` & `pilgram2-2.0.5/pilgram2/poprocket.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/reyes.py` & `pilgram2-2.0.5/pilgram2/reyes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/rise.py` & `pilgram2-2.0.5/pilgram2/rise.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/sierra.py` & `pilgram2-2.0.5/pilgram2/sierra.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/skyline.py` & `pilgram2-2.0.5/pilgram2/skyline.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/slumber.py` & `pilgram2-2.0.5/pilgram2/slumber.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/stinson.py` & `pilgram2-2.0.5/pilgram2/stinson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/sutro.py` & `pilgram2-2.0.5/pilgram2/sutro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/__init__.py` & `pilgram2-2.0.5/pilgram2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/assets/mtjimba.jpg` & `pilgram2-2.0.5/pilgram2/tests/assets/mtjimba.jpg`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_1977.py` & `pilgram2-2.0.5/pilgram2/tests/test_1977.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_aden.py` & `pilgram2-2.0.5/pilgram2/tests/test_aden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_amaro.py` & `pilgram2-2.0.5/pilgram2/tests/test_amaro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_ashby.py` & `pilgram2-2.0.5/pilgram2/tests/test_ashby.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_brannan.py` & `pilgram2-2.0.5/pilgram2/tests/test_brannan.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_brooklyn.py` & `pilgram2-2.0.5/pilgram2/tests/test_brooklyn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_charmes.py` & `pilgram2-2.0.5/pilgram2/tests/test_charmes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_clarendon.py` & `pilgram2-2.0.5/pilgram2/tests/test_clarendon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_crema.py` & `pilgram2-2.0.5/pilgram2/tests/test_crema.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_dogpatch.py` & `pilgram2-2.0.5/pilgram2/tests/test_dogpatch.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_earlybird.py` & `pilgram2-2.0.5/pilgram2/tests/test_earlybird.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_gingham.py` & `pilgram2-2.0.5/pilgram2/tests/test_gingham.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_ginza.py` & `pilgram2-2.0.5/pilgram2/tests/test_ginza.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_hefe.py` & `pilgram2-2.0.5/pilgram2/tests/test_hefe.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_helena.py` & `pilgram2-2.0.5/pilgram2/tests/test_helena.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_hudson.py` & `pilgram2-2.0.5/pilgram2/tests/test_hudson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_inkwell.py` & `pilgram2-2.0.5/pilgram2/tests/test_inkwell.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_juno.py` & `pilgram2-2.0.5/pilgram2/tests/test_juno.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_kelvin.py` & `pilgram2-2.0.5/pilgram2/tests/test_kelvin.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_lark.py` & `pilgram2-2.0.5/pilgram2/tests/test_lark.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_lofi.py` & `pilgram2-2.0.5/pilgram2/tests/test_lofi.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_ludwig.py` & `pilgram2-2.0.5/pilgram2/tests/test_ludwig.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_maven.py` & `pilgram2-2.0.5/pilgram2/tests/test_maven.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_mayfair.py` & `pilgram2-2.0.5/pilgram2/tests/test_mayfair.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_moon.py` & `pilgram2-2.0.5/pilgram2/tests/test_moon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_nashville.py` & `pilgram2-2.0.5/pilgram2/tests/test_nashville.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_perpetua.py` & `pilgram2-2.0.5/pilgram2/tests/test_perpetua.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_poprocket.py` & `pilgram2-2.0.5/pilgram2/tests/test_poprocket.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_reyes.py` & `pilgram2-2.0.5/pilgram2/tests/test_reyes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_rise.py` & `pilgram2-2.0.5/pilgram2/tests/test_rise.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_sierra.py` & `pilgram2-2.0.5/pilgram2/tests/test_sierra.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_skyline.py` & `pilgram2-2.0.5/pilgram2/tests/test_skyline.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_slumber.py` & `pilgram2-2.0.5/pilgram2/tests/test_slumber.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_stinson.py` & `pilgram2-2.0.5/pilgram2/tests/test_stinson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_sutro.py` & `pilgram2-2.0.5/pilgram2/tests/test_sutro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_toaster.py` & `pilgram2-2.0.5/pilgram2/tests/test_toaster.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_valencia.py` & `pilgram2-2.0.5/pilgram2/tests/test_valencia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_walden.py` & `pilgram2-2.0.5/pilgram2/tests/test_walden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_willow.py` & `pilgram2-2.0.5/pilgram2/tests/test_willow.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/tests/test_xpro2.py` & `pilgram2-2.0.5/pilgram2/tests/test_xpro2.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/toaster.py` & `pilgram2-2.0.5/pilgram2/toaster.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/__init__.py` & `pilgram2-2.0.5/pilgram2/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/add.py` & `pilgram2-2.0.5/pilgram2/util/add.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/apply_lut.py` & `pilgram2-2.0.5/pilgram2/util/apply_lut.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/clip.py` & `pilgram2-2.0.5/pilgram2/util/clip.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/fill.py` & `pilgram2-2.0.5/pilgram2/util/fill.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/invert.py` & `pilgram2-2.0.5/pilgram2/util/invert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/linear_gradient.py` & `pilgram2-2.0.5/pilgram2/util/linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/or_convert.py` & `pilgram2-2.0.5/pilgram2/util/or_convert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/radial_gradient.py` & `pilgram2-2.0.5/pilgram2/util/radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/subtract.py` & `pilgram2-2.0.5/pilgram2/util/subtract.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_add.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_apply_lut.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_apply_lut.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_clip.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_fill.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_invert.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_linear_gradient.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_or_convert.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_or_convert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_radial_gradient.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/util/tests/test_subtract.py` & `pilgram2-2.0.5/pilgram2/util/tests/test_subtract.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/valencia.py` & `pilgram2-2.0.5/pilgram2/valencia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/walden.py` & `pilgram2-2.0.5/pilgram2/walden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/willow.py` & `pilgram2-2.0.5/pilgram2/willow.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pilgram2/xpro2.py` & `pilgram2-2.0.5/pilgram2/xpro2.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.4/pyproject.toml` & `pilgram2-2.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,101 @@
-[project]
-name = "pilgram2"
-requires-python = ">=3.9,<3.13"
-version = "2.0.4"
-description = "library for instagram filters"
-authors = [
-  { name = "Michael G", email = "me@mgrl.de" },
-  { name = "Akiomi Kamakura", email = "akiomik@gmail.com" },
-]
-maintainers = [{ name = "Michael G", email = "me@mgrl.de" }]
-readme = "README.md"
-license = { file = "LICENSE" }
-classifiers = [
-  "License :: OSI Approved :: Apache Software License",
-  "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Topic :: Multimedia :: Graphics",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-]
-keywords = [
-  "pillow",
-  "instagram",
-  "instagram-filters",
-  "css-filters",
-  "image-blending",
-  "blend-modes",
-  "image-processing",
-  "data-augmentation",
-]
-
-[tool.poetry.urls]
-Homepage = "https://github.com/mgrl/pilgram2"
-Repository = "https://github.com/mgrl/pilgram2"
-"Bug Tracker" = "https://github.com/mgrl/pilgram2/issues"
-
-[tool.poetry]
-name = "pilgram2"
-version = "2.0.4"
-description = "library for instagram filters"
-authors = ["Michael G <me@mgrl.de>", "Akiomi Kamakura <akiomik@gmail.com>"]
-license = "Apache License 2.0"
-readme = "README.md"
-classifiers = [
-  "License :: OSI Approved :: Apache Software License",
-  "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Topic :: Multimedia :: Graphics",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-]
-keywords = [
-  "pillow",
-  "instagram",
-  "instagram-filters",
-  "css-filters",
-  "image-blending",
-  "blend-modes",
-  "image-processing",
-  "data-augmentation",
-]
-
-[tool.poetry.dependencies]
-python = ">=3.9,<3.13"
-numpy = "^1.26.1"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-Pillow = ">=9.3,<11.0"
-pytest-benchmark = "^4.0.0"
-pytest-mock = "^3.10.0"
-numpy = "^1.26.1"
-ruff = ">=0.0.270,<0.1.7"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.black]
-line-length = 120
-
-[tool.ruff]
-line-length = 120
-select = [
-  "E",  # pycodestyle
-  "W",  # pycodestyle
-  "F",  # pyflakes
-  "B",  # bugbear
-  "UP", # pyupgrade
-  "I",  # isort
-]
-
-[tool.pytest.ini_options]
-addopts = "-v --cov=pilgram2 --benchmark-skip"
-
-[tool.coverage.run]
-omit = ["*/tests/*"]
-
-[tool.coverage.report]
-show_missing = true
+[project]
+name = "pilgram2"
+requires-python = ">=3.9,<3.13"
+version = "2.0.5"
+description = "library for instagram filters"
+authors = [
+    { name = "Michael G", email = "me@mgrl.de" },
+    { name = "Akiomi Kamakura", email = "akiomik@gmail.com" },
+]
+maintainers = [
+    { name = "Michael G", email = "me@mgrl.de" },
+]
+readme = "README.md"
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Multimedia :: Graphics",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+keywords = [
+    "pillow",
+    "instagram",
+    "instagram-filters",
+    "css-filters",
+    "image-blending",
+    "blend-modes",
+    "image-processing",
+    "data-augmentation",
+]
+dependencies = [
+    "numpy>=1.26.1",
+]
+
+[project.license]
+file = "LICENSE"
+
+[project.urls]
+Homepage = "https://github.com/mgineer85/pilgram2"
+Repository = "https://github.com/mgineer85/pilgram2"
+"Bug Tracker" = "https://github.com/mgineer85/pilgram2/issues"
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.ruff]
+line-length = 120
+
+[tool.ruff.lint]
+select = [
+    "E",
+    "W",
+    "F",
+    "B",
+    "UP",
+    "I",
+]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
+[tool.pytest.ini_options]
+addopts = "-v --cov=pilgram2 --benchmark-skip"
+
+[tool.coverage.run]
+omit = [
+    "*/tests/*",
+]
+
+[tool.coverage.report]
+show_missing = true
+
+[tool.pdm.dev-dependencies]
+test = [
+    "pytest>=8.1.0",
+    "pytest-cov>=5.0.0",
+    "pillow>=10.0.0",
+    "pytest-benchmark>=4.0.0",
+    "pytest-mock>=3.10.0",
+]
+lint = [
+    "ruff>=0.3.5",
+]
+
+[tool.pdm.build]
+includes = [
+    "./pilgram2",
+]
+
+[tool.pdm.scripts]
+lint = "ruff check ."
+format = "ruff format ."
+test = "pytest --cov-report=term --cov-report=xml:coverage.xml"
+benchmark = "pytest --benchmark-only --benchmark-max-time=5 --benchmark-columns='mean,stddev,min,max'"
```

### Comparing `pilgram2-2.0.4/README.md` & `pilgram2-2.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pilgram2
 
 [![PyPI](https://img.shields.io/pypi/v/pilgram2.svg)](https://python.org/pypi/pilgram2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pilgram2.svg)](https://python.org/pypi/pilgram2)
-[![Python CI](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml/badge.svg)](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml)
-[![codecov](https://codecov.io/gh/mgrl/pilgram2/branch/main/graph/badge.svg)](https://codecov.io/gh/mgrl/pilgram2)
+[![Python CI](https://github.com/mgineer85/pilgram2/actions/workflows/ci.yml/badge.svg)](https://github.com/mgineer85/pilgram2/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/mgineer85/pilgram2/branch/main/graph/badge.svg)](https://codecov.io/gh/mgineer85/pilgram2)
 
 A python library for instagram filters.
 
-![screenshot](https://raw.githubusercontent.com/mgrl/pilgram2/main/screenshots/screenshot.png)
+![screenshot](https://raw.githubusercontent.com/mgineer85/pilgram2/main/screenshots/screenshot.png)
 
 The filter implementations are inspired by [CSSgram](https://una.im/CSSgram/).
 Pilgram2 was forked from [pilgram](https://github.com/akiomik/pilgram).
 Pilgram2 features more filter and supports non-quadratic images.
 
 ## Requirements
 
-- Python >= 3.8
+- Python >= 3.9
 - [Pillow](https://pillow.readthedocs.io/en/stable/) or [pillow-simd](https://github.com/uploadcare/pillow-simd)
 - [NumPy](https://numpy.org)
 
 ## Install
 
 ```sh
 pip install pillow # or pip install pillow-simd
```

