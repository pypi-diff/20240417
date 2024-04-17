# Comparing `tmp/capypdf-0.8.0.tar.gz` & `tmp/capypdf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capypdf-0.8.0.tar", last modified: Sun Jan 21 08:58:03 2024, max compression
+gzip compressed data, was "capypdf-0.9.0.tar", last modified: Mon Mar  4 16:35:31 2024, max compression
```

## Comparing `capypdf-0.8.0.tar` & `capypdf-0.9.0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
--rw-rw-rw-   0        0        0      348 2024-01-17 16:54:24.000000 capypdf-0.8.0/.clang-format
--rw-rw-rw-   0        0        0      808 2024-01-17 16:54:24.000000 capypdf-0.8.0/.github/workflows/linuxtests.yml
--rw-rw-rw-   0        0        0      101 2024-01-17 16:54:24.000000 capypdf-0.8.0/.gitignore
--rw-rw-rw-   0        0        0    11358 2024-01-17 16:54:24.000000 capypdf-0.8.0/COPYING
--rw-rw-rw-   0        0        0      175 2024-01-17 16:54:24.000000 capypdf-0.8.0/compilefuzz.sh
--rw-rw-rw-   0        0        0   236668 2024-01-17 16:54:24.000000 capypdf-0.8.0/icc/FOGRA29L.icc
--rw-rw-rw-   0        0        0   236680 2024-01-17 16:54:24.000000 capypdf-0.8.0/icc/FOGRA30L.icc
--rw-rw-rw-   0        0        0      430 2024-01-17 16:54:24.000000 capypdf-0.8.0/icc/readme.md
--rw-rw-rw-   0        0        0    10810 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/1bit_alpha.png
--rw-rw-rw-   0        0        0     1650 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/1bit_noalpha.png
--rw-rw-rw-   0        0        0    38795 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/capylogo.svg
--rw-rw-rw-   0        0        0    24990 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/capylogo_web.png
--rw-rw-rw-   0        0        0    13448 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/cmyk_tiff.tif
--rw-rw-rw-   0        0        0    38408 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/comic-colors.png
--rw-rw-rw-   0        0        0     3260 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/comic-lines.png
--rw-rw-rw-   0        0        0     3189 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/comic-richblack.png
--rw-rw-rw-   0        0        0   118339 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/flame_gradient.png
--rw-rw-rw-   0        0        0  6039784 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/fogra_cmyk.tif
--rw-rw-rw-   0        0        0    57042 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/gray_alpha.png
--rw-rw-rw-   0        0        0   267304 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/object_gradient.png
--rw-rw-rw-   0        0        0   139485 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/rgb_tiff.tif
--rw-rw-rw-   0        0        0    28468 2024-01-17 16:54:24.000000 capypdf-0.8.0/images/simple.jpg
--rw-rw-rw-   0        0        0    32517 2024-01-17 16:54:24.000000 capypdf-0.8.0/include/capypdf.h.in
--rw-rw-rw-   0        0        0      167 2024-01-17 16:54:24.000000 capypdf-0.8.0/include/meson.build
--rw-rw-rw-   0        0        0      985 2024-01-17 16:54:24.000000 capypdf-0.8.0/meson.build
--rw-rw-rw-   0        0        0       87 2024-01-17 16:54:24.000000 capypdf-0.8.0/meson.options
--rw-rw-rw-   0        0        0      866 2024-01-17 16:54:24.000000 capypdf-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0    45016 2024-01-17 16:54:24.000000 capypdf-0.8.0/python/capypdf.py
--rw-rw-rw-   0        0        0       67 2024-01-17 16:54:24.000000 capypdf-0.8.0/python/meson.build
--rw-rw-rw-   0        0        0     1369 2024-01-17 16:54:24.000000 capypdf-0.8.0/readme.md
--rw-rw-rw-   0        0        0     2579 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/errorhandling.cpp
--rw-rw-rw-   0        0        0     4982 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/errorhandling.hpp
--rw-rw-rw-   0        0        0     3282 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fembedtest.cpp
--rw-rw-rw-   0        0        0      437 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fontfuzz.cpp
--rw-rw-rw-   0        0        0     7916 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fontgen.cpp
--rw-rw-rw-   0        0        0     5658 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fontsubsetter.cpp
--rw-rw-rw-   0        0        0     1711 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fontsubsetter.hpp
--rw-rw-rw-   0        0        0     1007 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/fonttester.cpp
--rw-rw-rw-   0        0        0     8342 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/formtest.cpp
--rw-rw-rw-   0        0        0     1792 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/formxobj.cpp
--rw-rw-rw-   0        0        0    31759 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/ft_subsetter.cpp
--rw-rw-rw-   0        0        0     4818 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/ft_subsetter.hpp
--rw-rw-rw-   0        0        0    12985 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/imagefileops.cpp
--rw-rw-rw-   0        0        0      444 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/imagefileops.hpp
--rw-rw-rw-   0        0        0     1505 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/labtest.cpp
--rw-rw-rw-   0        0        0    11052 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/loremipsum.cpp
--rw-rw-rw-   0        0        0     1969 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/meson.build
--rw-rw-rw-   0        0        0    50367 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfcapi.cpp
--rw-rw-rw-   0        0        0     7438 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfcolorconverter.cpp
--rw-rw-rw-   0        0        0     2197 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfcolorconverter.hpp
--rw-rw-rw-   0        0        0     2403 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfcommon.cpp
--rw-rw-rw-   0        0        0    12740 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfcommon.hpp
--rw-rw-rw-   0        0        0    73853 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfdocument.cpp
--rw-rw-rw-   0        0        0    15536 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfdocument.hpp
--rw-rw-rw-   0        0        0    38503 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfdrawcontext.cpp
--rw-rw-rw-   0        0        0    12419 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfdrawcontext.hpp
--rw-rw-rw-   0        0        0     7836 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfgen.cpp
--rw-rw-rw-   0        0        0     6557 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfgen.hpp
--rw-rw-rw-   0        0        0    10721 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfparser.cpp
--rw-rw-rw-   0        0        0     4257 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfparser.hpp
--rw-rw-rw-   0        0        0     4108 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdftext.hpp
--rw-rw-rw-   0        0        0    18689 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/pdfviewer.cpp
--rw-rw-rw-   0        0        0     1195 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/subtype.cpp
--rw-rw-rw-   0        0        0     8603 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/utils.cpp
--rw-rw-rw-   0        0        0     1157 2024-01-17 16:54:24.000000 capypdf-0.8.0/src/utils.hpp
--rw-rw-rw-   0        0        0       84 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/.gitignore
--rw-rw-rw-   0        0        0      560 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/fmt.wrap
--rw-rw-rw-   0        0        0      453 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/freetype2.wrap
--rw-rw-rw-   0        0        0      406 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/lcms2.wrap
--rw-rw-rw-   0        0        0      674 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/libjpeg-turbo.wrap
--rw-rw-rw-   0        0        0      589 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/libpng.wrap
--rw-rw-rw-   0        0        0      580 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/libtiff.wrap
--rw-rw-rw-   0        0        0      535 2024-01-17 16:54:24.000000 capypdf-0.8.0/subprojects/zlib.wrap
--rw-rw-rw-   0        0        0    42259 2024-01-17 16:54:24.000000 capypdf-0.8.0/test/capypdftests.py
--rw-rw-rw-   0        0        0      757 2024-01-17 16:54:24.000000 capypdf-0.8.0/test/ctest.c
--rw-rw-rw-   0        0        0      178 2024-01-17 16:54:24.000000 capypdf-0.8.0/test/meson.build
--rw-rw-rw-   0        0        0      941 2024-01-17 16:54:24.000000 capypdf-0.8.0/test/syntaxchecks.py
--rw-rw-rw-   0        0        0     1063 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_annotate.png
--rw-rw-rw-   0        0        0    42992 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_blendmodes.png
--rw-rw-rw-   0        0        0     1187 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_colorpattern.png
--rw-rw-rw-   0        0        0     3309 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_gstate.png
--rw-rw-rw-   0        0        0     3072 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_icccolor.png
--rw-rw-rw-   0        0        0    22459 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_image.png
--rw-rw-rw-   0        0        0     2003 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_imagemask.png
--rw-rw-rw-   0        0        0     3675 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_linestyles.png
--rw-rw-rw-   0        0        0     4941 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_path.png
--rw-rw-rw-   0        0        0      691 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_printersmark.png
--rw-rw-rw-   0        0        0     3066 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_rasterimage.png
--rw-rw-rw-   0        0        0      726 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_separation.png
--rw-rw-rw-   0        0        0    13473 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_shading_cmyk.png
--rw-rw-rw-   0        0        0     6367 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_shading_gray.png
--rw-rw-rw-   0        0        0     7641 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_shading_rgb.png
--rw-rw-rw-   0        0        0     4777 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_simple.png
--rw-rw-rw-   0        0        0     1964 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_tagged.png
--rw-rw-rw-   0        0        0     4072 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_text.png
--rw-rw-rw-   0        0        0     3329 2024-01-17 16:54:24.000000 capypdf-0.8.0/testoutput/python_textobj.png
--rw-rw-rw-   0        0        0     8494 2024-01-17 16:54:24.000000 capypdf-0.8.0/tools/presentationtool.py
--rw-rw-rw-   0        0        0     8655 2024-01-17 16:54:24.000000 capypdf-0.8.0/tools/x3gen.py
--rw-r--r--   0        0        0    14871 2024-01-21 08:58:06.104538 capypdf-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-03-04 16:29:58.000000 capypdf-0.9.0/.clang-format
+-rw-rw-rw-   0        0        0      808 2024-03-04 16:29:58.000000 capypdf-0.9.0/.github/workflows/linuxtests.yml
+-rw-rw-rw-   0        0        0      101 2024-03-04 16:29:58.000000 capypdf-0.9.0/.gitignore
+-rw-rw-rw-   0        0        0    11358 2024-03-04 16:29:58.000000 capypdf-0.9.0/COPYING
+-rw-rw-rw-   0        0        0      175 2024-03-04 16:29:58.000000 capypdf-0.9.0/compilefuzz.sh
+-rw-rw-rw-   0        0        0   236668 2024-03-04 16:29:58.000000 capypdf-0.9.0/icc/FOGRA29L.icc
+-rw-rw-rw-   0        0        0   236680 2024-03-04 16:29:58.000000 capypdf-0.9.0/icc/FOGRA30L.icc
+-rw-rw-rw-   0        0        0      430 2024-03-04 16:29:58.000000 capypdf-0.9.0/icc/readme.md
+-rw-rw-rw-   0        0        0    10810 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/1bit_alpha.png
+-rw-rw-rw-   0        0        0     1650 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/1bit_noalpha.png
+-rw-rw-rw-   0        0        0    39196 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/capylogo.svg
+-rw-rw-rw-   0        0        0    24990 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/capylogo_web.png
+-rw-rw-rw-   0        0        0    13448 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/cmyk_tiff.tif
+-rw-rw-rw-   0        0        0    38408 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/comic-colors.png
+-rw-rw-rw-   0        0        0     3260 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/comic-lines.png
+-rw-rw-rw-   0        0        0     3189 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/comic-richblack.png
+-rw-rw-rw-   0        0        0   118339 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/flame_gradient.png
+-rw-rw-rw-   0        0        0  6039784 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/fogra_cmyk.tif
+-rw-rw-rw-   0        0        0    57042 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/gray_alpha.png
+-rw-rw-rw-   0        0        0   267304 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/object_gradient.png
+-rw-rw-rw-   0        0        0   139485 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/rgb_tiff.tif
+-rw-rw-rw-   0        0        0    28468 2024-03-04 16:29:58.000000 capypdf-0.9.0/images/simple.jpg
+-rw-rw-rw-   0        0        0    37068 2024-03-04 16:29:58.000000 capypdf-0.9.0/include/capypdf.h.in
+-rw-rw-rw-   0        0        0      167 2024-03-04 16:29:58.000000 capypdf-0.9.0/include/meson.build
+-rw-rw-rw-   0        0        0      985 2024-03-04 16:29:58.000000 capypdf-0.9.0/meson.build
+-rw-rw-rw-   0        0        0       87 2024-03-04 16:29:58.000000 capypdf-0.9.0/meson.options
+-rw-rw-rw-   0        0        0      866 2024-03-04 16:29:58.000000 capypdf-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0    48750 2024-03-04 16:29:58.000000 capypdf-0.9.0/python/capypdf.py
+-rw-rw-rw-   0        0        0       67 2024-03-04 16:29:58.000000 capypdf-0.9.0/python/meson.build
+-rw-rw-rw-   0        0        0     1369 2024-03-04 16:29:58.000000 capypdf-0.9.0/readme.md
+-rw-rw-rw-   0        0        0     2663 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/errorhandling.cpp
+-rw-rw-rw-   0        0        0     5025 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/errorhandling.hpp
+-rw-rw-rw-   0        0        0     3282 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fembedtest.cpp
+-rw-rw-rw-   0        0        0      437 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fontfuzz.cpp
+-rw-rw-rw-   0        0        0     7916 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fontgen.cpp
+-rw-rw-rw-   0        0        0     5658 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fontsubsetter.cpp
+-rw-rw-rw-   0        0        0     1711 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fontsubsetter.hpp
+-rw-rw-rw-   0        0        0     1007 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/fonttester.cpp
+-rw-rw-rw-   0        0        0     8342 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/formtest.cpp
+-rw-rw-rw-   0        0        0     1792 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/formxobj.cpp
+-rw-rw-rw-   0        0        0    31759 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/ft_subsetter.cpp
+-rw-rw-rw-   0        0        0     4818 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/ft_subsetter.hpp
+-rw-rw-rw-   0        0        0    12985 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/imagefileops.cpp
+-rw-rw-rw-   0        0        0      444 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/imagefileops.hpp
+-rw-rw-rw-   0        0        0     1505 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/labtest.cpp
+-rw-rw-rw-   0        0        0    10722 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/loremipsum.cpp
+-rw-rw-rw-   0        0        0     1999 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/meson.build
+-rw-rw-rw-   0        0        0      241 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pch/capypch.hpp
+-rw-rw-rw-   0        0        0    54038 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfcapi.cpp
+-rw-rw-rw-   0        0        0     7437 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfcolorconverter.cpp
+-rw-rw-rw-   0        0        0     2197 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfcolorconverter.hpp
+-rw-rw-rw-   0        0        0     3109 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfcommon.cpp
+-rw-rw-rw-   0        0        0    12837 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfcommon.hpp
+-rw-rw-rw-   0        0        0    75954 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfdocument.cpp
+-rw-rw-rw-   0        0        0    16233 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfdocument.hpp
+-rw-rw-rw-   0        0        0    39357 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfdrawcontext.cpp
+-rw-rw-rw-   0        0        0    12824 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfdrawcontext.hpp
+-rw-rw-rw-   0        0        0     7918 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfgen.cpp
+-rw-rw-rw-   0        0        0     6959 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfgen.hpp
+-rw-rw-rw-   0        0        0    11294 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfparser.cpp
+-rw-rw-rw-   0        0        0     4368 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfparser.hpp
+-rw-rw-rw-   0        0        0     4055 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdftext.hpp
+-rw-rw-rw-   0        0        0    18692 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/pdfviewer.cpp
+-rw-rw-rw-   0        0        0     1195 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/subtype.cpp
+-rw-rw-rw-   0        0        0     8649 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/utils.cpp
+-rw-rw-rw-   0        0        0     1180 2024-03-04 16:29:58.000000 capypdf-0.9.0/src/utils.hpp
+-rw-rw-rw-   0        0        0       84 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/.gitignore
+-rw-rw-rw-   0        0        0      560 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/fmt.wrap
+-rw-rw-rw-   0        0        0      453 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/freetype2.wrap
+-rw-rw-rw-   0        0        0      406 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/lcms2.wrap
+-rw-rw-rw-   0        0        0      686 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/libjpeg-turbo.wrap
+-rw-rw-rw-   0        0        0      589 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/libpng.wrap
+-rw-rw-rw-   0        0        0      580 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/libtiff.wrap
+-rw-rw-rw-   0        0        0      551 2024-03-04 16:29:58.000000 capypdf-0.9.0/subprojects/zlib.wrap
+-rw-rw-rw-   0        0        0    44138 2024-03-04 16:29:58.000000 capypdf-0.9.0/test/capypdftests.py
+-rw-rw-rw-   0        0        0      757 2024-03-04 16:29:58.000000 capypdf-0.9.0/test/ctest.c
+-rw-rw-rw-   0        0        0      178 2024-03-04 16:29:58.000000 capypdf-0.9.0/test/meson.build
+-rw-rw-rw-   0        0        0      941 2024-03-04 16:29:58.000000 capypdf-0.9.0/test/syntaxchecks.py
+-rw-rw-rw-   0        0        0     1063 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_annotate.png
+-rw-rw-rw-   0        0        0    42992 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_blendmodes.png
+-rw-rw-rw-   0        0        0     1187 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_colorpattern.png
+-rw-rw-rw-   0        0        0     1504 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_customroles.png
+-rw-rw-rw-   0        0        0     3309 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_gstate.png
+-rw-rw-rw-   0        0        0     3072 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_icccolor.png
+-rw-rw-rw-   0        0        0    22459 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_image.png
+-rw-rw-rw-   0        0        0     2003 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_imagemask.png
+-rw-rw-rw-   0        0        0     3675 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_linestyles.png
+-rw-rw-rw-   0        0        0     4941 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_path.png
+-rw-rw-rw-   0        0        0      725 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_printersmark.png
+-rw-rw-rw-   0        0        0     3066 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_rasterimage.png
+-rw-rw-rw-   0        0        0      726 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_separation.png
+-rw-rw-rw-   0        0        0    13473 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_shading_cmyk.png
+-rw-rw-rw-   0        0        0     6367 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_shading_gray.png
+-rw-rw-rw-   0        0        0     7641 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_shading_rgb.png
+-rw-rw-rw-   0        0        0     4777 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_simple.png
+-rw-rw-rw-   0        0        0     1413 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_tagged.png
+-rw-rw-rw-   0        0        0     4072 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_text.png
+-rw-rw-rw-   0        0        0     3329 2024-03-04 16:29:58.000000 capypdf-0.9.0/testoutput/python_textobj.png
+-rw-rw-rw-   0        0        0     8494 2024-03-04 16:29:58.000000 capypdf-0.9.0/tools/presentationtool.py
+-rw-rw-rw-   0        0        0     8655 2024-03-04 16:29:58.000000 capypdf-0.9.0/tools/x3gen.py
+-rw-r--r--   0        0        0    14871 2024-03-04 16:35:32.480157 capypdf-0.9.0/PKG-INFO
```

### Comparing `capypdf-0.8.0/.github/workflows/linuxtests.yml` & `capypdf-0.9.0/.github/workflows/linuxtests.yml`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/COPYING` & `capypdf-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/icc/FOGRA29L.icc` & `capypdf-0.9.0/icc/FOGRA29L.icc`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/icc/FOGRA30L.icc` & `capypdf-0.9.0/icc/FOGRA30L.icc`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/1bit_alpha.png` & `capypdf-0.9.0/images/1bit_alpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/1bit_noalpha.png` & `capypdf-0.9.0/images/1bit_noalpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/capylogo.svg` & `capypdf-0.9.0/images/capylogo.svg`

 * *Files 1% similar despite different names*

```diff
@@ -49,2377 +49,2402 @@
 00000300: 7262 6f61 7264 3d22 3022 0a20 2020 2020  rboard="0".     
 00000310: 696e 6b73 6361 7065 3a64 6573 6b63 6f6c  inkscape:deskcol
 00000320: 6f72 3d22 2364 3164 3164 3122 0a20 2020  or="#d1d1d1".   
 00000330: 2020 696e 6b73 6361 7065 3a64 6f63 756d    inkscape:docum
 00000340: 656e 742d 756e 6974 733d 226d 6d22 0a20  ent-units="mm". 
 00000350: 2020 2020 7368 6f77 6772 6964 3d22 6661      showgrid="fa
 00000360: 6c73 6522 0a20 2020 2020 696e 6b73 6361  lse".     inksca
-00000370: 7065 3a7a 6f6f 6d3d 2232 2e38 3238 3432  pe:zoom="2.82842
-00000380: 3732 220a 2020 2020 2069 6e6b 7363 6170  72".     inkscap
-00000390: 653a 6378 3d22 3336 372e 3639 3535 3222  e:cx="367.69552"
+00000370: 7065 3a7a 6f6f 6d3d 2232 2e30 3030 3030  pe:zoom="2.00000
+00000380: 3031 220a 2020 2020 2069 6e6b 7363 6170  01".     inkscap
+00000390: 653a 6378 3d22 3434 382e 3939 3939 3922  e:cx="448.99999"
 000003a0: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
-000003b0: 793d 2233 3139 2e32 3538 3722 0a20 2020  y="319.2587".   
-000003c0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-000003d0: 772d 7769 6474 683d 2233 3834 3022 0a20  w-width="3840". 
-000003e0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-000003f0: 646f 772d 6865 6967 6874 3d22 3230 3738  dow-height="2078
-00000400: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000410: 7769 6e64 6f77 2d78 3d22 3022 0a20 2020  window-x="0".   
-00000420: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000430: 772d 793d 2230 220a 2020 2020 2069 6e6b  w-y="0".     ink
-00000440: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
-00000450: 696d 697a 6564 3d22 3122 0a20 2020 2020  imized="1".     
-00000460: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
-00000470: 2d6c 6179 6572 3d22 6c61 7965 7231 220a  -layer="layer1".
-00000480: 2020 2020 2073 686f 7767 7569 6465 733d       showguides=
-00000490: 2274 7275 6522 202f 3e0a 2020 3c64 6566  "true" />.  <def
-000004a0: 730a 2020 2020 2069 643d 2264 6566 7332  s.     id="defs2
-000004b0: 223e 0a20 2020 203c 696e 6b73 6361 7065  ">.    <inkscape
-000004c0: 3a70 6174 682d 6566 6665 6374 0a20 2020  :path-effect.   
-000004d0: 2020 2020 6566 6665 6374 3d22 7461 7065      effect="tape
-000004e0: 725f 7374 726f 6b65 220a 2020 2020 2020  r_stroke".      
-000004f0: 2069 643d 2270 6174 682d 6566 6665 6374   id="path-effect
-00000500: 3422 0a20 2020 2020 2020 6973 5f76 6973  4".       is_vis
-00000510: 6962 6c65 3d22 7472 7565 220a 2020 2020  ible="true".    
-00000520: 2020 206c 7065 7665 7273 696f 6e3d 2231     lpeversion="1
-00000530: 220a 2020 2020 2020 2073 7472 6f6b 655f  ".       stroke_
-00000540: 7769 6474 683d 2234 220a 2020 2020 2020  width="4".      
-00000550: 2073 7562 7061 7468 3d22 3122 0a20 2020   subpath="1".   
-00000560: 2020 2020 6174 7461 6368 5f73 7461 7274      attach_start
-00000570: 3d22 302e 3536 3336 3638 3434 220a 2020  ="0.56366844".  
-00000580: 2020 2020 2065 6e64 5f6f 6666 7365 743d       end_offset=
-00000590: 2230 2e36 3234 3131 3630 3522 0a20 2020  "0.62411605".   
-000005a0: 2020 2020 7374 6172 745f 736d 6f6f 7468      start_smooth
-000005b0: 696e 673d 2230 2e34 220a 2020 2020 2020  ing="0.4".      
-000005c0: 2065 6e64 5f73 6d6f 6f74 6869 6e67 3d22   end_smoothing="
-000005d0: 302e 3522 0a20 2020 2020 2020 6a6f 696e  0.5".       join
-000005e0: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
-000005f0: 6564 220a 2020 2020 2020 2073 7461 7274  ed".       start
-00000600: 5f73 6861 7065 3d22 6365 6e74 6572 220a  _shape="center".
-00000610: 2020 2020 2020 2065 6e64 5f73 6861 7065         end_shape
-00000620: 3d22 6365 6e74 6572 220a 2020 2020 2020  ="center".      
-00000630: 206d 6974 6572 5f6c 696d 6974 3d22 3130   miter_limit="10
-00000640: 3022 202f 3e0a 2020 3c2f 6465 6673 3e0a  0" />.  </defs>.
-00000650: 2020 3c67 0a20 2020 2020 696e 6b73 6361    <g.     inksca
-00000660: 7065 3a6c 6162 656c 3d22 4c61 7965 7220  pe:label="Layer 
-00000670: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
-00000680: 3a67 726f 7570 6d6f 6465 3d22 6c61 7965  :groupmode="laye
-00000690: 7222 0a20 2020 2020 6964 3d22 6c61 7965  r".     id="laye
-000006a0: 7231 223e 0a20 2020 203c 7573 650a 2020  r1">.    <use.  
-000006b0: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
-000006c0: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
-000006d0: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
-000006e0: 3839 3835 2d38 220a 2020 2020 2020 2069  8985-8".       i
-000006f0: 643d 2275 7365 3236 3031 3622 0a20 2020  d="use26016".   
-00000700: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-00000710: 7261 6e73 6c61 7465 2832 2e33 3331 3830  ranslate(2.33180
-00000720: 3438 2c33 302e 3133 3335 3735 2922 202f  48,30.133575)" /
-00000730: 3e0a 2020 2020 3c75 7365 0a20 2020 2020  >.    <use.     
-00000740: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
-00000750: 3d22 3022 0a20 2020 2020 2020 786c 696e  ="0".       xlin
-00000760: 6b3a 6872 6566 3d22 2370 6174 6838 3938  k:href="#path898
-00000770: 352d 3822 0a20 2020 2020 2020 6964 3d22  5-8".       id="
-00000780: 7573 6532 3630 3130 220a 2020 2020 2020  use26010".      
-00000790: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-000007a0: 736c 6174 6528 3131 2e31 3033 3230 382c  slate(11.103208,
-000007b0: 3234 2e31 3237 3132 2922 202f 3e0a 2020  24.12712)" />.  
-000007c0: 2020 3c75 7365 0a20 2020 2020 2020 783d    <use.       x=
-000007d0: 2230 220a 2020 2020 2020 2079 3d22 3022  "0".       y="0"
-000007e0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-000007f0: 6566 3d22 2370 6174 6838 3938 352d 3822  ef="#path8985-8"
-00000800: 0a20 2020 2020 2020 6964 3d22 7573 6532  .       id="use2
-00000810: 3630 3038 220a 2020 2020 2020 2074 7261  6008".       tra
-00000820: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00000830: 6528 372e 3037 3135 3432 382c 3231 2e36  e(7.0715428,21.6
-00000840: 3831 3936 3129 2220 2f3e 0a20 2020 203c  81961)" />.    <
-00000850: 7573 650a 2020 2020 2020 2078 3d22 3022  use.       x="0"
-00000860: 0a20 2020 2020 2020 793d 2230 220a 2020  .       y="0".  
-00000870: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-00000880: 2223 7061 7468 3839 3835 220a 2020 2020  "#path8985".    
-00000890: 2020 2069 643d 2275 7365 3138 3830 3922     id="use18809"
-000008a0: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-000008b0: 6d3d 2274 7261 6e73 6c61 7465 2831 302e  m="translate(10.
-000008c0: 3339 3037 3231 2c33 352e 3937 3733 3237  390721,35.977327
-000008d0: 2922 202f 3e0a 2020 2020 3c75 7365 0a20  )" />.    <use. 
-000008e0: 2020 2020 2020 783d 2230 220a 2020 2020        x="0".    
-000008f0: 2020 2079 3d22 3022 0a20 2020 2020 2020     y="0".       
-00000900: 786c 696e 6b3a 6872 6566 3d22 2370 6174  xlink:href="#pat
-00000910: 6838 3938 3522 0a20 2020 2020 2020 6964  h8985".       id
-00000920: 3d22 7573 6531 3838 3037 220a 2020 2020  ="use18807".    
-00000930: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00000940: 616e 736c 6174 6528 3137 2e33 3435 3730  anslate(17.34570
-00000950: 362c 3334 2e37 3837 3638 3729 2220 2f3e  6,34.787687)" />
-00000960: 0a20 2020 203c 7573 650a 2020 2020 2020  .    <use.      
-00000970: 2078 3d22 3022 0a20 2020 2020 2020 793d   x="0".       y=
-00000980: 2230 220a 2020 2020 2020 2078 6c69 6e6b  "0".       xlink
-00000990: 3a68 7265 663d 2223 7061 7468 3839 3835  :href="#path8985
-000009a0: 220a 2020 2020 2020 2069 643d 2275 7365  ".       id="use
-000009b0: 3138 3830 3522 0a20 2020 2020 2020 7472  18805".       tr
-000009c0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-000009d0: 7465 2831 302e 3830 3132 3038 2c31 362e  te(10.801208,16.
-000009e0: 3134 3336 3838 2922 202f 3e0a 2020 2020  143688)" />.    
-000009f0: 3c75 7365 0a20 2020 2020 2020 783d 2230  <use.       x="0
-00000a00: 220a 2020 2020 2020 2079 3d22 3022 0a20  ".       y="0". 
-00000a10: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-00000a20: 3d22 2370 6174 6838 3938 3522 0a20 2020  ="#path8985".   
-00000a30: 2020 2020 6964 3d22 7573 6531 3838 3033      id="use18803
-00000a40: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
-00000a50: 726d 3d22 7472 616e 736c 6174 6528 3137  rm="translate(17
-00000a60: 2e36 3533 3337 372c 3137 2e38 3835 3834  .653377,17.88584
-00000a70: 3629 2220 2f3e 0a20 2020 203c 7061 7468  6)" />.    <path
-00000a80: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00000a90: 3431 392d 3322 0a20 2020 2020 2020 7374  419-3".       st
-00000aa0: 796c 653d 2266 696c 6c3a 2363 3031 3730  yle="fill:#c0170
-00000ab0: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00000ac0: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-00000ad0: 726f 3b73 7472 6f6b 653a 6e6f 6e65 3b73  ro;stroke:none;s
-00000ae0: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
-00000af0: 3435 3834 7078 3b73 7472 6f6b 652d 6c69  4584px;stroke-li
-00000b00: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00000b10: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00000b20: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00000b30: 3122 0a20 2020 2020 2020 643d 226d 202d  1".       d="m -
-00000b40: 3332 2e37 3638 3134 322c 3138 2e37 3039  32.768142,18.709
-00000b50: 3934 3520 6320 2d31 2e35 3936 3932 2c30  945 c -1.59692,0
-00000b60: 2e37 3537 3232 3720 302e 3030 352c 352e  .757227 0.005,5.
-00000b70: 3436 3433 3339 2031 2e31 3731 3135 2c37  464339 1.17115,7
-00000b80: 2e37 3234 3432 3920 312e 3535 3438 352c  .724429 1.55485,
-00000b90: 332e 3031 3334 3939 2031 332e 3736 3530  3.013499 13.7650
-00000ba0: 392c 3134 2e31 3634 3131 3920 3232 2e30  9,14.164119 22.0
-00000bb0: 3933 3232 3937 2c31 342e 3038 3538 3139  932297,14.085819
-00000bc0: 2031 2e33 3433 3638 2c2d 302e 3031 3234   1.34368,-0.0124
-00000bd0: 2033 2e34 3534 3138 392c 2d30 2e33 3636   3.454189,-0.366
-00000be0: 3439 2033 2e33 3239 3637 2c2d 312e 3730  49 3.32967,-1.70
-00000bf0: 3532 3820 2d30 2e31 3132 3832 2c2d 312e  528 -0.11282,-1.
-00000c00: 3231 3336 3720 2d32 2e31 3533 382c 2d31  21367 -2.1538,-1
-00000c10: 2e34 3836 3639 202d 332e 3336 3835 312c  .48669 -3.36851,
-00000c20: 2d31 2e35 3738 3139 202d 382e 3637 3031  -1.57819 -8.6701
-00000c30: 3139 372c 2d30 2e36 3533 3039 202d 3233  197,-0.65309 -23
-00000c40: 2e30 3931 3731 3937 2c31 352e 3032 3239  .0917197,15.0229
-00000c50: 3820 2d32 332e 3935 3932 3539 372c 3137  8 -23.9592597,17
-00000c60: 2e36 3130 3232 202d 302e 3637 3030 372c  .61022 -0.67007,
-00000c70: 312e 3939 3834 3120 2d30 2e32 3639 3237  1.99841 -0.26927
-00000c80: 2c34 2e31 3030 3732 2031 2e33 3031 3633  ,4.10072 1.30163
-00000c90: 2c34 2e30 3636 3835 2031 2e36 3530 332c  ,4.06685 1.6503,
-00000ca0: 2d30 2e30 3335 3520 312e 3935 3633 342c  -0.0355 1.95634,
-00000cb0: 2d30 2e38 3538 3337 2032 2e37 3434 3831  -0.85837 2.74481
-00000cc0: 2c2d 332e 3436 3135 3720 322e 3035 3932  ,-3.46157 2.0592
-00000cd0: 352c 2d36 2e37 3938 3831 2030 2e35 3439  5,-6.79881 0.549
-00000ce0: 3934 2c2d 3235 2e38 3337 3233 202d 302e  94,-25.83723 -0.
-00000cf0: 3633 3735 362c 2d33 312e 3838 3736 3136  63756,-31.887616
-00000d00: 202d 302e 3539 3831 322c 2d33 2e30 3437   -0.59812,-3.047
-00000d10: 3635 3620 2d31 2e33 3435 3239 2c2d 352e  656 -1.34529,-5.
-00000d20: 3438 3532 3432 202d 322e 3637 3531 362c  485242 -2.67516,
-00000d30: 2d34 2e38 3534 3636 3220 7a20 6d20 342e  -4.854662 z m 4.
-00000d40: 3030 3334 312c 322e 3733 3236 3820 6320  00341,2.73268 c 
-00000d50: 312e 3733 3038 312c 382e 3831 3330 3338  1.73081,8.813038
-00000d60: 2032 2e30 3536 3339 2c32 312e 3136 3631   2.05639,21.1661
-00000d70: 3938 2031 2e31 3530 3133 2c33 322e 3034  98 1.15013,32.04
-00000d80: 3436 3038 202d 302e 3330 3735 312c 332e  4608 -0.30751,3.
-00000d90: 3639 3133 3820 2d31 2e35 3733 3434 2c37  69138 -1.57344,7
-00000da0: 2e35 3731 3838 202d 342e 3638 3239 362c  .57188 -4.68296,
-00000db0: 372e 3831 3734 3720 2d32 2e32 3833 3036  7.81747 -2.28306
-00000dc0: 2c30 2e31 3830 3420 2d34 2e34 3031 3432  ,0.1804 -4.40142
-00000dd0: 2c2d 332e 3339 3536 202d 322e 3638 3237  ,-3.3956 -2.6827
-00000de0: 372c 2d36 2e37 3535 3433 2031 2e37 3535  7,-6.75543 1.755
-00000df0: 3134 2c2d 332e 3433 3130 3620 3135 2e33  14,-3.43106 15.3
-00000e00: 3530 3735 2c2d 3138 2e38 3435 3534 2032  5075,-18.84554 2
-00000e10: 362e 3739 3332 3339 372c 2d31 392e 3034  6.7932397,-19.04
-00000e20: 3932 3220 312e 3737 3531 392c 2d30 2e30  922 1.77519,-0.0
-00000e30: 3331 3620 342e 3231 3033 3739 2c31 2e32  316 4.210379,1.2
-00000e40: 3730 3438 2034 2e33 3734 3930 392c 332e  7048 4.374909,3.
-00000e50: 3033 3833 3420 302e 3138 3134 2c31 2e39  03834 0.1814,1.9
-00000e60: 3530 3039 202d 332e 3737 3837 3939 2c33  5009 -3.778799,3
-00000e70: 2e35 3335 3235 202d 352e 3733 3732 3239  .53525 -5.737229
-00000e80: 2c33 2e35 3533 3635 202d 3132 2e31 3338  ,3.55365 -12.138
-00000e90: 3438 3937 2c30 2e31 3134 3038 202d 3233  4897,0.11408 -23
-00000ea0: 2e31 3937 3439 3937 2c2d 3132 2e36 3432  .1974997,-12.642
-00000eb0: 3136 202d 3235 2e34 3032 3438 3937 2c2d  16 -25.4024897,-
-00000ec0: 3138 2e34 3833 3531 3220 2d30 2e39 3039  18.483512 -0.909
-00000ed0: 3631 2c2d 322e 3430 3937 3135 202d 312e  61,-2.409715 -1.
-00000ee0: 3439 3037 362c 2d38 2e30 3030 3033 3820  49076,-8.000038 
-00000ef0: 302e 3833 3638 332c 2d39 2e31 3033 3031  0.83683,-9.10301
-00000f00: 3820 312e 3933 3833 2c2d 302e 3931 3835  8 1.9383,-0.9185
-00000f10: 3132 2034 2e34 3738 3533 2c32 2e34 3937  12 4.47853,2.497
-00000f20: 3836 3920 352e 3335 3033 342c 362e 3933  869 5.35034,6.93
-00000f30: 3731 3132 207a 220a 2020 2020 2020 2073  7112 z".       s
-00000f40: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00000f50: 733d 2273 7363 7373 7363 7373 7373 7373  s="sscssscssssss
-00000f60: 7363 7373 7373 7322 202f 3e0a 2020 2020  scsssss" />.    
-00000f70: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-00000f80: 6c65 3d22 6669 6c6c 3a23 6530 3963 3138  le="fill:#e09c18
-00000f90: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00000fa0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
-00000fb0: 6b65 2d77 6964 7468 3a34 3b73 7472 6f6b  ke-width:4;strok
-00000fc0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00000fd0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00000fe0: 6974 6572 3b73 7472 6f6b 652d 6461 7368  iter;stroke-dash
-00000ff0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00001000: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00001010: 2020 2020 643d 224d 2037 322e 3137 3837      d="M 72.1787
-00001020: 3331 2c37 332e 3732 3837 3833 2039 302e  31,73.728783 90.
-00001030: 3430 3932 3637 2c35 322e 3430 3332 3936  409267,52.403296
-00001040: 2063 2030 2e35 3832 3632 362c 2d30 2e37   c 0.582626,-0.7
-00001050: 3136 3838 3420 2d36 2e33 3236 3434 2c2d  16884 -6.32644,-
-00001060: 352e 3433 3638 3838 2032 2e36 3335 3835  5.436888 2.63585
-00001070: 322c 2d39 2e35 3539 3234 3520 332e 3739  2,-9.559245 3.79
-00001080: 3532 3136 2c2d 312e 3734 3536 3733 2039  5216,-1.745673 9
-00001090: 2e39 3139 3231 312c 302e 3930 3538 3420  .919211,0.90584 
-000010a0: 3132 2e35 3236 3133 312c 332e 3737 3235  12.526131,3.7725
-000010b0: 3036 2032 2e34 3630 3339 2c2d 302e 3933  06 2.46039,-0.93
-000010c0: 3233 3438 2030 2e36 3335 3334 2c2d 302e  2348 0.63534,-0.
-000010d0: 3737 3734 3139 2031 2e38 3039 3932 2c2d  777419 1.80992,-
-000010e0: 302e 3730 3637 3434 2032 312e 3830 3830  0.706744 21.8080
-000010f0: 372c 2d30 2e38 3335 3032 3520 3335 2e31  7,-0.835025 35.1
-00001100: 3934 3238 2c2d 302e 3834 3839 3237 2035  9428,-0.848927 5
-00001110: 362e 3638 3133 382c 332e 3435 3720 332e  6.68138,3.457 3.
-00001120: 3434 3730 362c 302e 3639 3037 3735 2035  44706,0.690775 5
-00001130: 2e32 3733 3736 2c32 2e33 3331 3032 2036  .27376,2.33102 6
-00001140: 2e38 3839 3432 2c35 2e33 3135 3037 2034  .88942,5.31507 4
-00001150: 2e37 3737 3431 2c38 2e38 3233 3633 2035  .77741,8.82363 5
-00001160: 2e30 3535 3832 2c31 372e 3438 3233 3420  .05582,17.48234 
-00001170: 2d31 2e30 3536 392c 3237 2e32 3737 3832  -1.0569,27.27782
-00001180: 3820 2d31 2e34 3031 3836 2c32 2e32 3436  8 -1.40186,2.246
-00001190: 3434 202d 342e 3139 3238 362c 342e 3830  44 -4.19286,4.80
-000011a0: 3834 3320 2d36 2e38 3334 3931 2c34 2e39  843 -6.83491,4.9
-000011b0: 3835 3334 202d 3131 2e33 3234 3232 2c30  8534 -11.32422,0
-000011c0: 2e37 3538 3237 202d 3236 2e33 3434 3136  .75827 -26.34416
-000011d0: 2c2d 302e 3632 3637 202d 3331 2e39 3933  ,-0.6267 -31.993
-000011e0: 3739 2c2d 302e 3838 3739 3820 2d33 2e36  79,-0.88798 -3.6
-000011f0: 3332 3935 2c2d 302e 3136 3830 3120 2d36  3295,-0.16801 -6
-00001200: 2e38 3338 3232 2c33 2e34 3436 3632 202d  .83822,3.44662 -
-00001210: 372e 3930 3238 382c 362e 3136 3536 3920  7.90288,6.16569 
-00001220: 2d32 2e39 3833 3134 2c37 2e36 3138 3736  -2.98314,7.61876
-00001230: 3920 2d36 2e38 3937 3734 2c31 302e 3533  9 -6.89774,10.53
-00001240: 3137 3239 202d 3132 2e31 3632 3539 2c31  1729 -12.16259,1
-00001250: 352e 3232 3331 3939 2031 2e34 3835 3531  5.223199 1.48551
-00001260: 2c2d 352e 3131 3338 3220 2d31 2e36 3931  ,-5.11382 -1.691
-00001270: 3933 2c2d 382e 3135 3334 3420 2d33 2e31  93,-8.15344 -3.1
-00001280: 3634 3032 2c2d 382e 3533 3630 3920 2d30  6402,-8.53609 -0
-00001290: 2e31 3138 3534 2c31 2e34 3733 3635 202d  .11854,1.47365 -
-000012a0: 342e 3232 3230 352c 352e 3531 3037 3220  4.22205,5.51072 
-000012b0: 2d35 2e33 3936 3231 2c35 2e39 3436 3438  -5.39621,5.94648
-000012c0: 2031 2e32 3330 3937 2c2d 322e 3831 3720   1.23097,-2.817 
-000012d0: 302e 3133 3636 382c 2d34 2e30 3831 3534  0.13668,-4.08154
-000012e0: 202d 302e 3938 3830 372c 2d36 2e35 3539   -0.98807,-6.559
-000012f0: 3534 202d 302e 3132 3636 372c 2d30 2e35  54 -0.12667,-0.5
-00001300: 3738 3434 202d 302e 3336 3237 372c 2d31  7844 -0.36277,-1
-00001310: 2e30 3635 3120 2d30 2e38 3838 3332 2c2d  .0651 -0.88832,-
-00001320: 312e 3733 3535 3234 202d 312e 3530 3736  1.735524 -1.5076
-00001330: 3434 2c31 2e32 3935 3831 3420 2d32 2e33  44,1.295814 -2.3
-00001340: 3135 3136 312c 322e 3939 3534 3134 202d  15161,2.995414 -
-00001350: 352e 3334 3139 3838 2c33 2e39 3938 3033  5.341988,3.99803
-00001360: 3420 302e 3537 3035 332c 2d34 2e32 3532  4 0.57053,-4.252
-00001370: 3230 3120 2d31 2e32 3436 3232 392c 2d36  201 -1.246229,-6
-00001380: 2e37 3437 3234 3720 2d33 2e30 3731 3931  .747247 -3.07191
-00001390: 382c 2d31 302e 3433 3131 3938 202d 312e  8,-10.431198 -1.
-000013a0: 3232 3431 3039 2c33 2e34 3035 3730 3920  224109,3.405709 
-000013b0: 2d32 2e31 3230 3331 382c 352e 3333 3433  -2.120318,5.3343
-000013c0: 3932 202d 362e 3739 3132 3335 2c37 2e33  92 -6.791235,7.3
-000013d0: 3030 3136 3820 312e 3135 3530 3738 2c2d  00168 1.155078,-
-000013e0: 312e 3832 3837 3138 2031 2e38 3035 3039  1.828718 1.80509
-000013f0: 322c 2d33 2e34 3330 3230 3820 322e 3133  2,-3.430208 2.13
-00001400: 3934 372c 2d34 2e36 3136 3339 3720 6c20  947,-4.616397 l 
-00001410: 302e 3236 3531 3537 2c2d 322e 3537 3133  0.265157,-2.5713
-00001420: 3337 2063 202d 302e 3133 3032 3037 2c2d  37 c -0.130207,-
-00001430: 312e 3232 3831 3437 2030 2e30 3630 3936  1.228147 0.06096
-00001440: 2c2d 322e 3030 3432 3834 202d 302e 3837  ,-2.004284 -0.87
-00001450: 3836 3235 2c2d 332e 3534 3735 3131 202d  8625,-3.547511 -
-00001460: 302e 3038 3738 382c 302e 3632 3333 3531  0.08788,0.623351
-00001470: 202d 322e 3937 3032 3936 2c32 2e39 3233   -2.970296,2.923
-00001480: 3734 3820 2d34 2e39 3537 3232 362c 332e  748 -4.957226,3.
-00001490: 3132 3336 3834 2031 2e36 3939 3639 322c  123684 1.699692,
-000014a0: 2d34 2e31 3437 3036 3320 302e 3930 3130  -4.147063 0.9010
-000014b0: 342c 2d35 2e39 3539 3820 2d30 2e31 3232  4,-5.9598 -0.122
-000014c0: 3939 382c 2d37 2e37 3633 3620 2d30 2e38  998,-7.7636 -0.8
-000014d0: 3538 3036 332c 302e 3833 3236 3133 202d  58063,0.832613 -
-000014e0: 332e 3335 3931 3331 2c33 2e32 3530 3031  3.359131,3.25001
-000014f0: 3320 2d35 2e34 3630 3336 382c 332e 3534  3 -5.460368,3.54
-00001500: 3239 3238 2032 2e32 3533 3435 372c 2d33  2928 2.253457,-3
-00001510: 2e32 3431 3933 3620 2d30 2e32 3636 3232  .241936 -0.26622
-00001520: 382c 2d38 2e34 3733 3335 3820 2d31 2e30  8,-8.473358 -1.0
-00001530: 3334 3335 322c 2d39 2e38 3139 3836 206c  34352,-9.81986 l
-00001540: 202d 332e 3133 3134 3633 2c2d 322e 3034   -3.131463,-2.04
-00001550: 3734 3134 207a 220a 2020 2020 2020 2069  7414 z".       i
-00001560: 643d 2270 6174 6831 2d36 220a 2020 2020  d="path1-6".    
-00001570: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00001580: 7479 7065 733d 2263 6373 6363 7373 7373  types="ccsccssss
-00001590: 7373 6363 6363 6363 6363 6363 6363 6363  sscccccccccccccc
-000015a0: 6363 6322 202f 3e0a 2020 2020 3c70 6174  ccc" />.    <pat
-000015b0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-000015c0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-000015d0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000015e0: 7769 6474 683a 302e 3236 3435 3833 7078  width:0.264583px
-000015f0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00001600: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00001610: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00001620: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00001630: 2020 2020 643d 226d 2031 3237 2e37 3936      d="m 127.796
-00001640: 3733 2c32 3234 2e34 3830 3137 2063 2030  73,224.48017 c 0
-00001650: 2c30 2039 2e38 3638 3138 2c2d 392e 3032  ,0 9.86818,-9.02
-00001660: 3939 3320 3136 2e39 3334 3638 2c2d 3136  993 16.93468,-16
-00001670: 2e37 3134 3434 2034 2e38 3439 3533 2c2d  .71444 4.84953,-
-00001680: 352e 3237 3336 3620 352e 3734 3839 312c  5.27366 5.74891,
-00001690: 2d39 2e38 3132 3235 2037 2e36 3036 372c  -9.81225 7.6067,
-000016a0: 2d31 342e 3831 3737 3620 302e 3837 3135  -14.81776 0.8715
-000016b0: 342c 2d32 2e33 3438 3232 2033 2e31 3633  4,-2.34822 3.163
-000016c0: 3034 2c2d 382e 3638 3236 3720 3131 2e33  04,-8.68267 11.3
-000016d0: 3636 3838 2c2d 382e 3836 3538 3720 3132  6688,-8.86587 12
-000016e0: 2e33 3137 3534 2c2d 302e 3237 3530 3620  .31754,-0.27506 
-000016f0: 3134 2e36 3431 3035 2c34 2e33 3335 3937  14.64105,4.33597
-00001700: 2031 362e 3935 3537 322c 352e 3139 3436   16.95572,5.1946
-00001710: 3320 392e 3030 3334 342c 332e 3333 3939  3 9.00344,3.3399
-00001720: 3820 3139 2e30 3133 3336 2c35 2e34 3435  8 19.01336,5.445
-00001730: 3139 2032 312e 3832 3437 312c 372e 3234  19 21.82471,7.24
-00001740: 3439 2033 2e39 3631 3839 2c32 2e35 3336  49 3.96189,2.536
-00001750: 3234 202d 302e 3733 3234 372c 3139 2e33  24 -0.73247,19.3
-00001760: 3031 3733 202d 352e 3139 3531 362c 3230  0173 -5.19516,20
-00001770: 2e36 3738 3632 202d 372e 3436 3333 392c  .67862 -7.46339,
-00001780: 322e 3330 3237 3120 2d31 362e 3931 3630  2.30271 -16.9160
-00001790: 332c 2d32 2e39 3436 3033 202d 3233 2e31  3,-2.94603 -23.1
-000017a0: 3733 3931 2c30 2e37 3733 3437 220a 2020  7391,0.77347".  
-000017b0: 2020 2020 2069 643d 2270 6174 6834 3737       id="path477
-000017c0: 3922 0a20 2020 2020 2020 736f 6469 706f  9".       sodipo
-000017d0: 6469 3a6e 6f64 6574 7970 6573 3d22 6373  di:nodetypes="cs
-000017e0: 7373 7373 7363 2220 2f3e 0a20 2020 203c  sssssc" />.    <
-000017f0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00001800: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
-00001810: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00001820: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
-00001830: 3370 783b 7374 726f 6b65 2d6c 696e 6563  3px;stroke-linec
-00001840: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00001850: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00001860: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00001870: 2020 2020 2020 2064 3d22 6d20 3131 342e         d="m 114.
-00001880: 3735 3130 362c 3230 302e 3339 3337 3720  75106,200.39377 
-00001890: 6320 312e 3137 3134 382c 342e 3130 3939  c 1.17148,4.1099
-000018a0: 3820 312e 3332 3539 2c31 352e 3736 3331  8 1.3259,15.7631
-000018b0: 3220 302e 3935 3731 342c 3233 2e31 3334  2 0.95714,23.134
-000018c0: 3233 220a 2020 2020 2020 2069 643d 2270  23".       id="p
-000018d0: 6174 6834 3738 3122 0a20 2020 2020 2020  ath4781".       
-000018e0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-000018f0: 6573 3d22 6363 2220 2f3e 0a20 2020 203c  es="cc" />.    <
-00001900: 656c 6c69 7073 650a 2020 2020 2020 2073  ellipse.       s
-00001910: 7479 6c65 3d22 6f70 6163 6974 793a 302e  tyle="opacity:0.
-00001920: 3939 3b66 696c 6c3a 2330 3030 3030 303b  99;fill:#000000;
-00001930: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00001940: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00001950: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00001960: 6f6b 652d 7769 6474 683a 312e 3538 3735  oke-width:1.5875
-00001970: 652d 3038 3b73 7472 6f6b 652d 6c69 6e65  e-08;stroke-line
-00001980: 6361 703a 726f 756e 643b 7374 726f 6b65  cap:round;stroke
-00001990: 2d6c 696e 656a 6f69 6e3a 726f 756e 6422  -linejoin:round"
-000019a0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-000019b0: 3438 3335 220a 2020 2020 2020 2063 783d  4835".       cx=
-000019c0: 2231 3337 2e35 3439 3434 220a 2020 2020  "137.54944".    
-000019d0: 2020 2063 793d 2231 3833 2e38 3337 3633     cy="183.83763
-000019e0: 220a 2020 2020 2020 2072 783d 2231 2e33  ".       rx="1.3
-000019f0: 3334 3438 3431 220a 2020 2020 2020 2072  344841".       r
-00001a00: 793d 2232 2e33 3334 3439 3834 2220 2f3e  y="2.3344984" />
-00001a10: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00001a20: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
-00001a30: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
-00001a40: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
-00001a50: 2e32 3031 3336 3970 783b 7374 726f 6b65  .201369px;stroke
-00001a60: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00001a70: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00001a80: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
-00001a90: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-00001aa0: 6d20 3130 302e 3738 3537 312c 3136 362e  m 100.78571,166.
-00001ab0: 3535 3134 3520 6320 302c 3020 2d31 2e32  55145 c 0,0 -1.2
-00001ac0: 3036 3838 352c 2d32 2e32 3730 3631 202d  06885,-2.27061 -
-00001ad0: 322e 3338 3632 3535 2c2d 322e 3138 3735  2.386255,-2.1875
-00001ae0: 3720 2d31 2e31 3839 3438 2c30 2e30 3833  7 -1.18948,0.083
-00001af0: 3720 2d32 2e31 3537 3336 2c31 2e37 3730  7 -2.15736,1.770
-00001b00: 3038 202d 322e 3031 3732 322c 322e 3935  08 -2.01722,2.95
-00001b10: 3432 3420 302e 3133 3431 2c31 2e31 3332  424 0.1341,1.132
-00001b20: 3832 2032 2e35 3336 3138 2c32 2e32 3937  82 2.53618,2.297
-00001b30: 3635 2032 2e35 3336 3138 2c32 2e32 3937  65 2.53618,2.297
-00001b40: 3635 220a 2020 2020 2020 2069 643d 2270  65".       id="p
-00001b50: 6174 6835 3331 3322 0a20 2020 2020 2020  ath5313".       
-00001b60: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00001b70: 6573 3d22 6373 7363 2220 2f3e 0a20 2020  es="cssc" />.   
-00001b80: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00001b90: 796c 653d 2266 696c 6c3a 2330 3030 3030  yle="fill:#00000
-00001ba0: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00001bb0: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00001bc0: 6f6b 652d 7769 6474 683a 302e 3236 3435  oke-width:0.2645
-00001bd0: 3833 7078 3b73 7472 6f6b 652d 6c69 6e65  83px;stroke-line
-00001be0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00001bf0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00001c00: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00001c10: 0a20 2020 2020 2020 643d 226d 2031 3036  .       d="m 106
-00001c20: 2e37 3236 3137 2c31 3734 2e39 3631 3438  .72617,174.96148
-00001c30: 2063 2033 2e34 3432 3237 2c30 2e34 3338   c 3.44227,0.438
-00001c40: 3839 2035 2e36 3136 3737 2c30 2e36 3536  89 5.61677,0.656
-00001c50: 3533 2039 2e33 3138 3032 2c31 2e32 3034  53 9.31802,1.204
-00001c60: 3532 2030 2e31 3938 3833 2c30 2e30 3239  52 0.19883,0.029
-00001c70: 3420 2d30 2e35 3835 3335 2c30 2e38 3038  4 -0.58535,0.808
-00001c80: 3735 202d 302e 3738 3337 362c 302e 3737  75 -0.78376,0.77
-00001c90: 3635 3920 2d31 2e32 3431 3733 2c2d 302e  659 -1.24173,-0.
-00001ca0: 3230 3132 3520 2d31 2e35 3637 3635 2c2d  20125 -1.56765,-
-00001cb0: 302e 3339 3238 3720 2d32 2e33 3832 3534  0.39287 -2.38254
-00001cc0: 2c2d 302e 3037 3436 202d 302e 3938 3032  ,-0.0746 -0.9802
-00001cd0: 322c 302e 3338 3238 3420 2d30 2e32 3539  2,0.38284 -0.259
-00001ce0: 3734 2c31 2e31 3635 3635 202d 312e 3236  74,1.16565 -1.26
-00001cf0: 3737 372c 312e 3436 3737 3420 2d30 2e38  777,1.46774 -0.8
-00001d00: 3835 3238 2c30 2e32 3635 3320 2d32 2e34  8528,0.2653 -2.4
-00001d10: 3837 352c 2d30 2e31 3239 3934 202d 332e  875,-0.12994 -3.
-00001d20: 3036 3537 332c 2d30 2e38 3530 3837 202d  06573,-0.85087 -
-00001d30: 302e 3533 3333 362c 2d30 2e36 3635 202d  0.53336,-0.665 -
-00001d40: 302e 3631 3535 332c 2d31 2e31 3735 3039  0.61553,-1.17509
-00001d50: 202d 302e 3832 3631 342c 2d31 2e34 3634   -0.82614,-1.464
-00001d60: 3634 202d 302e 3036 3831 2c2d 302e 3039  64 -0.0681,-0.09
-00001d70: 3336 202d 302e 3738 3630 382c 2d30 2e31  36 -0.78608,-0.1
-00001d80: 3533 3832 202d 312e 3136 3235 392c 2d30  5382 -1.16259,-0
-00001d90: 2e35 3037 3138 202d 302e 3332 3237 342c  .50718 -0.32274,
-00001da0: 2d30 2e33 3032 3839 202d 302e 3036 3433  -0.30289 -0.0643
-00001db0: 2c2d 302e 3538 3134 3920 302e 3137 3035  ,-0.58149 0.1705
-00001dc0: 312c 2d30 2e35 3531 3536 207a 220a 2020  1,-0.55156 z".  
-00001dd0: 2020 2020 2069 643d 2270 6174 6835 3331       id="path531
-00001de0: 3522 0a20 2020 2020 2020 736f 6469 706f  5".       sodipo
-00001df0: 6469 3a6e 6f64 6574 7970 6573 3d22 7373  di:nodetypes="ss
-00001e00: 7373 7373 7373 7322 202f 3e0a 2020 2020  sssssss" />.    
-00001e10: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-00001e20: 6c65 3d22 6669 6c6c 3a6e 6f6e 653b 7374  le="fill:none;st
-00001e30: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00001e40: 6f6b 652d 7769 6474 683a 302e 3236 3435  oke-width:0.2645
-00001e50: 3833 7078 3b73 7472 6f6b 652d 6c69 6e65  83px;stroke-line
-00001e60: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00001e70: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00001e80: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00001e90: 0a20 2020 2020 2020 643d 224d 2032 392e  .       d="M 29.
-00001ea0: 3536 3635 3738 2c32 3434 2e39 3634 3535  566578,244.96455
-00001eb0: 2048 2031 3837 2e33 3637 3322 0a20 2020   H 187.3673".   
-00001ec0: 2020 2020 6964 3d22 7061 7468 3839 3437      id="path8947
-00001ed0: 2220 2f3e 0a20 2020 203c 7573 650a 2020  " />.    <use.  
-00001ee0: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
-00001ef0: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
-00001f00: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
-00001f10: 3839 3835 220a 2020 2020 2020 2069 643d  8985".       id=
-00001f20: 2275 7365 3138 3831 3322 0a20 2020 2020  "use18813".     
-00001f30: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00001f40: 6e73 6c61 7465 2831 2e36 3637 3134 3138  nslate(1.6671418
-00001f50: 2c32 362e 3438 3533 3038 2922 202f 3e0a  ,26.485308)" />.
-00001f60: 2020 2020 3c75 7365 0a20 2020 2020 2020      <use.       
-00001f70: 783d 2230 220a 2020 2020 2020 2079 3d22  x="0".       y="
-00001f80: 3022 0a20 2020 2020 2020 786c 696e 6b3a  0".       xlink:
-00001f90: 6872 6566 3d22 2370 6174 6838 3938 352d  href="#path8985-
-00001fa0: 3822 0a20 2020 2020 2020 6964 3d22 7573  8".       id="us
-00001fb0: 6532 3532 3034 220a 2020 2020 2020 2074  e25204".       t
-00001fc0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00001fd0: 6174 6528 2d31 342e 3235 3730 3135 2c32  ate(-14.257015,2
-00001fe0: 352e 3037 3635 3038 2922 202f 3e0a 2020  5.076508)" />.  
-00001ff0: 2020 3c75 7365 0a20 2020 2020 2020 783d    <use.       x=
-00002000: 2230 220a 2020 2020 2020 2079 3d22 3022  "0".       y="0"
-00002010: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-00002020: 6566 3d22 2370 6174 6838 3938 352d 3822  ef="#path8985-8"
-00002030: 0a20 2020 2020 2020 6964 3d22 7573 6532  .       id="use2
-00002040: 3532 3032 220a 2020 2020 2020 2074 7261  5202".       tra
-00002050: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00002060: 6528 2d31 302e 3130 3434 3037 2c32 312e  e(-10.104407,21.
-00002070: 3732 3239 3431 2922 202f 3e0a 2020 2020  722941)" />.    
-00002080: 3c75 7365 0a20 2020 2020 2020 783d 2230  <use.       x="0
-00002090: 220a 2020 2020 2020 2079 3d22 3022 0a20  ".       y="0". 
-000020a0: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-000020b0: 3d22 2370 6174 6838 3938 352d 3822 0a20  ="#path8985-8". 
-000020c0: 2020 2020 2020 6964 3d22 7573 6533 3533        id="use353
-000020d0: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
-000020e0: 726d 3d22 7472 616e 736c 6174 6528 3233  rm="translate(23
-000020f0: 2e39 3233 3435 392c 3231 2e31 3939 3138  .923459,21.19918
-00002100: 3429 2220 2f3e 0a20 2020 203c 7265 6374  4)" />.    <rect
-00002110: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00002120: 7061 6369 7479 3a30 2e39 393b 6669 6c6c  pacity:0.99;fill
-00002130: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
-00002140: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-00002150: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-00002160: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00002170: 7769 6474 683a 302e 333b 7374 726f 6b65  width:0.3;stroke
-00002180: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
-00002190: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
-000021a0: 6f75 6e64 3b73 7472 6f6b 652d 6461 7368  ound;stroke-dash
-000021b0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000021c0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000021d0: 2020 2020 6964 3d22 7265 6374 3230 3431      id="rect2041
-000021e0: 352d 332d 3622 0a20 2020 2020 2020 7769  5-3-6".       wi
-000021f0: 6474 683d 2233 2e34 3230 3332 3831 220a  dth="3.4203281".
-00002200: 2020 2020 2020 2068 6569 6768 743d 2232         height="2
-00002210: 332e 3430 3233 3432 220a 2020 2020 2020  3.402342".      
-00002220: 2078 3d22 3131 332e 3638 3339 3822 0a20   x="113.68398". 
-00002230: 2020 2020 2020 793d 2232 3435 2e34 3831        y="245.481
-00002240: 3633 2220 2f3e 0a20 2020 203c 7265 6374  63" />.    <rect
-00002250: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00002260: 7061 6369 7479 3a30 2e39 393b 6669 6c6c  pacity:0.99;fill
-00002270: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
-00002280: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-00002290: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-000022a0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000022b0: 7769 6474 683a 302e 333b 7374 726f 6b65  width:0.3;stroke
-000022c0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
-000022d0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
-000022e0: 6f75 6e64 3b73 7472 6f6b 652d 6461 7368  ound;stroke-dash
-000022f0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00002300: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00002310: 2020 2020 6964 3d22 7265 6374 3230 3431      id="rect2041
-00002320: 352d 3322 0a20 2020 2020 2020 7769 6474  5-3".       widt
-00002330: 683d 2233 2e34 3230 3332 3831 220a 2020  h="3.4203281".  
-00002340: 2020 2020 2068 6569 6768 743d 2232 332e       height="23.
-00002350: 3430 3233 3432 220a 2020 2020 2020 2078  402342".       x
-00002360: 3d22 3937 2e39 3036 3133 3622 0a20 2020  ="97.906136".   
-00002370: 2020 2020 793d 2232 3435 2e35 3439 3031      y="245.54901
-00002380: 2220 2f3e 0a20 2020 203c 7265 6374 0a20  " />.    <rect. 
-00002390: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-000023a0: 6369 7479 3a30 2e39 393b 6669 6c6c 3a23  city:0.99;fill:#
-000023b0: 6666 6666 6666 3b66 696c 6c2d 6f70 6163  ffffff;fill-opac
-000023c0: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-000023d0: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a23  nonzero;stroke:#
-000023e0: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-000023f0: 6474 683a 302e 333b 7374 726f 6b65 2d6c  dth:0.3;stroke-l
-00002400: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00002410: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
-00002420: 6e64 3b73 7472 6f6b 652d 6461 7368 6172  nd;stroke-dashar
-00002430: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00002440: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00002450: 2020 6964 3d22 7265 6374 3230 3431 352d    id="rect20415-
-00002460: 332d 3522 0a20 2020 2020 2020 7769 6474  3-5".       widt
-00002470: 683d 2233 2e34 3230 3332 3831 220a 2020  h="3.4203281".  
-00002480: 2020 2020 2068 6569 6768 743d 2239 2e37       height="9.7
-00002490: 3134 3230 3736 220a 2020 2020 2020 2078  142076".       x
-000024a0: 3d22 2d32 3538 2e36 3038 3436 220a 2020  ="-258.60846".  
-000024b0: 2020 2020 2079 3d22 3133 352e 3435 3636       y="135.4566
-000024c0: 3722 0a20 2020 2020 2020 7472 616e 7366  7".       transf
-000024d0: 6f72 6d3d 2272 6f74 6174 6528 2d39 3029  orm="rotate(-90)
-000024e0: 2220 2f3e 0a20 2020 203c 7265 6374 0a20  " />.    <rect. 
-000024f0: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-00002500: 6369 7479 3a30 2e39 393b 6669 6c6c 3a23  city:0.99;fill:#
-00002510: 6666 6666 6666 3b66 696c 6c2d 6f70 6163  ffffff;fill-opac
-00002520: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-00002530: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a23  nonzero;stroke:#
-00002540: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-00002550: 6474 683a 302e 333b 7374 726f 6b65 2d6c  dth:0.3;stroke-l
-00002560: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00002570: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
-00002580: 6e64 3b73 7472 6f6b 652d 6461 7368 6172  nd;stroke-dashar
-00002590: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-000025a0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-000025b0: 2020 6964 3d22 7265 6374 3230 3431 352d    id="rect20415-
-000025c0: 332d 352d 3322 0a20 2020 2020 2020 7769  3-5-3".       wi
-000025d0: 6474 683d 2233 2e34 3230 3332 3831 220a  dth="3.4203281".
-000025e0: 2020 2020 2020 2068 6569 6768 743d 2231         height="1
-000025f0: 332e 3439 3633 3434 220a 2020 2020 2020  3.496344".      
-00002600: 2078 3d22 2d32 3438 2e37 3736 3334 220a   x="-248.77634".
-00002610: 2020 2020 2020 2079 3d22 3133 342e 3736         y="134.76
-00002620: 3534 3622 0a20 2020 2020 2020 7472 616e  546".       tran
-00002630: 7366 6f72 6d3d 2272 6f74 6174 6528 2d39  sform="rotate(-9
-00002640: 3029 2220 2f3e 0a20 2020 203c 7265 6374  0)" />.    <rect
-00002650: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00002660: 7061 6369 7479 3a30 2e39 393b 6669 6c6c  pacity:0.99;fill
-00002670: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
-00002680: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-00002690: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-000026a0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000026b0: 7769 6474 683a 302e 333b 7374 726f 6b65  width:0.3;stroke
-000026c0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
-000026d0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
-000026e0: 6f75 6e64 3b73 7472 6f6b 652d 6461 7368  ound;stroke-dash
-000026f0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00002700: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00002710: 2020 2020 6964 3d22 7265 6374 3230 3431      id="rect2041
-00002720: 352d 332d 3722 0a20 2020 2020 2020 7769  5-3-7".       wi
-00002730: 6474 683d 2233 2e34 3230 3332 3831 220a  dth="3.4203281".
-00002740: 2020 2020 2020 2068 6569 6768 743d 2232         height="2
-00002750: 332e 3430 3233 3432 220a 2020 2020 2020  3.402342".      
-00002760: 2078 3d22 3133 342e 3236 3536 3422 0a20   x="134.26564". 
-00002770: 2020 2020 2020 793d 2232 3435 2e34 3532        y="245.452
-00002780: 3536 2220 2f3e 0a20 2020 203c 7061 7468  56" />.    <path
-00002790: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000027a0: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
-000027b0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-000027c0: 6964 7468 3a30 2e32 3634 3538 3370 783b  idth:0.264583px;
-000027d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-000027e0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-000027f0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00002800: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00002810: 2020 2064 3d22 4d20 3239 2e34 3039 3739     d="M 29.40979
-00002820: 372c 3235 352e 3239 3131 3120 4820 3138  7,255.29111 H 18
-00002830: 362e 3837 3434 3722 0a20 2020 2020 2020  6.87447".       
-00002840: 6964 3d22 7061 7468 3839 3439 2220 2f3e  id="path8949" />
-00002850: 0a20 2020 203c 7573 650a 2020 2020 2020  .    <use.      
-00002860: 2078 3d22 3022 0a20 2020 2020 2020 793d   x="0".       y=
-00002870: 2230 220a 2020 2020 2020 2078 6c69 6e6b  "0".       xlink
-00002880: 3a68 7265 663d 2223 7061 7468 3839 3835  :href="#path8985
-00002890: 2d38 220a 2020 2020 2020 2069 643d 2275  -8".       id="u
-000028a0: 7365 3235 3230 3822 0a20 2020 2020 2020  se25208".       
-000028b0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-000028c0: 6c61 7465 282d 3130 2e31 3734 3931 2c33  late(-10.17491,3
-000028d0: 312e 3939 3533 3235 2922 202f 3e0a 2020  1.995325)" />.  
-000028e0: 2020 3c75 7365 0a20 2020 2020 2020 783d    <use.       x=
-000028f0: 2230 220a 2020 2020 2020 2079 3d22 3022  "0".       y="0"
-00002900: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-00002910: 6566 3d22 2370 6174 6838 3938 352d 3822  ef="#path8985-8"
-00002920: 0a20 2020 2020 2020 6964 3d22 7573 6533  .       id="use3
-00002930: 3531 220a 2020 2020 2020 2074 7261 6e73  51".       trans
-00002940: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00002950: 3230 2e36 3232 3336 392c 3332 2e38 3933  20.622369,32.893
-00002960: 3634 3729 2220 2f3e 0a20 2020 203c 7573  647)" />.    <us
-00002970: 650a 2020 2020 2020 2078 3d22 3022 0a20  e.       x="0". 
-00002980: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
-00002990: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
-000029a0: 7061 7468 3839 3835 2d38 220a 2020 2020  path8985-8".    
-000029b0: 2020 2069 643d 2275 7365 3533 3522 0a20     id="use535". 
-000029c0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000029d0: 2274 7261 6e73 6c61 7465 2834 342e 3336  "translate(44.36
-000029e0: 3032 3638 2c33 322e 3231 3234 3235 2922  0268,32.212425)"
-000029f0: 202f 3e0a 2020 2020 3c75 7365 0a20 2020   />.    <use.   
-00002a00: 2020 2020 783d 2230 220a 2020 2020 2020      x="0".      
-00002a10: 2079 3d22 3022 0a20 2020 2020 2020 786c   y="0".       xl
-00002a20: 696e 6b3a 6872 6566 3d22 2370 6174 6838  ink:href="#path8
-00002a30: 3938 352d 3822 0a20 2020 2020 2020 6964  985-8".       id
-00002a40: 3d22 7573 6535 3337 220a 2020 2020 2020  ="use537".      
-00002a50: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00002a60: 736c 6174 6528 3534 2e37 3030 3733 322c  slate(54.700732,
-00002a70: 3331 2e34 3633 3337 3529 2220 2f3e 0a20  31.463375)" />. 
-00002a80: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00002a90: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
-00002aa0: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00002ab0: 7374 726f 6b65 2d77 6964 7468 3a30 2e32  stroke-width:0.2
-00002ac0: 3634 3538 3370 783b 7374 726f 6b65 2d6c  64583px;stroke-l
-00002ad0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00002ae0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-00002af0: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
-00002b00: 3a31 220a 2020 2020 2020 2064 3d22 4d20  :1".       d="M 
-00002b10: 3239 2e31 3335 3838 382c 3236 392e 3038  29.135888,269.08
-00002b20: 3937 3520 4820 3138 362e 3535 3836 220a  975 H 186.5586".
-00002b30: 2020 2020 2020 2069 643d 2270 6174 6838         id="path8
-00002b40: 3935 3122 202f 3e0a 2020 2020 3c75 7365  951" />.    <use
-00002b50: 0a20 2020 2020 2020 783d 2230 220a 2020  .       x="0".  
-00002b60: 2020 2020 2079 3d22 3022 0a20 2020 2020       y="0".     
-00002b70: 2020 786c 696e 6b3a 6872 6566 3d22 2370    xlink:href="#p
-00002b80: 6174 6838 3938 352d 3822 0a20 2020 2020  ath8985-8".     
-00002b90: 2020 6964 3d22 7573 6532 3532 3036 220a    id="use25206".
-00002ba0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00002bb0: 3d22 7472 616e 736c 6174 6528 2d31 332e  ="translate(-13.
-00002bc0: 3831 3139 3933 2c33 302e 3232 3535 3233  811993,30.225523
-00002bd0: 2922 202f 3e0a 2020 2020 3c75 7365 0a20  )" />.    <use. 
-00002be0: 2020 2020 2020 783d 2230 220a 2020 2020        x="0".    
-00002bf0: 2020 2079 3d22 3022 0a20 2020 2020 2020     y="0".       
-00002c00: 786c 696e 6b3a 6872 6566 3d22 2370 6174  xlink:href="#pat
-00002c10: 6838 3938 352d 3822 0a20 2020 2020 2020  h8985-8".       
-00002c20: 6964 3d22 7573 6532 3532 3130 220a 2020  id="use25210".  
-00002c30: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00002c40: 7472 616e 736c 6174 6528 2d36 2e36 3133  translate(-6.613
-00002c50: 3038 3931 2c32 332e 3234 3732 3433 2922  0891,23.247243)"
-00002c60: 202f 3e0a 2020 2020 3c75 7365 0a20 2020   />.    <use.   
-00002c70: 2020 2020 783d 2230 220a 2020 2020 2020      x="0".      
-00002c80: 2079 3d22 3022 0a20 2020 2020 2020 786c   y="0".       xl
-00002c90: 696e 6b3a 6872 6566 3d22 2370 6174 6838  ink:href="#path8
-00002ca0: 3938 352d 3822 0a20 2020 2020 2020 6964  985-8".       id
-00002cb0: 3d22 7573 6532 3532 3132 220a 2020 2020  ="use25212".    
-00002cc0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00002cd0: 616e 736c 6174 6528 2d36 2e35 3639 3635  anslate(-6.56965
-00002ce0: 3031 2c33 302e 3432 3933 3833 2922 202f  01,30.429383)" /
-00002cf0: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-00002d00: 2020 2073 7479 6c65 3d22 6669 6c6c 3a6e     style="fill:n
-00002d10: 6f6e 653b 7374 726f 6b65 3a23 3030 3030  one;stroke:#0000
-00002d20: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-00002d30: 302e 3236 3435 3833 7078 3b73 7472 6f6b  0.264583px;strok
-00002d40: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00002d50: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00002d60: 6974 6572 3b73 7472 6f6b 652d 6f70 6163  iter;stroke-opac
-00002d70: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-00002d80: 226d 2036 342e 3932 3634 3336 2c32 3538  "m 64.926436,258
-00002d90: 2e35 3236 3239 2063 202d 302e 3230 3836  .52629 c -0.2086
-00002da0: 392c 2d30 2e30 3538 3320 2d31 2e39 3334  9,-0.0583 -1.934
-00002db0: 3330 312c 2d31 2e34 3537 3835 202d 332e  301,-1.45785 -3.
-00002dc0: 3636 3334 3635 2c2d 312e 3435 3630 3220  663465,-1.45602 
-00002dd0: 2d32 2e30 3832 3037 312c 302e 3030 3220  -2.082071,0.002 
-00002de0: 2d33 2e31 3536 3438 392c 312e 3336 3934  -3.156489,1.3694
-00002df0: 3320 2d33 2e39 3739 3035 362c 322e 3537  3 -3.979056,2.57
-00002e00: 3533 3720 2d31 2e30 3735 3338 392c 312e  537 -1.075389,1.
-00002e10: 3537 3635 3820 2d31 2e31 3232 3634 342c  57658 -1.122644,
-00002e20: 332e 3837 3935 3920 2d30 2e31 3439 3931  3.87959 -0.14991
-00002e30: 322c 352e 3532 3031 3620 302e 3836 3139  2,5.52016 0.8619
-00002e40: 342c 312e 3435 3337 3120 322e 3535 3335  4,1.45371 2.5535
-00002e50: 3931 2c31 2e39 3731 3137 2034 2e31 3532  91,1.97117 4.152
-00002e60: 3233 342c 322e 3031 3930 3220 312e 3236  234,2.01902 1.26
-00002e70: 3435 3431 2c30 2e30 3337 3920 342e 3033  4541,0.0379 4.03
-00002e80: 3932 3937 2c2d 312e 3632 3331 2034 2e30  9297,-1.6231 4.0
-00002e90: 3339 3239 372c 2d31 2e36 3233 3122 0a20  39297,-1.6231". 
-00002ea0: 2020 2020 2020 6964 3d22 7061 7468 3136        id="path16
-00002eb0: 3331 392d 3722 0a20 2020 2020 2020 736f  319-7".       so
-00002ec0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00002ed0: 3d22 6373 7373 7363 2220 2f3e 0a20 2020  ="cssssc" />.   
-00002ee0: 203c 7573 650a 2020 2020 2020 2078 3d22   <use.       x="
-00002ef0: 3022 0a20 2020 2020 2020 793d 2230 220a  0".       y="0".
-00002f00: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-00002f10: 663d 2223 7061 7468 3839 3835 2d38 220a  f="#path8985-8".
-00002f20: 2020 2020 2020 2069 643d 2275 7365 3334         id="use34
-00002f30: 3922 0a20 2020 2020 2020 7472 616e 7366  9".       transf
-00002f40: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
-00002f50: 362e 3836 3139 3339 2c33 382e 3133 3236  6.861939,38.1326
-00002f60: 3538 2922 202f 3e0a 2020 2020 3c70 6174  58)" />.    <pat
-00002f70: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-00002f80: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-00002f90: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00002fa0: 7769 6474 683a 302e 3236 3435 3833 7078  width:0.264583px
-00002fb0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00002fc0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00002fd0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00002fe0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00002ff0: 2020 2020 643d 224d 2032 382e 3931 3239      d="M 28.9129
-00003000: 3634 2c32 3734 2e32 3034 3634 2048 2031  64,274.20464 H 1
-00003010: 3836 2e33 3335 3638 220a 2020 2020 2020  86.33568".      
-00003020: 2069 643d 2270 6174 6838 3935 312d 3622   id="path8951-6"
-00003030: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
-00003040: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00003050: 7061 6369 7479 3a30 2e39 393b 6669 6c6c  pacity:0.99;fill
-00003060: 3a23 3866 6430 6466 3b66 696c 6c2d 6f70  :#8fd0df;fill-op
-00003070: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-00003080: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-00003090: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000030a0: 7769 6474 683a 312e 3538 3735 652d 3038  width:1.5875e-08
-000030b0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000030c0: 726f 756e 643b 7374 726f 6b65 2d6c 696e  round;stroke-lin
-000030d0: 656a 6f69 6e3a 726f 756e 643b 7374 726f  ejoin:round;stro
-000030e0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-000030f0: 2020 2020 2069 643d 2270 6174 6838 3938       id="path898
-00003100: 3522 0a20 2020 2020 2020 6378 3d22 3137  5".       cx="17
-00003110: 352e 3937 3636 3122 0a20 2020 2020 2020  5.97661".       
-00003120: 6379 3d22 3135 332e 3533 3036 3422 0a20  cy="153.53064". 
-00003130: 2020 2020 2020 7278 3d22 312e 3939 3432        rx="1.9942
-00003140: 3230 3122 0a20 2020 2020 2020 7279 3d22  201".       ry="
-00003150: 322e 3332 3831 3431 220a 2020 2020 2020  2.328141".      
-00003160: 2074 7261 6e73 666f 726d 3d22 726f 7461   transform="rota
-00003170: 7465 2834 302e 3233 3732 3431 2922 202f  te(40.237241)" /
-00003180: 3e0a 2020 2020 3c75 7365 0a20 2020 2020  >.    <use.     
-00003190: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
-000031a0: 3d22 3022 0a20 2020 2020 2020 786c 696e  ="0".       xlin
-000031b0: 6b3a 6872 6566 3d22 2370 6174 6838 3938  k:href="#path898
-000031c0: 3522 0a20 2020 2020 2020 6964 3d22 7573  5".       id="us
-000031d0: 6531 3838 3131 220a 2020 2020 2020 2074  e18811".       t
-000031e0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000031f0: 6174 6528 332e 3730 3036 3436 322c 3333  ate(3.7006462,33
-00003200: 2e38 3934 3636 3129 2220 2f3e 0a20 2020  .894661)" />.   
-00003210: 203c 7573 650a 2020 2020 2020 2078 3d22   <use.       x="
-00003220: 3022 0a20 2020 2020 2020 793d 2230 220a  0".       y="0".
-00003230: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-00003240: 663d 2223 7061 7468 3839 3835 220a 2020  f="#path8985".  
-00003250: 2020 2020 2069 643d 2275 7365 3138 3831       id="use1881
-00003260: 3522 0a20 2020 2020 2020 7472 616e 7366  5".       transf
-00003270: 6f72 6d3d 2274 7261 6e73 6c61 7465 2834  orm="translate(4
-00003280: 2e32 3436 3436 3437 2c31 382e 3538 3931  .2464647,18.5891
-00003290: 3932 2922 202f 3e0a 2020 2020 3c70 6174  92)" />.    <pat
-000032a0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-000032b0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-000032c0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000032d0: 7769 6474 683a 302e 3236 3435 3833 7078  width:0.264583px
-000032e0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000032f0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00003300: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00003310: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00003320: 2020 2020 643d 226d 2035 322e 3931 3431      d="m 52.9141
-00003330: 3935 2c32 3438 2e39 3330 3732 2063 202d  95,248.93072 c -
-00003340: 302e 3433 3035 3131 2c2d 302e 3133 3837  0.430511,-0.1387
-00003350: 202d 322e 3438 3031 3736 2c2d 312e 3936   -2.480176,-1.96
-00003360: 3236 3620 2d37 2e30 3331 3534 2c2d 312e  266 -7.03154,-1.
-00003370: 3936 3236 3620 2d32 2e36 3537 3633 382c  96266 -2.657638,
-00003380: 3020 2d36 2e35 3337 3732 342c 312e 3533  0 -6.537724,1.53
-00003390: 3938 3720 2d37 2e37 3632 3931 382c 342e  987 -7.762918,4.
-000033a0: 3236 3433 3320 2d31 2e38 3132 3432 332c  26433 -1.812423,
-000033b0: 342e 3033 3032 3920 2d32 2e30 3436 3736  4.03029 -2.04676
-000033c0: 382c 3130 2e30 3134 3438 2030 2e35 3536  8,10.01448 0.556
-000033d0: 3433 382c 3133 2e35 3334 3339 2031 2e35  438,13.53439 1.5
-000033e0: 3035 3635 382c 322e 3033 3538 3720 342e  05658,2.03587 4.
-000033f0: 3534 3936 362c 322e 3336 3430 3220 372e  54966,2.36402 7.
-00003400: 3033 3736 332c 322e 3336 3430 3220 322e  03763,2.36402 2.
-00003410: 3734 3530 3334 2c30 2036 2e39 3836 3632  745034,0 6.98662
-00003420: 362c 2d31 2e36 3537 3237 2036 2e39 3836  6,-1.65727 6.986
-00003430: 3632 362c 2d31 2e36 3537 3237 220a 2020  626,-1.65727".  
-00003440: 2020 2020 2069 643d 2270 6174 6831 3633       id="path163
-00003450: 3139 220a 2020 2020 2020 2073 6f64 6970  19".       sodip
-00003460: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-00003470: 7373 7373 6322 202f 3e0a 2020 2020 3c75  ssssc" />.    <u
-00003480: 7365 0a20 2020 2020 2020 783d 2230 220a  se.       x="0".
-00003490: 2020 2020 2020 2079 3d22 3022 0a20 2020         y="0".   
-000034a0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
-000034b0: 2370 6174 6838 3938 352d 3822 0a20 2020  #path8985-8".   
-000034c0: 2020 2020 6964 3d22 7573 6533 3437 220a      id="use347".
-000034d0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-000034e0: 3d22 7472 616e 736c 6174 6528 3135 2e34  ="translate(15.4
-000034f0: 3137 3030 372c 3231 2e30 3532 3138 3229  17007,21.052182)
-00003500: 2220 2f3e 0a20 2020 203c 7573 650a 2020  " />.    <use.  
-00003510: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
-00003520: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
-00003530: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
-00003540: 3839 3835 2d38 220a 2020 2020 2020 2069  8985-8".       i
-00003550: 643d 2275 7365 3430 3222 0a20 2020 2020  d="use402".     
-00003560: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00003570: 6e73 6c61 7465 2831 382e 3134 3032 3933  nslate(18.140293
-00003580: 2c32 372e 3137 3639 3235 2922 202f 3e0a  ,27.176925)" />.
-00003590: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-000035a0: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-000035b0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-000035c0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000035d0: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
-000035e0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000035f0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00003600: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00003610: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00003620: 2038 362e 3435 3530 3835 2c32 3535 2e37   86.455085,255.7
-00003630: 3834 3720 362e 3033 3234 3734 2c31 332e  847 6.032474,13.
-00003640: 3237 3130 3322 0a20 2020 2020 2020 6964  27103".       id
-00003650: 3d22 7061 7468 3137 3037 392d 352d 3522  ="path17079-5-5"
-00003660: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00003670: 3a6e 6f64 6574 7970 6573 3d22 6363 2220  :nodetypes="cc" 
-00003680: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00003690: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-000036a0: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
-000036b0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-000036c0: 3a30 2e32 3634 3538 3370 783b 7374 726f  :0.264583px;stro
-000036d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000036e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000036f0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
-00003700: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00003710: 3d22 6d20 3935 2e33 3634 3737 392c 3235  ="m 95.364779,25
-00003720: 352e 3835 3631 3720 6320 302c 3020 2d32  5.85617 c 0,0 -2
-00003730: 2e32 3037 3739 372c 3130 2e36 3138 3535  .207797,10.61855
-00003740: 202d 342e 3231 3635 3931 2c31 352e 3333   -4.216591,15.33
-00003750: 3934 3820 2d30 2e37 3332 3932 362c 312e  948 -0.732926,1.
-00003760: 3732 3234 3720 2d31 2e39 3531 3634 362c  72247 -1.951646,
-00003770: 322e 3337 3434 202d 332e 3632 3532 392c  2.3744 -3.62529,
-00003780: 322e 3234 3738 3822 0a20 2020 2020 2020  2.24788".       
-00003790: 6964 3d22 7061 7468 3137 3037 392d 352d  id="path17079-5-
-000037a0: 3622 0a20 2020 2020 2020 736f 6469 706f  6".       sodipo
-000037b0: 6469 3a6e 6f64 6574 7970 6573 3d22 6373  di:nodetypes="cs
-000037c0: 6322 202f 3e0a 2020 2020 3c70 6174 680a  c" />.    <path.
-000037d0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000037e0: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
-000037f0: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-00003800: 6474 683a 302e 3236 3435 3833 7078 3b73  dth:0.264583px;s
-00003810: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003820: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003830: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00003840: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00003850: 2020 643d 226d 2031 3030 2e34 3731 3332    d="m 100.47132
-00003860: 2c32 3436 2e36 3139 3432 2063 2030 2e32  ,246.61942 c 0.2
-00003870: 3531 3139 2c2d 302e 3037 3431 2033 2e35  5119,-0.0741 3.5
-00003880: 3533 3034 2c2d 302e 3432 3139 2035 2e32  5304,-0.4219 5.2
-00003890: 3036 3735 2c2d 302e 3039 3738 2031 2e35  0675,-0.0978 1.5
-000038a0: 3136 3331 2c30 2e32 3937 3139 2033 2e30  1631,0.29719 3.0
-000038b0: 3734 3734 2c31 2e33 3639 3639 2033 2e37  7474,1.36969 3.7
-000038c0: 3839 3632 2c32 2e38 3234 3835 2031 2e30  8962,2.82485 1.0
-000038d0: 3537 3531 2c32 2e31 3532 3632 2030 2e38  5751,2.15262 0.8
-000038e0: 3936 3938 2c35 2e33 3033 3838 202d 302e  9698,5.30388 -0.
-000038f0: 3331 3337 342c 372e 3336 3238 3620 2d30  31374,7.36286 -0
-00003900: 2e37 3639 3033 2c31 2e33 3037 3833 202d  .76903,1.30783 -
-00003910: 322e 3437 3738 312c 312e 3833 3636 3820  2.47781,1.83668 
-00003920: 2d33 2e39 3138 2c32 2e30 3033 3534 202d  -3.918,2.00354 -
-00003930: 312e 3531 3336 392c 302e 3137 3533 3620  1.51369,0.17536 
-00003940: 2d34 2e30 3533 3835 2c30 2e31 3238 3133  -4.05385,0.12813
-00003950: 202d 342e 3035 3338 352c 302e 3132 3831   -4.05385,0.1281
-00003960: 3322 0a20 2020 2020 2020 6964 3d22 7061  3".       id="pa
-00003970: 7468 3136 3331 392d 372d 332d 3922 0a20  th16319-7-3-9". 
-00003980: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00003990: 6f64 6574 7970 6573 3d22 6373 7373 7363  odetypes="cssssc
-000039a0: 2220 2f3e 0a20 2020 203c 7573 650a 2020  " />.    <use.  
-000039b0: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
-000039c0: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
-000039d0: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
-000039e0: 3839 3835 2d38 220a 2020 2020 2020 2069  8985-8".       i
-000039f0: 643d 2275 7365 3533 3922 0a20 2020 2020  d="use539".     
-00003a00: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00003a10: 6e73 6c61 7465 2835 342e 3838 3938 3433  nslate(54.889843
-00003a20: 2c31 322e 3832 3537 3931 2922 202f 3e0a  ,12.825791)" />.
-00003a30: 2020 2020 3c75 7365 0a20 2020 2020 2020      <use.       
-00003a40: 783d 2230 220a 2020 2020 2020 2079 3d22  x="0".       y="
-00003a50: 3022 0a20 2020 2020 2020 786c 696e 6b3a  0".       xlink:
-00003a60: 6872 6566 3d22 2370 6174 6838 3938 352d  href="#path8985-
-00003a70: 3822 0a20 2020 2020 2020 6964 3d22 7573  8".       id="us
-00003a80: 6535 3431 220a 2020 2020 2020 2074 7261  e541".       tra
-00003a90: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00003aa0: 6528 3436 2e36 3436 3938 372c 3131 2e31  e(46.646987,11.1
-00003ab0: 3437 3234 3329 2220 2f3e 0a20 2020 203c  47243)" />.    <
-00003ac0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00003ad0: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
-00003ae0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00003af0: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
-00003b00: 3370 783b 7374 726f 6b65 2d6c 696e 6563  3px;stroke-linec
-00003b10: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00003b20: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00003b30: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00003b40: 2020 2020 2020 2064 3d22 6d20 3131 362e         d="m 116.
-00003b50: 3136 3133 342c 3234 362e 3534 3433 3420  16134,246.54434 
-00003b60: 6320 302e 3235 3131 392c 2d30 2e30 3734  c 0.25119,-0.074
-00003b70: 3120 332e 3535 3330 352c 2d30 2e34 3231  1 3.55305,-0.421
-00003b80: 3920 352e 3230 3637 372c 2d30 2e30 3937  9 5.20677,-0.097
-00003b90: 3820 312e 3531 3633 312c 302e 3239 3731  8 1.51631,0.2971
-00003ba0: 3920 342e 3930 3831 2c2d 302e 3231 3832  9 4.9081,-0.2182
-00003bb0: 2035 2e35 3839 3435 2c32 2e37 3230 3932   5.58945,2.72092
-00003bc0: 2030 2e35 3431 3632 2c32 2e33 3336 3420   0.54162,2.3364 
-00003bd0: 302e 3732 3831 392c 3134 2e39 3938 3531  0.72819,14.99851
-00003be0: 202d 302e 3237 3832 332c 3137 2e31 3634   -0.27823,17.164
-00003bf0: 3639 202d 312e 3033 3635 322c 322e 3233  69 -1.03652,2.23
-00003c00: 3039 3420 2d33 2e38 3830 3132 2c32 2e30  094 -3.88012,2.0
-00003c10: 3936 3333 202d 352e 3332 3033 312c 322e  9633 -5.32031,2.
-00003c20: 3236 3331 3920 2d31 2e35 3133 3639 2c30  26319 -1.51369,0
-00003c30: 2e31 3735 3336 202d 342e 3636 3933 322c  .17536 -4.66932,
-00003c40: 2d30 2e31 3132 3732 202d 342e 3636 3933  -0.11272 -4.6693
-00003c50: 322c 2d30 2e31 3132 3732 220a 2020 2020  2,-0.11272".    
-00003c60: 2020 2069 643d 2270 6174 6831 3633 3139     id="path16319
-00003c70: 2d37 2d33 2d39 2d32 220a 2020 2020 2020  -7-3-9-2".      
-00003c80: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00003c90: 7065 733d 2263 7373 7373 6322 202f 3e0a  pes="cssssc" />.
-00003ca0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00003cb0: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-00003cc0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-00003cd0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00003ce0: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
-00003cf0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00003d00: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00003d10: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00003d20: 793a 3122 0a20 2020 2020 2020 643d 224d  y:1".       d="M
-00003d30: 2031 3336 2e37 3532 3138 2c32 3437 2e32   136.75218,247.2
-00003d40: 3136 3831 2048 2031 3438 2e32 3533 3422  1681 H 148.2534"
-00003d50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00003d60: 3137 3037 392d 352d 322d 3022 202f 3e0a  17079-5-2-0" />.
-00003d70: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00003d80: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-00003d90: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-00003da0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00003db0: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
-00003dc0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00003dd0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00003de0: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00003df0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00003e00: 2031 3336 2e36 3635 3332 2c32 3536 2e36   136.66532,256.6
-00003e10: 3638 3432 2068 2038 2e36 3639 3634 220a  6842 h 8.66964".
-00003e20: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00003e30: 3730 3739 2d35 2d32 2d30 2d39 2220 2f3e  7079-5-2-0-9" />
-00003e40: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00003e50: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
-00003e60: 6666 6666 663b 6669 6c6c 2d6f 7061 6369  fffff;fill-opaci
-00003e70: 7479 3a30 2e33 3234 3834 3b73 7472 6f6b  ty:0.32484;strok
-00003e80: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00003e90: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
-00003ea0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00003eb0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00003ec0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00003ed0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00003ee0: 2020 2020 2064 3d22 6d20 3533 2e37 3839       d="m 53.789
-00003ef0: 3131 312c 3234 362e 3830 3434 3120 2d31  111,246.80441 -1
-00003f00: 2e37 3336 3937 332c 342e 3035 3834 3820  .736973,4.05848 
-00003f10: 6320 2d31 2e38 3933 3930 392c 2d30 2e37  c -1.893909,-0.7
-00003f20: 3438 3233 202d 342e 3138 3432 3736 2c2d  4823 -4.184276,-
-00003f30: 312e 3736 3330 3720 2d36 2e33 3831 3336  1.76307 -6.38136
-00003f40: 312c 2d31 2e36 3732 3339 202d 312e 3731  1,-1.67239 -1.71
-00003f50: 3739 352c 302e 3037 3039 202d 332e 3536  795,0.0709 -3.56
-00003f60: 3534 3439 2c30 2e35 3131 3735 202d 342e  5449,0.51175 -4.
-00003f70: 3734 3834 3133 2c31 2e37 3539 3534 202d  748413,1.75954 -
-00003f80: 312e 3439 3838 3039 2c31 2e35 3830 3934  1.498809,1.58094
-00003f90: 202d 312e 3930 3734 3335 2c34 2e30 3437   -1.907435,4.047
-00003fa0: 3838 202d 312e 3935 3730 3935 2c36 2e32  88 -1.957095,6.2
-00003fb0: 3235 3820 2d30 2e30 3438 3431 2c32 2e31  258 -0.04841,2.1
-00003fc0: 3232 3920 302e 3035 3832 392c 342e 3337  229 0.05829,4.37
-00003fd0: 3832 3720 312e 3533 3638 3438 2c35 2e39  827 1.536848,5.9
-00003fe0: 3032 3339 2031 2e37 3231 3631 372c 312e  0239 1.721617,1.
-00003ff0: 3737 3436 3620 332e 3838 3838 3636 2c31  77466 3.888866,1
-00004000: 2e37 3232 3537 2034 2e39 3236 3530 392c  .72257 4.926509,
-00004010: 312e 3737 3234 3120 322e 3035 3232 3739  1.77241 2.052279
-00004020: 2c30 2e30 3938 3620 342e 3337 3334 3231  ,0.0986 4.373421
-00004030: 2c2d 302e 3633 3435 3820 362e 3237 3537  ,-0.63458 6.2757
-00004040: 3932 2c2d 312e 3137 3932 3720 6c20 312e  92,-1.17927 l 1.
-00004050: 3635 3737 3939 2c33 2e38 3331 3336 2063  657799,3.83136 c
-00004060: 202d 322e 3431 3434 392c 312e 3037 3439   -2.41449,1.0749
-00004070: 3920 2d35 2e34 3332 3339 382c 312e 3537  9 -5.432398,1.57
-00004080: 3038 3820 2d38 2e32 3733 3935 332c 312e  088 -8.273953,1.
-00004090: 3632 3439 3920 2d32 2e37 3332 3938 392c  62499 -2.732989,
-000040a0: 302e 3035 3220 2d36 2e30 3031 3534 372c  0.052 -6.001547,
-000040b0: 2d30 2e36 3339 3633 202d 372e 3838 3331  -0.63963 -7.8831
-000040c0: 3432 2c2d 322e 3632 3234 3420 2d32 2e30  42,-2.62244 -2.0
-000040d0: 3530 3539 322c 2d32 2e31 3630 3920 2d32  50592,-2.1609 -2
-000040e0: 2e35 3736 3738 342c 2d35 2e36 3033 3132  .576784,-5.60312
-000040f0: 202d 322e 3439 3730 3532 2c2d 382e 3538   -2.497052,-8.58
-00004100: 3130 3520 302e 3039 3632 372c 2d33 2e35  105 0.09627,-3.5
-00004110: 3935 3735 2031 2e30 3336 3036 322c 2d37  9575 1.036062,-7
-00004120: 2e36 3237 3431 2033 2e35 3635 3232 322c  .62741 3.565222,
-00004130: 2d31 302e 3138 3531 3420 312e 3933 3831  -10.18514 1.9381
-00004140: 3235 2c2d 312e 3936 3030 3220 352e 3032  25,-1.96002 5.02
-00004150: 3134 362c 2d32 2e36 3639 3235 2037 2e37  146,-2.66925 7.7
-00004160: 3733 3830 372c 2d32 2e38 3139 3538 2032  73807,-2.81958 2
-00004170: 2e36 3532 3130 312c 2d30 2e31 3434 3835  .652101,-0.14485
-00004180: 2035 2e39 3132 3133 352c 312e 3132 3633   5.912135,1.1263
-00004190: 3220 372e 3734 3230 3132 2c31 2e38 3834  2 7.742012,1.884
-000041a0: 3920 7a22 0a20 2020 2020 2020 6964 3d22  9 z".       id="
-000041b0: 7061 7468 3138 3835 3322 0a20 2020 2020  path18853".     
-000041c0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-000041d0: 7970 6573 3d22 6363 7373 7373 7363 6373  ypes="ccsssssccs
-000041e0: 7373 7373 6322 202f 3e0a 2020 2020 3c70  ssssc" />.    <p
-000041f0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-00004200: 3d22 6669 6c6c 3a6e 6f6e 653b 6669 6c6c  ="fill:none;fill
-00004210: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00004220: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00004230: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
-00004240: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00004250: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00004260: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00004270: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00004280: 2020 2020 2064 3d22 6d20 3635 2e35 3038       d="m 65.508
-00004290: 3034 372c 3235 372e 3439 3539 3520 6320  047,257.49595 c 
-000042a0: 302c 3020 2d31 2e33 3731 3239 312c 2d32  0,0 -1.371291,-2
-000042b0: 2e31 3037 3834 202d 342e 3236 3737 3531  .10784 -4.267751
-000042c0: 2c2d 322e 3038 3332 3120 2d32 2e39 3132  ,-2.08321 -2.912
-000042d0: 3136 312c 302e 3032 3438 202d 342e 3933  161,0.0248 -4.93
-000042e0: 3032 3639 2c32 2e36 3430 3833 202d 352e  0269,2.64083 -5.
-000042f0: 3638 3037 3939 2c34 2e34 3639 3334 202d  680799,4.46934 -
-00004300: 302e 3635 3538 3132 2c31 2e35 3937 3735  0.655812,1.59775
-00004310: 202d 302e 3432 3532 3932 2c35 2e35 3831   -0.425292,5.581
-00004320: 3137 2030 2e38 3431 3832 312c 362e 3936  17 0.841821,6.96
-00004330: 3433 3520 312e 3130 3036 3839 2c31 2e32  435 1.100689,1.2
-00004340: 3031 3531 2031 2e39 3037 3835 2c32 2e31  0151 1.90785,2.1
-00004350: 3230 3136 2034 2e37 3139 3231 312c 322e  2016 4.719211,2.
-00004360: 3134 3836 3420 322e 3239 3430 3633 2c30  14864 2.294063,0
-00004370: 2e30 3233 3220 342e 3439 3136 3139 2c2d  .0232 4.491619,-
-00004380: 312e 3939 3832 3220 342e 3439 3136 3139  1.99822 4.491619
-00004390: 2c2d 312e 3939 3832 3220 6c20 2d30 2e37  ,-1.99822 l -0.7
-000043a0: 3233 3335 342c 2d32 2e34 3936 3739 2063  23354,-2.49679 c
-000043b0: 2030 2c30 202d 312e 3837 3936 3338 2c31   0,0 -1.879638,1
-000043c0: 2e33 3334 3836 202d 332e 3536 3433 3234  .33486 -3.564324
-000043d0: 2c31 2e33 3434 3239 202d 312e 3532 3139  ,1.34429 -1.5219
-000043e0: 3538 2c30 2e30 3039 202d 322e 3135 3731  58,0.009 -2.1571
-000043f0: 3031 2c2d 302e 3836 3732 202d 322e 3633  01,-0.8672 -2.63
-00004400: 3530 3035 2c2d 312e 3531 3331 202d 302e  5005,-1.5131 -0.
-00004410: 3636 3136 3139 2c2d 302e 3839 3431 3920  661619,-0.89419 
-00004420: 2d30 2e35 3738 3339 332c 2d32 2e38 3232  -0.578393,-2.822
-00004430: 3038 202d 302e 3032 3231 332c 2d33 2e37  08 -0.02213,-3.7
-00004440: 3835 3336 2030 2e33 3832 3731 352c 2d30  8536 0.382715,-0
-00004450: 2e36 3632 3735 2031 2e35 3731 3634 322c  .66275 1.571642,
-00004460: 2d31 2e38 3834 3036 2032 2e36 3533 3236  -1.88406 2.65326
-00004470: 332c 2d31 2e38 3439 3935 2031 2e38 3435  3,-1.84995 1.845
-00004480: 3738 2c30 2e30 3538 3220 322e 3831 3739  78,0.0582 2.8179
-00004490: 3035 2c30 2e38 3831 3637 2033 2e37 3630  05,0.88167 3.760
-000044a0: 3133 362c 312e 3631 3330 3120 7a22 0a20  136,1.61301 z". 
-000044b0: 2020 2020 2020 6964 3d22 7061 7468 3230        id="path20
-000044c0: 3336 3122 0a20 2020 2020 2020 736f 6469  361".       sodi
-000044d0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-000044e0: 6373 7373 7363 6373 7373 7363 6322 202f  cssssccsssscc" /
-000044f0: 3e0a 2020 2020 3c72 6563 740a 2020 2020  >.    <rect.    
-00004500: 2020 2073 7479 6c65 3d22 6f70 6163 6974     style="opacit
-00004510: 793a 302e 3939 3b66 696c 6c3a 2366 6666  y:0.99;fill:#fff
-00004520: 6666 663b 6669 6c6c 2d6f 7061 6369 7479  fff;fill-opacity
-00004530: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00004540: 7a65 726f 3b73 7472 6f6b 653a 2330 3030  zero;stroke:#000
-00004550: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00004560: 3a30 2e33 3b73 7472 6f6b 652d 6c69 6e65  :0.3;stroke-line
-00004570: 6361 703a 726f 756e 643b 7374 726f 6b65  cap:round;stroke
-00004580: 2d6c 696e 656a 6f69 6e3a 726f 756e 643b  -linejoin:round;
-00004590: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-000045a0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-000045b0: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-000045c0: 643d 2272 6563 7432 3034 3135 220a 2020  d="rect20415".  
-000045d0: 2020 2020 2077 6964 7468 3d22 332e 3432       width="3.42
-000045e0: 3033 3238 3122 0a20 2020 2020 2020 6865  03281".       he
-000045f0: 6967 6874 3d22 3133 2e36 3936 3831 3522  ight="13.696815"
-00004600: 0a20 2020 2020 2020 783d 2236 342e 3636  .       x="64.66
-00004610: 3435 3937 220a 2020 2020 2020 2079 3d22  4597".       y="
-00004620: 3235 352e 3334 3237 3422 202f 3e0a 2020  255.34274" />.  
-00004630: 2020 3c72 6563 740a 2020 2020 2020 2073    <rect.       s
-00004640: 7479 6c65 3d22 6f70 6163 6974 793a 302e  tyle="opacity:0.
-00004650: 3939 3b66 696c 6c3a 6e6f 6e65 3b66 696c  99;fill:none;fil
-00004660: 6c2d 6f70 6163 6974 793a 302e 3332 3438  l-opacity:0.3248
-00004670: 343b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  4;fill-rule:nonz
-00004680: 6572 6f3b 7374 726f 6b65 3a23 3030 3030  ero;stroke:#0000
-00004690: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-000046a0: 302e 333b 7374 726f 6b65 2d6c 696e 6563  0.3;stroke-linec
-000046b0: 6170 3a72 6f75 6e64 3b73 7472 6f6b 652d  ap:round;stroke-
-000046c0: 6c69 6e65 6a6f 696e 3a72 6f75 6e64 3b73  linejoin:round;s
-000046d0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-000046e0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-000046f0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
-00004700: 3d22 7265 6374 3230 3632 3522 0a20 2020  ="rect20625".   
-00004710: 2020 2020 7769 6474 683d 2230 2e30 3538      width="0.058
-00004720: 3036 3839 3031 220a 2020 2020 2020 2068  068901".       h
-00004730: 6569 6768 743d 2230 2e31 3239 3034 3035  eight="0.1290405
-00004740: 3422 0a20 2020 2020 2020 783d 2237 392e  4".       x="79.
-00004750: 3836 3038 3535 220a 2020 2020 2020 2079  860855".       y
-00004760: 3d22 3234 392e 3830 3036 3322 202f 3e0a  ="249.80063" />.
-00004770: 2020 2020 3c74 6578 740a 2020 2020 2020      <text.      
-00004780: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00004790: 6572 7665 220a 2020 2020 2020 2073 7479  erve".       sty
-000047a0: 6c65 3d22 666f 6e74 2d73 7479 6c65 3a6e  le="font-style:n
-000047b0: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
-000047c0: 6e74 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  nt:normal;font-w
-000047d0: 6569 6768 743a 6e6f 726d 616c 3b66 6f6e  eight:normal;fon
-000047e0: 742d 7374 7265 7463 683a 6e6f 726d 616c  t-stretch:normal
-000047f0: 3b66 6f6e 742d 7369 7a65 3a32 352e 3838  ;font-size:25.88
-00004800: 3337 7078 3b6c 696e 652d 6865 6967 6874  37px;line-height
-00004810: 3a31 2e32 353b 666f 6e74 2d66 616d 696c  :1.25;font-famil
-00004820: 793a 5562 756e 7475 3b2d 696e 6b73 6361  y:Ubuntu;-inksca
-00004830: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
-00004840: 6174 696f 6e3a 5562 756e 7475 3b6c 6574  ation:Ubuntu;let
-00004850: 7465 722d 7370 6163 696e 673a 3070 783b  ter-spacing:0px;
-00004860: 776f 7264 2d73 7061 6369 6e67 3a30 7078  word-spacing:0px
-00004870: 3b66 696c 6c3a 2330 3030 3030 303b 6669  ;fill:#000000;fi
-00004880: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00004890: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-000048a0: 7769 6474 683a 302e 3330 3333 3234 220a  width:0.303324".
-000048b0: 2020 2020 2020 2078 3d22 3632 2e33 3230         x="62.320
-000048c0: 3237 3422 0a20 2020 2020 2020 793d 2231  274".       y="1
-000048d0: 3330 2e38 3633 3432 220a 2020 2020 2020  30.86342".      
-000048e0: 2069 643d 2274 6578 7432 3036 3831 223e   id="text20681">
-000048f0: 3c74 7370 616e 0a20 2020 2020 2020 2020  <tspan.         
-00004900: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
-00004910: 696e 6522 0a20 2020 2020 2020 2020 6964  ine".         id
-00004920: 3d22 7473 7061 6e32 3036 3739 220a 2020  ="tspan20679".  
-00004930: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
-00004940: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
-00004950: 666f 6e74 2d76 6172 6961 6e74 3a6e 6f72  font-variant:nor
-00004960: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
-00004970: 626f 6c64 3b66 6f6e 742d 7374 7265 7463  bold;font-stretc
-00004980: 683a 6e6f 726d 616c 3b66 6f6e 742d 7369  h:normal;font-si
-00004990: 7a65 3a32 352e 3838 3337 7078 3b66 6f6e  ze:25.8837px;fon
-000049a0: 742d 6661 6d69 6c79 3a27 4e69 6d62 7573  t-family:'Nimbus
-000049b0: 2053 616e 7327 3b2d 696e 6b73 6361 7065   Sans';-inkscape
-000049c0: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
-000049d0: 696f 6e3a 274e 696d 6275 7320 5361 6e73  ion:'Nimbus Sans
-000049e0: 2042 6f6c 6427 3b73 7472 6f6b 652d 7769   Bold';stroke-wi
-000049f0: 6474 683a 302e 3330 3333 3234 220a 2020  dth:0.303324".  
-00004a00: 2020 2020 2020 2078 3d22 3632 2e33 3230         x="62.320
-00004a10: 3237 3422 0a20 2020 2020 2020 2020 793d  274".         y=
-00004a20: 2231 3330 2e38 3633 3432 223e 4361 7079  "130.86342">Capy
-00004a30: 5044 463c 2f74 7370 616e 3e3c 2f74 6578  PDF</tspan></tex
-00004a40: 743e 0a20 2020 203c 656c 6c69 7073 650a  t>.    <ellipse.
-00004a50: 2020 2020 2020 2073 7479 6c65 3d22 6f70         style="op
-00004a60: 6163 6974 793a 302e 3939 3b66 696c 6c3a  acity:0.99;fill:
-00004a70: 2338 6664 3064 663b 6669 6c6c 2d6f 7061  #8fd0df;fill-opa
-00004a80: 6369 7479 3a31 3b66 696c 6c2d 7275 6c65  city:1;fill-rule
-00004a90: 3a6e 6f6e 7a65 726f 3b73 7472 6f6b 653a  :nonzero;stroke:
-00004aa0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-00004ab0: 6964 7468 3a31 2e35 3837 3565 2d30 383b  idth:1.5875e-08;
-00004ac0: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
-00004ad0: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
-00004ae0: 6a6f 696e 3a72 6f75 6e64 3b73 7472 6f6b  join:round;strok
-00004af0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00004b00: 2020 2020 6964 3d22 7061 7468 3839 3835      id="path8985
-00004b10: 2d38 220a 2020 2020 2020 2063 783d 2232  -8".       cx="2
-00004b20: 3036 2e34 3633 3638 220a 2020 2020 2020  06.46368".      
-00004b30: 2063 793d 2231 3333 2e35 3831 3031 220a   cy="133.58101".
-00004b40: 2020 2020 2020 2072 783d 2231 2e34 3735         rx="1.475
-00004b50: 3630 3634 220a 2020 2020 2020 2072 793d  6064".       ry=
-00004b60: 2231 2e37 3232 3638 3834 220a 2020 2020  "1.7226884".    
-00004b70: 2020 2074 7261 6e73 666f 726d 3d22 726f     transform="ro
-00004b80: 7461 7465 2834 302e 3233 3732 3431 2922  tate(40.237241)"
-00004b90: 202f 3e0a 2020 2020 3c75 7365 0a20 2020   />.    <use.   
-00004ba0: 2020 2020 783d 2230 220a 2020 2020 2020      x="0".      
-00004bb0: 2079 3d22 3022 0a20 2020 2020 2020 786c   y="0".       xl
-00004bc0: 696e 6b3a 6872 6566 3d22 2370 6174 6838  ink:href="#path8
-00004bd0: 3938 352d 3822 0a20 2020 2020 2020 6964  985-8".       id
-00004be0: 3d22 7573 6532 3630 3036 220a 2020 2020  ="use26006".    
-00004bf0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00004c00: 616e 736c 6174 6528 322e 3131 3235 3232  anslate(2.112522
-00004c10: 322c 3233 2e36 3732 3536 3329 2220 2f3e  2,23.672563)" />
-00004c20: 0a20 2020 203c 7265 6374 0a20 2020 2020  .    <rect.     
-00004c30: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
-00004c40: 3a30 2e39 393b 6669 6c6c 3a6e 6f6e 653b  :0.99;fill:none;
-00004c50: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00004c60: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00004c70: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00004c80: 7374 726f 6b65 2d77 6964 7468 3a30 2e33  stroke-width:0.3
-00004c90: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00004ca0: 726f 756e 643b 7374 726f 6b65 2d6c 696e  round;stroke-lin
-00004cb0: 656a 6f69 6e3a 726f 756e 643b 7374 726f  ejoin:round;stro
-00004cc0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00004cd0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00004ce0: 3a31 220a 2020 2020 2020 2069 643d 2272  :1".       id="r
-00004cf0: 6563 7432 3034 3135 2d35 220a 2020 2020  ect20415-5".    
-00004d00: 2020 2077 6964 7468 3d22 332e 3432 3033     width="3.4203
-00004d10: 3238 3122 0a20 2020 2020 2020 6865 6967  281".       heig
-00004d20: 6874 3d22 3138 2e36 3037 3132 3122 0a20  ht="18.607121". 
-00004d30: 2020 2020 2020 783d 2237 302e 3438 3331        x="70.4831
-00004d40: 3722 0a20 2020 2020 2020 793d 2232 3535  7".       y="255
-00004d50: 2e33 3636 3733 2220 2f3e 0a20 2020 203c  .36673" />.    <
-00004d60: 7573 650a 2020 2020 2020 2078 3d22 3022  use.       x="0"
-00004d70: 0a20 2020 2020 2020 793d 2230 220a 2020  .       y="0".  
-00004d80: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-00004d90: 2223 7061 7468 3839 3835 2d38 220a 2020  "#path8985-8".  
-00004da0: 2020 2020 2069 643d 2275 7365 3236 3031       id="use2601
-00004db0: 3222 0a20 2020 2020 2020 7472 616e 7366  2".       transf
-00004dc0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
-00004dd0: 302e 3831 3333 3334 2c32 392e 3436 3339  0.813334,29.4639
-00004de0: 3135 2922 202f 3e0a 2020 2020 3c75 7365  15)" />.    <use
-00004df0: 0a20 2020 2020 2020 783d 2230 220a 2020  .       x="0".  
-00004e00: 2020 2020 2079 3d22 3022 0a20 2020 2020       y="0".     
-00004e10: 2020 786c 696e 6b3a 6872 6566 3d22 2370    xlink:href="#p
-00004e20: 6174 6838 3938 352d 3822 0a20 2020 2020  ath8985-8".     
-00004e30: 2020 6964 3d22 7573 6532 3630 3134 220a    id="use26014".
-00004e40: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00004e50: 3d22 7472 616e 736c 6174 6528 362e 3939  ="translate(6.99
-00004e60: 3832 3136 382c 3332 2e30 3033 3839 3429  82168,32.003894)
-00004e70: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
-00004e80: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00004e90: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-00004ea0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-00004eb0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
-00004ec0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00004ed0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00004ee0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
-00004ef0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00004f00: 2064 3d22 6d20 3733 2e31 3433 3239 312c   d="m 73.143291,
-00004f10: 3235 392e 3134 3531 3320 6320 302e 3230  259.14513 c 0.20
-00004f20: 3836 392c 2d30 2e30 3538 3320 322e 3434  869,-0.0583 2.44
-00004f30: 3539 3439 2c2d 322e 3230 3235 3720 342e  5949,-2.20257 4.
-00004f40: 3932 3734 3134 2c2d 322e 3233 3036 3720  927414,-2.23067 
-00004f50: 322e 3038 3139 3339 2c2d 302e 3032 3336  2.081939,-0.0236
-00004f60: 2033 2e31 3935 3530 342c 302e 3631 3220   3.195504,0.612 
-00004f70: 342e 3031 3830 3731 2c31 2e38 3137 3934  4.018071,1.81794
-00004f80: 2031 2e30 3735 3338 392c 312e 3537 3635   1.075389,1.5765
-00004f90: 3820 312e 3038 3336 3239 2c34 2e36 3337  8 1.083629,4.637
-00004fa0: 3032 2030 2e31 3130 3839 372c 362e 3237  02 0.110897,6.27
-00004fb0: 3735 3920 2d30 2e38 3631 3934 2c31 2e34  759 -0.86194,1.4
-00004fc0: 3533 3731 202d 322e 3334 3532 3332 2c32  5371 -2.345232,2
-00004fd0: 2e34 3537 3436 202d 342e 3039 3231 3933  .45746 -4.092193
-00004fe0: 2c32 2e34 3533 3839 202d 322e 3131 3832  ,2.45389 -2.1182
-00004ff0: 3637 2c2d 302e 3030 3420 2d33 2e34 3739  67,-0.004 -3.479
-00005000: 3236 332c 2d30 2e39 3435 3139 202d 342e  263,-0.94519 -4.
-00005010: 3538 3737 3231 2c2d 322e 3035 3439 3322  587721,-2.05493"
-00005020: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00005030: 3136 3331 392d 372d 3922 0a20 2020 2020  16319-7-9".     
-00005040: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-00005050: 7970 6573 3d22 6373 7373 7363 2220 2f3e  ypes="cssssc" />
-00005060: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00005070: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
-00005080: 6e65 3b66 696c 6c2d 6f70 6163 6974 793a  ne;fill-opacity:
-00005090: 313b 7374 726f 6b65 3a23 3030 3030 3030  1;stroke:#000000
-000050a0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000050b0: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
-000050c0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000050d0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-000050e0: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-000050f0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00005100: 2037 322e 3835 3037 3139 2c32 3537 2e39   72.850719,257.9
-00005110: 3831 3320 312e 3039 3633 3933 2c32 2e34  813 1.096393,2.4
-00005120: 3535 3937 2063 2030 2c30 2032 2e35 3035  5597 c 0,0 2.505
-00005130: 3633 372c 2d31 2e38 3530 3534 2033 2e38  637,-1.85054 3.8
-00005140: 3930 3939 362c 2d31 2e38 3134 3620 312e  90996,-1.8146 1.
-00005150: 3232 3432 3735 2c30 2e30 3331 3820 322e  224275,0.0318 2.
-00005160: 3538 3331 332c 302e 3536 3232 3920 332e  58313,0.56229 3.
-00005170: 3135 3539 3634 2c31 2e37 3135 3820 302e  155964,1.7158 0.
-00005180: 3634 3830 312c 312e 3330 3438 3920 302e  64801,1.30489 0.
-00005190: 3433 3735 3239 2c32 2e38 3236 3035 202d  437529,2.82605 -
-000051a0: 302e 3232 3036 3239 2c33 2e37 3639 202d  0.220629,3.769 -
-000051b0: 302e 3535 3539 3831 2c30 2e37 3936 3536  0.555981,0.79656
-000051c0: 202d 312e 3335 3930 3932 2c31 2e35 3030   -1.359092,1.500
-000051d0: 3837 202d 322e 3238 3038 3734 2c31 2e36  87 -2.280874,1.6
-000051e0: 3335 3720 2d31 2e34 3737 3031 382c 302e  357 -1.477018,0.
-000051f0: 3231 3630 3420 2d33 2e31 3830 3333 342c  21604 -3.180334,
-00005200: 2d30 2e35 3235 3738 202d 342e 3735 3533  -0.52578 -4.7553
-00005210: 362c 2d32 2e30 3934 3436 206c 202d 302e  6,-2.09446 l -0.
-00005220: 3535 3136 3633 2c33 2e30 3231 3835 2063  551663,3.02185 c
-00005230: 2030 2e37 3039 3534 342c 312e 3031 3938   0.709544,1.0198
-00005240: 3920 322e 3738 3135 3932 2c32 2e33 3430  9 2.781592,2.340
-00005250: 3534 2034 2e37 3335 3530 372c 322e 3331  54 4.735507,2.31
-00005260: 3630 3620 322e 3234 3839 3734 2c2d 302e  606 2.248974,-0.
-00005270: 3032 3832 2034 2e34 3339 3631 322c 2d31  0282 4.439612,-1
-00005280: 2e36 3233 3420 352e 3537 3036 3631 2c2d  .6234 5.570661,-
-00005290: 332e 3434 3038 3820 312e 3030 3136 3431  3.44088 1.001641
-000052a0: 2c2d 312e 3630 3935 3320 312e 3138 3439  ,-1.60953 1.1849
-000052b0: 3234 2c2d 352e 3435 3435 3820 302e 3433  24,-5.45458 0.43
-000052c0: 3037 342c 2d36 2e39 3931 3933 202d 302e  074,-6.99193 -0.
-000052d0: 3931 3732 3134 2c2d 312e 3836 3936 3720  917214,-1.86967 
-000052e0: 2d33 2e31 3636 3134 322c 2d33 2e32 3636  -3.166142,-3.266
-000052f0: 3832 202d 352e 3333 3730 3637 2c2d 332e  82 -5.337067,-3.
-00005300: 3139 3936 202d 322e 3432 3038 3336 2c30  1996 -2.420836,0
-00005310: 2e30 3735 202d 352e 3733 3436 3638 2c32  .075 -5.734668,2
-00005320: 2e36 3237 3039 202d 352e 3733 3436 3638  .62709 -5.734668
-00005330: 2c32 2e36 3237 3039 207a 220a 2020 2020  ,2.62709 z".    
-00005340: 2020 2069 643d 2270 6174 6832 3637 3434     id="path26744
-00005350: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
-00005360: 693a 6e6f 6465 7479 7065 733d 2263 6373  i:nodetypes="ccs
-00005370: 7373 7363 6373 7373 7363 2220 2f3e 0a20  sssccssssc" />. 
-00005380: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00005390: 6964 3d22 7265 6374 3230 3431 352d 352d  id="rect20415-5-
-000053a0: 3522 0a20 2020 2020 2020 7374 796c 653d  5".       style=
-000053b0: 226f 7061 6369 7479 3a30 2e39 393b 6669  "opacity:0.99;fi
-000053c0: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
-000053d0: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-000053e0: 6474 683a 302e 333b 7374 726f 6b65 2d6c  dth:0.3;stroke-l
-000053f0: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00005400: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
-00005410: 6e64 220a 2020 2020 2020 2064 3d22 6d20  nd".       d="m 
-00005420: 3838 2e34 3738 3731 312c 3232 322e 3930  88.478711,222.90
-00005430: 3138 3720 6320 302c 3020 302e 3332 3633  187 c 0,0 0.3263
-00005440: 3833 2c2d 302e 3433 3831 2031 2e37 3238  83,-0.4381 1.728
-00005450: 3730 332c 2d30 2e34 3338 3120 312e 3430  703,-0.4381 1.40
-00005460: 3233 322c 3020 312e 3639 3136 3235 2c30  232,0 1.691625,0
-00005470: 2e34 3338 3120 312e 3639 3136 3235 2c30  .4381 1.691625,0
-00005480: 2e34 3338 3120 7620 3138 2e33 3530 3235  .4381 v 18.35025
-00005490: 2063 202d 302e 3031 3032 392c 302e 3031   c -0.01029,0.01
-000054a0: 3336 202d 302e 3332 3736 3732 2c30 2e32  36 -0.327672,0.2
-000054b0: 3437 3732 202d 312e 3731 3031 3634 2c30  4772 -1.710164,0
-000054c0: 2e32 3536 3837 202d 312e 3338 3234 3932  .25687 -1.382492
-000054d0: 2c30 2e30 3039 202d 312e 3731 3031 3634  ,0.009 -1.710164
-000054e0: 2c2d 302e 3235 3638 3720 2d31 2e37 3130  ,-0.25687 -1.710
-000054f0: 3136 342c 2d30 2e32 3536 3837 207a 220a  164,-0.25687 z".
-00005500: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00005510: 6e6f 6465 7479 7065 733d 2263 7a63 637a  nodetypes="czccz
-00005520: 6363 2220 2f3e 0a20 2020 203c 7061 7468  cc" />.    <path
-00005530: 0a20 2020 2020 2020 6964 3d22 7265 6374  .       id="rect
-00005540: 3230 3431 352d 352d 352d 3322 0a20 2020  20415-5-5-3".   
-00005550: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
-00005560: 7479 3a30 2e39 393b 6669 6c6c 3a23 3030  ty:0.99;fill:#00
-00005570: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
-00005580: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
-00005590: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-000055a0: 302e 333b 7374 726f 6b65 2d6c 696e 6563  0.3;stroke-linec
-000055b0: 6170 3a72 6f75 6e64 3b73 7472 6f6b 652d  ap:round;stroke-
-000055c0: 6c69 6e65 6a6f 696e 3a72 6f75 6e64 220a  linejoin:round".
-000055d0: 2020 2020 2020 2064 3d22 6d20 3934 2e30         d="m 94.0
-000055e0: 3039 3037 352c 3232 332e 3235 3937 3120  09075,223.25971 
-000055f0: 6320 302c 2d30 2e34 3033 3434 2030 2e31  c 0,-0.40344 0.1
-00005600: 3535 3438 382c 2d30 2e35 3536 3538 2030  55488,-0.55658 0
-00005610: 2e32 3736 3137 2c2d 302e 3635 3532 3620  .27617,-0.65526 
-00005620: 302e 3132 3036 3832 2c2d 302e 3039 3837  0.120682,-0.0987
-00005630: 2030 2e34 3136 3935 312c 2d30 2e32 3736   0.416951,-0.276
-00005640: 3535 2031 2e34 3531 3431 322c 2d30 2e32  55 1.451412,-0.2
-00005650: 3636 3337 2031 2e30 3334 3436 312c 302e  6637 1.034461,0.
-00005660: 3031 3032 2031 2e31 3734 3234 2c30 2e30  0102 1.17424,0.0
-00005670: 3832 3120 312e 3430 3132 3436 2c30 2e32  821 1.401246,0.2
-00005680: 3538 3335 2030 2e31 3730 3739 322c 302e  5835 0.170792,0.
-00005690: 3133 3235 3720 302e 3239 3135 3031 2c30  13257 0.291501,0
-000056a0: 2e33 3838 3034 2030 2e32 3931 3530 312c  .38804 0.291501,
-000056b0: 302e 3636 3332 3820 7620 3138 2e32 3733  0.66328 v 18.273
-000056c0: 3420 6820 2d33 2e34 3230 3332 3820 7a22  4 h -3.420328 z"
-000056d0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-000056e0: 3a6e 6f64 6574 7970 6573 3d22 737a 7a73  :nodetypes="szzs
-000056f0: 7363 6373 2220 2f3e 0a20 2020 203c 7061  sccs" />.    <pa
-00005700: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-00005710: 2266 696c 6c3a 2337 3834 3432 313b 7374  "fill:#784421;st
-00005720: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00005730: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
-00005740: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00005750: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00005760: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00005770: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00005780: 2020 2020 2064 3d22 6d20 3137 342e 3331       d="m 174.31
-00005790: 3938 362c 3636 2e37 3433 3838 2063 202d  986,66.74388 c -
-000057a0: 302e 3138 3038 2c31 2e31 3932 3738 3520  0.1808,1.192785 
-000057b0: 2d36 2e38 3738 372c 3135 2e36 3231 3731  -6.8787,15.62171
-000057c0: 3320 2d31 362e 3034 3533 372c 3135 2e32  3 -16.04537,15.2
-000057d0: 3336 3337 3720 2d31 362e 3632 3130 312c  36377 -16.62101,
-000057e0: 2d30 2e36 3938 3639 3220 2d33 332e 3836  -0.698692 -33.86
-000057f0: 3537 352c 2d30 2e32 3537 3539 3420 2d34  575,-0.257594 -4
-00005800: 392e 3635 3734 362c 2d35 2e34 3337 3738  9.65746,-5.43778
-00005810: 3620 2d31 2e34 3732 3438 2c2d 302e 3438  6 -1.47248,-0.48
-00005820: 3330 3231 202d 342e 3530 3235 382c 2d32  3021 -4.50258,-2
-00005830: 2e33 3039 3732 3320 2d35 2e32 3033 3738  .309723 -5.20378
-00005840: 2c2d 312e 3737 3731 3636 202d 302e 3639  ,-1.777166 -0.69
-00005850: 3330 372c 302e 3532 3633 3835 2031 2e31  307,0.526385 1.1
-00005860: 3636 3833 2c32 2e30 3033 3730 3820 322e  6683,2.003708 2.
-00005870: 3337 3339 382c 322e 3730 3831 3837 2034  37398,2.708187 4
-00005880: 2e37 3734 3536 2c32 2e35 3530 3631 3720  .77456,2.550617 
-00005890: 3130 2e33 3836 3239 2c33 2e34 3739 3337  10.38629,3.47937
-000058a0: 3520 3134 2e33 3233 3639 2c37 2e36 3531  5 14.32369,7.651
-000058b0: 3835 2032 2e30 3033 3331 2c31 2e35 3831  85 2.00331,1.581
-000058c0: 3536 3220 2d38 2e31 3631 312c 3138 2e36  562 -8.1611,18.6
-000058d0: 3937 3432 3820 2d37 2e38 3537 3732 2c31  97428 -7.85772,1
-000058e0: 392e 3535 3037 3638 2031 2e35 3639 3435  9.550768 1.56945
-000058f0: 2c34 2e34 3134 3538 2031 362e 3238 3139  ,4.41458 16.2819
-00005900: 332c 2d31 382e 3237 3236 3039 2031 352e  3,-18.272609 15.
-00005910: 3939 3630 372c 2d31 392e 3530 3339 3936  99607,-19.503996
-00005920: 206c 2033 382e 3330 3634 312c 302e 3734   l 38.30641,0.74
-00005930: 3833 3534 2063 2036 2e31 3731 3735 2c2d  8354 c 6.17175,-
-00005940: 352e 3739 3930 3531 2036 2e35 3433 3939  5.799051 6.54399
-00005950: 2c2d 3133 2e31 3435 3132 3720 372e 3736  ,-13.145127 7.76
-00005960: 3431 382c 2d31 392e 3137 3635 3838 207a  418,-19.176588 z
-00005970: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-00005980: 6832 3022 0a20 2020 2020 2020 736f 6469  h20".       sodi
-00005990: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-000059a0: 6373 7373 6363 7363 6363 2220 2f3e 0a20  csssccsccc" />. 
-000059b0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000059c0: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
-000059d0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000059e0: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
-000059f0: 7472 6f6b 652d 7769 6474 683a 343b 7374  troke-width:4;st
-00005a00: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
-00005a10: 6e64 3b73 7472 6f6b 652d 6c69 6e65 6a6f  nd;stroke-linejo
-00005a20: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00005a30: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00005a40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00005a50: 0a20 2020 2020 2020 643d 224d 2037 332e  .       d="M 73.
-00005a60: 3135 3135 3131 2c37 322e 3936 3232 3139  151511,72.962219
-00005a70: 2039 302e 3532 3032 3734 2c35 332e 3937   90.520274,53.97
-00005a80: 3836 3920 6d20 3135 2e38 3237 3431 362c  869 m 15.827416,
-00005a90: 2d38 2e34 3931 3533 3220 6320 3236 2e34  -8.491532 c 26.4
-00005aa0: 3533 3832 2c2d 322e 3037 3034 3133 2033  5382,-2.070413 3
-00005ab0: 392e 3139 3835 2c2d 302e 3834 3631 3239  9.1985,-0.846129
-00005ac0: 2035 382e 3638 3736 352c 332e 3131 3330   58.68765,3.1130
-00005ad0: 3931 2033 2e34 3435 3231 2c30 2e36 3939  91 3.44521,0.699
-00005ae0: 3839 3420 352e 3237 3337 352c 322e 3333  894 5.27375,2.33
-00005af0: 3130 3220 362e 3838 3934 312c 352e 3331  102 6.88941,5.31
-00005b00: 3530 3720 342e 3737 3734 312c 382e 3832  507 4.77741,8.82
-00005b10: 3336 3320 352e 3035 3538 322c 3137 2e34  363 5.05582,17.4
-00005b20: 3832 3334 202d 312e 3035 3639 2c32 372e  8234 -1.0569,27.
-00005b30: 3237 3738 3320 2d31 2e34 3031 3836 2c32  27783 -1.40186,2
-00005b40: 2e32 3436 3434 202d 342e 3139 3238 362c  .24644 -4.19286,
-00005b50: 342e 3830 3834 3320 2d36 2e38 3334 3931  4.80843 -6.83491
-00005b60: 2c34 2e39 3835 3334 202d 3131 2e33 3234  ,4.98534 -11.324
-00005b70: 3232 2c30 2e37 3538 3237 202d 3236 2e33  22,0.75827 -26.3
-00005b80: 3434 3136 2c2d 302e 3632 3637 202d 3331  4416,-0.6267 -31
-00005b90: 2e39 3933 3739 2c2d 302e 3838 3739 3820  .99379,-0.88798 
-00005ba0: 2d33 2e36 3332 3935 2c2d 302e 3136 3830  -3.63295,-0.1680
-00005bb0: 3120 2d36 2e38 3338 3232 2c33 2e34 3436  1 -6.83822,3.446
-00005bc0: 3631 3720 2d37 2e39 3032 3838 2c36 2e31  617 -7.90288,6.1
-00005bd0: 3635 3639 202d 322e 3938 3331 342c 372e  6569 -2.98314,7.
-00005be0: 3631 3837 3631 202d 362e 3839 3737 342c  618761 -6.89774,
-00005bf0: 3130 2e35 3331 3733 3120 2d31 322e 3136  10.531731 -12.16
-00005c00: 3235 392c 3135 2e32 3233 3230 3122 0a20  259,15.223201". 
-00005c10: 2020 2020 2020 6964 3d22 7061 7468 3122        id="path1"
-00005c20: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00005c30: 3a6e 6f64 6574 7970 6573 3d22 6363 6373  :nodetypes="cccs
-00005c40: 7373 7373 7363 2220 2f3e 0a20 2020 203c  sssssc" />.    <
-00005c50: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00005c60: 653d 2266 696c 6c3a 2337 3834 3432 313b  e="fill:#784421;
-00005c70: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
-00005c80: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
-00005c90: 3370 783b 7374 726f 6b65 2d6c 696e 6563  3px;stroke-linec
-00005ca0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00005cb0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00005cc0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00005cd0: 2020 2020 2020 2064 3d22 6d20 3131 362e         d="m 116.
-00005ce0: 3235 3135 322c 3534 2e30 3639 3539 3620  25152,54.069596 
-00005cf0: 6320 322e 3437 3435 362c 312e 3230 3939  c 2.47456,1.2099
-00005d00: 3231 2034 2e34 3535 3735 2c31 2e39 3633  21 4.45575,1.963
-00005d10: 3532 2038 2e30 3833 3435 2c32 2e32 3038  52 8.08345,2.208
-00005d20: 3738 3520 342e 3435 3234 322c 302e 3330  785 4.45242,0.30
-00005d30: 3130 3234 2037 2e38 3630 3938 2c30 2e33  1024 7.86098,0.3
-00005d40: 3131 3737 3220 3131 2e32 3131 3734 2c2d  11772 11.21174,-
-00005d50: 302e 3432 3637 3435 2031 2e31 3330 3237  0.426745 1.13027
-00005d60: 2c2d 302e 3234 3931 3133 202d 392e 3832  ,-0.249113 -9.82
-00005d70: 3331 332c 2d34 2e33 3038 3731 3520 2d31  313,-4.308715 -1
-00005d80: 302e 3130 3337 362c 2d34 2e32 3631 3934  0.10376,-4.26194
-00005d90: 3220 2d30 2e32 3830 3634 2c30 2e30 3436  2 -0.28064,0.046
-00005da0: 3737 202d 392e 3139 3134 332c 322e 3437  77 -9.19143,2.47
-00005db0: 3938 3937 202d 392e 3139 3134 332c 322e  9897 -9.19143,2.
-00005dc0: 3437 3938 3937 207a 220a 2020 2020 2020  479897 z".      
-00005dd0: 2069 643d 2270 6174 6832 3122 0a20 2020   id="path21".   
-00005de0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-00005df0: 6574 7970 6573 3d22 6373 7373 6363 2220  etypes="cssscc" 
-00005e00: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00005e10: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00005e20: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
-00005e30: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00005e40: 3a33 3b73 7472 6f6b 652d 6c69 6e65 6361  :3;stroke-lineca
-00005e50: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
-00005e60: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00005e70: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00005e80: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-00005e90: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-00005ea0: 6d20 3133 352e 3239 3630 362c 3534 2e35  m 135.29606,54.5
-00005eb0: 3534 3836 3920 6320 2d39 2e39 3837 3238  54869 c -9.98728
-00005ec0: 2c2d 332e 3435 3835 3820 2d31 342e 3438  ,-3.45858 -14.48
-00005ed0: 3134 312c 2d32 2e36 3633 3638 202d 3138  141,-2.66368 -18
-00005ee0: 2e38 3038 3439 2c2d 312e 3733 3934 3422  .80849,-1.73944"
-00005ef0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00005f00: 3322 0a20 2020 2020 2020 736f 6469 706f  3".       sodipo
-00005f10: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00005f20: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
-00005f30: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00005f40: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
-00005f50: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00005f60: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-00005f70: 6964 7468 3a30 2e38 3635 3b73 7472 6f6b  idth:0.865;strok
-00005f80: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00005f90: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00005fa0: 6974 6572 3b73 7472 6f6b 652d 6461 7368  iter;stroke-dash
-00005fb0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00005fc0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00005fd0: 2020 2020 643d 226d 2031 3239 2e34 3135      d="m 129.415
-00005fe0: 3535 2c35 332e 3236 3739 3339 2063 2031  55,53.267939 c 1
-00005ff0: 2e31 3238 3334 2c32 2e34 3230 3938 202d  .12834,2.42098 -
-00006000: 312e 3239 3533 352c 332e 3834 3934 3920  1.29535,3.84949 
-00006010: 2d34 2e33 3432 3238 2c33 2e37 3139 3539  -4.34228,3.71959
-00006020: 202d 322e 3435 3635 372c 302e 3039 3931   -2.45657,0.0991
-00006030: 202d 352e 3330 3339 382c 2d32 2e31 3332   -5.30398,-2.132
-00006040: 3420 2d35 2e37 3334 332c 2d34 2e33 3835  4 -5.7343,-4.385
-00006050: 3132 2033 2e36 3231 3533 2c2d 302e 3434  12 3.62153,-0.44
-00006060: 3936 3320 362e 3331 3731 352c 2d30 2e39  963 6.31715,-0.9
-00006070: 3137 3535 2031 302e 3037 3635 382c 302e  1755 10.07658,0.
-00006080: 3636 3535 3320 7a22 0a20 2020 2020 2020  66553 z".       
-00006090: 6964 3d22 7061 7468 3422 0a20 2020 2020  id="path4".     
-000060a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-000060b0: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
-000060c0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000060d0: 6964 3d22 7061 7468 3431 392d 332d 3022  id="path419-3-0"
-000060e0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000060f0: 696c 6c3a 2363 3031 3730 303b 6669 6c6c  ill:#c01700;fill
-00006100: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
-00006110: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
-00006120: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-00006130: 7769 6474 683a 302e 3438 3631 3370 783b  width:0.48613px;
-00006140: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00006150: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00006160: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00006170: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00006180: 2020 2064 3d22 6d20 3231 382e 3936 3331     d="m 218.9631
-00006190: 392c 3533 2e37 3734 3833 3620 6320 2d30  9,53.774836 c -0
-000061a0: 2e37 3436 3032 2c30 2e34 3033 3335 3220  .74602,0.403352 
-000061b0: 2d30 2e37 3839 3233 2c31 2e32 3039 3738  -0.78923,1.20978
-000061c0: 3120 322e 3430 3830 342c 342e 3631 3733  1 2.40804,4.6173
-000061d0: 3835 2034 2e31 3934 3735 2c34 2e34 3730  85 4.19475,4.470
-000061e0: 3639 3820 3234 2e33 3539 3032 2c31 312e  698 24.35902,11.
-000061f0: 3735 3736 3036 2033 382e 3832 3238 382c  757606 38.82288,
-00006200: 3131 2e36 3839 3233 3820 322e 3434 3333  11.689238 2.4433
-00006210: 372c 2d30 2e33 3534 3034 3620 322e 3638  7,-0.354046 2.68
-00006220: 372c 2d30 2e34 3633 3338 3220 322e 3734  7,-0.463382 2.74
-00006230: 3033 342c 2d31 2e31 3034 3930 3320 302e  034,-1.104903 0.
-00006240: 3035 3637 2c2d 302e 3638 3135 3132 202d  0567,-0.681512 -
-00006250: 302e 3138 3935 372c 2d31 2e31 3239 3330  0.18957,-1.12930
-00006260: 3420 2d32 2e34 3038 3832 2c2d 302e 3833  4 -2.40882,-0.83
-00006270: 3931 3132 202d 382e 3339 3133 362c 312e  9112 -8.39136,1.
-00006280: 3039 3732 3534 202d 3332 2e37 3137 3337  097254 -32.71737
-00006290: 2c32 332e 3030 3238 3637 202d 3334 2e35  ,23.002867 -34.5
-000062a0: 3734 392c 3237 2e35 3138 3334 3820 2d31  749,27.518348 -1
-000062b0: 2e30 3539 3335 2c32 2e35 3735 3137 3720  .05935,2.575177 
-000062c0: 2d30 2e35 3033 3431 2c33 2e38 3137 3536  -0.50341,3.81756
-000062d0: 3720 302e 3138 3939 342c 332e 3933 3238  7 0.18994,3.9328
-000062e0: 3135 2030 2e37 3333 3638 2c30 2e31 3231  15 0.73368,0.121
-000062f0: 3935 3320 312e 3438 3930 332c 2d31 2e39  953 1.48903,-1.9
-00006300: 3438 3736 3720 312e 3432 3031 342c 2d36  48767 1.42014,-6
-00006310: 2e39 3435 3832 3420 2d30 2e31 3931 3431  .945824 -0.19141
-00006320: 2c2d 3133 2e38 3835 3133 3820 2d31 2e39  ,-13.885138 -1.9
-00006330: 3434 3732 2c2d 3234 2e31 3437 3120 2d35  4472,-24.1471 -5
-00006340: 2e38 3137 3236 2c2d 3334 2e37 3933 3334  .81726,-34.79334
-00006350: 3420 2d31 2e35 3335 3338 2c2d 342e 3232  4 -1.53538,-4.22
-00006360: 3130 3335 202d 322e 3034 3931 352c 2d34  1035 -2.04915,-4
-00006370: 2e34 3639 3934 3920 2d32 2e37 3830 3336  .469949 -2.78036
-00006380: 2c2d 342e 3037 3436 3033 207a 206d 2034  ,-4.074603 z m 4
-00006390: 2e35 3630 3432 2c31 2e38 3938 3430 3620  .56042,1.898406 
-000063a0: 6320 352e 3934 3334 342c 3135 2e33 3934  c 5.94344,15.394
-000063b0: 3334 3520 362e 3030 3138 322c 3138 2e38  345 6.00182,18.8
-000063c0: 3134 3035 3520 372e 3033 3534 2c33 382e  14055 7.0354,38.
-000063d0: 3834 3339 3339 2030 2e33 3530 3739 2c36  843939 0.35079,6
-000063e0: 2e37 3936 3734 3920 2d32 2e38 3039 3731  .796749 -2.80971
-000063f0: 2c37 2e35 3837 3430 3920 2d34 2e31 3837  ,7.587409 -4.187
-00006400: 3235 2c37 2e37 3238 3434 3920 2d34 2e31  25,7.728449 -4.1
-00006410: 3835 3934 2c30 2e34 3238 3620 2d34 2e39  8594,0.4286 -4.9
-00006420: 3734 3335 2c2d 332e 3736 3335 3835 202d  7435,-3.763585 -
-00006430: 312e 3737 3435 352c 2d38 2e35 3330 3038  1.77455,-8.53008
-00006440: 3320 342e 3338 3535 2c2d 362e 3533 3237  3 4.3855,-6.5327
-00006450: 3731 2032 302e 3230 3533 2c2d 3235 2e33  71 20.2053,-25.3
-00006460: 3338 3132 3620 3335 2e38 3134 3731 2c2d  38126 35.81471,-
-00006470: 3238 2e33 3731 3530 3820 332e 3232 3432  28.371508 3.2242
-00006480: 392c 2d30 2e34 3935 3435 3620 352e 3532  9,-0.495456 5.52
-00006490: 3036 342c 2d30 2e38 3839 3037 3220 362e  064,-0.889072 6.
-000064a0: 3235 3633 312c 322e 3238 3930 3832 2030  25631,2.289082 0
-000064b0: 2e38 3131 3335 2c33 2e35 3035 3737 3920  .81135,3.505779 
-000064c0: 2d30 2e39 3938 3033 2c34 2e35 3339 3231  -0.99803,4.53921
-000064d0: 3720 2d34 2e35 3630 3338 2c35 2e30 3437  7 -4.56038,5.047
-000064e0: 3733 3620 2d31 342e 3531 3730 322c 322e  736 -14.51702,2.
-000064f0: 3037 3232 3820 2d33 392e 3234 3430 372c  07228 -39.24407,
-00006500: 2d36 2e37 3733 3935 3720 2d34 332e 3939  -6.773957 -43.99
-00006510: 3732 312c 2d31 332e 3831 3834 3435 202d  721,-13.818445 -
-00006520: 322e 3634 3639 322c 2d33 2e39 3232 3931  2.64692,-3.92291
-00006530: 3920 2d32 2e32 3939 3938 2c2d 362e 3336  9 -2.29998,-6.36
-00006540: 3334 3836 202d 302e 3831 3836 362c 2d37  3486 -0.81866,-7
-00006550: 2e34 3733 3835 3320 312e 3236 3133 342c  .473853 1.26134,
-00006560: 2d30 2e39 3435 3438 2034 2e31 3834 3339  -0.94548 4.18439
-00006570: 2c2d 312e 3031 3739 3436 2036 2e32 3331  ,-1.017946 6.231
-00006580: 3633 2c34 2e32 3834 3638 3320 7a22 0a20  63,4.284683 z". 
-00006590: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-000065a0: 6f64 6574 7970 6573 3d22 7373 6373 7373  odetypes="sscsss
-000065b0: 7373 7373 7373 7373 6373 7373 7373 2220  sssssssscsssss" 
-000065c0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-000065d0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-000065e0: 6e6f 6e65 3b66 696c 6c2d 6f70 6163 6974  none;fill-opacit
-000065f0: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
-00006600: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-00006610: 343b 7374 726f 6b65 2d6c 696e 6563 6170  4;stroke-linecap
-00006620: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00006630: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00006640: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00006650: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00006660: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
-00006670: 2d39 312e 3535 3234 3733 2c31 3936 2e38  -91.552473,196.8
-00006680: 3633 3239 2032 312e 3837 3632 322c 2d32  6329 21.87622,-2
-00006690: 342e 3536 3734 2063 2031 2e38 3835 3532  4.5674 c 1.88552
-000066a0: 2c2d 322e 3332 3030 3120 3130 2e33 3432  ,-2.32001 10.342
-000066b0: 3033 2c2d 332e 3433 3131 3320 3133 2e33  03,-3.43113 13.3
-000066c0: 3236 3232 2c2d 332e 3235 3135 3720 3231  2622,-3.25157 21
-000066d0: 2e35 3833 3133 2c30 2e30 3136 3420 3335  .58313,0.0164 35
-000066e0: 2e32 3530 3131 2c30 2e31 3030 3935 2035  .25011,0.10095 5
-000066f0: 362e 3638 3133 3839 3737 2c33 2e34 3537  6.68138977,3.457
-00006700: 2033 2e34 3733 3235 3030 332c 302e 3534   3.47325003,0.54
-00006710: 3339 2035 2e32 3733 3735 3030 332c 322e  39 5.27375003,2.
-00006720: 3333 3130 3220 362e 3838 3934 3130 3033  33102 6.88941003
-00006730: 2c35 2e33 3135 3037 2034 2e37 3737 3431  ,5.31507 4.77741
-00006740: 3032 2c38 2e38 3233 3633 2035 2e30 3535  02,8.82363 5.055
-00006750: 3832 3032 2c31 372e 3438 3233 3420 2d31  8202,17.48234 -1
-00006760: 2e30 3536 392c 3237 2e32 3737 3833 202d  .0569,27.27783 -
-00006770: 312e 3430 3138 362c 322e 3234 3634 3420  1.40186,2.24644 
-00006780: 2d34 2e31 3932 3836 2c34 2e38 3038 3433  -4.19286,4.80843
-00006790: 202d 362e 3833 3439 3130 3033 2c34 2e39   -6.83491003,4.9
-000067a0: 3835 3334 202d 3131 2e33 3234 3231 3937  8534 -11.3242197
-000067b0: 372c 302e 3735 3832 3720 2d32 362e 3334  7,0.75827 -26.34
-000067c0: 3431 3439 3737 2c2d 302e 3632 3637 202d  414977,-0.6267 -
-000067d0: 3331 2e39 3933 3738 3937 372c 2d30 2e38  31.99378977,-0.8
-000067e0: 3837 3938 202d 332e 3633 3239 342c 2d30  8798 -3.63294,-0
-000067f0: 2e31 3638 3031 202d 362e 3833 3832 322c  .16801 -6.83822,
-00006800: 332e 3434 3636 3120 2d37 2e39 3032 3838  3.44661 -7.90288
-00006810: 2c36 2e31 3635 3639 202d 322e 3938 3331  ,6.16569 -2.9831
-00006820: 342c 372e 3631 3837 3620 2d36 2e38 3937  4,7.61876 -6.897
-00006830: 3734 2c31 302e 3533 3137 3320 2d31 322e  74,10.53173 -12.
-00006840: 3136 3235 392c 3135 2e32 3233 3222 0a20  16259,15.2232". 
-00006850: 2020 2020 2020 6964 3d22 7061 7468 312d        id="path1-
-00006860: 3922 0a20 2020 2020 2020 736f 6469 706f  9".       sodipo
-00006870: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00006880: 6373 7373 7373 7363 2220 2f3e 0a20 2020  cssssssc" />.   
-00006890: 203c 670a 2020 2020 2020 2069 643d 2267   <g.       id="g
-000068a0: 3230 220a 2020 2020 2020 2074 7261 6e73  20".       trans
-000068b0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-000068c0: 2d36 302e 3631 3632 3437 2c32 342e 3832  -60.616247,24.82
-000068d0: 3832 3637 2922 3e0a 2020 2020 2020 3c67  8267)">.      <g
-000068e0: 0a20 2020 2020 2020 2020 6964 3d22 6731  .         id="g1
-000068f0: 3922 3e0a 2020 2020 2020 2020 3c67 0a20  9">.        <g. 
-00006900: 2020 2020 2020 2020 2020 6964 3d22 6734            id="g4
-00006910: 3422 0a20 2020 2020 2020 2020 2020 7472  4".           tr
-00006920: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00006930: 302e 3731 3235 3335 3039 2c2d 302e 3331  0.71253509,-0.31
-00006940: 3731 3731 3934 2c30 2e33 3137 3137 3139  717194,0.3171719
-00006950: 342c 302e 3731 3235 3335 3039 2c32 342e  4,0.71253509,24.
-00006960: 3832 3032 382c 3539 2e34 3536 3437 3429  82028,59.456474)
-00006970: 223e 0a20 2020 2020 2020 2020 203c 7061  ">.          <pa
-00006980: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
-00006990: 7374 796c 653d 226f 7061 6369 7479 3a30  style="opacity:0
-000069a0: 2e39 393b 6669 6c6c 3a23 6630 6633 3666  .99;fill:#f0f36f
-000069b0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000069c0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
-000069d0: 6b65 2d77 6964 7468 3a30 2e31 3438 3535  ke-width:0.14855
-000069e0: 323b 7374 726f 6b65 2d6c 696e 6563 6170  2;stroke-linecap
-000069f0: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6d69  :round;stroke-mi
-00006a00: 7465 726c 696d 6974 3a33 2e34 3b73 7472  terlimit:3.4;str
-00006a10: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00006a20: 6e65 220a 2020 2020 2020 2020 2020 2020  ne".            
-00006a30: 2064 3d22 6d20 3133 342e 3738 3331 322c   d="m 134.78312,
-00006a40: 3139 2e35 3536 3334 3720 7620 2d30 2e36  19.556347 v -0.6
-00006a50: 3436 3038 3520 6320 3136 2e39 3639 3633  46085 c 16.96963
-00006a60: 2c2d 302e 3033 3039 2036 392e 3738 3039  ,-0.0309 69.7809
-00006a70: 382c 2d30 2e30 3636 3236 2038 362e 3735  8,-0.06626 86.75
-00006a80: 3036 342c 2d30 2e30 3633 3931 206c 2033  064,-0.06391 l 3
-00006a90: 2e32 3432 3631 2c34 2e35 652d 3420 302e  .24261,4.5e-4 0.
-00006aa0: 3537 3430 342c 302e 3332 3839 3920 6320  57404,0.32899 c 
-00006ab0: 302e 3331 3537 322c 302e 3138 3039 3434  0.31572,0.180944
-00006ac0: 2030 2e35 3734 3339 2c30 2e33 3430 3438   0.57439,0.34048
-00006ad0: 3520 302e 3537 3438 322c 302e 3335 3435  5 0.57482,0.3545
-00006ae0: 3332 2030 2e30 3031 2c30 2e30 3336 3533  32 0.001,0.03653
-00006af0: 202d 302e 3035 3433 2c30 2e31 3339 3530   -0.0543,0.13950
-00006b00: 3620 2d30 2e31 3230 3131 2c30 2e32 3233  6 -0.12011,0.223
-00006b10: 3330 3620 2d30 2e31 3737 332c 302e 3232  306 -0.1773,0.22
-00006b20: 3536 3520 2d30 2e36 3232 3434 2c30 2e33  565 -0.62244,0.3
-00006b30: 3830 3035 202d 312e 3233 3431 322c 302e  8005 -1.23412,0.
-00006b40: 3432 3830 3539 202d 3139 2e35 3933 3837  428059 -19.59387
-00006b50: 2c30 2e30 3335 3634 202d 3730 2e31 3933  ,0.03564 -70.193
-00006b60: 3933 2c30 2e30 3230 3735 202d 3839 2e37  93,0.02075 -89.7
-00006b70: 3837 3838 2c30 2e30 3230 3735 207a 220a  8788,0.02075 z".
-00006b80: 2020 2020 2020 2020 2020 2020 2069 643d               id=
-00006b90: 2270 6174 6831 3522 0a20 2020 2020 2020  "path15".       
-00006ba0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00006bb0: 6f64 6574 7970 6573 3d22 6363 7363 7363  odetypes="ccscsc
-00006bc0: 7373 6363 2220 2f3e 0a20 2020 2020 2020  sscc" />.       
-00006bd0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00006be0: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-00006bf0: 6369 7479 3a30 2e39 393b 6669 6c6c 3a23  city:0.99;fill:#
-00006c00: 6633 6465 3666 3b66 696c 6c2d 6f70 6163  f3de6f;fill-opac
-00006c10: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
-00006c20: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
-00006c30: 2e31 3438 3535 323b 7374 726f 6b65 2d6c  .148552;stroke-l
-00006c40: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00006c50: 6f6b 652d 6d69 7465 726c 696d 6974 3a33  oke-miterlimit:3
-00006c60: 2e34 3b73 7472 6f6b 652d 6461 7368 6172  .4;stroke-dashar
-00006c70: 7261 793a 6e6f 6e65 220a 2020 2020 2020  ray:none".      
-00006c80: 2020 2020 2020 2064 3d22 6d20 3133 352e         d="m 135.
-00006c90: 3032 3234 312c 3232 2e35 3131 3536 3220  02241,22.511562 
-00006ca0: 302e 3039 3335 2c2d 322e 3137 3738 3338  0.0935,-2.177838
-00006cb0: 2063 2031 392e 3437 3734 312c 302e 3138   c 19.47741,0.18
-00006cc0: 3538 3639 2036 392e 3837 3235 322c 2d30  5869 69.87252,-0
-00006cd0: 2e30 3731 3837 2038 392e 3334 3933 342c  .07187 89.34934,
-00006ce0: 302e 3038 3236 2031 2e30 3433 3036 2c30  0.0826 1.04306,0
-00006cf0: 2e31 3237 3832 3420 312e 3735 3337 392c  .127824 1.75379,
-00006d00: 312e 3138 3230 3739 2031 2e37 3835 382c  1.182079 1.7858,
-00006d10: 322e 3033 3531 3634 2030 2e30 3136 392c  2.035164 0.0169,
-00006d20: 302e 3435 3131 3736 202d 302e 3330 3538  0.451176 -0.3058
-00006d30: 352c 322e 3035 3530 3336 202d 312e 3937  5,2.055036 -1.97
-00006d40: 3031 372c 322e 3137 3530 3539 202d 3139  017,2.175059 -19
-00006d50: 2e34 3137 3236 2c2d 302e 3131 3335 3834  .41726,-0.113584
-00006d60: 202d 3639 2e38 3430 3937 2c2d 302e 3038   -69.84097,-0.08
-00006d70: 3131 202d 3839 2e32 3538 3437 2c2d 302e  11 -89.25847,-0.
-00006d80: 3038 3039 3920 7a22 0a20 2020 2020 2020  08099 z".       
-00006d90: 2020 2020 2020 6964 3d22 7061 7468 3136        id="path16
-00006da0: 220a 2020 2020 2020 2020 2020 2020 2073  ".             s
-00006db0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00006dc0: 733d 2263 6373 7373 6363 2220 2f3e 0a20  s="ccssscc" />. 
-00006dd0: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-00006de0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00006df0: 653d 226f 7061 6369 7479 3a30 2e39 393b  e="opacity:0.99;
-00006e00: 6669 6c6c 3a23 6264 6138 3337 3b66 696c  fill:#bda837;fil
-00006e10: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00006e20: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
-00006e30: 6964 7468 3a30 2e31 3438 3535 323b 7374  idth:0.148552;st
-00006e40: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
-00006e50: 6e64 3b73 7472 6f6b 652d 6d69 7465 726c  nd;stroke-miterl
-00006e60: 696d 6974 3a33 2e34 3b73 7472 6f6b 652d  imit:3.4;stroke-
-00006e70: 6461 7368 6172 7261 793a 6e6f 6e65 220a  dasharray:none".
-00006e80: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
-00006e90: 6d20 3133 352e 3032 3235 352c 3236 2e33  m 135.02255,26.3
-00006ea0: 3833 3438 3120 7620 2d31 2e35 3632 3738  83481 v -1.56278
-00006eb0: 3920 6320 3139 2e35 3032 2c30 2e31 3937  9 c 19.502,0.197
-00006ec0: 3931 2037 302e 3031 3738 332c 2d30 2e32  91 70.01783,-0.2
-00006ed0: 3530 3331 3720 3839 2e35 3138 3932 2c2d  50317 89.51892,-
-00006ee0: 302e 3032 3631 3420 302e 3436 3937 362c  0.02614 0.46976,
-00006ef0: 302e 3037 3038 3120 302e 3930 3230 392c  0.07081 0.90209,
-00006f00: 302e 3238 3932 3138 2031 2e31 3930 3836  0.289218 1.19086
-00006f10: 2c30 2e36 3030 3030 3520 302e 3339 352c  ,0.600005 0.395,
-00006f20: 302e 3432 3338 3131 2030 2e34 3235 3833  0.423811 0.42583
-00006f30: 2c31 2e30 3032 3632 3520 302e 3339 3437  ,1.002625 0.3947
-00006f40: 382c 312e 3532 3832 3237 202d 302e 3030  8,1.528227 -0.00
-00006f50: 322c 302e 3033 3036 3820 2d30 2e32 3739  2,0.03068 -0.279
-00006f60: 3036 2c30 2e32 3135 3731 3920 2d30 2e38  06,0.215719 -0.8
-00006f70: 3737 3039 2c30 2e35 3535 3132 206c 202d  7709,0.55512 l -
-00006f80: 302e 3836 3232 382c 302e 3438 3933 3720  0.86228,0.48937 
-00006f90: 6320 2d31 392e 3435 3330 372c 2d30 2e30  c -19.45307,-0.0
-00006fa0: 3830 3738 202d 3639 2e39 3132 3038 2c2d  8078 -69.91208,-
-00006fb0: 302e 3034 3835 3620 2d38 392e 3336 3532  0.04856 -89.3652
-00006fc0: 2c2d 302e 3032 3130 3120 7a22 0a20 2020  ,-0.02101 z".   
-00006fd0: 2020 2020 2020 2020 2020 6964 3d22 7061            id="pa
-00006fe0: 7468 3137 220a 2020 2020 2020 2020 2020  th17".          
-00006ff0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00007000: 7479 7065 733d 2263 6373 7373 7363 6363  types="ccssssccc
-00007010: 2220 2f3e 0a20 2020 2020 2020 2020 203c  " />.          <
-00007020: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-00007030: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
-00007040: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
-00007050: 303b 7374 726f 6b65 2d77 6964 7468 3a32  0;stroke-width:2
-00007060: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00007070: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00007080: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00007090: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-000070a0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-000070b0: 3122 0a20 2020 2020 2020 2020 2020 2020  1".             
-000070c0: 643d 226d 2031 3330 2e35 3835 3335 2c31  d="m 130.58535,1
-000070d0: 372e 3930 3432 3331 2039 342e 3434 3932  7.904231 94.4492
-000070e0: 382c 2d30 2e30 3734 3720 392e 3430 352c  8,-0.0747 9.405,
-000070f0: 352e 3432 3939 3833 202d 392e 3739 3637  5.429983 -9.7967
-00007100: 312c 352e 3635 3631 3337 202d 3934 2e31  1,5.656137 -94.1
-00007110: 3236 3334 2c30 2e30 3335 3839 2063 202d  2634,0.03589 c -
-00007120: 372e 3630 3736 392c 3020 2d37 2e34 3838  7.60769,0 -7.488
-00007130: 3936 2c2d 3131 2e30 3437 3330 3520 302e  96,-11.047305 0.
-00007140: 3036 3838 2c2d 3131 2e30 3437 3330 3520  0688,-11.047305 
-00007150: 7a22 0a20 2020 2020 2020 2020 2020 2020  z".             
-00007160: 6964 3d22 7061 7468 3130 220a 2020 2020  id="path10".    
-00007170: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00007180: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-00007190: 6363 6363 2220 2f3e 0a20 2020 2020 2020  cccc" />.       
-000071a0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000071b0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000071c0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-000071d0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-000071e0: 7468 3a32 3b73 7472 6f6b 652d 6c69 6e65  th:2;stroke-line
-000071f0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00007200: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00007210: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00007220: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00007230: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00007240: 2020 2020 643d 224d 2031 3334 2e34 3336      d="M 134.436
-00007250: 312c 3138 2e33 3137 3638 2056 2032 382e  1,18.31768 V 28.
-00007260: 3437 3837 3335 220a 2020 2020 2020 2020  478735".        
-00007270: 2020 2020 2069 643d 2270 6174 6831 3122       id="path11"
-00007280: 0a20 2020 2020 2020 2020 2020 2020 736f  .             so
-00007290: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-000072a0: 3d22 6363 2220 2f3e 0a20 2020 2020 2020  ="cc" />.       
-000072b0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000072c0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000072d0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-000072e0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-000072f0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
-00007300: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00007310: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00007320: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
-00007330: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00007340: 2020 2020 2020 2064 3d22 6d20 3232 352e         d="m 225.
-00007350: 3839 3137 2c31 382e 3036 3036 3833 2063  8917,18.060683 c
-00007360: 2030 2c30 2e35 3939 3433 3220 312e 3134   0,0.599432 1.14
-00007370: 3633 382c 322e 3237 3837 3039 202d 312e  638,2.278709 -1.
-00007380: 3734 3638 392c 322e 3237 3837 3039 2032  74689,2.278709 2
-00007390: 2e38 3232 3837 2c30 2e30 3534 3936 2032  .82287,0.05496 2
-000073a0: 2e39 3036 392c 342e 3333 3733 3520 2d30  .9069,4.33735 -0
-000073b0: 2e30 3232 322c 342e 3333 3733 3520 322e  .0222,4.33735 2.
-000073c0: 3931 3931 352c 3020 322e 3735 3433 332c  91915,0 2.75433,
-000073d0: 332e 3838 3231 3533 2030 2e30 3536 332c  3.882153 0.0563,
-000073e0: 332e 3838 3231 3533 220a 2020 2020 2020  3.882153".      
-000073f0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00007400: 3222 0a20 2020 2020 2020 2020 2020 2020  2".             
-00007410: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00007420: 6573 3d22 6363 6363 2220 2f3e 0a20 2020  es="cccc" />.   
-00007430: 2020 2020 2020 203c 7061 7468 0a20 2020         <path.   
-00007440: 2020 2020 2020 2020 2020 7374 796c 653d            style=
-00007450: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-00007460: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00007470: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
-00007480: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00007490: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-000074a0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-000074b0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-000074c0: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-000074d0: 3232 342e 3137 3839 392c 3234 2e36 3739  224.17899,24.679
-000074e0: 3335 3920 4820 3133 352e 3039 3222 0a20  359 H 135.092". 
-000074f0: 2020 2020 2020 2020 2020 2020 6964 3d22              id="
-00007500: 7061 7468 3133 220a 2020 2020 2020 2020  path13".        
-00007510: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00007520: 6465 7479 7065 733d 2263 6322 202f 3e0a  detypes="cc" />.
-00007530: 2020 2020 2020 2020 2020 3c70 6174 680a            <path.
-00007540: 2020 2020 2020 2020 2020 2020 2073 7479               sty
-00007550: 6c65 3d22 6669 6c6c 3a6e 6f6e 653b 7374  le="fill:none;st
-00007560: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00007570: 6f6b 652d 7769 6474 683a 302e 3236 3435  oke-width:0.2645
-00007580: 3833 7078 3b73 7472 6f6b 652d 6c69 6e65  83px;stroke-line
-00007590: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-000075a0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-000075b0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-000075c0: 0a20 2020 2020 2020 2020 2020 2020 643d  .             d=
-000075d0: 224d 2032 3234 2e31 3531 3737 2c32 302e  "M 224.15177,20.
-000075e0: 3333 3834 3439 2048 2031 3335 2e30 3634  338449 H 135.064
-000075f0: 3738 220a 2020 2020 2020 2020 2020 2020  78".            
-00007600: 2069 643d 2270 6174 6831 332d 3322 0a20   id="path13-3". 
-00007610: 2020 2020 2020 2020 2020 2020 736f 6469              sodi
-00007620: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00007630: 6363 2220 2f3e 0a20 2020 2020 2020 2020  cc" />.         
-00007640: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-00007650: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
-00007660: 7479 3a30 2e39 393b 6669 6c6c 3a23 6633  ty:0.99;fill:#f3
-00007670: 3665 3536 3b66 696c 6c2d 6f70 6163 6974  6e56;fill-opacit
-00007680: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
-00007690: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-000076a0: 302e 3239 3731 3033 3b73 7472 6f6b 652d  0.297103;stroke-
-000076b0: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
-000076c0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-000076d0: 332e 343b 7374 726f 6b65 2d64 6173 6861  3.4;stroke-dasha
-000076e0: 7272 6179 3a6e 6f6e 6522 0a20 2020 2020  rray:none".     
-000076f0: 2020 2020 2020 2020 643d 226d 2031 3330          d="m 130
-00007700: 2e30 3737 3732 2c32 372e 3931 3933 3532  .07772,27.919352
-00007710: 2063 202d 302e 3639 3731 312c 2d30 2e30   c -0.69711,-0.0
-00007720: 3638 3139 202d 312e 3138 3235 342c 2d30  6819 -1.18254,-0
-00007730: 2e31 3833 3332 3820 2d31 2e36 3833 3536  .183328 -1.68356
-00007740: 2c2d 302e 3339 3933 3331 202d 312e 3236  ,-0.399331 -1.26
-00007750: 3535 312c 2d30 2e35 3435 3539 3220 2d32  551,-0.545592 -2
-00007760: 2e31 3433 3133 2c2d 312e 3638 3030 3534  .14313,-1.680054
-00007770: 202d 322e 3432 3935 322c 2d33 2e31 3430   -2.42952,-3.140
-00007780: 3532 3520 2d30 2e31 3030 382c 2d30 2e35  525 -0.1008,-0.5
-00007790: 3134 3034 3320 2d30 2e30 3931 332c 2d31  14043 -0.0913,-1
-000077a0: 2e33 3636 3933 3520 302e 3032 3131 2c2d  .366935 0.0211,-
-000077b0: 312e 3839 3438 3034 2030 2e33 3438 3136  1.894804 0.34816
-000077c0: 2c2d 312e 3633 3438 3134 2031 2e33 3837  ,-1.634814 1.387
-000077d0: 3435 2c2d 322e 3831 3830 3536 2032 2e39  45,-2.818056 2.9
-000077e0: 3032 3839 2c2d 332e 3330 3439 3435 2030  0289,-3.304945 0
-000077f0: 2e36 3830 3633 2c2d 302e 3231 3836 3738  .68063,-0.218678
-00007800: 2030 2e39 3331 3638 2c2d 302e 3234 3232   0.93168,-0.2422
-00007810: 3338 2032 2e38 3130 3336 2c2d 302e 3236  38 2.81036,-0.26
-00007820: 3337 3438 206c 2031 2e37 3139 3537 2c2d  3748 l 1.71957,-
-00007830: 302e 3031 3936 3920 7620 342e 3532 3435  0.01969 v 4.5245
-00007840: 3337 2034 2e35 3234 3533 3820 6c20 2d31  37 4.524538 l -1
-00007850: 2e36 3031 3636 2c2d 302e 3030 3633 2063  .60166,-0.0063 c
-00007860: 202d 302e 3838 3039 312c 2d30 2e30 3033   -0.88091,-0.003
-00007870: 3520 2d31 2e36 3633 3535 2c2d 302e 3031  5 -1.66355,-0.01
-00007880: 3233 3620 2d31 2e37 3339 3231 2c2d 302e  236 -1.73921,-0.
-00007890: 3031 3937 3420 7a22 0a20 2020 2020 2020  01974 z".       
-000078a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000078b0: 220a 2020 2020 2020 2020 2020 2020 2073  ".             s
-000078c0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-000078d0: 733d 2263 7373 6373 7363 6363 6363 6322  s="csscsscccccc"
-000078e0: 202f 3e0a 2020 2020 2020 2020 2020 3c70   />.          <p
-000078f0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-00007900: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
-00007910: 302e 3939 3b66 696c 6c3a 2362 3662 3139  0.99;fill:#b6b19
-00007920: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00007930: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00007940: 6f6b 652d 7769 6474 683a 302e 3137 3637  oke-width:0.1767
-00007950: 3737 3b73 7472 6f6b 652d 6c69 6e65 6361  77;stroke-lineca
-00007960: 703a 726f 756e 643b 7374 726f 6b65 2d6d  p:round;stroke-m
-00007970: 6974 6572 6c69 6d69 743a 332e 343b 7374  iterlimit:3.4;st
-00007980: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00007990: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-000079a0: 7479 3a31 220a 2020 2020 2020 2020 2020  ty:1".          
-000079b0: 2020 2064 3d22 6d20 3232 362e 3430 3233     d="m 226.4023
-000079c0: 322c 3236 2e36 3733 3539 3320 6320 302e  2,26.673593 c 0.
-000079d0: 3031 3735 2c2d 302e 3039 3137 3120 2d30  0175,-0.09171 -0
-000079e0: 2e30 3339 312c 2d30 2e35 3137 3633 3320  .0391,-0.517633 
-000079f0: 2d30 2e30 3931 352c 2d30 2e36 3838 3738  -0.0915,-0.68878
-00007a00: 202d 302e 3039 3939 2c2d 302e 3332 3537   -0.0999,-0.3257
-00007a10: 3633 202d 302e 3238 3338 312c 2d30 2e36  63 -0.28381,-0.6
-00007a20: 3234 3538 3620 2d30 2e35 3332 3034 2c2d  24586 -0.53204,-
-00007a30: 302e 3836 3433 3436 202d 302e 3134 3731  0.864346 -0.1471
-00007a40: 322c 2d30 2e31 3432 3039 3920 2d30 2e34  2,-0.142099 -0.4
-00007a50: 3433 3134 2c2d 302e 3333 3230 3231 202d  4314,-0.332021 -
-00007a60: 302e 3631 3233 342c 2d30 2e33 3932 3836  0.61234,-0.39286
-00007a70: 3520 2d30 2e30 3632 392c 2d30 2e30 3232  5 -0.0629,-0.022
-00007a80: 3633 202d 302e 3131 3434 2c2d 302e 3034  63 -0.1144,-0.04
-00007a90: 3736 3520 2d30 2e31 3134 342c 2d30 2e30  765 -0.1144,-0.0
-00007aa0: 3535 3620 302c 2d30 2e30 3038 2030 2e30  556 0,-0.008 0.0
-00007ab0: 3535 332c 2d30 2e30 3337 3338 2030 2e31  553,-0.03738 0.1
-00007ac0: 3232 3737 2c2d 302e 3036 3533 3820 302e  2277,-0.06538 0.
-00007ad0: 3238 3134 392c 2d30 2e31 3136 3733 3220  28149,-0.116732 
-00007ae0: 302e 3633 3539 392c 2d30 2e34 3034 3938  0.63599,-0.40498
-00007af0: 3920 302e 3832 3338 312c 2d30 2e36 3639  9 0.82381,-0.669
-00007b00: 3836 3120 302e 3434 3931 362c 2d30 2e36  861 0.44916,-0.6
-00007b10: 3333 3434 3520 302e 3535 3536 322c 2d31  33445 0.55562,-1
-00007b20: 2e34 3833 3237 3420 302e 3238 3137 392c  .483274 0.28179,
-00007b30: 2d32 2e32 3439 3430 3520 2d30 2e31 3835  -2.249405 -0.185
-00007b40: 392c 2d30 2e35 3230 3132 3920 2d30 2e35  9,-0.520129 -0.5
-00007b50: 3633 3232 2c2d 302e 3936 3831 3132 202d  6322,-0.968112 -
-00007b60: 312e 3032 3137 342c 2d31 2e32 3133 3039  1.02174,-1.21309
-00007b70: 3820 6c20 2d30 2e31 3338 3633 2c2d 302e  8 l -0.13863,-0.
-00007b80: 3037 3430 3720 302e 3135 3839 332c 2d30  07407 0.15893,-0
-00007b90: 2e30 3431 3436 2063 2030 2e33 3834 3935  .04146 c 0.38495
-00007ba0: 2c2d 302e 3130 3034 3232 2030 2e37 3235  ,-0.100422 0.725
-00007bb0: 3734 2c2d 302e 3333 3133 3038 2030 2e38  74,-0.331308 0.8
-00007bc0: 3438 3639 2c2d 302e 3537 3439 3838 2030  4869,-0.574988 0
-00007bd0: 2e30 3239 2c2d 302e 3035 3733 3920 302e  .029,-0.05739 0.
-00007be0: 3035 3533 2c2d 302e 3130 3734 3037 2030  0553,-0.107407 0
-00007bf0: 2e30 3538 352c 2d30 2e31 3131 3134 3220  .0585,-0.111142 
-00007c00: 302e 3030 332c 2d30 2e30 3033 3720 312e  0.003,-0.0037 1.
-00007c10: 3338 3938 362c 302e 3739 3232 3431 2033  38986,0.792241 3
-00007c20: 2e30 3831 3432 2c31 2e37 3638 3833 3620  .08142,1.768836 
-00007c30: 312e 3639 3135 352c 302e 3937 3635 3935  1.69155,0.976595
-00007c40: 2033 2e30 3932 3335 2c31 2e37 3835 3033   3.09235,1.78503
-00007c50: 3420 332e 3131 3239 2c31 2e37 3936 3533  4 3.1129,1.79653
-00007c60: 3120 302e 3032 3832 2c30 2e30 3135 3831  1 0.0282,0.01581
-00007c70: 202d 302e 3639 3236 352c 302e 3434 3234   -0.69265,0.4424
-00007c80: 3439 202d 322e 3935 3832 392c 312e 3735  49 -2.95829,1.75
-00007c90: 3037 3720 2d31 2e36 3437 362c 302e 3935  077 -1.6476,0.95
-00007ca0: 3134 3236 202d 332e 3030 3336 2c31 2e37  1426 -3.0036,1.7
-00007cb0: 3332 3931 3420 2d33 2e30 3133 3333 2c31  32914 -3.01333,1
-00007cc0: 2e37 3336 3633 3920 2d30 2e30 312c 302e  .736639 -0.01,0.
-00007cd0: 3030 3337 202d 302e 3031 3237 2c2d 302e  0037 -0.0127,-0.
-00007ce0: 3031 3935 3820 2d30 2e30 3037 2c2d 302e  01958 -0.007,-0.
-00007cf0: 3035 3137 3820 7a22 0a20 2020 2020 2020  05178 z".       
-00007d00: 2020 2020 2020 6964 3d22 7061 7468 3138        id="path18
-00007d10: 220a 2020 2020 2020 2020 2020 2020 2073  ".             s
-00007d20: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00007d30: 733d 2263 6373 7373 6373 7373 6373 7363  s="ccssscssscssc
-00007d40: 7373 7363 6363 2220 2f3e 0a20 2020 2020  sssccc" />.     
-00007d50: 2020 203c 2f67 3e0a 2020 2020 2020 3c2f     </g>.      </
-00007d60: 673e 0a20 2020 2020 203c 7061 7468 0a20  g>.      <path. 
-00007d70: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00007d80: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
-00007d90: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00007da0: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00007db0: 6474 683a 302e 3135 3330 3531 7078 3b73  dth:0.153051px;s
-00007dc0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00007dd0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00007de0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00007df0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00007e00: 2020 2020 643d 226d 2031 3938 2e33 3237      d="m 198.327
-00007e10: 3538 2c32 2e30 3837 3539 3239 202d 332e  58,2.0875929 -3.
-00007e20: 3138 3739 322c 2d30 2e33 3335 3736 3720  18792,-0.335767 
-00007e30: 312e 3131 3231 332c 322e 3836 3539 3935  1.11213,2.865995
-00007e40: 207a 220a 2020 2020 2020 2020 2069 643d   z".         id=
-00007e50: 2270 6174 6831 3922 202f 3e0a 2020 2020  "path19" />.    
-00007e60: 3c2f 673e 0a20 2020 203c 7061 7468 0a20  </g>.    <path. 
-00007e70: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00007e80: 6c3a 2365 3039 6331 383b 6669 6c6c 2d6f  l:#e09c18;fill-o
-00007e90: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00007ea0: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-00007eb0: 683a 302e 3236 3435 3833 7078 3b73 7472  h:0.264583px;str
-00007ec0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00007ed0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00007ee0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
-00007ef0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00007f00: 643d 226d 2039 362e 3530 3236 3339 2c35  d="m 96.502639,5
-00007f10: 372e 3537 3033 3438 2063 202d 332e 3932  7.570348 c -3.92
-00007f20: 3636 3632 2c2d 302e 3539 3535 3836 202d  6662,-0.595586 -
-00007f30: 372e 3839 3337 3337 2c2d 342e 3532 3731  7.893737,-4.5271
-00007f40: 3332 202d 382e 3338 3130 3334 2c2d 382e  32 -8.381034,-8.
-00007f50: 3436 3836 3938 202d 302e 3338 3737 3535  468698 -0.387755
-00007f60: 2c2d 332e 3133 3634 3032 2031 2e38 3938  ,-3.136402 1.898
-00007f70: 3531 392c 2d36 2e39 3732 3134 3420 342e  519,-6.972144 4.
-00007f80: 3832 3730 3536 2c2d 382e 3136 3030 3135  827056,-8.160015
-00007f90: 2034 2e31 3732 3132 352c 2d31 2e36 3932   4.172125,-1.692
-00007fa0: 3239 3420 3130 2e30 3633 3535 392c 302e  294 10.063559,0.
-00007fb0: 3136 3436 3339 2031 332e 3033 3230 3339  164639 13.032039
-00007fc0: 2c33 2e35 3439 3639 3820 312e 3636 3036  ,3.549698 1.6606
-00007fd0: 342c 312e 3839 3336 3931 2032 2e31 3634  4,1.893691 2.164
-00007fe0: 3538 2c35 2e32 3435 3334 3220 312e 3031  58,5.245342 1.01
-00007ff0: 3638 362c 372e 3438 3733 3420 2d31 2e38  686,7.48734 -1.8
-00008000: 3036 3235 2c33 2e35 3238 3431 3220 2d36  0625,3.528412 -6
-00008010: 2e35 3735 3838 2c36 2e31 3836 3130 3620  .57588,6.186106 
-00008020: 2d31 302e 3439 3439 3231 2c35 2e35 3931  -10.494921,5.591
-00008030: 3637 3520 7a22 0a20 2020 2020 2020 6964  675 z".       id
-00008040: 3d22 7061 7468 3434 220a 2020 2020 2020  ="path44".      
-00008050: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00008060: 7065 733d 2273 7373 7373 7322 202f 3e0a  pes="ssssss" />.
-00008070: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00008080: 2073 7479 6c65 3d22 6669 6c6c 3a23 3738   style="fill:#78
-00008090: 3434 3231 3b73 7472 6f6b 653a 6e6f 6e65  4421;stroke:none
-000080a0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000080b0: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
-000080c0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000080d0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-000080e0: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-000080f0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00008100: 2031 3035 2e38 3635 3234 2c35 312e 3430   105.86524,51.40
-00008110: 3430 3436 2063 202d 332e 3234 3431 372c  4046 c -3.24417,
-00008120: 2d34 2e35 3830 3738 202d 352e 3331 3235  -4.58078 -5.3125
-00008130: 312c 2d35 2e30 3832 3335 3920 2d39 2e31  1,-5.082359 -9.1
-00008140: 3532 3736 362c 2d33 2e31 3232 3536 3520  52766,-3.122565 
-00008150: 2d35 2e31 3237 3235 342c 322e 3631 3635  -5.127254,2.6165
-00008160: 3836 202d 332e 3238 3635 3033 2c34 2e39  86 -3.286503,4.9
-00008170: 3339 3936 3320 2d31 2e36 3032 3332 332c  39963 -1.602323,
-00008180: 382e 3637 3634 3133 202d 352e 3234 3336  8.676413 -5.2436
-00008190: 3731 2c2d 322e 3735 3932 3232 202d 392e  71,-2.759222 -9.
-000081a0: 3630 3530 3539 2c2d 3131 2e33 3235 3731  605059,-11.32571
-000081b0: 3620 2d33 2e39 3430 3236 322c 2d31 342e  6 -3.940262,-14.
-000081c0: 3738 3436 3036 2038 2e34 3036 3937 342c  784606 8.406974,
-000081d0: 2d35 2e31 3333 3234 3620 3134 2e33 3333  -5.133246 14.333
-000081e0: 3830 312c 332e 3438 3738 3235 2031 342e  801,3.487825 14.
-000081f0: 3639 3533 3531 2c39 2e32 3330 3735 3820  695351,9.230758 
-00008200: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-00008210: 7468 3230 2d33 220a 2020 2020 2020 2073  th20-3".       s
-00008220: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00008230: 733d 2263 7363 7363 2220 2f3e 0a20 2020  s="cscsc" />.   
-00008240: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00008250: 796c 653d 2266 696c 6c3a 2330 3030 3030  yle="fill:#00000
-00008260: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00008270: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00008280: 6f6b 652d 7769 6474 683a 302e 3237 3734  oke-width:0.2774
-00008290: 3039 7078 3b73 7472 6f6b 652d 6c69 6e65  09px;stroke-line
-000082a0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-000082b0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-000082c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-000082d0: 0a20 2020 2020 2020 643d 226d 2038 362e  .       d="m 86.
-000082e0: 3031 3830 3335 2c34 382e 3132 3234 3237  018035,48.122427
-000082f0: 2063 202d 302e 3133 3232 3135 2c2d 342e   c -0.132215,-4.
-00008300: 3035 3239 3438 2032 2e38 3231 3432 332c  052948 2.821423,
-00008310: 2d37 2e35 3738 3734 3820 362e 3534 3635  -7.578748 6.5465
-00008320: 3937 2c2d 382e 3934 3037 3439 2031 2e39  97,-8.940749 1.9
-00008330: 3731 3036 322c 2d30 2e37 3230 3636 3120  71062,-0.720661 
-00008340: 3131 2e30 3239 3833 382c 2d30 2e35 3533  11.029838,-0.553
-00008350: 3931 2031 332e 3638 3034 3638 2c33 2e38  91 13.680468,3.8
-00008360: 3235 3331 3520 312e 3238 3638 332c 322e  25315 1.28683,2.
-00008370: 3132 3630 3236 2032 2e32 3336 3339 2c36  126026 2.23639,6
-00008380: 2e31 3938 3139 3520 2d30 2e35 3132 3332  .198195 -0.51232
-00008390: 2c39 2e31 3838 3938 3720 2d30 2e35 3230  ,9.188987 -0.520
-000083a0: 352c 2d34 2e37 3333 3235 3720 2d32 2e33  5,-4.733257 -2.3
-000083b0: 3434 3432 2c2d 362e 3934 3930 3338 202d  4442,-6.949038 -
-000083c0: 332e 3133 3638 382c 2d37 2e36 3533 3534  3.13688,-7.65354
-000083d0: 3220 2d32 2e38 3531 3232 372c 2d32 2e35  2 -2.851227,-2.5
-000083e0: 3334 3738 3920 2d38 2e37 3434 3833 382c  34789 -8.744838,
-000083f0: 2d32 2e37 3734 3036 3520 2d31 312e 3532  -2.774065 -11.52
-00008400: 3535 3235 2c2d 302e 3136 3230 3832 202d  5525,-0.162082 -
-00008410: 312e 3733 3538 372c 312e 3633 3035 3535  1.73587,1.630555
-00008420: 202d 322e 3336 3239 3832 2c33 2e39 3331   -2.362982,3.931
-00008430: 3432 3520 2d30 2e30 3738 3338 2c36 2e39  425 -0.07838,6.9
-00008440: 3835 3133 3720 312e 3232 3336 3033 2c31  85137 1.223603,1
-00008450: 2e36 3335 3533 2032 2e35 3031 3532 352c  .63553 2.501525,
-00008460: 342e 3539 3138 3036 2036 2e38 3332 3930  4.591806 6.83290
-00008470: 342c 362e 3635 3332 3931 202d 352e 3632  4,6.653291 -5.62
-00008480: 3639 3434 2c2d 302e 3231 3139 3935 202d  6944,-0.211995 -
-00008490: 3131 2e36 3733 3636 392c 2d35 2e38 3133  11.673669,-5.813
-000084a0: 3432 3720 2d31 312e 3830 3638 3632 2c2d  427 -11.806862,-
-000084b0: 392e 3839 3633 3537 207a 220a 2020 2020  9.896357 z".    
-000084c0: 2020 2069 643d 2270 6174 6835 220a 2020     id="path5".  
-000084d0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-000084e0: 6465 7479 7065 733d 2273 7373 6373 7373  detypes="ssscsss
-000084f0: 6373 2220 2f3e 0a20 2020 203c 7061 7468  cs" />.    <path
-00008500: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00008510: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
-00008520: 2d6f 7061 6369 7479 3a30 2e39 3934 3735  -opacity:0.99475
-00008530: 333b 7374 726f 6b65 3a6e 6f6e 653b 7374  3;stroke:none;st
-00008540: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
-00008550: 3538 3370 783b 7374 726f 6b65 2d6c 696e  583px;stroke-lin
-00008560: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00008570: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00008580: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00008590: 220a 2020 2020 2020 2064 3d22 6d20 3434  ".       d="m 44
-000085a0: 2e31 3631 3433 392c 3137 322e 3636 3931  .161439,172.6691
-000085b0: 3120 6320 302e 3535 3936 3432 2c2d 312e  1 c 0.559642,-1.
-000085c0: 3935 3233 3320 2d30 2e38 3036 3432 312c  95233 -0.806421,
-000085d0: 2d37 2e33 3135 3639 202d 312e 3432 3434  -7.31569 -1.4244
-000085e0: 3436 2c2d 382e 3232 3037 3620 2d31 2e38  46,-8.22076 -1.8
-000085f0: 3438 3239 322c 322e 3230 3235 3720 2d32  48292,2.20257 -2
-00008600: 2e30 3937 3435 362c 322e 3233 3932 3720  .097456,2.23927 
-00008610: 2d32 2e38 3734 3639 362c 322e 3530 3632  -2.874696,2.5062
-00008620: 3220 302e 3136 3537 3038 2c2d 302e 3639  2 0.165708,-0.69
-00008630: 3038 3920 302e 3737 3137 3135 2c2d 302e  089 0.771715,-0.
-00008640: 3935 3639 3420 302e 3032 3034 312c 2d32  95694 0.02041,-2
-00008650: 2e34 3032 3535 202d 302e 3736 3334 3932  .40255 -0.763492
-00008660: 2c32 2e32 3339 3739 202d 322e 3439 3734  ,2.23979 -2.4974
-00008670: 3439 2c33 2e36 3032 3332 202d 342e 3630  49,3.60232 -4.60
-00008680: 3935 3736 2c34 2e39 3231 3336 2030 2e35  9576,4.92136 0.5
-00008690: 3331 3833 342c 2d31 2e36 3030 3232 2031  31834,-1.60022 1
-000086a0: 2e33 3336 3938 362c 2d33 2e32 3634 3720  .336986,-3.2647 
-000086b0: 302e 3730 3737 3733 2c2d 342e 3631 3932  0.707773,-4.6192
-000086c0: 3420 2d30 2e35 3638 3531 372c 302e 3736  4 -0.568517,0.76
-000086d0: 3432 3420 2d31 2e32 3635 3639 362c 312e  424 -1.265696,1.
-000086e0: 3038 3131 3920 2d31 2e39 3832 3935 362c  08119 -1.982956,
-000086f0: 312e 3332 3833 3420 312e 3438 3434 372c  1.32834 1.48447,
-00008700: 2d32 2e37 3034 3634 2030 2e35 3233 3839  -2.70464 0.52389
-00008710: 342c 2d33 2e32 3635 3633 2030 2e32 3335  4,-3.26563 0.235
-00008720: 3635 312c 2d34 2e33 3437 3431 202d 312e  651,-4.34741 -1.
-00008730: 3838 3137 3039 2c32 2e34 3038 3635 202d  881709,2.40865 -
-00008740: 332e 3538 3435 3431 2c32 2e38 3738 3431  3.584541,2.87841
-00008750: 202d 352e 3532 3133 3034 2c33 2e38 3430   -5.521304,3.840
-00008760: 3337 2030 2e35 3435 3232 312c 2d31 2e39  37 0.545221,-1.9
-00008770: 3332 3334 2030 2e33 3838 3635 372c 2d33  3234 0.388657,-3
-00008780: 2e35 3238 3939 202d 302e 3436 3036 3435  .52899 -0.460645
-00008790: 2c2d 342e 3937 3837 202d 312e 3530 3537  ,-4.9787 -1.5057
-000087a0: 3533 2c31 2e33 3937 3038 202d 332e 3230  53,1.39708 -3.20
-000087b0: 3236 3533 2c31 2e33 3139 3239 202d 342e  2653,1.31929 -4.
-000087c0: 3033 3139 392c 302e 3937 3339 3120 322e  03199,0.97391 2.
-000087d0: 3039 3335 3537 2c2d 312e 3533 3738 3220  093557,-1.53782 
-000087e0: 322e 3432 3637 3335 2c2d 332e 3139 3834  2.426735,-3.1984
-000087f0: 3820 312e 3439 3431 3032 2c2d 352e 3337  8 1.494102,-5.37
-00008800: 3733 3920 2d31 2e35 3739 3839 352c 332e  739 -1.579895,3.
-00008810: 3632 3339 3920 2d33 2e38 3839 3832 392c  62399 -3.889829,
-00008820: 342e 3837 3338 3520 2d36 2e37 3939 3330  4.87385 -6.79930
-00008830: 332c 362e 3134 3333 3620 302e 3737 3335  3,6.14336 0.7735
-00008840: 3835 2c2d 312e 3338 3035 3520 312e 3935  85,-1.38055 1.95
-00008850: 3033 3339 2c2d 322e 3734 3639 3520 322e  0339,-2.74695 2.
-00008860: 3138 3130 3538 2c2d 342e 3030 3733 3920  181058,-4.00739 
-00008870: 2d30 2e35 3234 3338 332c 302e 3231 3934  -0.524383,0.2194
-00008880: 3320 2d30 2e39 3239 3339 372c 302e 3338  3 -0.929397,0.38
-00008890: 3536 3120 2d31 2e33 3431 3537 362c 302e  561 -1.341576,0.
-000088a0: 3235 3438 3620 322e 3239 3031 3833 2c2d  25486 2.290183,-
-000088b0: 322e 3730 3838 3720 312e 3333 3834 3839  2.70887 1.338489
-000088c0: 2c2d 342e 3833 3932 3920 302e 3831 3433  ,-4.83929 0.8143
-000088d0: 3539 2c2d 362e 3330 3532 202d 312e 3534  59,-6.3052 -1.54
-000088e0: 3739 312c 312e 3237 3339 3620 2d32 2e39  791,1.27396 -2.9
-000088f0: 3634 3535 362c 312e 3934 3430 3220 2d34  64556,1.94402 -4
-00008900: 2e37 3236 3438 352c 322e 3338 3130 3620  .726485,2.38106 
-00008910: 302e 3636 3730 3332 2c2d 322e 3236 3537  0.667032,-2.2657
-00008920: 3920 312e 3030 3834 332c 2d34 2e33 3233  9 1.00843,-4.323
-00008930: 3637 202d 302e 3539 3131 362c 2d37 2e30  67 -0.59116,-7.0
-00008940: 3936 3136 202d 312e 3034 3932 3437 2c30  9616 -1.049247,0
-00008950: 2e37 3432 3432 202d 312e 3233 3535 3339  .74242 -1.235539
-00008960: 2c31 2e33 3634 3439 202d 332e 3436 3938  ,1.36449 -3.4698
-00008970: 3631 2c31 2e36 3033 3733 2031 2e32 3633  61,1.60373 1.263
-00008980: 3730 332c 2d32 2e36 3531 3920 302e 3535  703,-2.6519 0.55
-00008990: 3735 3738 2c2d 342e 3935 3837 2030 2e31  7578,-4.9587 0.1
-000089a0: 3935 3937 382c 2d37 2e33 3031 3533 202d  95978,-7.30153 -
-000089b0: 312e 3639 3237 3537 2c32 2e37 3739 3231  1.692757,2.77921
-000089c0: 202d 312e 3938 3532 3534 382c 332e 3532   -1.9852548,3.52
-000089d0: 3437 3320 2d34 2e36 3136 3630 3738 2c33  473 -4.6166078,3
-000089e0: 2e39 3230 3431 2031 2e34 3430 3238 382c  .92041 1.440288,
-000089f0: 2d32 2e32 3231 3736 2030 2e30 3736 3338  -2.22176 0.07638
-00008a00: 2c2d 342e 3830 3732 3120 2d31 2e32 3139  ,-4.80721 -1.219
-00008a10: 3632 342c 2d36 2e39 3433 3836 2032 2e30  624,-6.94386 2.0
-00008a20: 3239 3035 362c 302e 3331 3439 3720 332e  29056,0.31497 3.
-00008a30: 3339 3830 3331 2c33 2e34 3135 3920 312e  398031,3.4159 1.
-00008a40: 3731 3233 3735 2c36 2e35 3432 3136 2032  712375,6.54216 2
-00008a50: 2e31 3436 3933 382c 2d30 2e34 3132 3837  .146938,-0.41287
-00008a60: 2032 2e37 3736 3239 3038 2c2d 332e 3236   2.7762908,-3.26
-00008a70: 3432 3220 332e 3933 3038 3831 382c 2d35  422 3.9308818,-5
-00008a80: 2e32 3731 3631 2031 2e33 3930 3331 372c  .27161 1.390317,
-00008a90: 322e 3431 3834 3520 322e 3839 3032 3631  2.41845 2.890261
-00008aa0: 2c34 2e35 3433 3738 2030 2e35 3432 3530  ,4.54378 0.54250
-00008ab0: 362c 382e 3632 3633 3120 6c20 332e 3032  6,8.62631 l 3.02
-00008ac0: 3439 3337 2c2d 322e 3930 3831 3620 6320  4937,-2.90816 c 
-00008ad0: 312e 3038 3632 322c 322e 3235 3037 2033  1.08622,2.2507 3
-00008ae0: 2e31 3831 3137 342c 332e 3736 3637 3420  .181174,3.76674 
-00008af0: 312e 3031 3936 3134 2c38 2e33 3832 3835  1.019614,8.38285
-00008b00: 206c 2034 2e31 3537 3931 322c 2d33 2e38   l 4.157912,-3.8
-00008b10: 3639 3334 2063 2031 2e33 3137 3436 2c32  6934 c 1.31746,2
-00008b20: 2e31 3439 3436 2032 2e38 3935 3132 342c  .14946 2.895124,
-00008b30: 332e 3436 3830 3220 2d30 2e31 3938 3736  3.46802 -0.19876
-00008b40: 312c 372e 3933 3334 3120 6c20 312e 3930  1,7.93341 l 1.90
-00008b50: 3038 3637 2c2d 312e 3631 3232 3820 6320  0867,-1.61228 c 
-00008b60: 2d30 2e36 3537 3136 352c 312e 3734 3635  -0.657165,1.7465
-00008b70: 202d 312e 3337 3533 3336 2c33 2e34 3732   -1.375336,3.472
-00008b80: 3931 202d 322e 3635 3131 3238 2c35 2e30  91 -2.651128,5.0
-00008b90: 3135 3732 2033 2e36 3430 3135 312c 2d31  1572 3.640151,-1
-00008ba0: 2e35 3136 3335 2034 2e33 3735 3937 322c  .51635 4.375972,
-00008bb0: 2d35 2e32 3239 3536 2035 2e39 3631 3832  -5.22956 5.96182
-00008bc0: 372c 2d38 2e32 3939 3739 2032 2e32 3632  7,-8.29979 2.262
-00008bd0: 3136 352c 322e 3536 3435 2031 2e36 3837  165,2.5645 1.687
-00008be0: 3933 372c 362e 3837 3732 3620 2d30 2e39  937,6.87726 -0.9
-00008bf0: 3932 3431 332c 382e 3135 3334 3120 322e  92413,8.15341 2.
-00008c00: 3631 3931 3434 2c30 2e31 3432 3737 2033  619144,0.14277 3
-00008c10: 2e32 3331 3230 362c 2d31 2e38 3531 3534  .231206,-1.85154
-00008c20: 2033 2e39 3634 3035 322c 2d33 2e30 3731   3.964052,-3.071
-00008c30: 3520 302e 3639 3430 3639 2c31 2e32 3130  5 0.694069,1.210
-00008c40: 3720 322e 3133 3431 3536 2c33 2e32 3433  7 2.134156,3.243
-00008c50: 3435 2030 2e36 3235 3533 382c 362e 3539  45 0.625538,6.59
-00008c60: 3534 3420 312e 3639 3037 3533 2c2d 302e  544 1.690753,-0.
-00008c70: 3633 3139 3220 332e 3738 3838 3237 2c2d  63192 3.788827,-
-00008c80: 332e 3137 3731 3620 352e 3235 3338 3538  3.17716 5.253858
-00008c90: 2c2d 352e 3036 3936 3220 302e 3831 3939  ,-5.06962 0.8199
-00008ca0: 3531 2c31 2e37 3831 3436 2031 2e34 3735  51,1.78146 1.475
-00008cb0: 3836 362c 332e 3837 3332 3620 302e 3131  866,3.87326 0.11
-00008cc0: 3439 3534 2c35 2e35 3939 3239 2030 2e39  4954,5.59929 0.9
-00008cd0: 3738 3237 332c 2d30 2e35 3639 3637 2031  78273,-0.56967 1
-00008ce0: 2e31 3233 3834 372c 2d31 2e34 3339 3720  .123847,-1.4397 
-00008cf0: 312e 3438 3836 3137 2c2d 322e 3233 3036  1.488617,-2.2306
-00008d00: 3620 312e 3035 3931 3931 2c32 2e35 3131  6 1.059191,2.511
-00008d10: 3038 2030 2e36 3833 3832 342c 332e 3630  08 0.683824,3.60
-00008d20: 3135 3220 2d30 2e33 3938 3333 352c 352e  152 -0.398335,5.
-00008d30: 3535 3731 3320 302e 3430 3037 3432 2c2d  55713 0.400742,-
-00008d40: 302e 3034 3838 2033 2e31 3534 3839 362c  0.0488 3.154896,
-00008d50: 2d32 2e36 3636 3520 342e 3330 3936 3232  -2.6665 4.309622
-00008d60: 2c2d 352e 3334 3932 3820 302c 3020 312e  ,-5.34928 0,0 1.
-00008d70: 3133 3439 3837 2c31 2e37 3939 3533 2030  134987,1.79953 0
-00008d80: 2e32 3139 3831 392c 332e 3032 3532 3720  .219819,3.02527 
-00008d90: 302e 3633 3439 332c 2d30 2e33 3438 3632  0.63493,-0.34862
-00008da0: 2032 2e36 3733 3030 382c 2d33 2e36 3935   2.673008,-3.695
-00008db0: 3333 2032 2e36 3733 3030 382c 2d33 2e36  33 2.673008,-3.6
-00008dc0: 3935 3333 2032 2e39 3732 3234 362c 352e  9533 2.972246,5.
-00008dd0: 3736 3739 3620 322e 3038 3939 3236 2c38  76796 2.089926,8
-00008de0: 2e31 3930 3938 2031 2e33 3631 3134 352c  .19098 1.361145,
-00008df0: 392e 3637 3331 3520 7a22 0a20 2020 2020  9.67315 z".     
-00008e00: 2020 6964 3d22 7061 7468 3622 0a20 2020    id="path6".   
-00008e10: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-00008e20: 6574 7970 6573 3d22 6363 6363 6363 6363  etypes="cccccccc
-00008e30: 6363 6363 6363 6363 6363 6363 6363 6363  cccccccccccccccc
-00008e40: 6363 6363 6363 6363 6363 6363 6363 6363  cccccccccccccccc
-00008e50: 6363 6363 2220 2f3e 0a20 2020 203c 7061  cccc" />.    <pa
-00008e60: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-00008e70: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-00008e80: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00008e90: 2d77 6964 7468 3a32 2e39 3b73 7472 6f6b  -width:2.9;strok
-00008ea0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00008eb0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00008ec0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00008ed0: 726c 696d 6974 3a33 2e34 3b73 7472 6f6b  rlimit:3.4;strok
-00008ee0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00008ef0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00008f00: 3122 0a20 2020 2020 2020 643d 226d 2031  1".       d="m 1
-00008f10: 3135 2e31 3933 3138 2c31 3033 2e32 3932  15.19318,103.292
-00008f20: 3135 2063 2030 2e38 3431 3431 2c2d 312e  15 c 0.84141,-1.
-00008f30: 3635 3437 3520 2d32 2e31 3434 3937 2c34  65475 -2.14497,4
-00008f40: 2e30 3232 3236 202d 342e 3233 3538 362c  .02226 -4.23586,
-00008f50: 342e 3638 3330 3820 302e 3237 3335 312c  4.68308 0.27351,
-00008f60: 2d32 2e36 3237 3636 202d 312e 3634 3033  -2.62766 -1.6403
-00008f70: 312c 2d38 2e31 3435 3437 202d 332e 3035  1,-8.14547 -3.05
-00008f80: 3236 382c 2d39 2e35 3137 3239 202d 302e  268,-9.51729 -0.
-00008f90: 3930 3836 362c 322e 3939 3438 202d 322e  90866,2.9948 -2.
-00008fa0: 3532 3839 312c 352e 3432 3435 3120 2d35  52891,5.42451 -5
-00008fb0: 2e32 3333 3436 2c36 2e34 3232 3936 2030  .23346,6.42296 0
-00008fc0: 2e34 3536 3135 2c2d 332e 3534 3634 3920  .45615,-3.54649 
-00008fd0: 2d30 2e35 3035 3536 2c2d 362e 3238 3034  -0.50556,-6.2804
-00008fe0: 3820 2d32 2e30 3934 3439 2c2d 392e 3333  8 -2.09449,-9.33
-00008ff0: 3838 3331 202d 312e 3639 3431 3534 2c32  8831 -1.694154,2
-00009000: 2e35 3735 3539 3120 2d33 2e33 3739 3133  .575591 -3.37913
-00009010: 382c 352e 3137 3336 3331 202d 352e 3835  8,5.173631 -5.85
-00009020: 3031 3934 2c35 2e38 3437 3432 3120 302e  0194,5.847421 0.
-00009030: 3438 3130 3133 2c2d 342e 3234 3834 3120  481013,-4.24841 
-00009040: 2d30 2e34 3330 3434 362c 2d38 2e33 3236  -0.430446,-8.326
-00009050: 3739 3420 2d32 2e31 3636 3335 322c 2d31  794 -2.166352,-1
-00009060: 322e 3330 3435 3035 202d 302e 3938 3630  2.304505 -0.9860
-00009070: 3636 2c32 2e38 3733 3439 3320 2d35 2e34  66,2.873493 -5.4
-00009080: 3330 3334 352c 372e 3130 3935 3238 202d  30345,7.109528 -
-00009090: 372e 3139 3038 3935 2c37 2e37 3838 3039  7.190895,7.78809
-000090a0: 3820 312e 3038 3333 3937 2c2d 322e 3635  8 1.083397,-2.65
-000090b0: 3333 3534 2032 2e33 3036 3134 332c 2d37  3354 2.306143,-7
-000090c0: 2e36 3037 3833 3420 312e 3637 3334 3137  .607834 1.673417
-000090d0: 2c2d 3130 2e36 3933 3531 3420 2d31 2e36  ,-10.693514 -1.6
-000090e0: 3033 3839 2c32 2e30 3838 3937 3920 2d34  0389,2.088979 -4
-000090f0: 2e33 3930 3238 392c 342e 3037 3534 3638  .390289,4.075468
-00009100: 202d 362e 3238 3531 3835 2c35 2e31 3431   -6.285185,5.141
-00009110: 3135 3520 302e 3935 3137 3935 2c2d 322e  155 0.951795,-2.
-00009120: 3436 3333 3331 2031 2e39 3039 3235 392c  463331 1.909259,
-00009130: 2d37 2e33 3438 3530 3720 302e 3439 3137  -7.348507 0.4917
-00009140: 3935 2c2d 3130 2e31 3036 3239 3420 2d31  95,-10.106294 -1
-00009150: 2e38 3830 3836 362c 332e 3032 3536 3738  .880866,3.025678
-00009160: 202d 332e 3535 3436 3938 2c34 2e31 3735   -3.554698,4.175
-00009170: 3232 202d 352e 3732 3530 3235 2c35 2e33  22 -5.725025,5.3
-00009180: 3634 3138 2031 2e34 3135 3435 2c2d 342e  6418 1.41545,-4.
-00009190: 3739 3234 3031 202d 302e 3232 3531 3737  792401 -0.225177
-000091a0: 2c2d 3133 2e30 3637 3831 3220 2d33 2e39  ,-13.067812 -3.9
-000091b0: 3033 3439 372c 2d31 322e 3732 3738 3420  03497,-12.72784 
-000091c0: 312e 3130 3432 3536 2c2d 312e 3336 3232  1.104256,-1.3622
-000091d0: 3520 322e 3331 3135 332c 2d32 2e35 3636  5 2.31153,-2.566
-000091e0: 3334 3920 322e 3739 3631 3737 2c2d 332e  349 2.796177,-3.
-000091f0: 3031 3335 3532 220a 2020 2020 2020 2069  013552".       i
-00009200: 643d 2270 6174 6837 220a 2020 2020 2020  d="path7".      
-00009210: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00009220: 7065 733d 2263 6363 6363 6363 6363 6363  pes="ccccccccccc
-00009230: 6363 6322 202f 3e0a 2020 2020 3c67 0a20  ccc" />.    <g. 
-00009240: 2020 2020 2020 6964 3d22 6734 3322 0a20        id="g43". 
-00009250: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00009260: 2274 7261 6e73 6c61 7465 282d 3837 2e36  "translate(-87.6
-00009270: 3733 3736 332c 3737 2e35 3032 3135 3829  73763,77.502158)
-00009280: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
-00009290: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-000092a0: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
-000092b0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-000092c0: 6964 7468 3a30 2e32 3634 3538 3370 783b  idth:0.264583px;
-000092d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-000092e0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-000092f0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00009300: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00009310: 2020 2020 2064 3d22 4d20 3135 2e30 3331       d="M 15.031
-00009320: 3834 332c 3133 2e30 3735 3634 3420 4320  843,13.075644 C 
-00009330: 3432 2e39 3036 3431 372c 3139 2e32 3839  42.906417,19.289
-00009340: 3036 3320 3739 2e36 3838 3036 362c 3138  063 79.688066,18
-00009350: 2e32 3437 3133 3720 3132 342e 3337 3831  .247137 124.3781
-00009360: 322c 3130 2e37 3633 3334 220a 2020 2020  2,10.76334".    
-00009370: 2020 2020 2069 643d 2270 6174 6832 220a       id="path2".
-00009380: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00009390: 693a 6e6f 6465 7479 7065 733d 2263 6322  i:nodetypes="cc"
-000093a0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-000093b0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-000093c0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-000093d0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000093e0: 7769 6474 683a 333b 7374 726f 6b65 2d6c  width:3;stroke-l
-000093f0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00009400: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-00009410: 723b 7374 726f 6b65 2d64 6173 6861 7272  r;stroke-dasharr
-00009420: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00009430: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00009440: 2020 2064 3d22 4d20 3130 2e37 3431 3836     d="M 10.74186
-00009450: 392c 3131 2e33 3330 3732 3920 4320 3139  9,11.330729 C 19
-00009460: 2e31 3832 3431 322c 382e 3431 3539 3730  .182412,8.415970
-00009470: 3120 3232 2e36 3730 3631 322c 352e 3036  1 22.670612,5.06
-00009480: 3732 3233 2035 352e 3336 3638 3535 2c34  7223 55.366855,4
-00009490: 2e32 3034 3333 3134 206c 2036 2e36 3437  .2043314 l 6.647
-000094a0: 3632 342c 382e 3632 3830 3730 3620 322e  624,8.6280706 2.
-000094b0: 3331 3932 3833 2c2d 392e 3136 3538 3133  319283,-9.165813
-000094c0: 3520 4320 3832 2e36 3937 3031 382c 332e  5 C 82.697018,3.
-000094d0: 3239 3738 3936 2039 372e 3337 3736 3338  297896 97.377638
-000094e0: 2c34 2e31 3136 3335 3537 2031 3039 2e39  ,4.1163557 109.9
-000094f0: 3233 3233 2c31 322e 3932 3932 3732 2031  2323,12.929272 1
-00009500: 3034 2e34 3235 3834 2c31 372e 3334 3737  04.42584,17.3477
-00009510: 3231 2031 3030 2e39 3730 3535 2c32 302e  21 100.97055,20.
-00009520: 3538 3330 3831 2038 372e 3039 3633 3339  583081 87.096339
-00009530: 2c32 352e 3030 3932 3031 2037 312e 3534  ,25.009201 71.54
-00009540: 3133 3939 2c32 392e 3937 3135 3033 2035  1399,29.971503 5
-00009550: 342e 3932 3733 3231 2c33 312e 3434 3331  4.927321,31.4431
-00009560: 3535 2033 342e 3231 3032 3431 2c32 352e  55 34.210241,25.
-00009570: 3635 3432 3138 2031 392e 3135 3632 3935  654218 19.156295
-00009580: 2c32 312e 3434 3737 3220 3134 2e31 3331  ,21.44772 14.131
-00009590: 3332 312c 3135 2e36 3739 3534 3120 3130  321,15.679541 10
-000095a0: 2e37 3431 3836 392c 3131 2e33 3330 3732  .741869,11.33072
-000095b0: 3920 5a22 0a20 2020 2020 2020 2020 6964  9 Z".         id
-000095c0: 3d22 7061 7468 3822 0a20 2020 2020 2020  ="path8".       
-000095d0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-000095e0: 7970 6573 3d22 6363 6363 6373 7363 2220  ypes="cccccssc" 
-000095f0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
-00009600: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00009610: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
-00009620: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00009630: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00009640: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
-00009650: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00009660: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00009670: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00009680: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00009690: 2020 2020 2020 2064 3d22 6d20 3130 382e         d="m 108.
-000096a0: 3736 3134 382c 3130 2e39 3138 3639 3520  76148,10.918695 
-000096b0: 6320 332e 3639 3534 312c 2d30 2e30 3435  c 3.69541,-0.045
-000096c0: 3833 2031 302e 3930 3131 382c 2d32 2e32  83 10.90118,-2.2
-000096d0: 3030 3035 3934 2031 302e 3930 3131 382c  000594 10.90118,
-000096e0: 2d32 2e32 3030 3035 3934 2031 2e37 3834  -2.2000594 1.784
-000096f0: 3131 2c32 2e33 3736 3033 3834 2034 2e30  11,2.3760384 4.0
-00009700: 3431 3936 2c33 2e36 3438 3133 3234 2036  4196,3.6481324 6
-00009710: 2e39 3936 3335 2c33 2e32 3937 3038 3834  .99635,3.2970884
-00009720: 206c 202d 3138 2e36 3338 3538 2c33 2e38   l -18.63858,3.8
-00009730: 3737 3630 3720 7a22 0a20 2020 2020 2020  77607 z".       
-00009740: 2020 6964 3d22 7061 7468 3922 0a20 2020    id="path9".   
-00009750: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00009760: 6f64 6574 7970 6573 3d22 6363 6363 6322  odetypes="ccccc"
-00009770: 202f 3e0a 2020 2020 3c2f 673e 0a20 203c   />.    </g>.  <
-00009780: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
+000003b0: 793d 2232 3130 2e39 3939 3939 220a 2020  y="210.99999".  
+000003c0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+000003d0: 6f77 2d77 6964 7468 3d22 3235 3334 220a  ow-width="2534".
+000003e0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
+000003f0: 6e64 6f77 2d68 6569 6768 743d 2231 3534  ndow-height="154
+00000400: 3222 0a20 2020 2020 696e 6b73 6361 7065  2".     inkscape
+00000410: 3a77 696e 646f 772d 783d 2234 3635 220a  :window-x="465".
+00000420: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
+00000430: 6e64 6f77 2d79 3d22 3239 3122 0a20 2020  ndow-y="291".   
+00000440: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
+00000450: 772d 6d61 7869 6d69 7a65 643d 2230 220a  w-maximized="0".
+00000460: 2020 2020 2069 6e6b 7363 6170 653a 6375       inkscape:cu
+00000470: 7272 656e 742d 6c61 7965 723d 226c 6179  rrent-layer="lay
+00000480: 6572 3122 0a20 2020 2020 7368 6f77 6775  er1".     showgu
+00000490: 6964 6573 3d22 7472 7565 2220 2f3e 0a20  ides="true" />. 
+000004a0: 203c 6465 6673 0a20 2020 2020 6964 3d22   <defs.     id="
+000004b0: 6465 6673 3222 3e0a 2020 2020 3c69 6e6b  defs2">.    <ink
+000004c0: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
+000004d0: 740a 2020 2020 2020 2065 6666 6563 743d  t.       effect=
+000004e0: 2274 6170 6572 5f73 7472 6f6b 6522 0a20  "taper_stroke". 
+000004f0: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
+00000500: 6666 6563 7434 220a 2020 2020 2020 2069  ffect4".       i
+00000510: 735f 7669 7369 626c 653d 2274 7275 6522  s_visible="true"
+00000520: 0a20 2020 2020 2020 6c70 6576 6572 7369  .       lpeversi
+00000530: 6f6e 3d22 3122 0a20 2020 2020 2020 7374  on="1".       st
+00000540: 726f 6b65 5f77 6964 7468 3d22 3422 0a20  roke_width="4". 
+00000550: 2020 2020 2020 7375 6270 6174 683d 2231        subpath="1
+00000560: 220a 2020 2020 2020 2061 7474 6163 685f  ".       attach_
+00000570: 7374 6172 743d 2230 2e35 3633 3636 3834  start="0.5636684
+00000580: 3422 0a20 2020 2020 2020 656e 645f 6f66  4".       end_of
+00000590: 6673 6574 3d22 302e 3632 3431 3136 3035  fset="0.62411605
+000005a0: 220a 2020 2020 2020 2073 7461 7274 5f73  ".       start_s
+000005b0: 6d6f 6f74 6869 6e67 3d22 302e 3422 0a20  moothing="0.4". 
+000005c0: 2020 2020 2020 656e 645f 736d 6f6f 7468        end_smooth
+000005d0: 696e 673d 2230 2e35 220a 2020 2020 2020  ing="0.5".      
+000005e0: 206a 6f69 6e74 7970 653d 2265 7874 7261   jointype="extra
+000005f0: 706f 6c61 7465 6422 0a20 2020 2020 2020  polated".       
+00000600: 7374 6172 745f 7368 6170 653d 2263 656e  start_shape="cen
+00000610: 7465 7222 0a20 2020 2020 2020 656e 645f  ter".       end_
+00000620: 7368 6170 653d 2263 656e 7465 7222 0a20  shape="center". 
+00000630: 2020 2020 2020 6d69 7465 725f 6c69 6d69        miter_limi
+00000640: 743d 2231 3030 2220 2f3e 0a20 203c 2f64  t="100" />.  </d
+00000650: 6566 733e 0a20 203c 670a 2020 2020 2069  efs>.  <g.     i
+00000660: 6e6b 7363 6170 653a 6c61 6265 6c3d 224c  nkscape:label="L
+00000670: 6179 6572 2031 220a 2020 2020 2069 6e6b  ayer 1".     ink
+00000680: 7363 6170 653a 6772 6f75 706d 6f64 653d  scape:groupmode=
+00000690: 226c 6179 6572 220a 2020 2020 2069 643d  "layer".     id=
+000006a0: 226c 6179 6572 3122 3e0a 2020 2020 3c75  "layer1">.    <u
+000006b0: 7365 0a20 2020 2020 2020 783d 2230 220a  se.       x="0".
+000006c0: 2020 2020 2020 2079 3d22 3022 0a20 2020         y="0".   
+000006d0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+000006e0: 2370 6174 6838 3938 352d 3822 0a20 2020  #path8985-8".   
+000006f0: 2020 2020 6964 3d22 7573 6532 3630 3136      id="use26016
+00000700: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
+00000710: 726d 3d22 7472 616e 736c 6174 6528 322e  rm="translate(2.
+00000720: 3333 3138 3034 382c 3330 2e31 3333 3537  3318048,30.13357
+00000730: 3529 2220 2f3e 0a20 2020 203c 7573 650a  5)" />.    <use.
+00000740: 2020 2020 2020 2078 3d22 3022 0a20 2020         x="0".   
+00000750: 2020 2020 793d 2230 220a 2020 2020 2020      y="0".      
+00000760: 2078 6c69 6e6b 3a68 7265 663d 2223 7061   xlink:href="#pa
+00000770: 7468 3839 3835 2d38 220a 2020 2020 2020  th8985-8".      
+00000780: 2069 643d 2275 7365 3236 3031 3022 0a20   id="use26010". 
+00000790: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+000007a0: 2274 7261 6e73 6c61 7465 2831 312e 3130  "translate(11.10
+000007b0: 3332 3038 2c32 342e 3132 3731 3229 2220  3208,24.12712)" 
+000007c0: 2f3e 0a20 2020 203c 7573 650a 2020 2020  />.    <use.    
+000007d0: 2020 2078 3d22 3022 0a20 2020 2020 2020     x="0".       
+000007e0: 793d 2230 220a 2020 2020 2020 2078 6c69  y="0".       xli
+000007f0: 6e6b 3a68 7265 663d 2223 7061 7468 3839  nk:href="#path89
+00000800: 3835 2d38 220a 2020 2020 2020 2069 643d  85-8".       id=
+00000810: 2275 7365 3236 3030 3822 0a20 2020 2020  "use26008".     
+00000820: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00000830: 6e73 6c61 7465 2837 2e30 3731 3534 3238  nslate(7.0715428
+00000840: 2c32 312e 3638 3139 3631 2922 202f 3e0a  ,21.681961)" />.
+00000850: 2020 2020 3c75 7365 0a20 2020 2020 2020      <use.       
+00000860: 783d 2230 220a 2020 2020 2020 2079 3d22  x="0".       y="
+00000870: 3022 0a20 2020 2020 2020 786c 696e 6b3a  0".       xlink:
+00000880: 6872 6566 3d22 2370 6174 6838 3938 3522  href="#path8985"
+00000890: 0a20 2020 2020 2020 6964 3d22 7573 6531  .       id="use1
+000008a0: 3838 3039 220a 2020 2020 2020 2074 7261  8809".       tra
+000008b0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+000008c0: 6528 3130 2e33 3930 3732 312c 3335 2e39  e(10.390721,35.9
+000008d0: 3737 3332 3729 2220 2f3e 0a20 2020 203c  77327)" />.    <
+000008e0: 7573 650a 2020 2020 2020 2078 3d22 3022  use.       x="0"
+000008f0: 0a20 2020 2020 2020 793d 2230 220a 2020  .       y="0".  
+00000900: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00000910: 2223 7061 7468 3839 3835 220a 2020 2020  "#path8985".    
+00000920: 2020 2069 643d 2275 7365 3138 3830 3722     id="use18807"
+00000930: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00000940: 6d3d 2274 7261 6e73 6c61 7465 2831 372e  m="translate(17.
+00000950: 3334 3537 3036 2c33 342e 3738 3736 3837  345706,34.787687
+00000960: 2922 202f 3e0a 2020 2020 3c75 7365 0a20  )" />.    <use. 
+00000970: 2020 2020 2020 783d 2230 220a 2020 2020        x="0".    
+00000980: 2020 2079 3d22 3022 0a20 2020 2020 2020     y="0".       
+00000990: 786c 696e 6b3a 6872 6566 3d22 2370 6174  xlink:href="#pat
+000009a0: 6838 3938 3522 0a20 2020 2020 2020 6964  h8985".       id
+000009b0: 3d22 7573 6531 3838 3035 220a 2020 2020  ="use18805".    
+000009c0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000009d0: 616e 736c 6174 6528 3130 2e38 3031 3230  anslate(10.80120
+000009e0: 382c 3136 2e31 3433 3638 3829 2220 2f3e  8,16.143688)" />
+000009f0: 0a20 2020 203c 7573 650a 2020 2020 2020  .    <use.      
+00000a00: 2078 3d22 3022 0a20 2020 2020 2020 793d   x="0".       y=
+00000a10: 2230 220a 2020 2020 2020 2078 6c69 6e6b  "0".       xlink
+00000a20: 3a68 7265 663d 2223 7061 7468 3839 3835  :href="#path8985
+00000a30: 220a 2020 2020 2020 2069 643d 2275 7365  ".       id="use
+00000a40: 3138 3830 3322 0a20 2020 2020 2020 7472  18803".       tr
+00000a50: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00000a60: 7465 2831 372e 3635 3333 3737 2c31 372e  te(17.653377,17.
+00000a70: 3838 3538 3436 2922 202f 3e0a 2020 2020  885846)" />.    
+00000a80: 3c70 6174 680a 2020 2020 2020 2069 643d  <path.       id=
+00000a90: 2270 6174 6834 3139 2d33 220a 2020 2020  "path419-3".    
+00000aa0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00000ab0: 6330 3137 3030 3b66 696c 6c2d 6f70 6163  c01700;fill-opac
+00000ac0: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
+00000ad0: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
+00000ae0: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
+00000af0: 3a30 2e32 3634 3538 3470 783b 7374 726f  :0.264584px;stro
+00000b00: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00000b10: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00000b20: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00000b30: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00000b40: 3d22 6d20 2d33 322e 3736 3831 3432 2c31  ="m -32.768142,1
+00000b50: 382e 3730 3939 3435 2063 202d 312e 3539  8.709945 c -1.59
+00000b60: 3639 322c 302e 3735 3732 3237 2030 2e30  692,0.757227 0.0
+00000b70: 3035 2c35 2e34 3634 3333 3920 312e 3137  05,5.464339 1.17
+00000b80: 3131 352c 372e 3732 3434 3239 2031 2e35  115,7.724429 1.5
+00000b90: 3534 3835 2c33 2e30 3133 3439 3920 3133  5485,3.013499 13
+00000ba0: 2e37 3635 3039 2c31 342e 3136 3431 3139  .76509,14.164119
+00000bb0: 2032 322e 3039 3332 3239 372c 3134 2e30   22.0932297,14.0
+00000bc0: 3835 3831 3920 312e 3334 3336 382c 2d30  85819 1.34368,-0
+00000bd0: 2e30 3132 3420 332e 3435 3431 3839 2c2d  .0124 3.454189,-
+00000be0: 302e 3336 3634 3920 332e 3332 3936 372c  0.36649 3.32967,
+00000bf0: 2d31 2e37 3035 3238 202d 302e 3131 3238  -1.70528 -0.1128
+00000c00: 322c 2d31 2e32 3133 3637 202d 322e 3135  2,-1.21367 -2.15
+00000c10: 3338 2c2d 312e 3438 3636 3920 2d33 2e33  38,-1.48669 -3.3
+00000c20: 3638 3531 2c2d 312e 3537 3831 3920 2d38  6851,-1.57819 -8
+00000c30: 2e36 3730 3131 3937 2c2d 302e 3635 3330  .6701197,-0.6530
+00000c40: 3920 2d32 332e 3039 3137 3139 372c 3135  9 -23.0917197,15
+00000c50: 2e30 3232 3938 202d 3233 2e39 3539 3235  .02298 -23.95925
+00000c60: 3937 2c31 372e 3631 3032 3220 2d30 2e36  97,17.61022 -0.6
+00000c70: 3730 3037 2c31 2e39 3938 3431 202d 302e  7007,1.99841 -0.
+00000c80: 3236 3932 372c 342e 3130 3037 3220 312e  26927,4.10072 1.
+00000c90: 3330 3136 332c 342e 3036 3638 3520 312e  30163,4.06685 1.
+00000ca0: 3635 3033 2c2d 302e 3033 3535 2031 2e39  6503,-0.0355 1.9
+00000cb0: 3536 3334 2c2d 302e 3835 3833 3720 322e  5634,-0.85837 2.
+00000cc0: 3734 3438 312c 2d33 2e34 3631 3537 2032  74481,-3.46157 2
+00000cd0: 2e30 3539 3235 2c2d 362e 3739 3838 3120  .05925,-6.79881 
+00000ce0: 302e 3534 3939 342c 2d32 352e 3833 3732  0.54994,-25.8372
+00000cf0: 3320 2d30 2e36 3337 3536 2c2d 3331 2e38  3 -0.63756,-31.8
+00000d00: 3837 3631 3620 2d30 2e35 3938 3132 2c2d  87616 -0.59812,-
+00000d10: 332e 3034 3736 3536 202d 312e 3334 3532  3.047656 -1.3452
+00000d20: 392c 2d35 2e34 3835 3234 3220 2d32 2e36  9,-5.485242 -2.6
+00000d30: 3735 3136 2c2d 342e 3835 3436 3632 207a  7516,-4.854662 z
+00000d40: 206d 2034 2e30 3033 3431 2c32 2e37 3332   m 4.00341,2.732
+00000d50: 3638 2063 2031 2e37 3330 3831 2c38 2e38  68 c 1.73081,8.8
+00000d60: 3133 3033 3820 322e 3035 3633 392c 3231  13038 2.05639,21
+00000d70: 2e31 3636 3139 3820 312e 3135 3031 332c  .166198 1.15013,
+00000d80: 3332 2e30 3434 3630 3820 2d30 2e33 3037  32.044608 -0.307
+00000d90: 3531 2c33 2e36 3931 3338 202d 312e 3537  51,3.69138 -1.57
+00000da0: 3334 342c 372e 3537 3138 3820 2d34 2e36  344,7.57188 -4.6
+00000db0: 3832 3936 2c37 2e38 3137 3437 202d 322e  8296,7.81747 -2.
+00000dc0: 3238 3330 362c 302e 3138 3034 202d 342e  28306,0.1804 -4.
+00000dd0: 3430 3134 322c 2d33 2e33 3935 3620 2d32  40142,-3.3956 -2
+00000de0: 2e36 3832 3737 2c2d 362e 3735 3534 3320  .68277,-6.75543 
+00000df0: 312e 3735 3531 342c 2d33 2e34 3331 3036  1.75514,-3.43106
+00000e00: 2031 352e 3335 3037 352c 2d31 382e 3834   15.35075,-18.84
+00000e10: 3535 3420 3236 2e37 3933 3233 3937 2c2d  554 26.7932397,-
+00000e20: 3139 2e30 3439 3232 2031 2e37 3735 3139  19.04922 1.77519
+00000e30: 2c2d 302e 3033 3136 2034 2e32 3130 3337  ,-0.0316 4.21037
+00000e40: 392c 312e 3237 3034 3820 342e 3337 3439  9,1.27048 4.3749
+00000e50: 3039 2c33 2e30 3338 3334 2030 2e31 3831  09,3.03834 0.181
+00000e60: 342c 312e 3935 3030 3920 2d33 2e37 3738  4,1.95009 -3.778
+00000e70: 3739 392c 332e 3533 3532 3520 2d35 2e37  799,3.53525 -5.7
+00000e80: 3337 3232 392c 332e 3535 3336 3520 2d31  37229,3.55365 -1
+00000e90: 322e 3133 3834 3839 372c 302e 3131 3430  2.1384897,0.1140
+00000ea0: 3820 2d32 332e 3139 3734 3939 372c 2d31  8 -23.1974997,-1
+00000eb0: 322e 3634 3231 3620 2d32 352e 3430 3234  2.64216 -25.4024
+00000ec0: 3839 372c 2d31 382e 3438 3335 3132 202d  897,-18.483512 -
+00000ed0: 302e 3930 3936 312c 2d32 2e34 3039 3731  0.90961,-2.40971
+00000ee0: 3520 2d31 2e34 3930 3736 2c2d 382e 3030  5 -1.49076,-8.00
+00000ef0: 3030 3338 2030 2e38 3336 3833 2c2d 392e  0038 0.83683,-9.
+00000f00: 3130 3330 3138 2031 2e39 3338 332c 2d30  103018 1.9383,-0
+00000f10: 2e39 3138 3531 3220 342e 3437 3835 332c  .918512 4.47853,
+00000f20: 322e 3439 3738 3639 2035 2e33 3530 3334  2.497869 5.35034
+00000f30: 2c36 2e39 3337 3131 3220 7a22 0a20 2020  ,6.937112 z".   
+00000f40: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00000f50: 6574 7970 6573 3d22 7373 6373 7373 6373  etypes="sscssscs
+00000f60: 7373 7373 7373 6373 7373 7373 2220 2f3e  sssssscsssss" />
+00000f70: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00000f80: 2020 7374 796c 653d 2266 696c 6c3a 2365    style="fill:#e
+00000f90: 3039 6331 383b 6669 6c6c 2d6f 7061 6369  09c18;fill-opaci
+00000fa0: 7479 3a31 3b73 7472 6f6b 653a 6e6f 6e65  ty:1;stroke:none
+00000fb0: 3b73 7472 6f6b 652d 7769 6474 683a 343b  ;stroke-width:4;
+00000fc0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00000fd0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00000fe0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00000ff0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00001000: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00001010: 220a 2020 2020 2020 2064 3d22 4d20 3732  ".       d="M 72
+00001020: 2e31 3738 3733 312c 3733 2e37 3238 3738  .178731,73.72878
+00001030: 3320 3930 2e34 3039 3236 372c 3532 2e34  3 90.409267,52.4
+00001040: 3033 3239 3620 6320 302e 3538 3236 3236  03296 c 0.582626
+00001050: 2c2d 302e 3731 3638 3834 202d 362e 3332  ,-0.716884 -6.32
+00001060: 3634 342c 2d35 2e34 3336 3838 3820 322e  644,-5.436888 2.
+00001070: 3633 3538 3532 2c2d 392e 3535 3932 3435  635852,-9.559245
+00001080: 2033 2e37 3935 3231 362c 2d31 2e37 3435   3.795216,-1.745
+00001090: 3637 3320 392e 3931 3932 3131 2c30 2e39  673 9.919211,0.9
+000010a0: 3035 3834 2031 322e 3532 3631 3331 2c33  0584 12.526131,3
+000010b0: 2e37 3732 3530 3620 322e 3436 3033 392c  .772506 2.46039,
+000010c0: 2d30 2e39 3332 3334 3820 302e 3633 3533  -0.932348 0.6353
+000010d0: 342c 2d30 2e37 3737 3431 3920 312e 3830  4,-0.777419 1.80
+000010e0: 3939 322c 2d30 2e37 3036 3734 3420 3231  992,-0.706744 21
+000010f0: 2e38 3038 3037 2c2d 302e 3833 3530 3235  .80807,-0.835025
+00001100: 2033 352e 3139 3432 382c 2d30 2e38 3438   35.19428,-0.848
+00001110: 3932 3720 3536 2e36 3831 3338 2c33 2e34  927 56.68138,3.4
+00001120: 3537 2033 2e34 3437 3036 2c30 2e36 3930  57 3.44706,0.690
+00001130: 3737 3520 352e 3237 3337 362c 322e 3333  775 5.27376,2.33
+00001140: 3130 3220 362e 3838 3934 322c 352e 3331  102 6.88942,5.31
+00001150: 3530 3720 342e 3737 3734 312c 382e 3832  507 4.77741,8.82
+00001160: 3336 3320 352e 3035 3538 322c 3137 2e34  363 5.05582,17.4
+00001170: 3832 3334 202d 312e 3035 3639 2c32 372e  8234 -1.0569,27.
+00001180: 3237 3738 3238 202d 312e 3430 3138 362c  277828 -1.40186,
+00001190: 322e 3234 3634 3420 2d34 2e31 3932 3836  2.24644 -4.19286
+000011a0: 2c34 2e38 3038 3433 202d 362e 3833 3439  ,4.80843 -6.8349
+000011b0: 312c 342e 3938 3533 3420 2d31 312e 3332  1,4.98534 -11.32
+000011c0: 3432 322c 302e 3735 3832 3720 2d32 362e  422,0.75827 -26.
+000011d0: 3334 3431 362c 2d30 2e36 3236 3720 2d33  34416,-0.6267 -3
+000011e0: 312e 3939 3337 392c 2d30 2e38 3837 3938  1.99379,-0.88798
+000011f0: 202d 332e 3633 3239 352c 2d30 2e31 3638   -3.63295,-0.168
+00001200: 3031 202d 362e 3833 3832 322c 332e 3434  01 -6.83822,3.44
+00001210: 3636 3220 2d37 2e39 3032 3838 2c36 2e31  662 -7.90288,6.1
+00001220: 3635 3639 202d 322e 3938 3331 342c 372e  6569 -2.98314,7.
+00001230: 3631 3837 3639 202d 362e 3839 3737 342c  618769 -6.89774,
+00001240: 3130 2e35 3331 3732 3920 2d31 322e 3136  10.531729 -12.16
+00001250: 3235 392c 3135 2e32 3233 3139 3920 312e  259,15.223199 1.
+00001260: 3438 3535 312c 2d35 2e31 3133 3832 202d  48551,-5.11382 -
+00001270: 312e 3639 3139 332c 2d38 2e31 3533 3434  1.69193,-8.15344
+00001280: 202d 332e 3136 3430 322c 2d38 2e35 3336   -3.16402,-8.536
+00001290: 3039 202d 302e 3131 3835 342c 312e 3437  09 -0.11854,1.47
+000012a0: 3336 3520 2d34 2e32 3232 3035 2c35 2e35  365 -4.22205,5.5
+000012b0: 3130 3732 202d 352e 3339 3632 312c 352e  1072 -5.39621,5.
+000012c0: 3934 3634 3820 312e 3233 3039 372c 2d32  94648 1.23097,-2
+000012d0: 2e38 3137 2030 2e31 3336 3638 2c2d 342e  .817 0.13668,-4.
+000012e0: 3038 3135 3420 2d30 2e39 3838 3037 2c2d  08154 -0.98807,-
+000012f0: 362e 3535 3935 3420 2d30 2e31 3236 3637  6.55954 -0.12667
+00001300: 2c2d 302e 3537 3834 3420 2d30 2e33 3632  ,-0.57844 -0.362
+00001310: 3737 2c2d 312e 3036 3531 202d 302e 3838  77,-1.0651 -0.88
+00001320: 3833 322c 2d31 2e37 3335 3532 3420 2d31  832,-1.735524 -1
+00001330: 2e35 3037 3634 342c 312e 3239 3538 3134  .507644,1.295814
+00001340: 202d 322e 3331 3531 3631 2c32 2e39 3935   -2.315161,2.995
+00001350: 3431 3420 2d35 2e33 3431 3938 382c 332e  414 -5.341988,3.
+00001360: 3939 3830 3334 2030 2e35 3730 3533 2c2d  998034 0.57053,-
+00001370: 342e 3235 3232 3031 202d 312e 3234 3632  4.252201 -1.2462
+00001380: 3239 2c2d 362e 3734 3732 3437 202d 332e  29,-6.747247 -3.
+00001390: 3037 3139 3138 2c2d 3130 2e34 3331 3139  071918,-10.43119
+000013a0: 3820 2d31 2e32 3234 3130 392c 332e 3430  8 -1.224109,3.40
+000013b0: 3537 3039 202d 322e 3132 3033 3138 2c35  5709 -2.120318,5
+000013c0: 2e33 3334 3339 3220 2d36 2e37 3931 3233  .334392 -6.79123
+000013d0: 352c 372e 3330 3031 3638 2031 2e31 3535  5,7.300168 1.155
+000013e0: 3037 382c 2d31 2e38 3238 3731 3820 312e  078,-1.828718 1.
+000013f0: 3830 3530 3932 2c2d 332e 3433 3032 3038  805092,-3.430208
+00001400: 2032 2e31 3339 3437 2c2d 342e 3631 3633   2.13947,-4.6163
+00001410: 3937 206c 2030 2e32 3635 3135 372c 2d32  97 l 0.265157,-2
+00001420: 2e35 3731 3333 3720 6320 2d30 2e31 3330  .571337 c -0.130
+00001430: 3230 372c 2d31 2e32 3238 3134 3720 302e  207,-1.228147 0.
+00001440: 3036 3039 362c 2d32 2e30 3034 3238 3420  06096,-2.004284 
+00001450: 2d30 2e38 3738 3632 352c 2d33 2e35 3437  -0.878625,-3.547
+00001460: 3531 3120 2d30 2e30 3837 3838 2c30 2e36  511 -0.08788,0.6
+00001470: 3233 3335 3120 2d32 2e39 3730 3239 362c  23351 -2.970296,
+00001480: 322e 3932 3337 3438 202d 342e 3935 3732  2.923748 -4.9572
+00001490: 3236 2c33 2e31 3233 3638 3420 312e 3639  26,3.123684 1.69
+000014a0: 3936 3932 2c2d 342e 3134 3730 3633 2030  9692,-4.147063 0
+000014b0: 2e39 3031 3034 2c2d 352e 3935 3938 202d  .90104,-5.9598 -
+000014c0: 302e 3132 3239 3938 2c2d 372e 3736 3336  0.122998,-7.7636
+000014d0: 202d 302e 3835 3830 3633 2c30 2e38 3332   -0.858063,0.832
+000014e0: 3631 3320 2d33 2e33 3539 3133 312c 332e  613 -3.359131,3.
+000014f0: 3235 3030 3133 202d 352e 3436 3033 3638  250013 -5.460368
+00001500: 2c33 2e35 3432 3932 3820 322e 3235 3334  ,3.542928 2.2534
+00001510: 3537 2c2d 332e 3234 3139 3336 202d 302e  57,-3.241936 -0.
+00001520: 3236 3632 3238 2c2d 382e 3437 3333 3538  266228,-8.473358
+00001530: 202d 312e 3033 3433 3532 2c2d 392e 3831   -1.034352,-9.81
+00001540: 3938 3620 6c20 2d33 2e31 3331 3436 332c  986 l -3.131463,
+00001550: 2d32 2e30 3437 3431 3420 7a22 0a20 2020  -2.047414 z".   
+00001560: 2020 2020 6964 3d22 7061 7468 312d 3622      id="path1-6"
+00001570: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00001580: 3a6e 6f64 6574 7970 6573 3d22 6363 7363  :nodetypes="ccsc
+00001590: 6373 7373 7373 7363 6363 6363 6363 6363  cssssssccccccccc
+000015a0: 6363 6363 6363 6363 2220 2f3e 0a20 2020  cccccccc" />.   
+000015b0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+000015c0: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
+000015d0: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000015e0: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
+000015f0: 3538 3370 783b 7374 726f 6b65 2d6c 696e  583px;stroke-lin
+00001600: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001610: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001620: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00001630: 220a 2020 2020 2020 2064 3d22 6d20 3132  ".       d="m 12
+00001640: 372e 3739 3637 332c 3232 342e 3438 3031  7.79673,224.4801
+00001650: 3720 6320 302c 3020 392e 3836 3831 382c  7 c 0,0 9.86818,
+00001660: 2d39 2e30 3239 3933 2031 362e 3933 3436  -9.02993 16.9346
+00001670: 382c 2d31 362e 3731 3434 3420 342e 3834  8,-16.71444 4.84
+00001680: 3935 332c 2d35 2e32 3733 3636 2035 2e37  953,-5.27366 5.7
+00001690: 3438 3931 2c2d 392e 3831 3232 3520 372e  4891,-9.81225 7.
+000016a0: 3630 3637 2c2d 3134 2e38 3137 3736 2030  6067,-14.81776 0
+000016b0: 2e38 3731 3534 2c2d 322e 3334 3832 3220  .87154,-2.34822 
+000016c0: 332e 3136 3330 342c 2d38 2e36 3832 3637  3.16304,-8.68267
+000016d0: 2031 312e 3336 3638 382c 2d38 2e38 3635   11.36688,-8.865
+000016e0: 3837 2031 322e 3331 3735 342c 2d30 2e32  87 12.31754,-0.2
+000016f0: 3735 3036 2031 342e 3634 3130 352c 342e  7506 14.64105,4.
+00001700: 3333 3539 3720 3136 2e39 3535 3732 2c35  33597 16.95572,5
+00001710: 2e31 3934 3633 2039 2e30 3033 3434 2c33  .19463 9.00344,3
+00001720: 2e33 3339 3938 2031 392e 3031 3333 362c  .33998 19.01336,
+00001730: 352e 3434 3531 3920 3231 2e38 3234 3731  5.44519 21.82471
+00001740: 2c37 2e32 3434 3920 332e 3936 3138 392c  ,7.2449 3.96189,
+00001750: 322e 3533 3632 3420 2d30 2e37 3332 3437  2.53624 -0.73247
+00001760: 2c31 392e 3330 3137 3320 2d35 2e31 3935  ,19.30173 -5.195
+00001770: 3136 2c32 302e 3637 3836 3220 2d37 2e34  16,20.67862 -7.4
+00001780: 3633 3339 2c32 2e33 3032 3731 202d 3136  6339,2.30271 -16
+00001790: 2e39 3136 3033 2c2d 322e 3934 3630 3320  .91603,-2.94603 
+000017a0: 2d32 332e 3137 3339 312c 302e 3737 3334  -23.17391,0.7734
+000017b0: 3722 0a20 2020 2020 2020 6964 3d22 7061  7".       id="pa
+000017c0: 7468 3437 3739 220a 2020 2020 2020 2073  th4779".       s
+000017d0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+000017e0: 733d 2263 7373 7373 7373 6322 202f 3e0a  s="cssssssc" />.
+000017f0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00001800: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
+00001810: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+00001820: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00001830: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
+00001840: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00001850: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00001860: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00001870: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00001880: 2031 3134 2e37 3531 3036 2c32 3030 2e33   114.75106,200.3
+00001890: 3933 3737 2063 2031 2e31 3731 3438 2c34  9377 c 1.17148,4
+000018a0: 2e31 3039 3938 2031 2e33 3235 392c 3135  .10998 1.3259,15
+000018b0: 2e37 3633 3132 2030 2e39 3537 3134 2c32  .76312 0.95714,2
+000018c0: 332e 3133 3432 3322 0a20 2020 2020 2020  3.13423".       
+000018d0: 6964 3d22 7061 7468 3437 3831 220a 2020  id="path4781".  
+000018e0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+000018f0: 6465 7479 7065 733d 2263 6322 202f 3e0a  detypes="cc" />.
+00001900: 2020 2020 3c65 6c6c 6970 7365 0a20 2020      <ellipse.   
+00001910: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
+00001920: 7479 3a30 2e39 393b 6669 6c6c 3a23 3030  ty:0.99;fill:#00
+00001930: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
+00001940: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
+00001950: 6e7a 6572 6f3b 7374 726f 6b65 3a6e 6f6e  nzero;stroke:non
+00001960: 653b 7374 726f 6b65 2d77 6964 7468 3a31  e;stroke-width:1
+00001970: 2e35 3837 3565 2d30 383b 7374 726f 6b65  .5875e-08;stroke
+00001980: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+00001990: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
+000019a0: 6f75 6e64 220a 2020 2020 2020 2069 643d  ound".       id=
+000019b0: 2270 6174 6834 3833 3522 0a20 2020 2020  "path4835".     
+000019c0: 2020 6378 3d22 3133 372e 3534 3934 3422    cx="137.54944"
+000019d0: 0a20 2020 2020 2020 6379 3d22 3138 332e  .       cy="183.
+000019e0: 3833 3736 3322 0a20 2020 2020 2020 7278  83763".       rx
+000019f0: 3d22 312e 3333 3434 3834 3122 0a20 2020  ="1.3344841".   
+00001a00: 2020 2020 7279 3d22 322e 3333 3434 3938      ry="2.334498
+00001a10: 3422 202f 3e0a 2020 2020 3c70 6174 680a  4" />.    <path.
+00001a20: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00001a30: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
+00001a40: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
+00001a50: 6474 683a 302e 3230 3133 3639 7078 3b73  dth:0.201369px;s
+00001a60: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00001a70: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00001a80: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00001a90: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00001aa0: 2020 643d 226d 2031 3030 2e37 3835 3731    d="m 100.78571
+00001ab0: 2c31 3636 2e35 3531 3435 2063 2030 2c30  ,166.55145 c 0,0
+00001ac0: 202d 312e 3230 3638 3835 2c2d 322e 3237   -1.206885,-2.27
+00001ad0: 3036 3120 2d32 2e33 3836 3235 352c 2d32  061 -2.386255,-2
+00001ae0: 2e31 3837 3537 202d 312e 3138 3934 382c  .18757 -1.18948,
+00001af0: 302e 3038 3337 202d 322e 3135 3733 362c  0.0837 -2.15736,
+00001b00: 312e 3737 3030 3820 2d32 2e30 3137 3232  1.77008 -2.01722
+00001b10: 2c32 2e39 3534 3234 2030 2e31 3334 312c  ,2.95424 0.1341,
+00001b20: 312e 3133 3238 3220 322e 3533 3631 382c  1.13282 2.53618,
+00001b30: 322e 3239 3736 3520 322e 3533 3631 382c  2.29765 2.53618,
+00001b40: 322e 3239 3736 3522 0a20 2020 2020 2020  2.29765".       
+00001b50: 6964 3d22 7061 7468 3533 3133 220a 2020  id="path5313".  
+00001b60: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00001b70: 6465 7479 7065 733d 2263 7373 6322 202f  detypes="cssc" /
+00001b80: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00001b90: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00001ba0: 3030 3030 3030 3b66 696c 6c2d 6f70 6163  000000;fill-opac
+00001bb0: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
+00001bc0: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
+00001bd0: 2e32 3634 3538 3370 783b 7374 726f 6b65  .264583px;stroke
+00001be0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00001bf0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00001c00: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00001c10: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00001c20: 6d20 3130 362e 3732 3631 372c 3137 342e  m 106.72617,174.
+00001c30: 3936 3134 3820 6320 332e 3434 3232 372c  96148 c 3.44227,
+00001c40: 302e 3433 3838 3920 352e 3631 3637 372c  0.43889 5.61677,
+00001c50: 302e 3635 3635 3320 392e 3331 3830 322c  0.65653 9.31802,
+00001c60: 312e 3230 3435 3220 302e 3139 3838 332c  1.20452 0.19883,
+00001c70: 302e 3032 3934 202d 302e 3538 3533 352c  0.0294 -0.58535,
+00001c80: 302e 3830 3837 3520 2d30 2e37 3833 3736  0.80875 -0.78376
+00001c90: 2c30 2e37 3736 3539 202d 312e 3234 3137  ,0.77659 -1.2417
+00001ca0: 332c 2d30 2e32 3031 3235 202d 312e 3536  3,-0.20125 -1.56
+00001cb0: 3736 352c 2d30 2e33 3932 3837 202d 322e  765,-0.39287 -2.
+00001cc0: 3338 3235 342c 2d30 2e30 3734 3620 2d30  38254,-0.0746 -0
+00001cd0: 2e39 3830 3232 2c30 2e33 3832 3834 202d  .98022,0.38284 -
+00001ce0: 302e 3235 3937 342c 312e 3136 3536 3520  0.25974,1.16565 
+00001cf0: 2d31 2e32 3637 3737 2c31 2e34 3637 3734  -1.26777,1.46774
+00001d00: 202d 302e 3838 3532 382c 302e 3236 3533   -0.88528,0.2653
+00001d10: 202d 322e 3438 3735 2c2d 302e 3132 3939   -2.4875,-0.1299
+00001d20: 3420 2d33 2e30 3635 3733 2c2d 302e 3835  4 -3.06573,-0.85
+00001d30: 3038 3720 2d30 2e35 3333 3336 2c2d 302e  087 -0.53336,-0.
+00001d40: 3636 3520 2d30 2e36 3135 3533 2c2d 312e  665 -0.61553,-1.
+00001d50: 3137 3530 3920 2d30 2e38 3236 3134 2c2d  17509 -0.82614,-
+00001d60: 312e 3436 3436 3420 2d30 2e30 3638 312c  1.46464 -0.0681,
+00001d70: 2d30 2e30 3933 3620 2d30 2e37 3836 3038  -0.0936 -0.78608
+00001d80: 2c2d 302e 3135 3338 3220 2d31 2e31 3632  ,-0.15382 -1.162
+00001d90: 3539 2c2d 302e 3530 3731 3820 2d30 2e33  59,-0.50718 -0.3
+00001da0: 3232 3734 2c2d 302e 3330 3238 3920 2d30  2274,-0.30289 -0
+00001db0: 2e30 3634 332c 2d30 2e35 3831 3439 2030  .0643,-0.58149 0
+00001dc0: 2e31 3730 3531 2c2d 302e 3535 3135 3620  .17051,-0.55156 
+00001dd0: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
+00001de0: 7468 3533 3135 220a 2020 2020 2020 2073  th5315".       s
+00001df0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00001e00: 733d 2273 7373 7373 7373 7373 2220 2f3e  s="sssssssss" />
+00001e10: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00001e20: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
+00001e30: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
+00001e40: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
+00001e50: 2e32 3634 3538 3370 783b 7374 726f 6b65  .264583px;stroke
+00001e60: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00001e70: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00001e80: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00001e90: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00001ea0: 4d20 3239 2e35 3636 3537 382c 3234 342e  M 29.566578,244.
+00001eb0: 3936 3435 3520 4820 3138 372e 3336 3733  96455 H 187.3673
+00001ec0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00001ed0: 6838 3934 3722 202f 3e0a 2020 2020 3c75  h8947" />.    <u
+00001ee0: 7365 0a20 2020 2020 2020 783d 2230 220a  se.       x="0".
+00001ef0: 2020 2020 2020 2079 3d22 3022 0a20 2020         y="0".   
+00001f00: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00001f10: 2370 6174 6838 3938 3522 0a20 2020 2020  #path8985".     
+00001f20: 2020 6964 3d22 7573 6531 3838 3133 220a    id="use18813".
+00001f30: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00001f40: 3d22 7472 616e 736c 6174 6528 312e 3636  ="translate(1.66
+00001f50: 3731 3431 382c 3236 2e34 3835 3330 3829  71418,26.485308)
+00001f60: 2220 2f3e 0a20 2020 203c 7573 650a 2020  " />.    <use.  
+00001f70: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
+00001f80: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
+00001f90: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
+00001fa0: 3839 3835 2d38 220a 2020 2020 2020 2069  8985-8".       i
+00001fb0: 643d 2275 7365 3235 3230 3422 0a20 2020  d="use25204".   
+00001fc0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
+00001fd0: 7261 6e73 6c61 7465 282d 3134 2e32 3537  ranslate(-14.257
+00001fe0: 3031 352c 3235 2e30 3736 3530 3829 2220  015,25.076508)" 
+00001ff0: 2f3e 0a20 2020 203c 7573 650a 2020 2020  />.    <use.    
+00002000: 2020 2078 3d22 3022 0a20 2020 2020 2020     x="0".       
+00002010: 793d 2230 220a 2020 2020 2020 2078 6c69  y="0".       xli
+00002020: 6e6b 3a68 7265 663d 2223 7061 7468 3839  nk:href="#path89
+00002030: 3835 2d38 220a 2020 2020 2020 2069 643d  85-8".       id=
+00002040: 2275 7365 3235 3230 3222 0a20 2020 2020  "use25202".     
+00002050: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00002060: 6e73 6c61 7465 282d 3130 2e31 3034 3430  nslate(-10.10440
+00002070: 372c 3231 2e37 3232 3934 3129 2220 2f3e  7,21.722941)" />
+00002080: 0a20 2020 203c 7573 650a 2020 2020 2020  .    <use.      
+00002090: 2078 3d22 3022 0a20 2020 2020 2020 793d   x="0".       y=
+000020a0: 2230 220a 2020 2020 2020 2078 6c69 6e6b  "0".       xlink
+000020b0: 3a68 7265 663d 2223 7061 7468 3839 3835  :href="#path8985
+000020c0: 2d38 220a 2020 2020 2020 2069 643d 2275  -8".       id="u
+000020d0: 7365 3335 3322 0a20 2020 2020 2020 7472  se353".       tr
+000020e0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+000020f0: 7465 2832 332e 3932 3334 3539 2c32 312e  te(23.923459,21.
+00002100: 3139 3931 3834 2922 202f 3e0a 2020 2020  199184)" />.    
+00002110: 3c72 6563 740a 2020 2020 2020 2073 7479  <rect.       sty
+00002120: 6c65 3d22 6f70 6163 6974 793a 302e 3939  le="opacity:0.99
+00002130: 3b66 696c 6c3a 2366 6666 6666 663b 6669  ;fill:#ffffff;fi
+00002140: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00002150: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+00002160: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00002170: 726f 6b65 2d77 6964 7468 3a30 2e33 3b73  roke-width:0.3;s
+00002180: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
+00002190: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
+000021a0: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
+000021b0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+000021c0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000021d0: 220a 2020 2020 2020 2069 643d 2272 6563  ".       id="rec
+000021e0: 7432 3034 3135 2d33 2d36 220a 2020 2020  t20415-3-6".    
+000021f0: 2020 2077 6964 7468 3d22 332e 3432 3033     width="3.4203
+00002200: 3238 3122 0a20 2020 2020 2020 6865 6967  281".       heig
+00002210: 6874 3d22 3233 2e34 3032 3334 3222 0a20  ht="23.402342". 
+00002220: 2020 2020 2020 783d 2231 3133 2e36 3833        x="113.683
+00002230: 3938 220a 2020 2020 2020 2079 3d22 3234  98".       y="24
+00002240: 352e 3438 3136 3322 202f 3e0a 2020 2020  5.48163" />.    
+00002250: 3c72 6563 740a 2020 2020 2020 2073 7479  <rect.       sty
+00002260: 6c65 3d22 6f70 6163 6974 793a 302e 3939  le="opacity:0.99
+00002270: 3b66 696c 6c3a 2366 6666 6666 663b 6669  ;fill:#ffffff;fi
+00002280: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00002290: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+000022a0: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000022b0: 726f 6b65 2d77 6964 7468 3a30 2e33 3b73  roke-width:0.3;s
+000022c0: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
+000022d0: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
+000022e0: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
+000022f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00002300: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00002310: 220a 2020 2020 2020 2069 643d 2272 6563  ".       id="rec
+00002320: 7432 3034 3135 2d33 220a 2020 2020 2020  t20415-3".      
+00002330: 2077 6964 7468 3d22 332e 3432 3033 3238   width="3.420328
+00002340: 3122 0a20 2020 2020 2020 6865 6967 6874  1".       height
+00002350: 3d22 3233 2e34 3032 3334 3222 0a20 2020  ="23.402342".   
+00002360: 2020 2020 783d 2239 372e 3930 3631 3336      x="97.906136
+00002370: 220a 2020 2020 2020 2079 3d22 3234 352e  ".       y="245.
+00002380: 3534 3930 3122 202f 3e0a 2020 2020 3c72  54901" />.    <r
+00002390: 6563 740a 2020 2020 2020 2073 7479 6c65  ect.       style
+000023a0: 3d22 6f70 6163 6974 793a 302e 3939 3b66  ="opacity:0.99;f
+000023b0: 696c 6c3a 2366 6666 6666 663b 6669 6c6c  ill:#ffffff;fill
+000023c0: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
+000023d0: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
+000023e0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+000023f0: 6b65 2d77 6964 7468 3a30 2e33 3b73 7472  ke-width:0.3;str
+00002400: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00002410: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00002420: 6e3a 726f 756e 643b 7374 726f 6b65 2d64  n:round;stroke-d
+00002430: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00002440: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00002450: 2020 2020 2020 2069 643d 2272 6563 7432         id="rect2
+00002460: 3034 3135 2d33 2d35 220a 2020 2020 2020  0415-3-5".      
+00002470: 2077 6964 7468 3d22 332e 3432 3033 3238   width="3.420328
+00002480: 3122 0a20 2020 2020 2020 6865 6967 6874  1".       height
+00002490: 3d22 392e 3731 3432 3037 3622 0a20 2020  ="9.7142076".   
+000024a0: 2020 2020 783d 222d 3235 382e 3630 3834      x="-258.6084
+000024b0: 3622 0a20 2020 2020 2020 793d 2231 3335  6".       y="135
+000024c0: 2e34 3536 3637 220a 2020 2020 2020 2074  .45667".       t
+000024d0: 7261 6e73 666f 726d 3d22 726f 7461 7465  ransform="rotate
+000024e0: 282d 3930 2922 202f 3e0a 2020 2020 3c72  (-90)" />.    <r
+000024f0: 6563 740a 2020 2020 2020 2073 7479 6c65  ect.       style
+00002500: 3d22 6f70 6163 6974 793a 302e 3939 3b66  ="opacity:0.99;f
+00002510: 696c 6c3a 2366 6666 6666 663b 6669 6c6c  ill:#ffffff;fill
+00002520: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
+00002530: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
+00002540: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00002550: 6b65 2d77 6964 7468 3a30 2e33 3b73 7472  ke-width:0.3;str
+00002560: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00002570: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00002580: 6e3a 726f 756e 643b 7374 726f 6b65 2d64  n:round;stroke-d
+00002590: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+000025a0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000025b0: 2020 2020 2020 2069 643d 2272 6563 7432         id="rect2
+000025c0: 3034 3135 2d33 2d35 2d33 220a 2020 2020  0415-3-5-3".    
+000025d0: 2020 2077 6964 7468 3d22 332e 3432 3033     width="3.4203
+000025e0: 3238 3122 0a20 2020 2020 2020 6865 6967  281".       heig
+000025f0: 6874 3d22 3133 2e34 3936 3334 3422 0a20  ht="13.496344". 
+00002600: 2020 2020 2020 783d 222d 3234 382e 3737        x="-248.77
+00002610: 3633 3422 0a20 2020 2020 2020 793d 2231  634".       y="1
+00002620: 3334 2e37 3635 3436 220a 2020 2020 2020  34.76546".      
+00002630: 2074 7261 6e73 666f 726d 3d22 726f 7461   transform="rota
+00002640: 7465 282d 3930 2922 202f 3e0a 2020 2020  te(-90)" />.    
+00002650: 3c72 6563 740a 2020 2020 2020 2073 7479  <rect.       sty
+00002660: 6c65 3d22 6f70 6163 6974 793a 302e 3939  le="opacity:0.99
+00002670: 3b66 696c 6c3a 2366 6666 6666 663b 6669  ;fill:#ffffff;fi
+00002680: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00002690: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+000026a0: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000026b0: 726f 6b65 2d77 6964 7468 3a30 2e33 3b73  roke-width:0.3;s
+000026c0: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
+000026d0: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
+000026e0: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
+000026f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00002700: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00002710: 220a 2020 2020 2020 2069 643d 2272 6563  ".       id="rec
+00002720: 7432 3034 3135 2d33 2d37 220a 2020 2020  t20415-3-7".    
+00002730: 2020 2077 6964 7468 3d22 332e 3432 3033     width="3.4203
+00002740: 3238 3122 0a20 2020 2020 2020 6865 6967  281".       heig
+00002750: 6874 3d22 3233 2e34 3032 3334 3222 0a20  ht="23.402342". 
+00002760: 2020 2020 2020 783d 2231 3334 2e32 3635        x="134.265
+00002770: 3634 220a 2020 2020 2020 2079 3d22 3234  64".       y="24
+00002780: 352e 3435 3235 3622 202f 3e0a 2020 2020  5.45256" />.    
+00002790: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+000027a0: 6c65 3d22 6669 6c6c 3a6e 6f6e 653b 7374  le="fill:none;st
+000027b0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+000027c0: 6f6b 652d 7769 6474 683a 302e 3236 3435  oke-width:0.2645
+000027d0: 3833 7078 3b73 7472 6f6b 652d 6c69 6e65  83px;stroke-line
+000027e0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+000027f0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00002800: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00002810: 0a20 2020 2020 2020 643d 224d 2032 392e  .       d="M 29.
+00002820: 3430 3937 3937 2c32 3535 2e32 3931 3131  409797,255.29111
+00002830: 2048 2031 3836 2e38 3734 3437 220a 2020   H 186.87447".  
+00002840: 2020 2020 2069 643d 2270 6174 6838 3934       id="path894
+00002850: 3922 202f 3e0a 2020 2020 3c75 7365 0a20  9" />.    <use. 
+00002860: 2020 2020 2020 783d 2230 220a 2020 2020        x="0".    
+00002870: 2020 2079 3d22 3022 0a20 2020 2020 2020     y="0".       
+00002880: 786c 696e 6b3a 6872 6566 3d22 2370 6174  xlink:href="#pat
+00002890: 6838 3938 352d 3822 0a20 2020 2020 2020  h8985-8".       
+000028a0: 6964 3d22 7573 6532 3532 3038 220a 2020  id="use25208".  
+000028b0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+000028c0: 7472 616e 736c 6174 6528 2d31 302e 3137  translate(-10.17
+000028d0: 3439 312c 3331 2e39 3935 3332 3529 2220  491,31.995325)" 
+000028e0: 2f3e 0a20 2020 203c 7573 650a 2020 2020  />.    <use.    
+000028f0: 2020 2078 3d22 3022 0a20 2020 2020 2020     x="0".       
+00002900: 793d 2230 220a 2020 2020 2020 2078 6c69  y="0".       xli
+00002910: 6e6b 3a68 7265 663d 2223 7061 7468 3839  nk:href="#path89
+00002920: 3835 2d38 220a 2020 2020 2020 2069 643d  85-8".       id=
+00002930: 2275 7365 3335 3122 0a20 2020 2020 2020  "use351".       
+00002940: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00002950: 6c61 7465 2832 302e 3632 3233 3639 2c33  late(20.622369,3
+00002960: 322e 3839 3336 3437 2922 202f 3e0a 2020  2.893647)" />.  
+00002970: 2020 3c75 7365 0a20 2020 2020 2020 783d    <use.       x=
+00002980: 2230 220a 2020 2020 2020 2079 3d22 3022  "0".       y="0"
+00002990: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
+000029a0: 6566 3d22 2370 6174 6838 3938 352d 3822  ef="#path8985-8"
+000029b0: 0a20 2020 2020 2020 6964 3d22 7573 6535  .       id="use5
+000029c0: 3335 220a 2020 2020 2020 2074 7261 6e73  35".       trans
+000029d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000029e0: 3434 2e33 3630 3236 382c 3332 2e32 3132  44.360268,32.212
+000029f0: 3432 3529 2220 2f3e 0a20 2020 203c 7573  425)" />.    <us
+00002a00: 650a 2020 2020 2020 2078 3d22 3022 0a20  e.       x="0". 
+00002a10: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
+00002a20: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00002a30: 7061 7468 3839 3835 2d38 220a 2020 2020  path8985-8".    
+00002a40: 2020 2069 643d 2275 7365 3533 3722 0a20     id="use537". 
+00002a50: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00002a60: 2274 7261 6e73 6c61 7465 2835 342e 3730  "translate(54.70
+00002a70: 3037 3332 2c33 312e 3436 3333 3735 2922  0732,31.463375)"
+00002a80: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00002a90: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00002aa0: 3a6e 6f6e 653b 7374 726f 6b65 3a23 3030  :none;stroke:#00
+00002ab0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+00002ac0: 683a 302e 3236 3435 3833 7078 3b73 7472  h:0.264583px;str
+00002ad0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00002ae0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00002af0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00002b00: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00002b10: 643d 224d 2032 392e 3133 3538 3838 2c32  d="M 29.135888,2
+00002b20: 3639 2e30 3839 3735 2048 2031 3836 2e35  69.08975 H 186.5
+00002b30: 3538 3622 0a20 2020 2020 2020 6964 3d22  586".       id="
+00002b40: 7061 7468 3839 3531 2220 2f3e 0a20 2020  path8951" />.   
+00002b50: 203c 7573 650a 2020 2020 2020 2078 3d22   <use.       x="
+00002b60: 3022 0a20 2020 2020 2020 793d 2230 220a  0".       y="0".
+00002b70: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
+00002b80: 663d 2223 7061 7468 3839 3835 2d38 220a  f="#path8985-8".
+00002b90: 2020 2020 2020 2069 643d 2275 7365 3235         id="use25
+00002ba0: 3230 3622 0a20 2020 2020 2020 7472 616e  206".       tran
+00002bb0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00002bc0: 282d 3133 2e38 3131 3939 332c 3330 2e32  (-13.811993,30.2
+00002bd0: 3235 3532 3329 2220 2f3e 0a20 2020 203c  25523)" />.    <
+00002be0: 7573 650a 2020 2020 2020 2078 3d22 3022  use.       x="0"
+00002bf0: 0a20 2020 2020 2020 793d 2230 220a 2020  .       y="0".  
+00002c00: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00002c10: 2223 7061 7468 3839 3835 2d38 220a 2020  "#path8985-8".  
+00002c20: 2020 2020 2069 643d 2275 7365 3235 3231       id="use2521
+00002c30: 3022 0a20 2020 2020 2020 7472 616e 7366  0".       transf
+00002c40: 6f72 6d3d 2274 7261 6e73 6c61 7465 282d  orm="translate(-
+00002c50: 362e 3631 3330 3839 312c 3233 2e32 3437  6.6130891,23.247
+00002c60: 3234 3329 2220 2f3e 0a20 2020 203c 7573  243)" />.    <us
+00002c70: 650a 2020 2020 2020 2078 3d22 3022 0a20  e.       x="0". 
+00002c80: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
+00002c90: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00002ca0: 7061 7468 3839 3835 2d38 220a 2020 2020  path8985-8".    
+00002cb0: 2020 2069 643d 2275 7365 3235 3231 3222     id="use25212"
+00002cc0: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00002cd0: 6d3d 2274 7261 6e73 6c61 7465 282d 362e  m="translate(-6.
+00002ce0: 3536 3936 3530 312c 3330 2e34 3239 3338  5696501,30.42938
+00002cf0: 3329 2220 2f3e 0a20 2020 203c 7061 7468  3)" />.    <path
+00002d00: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00002d10: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
+00002d20: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00002d30: 6964 7468 3a30 2e32 3634 3538 3370 783b  idth:0.264583px;
+00002d40: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00002d50: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00002d60: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00002d70: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00002d80: 2020 2064 3d22 6d20 3634 2e39 3236 3433     d="m 64.92643
+00002d90: 362c 3235 382e 3532 3632 3920 6320 2d30  6,258.52629 c -0
+00002da0: 2e32 3038 3639 2c2d 302e 3035 3833 202d  .20869,-0.0583 -
+00002db0: 312e 3933 3433 3031 2c2d 312e 3435 3738  1.934301,-1.4578
+00002dc0: 3520 2d33 2e36 3633 3436 352c 2d31 2e34  5 -3.663465,-1.4
+00002dd0: 3536 3032 202d 322e 3038 3230 3731 2c30  5602 -2.082071,0
+00002de0: 2e30 3032 202d 332e 3135 3634 3839 2c31  .002 -3.156489,1
+00002df0: 2e33 3639 3433 202d 332e 3937 3930 3536  .36943 -3.979056
+00002e00: 2c32 2e35 3735 3337 202d 312e 3037 3533  ,2.57537 -1.0753
+00002e10: 3839 2c31 2e35 3736 3538 202d 312e 3132  89,1.57658 -1.12
+00002e20: 3236 3434 2c33 2e38 3739 3539 202d 302e  2644,3.87959 -0.
+00002e30: 3134 3939 3132 2c35 2e35 3230 3136 2030  149912,5.52016 0
+00002e40: 2e38 3631 3934 2c31 2e34 3533 3731 2032  .86194,1.45371 2
+00002e50: 2e35 3533 3539 312c 312e 3937 3131 3720  .553591,1.97117 
+00002e60: 342e 3135 3232 3334 2c32 2e30 3139 3032  4.152234,2.01902
+00002e70: 2031 2e32 3634 3534 312c 302e 3033 3739   1.264541,0.0379
+00002e80: 2034 2e30 3339 3239 372c 2d31 2e36 3233   4.039297,-1.623
+00002e90: 3120 342e 3033 3932 3937 2c2d 312e 3632  1 4.039297,-1.62
+00002ea0: 3331 220a 2020 2020 2020 2069 643d 2270  31".       id="p
+00002eb0: 6174 6831 3633 3139 2d37 220a 2020 2020  ath16319-7".    
+00002ec0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00002ed0: 7479 7065 733d 2263 7373 7373 6322 202f  types="cssssc" /
+00002ee0: 3e0a 2020 2020 3c75 7365 0a20 2020 2020  >.    <use.     
+00002ef0: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
+00002f00: 3d22 3022 0a20 2020 2020 2020 786c 696e  ="0".       xlin
+00002f10: 6b3a 6872 6566 3d22 2370 6174 6838 3938  k:href="#path898
+00002f20: 352d 3822 0a20 2020 2020 2020 6964 3d22  5-8".       id="
+00002f30: 7573 6533 3439 220a 2020 2020 2020 2074  use349".       t
+00002f40: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00002f50: 6174 6528 3136 2e38 3631 3933 392c 3338  ate(16.861939,38
+00002f60: 2e31 3332 3635 3829 2220 2f3e 0a20 2020  .132658)" />.   
+00002f70: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+00002f80: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
+00002f90: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00002fa0: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
+00002fb0: 3538 3370 783b 7374 726f 6b65 2d6c 696e  583px;stroke-lin
+00002fc0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00002fd0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00002fe0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00002ff0: 220a 2020 2020 2020 2064 3d22 4d20 3238  ".       d="M 28
+00003000: 2e39 3132 3936 342c 3237 342e 3230 3436  .912964,274.2046
+00003010: 3420 4820 3138 362e 3333 3536 3822 0a20  4 H 186.33568". 
+00003020: 2020 2020 2020 6964 3d22 7061 7468 3839        id="path89
+00003030: 3531 2d36 2220 2f3e 0a20 2020 203c 656c  51-6" />.    <el
+00003040: 6c69 7073 650a 2020 2020 2020 2073 7479  lipse.       sty
+00003050: 6c65 3d22 6f70 6163 6974 793a 302e 3939  le="opacity:0.99
+00003060: 3b66 696c 6c3a 2338 6664 3064 663b 6669  ;fill:#8fd0df;fi
+00003070: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00003080: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+00003090: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000030a0: 726f 6b65 2d77 6964 7468 3a31 2e35 3837  roke-width:1.587
+000030b0: 3565 2d30 383b 7374 726f 6b65 2d6c 696e  5e-08;stroke-lin
+000030c0: 6563 6170 3a72 6f75 6e64 3b73 7472 6f6b  ecap:round;strok
+000030d0: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+000030e0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+000030f0: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+00003100: 7468 3839 3835 220a 2020 2020 2020 2063  th8985".       c
+00003110: 783d 2231 3735 2e39 3736 3631 220a 2020  x="175.97661".  
+00003120: 2020 2020 2063 793d 2231 3533 2e35 3330       cy="153.530
+00003130: 3634 220a 2020 2020 2020 2072 783d 2231  64".       rx="1
+00003140: 2e39 3934 3232 3031 220a 2020 2020 2020  .9942201".      
+00003150: 2072 793d 2232 2e33 3238 3134 3122 0a20   ry="2.328141". 
+00003160: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00003170: 2272 6f74 6174 6528 3430 2e32 3337 3234  "rotate(40.23724
+00003180: 3129 2220 2f3e 0a20 2020 203c 7573 650a  1)" />.    <use.
+00003190: 2020 2020 2020 2078 3d22 3022 0a20 2020         x="0".   
+000031a0: 2020 2020 793d 2230 220a 2020 2020 2020      y="0".      
+000031b0: 2078 6c69 6e6b 3a68 7265 663d 2223 7061   xlink:href="#pa
+000031c0: 7468 3839 3835 220a 2020 2020 2020 2069  th8985".       i
+000031d0: 643d 2275 7365 3138 3831 3122 0a20 2020  d="use18811".   
+000031e0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
+000031f0: 7261 6e73 6c61 7465 2833 2e37 3030 3634  ranslate(3.70064
+00003200: 3632 2c33 332e 3839 3436 3631 2922 202f  62,33.894661)" /
+00003210: 3e0a 2020 2020 3c75 7365 0a20 2020 2020  >.    <use.     
+00003220: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
+00003230: 3d22 3022 0a20 2020 2020 2020 786c 696e  ="0".       xlin
+00003240: 6b3a 6872 6566 3d22 2370 6174 6838 3938  k:href="#path898
+00003250: 3522 0a20 2020 2020 2020 6964 3d22 7573  5".       id="us
+00003260: 6531 3838 3135 220a 2020 2020 2020 2074  e18815".       t
+00003270: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00003280: 6174 6528 342e 3234 3634 3634 372c 3138  ate(4.2464647,18
+00003290: 2e35 3839 3139 3229 2220 2f3e 0a20 2020  .589192)" />.   
+000032a0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+000032b0: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
+000032c0: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000032d0: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
+000032e0: 3538 3370 783b 7374 726f 6b65 2d6c 696e  583px;stroke-lin
+000032f0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00003300: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00003310: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00003320: 220a 2020 2020 2020 2064 3d22 6d20 3532  ".       d="m 52
+00003330: 2e39 3134 3139 352c 3234 382e 3933 3037  .914195,248.9307
+00003340: 3220 6320 2d30 2e34 3330 3531 312c 2d30  2 c -0.430511,-0
+00003350: 2e31 3338 3720 2d32 2e34 3830 3137 362c  .1387 -2.480176,
+00003360: 2d31 2e39 3632 3636 202d 372e 3033 3135  -1.96266 -7.0315
+00003370: 342c 2d31 2e39 3632 3636 202d 322e 3635  4,-1.96266 -2.65
+00003380: 3736 3338 2c30 202d 362e 3533 3737 3234  7638,0 -6.537724
+00003390: 2c31 2e35 3339 3837 202d 372e 3736 3239  ,1.53987 -7.7629
+000033a0: 3138 2c34 2e32 3634 3333 202d 312e 3831  18,4.26433 -1.81
+000033b0: 3234 3233 2c34 2e30 3330 3239 202d 322e  2423,4.03029 -2.
+000033c0: 3034 3637 3638 2c31 302e 3031 3434 3820  046768,10.01448 
+000033d0: 302e 3535 3634 3338 2c31 332e 3533 3433  0.556438,13.5343
+000033e0: 3920 312e 3530 3536 3538 2c32 2e30 3335  9 1.505658,2.035
+000033f0: 3837 2034 2e35 3439 3636 2c32 2e33 3634  87 4.54966,2.364
+00003400: 3032 2037 2e30 3337 3633 2c32 2e33 3634  02 7.03763,2.364
+00003410: 3032 2032 2e37 3435 3033 342c 3020 362e  02 2.745034,0 6.
+00003420: 3938 3636 3236 2c2d 312e 3635 3732 3720  986626,-1.65727 
+00003430: 362e 3938 3636 3236 2c2d 312e 3635 3732  6.986626,-1.6572
+00003440: 3722 0a20 2020 2020 2020 6964 3d22 7061  7".       id="pa
+00003450: 7468 3136 3331 3922 0a20 2020 2020 2020  th16319".       
+00003460: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+00003470: 6573 3d22 6373 7373 7363 2220 2f3e 0a20  es="cssssc" />. 
+00003480: 2020 203c 7573 650a 2020 2020 2020 2078     <use.       x
+00003490: 3d22 3022 0a20 2020 2020 2020 793d 2230  ="0".       y="0
+000034a0: 220a 2020 2020 2020 2078 6c69 6e6b 3a68  ".       xlink:h
+000034b0: 7265 663d 2223 7061 7468 3839 3835 2d38  ref="#path8985-8
+000034c0: 220a 2020 2020 2020 2069 643d 2275 7365  ".       id="use
+000034d0: 3334 3722 0a20 2020 2020 2020 7472 616e  347".       tran
+000034e0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000034f0: 2831 352e 3431 3730 3037 2c32 312e 3035  (15.417007,21.05
+00003500: 3231 3832 2922 202f 3e0a 2020 2020 3c75  2182)" />.    <u
+00003510: 7365 0a20 2020 2020 2020 783d 2230 220a  se.       x="0".
+00003520: 2020 2020 2020 2079 3d22 3022 0a20 2020         y="0".   
+00003530: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00003540: 2370 6174 6838 3938 352d 3822 0a20 2020  #path8985-8".   
+00003550: 2020 2020 6964 3d22 7573 6534 3032 220a      id="use402".
+00003560: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00003570: 3d22 7472 616e 736c 6174 6528 3138 2e31  ="translate(18.1
+00003580: 3430 3239 332c 3237 2e31 3736 3932 3529  40293,27.176925)
+00003590: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+000035a0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000035b0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+000035c0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+000035d0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
+000035e0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+000035f0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00003600: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00003610: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00003620: 2064 3d22 6d20 3836 2e34 3535 3038 352c   d="m 86.455085,
+00003630: 3235 352e 3738 3437 2036 2e30 3332 3437  255.7847 6.03247
+00003640: 342c 3133 2e32 3731 3033 220a 2020 2020  4,13.27103".    
+00003650: 2020 2069 643d 2270 6174 6831 3730 3739     id="path17079
+00003660: 2d35 2d35 220a 2020 2020 2020 2073 6f64  -5-5".       sod
+00003670: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+00003680: 2263 6322 202f 3e0a 2020 2020 3c70 6174  "cc" />.    <pat
+00003690: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+000036a0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+000036b0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+000036c0: 7769 6474 683a 302e 3236 3435 3833 7078  width:0.264583px
+000036d0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000036e0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000036f0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00003700: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00003710: 2020 2020 643d 226d 2039 352e 3336 3437      d="m 95.3647
+00003720: 3739 2c32 3535 2e38 3536 3137 2063 2030  79,255.85617 c 0
+00003730: 2c30 202d 322e 3230 3737 3937 2c31 302e  ,0 -2.207797,10.
+00003740: 3631 3835 3520 2d34 2e32 3136 3539 312c  61855 -4.216591,
+00003750: 3135 2e33 3339 3438 202d 302e 3733 3239  15.33948 -0.7329
+00003760: 3236 2c31 2e37 3232 3437 202d 312e 3935  26,1.72247 -1.95
+00003770: 3136 3436 2c32 2e33 3734 3420 2d33 2e36  1646,2.3744 -3.6
+00003780: 3235 3239 2c32 2e32 3437 3838 220a 2020  2529,2.24788".  
+00003790: 2020 2020 2069 643d 2270 6174 6831 3730       id="path170
+000037a0: 3739 2d35 2d36 220a 2020 2020 2020 2073  79-5-6".       s
+000037b0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+000037c0: 733d 2263 7363 2220 2f3e 0a20 2020 203c  s="csc" />.    <
+000037d0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+000037e0: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+000037f0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00003800: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
+00003810: 3370 783b 7374 726f 6b65 2d6c 696e 6563  3px;stroke-linec
+00003820: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00003830: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00003840: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00003850: 2020 2020 2020 2064 3d22 6d20 3130 302e         d="m 100.
+00003860: 3437 3133 322c 3234 362e 3631 3934 3220  47132,246.61942 
+00003870: 6320 302e 3235 3131 392c 2d30 2e30 3734  c 0.25119,-0.074
+00003880: 3120 332e 3535 3330 342c 2d30 2e34 3231  1 3.55304,-0.421
+00003890: 3920 352e 3230 3637 352c 2d30 2e30 3937  9 5.20675,-0.097
+000038a0: 3820 312e 3531 3633 312c 302e 3239 3731  8 1.51631,0.2971
+000038b0: 3920 332e 3037 3437 342c 312e 3336 3936  9 3.07474,1.3696
+000038c0: 3920 332e 3738 3936 322c 322e 3832 3438  9 3.78962,2.8248
+000038d0: 3520 312e 3035 3735 312c 322e 3135 3236  5 1.05751,2.1526
+000038e0: 3220 302e 3839 3639 382c 352e 3330 3338  2 0.89698,5.3038
+000038f0: 3820 2d30 2e33 3133 3734 2c37 2e33 3632  8 -0.31374,7.362
+00003900: 3836 202d 302e 3736 3930 332c 312e 3330  86 -0.76903,1.30
+00003910: 3738 3320 2d32 2e34 3737 3831 2c31 2e38  783 -2.47781,1.8
+00003920: 3336 3638 202d 332e 3931 382c 322e 3030  3668 -3.918,2.00
+00003930: 3335 3420 2d31 2e35 3133 3639 2c30 2e31  354 -1.51369,0.1
+00003940: 3735 3336 202d 342e 3035 3338 352c 302e  7536 -4.05385,0.
+00003950: 3132 3831 3320 2d34 2e30 3533 3835 2c30  12813 -4.05385,0
+00003960: 2e31 3238 3133 220a 2020 2020 2020 2069  .12813".       i
+00003970: 643d 2270 6174 6831 3633 3139 2d37 2d33  d="path16319-7-3
+00003980: 2d39 220a 2020 2020 2020 2073 6f64 6970  -9".       sodip
+00003990: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+000039a0: 7373 7373 6322 202f 3e0a 2020 2020 3c75  ssssc" />.    <u
+000039b0: 7365 0a20 2020 2020 2020 783d 2230 220a  se.       x="0".
+000039c0: 2020 2020 2020 2079 3d22 3022 0a20 2020         y="0".   
+000039d0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+000039e0: 2370 6174 6838 3938 352d 3822 0a20 2020  #path8985-8".   
+000039f0: 2020 2020 6964 3d22 7573 6535 3339 220a      id="use539".
+00003a00: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00003a10: 3d22 7472 616e 736c 6174 6528 3534 2e38  ="translate(54.8
+00003a20: 3839 3834 332c 3132 2e38 3235 3739 3129  89843,12.825791)
+00003a30: 2220 2f3e 0a20 2020 203c 7573 650a 2020  " />.    <use.  
+00003a40: 2020 2020 2078 3d22 3022 0a20 2020 2020       x="0".     
+00003a50: 2020 793d 2230 220a 2020 2020 2020 2078    y="0".       x
+00003a60: 6c69 6e6b 3a68 7265 663d 2223 7061 7468  link:href="#path
+00003a70: 3839 3835 2d38 220a 2020 2020 2020 2069  8985-8".       i
+00003a80: 643d 2275 7365 3534 3122 0a20 2020 2020  d="use541".     
+00003a90: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00003aa0: 6e73 6c61 7465 2834 362e 3634 3639 3837  nslate(46.646987
+00003ab0: 2c31 312e 3134 3732 3433 2922 202f 3e0a  ,11.147243)" />.
+00003ac0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00003ad0: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
+00003ae0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+00003af0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00003b00: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
+00003b10: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00003b20: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00003b30: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00003b40: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00003b50: 2031 3136 2e31 3631 3334 2c32 3436 2e35   116.16134,246.5
+00003b60: 3434 3334 2063 2030 2e32 3531 3139 2c2d  4434 c 0.25119,-
+00003b70: 302e 3037 3431 2033 2e35 3533 3035 2c2d  0.0741 3.55305,-
+00003b80: 302e 3432 3139 2035 2e32 3036 3737 2c2d  0.4219 5.20677,-
+00003b90: 302e 3039 3738 2031 2e35 3136 3331 2c30  0.0978 1.51631,0
+00003ba0: 2e32 3937 3139 2034 2e39 3038 312c 2d30  .29719 4.9081,-0
+00003bb0: 2e32 3138 3220 352e 3538 3934 352c 322e  .2182 5.58945,2.
+00003bc0: 3732 3039 3220 302e 3534 3136 322c 322e  72092 0.54162,2.
+00003bd0: 3333 3634 2030 2e37 3238 3139 2c31 342e  3364 0.72819,14.
+00003be0: 3939 3835 3120 2d30 2e32 3738 3233 2c31  99851 -0.27823,1
+00003bf0: 372e 3136 3436 3920 2d31 2e30 3336 3532  7.16469 -1.03652
+00003c00: 2c32 2e32 3330 3934 202d 332e 3838 3031  ,2.23094 -3.8801
+00003c10: 322c 322e 3039 3633 3320 2d35 2e33 3230  2,2.09633 -5.320
+00003c20: 3331 2c32 2e32 3633 3139 202d 312e 3531  31,2.26319 -1.51
+00003c30: 3336 392c 302e 3137 3533 3620 2d34 2e36  369,0.17536 -4.6
+00003c40: 3639 3332 2c2d 302e 3131 3237 3220 2d34  6932,-0.11272 -4
+00003c50: 2e36 3639 3332 2c2d 302e 3131 3237 3222  .66932,-0.11272"
+00003c60: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00003c70: 3136 3331 392d 372d 332d 392d 3222 0a20  16319-7-3-9-2". 
+00003c80: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00003c90: 6f64 6574 7970 6573 3d22 6373 7373 7363  odetypes="cssssc
+00003ca0: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00003cb0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00003cc0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+00003cd0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00003ce0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
+00003cf0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00003d00: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00003d10: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00003d20: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00003d30: 2064 3d22 4d20 3133 362e 3735 3231 382c   d="M 136.75218,
+00003d40: 3234 372e 3231 3638 3120 4820 3134 382e  247.21681 H 148.
+00003d50: 3235 3334 220a 2020 2020 2020 2069 643d  2534".       id=
+00003d60: 2270 6174 6831 3730 3739 2d35 2d32 2d30  "path17079-5-2-0
+00003d70: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00003d80: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00003d90: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+00003da0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00003db0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
+00003dc0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00003dd0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00003de0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00003df0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00003e00: 2064 3d22 6d20 3133 362e 3636 3533 322c   d="m 136.66532,
+00003e10: 3235 362e 3636 3834 3220 6820 382e 3636  256.66842 h 8.66
+00003e20: 3936 3422 0a20 2020 2020 2020 6964 3d22  964".       id="
+00003e30: 7061 7468 3137 3037 392d 352d 322d 302d  path17079-5-2-0-
+00003e40: 3922 202f 3e0a 2020 2020 3c70 6174 680a  9" />.    <path.
+00003e50: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00003e60: 6c6c 3a23 6666 6666 6666 3b66 696c 6c2d  ll:#ffffff;fill-
+00003e70: 6f70 6163 6974 793a 302e 3332 3438 343b  opacity:0.32484;
+00003e80: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00003e90: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+00003ea0: 3435 3833 7078 3b73 7472 6f6b 652d 6c69  4583px;stroke-li
+00003eb0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00003ec0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00003ed0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00003ee0: 3122 0a20 2020 2020 2020 643d 226d 2035  1".       d="m 5
+00003ef0: 332e 3738 3931 3131 2c32 3436 2e38 3034  3.789111,246.804
+00003f00: 3431 202d 312e 3733 3639 3733 2c34 2e30  41 -1.736973,4.0
+00003f10: 3538 3438 2063 202d 312e 3839 3339 3039  5848 c -1.893909
+00003f20: 2c2d 302e 3734 3832 3320 2d34 2e31 3834  ,-0.74823 -4.184
+00003f30: 3237 362c 2d31 2e37 3633 3037 202d 362e  276,-1.76307 -6.
+00003f40: 3338 3133 3631 2c2d 312e 3637 3233 3920  381361,-1.67239 
+00003f50: 2d31 2e37 3137 3935 2c30 2e30 3730 3920  -1.71795,0.0709 
+00003f60: 2d33 2e35 3635 3434 392c 302e 3531 3137  -3.565449,0.5117
+00003f70: 3520 2d34 2e37 3438 3431 332c 312e 3735  5 -4.748413,1.75
+00003f80: 3935 3420 2d31 2e34 3938 3830 392c 312e  954 -1.498809,1.
+00003f90: 3538 3039 3420 2d31 2e39 3037 3433 352c  58094 -1.907435,
+00003fa0: 342e 3034 3738 3820 2d31 2e39 3537 3039  4.04788 -1.95709
+00003fb0: 352c 362e 3232 3538 202d 302e 3034 3834  5,6.2258 -0.0484
+00003fc0: 312c 322e 3132 3239 2030 2e30 3538 3239  1,2.1229 0.05829
+00003fd0: 2c34 2e33 3738 3237 2031 2e35 3336 3834  ,4.37827 1.53684
+00003fe0: 382c 352e 3930 3233 3920 312e 3732 3136  8,5.90239 1.7216
+00003ff0: 3137 2c31 2e37 3734 3636 2033 2e38 3838  17,1.77466 3.888
+00004000: 3836 362c 312e 3732 3235 3720 342e 3932  866,1.72257 4.92
+00004010: 3635 3039 2c31 2e37 3732 3431 2032 2e30  6509,1.77241 2.0
+00004020: 3532 3237 392c 302e 3039 3836 2034 2e33  52279,0.0986 4.3
+00004030: 3733 3432 312c 2d30 2e36 3334 3538 2036  73421,-0.63458 6
+00004040: 2e32 3735 3739 322c 2d31 2e31 3739 3237  .275792,-1.17927
+00004050: 206c 2031 2e36 3537 3739 392c 332e 3833   l 1.657799,3.83
+00004060: 3133 3620 6320 2d32 2e34 3134 3439 2c31  136 c -2.41449,1
+00004070: 2e30 3734 3939 202d 352e 3433 3233 3938  .07499 -5.432398
+00004080: 2c31 2e35 3730 3838 202d 382e 3237 3339  ,1.57088 -8.2739
+00004090: 3533 2c31 2e36 3234 3939 202d 322e 3733  53,1.62499 -2.73
+000040a0: 3239 3839 2c30 2e30 3532 202d 362e 3030  2989,0.052 -6.00
+000040b0: 3135 3437 2c2d 302e 3633 3936 3320 2d37  1547,-0.63963 -7
+000040c0: 2e38 3833 3134 322c 2d32 2e36 3232 3434  .883142,-2.62244
+000040d0: 202d 322e 3035 3035 3932 2c2d 322e 3136   -2.050592,-2.16
+000040e0: 3039 202d 322e 3537 3637 3834 2c2d 352e  09 -2.576784,-5.
+000040f0: 3630 3331 3220 2d32 2e34 3937 3035 322c  60312 -2.497052,
+00004100: 2d38 2e35 3831 3035 2030 2e30 3936 3237  -8.58105 0.09627
+00004110: 2c2d 332e 3539 3537 3520 312e 3033 3630  ,-3.59575 1.0360
+00004120: 3632 2c2d 372e 3632 3734 3120 332e 3536  62,-7.62741 3.56
+00004130: 3532 3232 2c2d 3130 2e31 3835 3134 2031  5222,-10.18514 1
+00004140: 2e39 3338 3132 352c 2d31 2e39 3630 3032  .938125,-1.96002
+00004150: 2035 2e30 3231 3436 2c2d 322e 3636 3932   5.02146,-2.6692
+00004160: 3520 372e 3737 3338 3037 2c2d 322e 3831  5 7.773807,-2.81
+00004170: 3935 3820 322e 3635 3231 3031 2c2d 302e  958 2.652101,-0.
+00004180: 3134 3438 3520 352e 3931 3231 3335 2c31  14485 5.912135,1
+00004190: 2e31 3236 3332 2037 2e37 3432 3031 322c  .12632 7.742012,
+000041a0: 312e 3838 3439 207a 220a 2020 2020 2020  1.8849 z".      
+000041b0: 2069 643d 2270 6174 6831 3838 3533 220a   id="path18853".
+000041c0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000041d0: 6e6f 6465 7479 7065 733d 2263 6373 7373  nodetypes="ccsss
+000041e0: 7373 6363 7373 7373 7363 2220 2f3e 0a20  ssccsssssc" />. 
+000041f0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00004200: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
+00004210: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00004220: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00004230: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+00004240: 3435 3833 7078 3b73 7472 6f6b 652d 6c69  4583px;stroke-li
+00004250: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00004260: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00004270: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00004280: 3122 0a20 2020 2020 2020 643d 226d 2036  1".       d="m 6
+00004290: 352e 3530 3830 3437 2c32 3537 2e34 3935  5.508047,257.495
+000042a0: 3935 2063 2030 2c30 202d 312e 3337 3132  95 c 0,0 -1.3712
+000042b0: 3931 2c2d 322e 3130 3738 3420 2d34 2e32  91,-2.10784 -4.2
+000042c0: 3637 3735 312c 2d32 2e30 3833 3231 202d  67751,-2.08321 -
+000042d0: 322e 3931 3231 3631 2c30 2e30 3234 3820  2.912161,0.0248 
+000042e0: 2d34 2e39 3330 3236 392c 322e 3634 3038  -4.930269,2.6408
+000042f0: 3320 2d35 2e36 3830 3739 392c 342e 3436  3 -5.680799,4.46
+00004300: 3933 3420 2d30 2e36 3535 3831 322c 312e  934 -0.655812,1.
+00004310: 3539 3737 3520 2d30 2e34 3235 3239 322c  59775 -0.425292,
+00004320: 352e 3538 3131 3720 302e 3834 3138 3231  5.58117 0.841821
+00004330: 2c36 2e39 3634 3335 2031 2e31 3030 3638  ,6.96435 1.10068
+00004340: 392c 312e 3230 3135 3120 312e 3930 3738  9,1.20151 1.9078
+00004350: 352c 322e 3132 3031 3620 342e 3731 3932  5,2.12016 4.7192
+00004360: 3131 2c32 2e31 3438 3634 2032 2e32 3934  11,2.14864 2.294
+00004370: 3036 332c 302e 3032 3332 2034 2e34 3931  063,0.0232 4.491
+00004380: 3631 392c 2d31 2e39 3938 3232 2034 2e34  619,-1.99822 4.4
+00004390: 3931 3631 392c 2d31 2e39 3938 3232 206c  91619,-1.99822 l
+000043a0: 202d 302e 3732 3333 3534 2c2d 322e 3439   -0.723354,-2.49
+000043b0: 3637 3920 6320 302c 3020 2d31 2e38 3739  679 c 0,0 -1.879
+000043c0: 3633 382c 312e 3333 3438 3620 2d33 2e35  638,1.33486 -3.5
+000043d0: 3634 3332 342c 312e 3334 3432 3920 2d31  64324,1.34429 -1
+000043e0: 2e35 3231 3935 382c 302e 3030 3920 2d32  .521958,0.009 -2
+000043f0: 2e31 3537 3130 312c 2d30 2e38 3637 3220  .157101,-0.8672 
+00004400: 2d32 2e36 3335 3030 352c 2d31 2e35 3133  -2.635005,-1.513
+00004410: 3120 2d30 2e36 3631 3631 392c 2d30 2e38  1 -0.661619,-0.8
+00004420: 3934 3139 202d 302e 3537 3833 3933 2c2d  9419 -0.578393,-
+00004430: 322e 3832 3230 3820 2d30 2e30 3232 3133  2.82208 -0.02213
+00004440: 2c2d 332e 3738 3533 3620 302e 3338 3237  ,-3.78536 0.3827
+00004450: 3135 2c2d 302e 3636 3237 3520 312e 3537  15,-0.66275 1.57
+00004460: 3136 3432 2c2d 312e 3838 3430 3620 322e  1642,-1.88406 2.
+00004470: 3635 3332 3633 2c2d 312e 3834 3939 3520  653263,-1.84995 
+00004480: 312e 3834 3537 382c 302e 3035 3832 2032  1.84578,0.0582 2
+00004490: 2e38 3137 3930 352c 302e 3838 3136 3720  .817905,0.88167 
+000044a0: 332e 3736 3031 3336 2c31 2e36 3133 3031  3.760136,1.61301
+000044b0: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+000044c0: 6174 6832 3033 3631 220a 2020 2020 2020  ath20361".      
+000044d0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000044e0: 7065 733d 2263 7373 7373 6363 7373 7373  pes="cssssccssss
+000044f0: 6363 2220 2f3e 0a20 2020 203c 7265 6374  cc" />.    <rect
+00004500: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
+00004510: 7061 6369 7479 3a30 2e39 393b 6669 6c6c  pacity:0.99;fill
+00004520: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
+00004530: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
+00004540: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
+00004550: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00004560: 7769 6474 683a 302e 333b 7374 726f 6b65  width:0.3;stroke
+00004570: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+00004580: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
+00004590: 6f75 6e64 3b73 7472 6f6b 652d 6461 7368  ound;stroke-dash
+000045a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000045b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000045c0: 2020 2020 6964 3d22 7265 6374 3230 3431      id="rect2041
+000045d0: 3522 0a20 2020 2020 2020 7769 6474 683d  5".       width=
+000045e0: 2233 2e34 3230 3332 3831 220a 2020 2020  "3.4203281".    
+000045f0: 2020 2068 6569 6768 743d 2231 332e 3639     height="13.69
+00004600: 3638 3135 220a 2020 2020 2020 2078 3d22  6815".       x="
+00004610: 3634 2e36 3634 3539 3722 0a20 2020 2020  64.664597".     
+00004620: 2020 793d 2232 3535 2e33 3432 3734 2220    y="255.34274" 
+00004630: 2f3e 0a20 2020 203c 7265 6374 0a20 2020  />.    <rect.   
+00004640: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
+00004650: 7479 3a30 2e39 393b 6669 6c6c 3a6e 6f6e  ty:0.99;fill:non
+00004660: 653b 6669 6c6c 2d6f 7061 6369 7479 3a30  e;fill-opacity:0
+00004670: 2e33 3234 3834 3b66 696c 6c2d 7275 6c65  .32484;fill-rule
+00004680: 3a6e 6f6e 7a65 726f 3b73 7472 6f6b 653a  :nonzero;stroke:
+00004690: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+000046a0: 6964 7468 3a30 2e33 3b73 7472 6f6b 652d  idth:0.3;stroke-
+000046b0: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
+000046c0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+000046d0: 756e 643b 7374 726f 6b65 2d64 6173 6861  und;stroke-dasha
+000046e0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+000046f0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00004700: 2020 2069 643d 2272 6563 7432 3036 3235     id="rect20625
+00004710: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
+00004720: 302e 3035 3830 3638 3930 3122 0a20 2020  0.058068901".   
+00004730: 2020 2020 6865 6967 6874 3d22 302e 3132      height="0.12
+00004740: 3930 3430 3534 220a 2020 2020 2020 2078  904054".       x
+00004750: 3d22 3739 2e38 3630 3835 3522 0a20 2020  ="79.860855".   
+00004760: 2020 2020 793d 2232 3439 2e38 3030 3633      y="249.80063
+00004770: 2220 2f3e 0a20 2020 203c 7465 7874 0a20  " />.    <text. 
+00004780: 2020 2020 2020 786d 6c3a 7370 6163 653d        xml:space=
+00004790: 2270 7265 7365 7276 6522 0a20 2020 2020  "preserve".     
+000047a0: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
+000047b0: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
+000047c0: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
+000047d0: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
+000047e0: 6c3b 666f 6e74 2d73 7472 6574 6368 3a6e  l;font-stretch:n
+000047f0: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
+00004800: 3235 2e38 3833 3770 783b 6c69 6e65 2d68  25.8837px;line-h
+00004810: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
+00004820: 6661 6d69 6c79 3a55 6275 6e74 753b 2d69  family:Ubuntu;-i
+00004830: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00004840: 6369 6669 6361 7469 6f6e 3a55 6275 6e74  cification:Ubunt
+00004850: 753b 6c65 7474 6572 2d73 7061 6369 6e67  u;letter-spacing
+00004860: 3a30 7078 3b77 6f72 642d 7370 6163 696e  :0px;word-spacin
+00004870: 673a 3070 783b 6669 6c6c 3a23 3030 3030  g:0px;fill:#0000
+00004880: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+00004890: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+000048a0: 726f 6b65 2d77 6964 7468 3a30 2e33 3033  roke-width:0.303
+000048b0: 3332 3422 0a20 2020 2020 2020 783d 2236  324".       x="6
+000048c0: 322e 3332 3032 3734 220a 2020 2020 2020  2.320274".      
+000048d0: 2079 3d22 3133 302e 3836 3334 3222 0a20   y="130.86342". 
+000048e0: 2020 2020 2020 6964 3d22 7465 7874 3230        id="text20
+000048f0: 3638 3122 3e3c 7473 7061 6e0a 2020 2020  681"><tspan.    
+00004900: 2020 2020 2073 6f64 6970 6f64 693a 726f       sodipodi:ro
+00004910: 6c65 3d22 6c69 6e65 220a 2020 2020 2020  le="line".      
+00004920: 2020 2069 643d 2274 7370 616e 3230 3637     id="tspan2067
+00004930: 3922 0a20 2020 2020 2020 2020 7374 796c  9".         styl
+00004940: 653d 2266 6f6e 742d 7374 796c 653a 6e6f  e="font-style:no
+00004950: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
+00004960: 743a 6e6f 726d 616c 3b66 6f6e 742d 7765  t:normal;font-we
+00004970: 6967 6874 3a62 6f6c 643b 666f 6e74 2d73  ight:bold;font-s
+00004980: 7472 6574 6368 3a6e 6f72 6d61 6c3b 666f  tretch:normal;fo
+00004990: 6e74 2d73 697a 653a 3235 2e38 3833 3770  nt-size:25.8837p
+000049a0: 783b 666f 6e74 2d66 616d 696c 793a 274e  x;font-family:'N
+000049b0: 696d 6275 7320 5361 6e73 273b 2d69 6e6b  imbus Sans';-ink
+000049c0: 7363 6170 652d 666f 6e74 2d73 7065 6369  scape-font-speci
+000049d0: 6669 6361 7469 6f6e 3a27 4e69 6d62 7573  fication:'Nimbus
+000049e0: 2053 616e 7320 426f 6c64 273b 7374 726f   Sans Bold';stro
+000049f0: 6b65 2d77 6964 7468 3a30 2e33 3033 3332  ke-width:0.30332
+00004a00: 3422 0a20 2020 2020 2020 2020 783d 2236  4".         x="6
+00004a10: 322e 3332 3032 3734 220a 2020 2020 2020  2.320274".      
+00004a20: 2020 2079 3d22 3133 302e 3836 3334 3222     y="130.86342"
+00004a30: 3e43 6170 7950 4446 3c2f 7473 7061 6e3e  >CapyPDF</tspan>
+00004a40: 3c2f 7465 7874 3e0a 2020 2020 3c65 6c6c  </text>.    <ell
+00004a50: 6970 7365 0a20 2020 2020 2020 7374 796c  ipse.       styl
+00004a60: 653d 226f 7061 6369 7479 3a30 2e39 393b  e="opacity:0.99;
+00004a70: 6669 6c6c 3a23 3866 6430 6466 3b66 696c  fill:#8fd0df;fil
+00004a80: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
+00004a90: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
+00004aa0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+00004ab0: 6f6b 652d 7769 6474 683a 312e 3538 3735  oke-width:1.5875
+00004ac0: 652d 3038 3b73 7472 6f6b 652d 6c69 6e65  e-08;stroke-line
+00004ad0: 6361 703a 726f 756e 643b 7374 726f 6b65  cap:round;stroke
+00004ae0: 2d6c 696e 656a 6f69 6e3a 726f 756e 643b  -linejoin:round;
+00004af0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00004b00: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00004b10: 6838 3938 352d 3822 0a20 2020 2020 2020  h8985-8".       
+00004b20: 6378 3d22 3230 362e 3436 3336 3822 0a20  cx="206.46368". 
+00004b30: 2020 2020 2020 6379 3d22 3133 332e 3538        cy="133.58
+00004b40: 3130 3122 0a20 2020 2020 2020 7278 3d22  101".       rx="
+00004b50: 312e 3437 3536 3036 3422 0a20 2020 2020  1.4756064".     
+00004b60: 2020 7279 3d22 312e 3732 3236 3838 3422    ry="1.7226884"
+00004b70: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00004b80: 6d3d 2272 6f74 6174 6528 3430 2e32 3337  m="rotate(40.237
+00004b90: 3234 3129 2220 2f3e 0a20 2020 203c 7573  241)" />.    <us
+00004ba0: 650a 2020 2020 2020 2078 3d22 3022 0a20  e.       x="0". 
+00004bb0: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
+00004bc0: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00004bd0: 7061 7468 3839 3835 2d38 220a 2020 2020  path8985-8".    
+00004be0: 2020 2069 643d 2275 7365 3236 3030 3622     id="use26006"
+00004bf0: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00004c00: 6d3d 2274 7261 6e73 6c61 7465 2832 2e31  m="translate(2.1
+00004c10: 3132 3532 3232 2c32 332e 3637 3235 3633  125222,23.672563
+00004c20: 2922 202f 3e0a 2020 2020 3c72 6563 740a  )" />.    <rect.
+00004c30: 2020 2020 2020 2073 7479 6c65 3d22 6f70         style="op
+00004c40: 6163 6974 793a 302e 3939 3b66 696c 6c3a  acity:0.99;fill:
+00004c50: 6e6f 6e65 3b66 696c 6c2d 6f70 6163 6974  none;fill-opacit
+00004c60: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
+00004c70: 6e7a 6572 6f3b 7374 726f 6b65 3a23 3030  nzero;stroke:#00
+00004c80: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+00004c90: 683a 302e 333b 7374 726f 6b65 2d6c 696e  h:0.3;stroke-lin
+00004ca0: 6563 6170 3a72 6f75 6e64 3b73 7472 6f6b  ecap:round;strok
+00004cb0: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+00004cc0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00004cd0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00004ce0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00004cf0: 6964 3d22 7265 6374 3230 3431 352d 3522  id="rect20415-5"
+00004d00: 0a20 2020 2020 2020 7769 6474 683d 2233  .       width="3
+00004d10: 2e34 3230 3332 3831 220a 2020 2020 2020  .4203281".      
+00004d20: 2068 6569 6768 743d 2231 382e 3630 3731   height="18.6071
+00004d30: 3231 220a 2020 2020 2020 2078 3d22 3730  21".       x="70
+00004d40: 2e34 3833 3137 220a 2020 2020 2020 2079  .48317".       y
+00004d50: 3d22 3235 352e 3336 3637 3322 202f 3e0a  ="255.36673" />.
+00004d60: 2020 2020 3c75 7365 0a20 2020 2020 2020      <use.       
+00004d70: 783d 2230 220a 2020 2020 2020 2079 3d22  x="0".       y="
+00004d80: 3022 0a20 2020 2020 2020 786c 696e 6b3a  0".       xlink:
+00004d90: 6872 6566 3d22 2370 6174 6838 3938 352d  href="#path8985-
+00004da0: 3822 0a20 2020 2020 2020 6964 3d22 7573  8".       id="us
+00004db0: 6532 3630 3132 220a 2020 2020 2020 2074  e26012".       t
+00004dc0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00004dd0: 6174 6528 3130 2e38 3133 3333 342c 3239  ate(10.813334,29
+00004de0: 2e34 3633 3931 3529 2220 2f3e 0a20 2020  .463915)" />.   
+00004df0: 203c 7573 650a 2020 2020 2020 2078 3d22   <use.       x="
+00004e00: 3022 0a20 2020 2020 2020 793d 2230 220a  0".       y="0".
+00004e10: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
+00004e20: 663d 2223 7061 7468 3839 3835 2d38 220a  f="#path8985-8".
+00004e30: 2020 2020 2020 2069 643d 2275 7365 3236         id="use26
+00004e40: 3031 3422 0a20 2020 2020 2020 7472 616e  014".       tran
+00004e50: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00004e60: 2836 2e39 3938 3231 3638 2c33 322e 3030  (6.9982168,32.00
+00004e70: 3338 3934 2922 202f 3e0a 2020 2020 3c70  3894)" />.    <p
+00004e80: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00004e90: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+00004ea0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+00004eb0: 652d 7769 6474 683a 302e 3236 3435 3833  e-width:0.264583
+00004ec0: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
+00004ed0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00004ee0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00004ef0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00004f00: 2020 2020 2020 643d 226d 2037 332e 3134        d="m 73.14
+00004f10: 3332 3931 2c32 3539 2e31 3435 3133 2063  3291,259.14513 c
+00004f20: 2030 2e32 3038 3639 2c2d 302e 3035 3833   0.20869,-0.0583
+00004f30: 2032 2e34 3435 3934 392c 2d32 2e32 3032   2.445949,-2.202
+00004f40: 3537 2034 2e39 3237 3431 342c 2d32 2e32  57 4.927414,-2.2
+00004f50: 3330 3637 2032 2e30 3831 3933 392c 2d30  3067 2.081939,-0
+00004f60: 2e30 3233 3620 332e 3139 3535 3034 2c30  .0236 3.195504,0
+00004f70: 2e36 3132 2034 2e30 3138 3037 312c 312e  .612 4.018071,1.
+00004f80: 3831 3739 3420 312e 3037 3533 3839 2c31  81794 1.075389,1
+00004f90: 2e35 3736 3538 2031 2e30 3833 3632 392c  .57658 1.083629,
+00004fa0: 342e 3633 3730 3220 302e 3131 3038 3937  4.63702 0.110897
+00004fb0: 2c36 2e32 3737 3539 202d 302e 3836 3139  ,6.27759 -0.8619
+00004fc0: 342c 312e 3435 3337 3120 2d32 2e33 3435  4,1.45371 -2.345
+00004fd0: 3233 322c 322e 3435 3734 3620 2d34 2e30  232,2.45746 -4.0
+00004fe0: 3932 3139 332c 322e 3435 3338 3920 2d32  92193,2.45389 -2
+00004ff0: 2e31 3138 3236 372c 2d30 2e30 3034 202d  .118267,-0.004 -
+00005000: 332e 3437 3932 3633 2c2d 302e 3934 3531  3.479263,-0.9451
+00005010: 3920 2d34 2e35 3837 3732 312c 2d32 2e30  9 -4.587721,-2.0
+00005020: 3534 3933 220a 2020 2020 2020 2069 643d  5493".       id=
+00005030: 2270 6174 6831 3633 3139 2d37 2d39 220a  "path16319-7-9".
+00005040: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00005050: 6e6f 6465 7479 7065 733d 2263 7373 7373  nodetypes="cssss
+00005060: 6322 202f 3e0a 2020 2020 3c70 6174 680a  c" />.    <path.
+00005070: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00005080: 6c6c 3a6e 6f6e 653b 6669 6c6c 2d6f 7061  ll:none;fill-opa
+00005090: 6369 7479 3a31 3b73 7472 6f6b 653a 2330  city:1;stroke:#0
+000050a0: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+000050b0: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
+000050c0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+000050d0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+000050e0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+000050f0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00005100: 2064 3d22 6d20 3732 2e38 3530 3731 392c   d="m 72.850719,
+00005110: 3235 372e 3938 3133 2031 2e30 3936 3339  257.9813 1.09639
+00005120: 332c 322e 3435 3539 3720 6320 302c 3020  3,2.45597 c 0,0 
+00005130: 322e 3530 3536 3337 2c2d 312e 3835 3035  2.505637,-1.8505
+00005140: 3420 332e 3839 3039 3936 2c2d 312e 3831  4 3.890996,-1.81
+00005150: 3436 2031 2e32 3234 3237 352c 302e 3033  46 1.224275,0.03
+00005160: 3138 2032 2e35 3833 3133 2c30 2e35 3632  18 2.58313,0.562
+00005170: 3239 2033 2e31 3535 3936 342c 312e 3731  29 3.155964,1.71
+00005180: 3538 2030 2e36 3438 3031 2c31 2e33 3034  58 0.64801,1.304
+00005190: 3839 2030 2e34 3337 3532 392c 322e 3832  89 0.437529,2.82
+000051a0: 3630 3520 2d30 2e32 3230 3632 392c 332e  605 -0.220629,3.
+000051b0: 3736 3920 2d30 2e35 3535 3938 312c 302e  769 -0.555981,0.
+000051c0: 3739 3635 3620 2d31 2e33 3539 3039 322c  79656 -1.359092,
+000051d0: 312e 3530 3038 3720 2d32 2e32 3830 3837  1.50087 -2.28087
+000051e0: 342c 312e 3633 3537 202d 312e 3437 3730  4,1.6357 -1.4770
+000051f0: 3138 2c30 2e32 3136 3034 202d 332e 3138  18,0.21604 -3.18
+00005200: 3033 3334 2c2d 302e 3532 3537 3820 2d34  0334,-0.52578 -4
+00005210: 2e37 3535 3336 2c2d 322e 3039 3434 3620  .75536,-2.09446 
+00005220: 6c20 2d30 2e35 3531 3636 332c 332e 3032  l -0.551663,3.02
+00005230: 3138 3520 6320 302e 3730 3935 3434 2c31  185 c 0.709544,1
+00005240: 2e30 3139 3839 2032 2e37 3831 3539 322c  .01989 2.781592,
+00005250: 322e 3334 3035 3420 342e 3733 3535 3037  2.34054 4.735507
+00005260: 2c32 2e33 3136 3036 2032 2e32 3438 3937  ,2.31606 2.24897
+00005270: 342c 2d30 2e30 3238 3220 342e 3433 3936  4,-0.0282 4.4396
+00005280: 3132 2c2d 312e 3632 3334 2035 2e35 3730  12,-1.6234 5.570
+00005290: 3636 312c 2d33 2e34 3430 3838 2031 2e30  661,-3.44088 1.0
+000052a0: 3031 3634 312c 2d31 2e36 3039 3533 2031  01641,-1.60953 1
+000052b0: 2e31 3834 3932 342c 2d35 2e34 3534 3538  .184924,-5.45458
+000052c0: 2030 2e34 3330 3734 2c2d 362e 3939 3139   0.43074,-6.9919
+000052d0: 3320 2d30 2e39 3137 3231 342c 2d31 2e38  3 -0.917214,-1.8
+000052e0: 3639 3637 202d 332e 3136 3631 3432 2c2d  6967 -3.166142,-
+000052f0: 332e 3236 3638 3220 2d35 2e33 3337 3036  3.26682 -5.33706
+00005300: 372c 2d33 2e31 3939 3620 2d32 2e34 3230  7,-3.1996 -2.420
+00005310: 3833 362c 302e 3037 3520 2d35 2e37 3334  836,0.075 -5.734
+00005320: 3636 382c 322e 3632 3730 3920 2d35 2e37  668,2.62709 -5.7
+00005330: 3334 3636 382c 322e 3632 3730 3920 7a22  34668,2.62709 z"
+00005340: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00005350: 3236 3734 3422 0a20 2020 2020 2020 736f  26744".       so
+00005360: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00005370: 3d22 6363 7373 7373 6363 7373 7373 6322  ="ccssssccssssc"
+00005380: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00005390: 2020 2020 2069 643d 2272 6563 7432 3034       id="rect204
+000053a0: 3135 2d35 2d35 220a 2020 2020 2020 2073  15-5-5".       s
+000053b0: 7479 6c65 3d22 6f70 6163 6974 793a 302e  tyle="opacity:0.
+000053c0: 3939 3b66 696c 6c3a 6e6f 6e65 3b73 7472  99;fill:none;str
+000053d0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+000053e0: 6b65 2d77 6964 7468 3a30 2e33 3b73 7472  ke-width:0.3;str
+000053f0: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00005400: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00005410: 6e3a 726f 756e 6422 0a20 2020 2020 2020  n:round".       
+00005420: 643d 226d 2038 382e 3437 3837 3131 2c32  d="m 88.478711,2
+00005430: 3232 2e39 3031 3837 2063 2030 2c30 2030  22.90187 c 0,0 0
+00005440: 2e33 3236 3338 332c 2d30 2e34 3338 3120  .326383,-0.4381 
+00005450: 312e 3732 3837 3033 2c2d 302e 3433 3831  1.728703,-0.4381
+00005460: 2031 2e34 3032 3332 2c30 2031 2e36 3931   1.40232,0 1.691
+00005470: 3632 352c 302e 3433 3831 2031 2e36 3931  625,0.4381 1.691
+00005480: 3632 352c 302e 3433 3831 2076 2031 382e  625,0.4381 v 18.
+00005490: 3335 3032 3520 6320 2d30 2e30 3130 3239  35025 c -0.01029
+000054a0: 2c30 2e30 3133 3620 2d30 2e33 3237 3637  ,0.0136 -0.32767
+000054b0: 322c 302e 3234 3737 3220 2d31 2e37 3130  2,0.24772 -1.710
+000054c0: 3136 342c 302e 3235 3638 3720 2d31 2e33  164,0.25687 -1.3
+000054d0: 3832 3439 322c 302e 3030 3920 2d31 2e37  82492,0.009 -1.7
+000054e0: 3130 3136 342c 2d30 2e32 3536 3837 202d  10164,-0.25687 -
+000054f0: 312e 3731 3031 3634 2c2d 302e 3235 3638  1.710164,-0.2568
+00005500: 3720 7a22 0a20 2020 2020 2020 736f 6469  7 z".       sodi
+00005510: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
+00005520: 637a 6363 7a63 6322 202f 3e0a 2020 2020  czcczcc" />.    
+00005530: 3c70 6174 680a 2020 2020 2020 2069 643d  <path.       id=
+00005540: 2272 6563 7432 3034 3135 2d35 2d35 2d33  "rect20415-5-5-3
+00005550: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+00005560: 6f70 6163 6974 793a 302e 3939 3b66 696c  opacity:0.99;fil
+00005570: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
+00005580: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00005590: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+000055a0: 6964 7468 3a30 2e33 3b73 7472 6f6b 652d  idth:0.3;stroke-
+000055b0: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
+000055c0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+000055d0: 756e 6422 0a20 2020 2020 2020 643d 226d  und".       d="m
+000055e0: 2039 342e 3030 3930 3735 2c32 3233 2e32   94.009075,223.2
+000055f0: 3539 3731 2063 2030 2c2d 302e 3430 3334  5971 c 0,-0.4034
+00005600: 3420 302e 3135 3534 3838 2c2d 302e 3535  4 0.155488,-0.55
+00005610: 3635 3820 302e 3237 3631 372c 2d30 2e36  658 0.27617,-0.6
+00005620: 3535 3236 2030 2e31 3230 3638 322c 2d30  5526 0.120682,-0
+00005630: 2e30 3938 3720 302e 3431 3639 3531 2c2d  .0987 0.416951,-
+00005640: 302e 3237 3635 3520 312e 3435 3134 3132  0.27655 1.451412
+00005650: 2c2d 302e 3236 3633 3720 312e 3033 3434  ,-0.26637 1.0344
+00005660: 3631 2c30 2e30 3130 3220 312e 3137 3432  61,0.0102 1.1742
+00005670: 342c 302e 3038 3231 2031 2e34 3031 3234  4,0.0821 1.40124
+00005680: 362c 302e 3235 3833 3520 302e 3137 3037  6,0.25835 0.1707
+00005690: 3932 2c30 2e31 3332 3537 2030 2e32 3931  92,0.13257 0.291
+000056a0: 3530 312c 302e 3338 3830 3420 302e 3239  501,0.38804 0.29
+000056b0: 3135 3031 2c30 2e36 3633 3238 2076 2031  1501,0.66328 v 1
+000056c0: 382e 3237 3334 2068 202d 332e 3432 3033  8.2734 h -3.4203
+000056d0: 3238 207a 220a 2020 2020 2020 2073 6f64  28 z".       sod
+000056e0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+000056f0: 2273 7a7a 7373 6363 7322 202f 3e0a 2020  "szzssccs" />.  
+00005700: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+00005710: 7479 6c65 3d22 6669 6c6c 3a23 3738 3434  tyle="fill:#7844
+00005720: 3231 3b73 7472 6f6b 653a 6e6f 6e65 3b73  21;stroke:none;s
+00005730: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+00005740: 3435 3833 7078 3b73 7472 6f6b 652d 6c69  4583px;stroke-li
+00005750: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00005760: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00005770: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00005780: 3122 0a20 2020 2020 2020 643d 226d 2031  1".       d="m 1
+00005790: 3734 2e33 3139 3836 2c36 362e 3734 3338  74.31986,66.7438
+000057a0: 3820 6320 2d30 2e31 3830 382c 312e 3139  8 c -0.1808,1.19
+000057b0: 3237 3835 202d 362e 3837 3837 2c31 352e  2785 -6.8787,15.
+000057c0: 3632 3137 3133 202d 3136 2e30 3435 3337  621713 -16.04537
+000057d0: 2c31 352e 3233 3633 3737 202d 3136 2e36  ,15.236377 -16.6
+000057e0: 3231 3031 2c2d 302e 3639 3836 3932 202d  2101,-0.698692 -
+000057f0: 3333 2e38 3635 3735 2c2d 302e 3235 3735  33.86575,-0.2575
+00005800: 3934 202d 3439 2e36 3537 3436 2c2d 352e  94 -49.65746,-5.
+00005810: 3433 3737 3836 202d 312e 3437 3234 382c  437786 -1.47248,
+00005820: 2d30 2e34 3833 3032 3120 2d34 2e35 3032  -0.483021 -4.502
+00005830: 3538 2c2d 322e 3330 3937 3233 202d 352e  58,-2.309723 -5.
+00005840: 3230 3337 382c 2d31 2e37 3737 3136 3620  20378,-1.777166 
+00005850: 2d30 2e36 3933 3037 2c30 2e35 3236 3338  -0.69307,0.52638
+00005860: 3520 312e 3136 3638 332c 322e 3030 3337  5 1.16683,2.0037
+00005870: 3038 2032 2e33 3733 3938 2c32 2e37 3038  08 2.37398,2.708
+00005880: 3138 3720 342e 3737 3435 362c 322e 3535  187 4.77456,2.55
+00005890: 3036 3137 2031 302e 3338 3632 392c 332e  0617 10.38629,3.
+000058a0: 3437 3933 3735 2031 342e 3332 3336 392c  479375 14.32369,
+000058b0: 372e 3635 3138 3520 322e 3030 3333 312c  7.65185 2.00331,
+000058c0: 312e 3538 3135 3632 202d 382e 3136 3131  1.581562 -8.1611
+000058d0: 2c31 382e 3639 3734 3238 202d 372e 3835  ,18.697428 -7.85
+000058e0: 3737 322c 3139 2e35 3530 3736 3820 312e  772,19.550768 1.
+000058f0: 3536 3934 352c 342e 3431 3435 3820 3136  56945,4.41458 16
+00005900: 2e32 3831 3933 2c2d 3138 2e32 3732 3630  .28193,-18.27260
+00005910: 3920 3135 2e39 3936 3037 2c2d 3139 2e35  9 15.99607,-19.5
+00005920: 3033 3939 3620 6c20 3338 2e33 3036 3431  03996 l 38.30641
+00005930: 2c30 2e37 3438 3335 3420 6320 362e 3137  ,0.748354 c 6.17
+00005940: 3137 352c 2d35 2e37 3939 3035 3120 362e  175,-5.799051 6.
+00005950: 3534 3339 392c 2d31 332e 3134 3531 3237  54399,-13.145127
+00005960: 2037 2e37 3634 3138 2c2d 3139 2e31 3736   7.76418,-19.176
+00005970: 3538 3820 7a22 0a20 2020 2020 2020 6964  588 z".       id
+00005980: 3d22 7061 7468 3230 220a 2020 2020 2020  ="path20".      
+00005990: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000059a0: 7065 733d 2263 7373 7363 6373 6363 6322  pes="csssccsccc"
+000059b0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+000059c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+000059d0: 3a6e 6f6e 653b 6669 6c6c 2d6f 7061 6369  :none;fill-opaci
+000059e0: 7479 3a31 3b73 7472 6f6b 653a 2330 3030  ty:1;stroke:#000
+000059f0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00005a00: 3a34 3b73 7472 6f6b 652d 6c69 6e65 6361  :4;stroke-lineca
+00005a10: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
+00005a20: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00005a30: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00005a40: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00005a50: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00005a60: 4d20 3733 2e31 3531 3531 312c 3732 2e39  M 73.151511,72.9
+00005a70: 3632 3231 3920 3930 2e35 3230 3237 342c  62219 90.520274,
+00005a80: 3533 2e39 3738 3639 206d 2031 352e 3832  53.97869 m 15.82
+00005a90: 3734 3136 2c2d 382e 3439 3135 3332 2063  7416,-8.491532 c
+00005aa0: 2032 362e 3435 3338 322c 2d32 2e30 3730   26.45382,-2.070
+00005ab0: 3431 3320 3339 2e31 3938 352c 2d30 2e38  413 39.1985,-0.8
+00005ac0: 3436 3132 3920 3538 2e36 3837 3635 2c33  46129 58.68765,3
+00005ad0: 2e31 3133 3039 3120 332e 3434 3532 312c  .113091 3.44521,
+00005ae0: 302e 3639 3938 3934 2035 2e32 3733 3735  0.699894 5.27375
+00005af0: 2c32 2e33 3331 3032 2036 2e38 3839 3431  ,2.33102 6.88941
+00005b00: 2c35 2e33 3135 3037 2034 2e37 3737 3431  ,5.31507 4.77741
+00005b10: 2c38 2e38 3233 3633 2035 2e30 3535 3832  ,8.82363 5.05582
+00005b20: 2c31 372e 3438 3233 3420 2d31 2e30 3536  ,17.48234 -1.056
+00005b30: 392c 3237 2e32 3737 3833 202d 312e 3430  9,27.27783 -1.40
+00005b40: 3138 362c 322e 3234 3634 3420 2d34 2e31  186,2.24644 -4.1
+00005b50: 3932 3836 2c34 2e38 3038 3433 202d 362e  9286,4.80843 -6.
+00005b60: 3833 3439 312c 342e 3938 3533 3420 2d31  83491,4.98534 -1
+00005b70: 312e 3332 3432 322c 302e 3735 3832 3720  1.32422,0.75827 
+00005b80: 2d32 362e 3334 3431 362c 2d30 2e36 3236  -26.34416,-0.626
+00005b90: 3720 2d33 312e 3939 3337 392c 2d30 2e38  7 -31.99379,-0.8
+00005ba0: 3837 3938 202d 332e 3633 3239 352c 2d30  8798 -3.63295,-0
+00005bb0: 2e31 3638 3031 202d 362e 3833 3832 322c  .16801 -6.83822,
+00005bc0: 332e 3434 3636 3137 202d 372e 3930 3238  3.446617 -7.9028
+00005bd0: 382c 362e 3136 3536 3920 2d32 2e39 3833  8,6.16569 -2.983
+00005be0: 3134 2c37 2e36 3138 3736 3120 2d36 2e38  14,7.618761 -6.8
+00005bf0: 3937 3734 2c31 302e 3533 3137 3331 202d  9774,10.531731 -
+00005c00: 3132 2e31 3632 3539 2c31 352e 3232 3332  12.16259,15.2232
+00005c10: 3031 220a 2020 2020 2020 2069 643d 2270  01".       id="p
+00005c20: 6174 6831 220a 2020 2020 2020 2073 6f64  ath1".       sod
+00005c30: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+00005c40: 2263 6363 7373 7373 7373 6322 202f 3e0a  "cccssssssc" />.
+00005c50: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00005c60: 2073 7479 6c65 3d22 6669 6c6c 3a23 3738   style="fill:#78
+00005c70: 3434 3231 3b73 7472 6f6b 653a 6e6f 6e65  4421;stroke:none
+00005c80: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00005c90: 3236 3435 3833 7078 3b73 7472 6f6b 652d  264583px;stroke-
+00005ca0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00005cb0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00005cc0: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00005cd0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00005ce0: 2031 3136 2e32 3531 3532 2c35 342e 3036   116.25152,54.06
+00005cf0: 3935 3936 2063 2032 2e34 3734 3536 2c31  9596 c 2.47456,1
+00005d00: 2e32 3039 3932 3120 342e 3435 3537 352c  .209921 4.45575,
+00005d10: 312e 3936 3335 3220 382e 3038 3334 352c  1.96352 8.08345,
+00005d20: 322e 3230 3837 3835 2034 2e34 3532 3432  2.208785 4.45242
+00005d30: 2c30 2e33 3031 3032 3420 372e 3836 3039  ,0.301024 7.8609
+00005d40: 382c 302e 3331 3137 3732 2031 312e 3231  8,0.311772 11.21
+00005d50: 3137 342c 2d30 2e34 3236 3734 3520 312e  174,-0.426745 1.
+00005d60: 3133 3032 372c 2d30 2e32 3439 3131 3320  13027,-0.249113 
+00005d70: 2d39 2e38 3233 3133 2c2d 342e 3330 3837  -9.82313,-4.3087
+00005d80: 3135 202d 3130 2e31 3033 3736 2c2d 342e  15 -10.10376,-4.
+00005d90: 3236 3139 3432 202d 302e 3238 3036 342c  261942 -0.28064,
+00005da0: 302e 3034 3637 3720 2d39 2e31 3931 3433  0.04677 -9.19143
+00005db0: 2c32 2e34 3739 3839 3720 2d39 2e31 3931  ,2.479897 -9.191
+00005dc0: 3433 2c32 2e34 3739 3839 3720 7a22 0a20  43,2.479897 z". 
+00005dd0: 2020 2020 2020 6964 3d22 7061 7468 3231        id="path21
+00005de0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
+00005df0: 693a 6e6f 6465 7479 7065 733d 2263 7373  i:nodetypes="css
+00005e00: 7363 6322 202f 3e0a 2020 2020 3c70 6174  scc" />.    <pat
+00005e10: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+00005e20: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+00005e30: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00005e40: 7769 6474 683a 333b 7374 726f 6b65 2d6c  width:3;stroke-l
+00005e50: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
+00005e60: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00005e70: 6572 3b73 7472 6f6b 652d 6461 7368 6172  er;stroke-dashar
+00005e80: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00005e90: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00005ea0: 2020 643d 226d 2031 3335 2e32 3936 3036    d="m 135.29606
+00005eb0: 2c35 342e 3535 3438 3639 2063 202d 392e  ,54.554869 c -9.
+00005ec0: 3938 3732 382c 2d33 2e34 3538 3538 202d  98728,-3.45858 -
+00005ed0: 3134 2e34 3831 3431 2c2d 322e 3636 3336  14.48141,-2.6636
+00005ee0: 3820 2d31 382e 3830 3834 392c 2d31 2e37  8 -18.80849,-1.7
+00005ef0: 3339 3434 220a 2020 2020 2020 2069 643d  3944".       id=
+00005f00: 2270 6174 6833 220a 2020 2020 2020 2073  "path3".       s
+00005f10: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00005f20: 733d 2263 6322 202f 3e0a 2020 2020 3c70  s="cc" />.    <p
+00005f30: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00005f40: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
+00005f50: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00005f60: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+00005f70: 6f6b 652d 7769 6474 683a 302e 3836 353b  oke-width:0.865;
+00005f80: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00005f90: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00005fa0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00005fb0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00005fc0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00005fd0: 220a 2020 2020 2020 2064 3d22 6d20 3132  ".       d="m 12
+00005fe0: 392e 3431 3535 352c 3533 2e32 3637 3933  9.41555,53.26793
+00005ff0: 3920 6320 312e 3132 3833 342c 322e 3432  9 c 1.12834,2.42
+00006000: 3039 3820 2d31 2e32 3935 3335 2c33 2e38  098 -1.29535,3.8
+00006010: 3439 3439 202d 342e 3334 3232 382c 332e  4949 -4.34228,3.
+00006020: 3731 3935 3920 2d32 2e34 3536 3537 2c30  71959 -2.45657,0
+00006030: 2e30 3939 3120 2d35 2e33 3033 3938 2c2d  .0991 -5.30398,-
+00006040: 322e 3133 3234 202d 352e 3733 3433 2c2d  2.1324 -5.7343,-
+00006050: 342e 3338 3531 3220 332e 3632 3135 332c  4.38512 3.62153,
+00006060: 2d30 2e34 3439 3633 2036 2e33 3137 3135  -0.44963 6.31715
+00006070: 2c2d 302e 3931 3735 3520 3130 2e30 3736  ,-0.91755 10.076
+00006080: 3538 2c30 2e36 3635 3533 207a 220a 2020  58,0.66553 z".  
+00006090: 2020 2020 2069 643d 2270 6174 6834 220a       id="path4".
+000060a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000060b0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+000060c0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+000060d0: 2020 2020 2069 643d 2270 6174 6834 3139       id="path419
+000060e0: 2d33 2d30 220a 2020 2020 2020 2073 7479  -3-0".       sty
+000060f0: 6c65 3d22 6669 6c6c 3a23 6330 3137 3030  le="fill:#c01700
+00006100: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00006110: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+00006120: 6f3b 7374 726f 6b65 3a6e 6f6e 653b 7374  o;stroke:none;st
+00006130: 726f 6b65 2d77 6964 7468 3a30 2e34 3836  roke-width:0.486
+00006140: 3133 7078 3b73 7472 6f6b 652d 6c69 6e65  13px;stroke-line
+00006150: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00006160: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00006170: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00006180: 0a20 2020 2020 2020 643d 226d 2032 3138  .       d="m 218
+00006190: 2e39 3633 3139 2c35 332e 3737 3438 3336  .96319,53.774836
+000061a0: 2063 202d 302e 3734 3630 322c 302e 3430   c -0.74602,0.40
+000061b0: 3333 3532 202d 302e 3738 3932 332c 312e  3352 -0.78923,1.
+000061c0: 3230 3937 3831 2032 2e34 3038 3034 2c34  209781 2.40804,4
+000061d0: 2e36 3137 3338 3520 342e 3139 3437 352c  .617385 4.19475,
+000061e0: 342e 3437 3036 3938 2032 342e 3335 3930  4.470698 24.3590
+000061f0: 322c 3131 2e37 3537 3630 3620 3338 2e38  2,11.757606 38.8
+00006200: 3232 3838 2c31 312e 3638 3932 3338 2032  2288,11.689238 2
+00006210: 2e34 3433 3337 2c2d 302e 3335 3430 3436  .44337,-0.354046
+00006220: 2032 2e36 3837 2c2d 302e 3436 3333 3832   2.687,-0.463382
+00006230: 2032 2e37 3430 3334 2c2d 312e 3130 3439   2.74034,-1.1049
+00006240: 3033 2030 2e30 3536 372c 2d30 2e36 3831  03 0.0567,-0.681
+00006250: 3531 3220 2d30 2e31 3839 3537 2c2d 312e  512 -0.18957,-1.
+00006260: 3132 3933 3034 202d 322e 3430 3838 322c  129304 -2.40882,
+00006270: 2d30 2e38 3339 3131 3220 2d38 2e33 3931  -0.839112 -8.391
+00006280: 3336 2c31 2e30 3937 3235 3420 2d33 322e  36,1.097254 -32.
+00006290: 3731 3733 372c 3233 2e30 3032 3836 3720  71737,23.002867 
+000062a0: 2d33 342e 3537 3439 2c32 372e 3531 3833  -34.5749,27.5183
+000062b0: 3438 202d 312e 3035 3933 352c 322e 3537  48 -1.05935,2.57
+000062c0: 3531 3737 202d 302e 3530 3334 312c 332e  5177 -0.50341,3.
+000062d0: 3831 3735 3637 2030 2e31 3839 3934 2c33  817567 0.18994,3
+000062e0: 2e39 3332 3831 3520 302e 3733 3336 382c  .932815 0.73368,
+000062f0: 302e 3132 3139 3533 2031 2e34 3839 3033  0.121953 1.48903
+00006300: 2c2d 312e 3934 3837 3637 2031 2e34 3230  ,-1.948767 1.420
+00006310: 3134 2c2d 362e 3934 3538 3234 202d 302e  14,-6.945824 -0.
+00006320: 3139 3134 312c 2d31 332e 3838 3531 3338  19141,-13.885138
+00006330: 202d 312e 3934 3437 322c 2d32 342e 3134   -1.94472,-24.14
+00006340: 3731 202d 352e 3831 3732 362c 2d33 342e  71 -5.81726,-34.
+00006350: 3739 3333 3434 202d 312e 3533 3533 382c  793344 -1.53538,
+00006360: 2d34 2e32 3231 3033 3520 2d32 2e30 3439  -4.221035 -2.049
+00006370: 3135 2c2d 342e 3436 3939 3439 202d 322e  15,-4.469949 -2.
+00006380: 3738 3033 362c 2d34 2e30 3734 3630 3320  78036,-4.074603 
+00006390: 7a20 6d20 342e 3536 3034 322c 312e 3839  z m 4.56042,1.89
+000063a0: 3834 3036 2063 2035 2e39 3433 3434 2c31  8406 c 5.94344,1
+000063b0: 352e 3339 3433 3435 2036 2e30 3031 3832  5.394345 6.00182
+000063c0: 2c31 382e 3831 3430 3535 2037 2e30 3335  ,18.814055 7.035
+000063d0: 342c 3338 2e38 3433 3933 3920 302e 3335  4,38.843939 0.35
+000063e0: 3037 392c 362e 3739 3637 3439 202d 322e  079,6.796749 -2.
+000063f0: 3830 3937 312c 372e 3538 3734 3039 202d  80971,7.587409 -
+00006400: 342e 3138 3732 352c 372e 3732 3834 3439  4.18725,7.728449
+00006410: 202d 342e 3138 3539 342c 302e 3432 3836   -4.18594,0.4286
+00006420: 202d 342e 3937 3433 352c 2d33 2e37 3633   -4.97435,-3.763
+00006430: 3538 3520 2d31 2e37 3734 3535 2c2d 382e  585 -1.77455,-8.
+00006440: 3533 3030 3833 2034 2e33 3835 352c 2d36  530083 4.3855,-6
+00006450: 2e35 3332 3737 3120 3230 2e32 3035 332c  .532771 20.2053,
+00006460: 2d32 352e 3333 3831 3236 2033 352e 3831  -25.338126 35.81
+00006470: 3437 312c 2d32 382e 3337 3135 3038 2033  471,-28.371508 3
+00006480: 2e32 3234 3239 2c2d 302e 3439 3534 3536  .22429,-0.495456
+00006490: 2035 2e35 3230 3634 2c2d 302e 3838 3930   5.52064,-0.8890
+000064a0: 3732 2036 2e32 3536 3331 2c32 2e32 3839  72 6.25631,2.289
+000064b0: 3038 3220 302e 3831 3133 352c 332e 3530  082 0.81135,3.50
+000064c0: 3537 3739 202d 302e 3939 3830 332c 342e  5779 -0.99803,4.
+000064d0: 3533 3932 3137 202d 342e 3536 3033 382c  539217 -4.56038,
+000064e0: 352e 3034 3737 3336 202d 3134 2e35 3137  5.047736 -14.517
+000064f0: 3032 2c32 2e30 3732 3238 202d 3339 2e32  02,2.07228 -39.2
+00006500: 3434 3037 2c2d 362e 3737 3339 3537 202d  4407,-6.773957 -
+00006510: 3433 2e39 3937 3231 2c2d 3133 2e38 3138  43.99721,-13.818
+00006520: 3434 3520 2d32 2e36 3436 3932 2c2d 332e  445 -2.64692,-3.
+00006530: 3932 3239 3139 202d 322e 3239 3939 382c  922919 -2.29998,
+00006540: 2d36 2e33 3633 3438 3620 2d30 2e38 3138  -6.363486 -0.818
+00006550: 3636 2c2d 372e 3437 3338 3533 2031 2e32  66,-7.473853 1.2
+00006560: 3631 3334 2c2d 302e 3934 3534 3820 342e  6134,-0.94548 4.
+00006570: 3138 3433 392c 2d31 2e30 3137 3934 3620  18439,-1.017946 
+00006580: 362e 3233 3136 332c 342e 3238 3436 3833  6.23163,4.284683
+00006590: 207a 220a 2020 2020 2020 2073 6f64 6970   z".       sodip
+000065a0: 6f64 693a 6e6f 6465 7479 7065 733d 2273  odi:nodetypes="s
+000065b0: 7363 7373 7373 7373 7373 7373 7363 7373  scssssssssssscss
+000065c0: 7373 7322 202f 3e0a 2020 2020 3c70 6174  sss" />.    <pat
+000065d0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+000065e0: 6669 6c6c 3a6e 6f6e 653b 6669 6c6c 2d6f  fill:none;fill-o
+000065f0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00006600: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00006610: 6964 7468 3a34 3b73 7472 6f6b 652d 6c69  idth:4;stroke-li
+00006620: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00006630: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00006640: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00006650: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00006660: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00006670: 643d 226d 202d 3931 2e35 3532 3437 332c  d="m -91.552473,
+00006680: 3139 362e 3836 3332 3920 3231 2e38 3736  196.86329 21.876
+00006690: 3232 2c2d 3234 2e35 3637 3420 6320 312e  22,-24.5674 c 1.
+000066a0: 3838 3535 322c 2d32 2e33 3230 3031 2031  88552,-2.32001 1
+000066b0: 302e 3334 3230 332c 2d33 2e34 3331 3133  0.34203,-3.43113
+000066c0: 2031 332e 3332 3632 322c 2d33 2e32 3531   13.32622,-3.251
+000066d0: 3537 2032 312e 3538 3331 332c 302e 3031  57 21.58313,0.01
+000066e0: 3634 2033 352e 3235 3031 312c 302e 3130  64 35.25011,0.10
+000066f0: 3039 3520 3536 2e36 3831 3338 3937 372c  095 56.68138977,
+00006700: 332e 3435 3720 332e 3437 3332 3530 3033  3.457 3.47325003
+00006710: 2c30 2e35 3433 3920 352e 3237 3337 3530  ,0.5439 5.273750
+00006720: 3033 2c32 2e33 3331 3032 2036 2e38 3839  03,2.33102 6.889
+00006730: 3431 3030 332c 352e 3331 3530 3720 342e  41003,5.31507 4.
+00006740: 3737 3734 3130 322c 382e 3832 3336 3320  7774102,8.82363 
+00006750: 352e 3035 3538 3230 322c 3137 2e34 3832  5.0558202,17.482
+00006760: 3334 202d 312e 3035 3639 2c32 372e 3237  34 -1.0569,27.27
+00006770: 3738 3320 2d31 2e34 3031 3836 2c32 2e32  783 -1.40186,2.2
+00006780: 3436 3434 202d 342e 3139 3238 362c 342e  4644 -4.19286,4.
+00006790: 3830 3834 3320 2d36 2e38 3334 3931 3030  80843 -6.8349100
+000067a0: 332c 342e 3938 3533 3420 2d31 312e 3332  3,4.98534 -11.32
+000067b0: 3432 3139 3737 2c30 2e37 3538 3237 202d  421977,0.75827 -
+000067c0: 3236 2e33 3434 3134 3937 372c 2d30 2e36  26.34414977,-0.6
+000067d0: 3236 3720 2d33 312e 3939 3337 3839 3737  267 -31.99378977
+000067e0: 2c2d 302e 3838 3739 3820 2d33 2e36 3332  ,-0.88798 -3.632
+000067f0: 3934 2c2d 302e 3136 3830 3120 2d36 2e38  94,-0.16801 -6.8
+00006800: 3338 3232 2c33 2e34 3436 3631 202d 372e  3822,3.44661 -7.
+00006810: 3930 3238 382c 362e 3136 3536 3920 2d32  90288,6.16569 -2
+00006820: 2e39 3833 3134 2c37 2e36 3138 3736 202d  .98314,7.61876 -
+00006830: 362e 3839 3737 342c 3130 2e35 3331 3733  6.89774,10.53173
+00006840: 202d 3132 2e31 3632 3539 2c31 352e 3232   -12.16259,15.22
+00006850: 3332 220a 2020 2020 2020 2069 643d 2270  32".       id="p
+00006860: 6174 6831 2d39 220a 2020 2020 2020 2073  ath1-9".       s
+00006870: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00006880: 733d 2263 6363 7373 7373 7373 6322 202f  s="cccssssssc" /
+00006890: 3e0a 2020 2020 3c67 0a20 2020 2020 2020  >.    <g.       
+000068a0: 6964 3d22 6732 3022 0a20 2020 2020 2020  id="g20".       
+000068b0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+000068c0: 6c61 7465 282d 3630 2e36 3136 3234 372c  late(-60.616247,
+000068d0: 3234 2e38 3238 3236 3729 223e 0a20 2020  24.828267)">.   
+000068e0: 2020 203c 670a 2020 2020 2020 2020 2069     <g.         i
+000068f0: 643d 2267 3139 223e 0a20 2020 2020 2020  d="g19">.       
+00006900: 203c 670a 2020 2020 2020 2020 2020 2069   <g.           i
+00006910: 643d 2267 3434 220a 2020 2020 2020 2020  d="g44".        
+00006920: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
+00006930: 7472 6978 2830 2e37 3132 3533 3530 392c  trix(0.71253509,
+00006940: 2d30 2e33 3137 3137 3139 342c 302e 3331  -0.31717194,0.31
+00006950: 3731 3731 3934 2c30 2e37 3132 3533 3530  717194,0.7125350
+00006960: 392c 3234 2e38 3230 3238 2c35 392e 3435  9,24.82028,59.45
+00006970: 3634 3734 2922 3e0a 2020 2020 2020 2020  6474)">.        
+00006980: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00006990: 2020 2020 2073 7479 6c65 3d22 6f70 6163       style="opac
+000069a0: 6974 793a 302e 3939 3b66 696c 6c3a 2366  ity:0.99;fill:#f
+000069b0: 3066 3336 663b 6669 6c6c 2d6f 7061 6369  0f36f;fill-opaci
+000069c0: 7479 3a31 3b73 7472 6f6b 653a 6e6f 6e65  ty:1;stroke:none
+000069d0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+000069e0: 3134 3835 3532 3b73 7472 6f6b 652d 6c69  148552;stroke-li
+000069f0: 6e65 6361 703a 726f 756e 643b 7374 726f  necap:round;stro
+00006a00: 6b65 2d6d 6974 6572 6c69 6d69 743a 332e  ke-miterlimit:3.
+00006a10: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00006a20: 6179 3a6e 6f6e 6522 0a20 2020 2020 2020  ay:none".       
+00006a30: 2020 2020 2020 643d 226d 2031 3334 2e37        d="m 134.7
+00006a40: 3833 3132 2c31 392e 3535 3633 3437 2076  8312,19.556347 v
+00006a50: 202d 302e 3634 3630 3835 2063 2031 362e   -0.646085 c 16.
+00006a60: 3936 3936 332c 2d30 2e30 3330 3920 3639  96963,-0.0309 69
+00006a70: 2e37 3830 3938 2c2d 302e 3036 3632 3620  .78098,-0.06626 
+00006a80: 3836 2e37 3530 3634 2c2d 302e 3036 3339  86.75064,-0.0639
+00006a90: 3120 6c20 332e 3234 3236 312c 342e 3565  1 l 3.24261,4.5e
+00006aa0: 2d34 2030 2e35 3734 3034 2c30 2e33 3238  -4 0.57404,0.328
+00006ab0: 3939 2063 2030 2e33 3135 3732 2c30 2e31  99 c 0.31572,0.1
+00006ac0: 3830 3934 3420 302e 3537 3433 392c 302e  80944 0.57439,0.
+00006ad0: 3334 3034 3835 2030 2e35 3734 3832 2c30  340485 0.57482,0
+00006ae0: 2e33 3534 3533 3220 302e 3030 312c 302e  .354532 0.001,0.
+00006af0: 3033 3635 3320 2d30 2e30 3534 332c 302e  03653 -0.0543,0.
+00006b00: 3133 3935 3036 202d 302e 3132 3031 312c  139506 -0.12011,
+00006b10: 302e 3232 3333 3036 202d 302e 3137 3733  0.223306 -0.1773
+00006b20: 2c30 2e32 3235 3635 202d 302e 3632 3234  ,0.22565 -0.6224
+00006b30: 342c 302e 3338 3030 3520 2d31 2e32 3334  4,0.38005 -1.234
+00006b40: 3132 2c30 2e34 3238 3035 3920 2d31 392e  12,0.428059 -19.
+00006b50: 3539 3338 372c 302e 3033 3536 3420 2d37  59387,0.03564 -7
+00006b60: 302e 3139 3339 332c 302e 3032 3037 3520  0.19393,0.02075 
+00006b70: 2d38 392e 3738 3738 382c 302e 3032 3037  -89.78788,0.0207
+00006b80: 3520 7a22 0a20 2020 2020 2020 2020 2020  5 z".           
+00006b90: 2020 6964 3d22 7061 7468 3135 220a 2020    id="path15".  
+00006ba0: 2020 2020 2020 2020 2020 2073 6f64 6970             sodip
+00006bb0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+00006bc0: 6373 6373 6373 7363 6322 202f 3e0a 2020  cscscsscc" />.  
+00006bd0: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
+00006be0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00006bf0: 3d22 6f70 6163 6974 793a 302e 3939 3b66  ="opacity:0.99;f
+00006c00: 696c 6c3a 2366 3364 6536 663b 6669 6c6c  ill:#f3de6f;fill
+00006c10: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00006c20: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
+00006c30: 6474 683a 302e 3134 3835 3532 3b73 7472  dth:0.148552;str
+00006c40: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00006c50: 643b 7374 726f 6b65 2d6d 6974 6572 6c69  d;stroke-miterli
+00006c60: 6d69 743a 332e 343b 7374 726f 6b65 2d64  mit:3.4;stroke-d
+00006c70: 6173 6861 7272 6179 3a6e 6f6e 6522 0a20  asharray:none". 
+00006c80: 2020 2020 2020 2020 2020 2020 643d 226d              d="m
+00006c90: 2031 3335 2e30 3232 3431 2c32 322e 3531   135.02241,22.51
+00006ca0: 3135 3632 2030 2e30 3933 352c 2d32 2e31  1562 0.0935,-2.1
+00006cb0: 3737 3833 3820 6320 3139 2e34 3737 3431  77838 c 19.47741
+00006cc0: 2c30 2e31 3835 3836 3920 3639 2e38 3732  ,0.185869 69.872
+00006cd0: 3532 2c2d 302e 3037 3138 3720 3839 2e33  52,-0.07187 89.3
+00006ce0: 3439 3334 2c30 2e30 3832 3620 312e 3034  4934,0.0826 1.04
+00006cf0: 3330 362c 302e 3132 3738 3234 2031 2e37  306,0.127824 1.7
+00006d00: 3533 3739 2c31 2e31 3832 3037 3920 312e  5379,1.182079 1.
+00006d10: 3738 3538 2c32 2e30 3335 3136 3420 302e  7858,2.035164 0.
+00006d20: 3031 3639 2c30 2e34 3531 3137 3620 2d30  0169,0.451176 -0
+00006d30: 2e33 3035 3835 2c32 2e30 3535 3033 3620  .30585,2.055036 
+00006d40: 2d31 2e39 3730 3137 2c32 2e31 3735 3035  -1.97017,2.17505
+00006d50: 3920 2d31 392e 3431 3732 362c 2d30 2e31  9 -19.41726,-0.1
+00006d60: 3133 3538 3420 2d36 392e 3834 3039 372c  13584 -69.84097,
+00006d70: 2d30 2e30 3831 3120 2d38 392e 3235 3834  -0.0811 -89.2584
+00006d80: 372c 2d30 2e30 3830 3939 207a 220a 2020  7,-0.08099 z".  
+00006d90: 2020 2020 2020 2020 2020 2069 643d 2270             id="p
+00006da0: 6174 6831 3622 0a20 2020 2020 2020 2020  ath16".         
+00006db0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00006dc0: 6574 7970 6573 3d22 6363 7373 7363 6322  etypes="ccssscc"
+00006dd0: 202f 3e0a 2020 2020 2020 2020 2020 3c70   />.          <p
+00006de0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00006df0: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
+00006e00: 302e 3939 3b66 696c 6c3a 2362 6461 3833  0.99;fill:#bda83
+00006e10: 373b 6669 6c6c 2d6f 7061 6369 7479 3a31  7;fill-opacity:1
+00006e20: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
+00006e30: 6f6b 652d 7769 6474 683a 302e 3134 3835  oke-width:0.1485
+00006e40: 3532 3b73 7472 6f6b 652d 6c69 6e65 6361  52;stroke-lineca
+00006e50: 703a 726f 756e 643b 7374 726f 6b65 2d6d  p:round;stroke-m
+00006e60: 6974 6572 6c69 6d69 743a 332e 343b 7374  iterlimit:3.4;st
+00006e70: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00006e80: 6f6e 6522 0a20 2020 2020 2020 2020 2020  one".           
+00006e90: 2020 643d 226d 2031 3335 2e30 3232 3535    d="m 135.02255
+00006ea0: 2c32 362e 3338 3334 3831 2076 202d 312e  ,26.383481 v -1.
+00006eb0: 3536 3237 3839 2063 2031 392e 3530 322c  562789 c 19.502,
+00006ec0: 302e 3139 3739 3120 3730 2e30 3137 3833  0.19791 70.01783
+00006ed0: 2c2d 302e 3235 3033 3137 2038 392e 3531  ,-0.250317 89.51
+00006ee0: 3839 322c 2d30 2e30 3236 3134 2030 2e34  892,-0.02614 0.4
+00006ef0: 3639 3736 2c30 2e30 3730 3831 2030 2e39  6976,0.07081 0.9
+00006f00: 3032 3039 2c30 2e32 3839 3231 3820 312e  0209,0.289218 1.
+00006f10: 3139 3038 362c 302e 3630 3030 3035 2030  19086,0.600005 0
+00006f20: 2e33 3935 2c30 2e34 3233 3831 3120 302e  .395,0.423811 0.
+00006f30: 3432 3538 332c 312e 3030 3236 3235 2030  42583,1.002625 0
+00006f40: 2e33 3934 3738 2c31 2e35 3238 3232 3720  .39478,1.528227 
+00006f50: 2d30 2e30 3032 2c30 2e30 3330 3638 202d  -0.002,0.03068 -
+00006f60: 302e 3237 3930 362c 302e 3231 3537 3139  0.27906,0.215719
+00006f70: 202d 302e 3837 3730 392c 302e 3535 3531   -0.87709,0.5551
+00006f80: 3220 6c20 2d30 2e38 3632 3238 2c30 2e34  2 l -0.86228,0.4
+00006f90: 3839 3337 2063 202d 3139 2e34 3533 3037  8937 c -19.45307
+00006fa0: 2c2d 302e 3038 3037 3820 2d36 392e 3931  ,-0.08078 -69.91
+00006fb0: 3230 382c 2d30 2e30 3438 3536 202d 3839  208,-0.04856 -89
+00006fc0: 2e33 3635 322c 2d30 2e30 3231 3031 207a  .3652,-0.02101 z
+00006fd0: 220a 2020 2020 2020 2020 2020 2020 2069  ".             i
+00006fe0: 643d 2270 6174 6831 3722 0a20 2020 2020  d="path17".     
+00006ff0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+00007000: 3a6e 6f64 6574 7970 6573 3d22 6363 7373  :nodetypes="ccss
+00007010: 7373 6363 6322 202f 3e0a 2020 2020 2020  ssccc" />.      
+00007020: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00007030: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00007040: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
+00007050: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
+00007060: 6474 683a 323b 7374 726f 6b65 2d6c 696e  dth:2;stroke-lin
+00007070: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00007080: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00007090: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000070a0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+000070b0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+000070c0: 2020 2020 2064 3d22 6d20 3133 302e 3538       d="m 130.58
+000070d0: 3533 352c 3137 2e39 3034 3233 3120 3934  535,17.904231 94
+000070e0: 2e34 3439 3238 2c2d 302e 3037 3437 2039  .44928,-0.0747 9
+000070f0: 2e34 3035 2c35 2e34 3239 3938 3320 2d39  .405,5.429983 -9
+00007100: 2e37 3936 3731 2c35 2e36 3536 3133 3720  .79671,5.656137 
+00007110: 2d39 342e 3132 3633 342c 302e 3033 3538  -94.12634,0.0358
+00007120: 3920 6320 2d37 2e36 3037 3639 2c30 202d  9 c -7.60769,0 -
+00007130: 372e 3438 3839 362c 2d31 312e 3034 3733  7.48896,-11.0473
+00007140: 3035 2030 2e30 3638 382c 2d31 312e 3034  05 0.0688,-11.04
+00007150: 3733 3035 207a 220a 2020 2020 2020 2020  7305 z".        
+00007160: 2020 2020 2069 643d 2270 6174 6831 3022       id="path10"
+00007170: 0a20 2020 2020 2020 2020 2020 2020 736f  .             so
+00007180: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00007190: 3d22 6363 6363 6363 6322 202f 3e0a 2020  ="ccccccc" />.  
+000071a0: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
+000071b0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+000071c0: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+000071d0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+000071e0: 652d 7769 6474 683a 323b 7374 726f 6b65  e-width:2;stroke
+000071f0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00007200: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00007210: 7465 723b 7374 726f 6b65 2d64 6173 6861  ter;stroke-dasha
+00007220: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00007230: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00007240: 2020 2020 2020 2020 2064 3d22 4d20 3133           d="M 13
+00007250: 342e 3433 3631 2c31 382e 3331 3736 3820  4.4361,18.31768 
+00007260: 5620 3238 2e34 3738 3733 3522 0a20 2020  V 28.478735".   
+00007270: 2020 2020 2020 2020 2020 6964 3d22 7061            id="pa
+00007280: 7468 3131 220a 2020 2020 2020 2020 2020  th11".          
+00007290: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+000072a0: 7479 7065 733d 2263 6322 202f 3e0a 2020  types="cc" />.  
+000072b0: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
+000072c0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+000072d0: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+000072e0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+000072f0: 652d 7769 6474 683a 302e 3236 3435 3833  e-width:0.264583
+00007300: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
+00007310: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00007320: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00007330: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00007340: 2020 2020 2020 2020 2020 2020 643d 226d              d="m
+00007350: 2032 3235 2e38 3931 372c 3138 2e30 3630   225.8917,18.060
+00007360: 3638 3320 6320 302c 302e 3539 3934 3332  683 c 0,0.599432
+00007370: 2031 2e31 3436 3338 2c32 2e32 3738 3730   1.14638,2.27870
+00007380: 3920 2d31 2e37 3436 3839 2c32 2e32 3738  9 -1.74689,2.278
+00007390: 3730 3920 322e 3832 3238 372c 302e 3035  709 2.82287,0.05
+000073a0: 3439 3620 322e 3930 3639 2c34 2e33 3337  496 2.9069,4.337
+000073b0: 3335 202d 302e 3032 3232 2c34 2e33 3337  35 -0.0222,4.337
+000073c0: 3335 2032 2e39 3139 3135 2c30 2032 2e37  35 2.91915,0 2.7
+000073d0: 3534 3333 2c33 2e38 3832 3135 3320 302e  5433,3.882153 0.
+000073e0: 3035 3633 2c33 2e38 3832 3135 3322 0a20  0563,3.882153". 
+000073f0: 2020 2020 2020 2020 2020 2020 6964 3d22              id="
+00007400: 7061 7468 3132 220a 2020 2020 2020 2020  path12".        
+00007410: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00007420: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
+00007430: 3e0a 2020 2020 2020 2020 2020 3c70 6174  >.          <pat
+00007440: 680a 2020 2020 2020 2020 2020 2020 2073  h.             s
+00007450: 7479 6c65 3d22 6669 6c6c 3a6e 6f6e 653b  tyle="fill:none;
+00007460: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00007470: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+00007480: 3435 3833 7078 3b73 7472 6f6b 652d 6c69  4583px;stroke-li
+00007490: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+000074a0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+000074b0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+000074c0: 3122 0a20 2020 2020 2020 2020 2020 2020  1".             
+000074d0: 643d 224d 2032 3234 2e31 3738 3939 2c32  d="M 224.17899,2
+000074e0: 342e 3637 3933 3539 2048 2031 3335 2e30  4.679359 H 135.0
+000074f0: 3932 220a 2020 2020 2020 2020 2020 2020  92".            
+00007500: 2069 643d 2270 6174 6831 3322 0a20 2020   id="path13".   
+00007510: 2020 2020 2020 2020 2020 736f 6469 706f            sodipo
+00007520: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00007530: 2220 2f3e 0a20 2020 2020 2020 2020 203c  " />.          <
+00007540: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00007550: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
+00007560: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
+00007570: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
+00007580: 2e32 3634 3538 3370 783b 7374 726f 6b65  .264583px;stroke
+00007590: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+000075a0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+000075b0: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+000075c0: 7479 3a31 220a 2020 2020 2020 2020 2020  ty:1".          
+000075d0: 2020 2064 3d22 4d20 3232 342e 3135 3137     d="M 224.1517
+000075e0: 372c 3230 2e33 3338 3434 3920 4820 3133  7,20.338449 H 13
+000075f0: 352e 3036 3437 3822 0a20 2020 2020 2020  5.06478".       
+00007600: 2020 2020 2020 6964 3d22 7061 7468 3133        id="path13
+00007610: 2d33 220a 2020 2020 2020 2020 2020 2020  -3".            
+00007620: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00007630: 7065 733d 2263 6322 202f 3e0a 2020 2020  pes="cc" />.    
+00007640: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00007650: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00007660: 6f70 6163 6974 793a 302e 3939 3b66 696c  opacity:0.99;fil
+00007670: 6c3a 2366 3336 6535 363b 6669 6c6c 2d6f  l:#f36e56;fill-o
+00007680: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00007690: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+000076a0: 6964 7468 3a30 2e32 3937 3130 333b 7374  idth:0.297103;st
+000076b0: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
+000076c0: 6e64 3b73 7472 6f6b 652d 6d69 7465 726c  nd;stroke-miterl
+000076d0: 696d 6974 3a33 2e34 3b73 7472 6f6b 652d  imit:3.4;stroke-
+000076e0: 6461 7368 6172 7261 793a 6e6f 6e65 220a  dasharray:none".
+000076f0: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+00007700: 6d20 3133 302e 3037 3737 322c 3237 2e39  m 130.07772,27.9
+00007710: 3139 3335 3220 6320 2d30 2e36 3937 3131  19352 c -0.69711
+00007720: 2c2d 302e 3036 3831 3920 2d31 2e31 3832  ,-0.06819 -1.182
+00007730: 3534 2c2d 302e 3138 3333 3238 202d 312e  54,-0.183328 -1.
+00007740: 3638 3335 362c 2d30 2e33 3939 3333 3120  68356,-0.399331 
+00007750: 2d31 2e32 3635 3531 2c2d 302e 3534 3535  -1.26551,-0.5455
+00007760: 3932 202d 322e 3134 3331 332c 2d31 2e36  92 -2.14313,-1.6
+00007770: 3830 3035 3420 2d32 2e34 3239 3532 2c2d  80054 -2.42952,-
+00007780: 332e 3134 3035 3235 202d 302e 3130 3038  3.140525 -0.1008
+00007790: 2c2d 302e 3531 3430 3433 202d 302e 3039  ,-0.514043 -0.09
+000077a0: 3133 2c2d 312e 3336 3639 3335 2030 2e30  13,-1.366935 0.0
+000077b0: 3231 312c 2d31 2e38 3934 3830 3420 302e  211,-1.894804 0.
+000077c0: 3334 3831 362c 2d31 2e36 3334 3831 3420  34816,-1.634814 
+000077d0: 312e 3338 3734 352c 2d32 2e38 3138 3035  1.38745,-2.81805
+000077e0: 3620 322e 3930 3238 392c 2d33 2e33 3034  6 2.90289,-3.304
+000077f0: 3934 3520 302e 3638 3036 332c 2d30 2e32  945 0.68063,-0.2
+00007800: 3138 3637 3820 302e 3933 3136 382c 2d30  18678 0.93168,-0
+00007810: 2e32 3432 3233 3820 322e 3831 3033 362c  .242238 2.81036,
+00007820: 2d30 2e32 3633 3734 3820 6c20 312e 3731  -0.263748 l 1.71
+00007830: 3935 372c 2d30 2e30 3139 3639 2076 2034  957,-0.01969 v 4
+00007840: 2e35 3234 3533 3720 342e 3532 3435 3338  .524537 4.524538
+00007850: 206c 202d 312e 3630 3136 362c 2d30 2e30   l -1.60166,-0.0
+00007860: 3036 3320 6320 2d30 2e38 3830 3931 2c2d  063 c -0.88091,-
+00007870: 302e 3030 3335 202d 312e 3636 3335 352c  0.0035 -1.66355,
+00007880: 2d30 2e30 3132 3336 202d 312e 3733 3932  -0.01236 -1.7392
+00007890: 312c 2d30 2e30 3139 3734 207a 220a 2020  1,-0.01974 z".  
+000078a0: 2020 2020 2020 2020 2020 2069 643d 2270             id="p
+000078b0: 6174 6831 3422 0a20 2020 2020 2020 2020  ath14".         
+000078c0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+000078d0: 6574 7970 6573 3d22 6373 7363 7373 6363  etypes="csscsscc
+000078e0: 6363 6363 2220 2f3e 0a20 2020 2020 2020  cccc" />.       
+000078f0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00007900: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
+00007910: 6369 7479 3a30 2e39 393b 6669 6c6c 3a23  city:0.99;fill:#
+00007920: 6236 6231 3930 3b66 696c 6c2d 6f70 6163  b6b190;fill-opac
+00007930: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
+00007940: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
+00007950: 2e31 3736 3737 373b 7374 726f 6b65 2d6c  .176777;stroke-l
+00007960: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
+00007970: 6f6b 652d 6d69 7465 726c 696d 6974 3a33  oke-miterlimit:3
+00007980: 2e34 3b73 7472 6f6b 652d 6461 7368 6172  .4;stroke-dashar
+00007990: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+000079a0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+000079b0: 2020 2020 2020 2020 643d 226d 2032 3236          d="m 226
+000079c0: 2e34 3032 3332 2c32 362e 3637 3335 3933  .40232,26.673593
+000079d0: 2063 2030 2e30 3137 352c 2d30 2e30 3931   c 0.0175,-0.091
+000079e0: 3731 202d 302e 3033 3931 2c2d 302e 3531  71 -0.0391,-0.51
+000079f0: 3736 3333 202d 302e 3039 3135 2c2d 302e  7633 -0.0915,-0.
+00007a00: 3638 3837 3820 2d30 2e30 3939 392c 2d30  68878 -0.0999,-0
+00007a10: 2e33 3235 3736 3320 2d30 2e32 3833 3831  .325763 -0.28381
+00007a20: 2c2d 302e 3632 3435 3836 202d 302e 3533  ,-0.624586 -0.53
+00007a30: 3230 342c 2d30 2e38 3634 3334 3620 2d30  204,-0.864346 -0
+00007a40: 2e31 3437 3132 2c2d 302e 3134 3230 3939  .14712,-0.142099
+00007a50: 202d 302e 3434 3331 342c 2d30 2e33 3332   -0.44314,-0.332
+00007a60: 3032 3120 2d30 2e36 3132 3334 2c2d 302e  021 -0.61234,-0.
+00007a70: 3339 3238 3635 202d 302e 3036 3239 2c2d  392865 -0.0629,-
+00007a80: 302e 3032 3236 3320 2d30 2e31 3134 342c  0.02263 -0.1144,
+00007a90: 2d30 2e30 3437 3635 202d 302e 3131 3434  -0.04765 -0.1144
+00007aa0: 2c2d 302e 3035 3536 2030 2c2d 302e 3030  ,-0.0556 0,-0.00
+00007ab0: 3820 302e 3035 3533 2c2d 302e 3033 3733  8 0.0553,-0.0373
+00007ac0: 3820 302e 3132 3237 372c 2d30 2e30 3635  8 0.12277,-0.065
+00007ad0: 3338 2030 2e32 3831 3439 2c2d 302e 3131  38 0.28149,-0.11
+00007ae0: 3637 3332 2030 2e36 3335 3939 2c2d 302e  6732 0.63599,-0.
+00007af0: 3430 3439 3839 2030 2e38 3233 3831 2c2d  404989 0.82381,-
+00007b00: 302e 3636 3938 3631 2030 2e34 3439 3136  0.669861 0.44916
+00007b10: 2c2d 302e 3633 3334 3435 2030 2e35 3535  ,-0.633445 0.555
+00007b20: 3632 2c2d 312e 3438 3332 3734 2030 2e32  62,-1.483274 0.2
+00007b30: 3831 3739 2c2d 322e 3234 3934 3035 202d  8179,-2.249405 -
+00007b40: 302e 3138 3539 2c2d 302e 3532 3031 3239  0.1859,-0.520129
+00007b50: 202d 302e 3536 3332 322c 2d30 2e39 3638   -0.56322,-0.968
+00007b60: 3131 3220 2d31 2e30 3231 3734 2c2d 312e  112 -1.02174,-1.
+00007b70: 3231 3330 3938 206c 202d 302e 3133 3836  213098 l -0.1386
+00007b80: 332c 2d30 2e30 3734 3037 2030 2e31 3538  3,-0.07407 0.158
+00007b90: 3933 2c2d 302e 3034 3134 3620 6320 302e  93,-0.04146 c 0.
+00007ba0: 3338 3439 352c 2d30 2e31 3030 3432 3220  38495,-0.100422 
+00007bb0: 302e 3732 3537 342c 2d30 2e33 3331 3330  0.72574,-0.33130
+00007bc0: 3820 302e 3834 3836 392c 2d30 2e35 3734  8 0.84869,-0.574
+00007bd0: 3938 3820 302e 3032 392c 2d30 2e30 3537  988 0.029,-0.057
+00007be0: 3339 2030 2e30 3535 332c 2d30 2e31 3037  39 0.0553,-0.107
+00007bf0: 3430 3720 302e 3035 3835 2c2d 302e 3131  407 0.0585,-0.11
+00007c00: 3131 3432 2030 2e30 3033 2c2d 302e 3030  1142 0.003,-0.00
+00007c10: 3337 2031 2e33 3839 3836 2c30 2e37 3932  37 1.38986,0.792
+00007c20: 3234 3120 332e 3038 3134 322c 312e 3736  241 3.08142,1.76
+00007c30: 3838 3336 2031 2e36 3931 3535 2c30 2e39  8836 1.69155,0.9
+00007c40: 3736 3539 3520 332e 3039 3233 352c 312e  76595 3.09235,1.
+00007c50: 3738 3530 3334 2033 2e31 3132 392c 312e  785034 3.1129,1.
+00007c60: 3739 3635 3331 2030 2e30 3238 322c 302e  796531 0.0282,0.
+00007c70: 3031 3538 3120 2d30 2e36 3932 3635 2c30  01581 -0.69265,0
+00007c80: 2e34 3432 3434 3920 2d32 2e39 3538 3239  .442449 -2.95829
+00007c90: 2c31 2e37 3530 3737 202d 312e 3634 3736  ,1.75077 -1.6476
+00007ca0: 2c30 2e39 3531 3432 3620 2d33 2e30 3033  ,0.951426 -3.003
+00007cb0: 362c 312e 3733 3239 3134 202d 332e 3031  6,1.732914 -3.01
+00007cc0: 3333 332c 312e 3733 3636 3339 202d 302e  333,1.736639 -0.
+00007cd0: 3031 2c30 2e30 3033 3720 2d30 2e30 3132  01,0.0037 -0.012
+00007ce0: 372c 2d30 2e30 3139 3538 202d 302e 3030  7,-0.01958 -0.00
+00007cf0: 372c 2d30 2e30 3531 3738 207a 220a 2020  7,-0.05178 z".  
+00007d00: 2020 2020 2020 2020 2020 2069 643d 2270             id="p
+00007d10: 6174 6831 3822 0a20 2020 2020 2020 2020  ath18".         
+00007d20: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00007d30: 6574 7970 6573 3d22 6363 7373 7363 7373  etypes="ccssscss
+00007d40: 7363 7373 6373 7373 6363 6322 202f 3e0a  scsscsssccc" />.
+00007d50: 2020 2020 2020 2020 3c2f 673e 0a20 2020          </g>.   
+00007d60: 2020 203c 2f67 3e0a 2020 2020 2020 3c70     </g>.      <p
+00007d70: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+00007d80: 6c65 3d22 6669 6c6c 3a23 3030 3030 3030  le="fill:#000000
+00007d90: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00007da0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+00007db0: 6b65 2d77 6964 7468 3a30 2e31 3533 3035  ke-width:0.15305
+00007dc0: 3170 783b 7374 726f 6b65 2d6c 696e 6563  1px;stroke-linec
+00007dd0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00007de0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00007df0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00007e00: 2020 2020 2020 2020 2064 3d22 6d20 3139           d="m 19
+00007e10: 382e 3332 3735 382c 322e 3038 3735 3932  8.32758,2.087592
+00007e20: 3920 2d33 2e31 3837 3932 2c2d 302e 3333  9 -3.18792,-0.33
+00007e30: 3537 3637 2031 2e31 3132 3133 2c32 2e38  5767 1.11213,2.8
+00007e40: 3635 3939 3520 7a22 0a20 2020 2020 2020  65995 z".       
+00007e50: 2020 6964 3d22 7061 7468 3139 2220 2f3e    id="path19" />
+00007e60: 0a20 2020 203c 2f67 3e0a 2020 2020 3c70  .    </g>.    <p
+00007e70: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00007e80: 3d22 6669 6c6c 3a23 6464 3162 3163 3b66  ="fill:#dd1b1c;f
+00007e90: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00007ea0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
+00007eb0: 2d77 6964 7468 3a30 2e32 3634 3538 3370  -width:0.264583p
+00007ec0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
+00007ed0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00007ee0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00007ef0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00007f00: 2020 2020 2064 3d22 6d20 3631 2e34 3039       d="m 61.409
+00007f10: 3239 312c 3630 2e39 3433 3438 3620 6320  291,60.943486 c 
+00007f20: 322e 3336 3631 3739 2c31 2e37 3236 3038  2.366179,1.72608
+00007f30: 3120 342e 3637 3231 3837 2c2d 302e 3034  1 4.672187,-0.04
+00007f40: 3530 3220 352e 3936 3135 3431 2c2d 302e  502 5.961541,-0.
+00007f50: 3438 3439 3032 206c 2030 2e36 3034 3831  484902 l 0.60481
+00007f60: 332c 312e 3337 3037 3832 202d 322e 3530  3,1.370782 -2.50
+00007f70: 3131 3633 2c31 2e31 3030 3733 3820 6320  1163,1.100738 c 
+00007f80: 2d32 2e31 3933 3132 312c 302e 3639 3531  -2.193121,0.6951
+00007f90: 3134 202d 332e 3434 3636 3838 2c2d 302e  14 -3.446688,-0.
+00007fa0: 3537 3739 3631 202d 342e 3036 3531 3931  577961 -4.065191
+00007fb0: 2c2d 312e 3938 3636 3138 207a 220a 2020  ,-1.986618 z".  
+00007fc0: 2020 2020 2069 643d 2270 6174 6832 3222       id="path22"
+00007fd0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00007fe0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00007ff0: 6322 202f 3e0a 2020 2020 3c70 6174 680a  c" />.    <path.
+00008000: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00008010: 6c6c 3a23 6530 3963 3138 3b66 696c 6c2d  ll:#e09c18;fill-
+00008020: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00008030: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+00008040: 7468 3a30 2e32 3634 3538 3370 783b 7374  th:0.264583px;st
+00008050: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00008060: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00008070: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00008080: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00008090: 2064 3d22 6d20 3936 2e35 3032 3633 392c   d="m 96.502639,
+000080a0: 3537 2e35 3730 3334 3820 6320 2d33 2e39  57.570348 c -3.9
+000080b0: 3236 3636 322c 2d30 2e35 3935 3538 3620  26662,-0.595586 
+000080c0: 2d37 2e38 3933 3733 372c 2d34 2e35 3237  -7.893737,-4.527
+000080d0: 3133 3220 2d38 2e33 3831 3033 342c 2d38  132 -8.381034,-8
+000080e0: 2e34 3638 3639 3820 2d30 2e33 3837 3735  .468698 -0.38775
+000080f0: 352c 2d33 2e31 3336 3430 3220 312e 3839  5,-3.136402 1.89
+00008100: 3835 3139 2c2d 362e 3937 3231 3434 2034  8519,-6.972144 4
+00008110: 2e38 3237 3035 362c 2d38 2e31 3630 3031  .827056,-8.16001
+00008120: 3520 342e 3137 3231 3235 2c2d 312e 3639  5 4.172125,-1.69
+00008130: 3232 3934 2031 302e 3036 3335 3539 2c30  2294 10.063559,0
+00008140: 2e31 3634 3633 3920 3133 2e30 3332 3033  .164639 13.03203
+00008150: 392c 332e 3534 3936 3938 2031 2e36 3630  9,3.549698 1.660
+00008160: 3634 2c31 2e38 3933 3639 3120 322e 3136  64,1.893691 2.16
+00008170: 3435 382c 352e 3234 3533 3432 2031 2e30  458,5.245342 1.0
+00008180: 3136 3836 2c37 2e34 3837 3334 202d 312e  1686,7.48734 -1.
+00008190: 3830 3632 352c 332e 3532 3834 3132 202d  80625,3.528412 -
+000081a0: 362e 3537 3538 382c 362e 3138 3631 3036  6.57588,6.186106
+000081b0: 202d 3130 2e34 3934 3932 312c 352e 3539   -10.494921,5.59
+000081c0: 3136 3735 207a 220a 2020 2020 2020 2069  1675 z".       i
+000081d0: 643d 2270 6174 6834 3422 0a20 2020 2020  d="path44".     
+000081e0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000081f0: 7970 6573 3d22 7373 7373 7373 2220 2f3e  ypes="ssssss" />
+00008200: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00008210: 2020 7374 796c 653d 2266 696c 6c3a 2337    style="fill:#7
+00008220: 3834 3432 313b 7374 726f 6b65 3a6e 6f6e  84421;stroke:non
+00008230: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
+00008240: 2e32 3634 3538 3370 783b 7374 726f 6b65  .264583px;stroke
+00008250: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00008260: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00008270: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00008280: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00008290: 6d20 3130 352e 3836 3532 342c 3531 2e34  m 105.86524,51.4
+000082a0: 3034 3034 3620 6320 2d33 2e32 3434 3137  04046 c -3.24417
+000082b0: 2c2d 342e 3538 3037 3820 2d35 2e33 3132  ,-4.58078 -5.312
+000082c0: 3531 2c2d 352e 3038 3233 3539 202d 392e  51,-5.082359 -9.
+000082d0: 3135 3237 3636 2c2d 332e 3132 3235 3635  152766,-3.122565
+000082e0: 202d 352e 3132 3732 3534 2c32 2e36 3136   -5.127254,2.616
+000082f0: 3538 3620 2d33 2e32 3836 3530 332c 342e  586 -3.286503,4.
+00008300: 3933 3939 3633 202d 312e 3630 3233 3233  939963 -1.602323
+00008310: 2c38 2e36 3736 3431 3320 2d35 2e32 3433  ,8.676413 -5.243
+00008320: 3637 312c 2d32 2e37 3539 3232 3220 2d39  671,-2.759222 -9
+00008330: 2e36 3035 3035 392c 2d31 312e 3332 3537  .605059,-11.3257
+00008340: 3136 202d 332e 3934 3032 3632 2c2d 3134  16 -3.940262,-14
+00008350: 2e37 3834 3630 3620 382e 3430 3639 3734  .784606 8.406974
+00008360: 2c2d 352e 3133 3332 3436 2031 342e 3333  ,-5.133246 14.33
+00008370: 3338 3031 2c33 2e34 3837 3832 3520 3134  3801,3.487825 14
+00008380: 2e36 3935 3335 312c 392e 3233 3037 3538  .695351,9.230758
+00008390: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+000083a0: 6174 6832 302d 3322 0a20 2020 2020 2020  ath20-3".       
+000083b0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+000083c0: 6573 3d22 6373 6373 6322 202f 3e0a 2020  es="cscsc" />.  
+000083d0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+000083e0: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
+000083f0: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+00008400: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+00008410: 726f 6b65 2d77 6964 7468 3a30 2e32 3737  roke-width:0.277
+00008420: 3430 3970 783b 7374 726f 6b65 2d6c 696e  409px;stroke-lin
+00008430: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00008440: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00008450: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00008460: 220a 2020 2020 2020 2064 3d22 6d20 3836  ".       d="m 86
+00008470: 2e30 3138 3033 352c 3438 2e31 3232 3432  .018035,48.12242
+00008480: 3720 6320 2d30 2e31 3332 3231 352c 2d34  7 c -0.132215,-4
+00008490: 2e30 3532 3934 3820 322e 3832 3134 3233  .052948 2.821423
+000084a0: 2c2d 372e 3537 3837 3438 2036 2e35 3436  ,-7.578748 6.546
+000084b0: 3539 372c 2d38 2e39 3430 3734 3920 312e  597,-8.940749 1.
+000084c0: 3937 3130 3632 2c2d 302e 3732 3036 3631  971062,-0.720661
+000084d0: 2031 312e 3032 3938 3338 2c2d 302e 3535   11.029838,-0.55
+000084e0: 3339 3120 3133 2e36 3830 3436 382c 332e  391 13.680468,3.
+000084f0: 3832 3533 3135 2031 2e32 3836 3833 2c32  825315 1.28683,2
+00008500: 2e31 3236 3032 3620 322e 3233 3633 392c  .126026 2.23639,
+00008510: 362e 3139 3831 3935 202d 302e 3531 3233  6.198195 -0.5123
+00008520: 322c 392e 3138 3839 3837 202d 302e 3532  2,9.188987 -0.52
+00008530: 3035 2c2d 342e 3733 3332 3537 202d 322e  05,-4.733257 -2.
+00008540: 3334 3434 322c 2d36 2e39 3439 3033 3820  34442,-6.949038 
+00008550: 2d33 2e31 3336 3838 2c2d 372e 3635 3335  -3.13688,-7.6535
+00008560: 3432 202d 322e 3835 3132 3237 2c2d 322e  42 -2.851227,-2.
+00008570: 3533 3437 3839 202d 382e 3734 3438 3338  534789 -8.744838
+00008580: 2c2d 322e 3737 3430 3635 202d 3131 2e35  ,-2.774065 -11.5
+00008590: 3235 3532 352c 2d30 2e31 3632 3038 3220  25525,-0.162082 
+000085a0: 2d31 2e37 3335 3837 2c31 2e36 3330 3535  -1.73587,1.63055
+000085b0: 3520 2d32 2e33 3632 3938 322c 332e 3933  5 -2.362982,3.93
+000085c0: 3134 3235 202d 302e 3037 3833 382c 362e  1425 -0.07838,6.
+000085d0: 3938 3531 3337 2031 2e32 3233 3630 332c  985137 1.223603,
+000085e0: 312e 3633 3535 3320 322e 3530 3135 3235  1.63553 2.501525
+000085f0: 2c34 2e35 3931 3830 3620 362e 3833 3239  ,4.591806 6.8329
+00008600: 3034 2c36 2e36 3533 3239 3120 2d35 2e36  04,6.653291 -5.6
+00008610: 3236 3934 342c 2d30 2e32 3131 3939 3520  26944,-0.211995 
+00008620: 2d31 312e 3637 3336 3639 2c2d 352e 3831  -11.673669,-5.81
+00008630: 3334 3237 202d 3131 2e38 3036 3836 322c  3427 -11.806862,
+00008640: 2d39 2e38 3936 3335 3720 7a22 0a20 2020  -9.896357 z".   
+00008650: 2020 2020 6964 3d22 7061 7468 3522 0a20      id="path5". 
+00008660: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00008670: 6f64 6574 7970 6573 3d22 7373 7363 7373  odetypes="ssscss
+00008680: 7363 7322 202f 3e0a 2020 2020 3c70 6174  scs" />.    <pat
+00008690: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+000086a0: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
+000086b0: 6c2d 6f70 6163 6974 793a 302e 3939 3437  l-opacity:0.9947
+000086c0: 3533 3b73 7472 6f6b 653a 6e6f 6e65 3b73  53;stroke:none;s
+000086d0: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+000086e0: 3435 3833 7078 3b73 7472 6f6b 652d 6c69  4583px;stroke-li
+000086f0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00008700: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00008710: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00008720: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
+00008730: 342e 3136 3134 3339 2c31 3732 2e36 3639  4.161439,172.669
+00008740: 3131 2063 2030 2e35 3539 3634 322c 2d31  11 c 0.559642,-1
+00008750: 2e39 3532 3333 202d 302e 3830 3634 3231  .95233 -0.806421
+00008760: 2c2d 372e 3331 3536 3920 2d31 2e34 3234  ,-7.31569 -1.424
+00008770: 3434 362c 2d38 2e32 3230 3736 202d 312e  446,-8.22076 -1.
+00008780: 3834 3832 3932 2c32 2e32 3032 3537 202d  848292,2.20257 -
+00008790: 322e 3039 3734 3536 2c32 2e32 3339 3237  2.097456,2.23927
+000087a0: 202d 322e 3837 3436 3936 2c32 2e35 3036   -2.874696,2.506
+000087b0: 3232 2030 2e31 3635 3730 382c 2d30 2e36  22 0.165708,-0.6
+000087c0: 3930 3839 2030 2e37 3731 3731 352c 2d30  9089 0.771715,-0
+000087d0: 2e39 3536 3934 2030 2e30 3230 3431 2c2d  .95694 0.02041,-
+000087e0: 322e 3430 3235 3520 2d30 2e37 3633 3439  2.40255 -0.76349
+000087f0: 322c 322e 3233 3937 3920 2d32 2e34 3937  2,2.23979 -2.497
+00008800: 3434 392c 332e 3630 3233 3220 2d34 2e36  449,3.60232 -4.6
+00008810: 3039 3537 362c 342e 3932 3133 3620 302e  09576,4.92136 0.
+00008820: 3533 3138 3334 2c2d 312e 3630 3032 3220  531834,-1.60022 
+00008830: 312e 3333 3639 3836 2c2d 332e 3236 3437  1.336986,-3.2647
+00008840: 2030 2e37 3037 3737 332c 2d34 2e36 3139   0.707773,-4.619
+00008850: 3234 202d 302e 3536 3835 3137 2c30 2e37  24 -0.568517,0.7
+00008860: 3634 3234 202d 312e 3236 3536 3936 2c31  6424 -1.265696,1
+00008870: 2e30 3831 3139 202d 312e 3938 3239 3536  .08119 -1.982956
+00008880: 2c31 2e33 3238 3334 2031 2e34 3834 3437  ,1.32834 1.48447
+00008890: 2c2d 322e 3730 3436 3420 302e 3532 3338  ,-2.70464 0.5238
+000088a0: 3934 2c2d 332e 3236 3536 3320 302e 3233  94,-3.26563 0.23
+000088b0: 3536 3531 2c2d 342e 3334 3734 3120 2d31  5651,-4.34741 -1
+000088c0: 2e38 3831 3730 392c 322e 3430 3836 3520  .881709,2.40865 
+000088d0: 2d33 2e35 3834 3534 312c 322e 3837 3834  -3.584541,2.8784
+000088e0: 3120 2d35 2e35 3231 3330 342c 332e 3834  1 -5.521304,3.84
+000088f0: 3033 3720 302e 3534 3532 3231 2c2d 312e  037 0.545221,-1.
+00008900: 3933 3233 3420 302e 3338 3836 3537 2c2d  93234 0.388657,-
+00008910: 332e 3532 3839 3920 2d30 2e34 3630 3634  3.52899 -0.46064
+00008920: 352c 2d34 2e39 3738 3720 2d31 2e35 3035  5,-4.9787 -1.505
+00008930: 3735 332c 312e 3339 3730 3820 2d33 2e32  753,1.39708 -3.2
+00008940: 3032 3635 332c 312e 3331 3932 3920 2d34  02653,1.31929 -4
+00008950: 2e30 3331 3939 2c30 2e39 3733 3931 2032  .03199,0.97391 2
+00008960: 2e30 3933 3535 372c 2d31 2e35 3337 3832  .093557,-1.53782
+00008970: 2032 2e34 3236 3733 352c 2d33 2e31 3938   2.426735,-3.198
+00008980: 3438 2031 2e34 3934 3130 322c 2d35 2e33  48 1.494102,-5.3
+00008990: 3737 3339 202d 312e 3537 3938 3935 2c33  7739 -1.579895,3
+000089a0: 2e36 3233 3939 202d 332e 3838 3938 3239  .62399 -3.889829
+000089b0: 2c34 2e38 3733 3835 202d 362e 3739 3933  ,4.87385 -6.7993
+000089c0: 3033 2c36 2e31 3433 3336 2030 2e37 3733  03,6.14336 0.773
+000089d0: 3538 352c 2d31 2e33 3830 3535 2031 2e39  585,-1.38055 1.9
+000089e0: 3530 3333 392c 2d32 2e37 3436 3935 2032  50339,-2.74695 2
+000089f0: 2e31 3831 3035 382c 2d34 2e30 3037 3339  .181058,-4.00739
+00008a00: 202d 302e 3532 3433 3833 2c30 2e32 3139   -0.524383,0.219
+00008a10: 3433 202d 302e 3932 3933 3937 2c30 2e33  43 -0.929397,0.3
+00008a20: 3835 3631 202d 312e 3334 3135 3736 2c30  8561 -1.341576,0
+00008a30: 2e32 3534 3836 2032 2e32 3930 3138 332c  .25486 2.290183,
+00008a40: 2d32 2e37 3038 3837 2031 2e33 3338 3438  -2.70887 1.33848
+00008a50: 392c 2d34 2e38 3339 3239 2030 2e38 3134  9,-4.83929 0.814
+00008a60: 3335 392c 2d36 2e33 3035 3220 2d31 2e35  359,-6.3052 -1.5
+00008a70: 3437 3931 2c31 2e32 3733 3936 202d 322e  4791,1.27396 -2.
+00008a80: 3936 3435 3536 2c31 2e39 3434 3032 202d  964556,1.94402 -
+00008a90: 342e 3732 3634 3835 2c32 2e33 3831 3036  4.726485,2.38106
+00008aa0: 2030 2e36 3637 3033 322c 2d32 2e32 3635   0.667032,-2.265
+00008ab0: 3739 2031 2e30 3038 3433 2c2d 342e 3332  79 1.00843,-4.32
+00008ac0: 3336 3720 2d30 2e35 3931 3136 2c2d 372e  367 -0.59116,-7.
+00008ad0: 3039 3631 3620 2d31 2e30 3439 3234 372c  09616 -1.049247,
+00008ae0: 302e 3734 3234 3220 2d31 2e32 3335 3533  0.74242 -1.23553
+00008af0: 392c 312e 3336 3434 3920 2d33 2e34 3639  9,1.36449 -3.469
+00008b00: 3836 312c 312e 3630 3337 3320 312e 3236  861,1.60373 1.26
+00008b10: 3337 3033 2c2d 322e 3635 3139 2030 2e35  3703,-2.6519 0.5
+00008b20: 3537 3537 382c 2d34 2e39 3538 3720 302e  57578,-4.9587 0.
+00008b30: 3139 3539 3738 2c2d 372e 3330 3135 3320  195978,-7.30153 
+00008b40: 2d31 2e36 3932 3735 372c 322e 3737 3932  -1.692757,2.7792
+00008b50: 3120 2d31 2e39 3835 3235 3438 2c33 2e35  1 -1.9852548,3.5
+00008b60: 3234 3733 202d 342e 3631 3636 3037 382c  2473 -4.6166078,
+00008b70: 332e 3932 3034 3120 312e 3434 3032 3838  3.92041 1.440288
+00008b80: 2c2d 322e 3232 3137 3620 302e 3037 3633  ,-2.22176 0.0763
+00008b90: 382c 2d34 2e38 3037 3231 202d 312e 3231  8,-4.80721 -1.21
+00008ba0: 3936 3234 2c2d 362e 3934 3338 3620 322e  9624,-6.94386 2.
+00008bb0: 3032 3930 3536 2c30 2e33 3134 3937 2033  029056,0.31497 3
+00008bc0: 2e33 3938 3033 312c 332e 3431 3539 2031  .398031,3.4159 1
+00008bd0: 2e37 3132 3337 352c 362e 3534 3231 3620  .712375,6.54216 
+00008be0: 322e 3134 3639 3338 2c2d 302e 3431 3238  2.146938,-0.4128
+00008bf0: 3720 322e 3737 3632 3930 382c 2d33 2e32  7 2.7762908,-3.2
+00008c00: 3634 3232 2033 2e39 3330 3838 3138 2c2d  6422 3.9308818,-
+00008c10: 352e 3237 3136 3120 312e 3339 3033 3137  5.27161 1.390317
+00008c20: 2c32 2e34 3138 3435 2032 2e38 3930 3236  ,2.41845 2.89026
+00008c30: 312c 342e 3534 3337 3820 302e 3534 3235  1,4.54378 0.5425
+00008c40: 3036 2c38 2e36 3236 3331 206c 2033 2e30  06,8.62631 l 3.0
+00008c50: 3234 3933 372c 2d32 2e39 3038 3136 2063  24937,-2.90816 c
+00008c60: 2031 2e30 3836 3232 2c32 2e32 3530 3720   1.08622,2.2507 
+00008c70: 332e 3138 3131 3734 2c33 2e37 3636 3734  3.181174,3.76674
+00008c80: 2031 2e30 3139 3631 342c 382e 3338 3238   1.019614,8.3828
+00008c90: 3520 6c20 342e 3135 3739 3132 2c2d 332e  5 l 4.157912,-3.
+00008ca0: 3836 3933 3420 6320 312e 3331 3734 362c  86934 c 1.31746,
+00008cb0: 322e 3134 3934 3620 322e 3839 3531 3234  2.14946 2.895124
+00008cc0: 2c33 2e34 3638 3032 202d 302e 3139 3837  ,3.46802 -0.1987
+00008cd0: 3631 2c37 2e39 3333 3431 206c 2031 2e39  61,7.93341 l 1.9
+00008ce0: 3030 3836 372c 2d31 2e36 3132 3238 2063  00867,-1.61228 c
+00008cf0: 202d 302e 3635 3731 3635 2c31 2e37 3436   -0.657165,1.746
+00008d00: 3520 2d31 2e33 3735 3333 362c 332e 3437  5 -1.375336,3.47
+00008d10: 3239 3120 2d32 2e36 3531 3132 382c 352e  291 -2.651128,5.
+00008d20: 3031 3537 3220 332e 3634 3031 3531 2c2d  01572 3.640151,-
+00008d30: 312e 3531 3633 3520 342e 3337 3539 3732  1.51635 4.375972
+00008d40: 2c2d 352e 3232 3935 3620 352e 3936 3138  ,-5.22956 5.9618
+00008d50: 3237 2c2d 382e 3239 3937 3920 322e 3236  27,-8.29979 2.26
+00008d60: 3231 3635 2c32 2e35 3634 3520 312e 3638  2165,2.5645 1.68
+00008d70: 3739 3337 2c36 2e38 3737 3236 202d 302e  7937,6.87726 -0.
+00008d80: 3939 3234 3133 2c38 2e31 3533 3431 2032  992413,8.15341 2
+00008d90: 2e36 3139 3134 342c 302e 3134 3237 3720  .619144,0.14277 
+00008da0: 332e 3233 3132 3036 2c2d 312e 3835 3135  3.231206,-1.8515
+00008db0: 3420 332e 3936 3430 3532 2c2d 332e 3037  4 3.964052,-3.07
+00008dc0: 3135 2030 2e36 3934 3036 392c 312e 3231  15 0.694069,1.21
+00008dd0: 3037 2032 2e31 3334 3135 362c 332e 3234  07 2.134156,3.24
+00008de0: 3334 3520 302e 3632 3535 3338 2c36 2e35  345 0.625538,6.5
+00008df0: 3935 3434 2031 2e36 3930 3735 332c 2d30  9544 1.690753,-0
+00008e00: 2e36 3331 3932 2033 2e37 3838 3832 372c  .63192 3.788827,
+00008e10: 2d33 2e31 3737 3136 2035 2e32 3533 3835  -3.17716 5.25385
+00008e20: 382c 2d35 2e30 3639 3632 2030 2e38 3139  8,-5.06962 0.819
+00008e30: 3935 312c 312e 3738 3134 3620 312e 3437  951,1.78146 1.47
+00008e40: 3538 3636 2c33 2e38 3733 3236 2030 2e31  5866,3.87326 0.1
+00008e50: 3134 3935 342c 352e 3539 3932 3920 302e  14954,5.59929 0.
+00008e60: 3937 3832 3733 2c2d 302e 3536 3936 3720  978273,-0.56967 
+00008e70: 312e 3132 3338 3437 2c2d 312e 3433 3937  1.123847,-1.4397
+00008e80: 2031 2e34 3838 3631 372c 2d32 2e32 3330   1.488617,-2.230
+00008e90: 3636 2031 2e30 3539 3139 312c 322e 3531  66 1.059191,2.51
+00008ea0: 3130 3820 302e 3638 3338 3234 2c33 2e36  108 0.683824,3.6
+00008eb0: 3031 3532 202d 302e 3339 3833 3335 2c35  0152 -0.398335,5
+00008ec0: 2e35 3537 3133 2030 2e34 3030 3734 322c  .55713 0.400742,
+00008ed0: 2d30 2e30 3438 3820 332e 3135 3438 3936  -0.0488 3.154896
+00008ee0: 2c2d 322e 3636 3635 2034 2e33 3039 3632  ,-2.6665 4.30962
+00008ef0: 322c 2d35 2e33 3439 3238 2030 2c30 2031  2,-5.34928 0,0 1
+00008f00: 2e31 3334 3938 372c 312e 3739 3935 3320  .134987,1.79953 
+00008f10: 302e 3231 3938 3139 2c33 2e30 3235 3237  0.219819,3.02527
+00008f20: 2030 2e36 3334 3933 2c2d 302e 3334 3836   0.63493,-0.3486
+00008f30: 3220 322e 3637 3330 3038 2c2d 332e 3639  2 2.673008,-3.69
+00008f40: 3533 3320 322e 3637 3330 3038 2c2d 332e  533 2.673008,-3.
+00008f50: 3639 3533 3320 322e 3937 3232 3436 2c35  69533 2.972246,5
+00008f60: 2e37 3637 3936 2032 2e30 3839 3932 362c  .76796 2.089926,
+00008f70: 382e 3139 3039 3820 312e 3336 3131 3435  8.19098 1.361145
+00008f80: 2c39 2e36 3733 3135 207a 220a 2020 2020  ,9.67315 z".    
+00008f90: 2020 2069 643d 2270 6174 6836 220a 2020     id="path6".  
+00008fa0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00008fb0: 6465 7479 7065 733d 2263 6363 6363 6363  detypes="ccccccc
+00008fc0: 6363 6363 6363 6363 6363 6363 6363 6363  cccccccccccccccc
+00008fd0: 6363 6363 6363 6363 6363 6363 6363 6363  cccccccccccccccc
+00008fe0: 6363 6363 6322 202f 3e0a 2020 2020 3c70  ccccc" />.    <p
+00008ff0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00009000: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+00009010: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+00009020: 652d 7769 6474 683a 322e 393b 7374 726f  e-width:2.9;stro
+00009030: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00009040: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00009050: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00009060: 6572 6c69 6d69 743a 332e 343b 7374 726f  erlimit:3.4;stro
+00009070: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00009080: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00009090: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+000090a0: 3131 352e 3139 3331 382c 3130 332e 3239  115.19318,103.29
+000090b0: 3231 3520 6320 302e 3834 3134 312c 2d31  215 c 0.84141,-1
+000090c0: 2e36 3534 3735 202d 322e 3134 3439 372c  .65475 -2.14497,
+000090d0: 342e 3032 3232 3620 2d34 2e32 3335 3836  4.02226 -4.23586
+000090e0: 2c34 2e36 3833 3038 2030 2e32 3733 3531  ,4.68308 0.27351
+000090f0: 2c2d 322e 3632 3736 3620 2d31 2e36 3430  ,-2.62766 -1.640
+00009100: 3331 2c2d 382e 3134 3534 3720 2d33 2e30  31,-8.14547 -3.0
+00009110: 3532 3638 2c2d 392e 3531 3732 3920 2d30  5268,-9.51729 -0
+00009120: 2e39 3038 3636 2c32 2e39 3934 3820 2d32  .90866,2.9948 -2
+00009130: 2e35 3238 3931 2c35 2e34 3234 3531 202d  .52891,5.42451 -
+00009140: 352e 3233 3334 362c 362e 3432 3239 3620  5.23346,6.42296 
+00009150: 302e 3435 3631 352c 2d33 2e35 3436 3439  0.45615,-3.54649
+00009160: 202d 302e 3530 3535 362c 2d36 2e32 3830   -0.50556,-6.280
+00009170: 3438 202d 322e 3039 3434 392c 2d39 2e33  48 -2.09449,-9.3
+00009180: 3338 3833 3120 2d31 2e36 3934 3135 342c  38831 -1.694154,
+00009190: 322e 3537 3535 3931 202d 332e 3337 3931  2.575591 -3.3791
+000091a0: 3338 2c35 2e31 3733 3633 3120 2d35 2e38  38,5.173631 -5.8
+000091b0: 3530 3139 342c 352e 3834 3734 3231 2030  50194,5.847421 0
+000091c0: 2e34 3831 3031 332c 2d34 2e32 3438 3431  .481013,-4.24841
+000091d0: 202d 302e 3433 3034 3436 2c2d 382e 3332   -0.430446,-8.32
+000091e0: 3637 3934 202d 322e 3136 3633 3532 2c2d  6794 -2.166352,-
+000091f0: 3132 2e33 3034 3530 3520 2d30 2e39 3836  12.304505 -0.986
+00009200: 3036 362c 322e 3837 3334 3933 202d 352e  066,2.873493 -5.
+00009210: 3433 3033 3435 2c37 2e31 3039 3532 3820  430345,7.109528 
+00009220: 2d37 2e31 3930 3839 352c 372e 3738 3830  -7.190895,7.7880
+00009230: 3938 2031 2e30 3833 3339 372c 2d32 2e36  98 1.083397,-2.6
+00009240: 3533 3335 3420 322e 3330 3631 3433 2c2d  53354 2.306143,-
+00009250: 372e 3630 3738 3334 2031 2e36 3733 3431  7.607834 1.67341
+00009260: 372c 2d31 302e 3639 3335 3134 202d 312e  7,-10.693514 -1.
+00009270: 3630 3338 392c 322e 3038 3839 3739 202d  60389,2.088979 -
+00009280: 342e 3339 3032 3839 2c34 2e30 3735 3436  4.390289,4.07546
+00009290: 3820 2d36 2e32 3835 3138 352c 352e 3134  8 -6.285185,5.14
+000092a0: 3131 3535 2030 2e39 3531 3739 352c 2d32  1155 0.951795,-2
+000092b0: 2e34 3633 3333 3120 312e 3930 3932 3539  .463331 1.909259
+000092c0: 2c2d 372e 3334 3835 3037 2030 2e34 3931  ,-7.348507 0.491
+000092d0: 3739 352c 2d31 302e 3130 3632 3934 202d  795,-10.106294 -
+000092e0: 312e 3838 3038 3636 2c33 2e30 3235 3637  1.880866,3.02567
+000092f0: 3820 2d33 2e35 3534 3639 382c 342e 3137  8 -3.554698,4.17
+00009300: 3532 3220 2d35 2e37 3235 3032 352c 352e  522 -5.725025,5.
+00009310: 3336 3431 3820 312e 3431 3534 352c 2d34  36418 1.41545,-4
+00009320: 2e37 3932 3430 3120 2d30 2e32 3235 3137  .792401 -0.22517
+00009330: 372c 2d31 332e 3036 3738 3132 202d 332e  7,-13.067812 -3.
+00009340: 3930 3334 3937 2c2d 3132 2e37 3237 3834  903497,-12.72784
+00009350: 2031 2e31 3034 3235 362c 2d31 2e33 3632   1.104256,-1.362
+00009360: 3235 2032 2e33 3131 3533 2c2d 322e 3536  25 2.31153,-2.56
+00009370: 3633 3439 2032 2e37 3936 3137 372c 2d33  6349 2.796177,-3
+00009380: 2e30 3133 3535 3222 0a20 2020 2020 2020  .013552".       
+00009390: 6964 3d22 7061 7468 3722 0a20 2020 2020  id="path7".     
+000093a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000093b0: 7970 6573 3d22 6363 6363 6363 6363 6363  ypes="cccccccccc
+000093c0: 6363 6363 2220 2f3e 0a20 2020 203c 670a  cccc" />.    <g.
+000093d0: 2020 2020 2020 2069 643d 2267 3433 220a         id="g43".
+000093e0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000093f0: 3d22 7472 616e 736c 6174 6528 2d38 372e  ="translate(-87.
+00009400: 3637 3337 3633 2c37 372e 3530 3231 3538  673763,77.502158
+00009410: 2922 3e0a 2020 2020 2020 3c70 6174 680a  )">.      <path.
+00009420: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00009430: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+00009440: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00009450: 7769 6474 683a 302e 3236 3435 3833 7078  width:0.264583px
+00009460: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00009470: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00009480: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00009490: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000094a0: 2020 2020 2020 643d 224d 2031 352e 3033        d="M 15.03
+000094b0: 3138 3433 2c31 332e 3037 3536 3434 2043  1843,13.075644 C
+000094c0: 2034 322e 3930 3634 3137 2c31 392e 3238   42.906417,19.28
+000094d0: 3930 3633 2037 392e 3638 3830 3636 2c31  9063 79.688066,1
+000094e0: 382e 3234 3731 3337 2031 3234 2e33 3738  8.247137 124.378
+000094f0: 3132 2c31 302e 3736 3333 3422 0a20 2020  12,10.76334".   
+00009500: 2020 2020 2020 6964 3d22 7061 7468 3222        id="path2"
+00009510: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
+00009520: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00009530: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+00009540: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00009550: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
+00009560: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00009570: 2d77 6964 7468 3a33 3b73 7472 6f6b 652d  -width:3;stroke-
+00009580: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00009590: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+000095a0: 6572 3b73 7472 6f6b 652d 6461 7368 6172  er;stroke-dashar
+000095b0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+000095c0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+000095d0: 2020 2020 643d 224d 2031 302e 3734 3138      d="M 10.7418
+000095e0: 3639 2c31 312e 3333 3037 3239 2043 2031  69,11.330729 C 1
+000095f0: 392e 3138 3234 3132 2c38 2e34 3135 3937  9.182412,8.41597
+00009600: 3031 2032 322e 3637 3036 3132 2c35 2e30  01 22.670612,5.0
+00009610: 3637 3232 3320 3535 2e33 3636 3835 352c  67223 55.366855,
+00009620: 342e 3230 3433 3331 3420 6c20 362e 3634  4.2043314 l 6.64
+00009630: 3736 3234 2c38 2e36 3238 3037 3036 2032  7624,8.6280706 2
+00009640: 2e33 3139 3238 332c 2d39 2e31 3635 3831  .319283,-9.16581
+00009650: 3335 2043 2038 322e 3639 3730 3138 2c33  35 C 82.697018,3
+00009660: 2e32 3937 3839 3620 3937 2e33 3737 3633  .297896 97.37763
+00009670: 382c 342e 3131 3633 3535 3720 3130 392e  8,4.1163557 109.
+00009680: 3932 3332 332c 3132 2e39 3239 3237 3220  92323,12.929272 
+00009690: 3130 342e 3432 3538 342c 3137 2e33 3437  104.42584,17.347
+000096a0: 3732 3120 3130 302e 3937 3035 352c 3230  721 100.97055,20
+000096b0: 2e35 3833 3038 3120 3837 2e30 3936 3333  .583081 87.09633
+000096c0: 392c 3235 2e30 3039 3230 3120 3731 2e35  9,25.009201 71.5
+000096d0: 3431 3339 392c 3239 2e39 3731 3530 3320  41399,29.971503 
+000096e0: 3534 2e39 3237 3332 312c 3331 2e34 3433  54.927321,31.443
+000096f0: 3135 3520 3334 2e32 3130 3234 312c 3235  155 34.210241,25
+00009700: 2e36 3534 3231 3820 3139 2e31 3536 3239  .654218 19.15629
+00009710: 352c 3231 2e34 3437 3732 2031 342e 3133  5,21.44772 14.13
+00009720: 3133 3231 2c31 352e 3637 3935 3431 2031  1321,15.679541 1
+00009730: 302e 3734 3138 3639 2c31 312e 3333 3037  0.741869,11.3307
+00009740: 3239 205a 220a 2020 2020 2020 2020 2069  29 Z".         i
+00009750: 643d 2270 6174 6838 220a 2020 2020 2020  d="path8".      
+00009760: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00009770: 7479 7065 733d 2263 6363 6363 7373 6322  types="cccccssc"
+00009780: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00009790: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+000097a0: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
+000097b0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+000097c0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+000097d0: 652d 7769 6474 683a 302e 3236 3435 3833  e-width:0.264583
+000097e0: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
+000097f0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00009800: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00009810: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00009820: 2020 2020 2020 2020 643d 226d 2031 3038          d="m 108
+00009830: 2e37 3631 3438 2c31 302e 3931 3836 3935  .76148,10.918695
+00009840: 2063 2033 2e36 3935 3431 2c2d 302e 3034   c 3.69541,-0.04
+00009850: 3538 3320 3130 2e39 3031 3138 2c2d 322e  583 10.90118,-2.
+00009860: 3230 3030 3539 3420 3130 2e39 3031 3138  2000594 10.90118
+00009870: 2c2d 322e 3230 3030 3539 3420 312e 3738  ,-2.2000594 1.78
+00009880: 3431 312c 322e 3337 3630 3338 3420 342e  411,2.3760384 4.
+00009890: 3034 3139 362c 332e 3634 3831 3332 3420  04196,3.6481324 
+000098a0: 362e 3939 3633 352c 332e 3239 3730 3838  6.99635,3.297088
+000098b0: 3420 6c20 2d31 382e 3633 3835 382c 332e  4 l -18.63858,3.
+000098c0: 3837 3736 3037 207a 220a 2020 2020 2020  877607 z".      
+000098d0: 2020 2069 643d 2270 6174 6839 220a 2020     id="path9".  
+000098e0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000098f0: 6e6f 6465 7479 7065 733d 2263 6363 6363  nodetypes="ccccc
+00009900: 2220 2f3e 0a20 2020 203c 2f67 3e0a 2020  " />.    </g>.  
+00009910: 3c2f 673e 0a3c 2f73 7667 3e0a            </g>.</svg>.
```

### Comparing `capypdf-0.8.0/images/capylogo_web.png` & `capypdf-0.9.0/images/capylogo_web.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/cmyk_tiff.tif` & `capypdf-0.9.0/images/cmyk_tiff.tif`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/comic-colors.png` & `capypdf-0.9.0/images/comic-colors.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/comic-lines.png` & `capypdf-0.9.0/images/comic-lines.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/comic-richblack.png` & `capypdf-0.9.0/images/comic-richblack.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/flame_gradient.png` & `capypdf-0.9.0/images/flame_gradient.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/fogra_cmyk.tif` & `capypdf-0.9.0/images/fogra_cmyk.tif`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/gray_alpha.png` & `capypdf-0.9.0/images/gray_alpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/object_gradient.png` & `capypdf-0.9.0/images/object_gradient.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/rgb_tiff.tif` & `capypdf-0.9.0/images/rgb_tiff.tif`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/images/simple.jpg` & `capypdf-0.9.0/images/simple.jpg`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/include/capypdf.h.in` & `capypdf-0.9.0/include/capypdf.h.in`

 * *Files 16% similar despite different names*

```diff
@@ -140,14 +140,90 @@
 
 typedef enum {
     CAPY_COMPRESSION_NONE,
     CAPY_COMPRESSION_DEFLATE,
     // CAPY_COMPRESSION_CCIT4,
 } CapyPDF_Compression;
 
+typedef enum {
+    CAPY_ANNOTATION_FLAG_NONE = 0,
+    CAPY_ANNOTATION_FLAG_INVISIBLE = 1,
+    CAPY_ANNOTATION_FLAG_HIDDEN = (1 << 1),
+    CAPY_ANNOTATION_FLAG_PRINT = (1 << 2),
+    CAPY_ANNOTATION_FLAG_NOZOOM = (1 << 3),
+    CAPY_ANNOTATION_FLAG_NOROTATE = (1 << 4),
+    CAPY_ANNOTATION_FLAG_NOVIEW = (1 << 5),
+    CAPY_ANNOTATION_FLAG_READONLY = (1 << 6),
+    CAPY_ANNOTATION_FLAG_LOCKED = (1 << 7),
+    CAPY_ANNOTATION_FLAG_TOGGLENOVIEW = (1 << 8),
+    CAPY_ANNOTATION_FLAG_LOCKEDCONTENTS = (1 << 9),
+} CapyPDF_AnnotationFlags;
+
+typedef enum {
+    CAPY_STRUCTURE_TYPE_DOCUMENT,
+    CAPY_STRUCTURE_TYPE_DOCUMENT_FRAGMENT,
+
+    CAPY_STRUCTURE_TYPE_PART,
+    CAPY_STRUCTURE_TYPE_SECT,
+    CAPY_STRUCTURE_TYPE_DIV,
+    CAPY_STRUCTURE_TYPE_ASIDE,
+    CAPY_STRUCTURE_TYPE_NONSTRUCT,
+
+    CAPY_STRUCTURE_TYPE_P,
+    CAPY_STRUCTURE_TYPE_H,
+    CAPY_STRUCTURE_TYPE_H1,
+    CAPY_STRUCTURE_TYPE_H2,
+    CAPY_STRUCTURE_TYPE_H3,
+    CAPY_STRUCTURE_TYPE_H4,
+    CAPY_STRUCTURE_TYPE_H5,
+    CAPY_STRUCTURE_TYPE_H6,
+    CAPY_STRUCTURE_TYPE_H7,
+    CAPY_STRUCTURE_TYPE_TITLE,
+    CAPY_STRUCTURE_TYPE_FENOTE,
+
+    CAPY_STRUCTURE_TYPE_SUB,
+
+    CAPY_STRUCTURE_TYPE_LBL,
+    CAPY_STRUCTURE_TYPE_SPAN,
+    CAPY_STRUCTURE_TYPE_EM,
+    CAPY_STRUCTURE_TYPE_STRONG,
+    CAPY_STRUCTURE_TYPE_LINK,
+    CAPY_STRUCTURE_TYPE_ANNOT,
+    CAPY_STRUCTURE_TYPE_FORM,
+
+    CAPY_STRUCTURE_TYPE_RUBY,
+    CAPY_STRUCTURE_TYPE_RB,
+    CAPY_STRUCTURE_TYPE_RT,
+    CAPY_STRUCTURE_TYPE_RP,
+    CAPY_STRUCTURE_TYPE_WARICHU,
+    CAPY_STRUCTURE_TYPE_WT,
+    CAPY_STRUCTURE_TYPE_WP,
+
+    CAPY_STRUCTURE_TYPE_L,
+    CAPY_STRUCTURE_TYPE_LI,
+    CAPY_STRUCTURE_TYPE_LBODY,
+    CAPY_STRUCTURE_TYPE_TABLE,
+    CAPY_STRUCTURE_TYPE_TR,
+    CAPY_STRUCTURE_TYPE_TH,
+    CAPY_STRUCTURE_TYPE_TD,
+    CAPY_STRUCTURE_TYPE_THEAD,
+    CAPY_STRUCTURE_TYPE_TBODY,
+    CAPY_STRUCTURE_TYPE_TFOOT,
+
+    CAPY_STRUCTURE_TYPE_CAPTION,
+
+    CAPY_STRUCTURE_TYPE_FIGURE,
+
+    CAPY_STRUCTURE_TYPE_FORMULA,
+
+    CAPY_STRUCTURE_TYPE_ARTIFACT,
+
+    CAPY_STRUCTURE_TYPE_NUM_ITEMS
+} CapyPDF_StructureType;
+
 // clang-format off
 /* Not used yet.
 enum CAPYPDF_Color_Management_Policy {
     CAPY_CCP_Preserve,                  // Pass all colors directly through without conversion or checking.
     CAPY_CCP_ToOutput,                  // Convert everything to output colorspace
     CAPY_CCP_ToOutputExceptManaged,     // Convert everything to output cs except color managed content (ICC, L*a*b* etc)
     CAPY_CCP_OnlyOutputAllowed,         // Use of any colorspace except output is an error except using Gray in RGB and CMYK.
@@ -237,14 +313,18 @@
     int32_t id;
 } CapyPDF_SeparationId;
 
 typedef struct {
     int32_t id;
 } CapyPDF_PatternId;
 
+typedef struct {
+    int32_t id;
+} CapyPDF_RoleId;
+
 // Options
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_new(CapyPDF_Options **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_destroy(CapyPDF_Options *) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_title(CapyPDF_Options *opt,
                                                  const char *utf8_title) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_author(CapyPDF_Options *opt,
@@ -258,14 +338,16 @@
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_colorspace(CapyPDF_Options *opt,
                                                       CapyPDF_Colorspace cs) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_output_intent(CapyPDF_Options *opt,
                                                          CapyPDF_Intent_Subtype stype,
                                                          const char *identifier) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_default_page_properties(
     CapyPDF_Options *opt, const CapyPDF_PageProperties *prop) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_tagged(CapyPDF_Options *opt,
+                                                  int32_t is_tagged) CAPYPDF_NOEXCEPT;
 
 // Page properties.
 CAPYPDF_PUBLIC CapyPDF_EC capy_page_properties_new(CapyPDF_PageProperties **out_ptr)
     CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_page_properties_destroy(CapyPDF_PageProperties *) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_page_properties_set_pagebox(CapyPDF_PageProperties *prop,
                                                            CapyPDF_Page_Box boxtype,
@@ -277,95 +359,123 @@
 // Generator
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_new(const char *filename,
                                              const CapyPDF_Options *options,
                                              CapyPDF_Generator **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_page(CapyPDF_Generator *g,
                                                   CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_form_xobject(
-    CapyPDF_Generator *g, CapyPDF_DrawContext *ctx, CapyPDF_FormXObjectId *fxid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_color_pattern(CapyPDF_Generator *g,
-                                                           CapyPDF_DrawContext *ctx,
-                                                           CapyPDF_PatternId *pid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_jpg(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_form_xobject(CapyPDF_Generator *gen,
+                                                          CapyPDF_DrawContext *ctx,
+                                                          CapyPDF_FormXObjectId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_color_pattern(
+    CapyPDF_Generator *g, CapyPDF_DrawContext *ctx, CapyPDF_PatternId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_jpg(CapyPDF_Generator *gen,
                                                    const char *fname,
                                                    CapyPDF_Image_Interpolation interpolate,
-                                                   CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT;
+                                                   CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT;
 // FIXME, specify whether to compress the file or not.
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_file(CapyPDF_Generator *g,
-                                                    const char *fname,
-                                                    CapyPDF_EmbeddedFileId *fid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_font(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_file(
+    CapyPDF_Generator *g, const char *fname, CapyPDF_EmbeddedFileId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_font(CapyPDF_Generator *gen,
                                                    const char *fname,
-                                                   CapyPDF_FontId *fid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_image(CapyPDF_Generator *g,
+                                                   CapyPDF_FontId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_image(CapyPDF_Generator *gen,
                                                     const char *fname,
                                                     CapyPDF_Image_Interpolation interpolate,
-                                                    CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_mask_image(CapyPDF_Generator *g,
+                                                    CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_mask_image(CapyPDF_Generator *gen,
                                                          const char *fname,
-                                                         CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_image(CapyPDF_Generator *g,
+                                                         CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_image(CapyPDF_Generator *gen,
                                                    CapyPDF_RasterImage *image,
-                                                   CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_function(
-    CapyPDF_Generator *g, CapyPDF_Type2Function *func, CapyPDF_FunctionId *fid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_shading(
-    CapyPDF_Generator *g, CapyPDF_Type2Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type3_shading(
-    CapyPDF_Generator *g, CapyPDF_Type3Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type4_shading(
-    CapyPDF_Generator *g, CapyPDF_Type4Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type6_shading(
-    CapyPDF_Generator *g, CapyPDF_Type6Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_graphics_state(CapyPDF_Generator *g,
+                                                   CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_function(CapyPDF_Generator *gen,
+                                                            CapyPDF_Type2Function *func,
+                                                            CapyPDF_FunctionId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type2Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type3_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type3Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type4_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type4Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type6_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type6Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_graphics_state(CapyPDF_Generator *gen,
                                                             const CapyPDF_GraphicsState *state,
-                                                            CapyPDF_GraphicsStateId *gsid)
+                                                            CapyPDF_GraphicsStateId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_structure_item(CapyPDF_Generator *gen,
+                                                            const CapyPDF_StructureType stype,
+                                                            const CapyPDF_StructureItemId *parent,
+                                                            CapyPDF_StructureItemId *out_ptr)
     CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC
+capy_generator_add_custom_structure_item(CapyPDF_Generator *gen,
+                                         const CapyPDF_RoleId role,
+                                         const CapyPDF_StructureItemId *parent,
+                                         CapyPDF_StructureItemId *out_ptr) CAPYPDF_NOEXCEPT;
+
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_icc_profile(
-    CapyPDF_Generator *g, const char *fname, CapyPDF_IccColorSpaceId *iid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_separation_simple(CapyPDF_Generator *g,
+    CapyPDF_Generator *gen, const char *fname, CapyPDF_IccColorSpaceId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_separation_simple(CapyPDF_Generator *gen,
                                                                   const char *separation_name,
                                                                   const CapyPDF_Color *c,
-                                                                  CapyPDF_SeparationId *sid)
+                                                                  CapyPDF_SeparationId *out_ptr)
     CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_write(CapyPDF_Generator *g) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_write(CapyPDF_Generator *gen) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC
-capy_generator_add_optional_content_group(CapyPDF_Generator *g,
+capy_generator_add_optional_content_group(CapyPDF_Generator *gen,
                                           const CapyPDF_OptionalContentGroup *ocg,
-                                          CapyPDF_OptionalContentGroupId *ocgid) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_annotation(CapyPDF_Generator *g,
+                                          CapyPDF_OptionalContentGroupId *out_ptr) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_annotation(CapyPDF_Generator *gen,
                                                            CapyPDF_Annotation *annotation,
-                                                           CapyPDF_AnnotationId *aid)
+                                                           CapyPDF_AnnotationId *out_ptr)
+    CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_rolemap_entry(CapyPDF_Generator *gen,
+                                                           const char *name,
+                                                           CapyPDF_StructureType builtin,
+                                                           CapyPDF_RoleId *out_ptr)
     CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_destroy(CapyPDF_Generator *g) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_destroy(CapyPDF_Generator *gen) CAPYPDF_NOEXCEPT;
 
 // FIXME: this must be changed to support PDF links that point to
 // specific coordinates on a page.
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_outline(CapyPDF_Generator *generator,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_outline(CapyPDF_Generator *gen,
                                                      const char *utf8_text,
                                                      int32_t page_number,
                                                      CapyPDF_OutlineId *parent,
                                                      CapyPDF_OutlineId *out_ptr) CAPYPDF_NOEXCEPT;
 
 // Probably not final API.
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_text_width(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_text_width(CapyPDF_Generator *gen,
                                                     const char *utf8_text,
                                                     CapyPDF_FontId font,
                                                     double pointsize,
-                                                    double *width) CAPYPDF_NOEXCEPT;
+                                                    double *out_ptr) CAPYPDF_NOEXCEPT;
 
 // Draw context
 
 CAPYPDF_PUBLIC CapyPDF_EC
-capy_page_draw_context_new(CapyPDF_Generator *g, CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT;
+capy_page_draw_context_new(CapyPDF_Generator *gen, CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_b(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_B(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_Bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BDC_builtin(
+    CapyPDF_DrawContext *ctx, CapyPDF_StructureItemId structid) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BDC_ocg(
     CapyPDF_DrawContext *ctx, CapyPDF_OptionalContentGroupId ocgid) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BMC(CapyPDF_DrawContext *ctx,
                                           const char *tag) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_c(CapyPDF_DrawContext *ctx,
                                         double x1,
                                         double y1,
@@ -445,53 +555,55 @@
                                               CapyPDF_FontId fid,
                                               double point_size,
                                               double x,
                                               double y) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_render_text_obj(CapyPDF_DrawContext *ctx,
                                                   CapyPDF_Text *text) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_set_page_transition(
-    CapyPDF_DrawContext *dc, CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT;
+    CapyPDF_DrawContext *ctx, CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC
-capy_dc_add_simple_navigation(CapyPDF_DrawContext *dc,
+capy_dc_add_simple_navigation(CapyPDF_DrawContext *ctx,
                               const CapyPDF_OptionalContentGroupId *ocgarray,
                               int32_t array_size,
                               const CapyPDF_Transition *tr) CAPYPDF_NOEXCEPT;
-CAPYPDF_PUBLIC CapyPDF_EC capy_dc_text_new(CapyPDF_DrawContext *dc,
+CAPYPDF_PUBLIC CapyPDF_EC capy_dc_text_new(CapyPDF_DrawContext *ctx,
                                            CapyPDF_Text **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_set_custom_page_properties(
-    CapyPDF_DrawContext *dc, const CapyPDF_PageProperties *custom_properties);
-CAPYPDF_PUBLIC CapyPDF_EC capy_dc_annotate(CapyPDF_DrawContext *dc,
+    CapyPDF_DrawContext *ctx, const CapyPDF_PageProperties *custom_properties);
+CAPYPDF_PUBLIC CapyPDF_EC capy_dc_annotate(CapyPDF_DrawContext *ctx,
                                            CapyPDF_AnnotationId aid) CAPYPDF_NOEXCEPT;
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_destroy(CapyPDF_DrawContext *) CAPYPDF_NOEXCEPT;
 
 // Form XObjects.
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_form_xobject_new(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_form_xobject_new(CapyPDF_Generator *gen,
                                                 double w,
                                                 double h,
                                                 CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT;
 
 // Color Pattern
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_color_pattern_context_new(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_color_pattern_context_new(CapyPDF_Generator *gen,
                                                          CapyPDF_DrawContext **out_ptr,
                                                          double w,
                                                          double h) CAPYPDF_NOEXCEPT;
 
 // Text
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_text_destroy(CapyPDF_Text *text) CAPYPDF_NOEXCEPT;
 // This is basically cmd_Tj except that it does kerning if the font and Freetype support it.
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_render_text(CapyPDF_Text *text,
                                                 const char *utf8_text) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_set_nonstroke(CapyPDF_Text *text,
                                                   const CapyPDF_Color *color) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_set_stroke(CapyPDF_Text *text,
                                                const CapyPDF_Color *color) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_BDC_builtin(CapyPDF_Text *text,
+                                                    CapyPDF_StructureItemId stid) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_EMC(CapyPDF_Text *text) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tc(CapyPDF_Text *text, double spacing) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Td(CapyPDF_Text *text, double x, double y) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tf(CapyPDF_Text *text,
                                            CapyPDF_FontId font,
                                            double pointsize) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_TL(CapyPDF_Text *text, double leading) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tm(CapyPDF_Text *text,
@@ -501,14 +613,15 @@
                                            double d,
                                            double e,
                                            double f) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tr(CapyPDF_Text *text,
                                            CapyPDF_Text_Mode tmode) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tw(CapyPDF_Text *text, double spacing) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tstar(CapyPDF_Text *text) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_text_destroy(CapyPDF_Text *text) CAPYPDF_NOEXCEPT;
 
 // Color
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_color_new(CapyPDF_Color **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_color_destroy(CapyPDF_Color *color) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_color_set_rgb(CapyPDF_Color *c, double r, double g, double b)
     CAPYPDF_NOEXCEPT;
@@ -563,81 +676,85 @@
                                                      int32_t h) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_raster_image_set_pixel_data(CapyPDF_RasterImage *image,
                                                            const char *buf,
                                                            int32_t bufsize) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_raster_image_destroy(CapyPDF_RasterImage *image) CAPYPDF_NOEXCEPT;
 
 // Functions
-CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_new(CapyPDF_Type2Function **out_ptr,
-                                                  double *domain,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_new(double *domain,
                                                   int32_t domain_size,
                                                   const CapyPDF_Color *c1,
                                                   const CapyPDF_Color *c2,
-                                                  double n) CAPYPDF_NOEXCEPT;
+                                                  double n,
+                                                  CapyPDF_Type2Function **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_destroy(CapyPDF_Type2Function *func) CAPYPDF_NOEXCEPT;
 
 // Shadings
-CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_new(CapyPDF_Type2Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_new(CapyPDF_Colorspace cs,
                                                  double x0,
                                                  double y0,
                                                  double x1,
                                                  double y1,
                                                  CapyPDF_FunctionId func,
                                                  int32_t extend1,
-                                                 int32_t extend2) CAPYPDF_NOEXCEPT;
+                                                 int32_t extend2,
+                                                 CapyPDF_Type2Shading **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_destroy(CapyPDF_Type2Shading *shade) CAPYPDF_NOEXCEPT;
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_new(CapyPDF_Type3Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_new(CapyPDF_Colorspace cs,
                                                  double *coords,
                                                  CapyPDF_FunctionId func,
                                                  int32_t extend1,
-                                                 int32_t extend2) CAPYPDF_NOEXCEPT;
+                                                 int32_t extend2,
+                                                 CapyPDF_Type3Shading **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_destroy(CapyPDF_Type3Shading *shade) CAPYPDF_NOEXCEPT;
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_new(CapyPDF_Type4Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_new(CapyPDF_Colorspace cs,
                                                  double minx,
                                                  double miny,
                                                  double maxx,
-                                                 double maxy) CAPYPDF_NOEXCEPT;
+                                                 double maxy,
+                                                 CapyPDF_Type4Shading **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_add_triangle(CapyPDF_Type4Shading *shade,
-                                                          double *coords,
-                                                          CapyPDF_Color **colors) CAPYPDF_NOEXCEPT;
+                                                          const double *coords,
+                                                          const CapyPDF_Color **colors)
+    CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_extend(CapyPDF_Type4Shading *shade,
                                                     int32_t flag,
-                                                    double *coords,
-                                                    CapyPDF_Color *color) CAPYPDF_NOEXCEPT;
+                                                    const double *coords,
+                                                    const CapyPDF_Color *color) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_destroy(CapyPDF_Type4Shading *shade) CAPYPDF_NOEXCEPT;
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_new(CapyPDF_Type6Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_new(CapyPDF_Colorspace cs,
                                                  double minx,
                                                  double miny,
                                                  double maxx,
-                                                 double maxy) CAPYPDF_NOEXCEPT;
+                                                 double maxy,
+                                                 CapyPDF_Type6Shading **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_add_patch(CapyPDF_Type6Shading *shade,
-                                                       double *coords,
-                                                       CapyPDF_Color **colors) CAPYPDF_NOEXCEPT;
+                                                       const double *coords,
+                                                       const CapyPDF_Color **colors)
+    CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_extend(CapyPDF_Type6Shading *shade,
                                                     int32_t flag,
-                                                    double *coords,
-                                                    CapyPDF_Color **colors) CAPYPDF_NOEXCEPT;
+                                                    const double *coords,
+                                                    const CapyPDF_Color **colors) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_destroy(CapyPDF_Type6Shading *shade) CAPYPDF_NOEXCEPT;
 
 // Annotations.
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_annotation_new(const char *utf8_text,
                                                    CapyPDF_Annotation **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_file_attachment_annotation_new(
     CapyPDF_EmbeddedFileId fid, CapyPDF_Annotation **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_printers_mark_annotation_new(
     CapyPDF_FormXObjectId fid, CapyPDF_Annotation **out_ptr) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_set_rectangle(
     CapyPDF_Annotation *annotation, double x1, double y1, double x2, double y2) CAPYPDF_NOEXCEPT;
+CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_set_flags(CapyPDF_Annotation *annotation,
+                                                    CapyPDF_AnnotationFlags flags) CAPYPDF_NOEXCEPT;
 CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_destroy(CapyPDF_Annotation *annotation) CAPYPDF_NOEXCEPT;
 
 // Error
 
 CAPYPDF_PUBLIC const char *capy_error_message(CapyPDF_EC error_code) CAPYPDF_NOEXCEPT;
 
 #ifdef __cplusplus
```

### Comparing `capypdf-0.8.0/meson.build` & `capypdf-0.9.0/meson.build`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('capypdf', 'cpp', 'c',
-  version: '0.8.0',
+  version: '0.9.0',
   default_options : ['cpp_std=c++23,c++latest', 'default_library=static'])
 
 version = meson.project_version()
 varr = version.split('.')
 cdata = configuration_data()
 cdata.set_quoted('CAPYPDF_VERSION_STR', version)
 cdata.set('CAPYPDF_VERSION_MAJOR', varr[0])
```

### Comparing `capypdf-0.8.0/pyproject.toml` & `capypdf-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.meson-python]
 shared-libs-win32 = true
 
 
 [project]
 name = 'capypdf'
-version = '0.8.0'
+version = '0.9.0'
 description = 'A color managed PDF generation library tech preview'
 readme = 'readme.md'
 requires-python = '>=3.10'
 license = {file = 'COPYING'}
 authors = [
   {name = 'Jussi Pakkanen', email = 'jpakkane@gmail.com'},
 ]
```

### Comparing `capypdf-0.8.0/python/capypdf.py` & `capypdf-0.9.0/python/capypdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2023-2024 Jussi Pakkanen
 
 
 import ctypes
 import os, sys
 import math
-from enum import Enum
+from enum import Enum, IntFlag, auto
 
 class LineCapStyle(Enum):
     Butt = 0
     Round = 1
     Projection_Square = 2
 
 class LineJoinStyle(Enum):
@@ -83,14 +83,85 @@
     # PDFE = 2
 
 class ImageInterpolation(Enum):
     Automatic = 0
     Pixelated = 1
     Smooth = 2
 
+class AnnotationFlag(IntFlag):
+    Invisible = auto()
+    Hidden = auto()
+    Print = auto()
+    Nozoom = auto()
+    NoRotate = auto()
+    NoView = auto()
+    ReadOnly = auto()
+    Locked = auto()
+    ToggleNoView = auto()
+    LockedContents = auto()
+
+class StructureType(Enum):
+    Document = 0
+    DocumentFragment = 1
+
+    Part = 2,
+    Sect = 3,
+    Div = 4
+    Aside = 5
+    Nonstruct = 6
+
+    P = 7
+    H = 8
+    H1 = 9
+    H2 = 10
+    H3 = 11
+    H4 = 12
+    H5 = 13
+    H6 = 14
+    H7 = 15
+    Title = 16
+    FENote = 17
+
+    Sub = 18
+
+    Lbl = 19
+    Span = 20
+    Em = 21
+    Strong = 22
+    Link = 23
+    Annot = 24
+    Form = 25
+
+    Ruby = 26,
+    RB = 27
+    RT = 28
+    RP = 29
+    Warichu = 30
+    WT = 31
+    WP = 32
+
+    L = 33
+    Li = 34
+    LBody = 35
+    Table = 36
+    TR = 37
+    TH = 38
+    TD = 39
+    Thead = 40
+    TBody = 41
+    TFoot = 42
+
+    Caption = 43
+
+    Figure = 44
+
+    Formula = 45
+
+    Artifact = 46
+
 class CapyPDFException(Exception):
     def __init__(*args, **kwargs):
         Exception.__init__(*args, **kwargs)
 
 ec_type = ctypes.c_int32
 enum_type = ctypes.c_int32
 
@@ -129,26 +200,34 @@
 
 class EmbeddedFileId(ctypes.Structure):
     _fields_ = [('id', ctypes.c_int32)]
 
 class FormXObjectId(ctypes.Structure):
     _fields_ = [('id', ctypes.c_int32)]
 
+class StructureItemId(ctypes.Structure):
+    _fields_ = [('id', ctypes.c_int32)]
+
+class RoleId(ctypes.Structure):
+    _fields_ = [('id', ctypes.c_int32)]
+
+
 cfunc_types = (
 
 ('capy_options_new', [ctypes.c_void_p]),
 ('capy_options_destroy', [ctypes.c_void_p]),
 ('capy_options_set_colorspace', [ctypes.c_void_p, enum_type]),
 ('capy_options_set_device_profile', [ctypes.c_void_p, enum_type, ctypes.c_char_p]),
 ('capy_options_set_title', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_options_set_author', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_options_set_creator', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_options_set_language', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_options_set_output_intent', [ctypes.c_void_p, enum_type, ctypes.c_char_p]),
 ('capy_options_set_default_page_properties', [ctypes.c_void_p, ctypes.c_void_p]),
+('capy_options_set_tagged', [ctypes.c_void_p, ctypes.c_int32]),
 
 ('capy_page_properties_new', [ctypes.c_void_p]),
 ('capy_page_properties_destroy', [ctypes.c_void_p]),
 ('capy_page_properties_set_pagebox',
     [ctypes.c_void_p, enum_type, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 
 ('capy_generator_new', [ctypes.c_char_p, ctypes.c_void_p, ctypes.c_void_p]),
@@ -163,20 +242,23 @@
 ('capy_generator_load_font', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_void_p]),
 ('capy_generator_add_image', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_type2_function', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_type2_shading', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_type3_shading', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_type4_shading', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_type6_shading', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
+('capy_generator_add_structure_item', [ctypes.c_void_p, enum_type, ctypes.c_void_p, ctypes.c_void_p]),
+('capy_generator_add_custom_structure_item', [ctypes.c_void_p, RoleId, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_write', [ctypes.c_void_p]),
 ('capy_generator_add_graphics_state', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_optional_content_group', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_outline', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_int32, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_create_separation_simple', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_text_width', [ctypes.c_void_p, ctypes.c_char_p, FontId, ctypes.c_double, ctypes.POINTER(ctypes.c_double)]),
+('capy_generator_add_rolemap_entry', [ctypes.c_void_p, ctypes.c_char_p, enum_type, ctypes.c_void_p]),
 ('capy_generator_destroy', [ctypes.c_void_p]),
 
 ('capy_page_draw_context_new', [ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_dc_add_simple_navigation', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_int32, ctypes.c_void_p]),
 ('capy_dc_cmd_b', [ctypes.c_void_p]),
 ('capy_dc_cmd_B', [ctypes.c_void_p]),
 ('capy_dc_cmd_bstar', [ctypes.c_void_p]),
@@ -230,14 +312,16 @@
 ('capy_dc_annotate', [ctypes.c_void_p, AnnotationId]),
 ('capy_dc_destroy', [ctypes.c_void_p]),
 
 ('capy_color_pattern_context_new', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_double, ctypes.c_double]),
 ('capy_form_xobject_new', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_void_p]),
 
 ('capy_text_destroy', [ctypes.c_void_p]),
+('capy_text_cmd_BDC_builtin', [ctypes.c_void_p, StructureItemId]),
+('capy_text_cmd_EMC', [ctypes.c_void_p]),
 ('capy_text_cmd_Tc', [ctypes.c_void_p, ctypes.c_double]),
 ('capy_text_cmd_Td', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double]),
 ('capy_text_cmd_Tf', [ctypes.c_void_p, FontId, ctypes.c_double]),
 ('capy_text_cmd_TL', [ctypes.c_void_p, ctypes.c_double]),
 ('capy_text_cmd_Tm', [ctypes.c_void_p,
     ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_text_cmd_Tr', [ctypes.c_void_p, enum_type]),
@@ -273,53 +357,53 @@
 ('capy_raster_image_set_size', [ctypes.c_void_p, ctypes.c_int32, ctypes.c_int32]),
 ('capy_raster_image_set_pixel_data', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_int32]),
 ('capy_raster_image_destroy', [ctypes.c_void_p]),
 
 ('capy_optional_content_group_new', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_optional_content_group_destroy', [ctypes.c_void_p]),
 
-('capy_type2_function_new', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_int32, ctypes.c_void_p, ctypes.c_void_p, ctypes.c_double]),
+('capy_type2_function_new', [ctypes.c_void_p, ctypes.c_int32, ctypes.c_void_p, ctypes.c_void_p, ctypes.c_double, ctypes.c_void_p]),
 ('capy_type2_function_destroy', [ctypes.c_void_p]),
 
-('capy_type2_shading_new', [ctypes.c_void_p, enum_type,
+('capy_type2_shading_new', [enum_type,
                             ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                            FunctionId, ctypes.c_int32, ctypes.c_int32]),
+                            FunctionId, ctypes.c_int32, ctypes.c_int32,
+                            ctypes.c_void_p]),
 ('capy_type2_shading_destroy', [ctypes.c_void_p]),
 
 
-('capy_type3_shading_new', [ctypes.c_void_p, enum_type, ctypes.POINTER(ctypes.c_double),
-                            FunctionId, ctypes.c_int32, ctypes.c_int32]),
+('capy_type3_shading_new', [enum_type, ctypes.POINTER(ctypes.c_double),
+                            FunctionId, ctypes.c_int32, ctypes.c_int32, ctypes.c_void_p]),
 ('capy_type3_shading_destroy', [ctypes.c_void_p]),
 
-('capy_type4_shading_new', [ctypes.c_void_p, enum_type,
-                            ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_type4_shading_new', [enum_type, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_void_p]),
 ('capy_type4_shading_add_triangle', [ctypes.c_void_p,
                                      ctypes.POINTER(ctypes.c_double),
                                      ctypes.c_void_p]),
 ('capy_type4_shading_extend', [ctypes.c_void_p,
                                ctypes.c_int32,
                                ctypes.POINTER(ctypes.c_double),
                                ctypes.c_void_p]),
 ('capy_type4_shading_destroy', [ctypes.c_void_p]),
 
-('capy_type6_shading_new', [ctypes.c_void_p, enum_type,
-                            ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_type6_shading_new', [enum_type, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_void_p]),
 ('capy_type6_shading_add_patch', [ctypes.c_void_p,
                                   ctypes.POINTER(ctypes.c_double),
                                   ctypes.c_void_p]),
 ('capy_type6_shading_extend', [ctypes.c_void_p,
                                ctypes.c_int32,
                                ctypes.POINTER(ctypes.c_double),
                                ctypes.c_void_p]),
 ('capy_type6_shading_destroy', [ctypes.c_void_p]),
 
 ('capy_text_annotation_new', [ctypes.c_char_p, ctypes.c_void_p]),
 ('capy_file_attachment_annotation_new', [EmbeddedFileId, ctypes.c_void_p]),
 ('capy_printers_mark_annotation_new', [FormXObjectId, ctypes.c_void_p]),
 ('capy_annotation_set_rectangle', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_annotation_set_flags', [ctypes.c_void_p, enum_type]),
 ('capy_annotation_destroy', [ctypes.c_void_p]),
 
 )
 
 if sys.platform == 'win32':
     libfile_name = 'capypdf-0.dll'
 elif sys.platform == 'darwin':
@@ -431,14 +515,19 @@
         check_error(libfile.capy_options_set_output_intent(self, stype.value, identifier.encode('utf-8')))
 
     def set_default_page_properties(self, props):
         if not isinstance(props, PageProperties):
             raise CapyPDFException('Argument is not a PageProperties object.')
         check_error(libfile.capy_options_set_default_page_properties(self, props))
 
+    def set_tagged(self, is_tagged):
+        tagint = 1 if is_tagged else 0
+        check_error(libfile.capy_options_set_tagged(self, tagint))
+
+
 class PageProperties:
     def __init__(self):
         opt = ctypes.c_void_p()
         check_error(libfile.capy_page_properties_new(ctypes.pointer(opt)))
         self._as_parameter_ = opt
 
     def __del__(self):
@@ -470,14 +559,20 @@
 
     def cmd_BDC(self, ocg):
         if not isinstance(ocg, OptionalContentGroupId):
             raise CapyPDFException('Argument must be an optional content group ID.')
         check_error(libfile.capy_dc_cmd_BDC_ocg(self, ocg))
         # FIXME, return a context manager.
 
+    def cmd_BDC_builtin(self, structid):
+        if not isinstance(structid, StructureItemId):
+            raise CapyPDFException('Argument must be a structure item ID.')
+        check_error(libfile.capy_dc_cmd_BDC_builtin(self, structid))
+        return MarkedContextManager(self)
+
     def cmd_BMC(self, tag):
         check_error(libfile.capy_dc_cmd_BMC(self, tag.encode('UTF-8')))
         return MarkedContextManager(self)
 
     def cmd_c(self, x1, y1, x2, y2, x3, y3):
         check_error(libfile.capy_dc_cmd_c(self, x1, y1, x2, y2, x3, y3))
 
@@ -825,14 +920,31 @@
     def add_type6_shading(self, type6shade):
         if not isinstance(type6shade, Type6Shading):
             raise CapyPDFException('Argument must be a type 4 shading object.')
         shid = ShadingId()
         check_error(libfile.capy_generator_add_type6_shading(self, type6shade, ctypes.pointer(shid)))
         return shid
 
+    def add_structure_item(self, struct_type, parent=None):
+        if parent is None:
+            parentptr = None
+        else:
+            if not isinstance(parent, StructureItemId):
+                raise CapyPDFException('Second argument must be a StructureItemID or None.')
+            parentptr = ctypes.pointer(parent)
+        stid = StructureItemId()
+        if isinstance(struct_type, StructureType):
+            check_error(libfile.capy_generator_add_structure_item(self, struct_type.value, parentptr, ctypes.pointer(stid)))
+        elif isinstance(struct_type, RoleId):
+            check_error(libfile.capy_generator_add_custom_structure_item(self, struct_type, parentptr, ctypes.pointer(stid)))
+        else:
+            raise CapyPDFException('First argument must be a structure item or role id.')
+        return stid
+
+
     def create_separation_simple(self, name, color):
         if not isinstance(color, Color):
             raise CapyPDFException('Color argument must be a color object.')
         sepid = SeparationId()
         text_bytes = name.encode('UTF-8')
         check_error(libfile.capy_generator_create_separation_simple(self, text_bytes, color, ctypes.pointer(sepid)))
         return sepid
@@ -874,14 +986,23 @@
         return ocgid
 
     def create_annotation(self, annotation):
         aid = AnnotationId()
         check_error(libfile.capy_generator_create_annotation(self, annotation, ctypes.pointer(aid)))
         return aid
 
+    def add_rolemap_entry(self, name, builtin_type):
+        if not isinstance(builtin_type, StructureType):
+            raise CapyPDFException('Builtin type must be a StructureType.')
+        roid = RoleId()
+        name_bytes = name.encode('ASCII')
+        check_error(libfile.capy_generator_add_rolemap_entry(self, name_bytes, builtin_type.value, ctypes.pointer(roid)))
+        return roid
+
+
 class Text:
     def __init__(self, dc):
         if not isinstance(dc, DrawContext):
             raise CapyPDFException('Argument must be a DrawingContext (preferably use its .text_new() method instead).')
         self._as_parameter_ = None
         opt = ctypes.c_void_p()
         check_error(libfile.capy_dc_text_new(dc, ctypes.pointer(opt)))
@@ -909,14 +1030,21 @@
 
     def set_nonstroke(self, color):
         check_error(libfile.capy_text_set_nonstroke(self, color))
 
     def set_stroke(self, color):
         check_error(libfile.capy_text_set_stroke(self, color))
 
+    def cmd_BDC_builtin(self, struct_id):
+        check_error(libfile.capy_text_cmd_BDC_builtin(self, struct_id))
+        return MarkedContextManager(self)
+
+    def cmd_EMC(self):
+        check_error(libfile.capy_text_cmd_EMC(self))
+
     def cmd_Tc(self, spacing):
         check_error(libfile.capy_text_cmd_Tc(self, spacing))
 
     def cmd_Td(self, x, y):
         check_error(libfile.capy_text_cmd_Td(self, x, y))
 
     def cmd_Tf(self, fontid, ptsize):
@@ -1049,54 +1177,52 @@
     def __del__(self):
         check_error(libfile.capy_optional_content_group_destroy(self))
 
 class Type2Function:
     def __init__(self, domain, c1, c2, n):
         self._as_parameter_ = None
         t2f = ctypes.c_void_p()
-        check_error(libfile.capy_type2_function_new(ctypes.pointer(t2f), *to_array(ctypes.c_double, domain), c1, c2, n))
+        check_error(libfile.capy_type2_function_new(*to_array(ctypes.c_double, domain), c1, c2, n, ctypes.pointer(t2f)))
         self._as_parameter_ = t2f
 
     def __del__(self):
         check_error(libfile.capy_type2_function_destroy(self))
 
 class Type2Shading:
     def __init__(self, cs, x0, y0, x1, y1, funcid, extend1, extend2):
         e1 = 1 if extend1 else 0
         e2 = 1 if extend2 else 0
         self._as_parameter_ = None
         t2s = ctypes.c_void_p()
-        check_error(libfile.capy_type2_shading_new(ctypes.pointer(t2s),
-            cs.value, x0, y0, x1, y1, funcid, e1, e2))
+        check_error(libfile.capy_type2_shading_new(cs.value, x0, y0, x1, y1, funcid, e1, e2, ctypes.pointer(t2s)))
         self._as_parameter_ = t2s
 
     def __del__(self):
         check_error(libfile.capy_type2_shading_destroy(self))
 
 class Type3Shading:
     def __init__(self, cs, coords, funcid, extend1, extend2):
         e1 = 1 if extend1 else 0
         e2 = 1 if extend2 else 0
         if len(coords) != 6:
             raise CapyPDFException('Coords array must hold exactly 6 doubles.')
         self._as_parameter_ = None
         t3s = ctypes.c_void_p()
-        check_error(libfile.capy_type3_shading_new(ctypes.pointer(t3s),
-            cs.value, to_array(ctypes.c_double, coords)[0], funcid, e1, e2))
+        check_error(libfile.capy_type3_shading_new(cs.value, to_array(ctypes.c_double, coords)[0], funcid, e1, e2, ctypes.pointer(t3s)))
         self._as_parameter_ = t3s
 
     def __del__(self):
         check_error(libfile.capy_type3_shading_destroy(self))
 
 
 class Type4Shading:
     def __init__(self, cs, minx, miny, maxx, maxy):
         t4s = ctypes.c_void_p()
-        check_error(libfile.capy_type4_shading_new(ctypes.pointer(t4s), cs.value,
-                    minx, miny, maxx, maxy))
+        check_error(libfile.capy_type4_shading_new(cs.value,
+                    minx, miny, maxx, maxy, ctypes.pointer(t4s)))
         self._as_parameter_ = t4s
 
     def __del__(self):
         check_error(libfile.capy_type4_shading_destroy(self))
 
     def add_triangle(self, coords, colors):
         if len(coords) != 6:
@@ -1121,16 +1247,16 @@
         else:
             raise CapyPDFException(f'Bad flag value {flag}')
 
 
 class Type6Shading:
     def __init__(self, cs, minx, miny, maxx, maxy):
         t6s = ctypes.c_void_p()
-        check_error(libfile.capy_type6_shading_new(ctypes.pointer(t6s), cs.value,
-                    minx, miny, maxx, maxy))
+        check_error(libfile.capy_type6_shading_new(cs.value,
+                    minx, miny, maxx, maxy, ctypes.pointer(t6s)))
         self._as_parameter_ = t6s
 
     def __del__(self):
         check_error(libfile.capy_type6_shading_destroy(self))
 
     def add_patch(self, coords, colors):
         if len(coords) != 24:
@@ -1162,14 +1288,19 @@
 
     def __del__(self):
         check_error(libfile.capy_annotation_destroy(self))
 
     def set_rectangle(self, x1, y1, x2, y2):
         check_error(libfile.capy_annotation_set_rectangle(self, x1, y1, x2, y2))
 
+    def set_flags(self, flags):
+        if not isinstance(flags, AnnotationFlag):
+            raise CapyPDFException('Flag argument is not an AnnotationFlag.')
+        check_error(libfile.capy_annotation_set_flags(self, flags.value ))
+
     @classmethod
     def new_text_annotation(cls, text):
         ta = ctypes.c_void_p()
         check_error(libfile.capy_text_annotation_new(text.encode('utf-8'), ctypes.pointer(ta)))
         return Annotation(ta)
 
     @classmethod
```

### Comparing `capypdf-0.8.0/readme.md` & `capypdf-0.9.0/readme.md`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/errorhandling.cpp` & `capypdf-0.9.0/src/errorhandling.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 "Color spaces are not of the same type.",
 "Boolean integer value must be 0 or 1.",
 "Gradient must start with a full patch.",
 "Object created for one document used with a different document",
 "Argument must be ASCII.",
 "File does not exist.",
 "Annotation is missing location rectangle.",
-"BMC argument must be of the form \"/name\"",
+"Argument must not start with a slash or be empty.",
+"Nesting marked content is forbidden.",
+"Rolemap entry is already defined.",
 };
 
 // clang-format on
 
 const char *error_text(ErrorCode ec) noexcept {
     const int index = (int32_t)ec;
     if(index < 0 || (std::size_t)index >= error_texts.size()) {
```

### Comparing `capypdf-0.8.0/src/errorhandling.hpp` & `capypdf-0.9.0/src/errorhandling.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     ColorspaceMismatch,
     BadBoolean,
     BadStripStart,
     IncorrectDocumentForObject,
     NotASCII,
     FileDoesNotExist,
     AnnotationMissingRect,
-    BadBMC,
+    SlashStart,
+    NestedBMC,
+    RoleAlreadyDefined,
     // When you add an error code here, also add the string representation in the .cpp file.
     NumErrors,
 };
 
 const char *error_text(ErrorCode ec) noexcept;
 
 [[noreturn]] void printandabort(ErrorCode ec) noexcept;
```

### Comparing `capypdf-0.8.0/src/fembedtest.cpp` & `capypdf-0.9.0/src/fembedtest.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/fontgen.cpp` & `capypdf-0.9.0/src/fontgen.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/fontsubsetter.cpp` & `capypdf-0.9.0/src/fontsubsetter.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/fontsubsetter.hpp` & `capypdf-0.9.0/src/fontsubsetter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/fonttester.cpp` & `capypdf-0.9.0/src/fonttester.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/formtest.cpp` & `capypdf-0.9.0/src/formtest.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/formxobj.cpp` & `capypdf-0.9.0/src/formxobj.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/ft_subsetter.cpp` & `capypdf-0.9.0/src/ft_subsetter.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/ft_subsetter.hpp` & `capypdf-0.9.0/src/ft_subsetter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/imagefileops.cpp` & `capypdf-0.9.0/src/imagefileops.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/labtest.cpp` & `capypdf-0.9.0/src/labtest.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/loremipsum.cpp` & `capypdf-0.9.0/src/loremipsum.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             fprintf(stderr, "%s\n", error_text(rc.error()));                                       \
             std::abort();                                                                          \
         }                                                                                          \
     }
 
 namespace {
 
-CapyPDF_StructureItemId document_root;
+CapyPDF_StructureItemId document_root_item;
 
 // #define YOLO
 
 #ifdef YOLO
 const std::vector<std::string> column1{
     "Lorem ipsum dolor sit amet, consectetur",
 };
@@ -146,17 +146,16 @@
                    double column_left,
                    double column_top) {
     const double target_width = cm2pt(8);
     auto textobj = PdfText(&ctx);
     CHCK(textobj.cmd_Tf(textfont, textsize));
     CHCK(textobj.cmd_Td(column_left, column_top));
     CHCK(textobj.cmd_TL(leading));
-    CHCK(textobj.cmd_BDC(
-        asciistring::from_cstr("Document").value(),
-        gen.add_structure_item(asciistring::from_cstr("Document").value(), document_root).value()));
+    CHCK(
+        textobj.cmd_BDC(gen.add_structure_item(CAPY_STRUCTURE_TYPE_P, document_root_item).value()));
     for(size_t i = 0; i < text_lines.size(); ++i) {
         const auto l = u8string::from_cstr(text_lines[i]).value();
         if(i + 1 < text_lines.size() && text_lines[i + 1].empty()) {
             CHCK(textobj.cmd_Tw(0));
             CHCK(textobj.render_text(l));
             CHCK(textobj.cmd_Tstar());
         } else {
@@ -166,17 +165,15 @@
                 const int ns = num_spaces(l.sv());
                 const double word_spacing = ns != 0 ? extra_w / ns : 0;
                 CHCK(textobj.cmd_Tw(word_spacing));
                 CHCK(textobj.render_text(l));
             } else {
                 CHCK(textobj.cmd_EMC());
                 CHCK(textobj.cmd_BDC(
-                    asciistring::from_cstr("P").value(),
-                    gen.add_structure_item(asciistring::from_cstr("P").value(), document_root)
-                        .value()));
+                    gen.add_structure_item(CAPY_STRUCTURE_TYPE_P, document_root_item).value()));
             }
             CHCK(textobj.cmd_Tstar());
         }
     }
     CHCK(textobj.cmd_EMC());
     CHCK(ctx.render_text(textobj));
 }
@@ -185,26 +182,23 @@
     auto titlefont = gen.load_font("/usr/share/fonts/truetype/noto/NotoSans-Bold.ttf").value();
     auto authorfont = gen.load_font("/usr/share/fonts/truetype/noto/NotoSans-Regular.ttf").value();
     const double titley = cm2pt(29 - 2.5);
     const double authory = cm2pt(29 - 3.5);
     const double titlesize = 28;
     const double authorsize = 18;
 
-    CHCK(ctx.cmd_BDC(
-        asciistring::from_cstr("P").value(),
-        gen.add_structure_item(asciistring::from_cstr("Title").value(), document_root).value()));
+    auto title_item = gen.add_structure_item(CAPY_STRUCTURE_TYPE_H1, document_root_item).value();
+    CHCK(ctx.cmd_BDC(title_item));
     CHCK(ctx.render_text(title,
                          titlefont,
                          titlesize,
                          midx - text_width(title.sv(), gen, titlefont, titlesize) / 2,
                          titley));
     CHCK(ctx.cmd_EMC());
-    CHCK(ctx.cmd_BDC(
-        asciistring::from_cstr("H2").value(),
-        gen.add_structure_item(asciistring::from_cstr("Author").value(), document_root).value()));
+    CHCK(ctx.cmd_BDC(gen.add_structure_item(CAPY_STRUCTURE_TYPE_H2, document_root_item).value()));
     CHCK(ctx.render_text(author,
                          authorfont,
                          authorsize,
                          midx - text_width(author.sv(), gen, authorfont, authorsize) / 2,
                          authory));
     CHCK(ctx.cmd_EMC());
 }
@@ -232,17 +226,15 @@
     CHCK(ctx.cmd_EMC());
 }
 
 void draw_email(PdfGen &gen, PdfDrawContext &ctx) {
     auto emailfont = gen.load_font("/usr/share/fonts/truetype/noto/NotoMono-Regular.ttf").value();
     const double emailsize = 16;
     const double emaily = cm2pt(29 - 4.3);
-    CHCK(ctx.cmd_BDC(
-        asciistring::from_cstr("H3").value(),
-        gen.add_structure_item(asciistring::from_cstr("Email").value(), document_root).value()));
+    CHCK(ctx.cmd_BDC(gen.add_structure_item(CAPY_STRUCTURE_TYPE_H3, document_root_item).value()));
     CHCK(ctx.render_text(email,
                          emailfont,
                          emailsize,
                          midx - text_width(email.sv(), gen, emailfont, emailsize) / 2,
                          emaily));
     CHCK(ctx.cmd_EMC());
 }
@@ -253,13 +245,13 @@
     opts.lang = asciistring::from_cstr("en-US").value();
     GenPopper genpop("loremipsum.pdf", opts);
     PdfGen &gen = *genpop.g;
 
     auto ctxguard = gen.guarded_page_context();
     auto &ctx = ctxguard.ctx;
 
-    document_root = gen.add_structure_item(asciistring::from_cstr("Document").value(), {}).value();
+    document_root_item = gen.add_structure_item(CAPY_STRUCTURE_TYPE_DOCUMENT, {}).value();
     draw_headings(gen, ctx);
     draw_email(gen, ctx);
     draw_maintext(gen, ctx);
     return 0;
 }
```

### Comparing `capypdf-0.8.0/src/meson.build` & `capypdf-0.9.0/src/meson.build`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   #link_args: ['-static-libstdc++'],
   cpp_args: cpp_args,
   dependencies: capydeps,
   gnu_symbol_visibility: 'inlineshidden',
   version: version,
   soversion: soversion,
   install: true,
+  cpp_pch: 'pch/capypch.hpp',
 )
 
 capypdf_dep = declare_dependency(include_directories: pubinc,
   link_with: capypdf_lib,
 )
 
 capypdf_internal_dep = declare_dependency(include_directories: pubinc,
```

### Comparing `capypdf-0.8.0/src/pdfcapi.cpp` & `capypdf-0.9.0/src/pdfcapi.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -154,274 +154,339 @@
     if(!props->mediabox) {
         return conv_err(ErrorCode::MissingMediabox);
     }
     opts->default_page_properties = *props;
     RETNOERR;
 }
 
+CAPYPDF_PUBLIC CapyPDF_EC capy_options_set_tagged(CapyPDF_Options *opt,
+                                                  int32_t is_tagged) CAPYPDF_NOEXCEPT {
+    CHECK_BOOLEAN(is_tagged);
+    auto opts = reinterpret_cast<PdfGenerationData *>(opt);
+    opts->is_tagged = is_tagged;
+    RETNOERR;
+}
+
 CapyPDF_EC capy_generator_new(const char *filename,
                               const CapyPDF_Options *options,
                               CapyPDF_Generator **out_ptr) CAPYPDF_NOEXCEPT {
     CHECK_NULL(filename);
     CHECK_NULL(options);
     CHECK_NULL(out_ptr);
     auto opts = reinterpret_cast<const PdfGenerationData *>(options);
     auto rc = PdfGen::construct(filename, *opts);
     if(rc) {
         *out_ptr = reinterpret_cast<CapyPDF_Generator *>(rc.value().release());
     }
     return conv_err(rc);
 }
 
-CapyPDF_EC capy_generator_add_page(CapyPDF_Generator *g,
-                                   CapyPDF_DrawContext *dctx) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto *ctx = reinterpret_cast<PdfDrawContext *>(dctx);
+CapyPDF_EC capy_generator_add_page(CapyPDF_Generator *gen,
+                                   CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto *dc = reinterpret_cast<PdfDrawContext *>(ctx);
 
-    auto rc = gen->add_page(*ctx);
+    auto rc = g->add_page(*dc);
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_form_xobject(
-    CapyPDF_Generator *g, CapyPDF_DrawContext *dctx, CapyPDF_FormXObjectId *fxid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto *ctx = reinterpret_cast<PdfDrawContext *>(dctx);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_form_xobject(CapyPDF_Generator *gen,
+                                                          CapyPDF_DrawContext *ctx,
+                                                          CapyPDF_FormXObjectId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto *dc = reinterpret_cast<PdfDrawContext *>(ctx);
 
-    auto rc = gen->add_form_xobject(*ctx);
+    auto rc = g->add_form_xobject(*dc);
     if(rc) {
-        *fxid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_color_pattern(
-    CapyPDF_Generator *g, CapyPDF_DrawContext *ctx, CapyPDF_PatternId *pid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto *colorctx = reinterpret_cast<PdfDrawContext *>(ctx);
-    auto rc = gen->add_pattern(*colorctx);
+    CapyPDF_Generator *gen, CapyPDF_DrawContext *ctx, CapyPDF_PatternId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto *colordc = reinterpret_cast<PdfDrawContext *>(ctx);
+    auto rc = g->add_pattern(*colordc);
     if(rc) {
-        *pid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_jpg(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_jpg(CapyPDF_Generator *gen,
                                                    const char *fname,
                                                    CapyPDF_Image_Interpolation interpolate,
-                                                   CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->embed_jpg(fname, interpolate);
+                                                   CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->embed_jpg(fname, interpolate);
     if(rc) {
-        *iid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_file(CapyPDF_Generator *g,
-                                                    const char *fname,
-                                                    CapyPDF_EmbeddedFileId *fid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->embed_file(fname);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_embed_file(
+    CapyPDF_Generator *gen, const char *fname, CapyPDF_EmbeddedFileId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->embed_file(fname);
     if(rc) {
-        *fid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_font(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_font(CapyPDF_Generator *gen,
                                                    const char *fname,
-                                                   CapyPDF_FontId *fid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->load_font(fname);
+                                                   CapyPDF_FontId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->load_font(fname);
     if(rc) {
-        *fid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_image(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_image(CapyPDF_Generator *gen,
                                                     const char *fname,
                                                     CapyPDF_Image_Interpolation interpolate,
-                                                    CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->load_image(fname, interpolate);
+                                                    CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->load_image(fname, interpolate);
     if(rc) {
-        *iid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_mask_image(CapyPDF_Generator *g,
-                                                         const char *fname,
-                                                         CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->load_mask_image(fname);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_mask_image(
+    CapyPDF_Generator *gen, const char *fname, CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->load_mask_image(fname);
     if(rc) {
-        *iid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_image(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_image(CapyPDF_Generator *gen,
                                                    CapyPDF_RasterImage *image,
-                                                   CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+                                                   CapyPDF_ImageId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *im = reinterpret_cast<RasterImage *>(image);
-    auto rc = gen->add_image(std::move(*im));
+    auto rc = g->add_image(std::move(*im));
     if(rc) {
-        *iid = rc.value();
+        *out_ptr = rc.value();
     }
     *im = RasterImage{};
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_function(
-    CapyPDF_Generator *g, CapyPDF_Type2Function *func, CapyPDF_FunctionId *fid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_function(CapyPDF_Generator *gen,
+                                                            CapyPDF_Type2Function *func,
+                                                            CapyPDF_FunctionId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *f = reinterpret_cast<FunctionType2 *>(func);
-    auto rc = gen->add_function(*f);
+    auto rc = g->add_function(*f);
     if(rc) {
-        *fid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_shading(
-    CapyPDF_Generator *g, CapyPDF_Type2Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type2_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type2Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *sh = reinterpret_cast<ShadingType2 *>(shade);
-    auto rc = gen->add_shading(*sh);
+    auto rc = g->add_shading(*sh);
     if(rc) {
-        *shid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type3_shading(
-    CapyPDF_Generator *g, CapyPDF_Type3Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type3_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type3Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *sh = reinterpret_cast<ShadingType3 *>(shade);
-    auto rc = gen->add_shading(*sh);
+    auto rc = g->add_shading(*sh);
     if(rc) {
-        *shid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type4_shading(
-    CapyPDF_Generator *g, CapyPDF_Type4Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type4_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type4Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *sh = reinterpret_cast<ShadingType4 *>(shade);
-    auto rc = gen->add_shading(*sh);
+    auto rc = g->add_shading(*sh);
     if(rc) {
-        *shid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type6_shading(
-    CapyPDF_Generator *g, CapyPDF_Type6Shading *shade, CapyPDF_ShadingId *shid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_type6_shading(CapyPDF_Generator *gen,
+                                                           CapyPDF_Type6Shading *shade,
+                                                           CapyPDF_ShadingId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *sh = reinterpret_cast<ShadingType6 *>(shade);
-    auto rc = gen->add_shading(*sh);
+    auto rc = g->add_shading(*sh);
     if(rc) {
-        *shid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_graphics_state(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_graphics_state(CapyPDF_Generator *gen,
                                                             const CapyPDF_GraphicsState *state,
-                                                            CapyPDF_GraphicsStateId *gsid)
+                                                            CapyPDF_GraphicsStateId *out_ptr)
     CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *s = reinterpret_cast<const GraphicsState *>(state);
-    auto rc = gen->add_graphics_state(*s);
+    auto rc = g->add_graphics_state(*s);
+    if(rc) {
+        *out_ptr = rc.value();
+    }
+    return conv_err(rc);
+}
+
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_structure_item(CapyPDF_Generator *gen,
+                                                            const CapyPDF_StructureType stype,
+                                                            const CapyPDF_StructureItemId *parent,
+                                                            CapyPDF_StructureItemId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    std::optional<CapyPDF_StructureItemId> item_parent;
+    if(parent) {
+        item_parent = *parent;
+    }
+    auto rc = g->add_structure_item(stype, item_parent);
+    if(rc) {
+        *out_ptr = rc.value();
+    }
+    return conv_err(rc);
+}
+
+CAPYPDF_PUBLIC CapyPDF_EC
+capy_generator_add_custom_structure_item(CapyPDF_Generator *gen,
+                                         const CapyPDF_RoleId role,
+                                         const CapyPDF_StructureItemId *parent,
+                                         CapyPDF_StructureItemId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    std::optional<CapyPDF_StructureItemId> item_parent;
+    if(parent) {
+        item_parent = *parent;
+    }
+    auto rc = g->add_structure_item(role, item_parent);
     if(rc) {
-        *gsid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_load_icc_profile(
-    CapyPDF_Generator *g, const char *fname, CapyPDF_IccColorSpaceId *iid) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    auto rc = gen->load_icc_file(fname);
+    CapyPDF_Generator *gen, const char *fname, CapyPDF_IccColorSpaceId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->load_icc_file(fname);
     if(rc) {
-        *iid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_separation_simple(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_separation_simple(CapyPDF_Generator *gen,
                                                                   const char *separation_name,
                                                                   const CapyPDF_Color *c,
-                                                                  CapyPDF_SeparationId *sid)
+                                                                  CapyPDF_SeparationId *out_ptr)
     CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     const auto *color = reinterpret_cast<const Color *>(c);
     auto name = asciistring::from_cstr(separation_name);
     if(!name) {
         return conv_err(name);
     }
     if(!std::holds_alternative<DeviceCMYKColor>(*color)) {
         return conv_err(ErrorCode::ColorspaceMismatch);
     }
     const auto &cmyk = std::get<DeviceCMYKColor>(*color);
-    auto rc = gen->create_separation(name.value(), cmyk);
+    auto rc = g->create_separation(name.value(), cmyk);
     if(rc) {
-        *sid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CapyPDF_EC capy_generator_write(CapyPDF_Generator *generator) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+CapyPDF_EC capy_generator_write(CapyPDF_Generator *gen) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto rc = g->write();
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC
-capy_generator_add_optional_content_group(CapyPDF_Generator *generator,
-                                          const CapyPDF_OptionalContentGroup *ocg,
-                                          CapyPDF_OptionalContentGroupId *ocgid) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_optional_content_group(
+    CapyPDF_Generator *gen,
+    const CapyPDF_OptionalContentGroup *ocg,
+    CapyPDF_OptionalContentGroupId *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     const auto *group = reinterpret_cast<const OptionalContentGroup *>(ocg);
     auto rc = g->add_optional_content_group(*group);
     if(rc) {
-        *ocgid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_generator_create_annotation(CapyPDF_Generator *gen,
                                                            CapyPDF_Annotation *annotation,
-                                                           CapyPDF_AnnotationId *aid)
+                                                           CapyPDF_AnnotationId *out_ptr)
     CAPYPDF_NOEXCEPT {
     auto *g = reinterpret_cast<PdfGen *>(gen);
     auto *a = reinterpret_cast<Annotation *>(annotation);
     auto rc = g->create_annotation(*a);
     if(rc) {
-        *aid = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CapyPDF_EC capy_generator_destroy(CapyPDF_Generator *generator) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_rolemap_entry(CapyPDF_Generator *gen,
+                                                           const char *name,
+                                                           CapyPDF_StructureType builtin,
+                                                           CapyPDF_RoleId *out_ptr)
+    CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    auto rc = g->add_rolemap_entry(name, builtin);
+    if(rc) {
+        *out_ptr = rc.value();
+    }
+    return conv_err(rc);
+}
+
+CapyPDF_EC capy_generator_destroy(CapyPDF_Generator *gen) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     delete g;
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_outline(CapyPDF_Generator *generator,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_add_outline(CapyPDF_Generator *gen,
                                                      const char *utf8_text,
                                                      int32_t page_number,
                                                      CapyPDF_OutlineId *parent,
                                                      CapyPDF_OutlineId *out_ptr) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto u8t = u8string::from_cstr(utf8_text);
     if(!u8t) {
         return conv_err(u8t);
     }
     if(page_number < 0 || page_number >= g->num_pages()) {
         return conv_err(ErrorCode::IndexOutOfBounds);
     }
@@ -433,154 +498,160 @@
     auto rc = g->add_outline(u8t.value(), page_id, pobj);
     if(rc) {
         *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_generator_text_width(CapyPDF_Generator *generator,
+CAPYPDF_PUBLIC CapyPDF_EC capy_generator_text_width(CapyPDF_Generator *gen,
                                                     const char *utf8_text,
                                                     CapyPDF_FontId font,
                                                     double pointsize,
-                                                    double *width) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+                                                    double *out_ptr) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     auto u8t = u8string::from_cstr(utf8_text);
     if(!u8t) {
         return conv_err(u8t);
     }
     auto rc = g->utf8_text_width(u8t.value(), font, pointsize);
     if(rc) {
-        *width = rc.value();
+        *out_ptr = rc.value();
     }
     return conv_err(rc);
 }
 
 // Draw Context
 
-CapyPDF_EC capy_page_draw_context_new(CapyPDF_Generator *g,
+CapyPDF_EC capy_page_draw_context_new(CapyPDF_Generator *gen,
                                       CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(gen->new_page_draw_context());
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(g->new_page_draw_context());
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_b(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_b());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_b());
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_B(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_B());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_B());
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_bstar());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_bstar());
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_Bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_Bstar());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_Bstar());
+}
+
+CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BDC_builtin(
+    CapyPDF_DrawContext *ctx, CapyPDF_StructureItemId structid) CAPYPDF_NOEXCEPT {
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_BDC(structid));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BDC_ocg(
     CapyPDF_DrawContext *ctx, CapyPDF_OptionalContentGroupId ocgid) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_BDC(ocgid));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_BDC(ocgid));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_BMC(CapyPDF_DrawContext *ctx,
                                           const char *tag) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_BMC(tag));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_BMC(tag));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_c(CapyPDF_DrawContext *ctx,
                                         double x1,
                                         double y1,
                                         double x2,
                                         double y2,
                                         double x3,
                                         double y3) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_c(x1, y1, x2, y2, x3, y3));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_c(x1, y1, x2, y2, x3, y3));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_cm(CapyPDF_DrawContext *ctx,
                                          double m1,
                                          double m2,
                                          double m3,
                                          double m4,
                                          double m5,
                                          double m6) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_cm(m1, m2, m3, m4, m5, m6));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_cm(m1, m2, m3, m4, m5, m6));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_d(CapyPDF_DrawContext *ctx,
                                         double *dash_array,
                                         int32_t array_size,
                                         double phase) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_d(dash_array, array_size, phase));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_d(dash_array, array_size, phase));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_EMC(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_EMC());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_EMC());
 }
 
 CapyPDF_EC capy_dc_cmd_f(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_f());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_f());
 }
 
 CapyPDF_EC capy_dc_cmd_fstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_fstar());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_fstar());
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_G(CapyPDF_DrawContext *ctx, double gray) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_G(gray));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_G(gray));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_g(CapyPDF_DrawContext *ctx, double gray) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_g(gray));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_g(gray));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_gs(CapyPDF_DrawContext *ctx,
                                          CapyPDF_GraphicsStateId gsid) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_gs(gsid));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_gs(gsid));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_h(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_h());
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_h());
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_i(CapyPDF_DrawContext *ctx,
                                         double flatness) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_i(flatness));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_i(flatness));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_j(CapyPDF_DrawContext *ctx,
                                         CapyPDF_Line_Join join_style) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_j(join_style));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_j(join_style));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_J(CapyPDF_DrawContext *ctx,
                                         CapyPDF_Line_Cap cap_style) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_J(cap_style));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_J(cap_style));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC
 capy_dc_cmd_k(CapyPDF_DrawContext *ctx, double c, double m, double y, double k) CAPYPDF_NOEXCEPT {
     auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     return conv_err(dc->cmd_k(c, m, y, k));
 }
@@ -590,16 +661,16 @@
     auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     return conv_err(dc->cmd_K(c, m, y, k));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_l(CapyPDF_DrawContext *ctx,
                                         double x,
                                         double y) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return conv_err(c->cmd_l(x, y));
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->cmd_l(x, y));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_cmd_m(CapyPDF_DrawContext *ctx,
                                         double x,
                                         double y) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return conv_err(c->cmd_m(x, y));
@@ -730,47 +801,47 @@
                                                   CapyPDF_Text *text) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     auto t = reinterpret_cast<PdfText *>(text);
     return conv_err(c->render_text(*t));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_set_page_transition(
-    CapyPDF_DrawContext *dc, CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT {
-    auto ctx = reinterpret_cast<PdfDrawContext *>(dc);
+    CapyPDF_DrawContext *ctx, CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT {
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     auto t = reinterpret_cast<Transition *>(transition);
-    auto rc = ctx->set_transition(*t);
+    auto rc = dc->set_transition(*t);
     return conv_err(rc);
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_set_custom_page_properties(
-    CapyPDF_DrawContext *dc, const CapyPDF_PageProperties *custom_properties) {
+    CapyPDF_DrawContext *ctx, const CapyPDF_PageProperties *custom_properties) {
     CHECK_NULL(custom_properties);
-    auto *ctx = reinterpret_cast<PdfDrawContext *>(dc);
+    auto *dc = reinterpret_cast<PdfDrawContext *>(ctx);
     auto *cprop = reinterpret_cast<const PageProperties *>(custom_properties);
-    return conv_err(ctx->set_custom_page_properties(*cprop));
+    return conv_err(dc->set_custom_page_properties(*cprop));
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_dc_annotate(CapyPDF_DrawContext *dc,
+CAPYPDF_PUBLIC CapyPDF_EC capy_dc_annotate(CapyPDF_DrawContext *ctx,
                                            CapyPDF_AnnotationId aid) CAPYPDF_NOEXCEPT {
-    auto *ctx = reinterpret_cast<PdfDrawContext *>(dc);
-    return conv_err(ctx->annotate(aid));
+    auto *dc = reinterpret_cast<PdfDrawContext *>(ctx);
+    return conv_err(dc->annotate(aid));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC
-capy_dc_add_simple_navigation(CapyPDF_DrawContext *dc,
+capy_dc_add_simple_navigation(CapyPDF_DrawContext *ctx,
                               const CapyPDF_OptionalContentGroupId *ocgarray,
                               int32_t array_size,
                               const CapyPDF_Transition *tr) CAPYPDF_NOEXCEPT {
-    auto ctx = reinterpret_cast<PdfDrawContext *>(dc);
+    auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     std::optional<Transition> transition;
     if(tr) {
         transition = *reinterpret_cast<const Transition *>(tr);
     }
     std::span<const CapyPDF_OptionalContentGroupId> ocgspan(ocgarray, ocgarray + array_size);
-    auto rc = ctx->add_simple_navigation(ocgspan, transition);
+    auto rc = dc->add_simple_navigation(ocgspan, transition);
     return conv_err(rc);
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_dc_text_new(CapyPDF_DrawContext *dc,
                                            CapyPDF_Text **out_ptr) CAPYPDF_NOEXCEPT {
     CHECK_NULL(dc);
     *out_ptr = reinterpret_cast<CapyPDF_Text *>(
@@ -779,28 +850,28 @@
 }
 
 CapyPDF_EC capy_dc_destroy(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<PdfDrawContext *>(ctx);
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_form_xobject_new(CapyPDF_Generator *g,
+CAPYPDF_PUBLIC CapyPDF_EC capy_form_xobject_new(CapyPDF_Generator *gen,
                                                 double w,
                                                 double h,
                                                 CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT {
-    auto *gen = reinterpret_cast<PdfGen *>(g);
-    *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(gen->new_form_xobject(w, h));
+    auto *g = reinterpret_cast<PdfGen *>(gen);
+    *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(g->new_form_xobject(w, h));
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_color_pattern_context_new(CapyPDF_Generator *generator,
+CAPYPDF_PUBLIC CapyPDF_EC capy_color_pattern_context_new(CapyPDF_Generator *gen,
                                                          CapyPDF_DrawContext **out_ptr,
                                                          double w,
                                                          double h) CAPYPDF_NOEXCEPT {
-    auto *g = reinterpret_cast<PdfGen *>(generator);
+    auto *g = reinterpret_cast<PdfGen *>(gen);
     *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(g->new_color_pattern(w, h));
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_render_text(CapyPDF_Text *text,
                                                 const char *utf8_text) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
@@ -821,14 +892,25 @@
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_set_stroke(CapyPDF_Text *text,
                                                const CapyPDF_Color *color) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     const auto *c = reinterpret_cast<const Color *>(color);
     return conv_err(t->stroke_color(*c));
 }
 
+CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_BDC_builtin(CapyPDF_Text *text,
+                                                    CapyPDF_StructureItemId stid) CAPYPDF_NOEXCEPT {
+    auto *t = reinterpret_cast<PdfText *>(text);
+    return conv_err(t->cmd_BDC(stid));
+}
+
+CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_EMC(CapyPDF_Text *text) CAPYPDF_NOEXCEPT {
+    auto *t = reinterpret_cast<PdfText *>(text);
+    return conv_err(t->cmd_EMC());
+}
+
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Tc(CapyPDF_Text *text, double spacing) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     return conv_err(t->cmd_Tc(spacing));
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_text_cmd_Td(CapyPDF_Text *text,
                                            double x,
@@ -1063,61 +1145,62 @@
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_raster_image_destroy(CapyPDF_RasterImage *image) CAPYPDF_NOEXCEPT {
     auto *ri = reinterpret_cast<RasterImage *>(image);
     delete ri;
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_new(CapyPDF_Type2Function **out_ptr,
-                                                  double *domain,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_new(double *domain,
                                                   int32_t domain_size,
                                                   const CapyPDF_Color *c1,
                                                   const CapyPDF_Color *c2,
-                                                  double n) CAPYPDF_NOEXCEPT {
+                                                  double n,
+                                                  CapyPDF_Type2Function **out_ptr)
+    CAPYPDF_NOEXCEPT {
     *out_ptr = reinterpret_cast<CapyPDF_Type2Function *>(
         new FunctionType2{std::vector<double>(domain, domain + domain_size),
                           *reinterpret_cast<const Color *>(c1),
                           *reinterpret_cast<const Color *>(c2),
                           n});
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type2_function_destroy(CapyPDF_Type2Function *func)
     CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<FunctionType2 *>(func);
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_new(CapyPDF_Type2Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_new(CapyPDF_Colorspace cs,
                                                  double x0,
                                                  double y0,
                                                  double x1,
                                                  double y1,
                                                  CapyPDF_FunctionId func,
                                                  int32_t extend1,
-                                                 int32_t extend2) CAPYPDF_NOEXCEPT {
+                                                 int32_t extend2,
+                                                 CapyPDF_Type2Shading **out_ptr) CAPYPDF_NOEXCEPT {
     CHECK_BOOLEAN(extend1);
     CHECK_BOOLEAN(extend2);
     *out_ptr = reinterpret_cast<CapyPDF_Type2Shading *>(
         new ShadingType2{cs, x0, y0, x1, y1, func, extend1 != 0, extend2 != 0});
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type2_shading_destroy(CapyPDF_Type2Shading *shade) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<ShadingType2 *>(shade);
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_new(CapyPDF_Type3Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_new(CapyPDF_Colorspace cs,
                                                  double *coords,
                                                  CapyPDF_FunctionId func,
                                                  int32_t extend1,
-                                                 int32_t extend2) CAPYPDF_NOEXCEPT {
+                                                 int32_t extend2,
+                                                 CapyPDF_Type3Shading **out_ptr) CAPYPDF_NOEXCEPT {
     CHECK_BOOLEAN(extend1);
     CHECK_BOOLEAN(extend2);
     *out_ptr = reinterpret_cast<CapyPDF_Type3Shading *>(new ShadingType3{cs,
                                                                          coords[0],
                                                                          coords[1],
                                                                          coords[2],
                                                                          coords[3],
@@ -1130,56 +1213,57 @@
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type3_shading_destroy(CapyPDF_Type3Shading *shade) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<ShadingType3 *>(shade);
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_new(CapyPDF_Type4Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_new(CapyPDF_Colorspace cs,
                                                  double minx,
                                                  double miny,
                                                  double maxx,
-                                                 double maxy) CAPYPDF_NOEXCEPT {
+                                                 double maxy,
+                                                 CapyPDF_Type4Shading **out_ptr) CAPYPDF_NOEXCEPT {
     auto *shobj = new ShadingType4{};
     shobj->colorspace = cs;
     shobj->minx = minx;
     shobj->miny = miny;
     shobj->maxx = maxx;
     shobj->maxy = maxy;
     *out_ptr = reinterpret_cast<CapyPDF_Type4Shading *>(shobj);
     RETNOERR;
 }
 
-static ShadingPoint conv_shpoint(double *coords, Color *color) {
+static ShadingPoint conv_shpoint(const double *coords, const Color *color) {
     ShadingPoint sp;
     sp.c = *color;
     sp.p.x = coords[0];
     sp.p.y = coords[1];
     return sp;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_add_triangle(CapyPDF_Type4Shading *shade,
-                                                          double *coords,
-                                                          CapyPDF_Color **color) CAPYPDF_NOEXCEPT {
+                                                          const double *coords,
+                                                          const CapyPDF_Color **color)
+    CAPYPDF_NOEXCEPT {
     auto *sh = reinterpret_cast<ShadingType4 *>(shade);
-    auto *cc = reinterpret_cast<Color **>(color);
+    auto *cc = reinterpret_cast<const Color **>(color);
     ShadingPoint sp1 = conv_shpoint(coords, cc[0]);
     ShadingPoint sp2 = conv_shpoint(coords + 2, cc[1]);
     ShadingPoint sp3 = conv_shpoint(coords + 4, cc[2]);
     sh->start_strip(sp1, sp2, sp3);
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_extend(CapyPDF_Type4Shading *shade,
                                                     int32_t flag,
-                                                    double *coords,
-                                                    CapyPDF_Color *color) CAPYPDF_NOEXCEPT {
+                                                    const double *coords,
+                                                    const CapyPDF_Color *color) CAPYPDF_NOEXCEPT {
     auto *sh = reinterpret_cast<ShadingType4 *>(shade);
-    auto *cc = reinterpret_cast<Color *>(color);
+    auto *cc = reinterpret_cast<const Color *>(color);
     if(flag == 1 || flag == 2) {
         if(sh->elements.empty()) {
             conv_err(ErrorCode::BadStripStart);
         }
         ShadingPoint sp = conv_shpoint(coords, cc);
         sh->extend_strip(sp, flag);
     } else {
@@ -1189,57 +1273,59 @@
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type4_shading_destroy(CapyPDF_Type4Shading *shade) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<ShadingType4 *>(shade);
     RETNOERR;
 }
 
-CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_new(CapyPDF_Type6Shading **out_ptr,
-                                                 CapyPDF_Colorspace cs,
+CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_new(CapyPDF_Colorspace cs,
                                                  double minx,
                                                  double miny,
                                                  double maxx,
-                                                 double maxy) CAPYPDF_NOEXCEPT {
+                                                 double maxy,
+                                                 CapyPDF_Type6Shading **out_ptr) CAPYPDF_NOEXCEPT {
     auto *shobj = new ShadingType6{};
     shobj->colorspace = cs;
     shobj->minx = minx;
     shobj->miny = miny;
     shobj->maxx = maxx;
     shobj->maxy = maxy;
     *out_ptr = reinterpret_cast<CapyPDF_Type6Shading *>(shobj);
     RETNOERR;
 }
 
-template<typename T> static void grab_coons_data(T &patch, double *coords, Color **colors) {
+template<typename T>
+static void grab_coons_data(T &patch, const double *coords, const Color **colors) {
     for(int i = 0; i < (int)patch.p.size(); ++i) {
         patch.p[i].x = coords[2 * i];
         patch.p[i].y = coords[2 * i + 1];
     }
     for(int i = 0; i < (int)patch.c.size(); ++i) {
         patch.c[i] = *colors[i];
     }
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_add_patch(CapyPDF_Type6Shading *shade,
-                                                       double *coords,
-                                                       CapyPDF_Color **colors) CAPYPDF_NOEXCEPT {
+                                                       const double *coords,
+                                                       const CapyPDF_Color **colors)
+    CAPYPDF_NOEXCEPT {
     auto *sh = reinterpret_cast<ShadingType6 *>(shade);
-    auto **cc = reinterpret_cast<Color **>(colors);
+    auto **cc = reinterpret_cast<const Color **>(colors);
     FullCoonsPatch cp;
     grab_coons_data(cp, coords, cc);
     sh->elements.emplace_back(std::move(cp));
     RETNOERR;
 }
 
 CAPYPDF_PUBLIC CapyPDF_EC capy_type6_shading_extend(CapyPDF_Type6Shading *shade,
                                                     int32_t flag,
-                                                    double *coords,
-                                                    CapyPDF_Color **colors) CAPYPDF_NOEXCEPT {
+                                                    const double *coords,
+                                                    const CapyPDF_Color **colors) CAPYPDF_NOEXCEPT {
     auto *sh = reinterpret_cast<ShadingType6 *>(shade);
-    auto **cc = reinterpret_cast<Color **>(colors);
+    auto **cc = reinterpret_cast<const Color **>(colors);
     if(flag == 1 || flag == 2 || flag == 3) {
         if(sh->elements.empty()) {
             conv_err(ErrorCode::BadStripStart);
         }
         ContinuationCoonsPatch ccp;
         grab_coons_data(ccp, coords, cc);
         sh->elements.emplace_back(std::move(ccp));
@@ -1284,14 +1370,21 @@
 CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_set_rectangle(
     CapyPDF_Annotation *annotation, double x1, double y1, double x2, double y2) CAPYPDF_NOEXCEPT {
     auto *a = reinterpret_cast<Annotation *>(annotation);
     a->rect = PdfRectangle{x1, y1, x2, y2};
     RETNOERR;
 }
 
+CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_set_flags(
+    CapyPDF_Annotation *annotation, CapyPDF_AnnotationFlags flags) CAPYPDF_NOEXCEPT {
+    auto *a = reinterpret_cast<Annotation *>(annotation);
+    a->flags = flags;
+    RETNOERR;
+}
+
 CAPYPDF_PUBLIC CapyPDF_EC capy_annotation_destroy(CapyPDF_Annotation *annotation) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<Annotation *>(annotation);
     RETNOERR;
 }
 
 // Error handling.
```

### Comparing `capypdf-0.8.0/src/pdfcolorconverter.cpp` & `capypdf-0.9.0/src/pdfcolorconverter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                                     INTENT_SATURATION,
                                     INTENT_PERCEPTUAL};
 
 }
 
 namespace capypdf {
 
-
 LcmsHolder::~LcmsHolder() { deallocate(); }
 
 void LcmsHolder::deallocate() {
     if(h) {
         cmsCloseProfile(h);
     }
     h = nullptr;
```

### Comparing `capypdf-0.8.0/src/pdfcolorconverter.hpp` & `capypdf-0.9.0/src/pdfcolorconverter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/pdfcommon.cpp` & `capypdf-0.9.0/src/pdfcommon.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -28,14 +28,66 @@
     }
 
     return unpacked;
 }
 
 } // namespace
 
+const std::array<const char *, (int)CAPY_STRUCTURE_TYPE_NUM_ITEMS> structure_type_names{
+    // clang-format off
+    "Document",
+    "DocumentFragment",
+    "Part",
+    "Sect",
+    "Div",
+    "Aside",
+    "NonStruct",
+    "P",
+    "H",
+    "H1",
+    "H2",
+    "H3",
+    "H4",
+    "H5",
+    "H6",
+    "H7",
+    "Title",
+    "FENote",
+    "Sub",
+    "Lbl",
+    "Span",
+    "Em",
+    "Strong",
+    "Link",
+    "Annot",
+    "Form",
+    "Ruby",
+    "RB",
+    "RT",
+    "RP",
+    "Warichu",
+    "WT",
+    "WP",
+    "L",
+    "LI",
+    "LBody",
+    "Table",
+    "TR",
+    "TH",
+    "TD",
+    "THead",
+    "TBody",
+    "TFoot",
+    "Caption",
+    "Figure",
+    "Formula",
+    "Artifact",
+    // clang-format on
+};
+
 rvoe<asciistring> asciistring::from_cstr(const char *cstr) {
     if(!is_ascii(cstr)) {
         RETERR(NotASCII);
     }
     return asciistring(cstr);
 }
```

### Comparing `capypdf-0.8.0/src/pdfcommon.hpp` & `capypdf-0.9.0/src/pdfcommon.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 DEF_BASIC_OPERATORS(CapyPDF_OptionalContentGroupId);
 
 DEF_BASIC_OPERATORS(CapyPDF_TransparencyGroupId);
 
 namespace capypdf {
 
+extern const std::array<const char *, (int)CAPY_STRUCTURE_TYPE_NUM_ITEMS> structure_type_names;
+
 // Does not check if the given buffer is valid UTF-8.
 // If it is not, UB ensues.
 class CodepointIterator {
 public:
     struct CharInfo {
         uint32_t codepoint;
         uint32_t byte_count;
```

### Comparing `capypdf-0.8.0/src/pdfdocument.cpp` & `capypdf-0.9.0/src/pdfdocument.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 #include FT_FONT_FORMATS_H
 #include FT_OPENTYPE_VALIDATE_H
 
 namespace capypdf {
 
 namespace {
 
-std::array<const char *, 3> intentnames{"/GTS_PDFX", "/GTS_PDFA", "/ISO_PDFE"};
+const std::array<const char *, 3> intentnames{"/GTS_PDFX", "/GTS_PDFA", "/ISO_PDFE"};
 
-std::array<const char *, 12> transition_names{
+const std::array<const char *, 12> transition_names{
     "/Split",
     "/Blinds",
     "/Box",
     "/Wipe",
     "/Dissolve",
     "/Glitter",
     "/R",
@@ -205,37 +205,34 @@
         assert(flag >= 0 && flag < 3);
         const char *ptr;
         ptr = (const char *)(&flag);
         s.append(ptr, ptr + sizeof(char));
         ERCV(append_floatvalue<uint32_t>(s, xratio));
         ERCV(append_floatvalue<uint32_t>(s, yratio));
 
-        if(std::holds_alternative<DeviceRGBColor>(e.sp.c)) {
+        if(auto *c = std::get_if<DeviceRGBColor>(&e.sp.c)) {
             if(shade.colorspace != CAPY_CS_DEVICE_RGB) {
                 RETERR(ColorspaceMismatch);
             }
-            const auto &c = std::get<DeviceRGBColor>(e.sp.c);
-            ERCV(append_floatvalue<uint16_t>(s, c.r.v()));
-            ERCV(append_floatvalue<uint16_t>(s, c.g.v()));
-            ERCV(append_floatvalue<uint16_t>(s, c.b.v()));
-        } else if(std::holds_alternative<DeviceGrayColor>(e.sp.c)) {
+            ERCV(append_floatvalue<uint16_t>(s, c->r.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->g.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->b.v()));
+        } else if(auto *c = std::get_if<DeviceGrayColor>(&e.sp.c)) {
             if(shade.colorspace != CAPY_CS_DEVICE_GRAY) {
                 RETERR(ColorspaceMismatch);
             }
-            const auto &c = std::get<DeviceGrayColor>(e.sp.c);
-            ERCV(append_floatvalue<uint16_t>(s, c.v.v()));
-        } else if(std::holds_alternative<DeviceCMYKColor>(e.sp.c)) {
+            ERCV(append_floatvalue<uint16_t>(s, c->v.v()));
+        } else if(auto *c = std::get_if<DeviceCMYKColor>(&e.sp.c)) {
             if(shade.colorspace != CAPY_CS_DEVICE_CMYK) {
                 RETERR(ColorspaceMismatch);
             }
-            const auto &c = std::get<DeviceCMYKColor>(e.sp.c);
-            ERCV(append_floatvalue<uint16_t>(s, c.c.v()));
-            ERCV(append_floatvalue<uint16_t>(s, c.m.v()));
-            ERCV(append_floatvalue<uint16_t>(s, c.y.v()));
-            ERCV(append_floatvalue<uint16_t>(s, c.k.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->c.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->m.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->y.v()));
+            ERCV(append_floatvalue<uint16_t>(s, c->k.v()));
         } else {
             fprintf(stderr, "Color space not supported yet.");
             std::abort();
         }
     }
     return std::move(s);
 }
@@ -331,23 +328,20 @@
     case CAPY_CS_DEVICE_CMYK:
         return 4;
     }
     std::abort();
 }
 
 void color2numbers(std::back_insert_iterator<std::string> &app, const Color &c) {
-    if(std::holds_alternative<DeviceRGBColor>(c)) {
-        const auto &rgb = std::get<DeviceRGBColor>(c);
-        fmt::format_to(app, "{} {} {}", rgb.r.v(), rgb.g.v(), rgb.b.v());
-    } else if(std::holds_alternative<DeviceGrayColor>(c)) {
-        const auto &gray = std::get<DeviceGrayColor>(c);
-        fmt::format_to(app, "{}", gray.v.v());
-    } else if(std::holds_alternative<DeviceCMYKColor>(c)) {
-        const auto &cmyk = std::get<DeviceCMYKColor>(c);
-        fmt::format_to(app, "{} {} {} {}", cmyk.c.v(), cmyk.m.v(), cmyk.y.v(), cmyk.k.v());
+    if(auto *rgb = std::get_if<DeviceRGBColor>(&c)) {
+        fmt::format_to(app, "{} {} {}", rgb->r.v(), rgb->g.v(), rgb->b.v());
+    } else if(auto *gray = std::get_if<DeviceGrayColor>(&c)) {
+        fmt::format_to(app, "{}", gray->v.v());
+    } else if(auto *cmyk = std::get_if<DeviceCMYKColor>(&c)) {
+        fmt::format_to(app, "{} {} {} {}", cmyk->c.v(), cmyk->m.v(), cmyk->y.v(), cmyk->k.v());
     } else {
         fprintf(stderr, "Colorspace not supported yet.\n");
         std::abort();
     }
 }
 
 } // namespace
@@ -413,19 +407,20 @@
 int32_t PdfDocument::create_page_group() {
     std::string buf = fmt::format(R"(<<
   /S /Transparency
   /CS {}
 >>
 )",
                                   colorspace_names.at((int)opts.output_colorspace));
-    return add_object(FullPDFObject{std::move(buf), ""});
+    return add_object(FullPDFObject{std::move(buf), {}});
 }
 
-rvoe<NoReturnValue> PdfDocument::add_page(std::string resource_data,
-                                          std::string page_data,
+rvoe<NoReturnValue> PdfDocument::add_page(std::string resource_dict,
+                                          std::string unclosed_object_dict,
+                                          std::string command_stream,
                                           const PageProperties &custom_props,
                                           const std::unordered_set<CapyPDF_FormWidgetId> &fws,
                                           const std::unordered_set<CapyPDF_AnnotationId> &annots,
                                           const std::vector<CapyPDF_StructureItemId> &structs,
                                           const std::optional<Transition> &transition,
                                           const std::vector<SubPageNavigation> &subnav) {
     for(const auto &a : fws) {
@@ -439,16 +434,26 @@
         }
     }
     for(const auto &s : structs) {
         if(structure_use.find(s) != structure_use.cend()) {
             RETERR(StructureReuse);
         }
     }
-    const auto resource_num = add_object(FullPDFObject{std::move(resource_data), ""});
-    const auto commands_num = add_object(FullPDFObject{std::move(page_data), ""});
+    const auto resource_num = add_object(FullPDFObject{std::move(resource_dict), {}});
+    int32_t commands_num{-1};
+    if(opts.compress_streams) {
+        commands_num = add_object(
+            DeflatePDFObject{std::move(unclosed_object_dict), std::move(command_stream)});
+    } else {
+        fmt::format_to(std::back_inserter(unclosed_object_dict),
+                       "  /Length {}\n>>\n",
+                       command_stream.length());
+        commands_num =
+            add_object(FullPDFObject{std::move(unclosed_object_dict), std::move(command_stream)});
+    }
     DelayedPage p;
     p.page_num = (int32_t)pages.size();
     p.custom_props = custom_props;
     for(const auto &a : fws) {
         p.used_form_widgets.push_back(a);
     }
     for(const auto &a : annots) {
@@ -458,25 +463,26 @@
     if(!subnav.empty()) {
         p.subnav_root = create_subnavigation(subnav);
     }
     if(!structs.empty()) {
         p.structparents = (int32_t)structure_parent_tree_items.size();
         structure_parent_tree_items.push_back(structs);
     }
-    const auto page_num = add_object(std::move(p));
+    const auto page_object_num = add_object(std::move(p));
     for(const auto &fw : fws) {
-        form_use[fw] = page_num;
+        form_use[fw] = page_object_num;
     }
     for(const auto &a : annots) {
-        annotation_use[a] = page_num;
+        annotation_use[a] = page_object_num;
     }
+    int32_t mcid_num = 0;
     for(const auto &s : structs) {
-        structure_use[s] = page_num;
+        structure_use[s] = StructureUsage{(int32_t)pages.size(), mcid_num++};
     }
-    pages.emplace_back(PageOffsets{resource_num, commands_num, page_num});
+    pages.emplace_back(PageOffsets{resource_num, commands_num, page_object_num});
     return NoReturnValue{};
 }
 
 void PdfDocument::add_form_xobject(std::string xobj_dict, std::string xobj_stream) {
     const auto xobj_num = add_object(FullPDFObject{std::move(xobj_dict), std::move(xobj_stream)});
 
     form_xobjects.emplace_back(FormXObjectInfo{xobj_num});
@@ -505,15 +511,15 @@
 )";
         for(const auto &i : subnav) {
             fmt::format_to(rootapp, "      {} 0 R\n", ocg_object_number(i.id));
         }
         rootbuf += "    ]\n  >>\n";
         fmt::format_to(rootapp, "  /Prev {} 0 R\n>>\n", root_obj + 1 + subnav.size());
 
-        add_object(FullPDFObject{std::move(rootbuf), ""});
+        add_object(FullPDFObject{std::move(rootbuf), {}});
     }
     int32_t first_obj = document_objects.size();
 
     for(size_t i = 0; i < subnav.size(); ++i) {
         const auto &sn = subnav[i];
         std::string buf = R"(<<
   /Type /NavNode
@@ -542,28 +548,28 @@
     /State [ /OFF {} 0 R ]
   >>
 )",
                            ocg_object_number(subnav[i - 1].id));
             fmt::format_to(app, "  /Prev {} 0 R\n", first_obj + i - 1);
         }
         buf += ">>\n";
-        add_object(FullPDFObject{std::move(buf), ""});
+        add_object(FullPDFObject{std::move(buf), {}});
     }
     add_object(FullPDFObject{fmt::format(R"(<<
   /Type /NavNode
   /PA <<
     /S /SetOCGState
     /State [ /OFF {} 0 R ]
   >>
   /Prev {} 0 R
 >>
 )",
                                          ocg_object_number(subnav.back().id),
                                          first_obj + subnav.size() - 1),
-                             ""});
+                             {}});
     return root_obj;
 }
 
 int32_t PdfDocument::add_object(ObjectType object) {
     auto object_num = (int32_t)document_objects.size();
     document_objects.push_back(std::move(object));
     return object_num;
@@ -597,15 +603,15 @@
     /{}
     /DeviceCMYK
     {} 0 R
 ]
 )",
                    name.c_str(),
                    fn_num);
-    separation_objects.push_back(add_object(FullPDFObject{buf, ""}));
+    separation_objects.push_back(add_object(FullPDFObject{buf, {}}));
     return CapyPDF_SeparationId{(int32_t)separation_objects.size() - 1};
 }
 
 LabId PdfDocument::add_lab_colorspace(const LabColorSpace &lab) {
     std::string buf = fmt::format(
         R"([ /Lab
   <<
@@ -782,30 +788,44 @@
                                   0,
                                   embedded_files.size() - 1);
     auto app = std::back_inserter(buf);
     for(size_t i = 0; i < embedded_files.size(); ++i) {
         fmt::format_to(app, "    (embobj{:06}) {} 0 R\n", i, embedded_files[i].filespec_obj);
     }
     buf += "  ]\n>>\n";
-    return add_object(FullPDFObject{std::move(buf), ""});
+    return add_object(FullPDFObject{std::move(buf), {}});
 }
 
 rvoe<int32_t> PdfDocument::create_structure_parent_tree() {
     std::string buf = "<< /Nums [\n";
     auto app = std::back_inserter(buf);
     for(size_t i = 0; i < structure_parent_tree_items.size(); ++i) {
         const auto &entry = structure_parent_tree_items[i];
         fmt::format_to(app, "  {} [\n", i);
         for(const auto &sitem : entry) {
             fmt::format_to(app, "    {} 0 R\n", structure_items.at(sitem.id).obj_id);
         }
         buf += "  ]\n";
     }
     buf += "] >>\n";
-    return add_object(FullPDFObject{std::move(buf), ""});
+    return add_object(FullPDFObject{std::move(buf), {}});
+}
+
+rvoe<CapyPDF_RoleId> PdfDocument::add_rolemap_entry(std::string name,
+                                                    CapyPDF_StructureType builtin_type) {
+    if(name.empty() || name.front() == '/') {
+        RETERR(SlashStart);
+    }
+    for(const auto &i : rolemap) {
+        if(i.name == name) {
+            RETERR(RoleAlreadyDefined);
+        }
+    }
+    rolemap.emplace_back(RolemapEnty{std::move(name), builtin_type});
+    return CapyPDF_RoleId{(int32_t)rolemap.size() - 1};
 }
 
 rvoe<NoReturnValue> PdfDocument::create_catalog() {
     std::string buf;
     auto app = std::back_inserter(buf);
     std::string outline;
     std::string name;
@@ -819,15 +839,15 @@
         ERC(outlines, create_outlines());
         outline = fmt::format("  /Outlines {} 0 R\n", outlines);
     }
     if(!structure_items.empty()) {
         ERC(treeid, create_structure_parent_tree());
         structure_parent_tree_object = treeid;
         create_structure_root_dict();
-        structure = fmt::format("  /StructureTreeRoot {} 0 R\n", *structure_root_object);
+        structure = fmt::format("  /StructTreeRoot {} 0 R\n", *structure_root_object);
     }
     fmt::format_to(app,
                    R"(<<
   /Type /Catalog
   /Pages {} 0 R
 )",
                    pages_object);
@@ -867,15 +887,15 @@
             fmt::format_to(app, "      {} 0 R\n", o);
         }
         buf += "    ]\n";
         buf += "    /D << /BaseState /ON >>\n";
         buf += "  >>\n";
     }
     buf += ">>\n";
-    add_object(FullPDFObject{buf, ""});
+    add_object(FullPDFObject{buf, {}});
     return NoReturnValue{};
 }
 
 void PdfDocument::create_output_intent() {
     std::string buf;
     assert(output_profile);
     assert(opts.subtype);
@@ -885,15 +905,15 @@
   /OutputConditionIdentifier {}
   /DestOutputProfile {} 0 R
 >>
 )",
                       intentnames.at((int)*opts.subtype),
                       pdfstring_quote(opts.intent_condition_identifier),
                       icc_profiles.at(output_profile->id).stream_num);
-    output_intent_object = add_object(FullPDFObject{buf, ""});
+    output_intent_object = add_object(FullPDFObject{buf, {}});
 }
 
 rvoe<int32_t> PdfDocument::create_outlines() {
     int32_t first_obj_num = (int32_t)document_objects.size();
     int32_t catalog_obj_num = first_obj_num + (int32_t)outlines.items.size();
     for(int32_t cur_id = 0; cur_id < (int32_t)outlines.items.size(); ++cur_id) {
         const auto &cur_obj = outlines.items[cur_id];
@@ -931,15 +951,15 @@
         /*
         if(node_counts[cur_id] > 0) {
             fmt::format_to(app, "  /Count {}\n", -node_counts[cur_id]);
         }*/
         fmt::format_to(app,
                        "  /Parent {} 0 R\n>>",
                        parent_id >= 0 ? first_obj_num + parent_id : catalog_obj_num);
-        add_object(FullPDFObject{std::move(oitem), ""});
+        add_object(FullPDFObject{std::move(oitem), {}});
     }
     const auto &top_level = outlines.children.at(-1);
     std::string buf = fmt::format(R"(<<
   /Type /Outlines
   /First {} 0 R
   /Last {} 0 R
   /Count {}
@@ -947,19 +967,20 @@
 )",
                                   first_obj_num + top_level.front(),
                                   first_obj_num + top_level.back(),
                                   outlines.children.at(-1).size());
 
     assert(catalog_obj_num == (int32_t)document_objects.size());
     // FIXME: add output intents here. PDF spec 14.11.5
-    return add_object(FullPDFObject{std::move(buf), ""});
+    return add_object(FullPDFObject{std::move(buf), {}});
 }
 
 void PdfDocument::create_structure_root_dict() {
     std::string buf;
+    auto app = std::back_inserter(buf);
     std::optional<CapyPDF_StructureItemId> rootobj;
 
     if(!structure_parent_tree_object) {
         fprintf(stderr, "Internal error!\n");
         std::abort();
     }
     for(int32_t i = 0; i < (int32_t)structure_items.size(); ++i) {
@@ -967,25 +988,36 @@
             rootobj = CapyPDF_StructureItemId{i};
             break;
         }
         // FIXME, check that there is only one.
     }
     assert(rootobj);
     // /ParentTree
-    buf = fmt::format(R"(<<
+    fmt::format_to(app,
+                   R"(<<
   /Type /StructTreeRoot
   /K [ {} 0 R ]
   /ParentTree {} 0 R
   /ParentTreeNextKey {}
->>
 )",
-                      structure_items[rootobj->id].obj_id,
-                      structure_parent_tree_object.value(),
-                      structure_parent_tree_items.size());
-    structure_root_object = add_object(FullPDFObject{buf, ""});
+                   structure_items[rootobj->id].obj_id,
+                   structure_parent_tree_object.value(),
+                   structure_parent_tree_items.size());
+    if(!rolemap.empty()) {
+        buf += "  /RoleMap <<\n";
+        for(const auto &i : rolemap) {
+            fmt::format_to(app,
+                           "    {} /{}\n",
+                           bytes2pdfstringliteral(i.name),
+                           structure_type_names.at(i.builtin));
+        }
+        buf += "  >>\n";
+    }
+    buf += ">>\n";
+    structure_root_object = add_object(FullPDFObject{buf, {}});
 }
 
 rvoe<NoReturnValue>
 PdfDocument::write_cross_reference_table(const std::vector<uint64_t> &object_offsets) {
     std::string buf;
     auto app = std::back_inserter(buf);
     fmt::format_to(app,
@@ -1280,55 +1312,52 @@
     auto loc = annotation_use.find(annotation.id);
     // It is ok for an annotation not to be used.
 
     assert(annotation.a.rect);
     std::string dict = fmt::format(R"(<<
   /Type /Annot
   /Rect [ {:f} {:f} {:f} {:f} ]
+  /F {}
 )",
                                    annotation.a.rect->x1,
                                    annotation.a.rect->y1,
                                    annotation.a.rect->x2,
-                                   annotation.a.rect->y2);
+                                   annotation.a.rect->y2,
+                                   (int)annotation.a.flags);
     auto app = std::back_inserter(dict);
     if(loc != annotation_use.end()) {
         fmt::format_to(app, "  /P {} 0 R\n", loc->second);
     }
-    if(std::holds_alternative<TextAnnotation>(annotation.a.sub)) {
-        const auto &ta = std::get<TextAnnotation>(annotation.a.sub);
+    if(const auto ta = std::get_if<TextAnnotation>(&annotation.a.sub)) {
         fmt::format_to(app,
                        R"(  /Subtype /Text
   /Contents {}
 )",
-                       utf8_to_pdfmetastr(ta.content));
-    } else if(std::holds_alternative<FileAttachmentAnnotation>(annotation.a.sub)) {
-        auto &faa = std::get<FileAttachmentAnnotation>(annotation.a.sub);
-
+                       utf8_to_pdfmetastr(ta->content));
+    } else if(auto faa = std::get_if<FileAttachmentAnnotation>(&annotation.a.sub)) {
         fmt::format_to(app,
                        R"(  /Subtype /FileAttachment
   /FS {} 0 R
 )",
-                       embedded_files[faa.fileid.id].filespec_obj);
-    } else if(std::holds_alternative<UriAnnotation>(annotation.a.sub)) {
-        auto &ua = std::get<UriAnnotation>(annotation.a.sub);
-        auto uri_as_str = pdfstring_quote(ua.uri.sv());
+                       embedded_files[faa->fileid.id].filespec_obj);
+    } else if(auto ua = std::get_if<UriAnnotation>(&annotation.a.sub)) {
+        auto uri_as_str = pdfstring_quote(ua->uri.sv());
         fmt::format_to(app,
                        R"(  /Subtype /Link
   /Contents {}
   /A <<
     /S /URI
     /URI {}
   >>
 )",
                        uri_as_str,
                        uri_as_str);
-    } else if(std::holds_alternative<ScreenAnnotation>(annotation.a.sub)) {
-        auto &sa = std::get<ScreenAnnotation>(annotation.a.sub);
-        int32_t media_filespec = embedded_files.at(sa.mediafile.id).filespec_obj;
-        if(!sa.times) {
+    } else if(auto sa = std::get_if<ScreenAnnotation>(&annotation.a.sub)) {
+        int32_t media_filespec = embedded_files.at(sa->mediafile.id).filespec_obj;
+        if(!sa->times) {
             fmt::format_to(app,
                            R"(  /Subtype /Screen
   /A <<
     /Type /Action
     /S /Rendition
     /OP 0
     /AN {} 0 R
@@ -1342,15 +1371,15 @@
         /D {} 0 R
         /P << /TF (TEMPALWAYS) >>
       >>
     >>
   >>
 )",
                            obj_num,
-                           sa.mimetype,
+                           sa->mimetype,
                            media_filespec);
         } else {
             // NOTE! This should work but does not. Acrobat reader will error
             // out if there are any entries in the MH dictionary, regardless whether they
             // are time or frame dictionaries.
             fmt::format_to(app,
                            R"(  /Subtype /Screen
@@ -1377,26 +1406,25 @@
           /E << /S /T /T << /S /S /V {:f} >> >>
         >>
       >>
     >>
   >>
 )",
                            obj_num,
-                           sa.mimetype,
+                           sa->mimetype,
                            media_filespec,
-                           sa.times->starttime,
-                           sa.times->endtime);
+                           sa->times->starttime,
+                           sa->times->endtime);
         }
-    } else if(std::holds_alternative<PrintersMarkAnnotation>(annotation.a.sub)) {
-        auto &pma = std::get<PrintersMarkAnnotation>(annotation.a.sub);
+    } else if(auto pma = std::get_if<PrintersMarkAnnotation>(&annotation.a.sub)) {
         fmt::format_to(app,
                        R"(  /Subtype /PrinterMark
   /AP << /N {} 0 R >>
 )",
-                       form_xobjects.at(pma.appearance.id).xobj_num);
+                       form_xobjects.at(pma->appearance.id).xobj_num);
     } else {
         fprintf(stderr, "Unknown annotation type.\n");
         std::abort();
     }
     dict += ">>\n";
     ERCV(write_finished_object(obj_num, dict, ""));
     return NoReturnValue{};
@@ -1417,28 +1445,47 @@
         if(structure_items[i].parent) {
             auto current_parent = structure_items.at(structure_items[i].parent->id).obj_id;
             if(current_parent == si.obj_id) {
                 children.emplace_back(CapyPDF_StructureItemId{i});
             }
         }
     }
-    std::string dict = fmt::format(R"(<<
+    std::string dict = R"(<<
   /Type /StructElem
-  /S /{}
-  /P {} 0 R
-)",
-                                   si.stype.sv(),
-                                   parent_object);
+)";
     auto app = std::back_inserter(dict);
+    if(auto bi = std::get_if<CapyPDF_StructureType>(&si.stype)) {
+        fmt::format_to(app,
+                       R"(  /S /{}
+)",
+                       structure_type_names.at(*bi));
+    } else if(auto ri = std::get_if<CapyPDF_RoleId>(&si.stype)) {
+        const auto &role = *ri;
+        fmt::format_to(app, "  /S {}\n", bytes2pdfstringliteral(rolemap.at(role.id).name));
+    } else {
+        fprintf(stderr, "UNREACHABLE.\n");
+        std::abort();
+    }
+    fmt::format_to(app, "  /P {} 0 R\n", parent_object);
+
     if(!children.empty()) {
         dict += "  /K [\n";
         for(const auto &c : children) {
             fmt::format_to(app, "    {} 0 R\n", structure_items.at(c.id).obj_id);
         }
         dict += "  ]\n";
+    } else {
+        // FIXME. Maybe not correct? Assumes that a struct item
+        // either has children or is used on a page. Not both.
+        const auto it = structure_use.find(dsi.sid);
+        if(it != structure_use.end()) {
+            const auto &[page_num, mcid_num] = it->second;
+            fmt::format_to(app, "  /Pg {} 0 R\n", pages.at(page_num).page_obj_num);
+            fmt::format_to(app, "  /K {}\n", mcid_num);
+        }
     }
     dict += ">>\n";
     ERCV(write_finished_object(obj_num, dict, ""));
     return NoReturnValue{};
 }
 
 rvoe<NoReturnValue> PdfDocument::write_finished_object(int32_t object_number,
@@ -1489,15 +1536,15 @@
     fmt::format_to(std::back_inserter(buf),
                    R"(<<
   /N {}
 )",
                    num_channels);
     auto stream_obj_id = add_object(DeflatePDFObject{std::move(buf), std::string{contents}});
     auto obj_id =
-        add_object(FullPDFObject{fmt::format("[ /ICCBased {} 0 R ]\n", stream_obj_id), ""});
+        add_object(FullPDFObject{fmt::format("[ /ICCBased {} 0 R ]\n", stream_obj_id), {}});
     icc_profiles.emplace_back(IccInfo{stream_obj_id, obj_id, num_channels});
     return CapyPDF_IccColorSpaceId{(int32_t)icc_profiles.size() - 1};
 }
 
 rvoe<NoReturnValue> PdfDocument::write_bytes(const char *buf, size_t buf_size) {
     if(fwrite(buf, 1, buf_size, ofile) != buf_size) {
         perror(nullptr);
@@ -1557,15 +1604,15 @@
                    R"(<<
   /Type /Font
   /Subtype /Type1
   /BaseFont /{}
 >>
 )",
                    font_names[font]);
-    font_objects.push_back(FontInfo{-1, -1, add_object(FullPDFObject{font_dict, ""}), size_t(-1)});
+    font_objects.push_back(FontInfo{-1, -1, add_object(FullPDFObject{font_dict, {}}), size_t(-1)});
     auto fontid = CapyPDF_FontId{(int32_t)font_objects.size() - 1};
     builtin_fonts[font] = fontid;
     return fontid;
 }
 
 uint32_t PdfDocument::glyph_for_codepoint(FT_Face face, uint32_t ucs4) {
     assert(face);
@@ -1721,20 +1768,18 @@
         buf += "  /Interpolate true\n";
     }
 
     // An image may only have ImageMask or ColorSpace key, not both.
     if(is_mask) {
         buf += "  /ImageMask true\n";
     } else {
-        if(std::holds_alternative<CapyPDF_Colorspace>(colorspace)) {
-            const auto &cs = std::get<CapyPDF_Colorspace>(colorspace);
-            fmt::format_to(app, "  /ColorSpace {}\n", colorspace_names.at(cs));
-        } else if(std::holds_alternative<CapyPDF_IccColorSpaceId>(colorspace)) {
-            const auto &icc = std::get<CapyPDF_IccColorSpaceId>(colorspace);
-            const auto icc_obj = icc_profiles.at(icc.id).object_num;
+        if(auto cs = std::get_if<CapyPDF_Colorspace>(&colorspace)) {
+            fmt::format_to(app, "  /ColorSpace {}\n", colorspace_names.at(*cs));
+        } else if(auto icc = std::get_if<CapyPDF_IccColorSpaceId>(&colorspace)) {
+            const auto icc_obj = icc_profiles.at(icc->id).object_num;
             fmt::format_to(app, "  /ColorSpace {} 0 R\n", icc_obj);
         } else {
             fprintf(stderr, "Unknown colorspace.");
             std::abort();
         }
     }
     if(smask_id) {
@@ -2074,15 +2119,15 @@
   /Type /Filespec
   /F {}
   /EF << /F {} 0 R >>
 >>
 )",
                        pdfstring_quote(fname.filename().string()),
                        fileobj_id);
-    auto filespec_id = add_object(FullPDFObject{std::move(dict), ""});
+    auto filespec_id = add_object(FullPDFObject{std::move(dict), {}});
     embedded_files.emplace_back(EmbeddedFileObject{filespec_id, fileobj_id});
     return CapyPDF_EmbeddedFileId{(int32_t)embedded_files.size() - 1};
 }
 
 rvoe<CapyPDF_AnnotationId> PdfDocument::create_annotation(const Annotation &a) {
     if(!a.rect) {
         RETERR(AnnotationMissingRect);
@@ -2090,49 +2135,61 @@
     auto annot_id = (int32_t)annotations.size();
     auto obj_id = add_object(DelayedAnnotation{annot_id, a});
     annotations.push_back((int32_t)obj_id);
     return CapyPDF_AnnotationId{annot_id};
 }
 
 rvoe<CapyPDF_StructureItemId>
-PdfDocument::add_structure_item(const asciistring &stype,
+PdfDocument::add_structure_item(const CapyPDF_StructureType stype,
                                 std::optional<CapyPDF_StructureItemId> parent) {
     if(parent) {
         CHECK_INDEXNESS_V(parent->id, structure_items);
     }
     auto stritem_id = (int32_t)structure_items.size();
     auto obj_id = add_object(DelayedStructItem{stritem_id});
     structure_items.push_back(StructItem{obj_id, stype, parent});
     return CapyPDF_StructureItemId{(int32_t)structure_items.size() - 1};
 }
 
+rvoe<CapyPDF_StructureItemId>
+PdfDocument::add_structure_item(const CapyPDF_RoleId role,
+                                std::optional<CapyPDF_StructureItemId> parent) {
+    if(parent) {
+        CHECK_INDEXNESS_V(parent->id, structure_items);
+    }
+    auto stritem_id = (int32_t)structure_items.size();
+    auto obj_id = add_object(DelayedStructItem{stritem_id});
+    structure_items.push_back(StructItem{obj_id, role, parent});
+    return CapyPDF_StructureItemId{(int32_t)structure_items.size() - 1};
+}
+
 rvoe<CapyPDF_OptionalContentGroupId>
 PdfDocument::add_optional_content_group(const OptionalContentGroup &g) {
     auto id = add_object(FullPDFObject{fmt::format(R"(<<
   /Type /OCG
   /Name {}
 >>
 )",
                                                    pdfstring_quote(g.name)),
-                                       ""});
+                                       {}});
     ocg_items.push_back(id);
     return CapyPDF_OptionalContentGroupId{(int32_t)ocg_items.size() - 1};
 }
 
 rvoe<CapyPDF_TransparencyGroupId>
 PdfDocument::add_transparency_group(PdfDrawContext &ctx, const TransparencyGroupExtra *ex) {
     if(ctx.draw_context_type() != CAPY_DC_TRANSPARENCY_GROUP) {
         RETERR(InvalidDrawContextType);
     }
     if(ctx.marked_content_depth() != 0) {
         RETERR(UnclosedMarkedContent);
     }
     auto sc_var = ctx.serialize(ex);
     auto &d = std::get<SerializedXObject>(sc_var);
-    auto objid = add_object(FullPDFObject{std::move(d.dict), std::move(d.stream)});
+    auto objid = add_object(FullPDFObject{std::move(d.dict), std::move(d.command_stream)});
     transparency_groups.push_back(objid);
     return CapyPDF_TransparencyGroupId{(int32_t)transparency_groups.size() - 1};
 }
 
 std::optional<double>
 PdfDocument::glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const {
     FT_Face face = fonts.at(fid.id).fontdata.face.get();
```

### Comparing `capypdf-0.8.0/src/pdfdocument.hpp` & `capypdf-0.9.0/src/pdfdocument.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     u8string creator;
     asciistring lang;
     bool is_tagged = false;
     CapyPDF_Colorspace output_colorspace = CAPY_CS_DEVICE_RGB;
     ColorProfiles prof;
     std::optional<CapyPDF_Intent_Subtype> subtype;
     std::string intent_condition_identifier;
+    bool compress_streams = false;
 };
 
 struct Outline {
     u8string title;
     PageId dest;
     std::optional<CapyPDF_OutlineId> parent;
 };
@@ -253,61 +254,73 @@
                      ScreenAnnotation,
                      PrintersMarkAnnotation>
     AnnotationSubType;
 
 struct Annotation {
     AnnotationSubType sub;
     std::optional<PdfRectangle> rect;
+    CapyPDF_AnnotationFlags flags{CAPY_ANNOTATION_FLAG_NONE};
 };
 
 struct DelayedAnnotation {
     CapyPDF_AnnotationId id;
     Annotation a;
 };
 
 struct DelayedStructItem {
     CapyPDF_StructureItemId sid;
 };
 
 struct StructItem {
     int32_t obj_id;
-    asciistring stype;
+    std::variant<CapyPDF_StructureType, CapyPDF_RoleId> stype;
     std::optional<CapyPDF_StructureItemId> parent;
 };
 
+struct StructureUsage {
+    int32_t page_num;
+    int32_t mcid_num;
+};
+
 typedef std::variant<DummyIndexZero,
                      FullPDFObject,
                      DeflatePDFObject,
                      DelayedSubsetFontData,
                      DelayedSubsetFontDescriptor,
                      DelayedSubsetCMap,
                      DelayedSubsetFont,
                      DelayedPages,
                      DelayedPage,
                      DelayedCheckboxWidgetAnnotation, // FIXME, convert to hold all widgets
                      DelayedAnnotation,
                      DelayedStructItem>
     ObjectType;
 
+struct RolemapEnty {
+    std::string name;
+    CapyPDF_StructureType builtin;
+};
+
 typedef std::variant<CapyPDF_Colorspace, CapyPDF_IccColorSpaceId> ColorspaceType;
 
 class PdfDocument {
 public:
     static rvoe<PdfDocument> construct(const PdfGenerationData &d, PdfColorConverter cm);
 
     PdfDocument(PdfDocument &&o) = default;
 
     friend class PdfGen;
     friend class PdfDrawContext;
 
     rvoe<NoReturnValue> write_to_file(FILE *output_file);
 
     // Pages
-    rvoe<NoReturnValue> add_page(std::string resource_data,
-                                 std::string page_data,
+    rvoe<NoReturnValue> add_page(std::string resource_dict,
+                                 std::string unclosed_object_dict,
+                                 std::string command_stream,
                                  const PageProperties &custom_props,
                                  const std::unordered_set<CapyPDF_FormWidgetId> &form_widgets,
                                  const std::unordered_set<CapyPDF_AnnotationId> &annots,
                                  const std::vector<CapyPDF_StructureItemId> &structs,
                                  const std::optional<Transition> &transition,
                                  const std::vector<SubPageNavigation> &subnav);
 
@@ -361,29 +374,33 @@
     // Raw files
     rvoe<CapyPDF_EmbeddedFileId> embed_file(const std::filesystem::path &fname);
 
     // Annotations.
     rvoe<CapyPDF_AnnotationId> create_annotation(const Annotation &a);
 
     // Structure items
-    rvoe<CapyPDF_StructureItemId> add_structure_item(const asciistring &stype,
+    rvoe<CapyPDF_StructureItemId> add_structure_item(const CapyPDF_StructureType stype,
+                                                     std::optional<CapyPDF_StructureItemId> parent);
+    rvoe<CapyPDF_StructureItemId> add_structure_item(const CapyPDF_RoleId role,
                                                      std::optional<CapyPDF_StructureItemId> parent);
 
     // Optional content groups
     rvoe<CapyPDF_OptionalContentGroupId> add_optional_content_group(const OptionalContentGroup &g);
 
     // Transparency groups
     rvoe<CapyPDF_TransparencyGroupId> add_transparency_group(PdfDrawContext &ctx,
                                                              const TransparencyGroupExtra *ex);
 
     std::optional<double>
     glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const;
 
     rvoe<int32_t> create_structure_parent_tree();
 
+    rvoe<CapyPDF_RoleId> add_rolemap_entry(std::string name, CapyPDF_StructureType builtin_type);
+
 private:
     PdfDocument(const PdfGenerationData &d, PdfColorConverter cm);
     rvoe<NoReturnValue> init();
 
     rvoe<NoReturnValue> write_to_file_impl();
 
     int32_t add_object(ObjectType object);
@@ -472,18 +489,19 @@
     std::vector<FormXObjectInfo> form_xobjects;
     std::vector<int32_t> form_widgets;
     std::vector<EmbeddedFileObject> embedded_files;
     std::vector<int32_t> annotations;
     std::vector<StructItem> structure_items;
     std::vector<int32_t> ocg_items;
     std::vector<int32_t> transparency_groups;
+    std::vector<RolemapEnty> rolemap;
     // A form widget can be used on one and only one page.
     std::unordered_map<CapyPDF_FormWidgetId, int32_t> form_use;
     std::unordered_map<CapyPDF_AnnotationId, int32_t> annotation_use;
-    std::unordered_map<CapyPDF_StructureItemId, int32_t> structure_use;
+    std::unordered_map<CapyPDF_StructureItemId, StructureUsage> structure_use;
     std::vector<std::vector<CapyPDF_StructureItemId>>
         structure_parent_tree_items; // FIXME should be a variant of some sort?
     std::optional<CapyPDF_IccColorSpaceId> output_profile;
     std::optional<int32_t> output_intent_object;
     std::optional<int32_t> structure_root_object;
     std::optional<int32_t> structure_parent_tree_object;
     int32_t pages_object;
```

### Comparing `capypdf-0.8.0/src/pdfdrawcontext.cpp` & `capypdf-0.9.0/src/pdfdrawcontext.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -21,31 +21,30 @@
 PdfDrawContext::PdfDrawContext(
     PdfDocument *doc, PdfColorConverter *cm, CapyPDF_Draw_Context_Type dtype, double w, double h)
     : doc(doc), cm(cm), context_type{dtype}, cmd_appender(commands), w{w}, h{h} {}
 
 PdfDrawContext::~PdfDrawContext() {}
 
 DCSerialization PdfDrawContext::serialize(const TransparencyGroupExtra *trinfo) {
-    SerializedBasicContext sc;
-    sc.dict = build_resource_dict();
+    auto resource_dict = build_resource_dict();
     if(context_type == CAPY_DC_FORM_XOBJECT) {
         std::string dict = fmt::format(
             R"(<<
   /Type /XObject
   /Subtype /Form
   /BBox [ {:f} {:f} {:f} {:f} ]
   /Resources {}
   /Length {}
 >>
 )",
             0.0,
             0.0,
             w,
             h,
-            sc.dict,
+            resource_dict,
             commands.size());
         return SerializedXObject{std::move(dict), commands};
     } else if(context_type == CAPY_DC_TRANSPARENCY_GROUP) {
         std::string dict = R"(<<
   /Type /XObject
   /Subtype /Form
 )";
@@ -64,30 +63,24 @@
         }
         fmt::format_to(app,
                        R"(  >>
   /Resources {}
   /Length {}
 >>
 )",
-                       sc.dict,
+                       resource_dict,
                        commands.size());
         return SerializedXObject{std::move(dict), commands};
     } else {
-        sc.commands = fmt::format(
-            R"(<<
-  /Length {}
->>
-stream
-{}
-endstream
-)",
-            commands.size(),
-            commands);
+        SerializedBasicContext sc;
+        sc.resource_dict = std::move(resource_dict);
+        sc.unclosed_object_dict = "<<\n";
+        sc.command_stream = commands;
+        return sc;
     }
-    return sc;
 }
 
 void PdfDrawContext::clear() {
     commands.clear();
     used_images.clear();
     used_subset_fonts.clear();
     used_fonts.clear();
@@ -252,34 +245,48 @@
         for(const auto &[key, value] : attributes.value()) {
             // FIXME: validate value contents properly.
             fmt::format_to(cmd_appender, "{}  /{} ({})\n", ind, key, value);
         }
     }
     fmt::format_to(cmd_appender, "{}>>\n", ind);
     fmt::format_to(cmd_appender, "{}BDC\n", ind);
+    ERCV(indent(DrawStateType::MarkedContent));
     ++marked_depth;
-    indent(DrawStateType::MarkedContent);
     RETOK;
 }
 
+rvoe<NoReturnValue> PdfDrawContext::cmd_BDC(CapyPDF_StructureItemId sid) {
+    const auto &itemtype = doc->structure_items.at(sid.id).stype;
+    if(auto builtin = std::get_if<CapyPDF_StructureType>(&itemtype)) {
+        ERC(astr, asciistring::from_cstr(structure_type_names.at(*builtin)));
+        return cmd_BDC(astr, sid, {});
+    } else if(auto role = std::get_if<CapyPDF_RoleId>(&itemtype)) {
+        auto quoted = bytes2pdfstringliteral(doc->rolemap.at(role->id).name, false);
+        ERC(astr, asciistring::from_cstr(quoted.c_str()));
+        return cmd_BDC(astr, sid, {});
+    } else {
+        std::abort();
+    }
+}
+
 rvoe<NoReturnValue> PdfDrawContext::cmd_BDC(CapyPDF_OptionalContentGroupId ocgid) {
     ++marked_depth;
     used_ocgs.insert(ocgid);
     fmt::format_to(cmd_appender, "{}/OC /oc{} BDC\n", ind, doc->ocg_object_number(ocgid));
-    indent(DrawStateType::MarkedContent);
+    ERCV(indent(DrawStateType::MarkedContent));
     RETOK;
 }
 
 rvoe<NoReturnValue> PdfDrawContext::cmd_BMC(std::string_view tag) {
-    if(tag.size() < 2 or tag.front() != '/') {
-        RETERR(BadBMC);
+    if(tag.size() < 2 || tag.front() == '/') {
+        RETERR(SlashStart);
     }
     ++marked_depth;
-    fmt::format_to(cmd_appender, "{}{} BMC\n", ind, tag);
-    indent(DrawStateType::MarkedContent);
+    fmt::format_to(cmd_appender, "{}/{} BMC\n", ind, tag);
+    ERCV(indent(DrawStateType::MarkedContent));
     RETOK;
 }
 
 rvoe<NoReturnValue>
 PdfDrawContext::cmd_c(double x1, double y1, double x2, double y2, double x3, double y3) {
     fmt::format_to(
         cmd_appender, "{}{:f} {:f} {:f} {:f} {:f} {:f} c\n", ind, x1, y1, x2, y2, x3, y3);
@@ -436,15 +443,15 @@
     commands += "n\n";
     RETOK;
 }
 
 rvoe<NoReturnValue> PdfDrawContext::cmd_q() {
     commands += ind;
     commands += "q\n";
-    indent(DrawStateType::SaveState);
+    ERCV(indent(DrawStateType::SaveState));
     RETOK;
 }
 
 rvoe<NoReturnValue> PdfDrawContext::cmd_Q() {
     ERCV(dedent(DrawStateType::SaveState));
     commands += ind;
     commands += "Q\n";
@@ -584,28 +591,28 @@
                                                  LimitDouble g,
                                                  LimitDouble b) const {
     fmt::format_to(out, "{}{:f} {:f} {:f} rg\n", indent, r.v(), g.v(), b.v());
     RETOK;
 }
 
 rvoe<NoReturnValue> PdfDrawContext::set_color(const Color &c, bool stroke) {
-    if(std::holds_alternative<DeviceRGBColor>(c)) {
-        return set_color(std::get<DeviceRGBColor>(c), stroke);
-    } else if(std::holds_alternative<DeviceGrayColor>(c)) {
-        return set_color(std::get<DeviceGrayColor>(c), stroke);
-    } else if(std::holds_alternative<DeviceCMYKColor>(c)) {
-        return set_color(std::get<DeviceCMYKColor>(c), stroke);
-    } else if(std::holds_alternative<ICCColor>(c)) {
-        return set_color(std::get<ICCColor>(c), stroke);
-    } else if(std::holds_alternative<LabColor>(c)) {
-        return set_color(std::get<LabColor>(c), stroke);
-    } else if(std::holds_alternative<CapyPDF_PatternId>(c)) {
-        return set_color(std::get<CapyPDF_PatternId>(c), stroke);
-    } else if(std::holds_alternative<SeparationColor>(c)) {
-        return set_color(std::get<SeparationColor>(c), stroke);
+    if(auto cv = std::get_if<DeviceRGBColor>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<DeviceGrayColor>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<DeviceCMYKColor>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<ICCColor>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<LabColor>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<CapyPDF_PatternId>(&c)) {
+        return set_color(*cv, stroke);
+    } else if(auto cv = std::get_if<SeparationColor>(&c)) {
+        return set_color(*cv, stroke);
     } else {
         printf("Given colorspace not supported yet.\n");
         fflush(stdout);
         std::abort();
     }
     RETOK;
 }
@@ -766,20 +773,20 @@
                                                            std::string &serialisation,
                                                            CapyPDF_FontId &current_font,
                                                            int32_t &current_subset,
                                                            double &current_pointsize) {
     std::back_insert_iterator<std::string> app = std::back_inserter(serialisation);
     bool is_first = true;
     for(const auto &e : charseq) {
-        if(std::holds_alternative<double>(e)) {
+        if(auto dbl = std::get_if<double>(&e)) {
             if(is_first) {
                 serialisation += ind;
                 serialisation += "[ ";
             }
-            fmt::format_to(app, "{:f} ", std::get<double>(e));
+            fmt::format_to(app, "{:f} ", *dbl);
         } else {
             assert(std::holds_alternative<uint32_t>(e));
             const auto codepoint = std::get<uint32_t>(e);
             ERC(current_subset_glyph, doc->get_subset_glyph(current_font, codepoint));
             used_subset_fonts.insert(current_subset_glyph.ss);
             if(current_subset_glyph.ss.subset_id != current_subset) {
                 if(!is_first) {
@@ -848,15 +855,15 @@
 }
 
 rvoe<NoReturnValue> PdfDrawContext::render_text(const PdfText &textobj) {
     if(textobj.creator() != this) {
         RETERR(WrongDrawContext);
     }
     std::string serialisation{ind + "BT\n"};
-    indent(DrawStateType::Text);
+    ERCV(indent(DrawStateType::Text));
     std::back_insert_iterator<std::string> app = std::back_inserter(serialisation);
     int32_t current_subset{-1};
     CapyPDF_FontId current_font{-1};
     double current_pointsize{-1};
 
     auto visitor = overloaded{
         [&](const TStar_arg &) -> rvoe<NoReturnValue> {
@@ -939,54 +946,60 @@
 
         [&](const Tz_arg &tz) -> rvoe<NoReturnValue> {
             fmt::format_to(app, "{}{:f} Tz\n", ind, tz.scaling);
             return NoReturnValue{};
         },
 
         [&](const StructureItem &sitem) -> rvoe<NoReturnValue> {
+            // FIXME, convert to a serialize method and make
+            // this and cmd_BDC use that.
             ERC(mcid_id, add_bcd_structure(sitem.sid));
-            fmt::format_to(
-                app, "{}/{} << /MCID {} >>\n{}BDC\n", ind, sitem.name.sv(), mcid_id, ind);
-            indent(DrawStateType::MarkedContent);
+            auto item = doc->structure_items.at(sitem.sid.id).stype;
+            if(auto itemid = std::get_if<CapyPDF_StructureType>(&item)) {
+                const auto &itemstr = structure_type_names.at(*itemid);
+                fmt::format_to(app, "{}/{} << /MCID {} >>\n{}BDC\n", ind, itemstr, mcid_id, ind);
+            } else if(auto ri = std::get_if<CapyPDF_RoleId>(&item)) {
+                const auto &role = *ri;
+                auto rolename = bytes2pdfstringliteral(doc->rolemap.at(role.id).name);
+                fmt::format_to(app, "{}{} << /MCID {} >>\n{}BDC\n", ind, rolename, mcid_id, ind);
+            } else {
+                fprintf(stderr, "FIXME 1\n");
+                std::abort();
+            }
+            ERCV(indent(DrawStateType::MarkedContent));
             return NoReturnValue{};
         },
 
         [&](const Emc_arg &) -> rvoe<NoReturnValue> {
             ERCV(dedent(DrawStateType::MarkedContent));
             fmt::format_to(app, "{}EMC\n", ind);
             return NoReturnValue{};
         },
 
         [&](const Stroke_arg &sarg) -> rvoe<NoReturnValue> {
-            if(std::holds_alternative<DeviceRGBColor>(sarg.c)) {
-                auto &rgb = std::get<DeviceRGBColor>(sarg.c);
-                ERCV(serialize_RG(app, ind, rgb.r, rgb.g, rgb.b));
-            } else if(std::holds_alternative<DeviceGrayColor>(sarg.c)) {
-                auto &gray = std::get<DeviceGrayColor>(sarg.c);
-                ERCV(serialize_G(app, ind, gray.v));
-            } else if(std::holds_alternative<DeviceCMYKColor>(sarg.c)) {
-                auto &cmyk = std::get<DeviceCMYKColor>(sarg.c);
-                ERCV(serialize_K(app, ind, cmyk.c, cmyk.m, cmyk.y, cmyk.k));
+            if(auto rgb = std::get_if<DeviceRGBColor>(&sarg.c)) {
+                ERCV(serialize_RG(app, ind, rgb->r, rgb->g, rgb->b));
+            } else if(auto gray = std::get_if<DeviceGrayColor>(&sarg.c)) {
+                ERCV(serialize_G(app, ind, gray->v));
+            } else if(auto cmyk = std::get_if<DeviceCMYKColor>(&sarg.c)) {
+                ERCV(serialize_K(app, ind, cmyk->c, cmyk->m, cmyk->y, cmyk->k));
             } else {
                 printf("Given text stroke colorspace not supported yet.\n");
                 std::abort();
             }
             return NoReturnValue{};
         },
 
         [&](const Nonstroke_arg &nsarg) -> rvoe<NoReturnValue> {
-            if(std::holds_alternative<DeviceRGBColor>(nsarg.c)) {
-                auto &rgb = std::get<DeviceRGBColor>(nsarg.c);
-                ERCV(serialize_rg(app, ind, rgb.r, rgb.g, rgb.b));
-            } else if(std::holds_alternative<DeviceGrayColor>(nsarg.c)) {
-                auto &gray = std::get<DeviceGrayColor>(nsarg.c);
-                ERCV(serialize_g(app, ind, gray.v));
-            } else if(std::holds_alternative<DeviceCMYKColor>(nsarg.c)) {
-                auto &cmyk = std::get<DeviceCMYKColor>(nsarg.c);
-                ERCV(serialize_k(app, ind, cmyk.c, cmyk.m, cmyk.y, cmyk.k));
+            if(auto rgb = std::get_if<DeviceRGBColor>(&nsarg.c)) {
+                ERCV(serialize_rg(app, ind, rgb->r, rgb->g, rgb->b));
+            } else if(auto gray = std::get_if<DeviceGrayColor>(&nsarg.c)) {
+                ERCV(serialize_g(app, ind, gray->v));
+            } else if(auto cmyk = std::get_if<DeviceCMYKColor>(&nsarg.c)) {
+                ERCV(serialize_k(app, ind, cmyk->c, cmyk->m, cmyk->y, cmyk->k));
             } else {
                 printf("Given text nonstroke colorspace not supported yet.\n");
                 std::abort();
             }
             return NoReturnValue{};
         },
     };
```

### Comparing `capypdf-0.8.0/src/pdfdrawcontext.hpp` & `capypdf-0.9.0/src/pdfdrawcontext.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #include <pdfdocument.hpp>
 #include <string>
 #include <string_view>
 #include <unordered_set>
 #include <vector>
 #include <optional>
 #include <span>
-#include <stack>
 
 template<> struct std::hash<capypdf::FontSubset> {
     size_t operator()(capypdf::FontSubset const &s) const noexcept {
         const size_t x = (size_t)s.fid.id;
         const size_t y = s.subset_id;
         if constexpr(sizeof(size_t) == 8) {
             return (x << 32) + y;
@@ -40,21 +39,22 @@
     GstatePopper() = delete;
     GstatePopper(const GstatePopper &) = delete;
 
     ~GstatePopper();
 };
 
 struct SerializedBasicContext {
-    std::string dict;
-    std::string commands;
+    std::string resource_dict;
+    std::string unclosed_object_dict;
+    std::string command_stream;
 };
 
 struct SerializedXObject {
-    std::string dict;
-    std::string stream;
+    std::string dict; // FIXME, convert to unclosed so these can be compressed.
+    std::string command_stream;
 };
 
 typedef std::variant<SerializedBasicContext, SerializedXObject> DCSerialization;
 
 struct PdfGlyph {
     uint32_t codepoint;
     double x, y;
@@ -86,18 +86,16 @@
     rvoe<NoReturnValue> cmd_B();
     rvoe<NoReturnValue> cmd_bstar();
     rvoe<NoReturnValue> cmd_Bstar();
     rvoe<NoReturnValue>
     cmd_BDC(const asciistring &name,
             std::optional<CapyPDF_StructureItemId> sid,
             const std::optional<std::unordered_map<std::string, std::string>> &attributes);
-    rvoe<NoReturnValue> cmd_BDC(const asciistring &name,
-                                std::optional<CapyPDF_StructureItemId> sid) {
-        return cmd_BDC(name, sid, {});
-    }
+    // FIXME, needs an argument to specify extra dict.
+    rvoe<NoReturnValue> cmd_BDC(CapyPDF_StructureItemId sid);
     rvoe<NoReturnValue> cmd_BDC(CapyPDF_OptionalContentGroupId id);
     rvoe<NoReturnValue> cmd_BMC(std::string_view tag);
     rvoe<NoReturnValue> cmd_c(double x1, double y1, double x2, double y2, double x3, double y3);
     rvoe<NoReturnValue> cmd_cm(double m1, double m2, double m3, double m4, double m5, double m6);
     rvoe<NoReturnValue> cmd_CS(std::string_view cspace_name);
     rvoe<NoReturnValue> cmd_cs(std::string_view cspace_name);
     rvoe<NoReturnValue> cmd_d(double *dash_array, size_t dash_array_length, double phase);
@@ -225,15 +223,15 @@
         return used_structures;
     }
 
     const std::optional<Transition> &get_transition() const { return transition; }
 
     const std::vector<SubPageNavigation> &get_subpage_navigation() const { return sub_navigations; }
 
-    bool has_unclosed_state() const { return !dstates.empty(); }
+    bool has_unclosed_state() const { return !dstate_stack.empty(); }
 
     rvoe<NoReturnValue> set_transition(const Transition &tr);
 
     rvoe<NoReturnValue> add_simple_navigation(std::span<const CapyPDF_OptionalContentGroupId> navs,
                                               const std::optional<Transition> &tr);
 
     const PageProperties &get_custom_props() const { return custom_props; }
@@ -245,30 +243,38 @@
                                                std::string &serialisation,
                                                CapyPDF_FontId &current_font,
                                                int32_t &current_subset,
                                                double &current_pointsize);
     rvoe<NoReturnValue>
     utf8_to_kerned_chars(const u8string &text, std::vector<CharItem> &charseq, CapyPDF_FontId fid);
 
-    void indent(DrawStateType dtype) {
-        dstates.push(dtype);
+    rvoe<NoReturnValue> indent(DrawStateType dtype) {
+        if(dtype == DrawStateType::MarkedContent) {
+            for(const auto &s : dstate_stack) {
+                if(s == dtype) {
+                    RETERR(NestedBMC);
+                }
+            }
+        }
+        dstate_stack.push_back(dtype);
         ind += "  ";
+        return NoReturnValue{};
     }
 
     rvoe<NoReturnValue> dedent(DrawStateType dtype) {
-        if(dstates.empty()) {
+        if(dstate_stack.empty()) {
             RETERR(DrawStateEndMismatch);
         }
-        if(dstates.top() != dtype) {
+        if(dstate_stack.back() != dtype) {
             RETERR(DrawStateEndMismatch);
         }
         if(ind.size() < 2) {
             std::abort();
         }
-        dstates.pop();
+        dstate_stack.pop_back();
         ind.pop_back();
         ind.pop_back();
         return NoReturnValue{};
     }
 
     rvoe<int32_t> add_bcd_structure(CapyPDF_StructureItemId sid);
 
@@ -288,15 +294,16 @@
     std::unordered_set<CapyPDF_FormWidgetId> used_widgets;
     std::unordered_set<CapyPDF_AnnotationId> used_annotations;
     std::vector<CapyPDF_StructureItemId> used_structures; // A vector because numbering is relevant.
     std::unordered_set<CapyPDF_OptionalContentGroupId> used_ocgs;
     std::unordered_set<CapyPDF_TransparencyGroupId> used_trgroups;
     std::vector<SubPageNavigation> sub_navigations;
 
-    std::stack<DrawStateType> dstates;
+    // Not a std::stack because we need to access all entries.
+    std::vector<DrawStateType> dstate_stack;
     std::optional<Transition> transition;
 
     PageProperties custom_props;
     // Reminder: If you add stuff here, also add them to .clear().
     bool is_finalized = false;
     bool uses_all_colorspace = false;
     double w = -1;
```

### Comparing `capypdf-0.8.0/src/pdfgen.cpp` & `capypdf-0.9.0/src/pdfgen.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,17 @@
     }
     if(ctx.has_unclosed_state()) {
         RETERR(DrawStateEndMismatch);
     }
     auto sc_var = ctx.serialize();
     assert(std::holds_alternative<SerializedBasicContext>(sc_var));
     auto &sc = std::get<SerializedBasicContext>(sc_var);
-    ERCV(pdoc.add_page(std::move(sc.dict),
-                       std::move(sc.commands),
+    ERCV(pdoc.add_page(std::move(sc.resource_dict),
+                       std::move(sc.unclosed_object_dict),
+                       std::move(sc.command_stream),
                        ctx.get_custom_props(),
                        ctx.get_form_usage(),
                        ctx.get_annotation_usage(),
                        ctx.get_structure_usage(),
                        ctx.get_transition(),
                        ctx.get_subpage_navigation()));
     ctx.clear();
@@ -172,15 +173,15 @@
     }
     if(ctx.marked_content_depth() != 0) {
         RETERR(UnclosedMarkedContent);
     }
     auto sc_var = ctx.serialize();
     assert(std::holds_alternative<SerializedXObject>(sc_var));
     auto &sc = std::get<SerializedXObject>(sc_var);
-    pdoc.add_form_xobject(std::move(sc.dict), std::move(sc.stream));
+    pdoc.add_form_xobject(std::move(sc.dict), std::move(sc.command_stream));
     ctx.clear();
     CapyPDF_FormXObjectId fxoid;
     fxoid.id = (int32_t)pdoc.form_xobjects.size() - 1;
     return rvoe<CapyPDF_FormXObjectId>{fxoid};
 }
 
 rvoe<CapyPDF_PatternId> PdfGen::add_pattern(PdfDrawContext &ctx) { return pdoc.add_pattern(ctx); }
```

### Comparing `capypdf-0.8.0/src/pdfgen.hpp` & `capypdf-0.9.0/src/pdfgen.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -132,31 +132,41 @@
 
     rvoe<CapyPDF_OutlineId>
     add_outline(const u8string &title_utf8, PageId dest, std::optional<CapyPDF_OutlineId> parent) {
         return pdoc.add_outline(title_utf8, dest, parent);
     }
 
     rvoe<CapyPDF_StructureItemId>
-    add_structure_item(const asciistring &stype, std::optional<CapyPDF_StructureItemId> parent) {
+    add_structure_item(const CapyPDF_StructureType stype,
+                       std::optional<CapyPDF_StructureItemId> parent) {
         return pdoc.add_structure_item(stype, parent);
     }
 
+    rvoe<CapyPDF_StructureItemId>
+    add_structure_item(const CapyPDF_RoleId role, std::optional<CapyPDF_StructureItemId> parent) {
+        return pdoc.add_structure_item(role, parent);
+    }
+
     rvoe<CapyPDF_OptionalContentGroupId> add_optional_content_group(const OptionalContentGroup &g) {
         return pdoc.add_optional_content_group(g);
     }
 
     int32_t num_pages() const { return (int32_t)pdoc.pages.size(); }
 
     std::optional<double>
     glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const {
         return pdoc.glyph_advance(fid, pointsize, codepoint);
     }
 
     rvoe<double> utf8_text_width(const u8string &txt, CapyPDF_FontId fid, double pointsize) const;
 
+    rvoe<CapyPDF_RoleId> add_rolemap_entry(std::string name, CapyPDF_StructureType builtin_type) {
+        return pdoc.add_rolemap_entry(std::move(name), builtin_type);
+    }
+
 private:
     PdfGen(std::filesystem::path ofilename,
            std::unique_ptr<FT_LibraryRec_, FT_Error (*)(FT_LibraryRec_ *)> ft,
            PdfDocument pdoc)
         : ofilename(std::move(ofilename)), ft(std::move(ft)), pdoc(std::move(pdoc)) {}
 
     std::filesystem::path ofilename;
```

### Comparing `capypdf-0.8.0/src/pdfparser.cpp` & `capypdf-0.9.0/src/pdfparser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 const std::regex objref{R"((^\d+)\s+(\d+)\s+R)"};
 const std::regex stringlit{R"(^/([a-zA-Z][-a-zA-Z0-9+]+))"};
 const std::regex stringobj{R"(^\()"};
 const std::regex endobj{R"(^endobj)"};
 const std::regex number{R"(^-?\d+)"};
 const std::regex real{R"(^(-?\d+\.\d+))"};
 const std::regex hexstr{R"(^<([0-9a-fA-F]+)>)"};
+const std::regex boolstr{R"(^(true|false)\b)"};
 
 } // namespace
 
 const char *text1 =
     R"(3 0 obj << /key /value /otherkey [ 1 0 R ] /StringKey (a \(b(c)) /intkey 55 /realkey 9.34 /hexkey <03830A0b> >> endobj)";
 
 const char *text2 = R"(9 0 obj
@@ -43,14 +44,15 @@
 /Flags 4
 /FontBBox[-543 -303 1278 982]/ItalicAngle 0
 /Ascent 891
 /Descent -216
 /CapHeight 981
 /StemV 80
 /FontFile2 7 0 R
+/BoolEntry true
 >>
 endobj
 )";
 
 int PdfLexer::lex_string(const char *t) {
     bool prev_was_backslash = false;
     int num_parens = 1;
@@ -127,19 +129,19 @@
             int64_t onum = atoll(text.c_str() + offset);
             int64_t version = atoll(text.c_str() + offset + m.position(2));
             offset += m.length();
             return PdfTokenObjRef(onum, version);
         } else if(std::regex_search(text.c_str() + offset, m, stringobj)) {
             ++offset;
             auto advance = lex_string(text.c_str() + offset);
-            if(advance < 0) {
+            if(advance <= 0) {
                 // std::cout << "\nParent string parsing failed.\n";
                 return PdfTokenError{};
             }
-            std::string temptext(text.c_str() + offset, advance);
+            std::string temptext(text.c_str() + offset, advance - 1);
             offset += advance;
             return PdfTokenString(std::move(temptext));
         } else if(std::regex_search(text.c_str() + offset, m, real)) {
             double value = strtod(text.c_str() + offset, nullptr);
             offset += m.length();
             return PdfTokenReal{value};
         } else if(std::regex_search(text.c_str() + offset, m, number)) {
@@ -149,14 +151,18 @@
         } else if(std::regex_search(text.c_str() + offset, m, endobj)) {
             offset += m.length();
             return PdfTokenEndObj{};
         } else if(std::regex_search(text.c_str() + offset, m, hexstr)) {
             std::string hexs(text.c_str() + offset + m.position(1), m.length(1));
             offset += m.length();
             return PdfTokenHexString{std::move(hexs)};
+        } else if(std::regex_search(text.c_str() + offset, m, boolstr)) {
+            std::string_view bools(text.c_str() + offset + m.position(1), m.length(1));
+            offset += m.length();
+            return PdfTokenBoolean{bools == "true"};
         } else {
             return PdfTokenError{};
         }
     }
     return PdfTokenFinished{};
 }
 
@@ -183,14 +189,17 @@
 std::optional<PdfValueElement> PdfParser::parse_value() {
     if(auto intval = accept<PdfTokenInteger>(); intval) {
         return intval->value;
     }
     if(auto realval = accept<PdfTokenReal>(); realval) {
         return realval->value;
     }
+    if(auto boolval = accept<PdfTokenBoolean>(); boolval) {
+        return boolval->value;
+    }
     if(auto refval = accept<PdfTokenObjRef>(); refval) {
         return PdfNodeObjRef{refval->objnum, refval->version};
     }
     if(auto strval = accept<PdfTokenString>(); strval) {
         return PdfNodeString{strval->text};
     }
     if(auto strval = accept<PdfTokenStringLiteral>(); strval) {
@@ -284,14 +293,17 @@
     const char *ind = with_indent ? indent.c_str() : "";
     if(std::holds_alternative<int64_t>(e)) {
         const auto &v = std::get<int64_t>(e);
         fmt::format_to(app, "{}{}\n", ind, v);
     } else if(std::holds_alternative<double>(e)) {
         const auto &v = std::get<double>(e);
         fmt::format_to(app, "{}{}\n", ind, v);
+    } else if(std::holds_alternative<bool>(e)) {
+        const auto &v = std::get<bool>(e);
+        fmt::format_to(app, "{}{}\n", ind, v ? "true" : "false");
     } else if(std::holds_alternative<PdfNodeArray>(e)) {
         const auto &v = std::get<PdfNodeArray>(e);
         fmt::format_to(app, "{}[\n", ind);
         indent += "    ";
         print_array(def.arrays[v.i]);
         indent.pop_back();
         indent.pop_back();
```

### Comparing `capypdf-0.8.0/src/pdfparser.hpp` & `capypdf-0.9.0/src/pdfparser.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     int64_t value;
 };
 
 struct PdfTokenReal {
     double value;
 };
 
+struct PdfTokenBoolean {
+    bool value;
+};
+
 struct PdfTokenEndObj {};
 
 struct PdfTokenFinished {};
 
 struct PdfTokenError {};
 
 typedef std::variant<PdfTokenDictStart,
@@ -68,14 +72,15 @@
                      PdfTokenStringLiteral,
                      PdfTokenObjName,
                      PdfTokenObjRef,
                      PdfTokenEndObj,
                      PdfTokenHexString,
                      PdfTokenInteger,
                      PdfTokenReal,
+                     PdfTokenBoolean,
                      PdfTokenError,
                      PdfTokenFinished>
     PdfToken;
 
 class PdfLexer {
 public:
     explicit PdfLexer(const char *t) : text(t), offset(0) {}
@@ -101,20 +106,22 @@
 };
 struct PdfNodeString {
     std::string value;
 };
 struct PdfNodeStringLiteral {
     std::string value;
 }; // Without leading slash.
+
 struct PdfNodeHexString {
     std::string value;
 };
 
 typedef std::variant<int64_t,
                      double,
+                     bool,
                      PdfNodeArray,
                      PdfNodeDict,
                      PdfNodeObjRef,
                      PdfNodeString,
                      PdfNodeStringLiteral,
                      PdfNodeHexString>
     PdfValueElement;
```

### Comparing `capypdf-0.8.0/src/pdftext.hpp` & `capypdf-0.9.0/src/pdftext.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 };
 
 struct Nonstroke_arg {
     Color c;
 };
 
 struct StructureItem {
-    asciistring name;
     CapyPDF_StructureItemId sid;
 };
 
 typedef std::variant<TStar_arg,
                      Tc_arg,
                      Td_arg,
                      TD_arg,
@@ -102,16 +101,16 @@
                      Nonstroke_arg>
     TextEvent;
 
 class PdfText {
 public:
     explicit PdfText(PdfDrawContext *dc) : dc{dc} {};
 
-    rvoe<NoReturnValue> cmd_BDC(const asciistring &name, CapyPDF_StructureItemId sid) {
-        events.emplace_back(StructureItem{name, sid});
+    rvoe<NoReturnValue> cmd_BDC(CapyPDF_StructureItemId sid) {
+        events.emplace_back(StructureItem{sid});
         RETOK;
     }
 
     rvoe<NoReturnValue> cmd_EMC() {
         events.emplace_back(Emc_arg{});
         RETOK;
     }
```

### Comparing `capypdf-0.8.0/src/pdfviewer.cpp` & `capypdf-0.9.0/src/pdfviewer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -532,13 +532,13 @@
 }
 
 } // namespace
 
 int main(int argc, char **argv) {
     App app;
     app.ifile = "title.pdf";
-    app.app = gtk_application_new("io.github.jpakkane.pdfviewer", G_APPLICATION_FLAGS_NONE);
+    app.app = gtk_application_new("io.github.jpakkane.pdfviewer", G_APPLICATION_DEFAULT_FLAGS);
     g_signal_connect(app.app, "activate", G_CALLBACK(activate), static_cast<gpointer>(&app));
     int status = g_application_run(G_APPLICATION(app.app), argc, argv);
     g_object_unref(app.app);
     return status;
 }
```

### Comparing `capypdf-0.8.0/src/subtype.cpp` & `capypdf-0.9.0/src/subtype.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/src/utils.cpp` & `capypdf-0.9.0/src/utils.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -258,19 +258,21 @@
             return false;
         }
     }
     return true;
 }
 
 // As in PDF 2.0 spec 7.3.5
-std::string bytes2pdfstringliteral(std::string_view raw) {
+std::string bytes2pdfstringliteral(std::string_view raw, bool add_slash) {
     std::string result;
     char buf[10];
     result.reserve(raw.size() + 1);
-    result.push_back('/');
+    if(add_slash) {
+        result.push_back('/');
+    }
     for(const unsigned char c : raw) {
         if(needs_quoting(c)) {
             result += '#';
             if(snprintf(buf, 10, "%02x", (unsigned int)c) != 2) {
                 std::abort();
             }
             result += buf;
```

### Comparing `capypdf-0.8.0/src/utils.hpp` & `capypdf-0.9.0/src/utils.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 
 std::string current_date_string();
 
 std::string pdfstring_quote(std::string_view raw_string);
 
 bool is_ascii(std::string_view text);
 
-std::string bytes2pdfstringliteral(std::string_view raw);
+std::string bytes2pdfstringliteral(std::string_view raw, bool add_slash = true);
 
 std::string create_trailer_id();
 
 } // namespace capypdf
```

### Comparing `capypdf-0.8.0/subprojects/fmt.wrap` & `capypdf-0.9.0/subprojects/zlib.wrap`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [wrap-file]
-directory = fmt-10.1.1
-source_url = https://github.com/fmtlib/fmt/archive/10.1.1.tar.gz
-source_filename = fmt-10.1.1.tar.gz
-source_hash = 78b8c0a72b1c35e4443a7e308df52498252d1cefc2b08c9a97bc9ee6cfe61f8b
-patch_filename = fmt_10.1.1-1_patch.zip
-patch_url = https://wrapdb.mesonbuild.com/v2/fmt_10.1.1-1/get_patch
-patch_hash = adec33acaf87c0859c52b242a44bc71c3427751da3f1adaed511f4186794a42f
-source_fallback_url = https://github.com/mesonbuild/wrapdb/releases/download/fmt_10.1.1-1/fmt-10.1.1.tar.gz
-wrapdb_version = 10.1.1-1
+directory = zlib-1.3.1
+source_url = http://zlib.net/fossils/zlib-1.3.1.tar.gz
+source_fallback_url = https://github.com/mesonbuild/wrapdb/releases/download/zlib_1.3.1-1/zlib-1.3.1.tar.gz
+source_filename = zlib-1.3.1.tar.gz
+source_hash = 9a93b2b7dfdac77ceba5a558a580e74667dd6fede4585b91eefb60f03b72df23
+patch_filename = zlib_1.3.1-1_patch.zip
+patch_url = https://wrapdb.mesonbuild.com/v2/zlib_1.3.1-1/get_patch
+patch_hash = e79b98eb24a75392009cec6f99ca5cdca9881ff20bfa174e8b8926d5c7a47095
+wrapdb_version = 1.3.1-1
 
 [provide]
-fmt = fmt_dep
+zlib = zlib_dep
```

### Comparing `capypdf-0.8.0/subprojects/libjpeg-turbo.wrap` & `capypdf-0.9.0/subprojects/libjpeg-turbo.wrap`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [wrap-file]
-directory = libjpeg-turbo-3.0.1
-source_url = https://sourceforge.net/projects/libjpeg-turbo/files/3.0.1/libjpeg-turbo-3.0.1.tar.gz
-source_filename = libjpeg-turbo-3.0.1.tar.gz
-source_hash = 22429507714ae147b3acacd299e82099fce5d9f456882fc28e252e4579ba2a75
-patch_filename = libjpeg-turbo_3.0.1-1_patch.zip
-patch_url = https://wrapdb.mesonbuild.com/v2/libjpeg-turbo_3.0.1-1/get_patch
-patch_hash = fe56c562a4be3d699f3948fb0ae9452445b94795540a7f6bd58e6fd2fd5b53cd
-source_fallback_url = https://github.com/mesonbuild/wrapdb/releases/download/libjpeg-turbo_3.0.1-1/libjpeg-turbo-3.0.1.tar.gz
-wrapdb_version = 3.0.1-1
+directory = libjpeg-turbo-3.0.2
+source_url = https://github.com/libjpeg-turbo/libjpeg-turbo/releases/download/3.0.2/libjpeg-turbo-3.0.2.tar.gz
+source_filename = libjpeg-turbo-3.0.2.tar.gz
+source_hash = c2ce515a78d91b09023773ef2770d6b0df77d674e144de80d63e0389b3a15ca6
+patch_filename = libjpeg-turbo_3.0.2-1_patch.zip
+patch_url = https://wrapdb.mesonbuild.com/v2/libjpeg-turbo_3.0.2-1/get_patch
+patch_hash = 271788065332bcb52d504edc86466dc802a705c64b825e018ed927371ac53cf1
+source_fallback_url = https://github.com/mesonbuild/wrapdb/releases/download/libjpeg-turbo_3.0.2-1/libjpeg-turbo-3.0.2.tar.gz
+wrapdb_version = 3.0.2-1
 
 [provide]
 dependency_names = libjpeg, libturbojpeg
```

### Comparing `capypdf-0.8.0/subprojects/libtiff.wrap` & `capypdf-0.9.0/subprojects/libtiff.wrap`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/test/capypdftests.py` & `capypdf-0.9.0/test/capypdftests.py`

 * *Files 3% similar despite different names*

```diff
@@ -892,55 +892,85 @@
 
     @validate_image('python_tagged', 200, 200)
     def test_tagged(self, ofilename, w, h):
         prop = capypdf.PageProperties()
         prop.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         opt = capypdf.Options()
         opt.set_default_page_properties(prop)
+        opt.set_tagged(True)
         with capypdf.Generator(ofilename, opt) as gen:
             fid = gen.load_font(noto_fontdir / 'NotoSerif-Regular.ttf')
             bfid = gen.load_font(noto_fontdir / 'NotoSans-Bold.ttf')
-            title = 'This is the title'
+            title = 'H1 element'
+            doc_id = gen.add_structure_item(capypdf.StructureType.Document)
+
             with gen.page_draw_context() as ctx:
-                tw = gen.text_width(title,bfid, 16)
-                with ctx.cmd_BMC('/Title'):
-                    ctx.render_text(title, bfid, 16, 100-tw/2, 170)
-                with ctx.cmd_BMC('/Artifact'):
+                tw = gen.text_width(title,bfid, 14)
+                title_id = gen.add_structure_item(capypdf.StructureType.H1, doc_id)
+                with ctx.cmd_BDC_builtin(title_id):
+                    ctx.render_text(title, bfid, 14, 100-tw/2, 170)
+                with ctx.cmd_BMC('Artifact'):
                     ctx.cmd_w(1.5)
                     ctx.cmd_m(50, 155)
                     ctx.cmd_l(150, 155)
                     ctx.cmd_S()
-                with ctx.cmd_BMC('/p'):
+                with ctx.cmd_BDC_builtin(gen.add_structure_item(capypdf.StructureType.P, doc_id)):
                     with ctx.text_new() as t:
                         t.cmd_Td(20, 130)
                         t.cmd_Tf(fid, 8)
                         t.cmd_TL(10)
-                        t.render_text('This is a single paragraph of text that')
-                        t.cmd_Tstar()
-                        t.render_text('contains multiple lines.')
-                with ctx.cmd_BMC('/p'):
+                        t.render_text('Text object inside marked content')
+                with ctx.text_new() as t:
+                    t.cmd_Td(20, 100)
+                    t.cmd_Tf(fid, 8)
+                    t.cmd_TL(10)
+                    with t.cmd_BDC_builtin(gen.add_structure_item(capypdf.StructureType.P, doc_id)):
+                        t.render_text('Marked content inside text object.')
+
+    @validate_image('python_customroles', 200, 200)
+    def test_tagged(self, ofilename, w, h):
+        prop = capypdf.PageProperties()
+        prop.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
+        opt = capypdf.Options()
+        opt.set_default_page_properties(prop)
+        opt.set_tagged(True)
+        with capypdf.Generator(ofilename, opt) as gen:
+            fid = gen.load_font(noto_fontdir / 'NotoSerif-Regular.ttf')
+            bfid = gen.load_font(noto_fontdir / 'NotoSans-Bold.ttf')
+            title = 'Headline text'
+            head_role = gen.add_rolemap_entry("Headline", capypdf.StructureType.H1)
+            text_role = gen.add_rolemap_entry("Text body", capypdf.StructureType.P)
+            doc_id = gen.add_structure_item(capypdf.StructureType.Document)
+
+            with gen.page_draw_context() as ctx:
+                tw = gen.text_width(title,bfid, 14)
+                title_id = gen.add_structure_item(head_role, doc_id)
+                with ctx.cmd_BDC_builtin(title_id):
+                    ctx.render_text(title, bfid, 14, 100-tw/2, 170)
+                with ctx.cmd_BDC_builtin(gen.add_structure_item(text_role, doc_id)):
                     with ctx.text_new() as t:
-                        t.cmd_Td(20, 100)
+                        t.cmd_Td(20, 130)
                         t.cmd_Tf(fid, 8)
                         t.cmd_TL(10)
-                        t.render_text('This is a second paragraph that also')
-                        t.cmd_Tstar()
-                        t.render_text('contains multiple lines. It even')
-                        t.cmd_Tstar()
-                        t.render_text('contains more than one sentence.')
-        # NOTE: not actually tagged yet, only marked.
-        # Needs a structure tree but that is not yet implemented.
+                        t.render_text('Text object inside custom role mark.')
+                with ctx.text_new() as t:
+                    t.cmd_Td(20, 100)
+                    t.cmd_Tf(fid, 8)
+                    t.cmd_TL(10)
+                    with t.cmd_BDC_builtin(gen.add_structure_item(text_role, doc_id)):
+                        t.render_text('Custom role mark inside text object.')
+
 
     @validate_image('python_printersmark', 200, 200)
     def test_printersmark(self, ofilename, w, h):
         cropmark_size = 5
         bleed_size = 2*cropmark_size
         prop = capypdf.PageProperties()
         prop.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
-        prop.set_pagebox(capypdf.PageBox.Art, bleed_size, bleed_size, w - 2*bleed_size, h - 2*bleed_size)
+        prop.set_pagebox(capypdf.PageBox.Trim, bleed_size, bleed_size, w - 2*bleed_size, h - 2*bleed_size)
         opt = capypdf.Options()
         opt.set_default_page_properties(prop)
         with capypdf.Generator(ofilename, opt) as gen:
             vctx = capypdf.FormXObjectDrawContext(gen, 1, cropmark_size)
             vctx.cmd_re(0, 0, 1, cropmark_size)
             vctx.cmd_f()
             vid = gen.add_form_xobject(vctx)
@@ -949,34 +979,37 @@
             hctx.cmd_re(0, 0, cropmark_size, 1)
             hctx.cmd_f()
             hid = gen.add_form_xobject(hctx)
             del hctx
             with gen.page_draw_context() as ctx:
                 ctx.cmd_rg(0.9, 0.1, 0.1)
                 ctx.cmd_re(bleed_size, bleed_size, w-2*bleed_size, h-2*bleed_size)
-                #ctx.cmd_re(10, 10, 20, 20)
                 ctx.cmd_f()
 
                 # Vertical annotations
                 a = capypdf.Annotation.new_printers_mark_annotation(vid)
                 a.set_rectangle(bleed_size-0.5, 0, bleed_size+.5, cropmark_size)
+                a.set_flags(capypdf.AnnotationFlag.Print | capypdf.AnnotationFlag.ReadOnly)
                 aid = gen.create_annotation(a)
                 ctx.annotate(aid)
                 a = capypdf.Annotation.new_printers_mark_annotation(vid)
                 a.set_rectangle(bleed_size-0.5, h-cropmark_size, bleed_size+.5, h)
+                a.set_flags(capypdf.AnnotationFlag.Print | capypdf.AnnotationFlag.ReadOnly)
                 aid = gen.create_annotation(a)
                 ctx.annotate(aid)
 
                 # Horizontal annotations
                 a = capypdf.Annotation.new_printers_mark_annotation(hid)
                 a.set_rectangle(0, bleed_size - 0.5, cropmark_size, bleed_size+.5)
+                a.set_flags(capypdf.AnnotationFlag.Print | capypdf.AnnotationFlag.ReadOnly)
                 aid = gen.create_annotation(a)
                 ctx.annotate(aid)
                 a = capypdf.Annotation.new_printers_mark_annotation(hid)
                 a.set_rectangle(0, h - bleed_size - 0.5, cropmark_size, h - bleed_size+.5)
+                a.set_flags(capypdf.AnnotationFlag.Print | capypdf.AnnotationFlag.ReadOnly)
                 aid = gen.create_annotation(a)
                 ctx.annotate(aid)
 
                 # The other corners would go here, but I'm lazy.
 
 
 if __name__ == "__main__":
```

### Comparing `capypdf-0.8.0/test/ctest.c` & `capypdf-0.9.0/test/ctest.c`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/test/syntaxchecks.py` & `capypdf-0.9.0/test/syntaxchecks.py`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_annotate.png` & `capypdf-0.9.0/testoutput/python_annotate.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_blendmodes.png` & `capypdf-0.9.0/testoutput/python_blendmodes.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_colorpattern.png` & `capypdf-0.9.0/testoutput/python_colorpattern.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_gstate.png` & `capypdf-0.9.0/testoutput/python_gstate.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_icccolor.png` & `capypdf-0.9.0/testoutput/python_icccolor.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_image.png` & `capypdf-0.9.0/testoutput/python_image.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_imagemask.png` & `capypdf-0.9.0/testoutput/python_imagemask.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_linestyles.png` & `capypdf-0.9.0/testoutput/python_linestyles.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_path.png` & `capypdf-0.9.0/testoutput/python_path.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_rasterimage.png` & `capypdf-0.9.0/testoutput/python_rasterimage.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_separation.png` & `capypdf-0.9.0/testoutput/python_separation.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_shading_cmyk.png` & `capypdf-0.9.0/testoutput/python_shading_cmyk.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_shading_gray.png` & `capypdf-0.9.0/testoutput/python_shading_gray.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_shading_rgb.png` & `capypdf-0.9.0/testoutput/python_shading_rgb.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_simple.png` & `capypdf-0.9.0/testoutput/python_simple.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_text.png` & `capypdf-0.9.0/testoutput/python_text.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/testoutput/python_textobj.png` & `capypdf-0.9.0/testoutput/python_textobj.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/tools/presentationtool.py` & `capypdf-0.9.0/tools/presentationtool.py`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/tools/x3gen.py` & `capypdf-0.9.0/tools/x3gen.py`

 * *Files identical despite different names*

### Comparing `capypdf-0.8.0/PKG-INFO` & `capypdf-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capypdf
-Version: 0.8.0
+Version: 0.9.0
 Summary: A color managed PDF generation library tech preview
 Author-Email: Jussi Pakkanen <jpakkane@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

