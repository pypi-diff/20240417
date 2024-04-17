# Comparing `tmp/babelfont-3.0.1.tar.gz` & `tmp/babelfont-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelfont-3.0.1.tar", max compression
+gzip compressed data, was "babelfont-3.0.2.tar", last modified: Wed Apr 17 09:51:00 2024, max compression
```

## Comparing `babelfont-3.0.1.tar` & `babelfont-3.0.2.tar`

### file list

```diff
@@ -1,30 +1,291 @@
--rw-r--r--   0        0        0    11358 2023-06-06 14:10:29.366930 babelfont-3.0.1/LICENSE
--rw-r--r--   0        0        0     1487 2022-10-19 21:49:42.369264 babelfont-3.0.1/README.md
--rw-r--r--   0        0        0      601 2023-06-15 09:25:27.322460 babelfont-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      211 2022-10-19 21:49:42.371205 babelfont-3.0.1/src/babelfont/Anchor.py
--rw-r--r--   0        0        0     3493 2023-06-06 15:32:36.882623 babelfont-3.0.1/src/babelfont/Axis.py
--rw-r--r--   0        0        0     7637 2022-10-19 21:49:42.371911 babelfont-3.0.1/src/babelfont/BaseObject.py
--rw-r--r--   0        0        0      224 2022-10-19 21:49:42.372255 babelfont-3.0.1/src/babelfont/Component.py
--rw-r--r--   0        0        0     7461 2022-10-19 21:49:42.372605 babelfont-3.0.1/src/babelfont/Font.py
--rw-r--r--   0        0        0     1544 2022-10-19 21:49:42.373015 babelfont-3.0.1/src/babelfont/Glyph.py
--rw-r--r--   0        0        0      242 2022-10-19 21:49:42.373332 babelfont-3.0.1/src/babelfont/Guide.py
--rw-r--r--   0        0        0     1256 2022-10-19 21:49:42.373694 babelfont-3.0.1/src/babelfont/Instance.py
--rw-r--r--   0        0        0     4549 2022-10-19 21:49:42.374044 babelfont-3.0.1/src/babelfont/Layer.py
--rw-r--r--   0        0        0     3123 2022-10-19 21:49:42.374368 babelfont-3.0.1/src/babelfont/Master.py
--rw-r--r--   0        0        0     1318 2022-10-19 21:49:42.374742 babelfont-3.0.1/src/babelfont/Names.py
--rw-r--r--   0        0        0      767 2022-10-19 21:49:42.375075 babelfont-3.0.1/src/babelfont/Node.py
--rw-r--r--   0        0        0     1469 2022-10-19 21:49:42.375377 babelfont-3.0.1/src/babelfont/Shape.py
--rw-r--r--   0        0        0      566 2022-10-19 21:49:42.375788 babelfont-3.0.1/src/babelfont/__init__.py
--rw-r--r--   0        0        0      738 2022-10-19 21:49:42.376105 babelfont-3.0.1/src/babelfont/__main__.py
--rw-r--r--   0        0        0     2194 2022-10-19 21:49:42.376432 babelfont-3.0.1/src/babelfont/convertors/__init__.py
--rw-r--r--   0        0        0     7521 2022-10-19 21:49:42.376767 babelfont-3.0.1/src/babelfont/convertors/designspace.py
--rw-r--r--   0        0        0     6822 2022-10-19 21:49:42.377119 babelfont-3.0.1/src/babelfont/convertors/fontlab.py
--rw-r--r--   0        0        0    30419 2023-05-22 11:43:03.853417 babelfont-3.0.1/src/babelfont/convertors/glyphs.py
--rw-r--r--   0        0        0    14882 2023-05-22 11:36:45.328197 babelfont-3.0.1/src/babelfont/convertors/gsobject.py
--rw-r--r--   0        0        0     3887 2022-10-19 21:49:42.378291 babelfont-3.0.1/src/babelfont/convertors/nfsf.py
--rw-r--r--   0        0        0    16280 2023-06-06 15:32:22.421394 babelfont-3.0.1/src/babelfont/convertors/truetype.py
--rw-r--r--   0        0        0      718 2022-10-19 21:49:42.378991 babelfont-3.0.1/src/babelfont/convertors/ufo.py
--rw-r--r--   0        0        0        0 2022-10-19 21:49:42.379066 babelfont-3.0.1/src/babelfont/fontFilters/__init__.py
--rw-r--r--   0        0        0     2456 2022-10-19 21:49:42.379370 babelfont-3.0.1/src/babelfont/fontFilters/featureWriters.py
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 babelfont-3.0.1/setup.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 babelfont-3.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 09:50:53.000000 babelfont-3.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.454701 babelfont-3.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:50:53.000000 babelfont-3.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:50:53.000000 babelfont-3.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 09:50:53.000000 babelfont-3.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 09:50:53.000000 babelfont-3.0.2/AUTHORS.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.454701 babelfont-3.0.2/Babelfont.glyphsFileFormat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/MacOS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120208 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/MacOS/plugin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:50:53.000000 babelfont-3.0.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 09:50:53.000000 babelfont-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-17 09:50:53.000000 babelfont-3.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-17 09:51:00.502701 babelfont-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 09:50:53.000000 babelfont-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Anchor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Axis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Font.md
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Gemfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Glyph.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Instance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Master.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Names.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Shape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/_data/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    36234 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-17 09:50:53.000000 babelfont-3.0.2/makedoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56244 2024-04-17 09:50:53.000000 babelfont-3.0.2/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 09:50:53.000000 babelfont-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:51:00.502701 babelfont-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.458701 babelfont-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.466701 babelfont-3.0.2/src/babelfont/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/BaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.466701 babelfont-3.0.2/src/babelfont/convertors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontforge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/convertors/fontlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontlab/vfj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/convertors/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26782 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphspackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/nfsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/ufo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/fontFilters/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/anchorPropagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/featureWriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/marks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/src/babelfont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 09:50:53.000000 babelfont-3.0.2/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.474701 babelfont-3.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1118555 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Castoro Roman.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Glyphs2ManyAxes.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/GlyphsFileFormatv3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/GlyphsFileFormatv3.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/LICENSE_MutatorSans
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/LICENSE_UbuTestData.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/NewFont-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Nunito-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   157208 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53914 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/SimpleTwoAxis.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/SimpleTwoAxis3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.474701 babelfont-3.0.2/tests/data/Test1.roundtrip.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.roundtrip.ufo/features.fea
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/Test1.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/i.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/idotless.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)   432392 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Ysabeau[wght].ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/glyphsLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestBasic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFileName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInactive.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.482701 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/order.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/TestReencode.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.482701 babelfont-3.0.2/tests/data/glyphsLib/master_ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/tests/data/testotfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c2c3fc37b2d4c3cb2ef726c6cdaaabd4b7f3eb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125256 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    21160 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    22980 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/HBTest-VF.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/MORXTwentyeight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/TRAK.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106096 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs3_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_otf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_ufo_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_vfj_loader.py
```

### Comparing `babelfont-3.0.1/LICENSE` & `babelfont-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.1/README.md` & `babelfont-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.1/src/babelfont/Axis.py` & `babelfont-3.0.2/src/babelfont/Axis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional, Dict, Tuple
 from .BaseObject import BaseObject, I18NDictionary
 from dataclasses import dataclass, field
 import uuid
 from fontTools.varLib.models import normalizeValue
 
 
 @dataclass
@@ -43,14 +44,22 @@
     )
     map: [(int, int)] = field(
         default=None,
         metadata={
             "description": """The mapping between userspace and designspace coordinates."""
         },
     )
+    hidden: bool = field(
+        default=False,
+        metadata={
+            "description": """If `True`, this axis is hidden from the user interface.
+            Hidden axes are used for internal font generation and are not displayed in the
+            user interface."""
+        },
+    )
 
 
 @dataclass
 class Axis(BaseObject, _AxisFields):
     """Represents an axis in a multiple master or variable font."""
 
     _write_one_line = True
@@ -59,15 +68,20 @@
         # If they smacked my name with a bare string, replace with I18NDict
         if isinstance(self.name, str):
             self.name = I18NDictionary.with_default(self.name)
         super().__post_init__()
 
     def normalize_value(self, value):
         return normalizeValue(
-            value, (self.map_forward(self.min), self.map_forward(self.default), self.map_forward(self.max))
+            self.map_forward(value),
+            (
+                self.map_forward(self.min),
+                self.map_forward(self.default),
+                self.map_forward(self.max),
+            ),
         )
 
     def denormalize_value(self, value):
         if value == 0:
             return self.default
         elif value > 0:
             return self.default + (self.max - self.default) * value
@@ -96,22 +110,35 @@
     def axisTag(self):
         return self.tag
 
     @property
     def defaultValue(self):
         return self.default
 
+    @property
+    def inverted_map(self) -> Optional[Tuple[float, float]]:
+        if not self.map:
+            return None
+        return [(v, k) for k, v in self.map]
+
     # Stolen from fontTools.designspaceLib
 
     def map_forward(self, v):
         from fontTools.varLib.models import piecewiseLinearMap
 
         if not self.map:
             return v
-        return piecewiseLinearMap(v, {k: v for k, v in self.map.items()})
+        return piecewiseLinearMap(v, dict(self.map))
 
     def map_backward(self, v):
         from fontTools.varLib.models import piecewiseLinearMap
 
         if not self.map:
             return v
-        return piecewiseLinearMap(v, {v: k for k, v in self.map.items()})
+        return piecewiseLinearMap(v, {v: k for k, v in self.map})
+
+    # These are just better names
+    def userspace_to_designspace(self, v):
+        return self.map_forward(v)
+
+    def designspace_to_userspace(self, v):
+        return self.map_backward(v)
```

### Comparing `babelfont-3.0.1/src/babelfont/BaseObject.py` & `babelfont-3.0.2/src/babelfont/BaseObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from dataclasses import dataclass, fields, field
 import orjson
-from io import StringIO
 from collections import namedtuple
 import datetime
 
 
 class IncompatibleMastersError(ValueError):
     pass
 
+
 Color = namedtuple("Color", "r,g,b,a", defaults=[0, 0, 0, 0])
 Position = namedtuple("Position", "x,y,angle", defaults=[0, 0, 0])
-OTValue = namedtuple("OTValue", "table,field,value")
+
+
+@dataclass
+class OTValue:
+    table: str
+    field: str
+    value: any
+
 
 class I18NDictionary(dict):
     @classmethod
     def with_default(cls, s):
         inst = cls()
         inst.set_default(s)
         return inst
@@ -33,16 +40,14 @@
             return self.get_default()
 
     def get_default(self):
         if "dflt" in self:
             return self["dflt"]
         elif len(list(self.values())):
             return list(self.values())[0]
-        else:
-            return "unknown"
 
     def set_default(self, value):
         if value:
             self["dflt"] = value
 
     def write(self, stream, indent):
         if len(self.keys()) > 1:
@@ -55,17 +60,17 @@
         rv = dict(self)
         if "dflt" in rv:
             if "en" not in rv:
                 rv["en"] = rv["dflt"]
             del rv["dflt"]
         return rv
 
+
 @dataclass
 class BaseObject:
-
     # OK, what's going on here? And why do we split _FoobarFields from Foobar?
     # We want to achieve the following:
     #    * A ``_formatspecific`` field on *every* derived object...
     #    * ...which does not need to be added to the constructor arguments
     #    * ...but which (for convenience when instantiating from JSON) has an
     #      alias of ``_`` which *can* be added to the constructor arguments
 
@@ -120,16 +125,16 @@
         return False
 
     def _write_value(self, stream, k, v, indent=0):
         if hasattr(v, "write"):
             v.write(stream, indent + 1)
         elif isinstance(v, tuple):
             stream.write(b"[")
-            for ix, l in enumerate(v):
-                self._write_value(stream, k, l, indent + 1)
+            for ix, entry in enumerate(v):
+                self._write_value(stream, k, entry, indent + 1)
                 if ix < len(v) - 1:
                     stream.write(b", ")
             stream.write(b"]")
         elif isinstance(v, dict):
             stream.write(b"{")
             for ix, (k1, v1) in enumerate(v.items()):
                 if self._should_separate_when_serializing(k):
@@ -143,19 +148,19 @@
                 stream.write(b": ")
                 self._write_value(stream, k, v1, indent + 1)
                 if ix < len(v.items()) - 1:
                     stream.write(b", ")
             stream.write(b"}")
         elif isinstance(v, list):
             stream.write(b"[")
-            for ix, l in enumerate(v):
+            for ix, item in enumerate(v):
                 if self._should_separate_when_serializing(k):
                     stream.write(b"\n")
                     stream.write(b"  " * (indent + 2))
-                self._write_value(stream, k, l, indent + 1)
+                self._write_value(stream, k, item, indent + 1)
                 if ix < len(v) - 1:
                     stream.write(b", ")
             if self._should_separate_when_serializing(k):
                 stream.write(b"\n")
                 stream.write(b"  " * (indent + 1))
             stream.write(b"]")
         elif isinstance(v, datetime.datetime):
@@ -170,15 +175,17 @@
         towrite = []
         for f in fields(self):
             k = f.name
             if "skip_serialize" in f.metadata or "python_only" in f.metadata:
                 continue
             v = getattr(self, k)
             default = f.default
-            if (not v and not "serialize_if_false" in f.metadata) or (default and v == default):
+            if (not v and "serialize_if_false" not in f.metadata) or (
+                default and v == default
+            ):
                 continue
             towrite.append((k, v))
 
         for ix, (k, v) in enumerate(towrite):
             if not self._write_one_line:
                 stream.write(b"\n")
                 stream.write(b"  " * (indent + 1))
```

### Comparing `babelfont-3.0.1/src/babelfont/Font.py` & `babelfont-3.0.2/src/babelfont/Font.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import functools
+import logging
 from dataclasses import dataclass, field
 from datetime import datetime
-from .BaseObject import BaseObject, OTValue, IncompatibleMastersError
-from .Glyph import GlyphList
+from typing import Dict, List
+
+from fontTools.feaLib.variableScalar import VariableScalar
+from fontTools.varLib.models import VariationModel
+
 from .Axis import Axis
+from .BaseObject import BaseObject, IncompatibleMastersError, OTValue
+from .Features import Features
+from .Glyph import GlyphList
 from .Instance import Instance
 from .Master import Master
 from .Names import Names
-import functools
-from fontTools.varLib.models import VariationModel
-from fontFeatures import FontFeatures
-from fontTools.feaLib.variableScalar import VariableScalar
-import fontFeatures
-import logging
-
 
 log = logging.getLogger(__name__)
 
+
 @dataclass
 class _FontFields:
     upm: int = field(default=1000, metadata={"description": "The font's units per em."})
     version: (int, int) = field(
         default=(1, 0),
         metadata={
             "description": "Font version number as a tuple of integers (major, minor).",
@@ -87,24 +89,35 @@
             "json_type": "str",
         },
     )
     names: Names = field(default_factory=Names, metadata={"skip_serialize": True})
     customOpenTypeValues: [OTValue] = field(
         default_factory=list,
         metadata={
-            "description": "Any values to be placed in OpenType tables on export to override defaults"
+            "description": "Any values to be placed in OpenType tables on export to override defaults; these must be font-wide. Metrics which may vary by master should be placed in the `metrics` field of a Master."
         },
     )
-    features: FontFeatures = field(
-        default_factory=FontFeatures,
+    features: Features = field(
+        default_factory=Features,
         metadata={
-            "skip_serialize": True,
             "description": "A representation of the font's OpenType features",
         },
     )
+    first_kern_groups: Dict[str, List[str]] = field(
+        default_factory=dict,
+        metadata={
+            "description": "A dictionary of kerning groups, where the key is the group name and the value is a list of glyph names in the group."
+        },
+    )
+    second_kern_groups: Dict[str, List[str]] = field(
+        default_factory=dict,
+        metadata={
+            "description": "A dictionary of kerning groups, where the key is the group name and the value is a list of glyph names in the group."
+        },
+    )
 
 
 @dataclass
 class Font(_FontFields, BaseObject):
     """Represents a font, with one or more masters."""
 
     def __repr__(self):
@@ -133,15 +146,15 @@
         for a in self.axes:
             if a.tag in location2:
                 location2[a.tag] = a.map_backward(location2[a.tag])
         return location2
 
     @functools.cached_property
     def default_master(self):
-        default_loc = {a.tag: a.map_forward(a.default) for a in self.axes}
+        default_loc = {a.tag: a.userspace_to_designspace(a.default) for a in self.axes}
         for m in self.masters:
             if m.location == default_loc:
                 return m
         if len(self.masters) == 1:
             return self.masters[0]
         raise ValueError("Could not determine default master")
 
@@ -166,41 +179,44 @@
             axisOrder=[a.tag for a in self.axes],
         )
 
     @functools.cached_property
     def _all_kerning(self):
         all_keys = [set(m.kerning.keys()) for m in self.masters]
         kerndict = {}
-        for (l, r) in list(set().union(*all_keys)):
+        for left, right in list(set().union(*all_keys)):
             kern = VariableScalar()
             kern.axes = self.axes
             for m in self.masters:
-                thiskern = m.kerning.get((l, r), 0)
-                if (l, r) not in m.kerning:
+                thiskern = m.kerning.get((left, right), 0)
+                if (left, right) not in m.kerning:
                     log.debug(
                         "Master %s did not define a kern pair for (%s, %s), using 0"
-                        % (m.name.get_default(), l, r)
+                        % (m.name.get_default(), left, right)
                     )
                 kern.add_value(m.location, thiskern)
-            kerndict[(l, r)] = kern
+            kerndict[(left, right)] = kern
         return kerndict
 
     @functools.cached_property
     def _all_anchors(self):
         _all_anchors_dict = {}
         for g in sorted(self.glyphs.keys()):
             default_layer = self.default_master.get_glyph_layer(g)
             has_mark = None
             for a in default_layer.anchors_dict.keys():
                 if a[0] == "_":
                     if has_mark:
-                        log.warning("Glyph %s tried to be in two mark classes (%s, %s). The first one will win." % (g, has_mark, a))
+                        log.warning(
+                            "Glyph %s tried to be in two mark classes (%s, %s). The first one will win."
+                            % (g, has_mark, a)
+                        )
                         continue
                     has_mark = a
-                if not a in _all_anchors_dict:
+                if a not in _all_anchors_dict:
                     _all_anchors_dict[a] = {}
                 _all_anchors_dict[a][g] = self.get_variable_anchor(g, a)
         return _all_anchors_dict
 
     def get_variable_anchor(self, glyph, anchorname):
         x_vs = VariableScalar()
         x_vs.axes = self.axes
```

### Comparing `babelfont-3.0.1/src/babelfont/Glyph.py` & `babelfont-3.0.2/src/babelfont/Glyph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,60 @@
+from typing import Optional, List
+
 from dataclasses import dataclass, field
 from .BaseObject import BaseObject
 from .Layer import Layer
 from fontTools.misc.filenames import userNameToFileName
 import os
 
 
+@dataclass
+class _GlyphFields:
+    name: str
+    production_name: Optional[str] = None
+    category: str = "base"
+    codepoints: List[int] = field(default_factory=list)
+    layers: List[Layer] = field(
+        default_factory=list, repr=False, metadata={"skip_serialize": True}
+    )
+    exported: bool = field(default=True, metadata={"serialize_if_false": True})
+    direction: str = field(default="LTR", repr=False)
+
+
+@dataclass
+class Glyph(BaseObject, _GlyphFields):
+    _write_one_line = True
+
+    @property
+    def babelfont_filename(self):
+        return os.path.join("glyphs", (userNameToFileName(self.name) + ".nfsglyph"))
+
+
 class GlyphList(dict):
     def append(self, thing):
         self[thing.name] = thing
 
     def write(self, stream, indent):
         stream.write(b"[")
-        for ix, l in enumerate(self):
+        for ix, item in enumerate(self):
             stream.write(b"\n")
             stream.write(b"  " * (indent + 2))
-            l.write(stream, indent + 1)
+            item.write(stream, indent + 1)
             if ix < len(self) - 1:
                 stream.write(b", ")
             else:
                 stream.write(b"\n")
         stream.write(b"]")
 
-    def __iter__(self):
+    def __iter__(self) -> "GlyphList":
         self._n = 0
         self._values = list(self.values())
         return self
 
-    def __next__(self):
+    def __next__(self) -> Glyph:
         if self._n < len(self._values):
             result = self._values[self._n]
             self._n += 1
             return result
         else:
             raise StopIteration
 
-@dataclass
-class _GlyphFields:
-    name: str
-    production_name: str = None
-    category: str = "base"
-    codepoints: [int] = field(default_factory=list)
-    layers: [Layer] = field(default_factory=list, repr=False, metadata={"skip_serialize": True})
-    exported: bool = field(default=True, metadata={"serialize_if_false": True})
-    direction: str = field(default="LTR", repr=False)
-
-
-@dataclass
-class Glyph(BaseObject, _GlyphFields):
-
-    _write_one_line = True
-
-    @property
-    def babelfont_filename(self):
-        return os.path.join("glyphs", (userNameToFileName(self.name) + ".nfsglyph"))
-
```

### Comparing `babelfont-3.0.1/src/babelfont/Instance.py` & `babelfont-3.0.2/src/babelfont/Instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 class _InstanceFields:
     name: I18NDictionary = field(metadata={"description": "The name of this instance."})
     location: dict = field(
         metadata={
             "description": """A dictionary mapping axis tags to coordinates in order to locate this instance in the design space."""
         }
     )
-    styleName: I18NDictionary = field(default_factory=I18NDictionary,
-        metadata={"description": "The style name of this instance."})
-
+    styleName: I18NDictionary = field(
+        default_factory=I18NDictionary,
+        metadata={"description": "The style name of this instance."},
+    )
 
 
 @dataclass
 class Instance(BaseObject, _InstanceFields):
     """An object representing a named or static instance."""
 
     _write_one_line = True
 
-
     def __post_init__(self):
         # If they smacked my name with a bare string, replace with I18NDict
         if isinstance(self.name, str):
             self.name = I18NDictionary.with_default(self.name)
         if isinstance(self.styleName, str):
             self.styleName = I18NDictionary.with_default(self.styleName)
         super().__post_init__()
```

### Comparing `babelfont-3.0.1/src/babelfont/Layer.py` & `babelfont-3.0.2/src/babelfont/Layer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,123 @@
 from dataclasses import dataclass, field
 from functools import cached_property
+from typing import List, Optional
 
-from fontTools.ufoLib.pointPen import PointToSegmentPen, SegmentToPointPen, AbstractPointPen
+from fontTools.ufoLib.pointPen import (
+    PointToSegmentPen,
+    SegmentToPointPen,
+    AbstractPointPen,
+)
 from fontTools.pens.boundsPen import BoundsPen
 from fontTools.pens.recordingPen import DecomposingRecordingPen
 
 from .BaseObject import BaseObject, Color
 from .Guide import Guide
 from .Anchor import Anchor
 from .Node import Node
 from .Shape import Shape
 import uuid
 
 
 @dataclass
 class _LayerFields:
     width: int = 0
+    height: int = 0
+    vertWidth: Optional[int] = None
     name: str = None
     _master: str = None
-    id: str = field(default_factory = lambda: str(uuid.uuid1()))
-    guides: [Guide] = field(default_factory = list, repr=False)
-    shapes: [Shape] = field(default_factory=list, repr=False, metadata={"separate_items": True})
-    anchors: [Anchor] = field(default_factory = list, repr=False)
+    id: str = field(default_factory=lambda: str(uuid.uuid1()))
+    guides: List[Guide] = field(default_factory=list, repr=False)
+    shapes: List[Shape] = field(
+        default_factory=list, repr=False, metadata={"separate_items": True}
+    )
+    anchors: List[Anchor] = field(default_factory=list, repr=False)
     color: Color = None
     layerIndex: int = 0
-    # hints: [Hint]
-    _background: str = field(default=None,repr=False)
-    isBackground: bool = field(default=False,repr=False)
-    location: [float] = None
-    _font: object = field(
+    # hints: List[Hint]
+    background: Optional[str] = field(default=None, repr=False)
+    isBackground: bool = field(default=False, repr=False)
+    location: List[float] = None
+    _font: Optional["Font"] = field(
         default=None, repr=False, metadata={"python_only": True}
-    )  # Can't type Font because of circularity
+    )
+    _glyph: Optional["Glyph"] = field(
+        default=None, repr=False, metadata={"python_only": True}
+    )
 
 
 @dataclass
 class Layer(BaseObject, _LayerFields):
     @property
     def master(self):
         assert self._font
+        if not self._master:
+            return None
         return self._font.master(self._master)
 
     @property
-    def paths(self):
+    def paths(self) -> List[Shape]:
         return [x for x in self.shapes if x.is_path]
 
     @property
-    def components(self):
+    def components(self) -> List[Shape]:
         return [x for x in self.shapes if x.is_component]
 
-    def recursiveComponentSet(self):
+    def recursive_component_set(self):
         mine = set([x.ref for x in self.components])
         theirs = set()
         for c in mine:
-            theirs |= self.master.get_glyph_layer(c).recursiveComponentSet()
+            other_layer = self.master.get_glyph_layer(c)
+            theirs |= other_layer.recursive_component_set()
         return mine | theirs
 
+    def _background_of(self) -> Optional["Layer"]:
+        for layer in self._glyph.layers:
+            if layer.background == self.id:
+                return layer
+
+    def _background_layer(self) -> Optional["Layer"]:
+        if not self.background:
+            return
+        for layer in self._glyph.layers:
+            if layer.id == self.background:
+                return layer
+
+    def _nested_component_dict(self) -> dict[str, "Layer"]:
+        result = {}
+        todo = [x.ref for x in self.components]
+        while todo:
+            current = todo.pop()
+            if current in result:
+                continue
+            if self.master:
+                result[current] = self.master.get_glyph_layer(current)
+            else:
+                # Find a glyph with same layerid?
+                for layer in self._font.glyphs[current].layers:
+                    if layer.id == self.id:
+                        result[current] = layer
+                        break
+                if current not in result and self.isBackground:
+                    master_layer = self._background_of()
+                    if master_layer:
+                        master = master_layer._font.master(master_layer._master)
+                        result[current] = master.get_glyph_layer(current)
+                        if result[current] and result[current]._background_layer():
+                            result[current] = result[current]._background_layer()
+
+                if current not in result or not result[current]:
+                    raise ValueError("Could not find layer")
+            todo.extend([x.ref for x in result[current].components])
+        return result
+
     @cached_property
     def bounds(self):
         glyphset = {}
-        for c in list(self.recursiveComponentSet()):
+        for c in list(self.recursive_component_set()):
             glyphset[c] = self.master.get_glyph_layer(c)
         pen = BoundsPen(glyphset)
         self.draw(pen)
         return pen.bounds
 
     @property
     def lsb(self):
@@ -74,21 +129,21 @@
     def rsb(self):
         if not self.bounds:  # Space glyph
             return 0
         return self.width - self.bounds[2]
 
     @property
     def valid(self):
-        if not self._font:
+        if not self._font or not self._glyph:
             return False
         return True
 
     @property
     def anchors_dict(self):
-        return { a.name: a for a in self.anchors }
+        return {a.name: a for a in self.anchors}
 
     # Pen protocol support...
 
     def draw(self, pen):
         pen = PointToSegmentPen(pen)
         return self.drawPoints(pen)
 
@@ -107,27 +162,16 @@
 
     def clearContours(self):
         self.shapes = []
 
     def getPen(self):
         return SegmentToPointPen(LayerPen(self))
 
-    def _nestedComponentDict(self):
-        result = {}
-        todo = [x.ref for x in self.components]
-        while todo:
-            current = todo.pop()
-            if current in result:
-                continue
-            result[current] = self.master.get_glyph_layer(current)
-            todo.extend([x.ref for x in result[current].components])
-        return result
-
     def decompose(self):
-        pen = DecomposingRecordingPen(self._nestedComponentDict())
+        pen = DecomposingRecordingPen(self._nested_component_dict())
         self.draw(pen)
         self.clearContours()
         pen.replay(self.getPen())
 
 
 class LayerPen(AbstractPointPen):
     def __init__(self, target):
@@ -137,17 +181,19 @@
     def beginPath(self, identifier=None, **kwargs):
         self.curPath = []
 
     def endPath(self):
         """End the current sub path."""
         self.target.shapes.append(Shape(nodes=self.curPath))
 
-    def addPoint(self, pt, segmentType=None, smooth=False, name=None,
-                 identifier=None, **kwargs):
+    def addPoint(
+        self, pt, segmentType=None, smooth=False, name=None, identifier=None, **kwargs
+    ):
+        if segmentType == "move":
+            return
         ourtype = Node._from_pen_type[segmentType]
         if smooth:
             ourtype = ourtype + "s"
         self.curPath.append(Node(pt[0], pt[1], ourtype))
 
-    def addComponent(self, baseGlyphName, transformation, identifier=None,
-                     **kwargs):
+    def addComponent(self, baseGlyphName, transformation, identifier=None, **kwargs):
         self.target.shapes.append(Shape(ref=baseGlyphName, transform=transformation))
```

### Comparing `babelfont-3.0.1/src/babelfont/Names.py` & `babelfont-3.0.2/src/babelfont/Names.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .BaseObject import BaseObject, I18NDictionary
 from dataclasses import dataclass, asdict
 
 
 @dataclass
 class Names(BaseObject):
     """A table of global, localizable names for the font."""
+
     familyName: I18NDictionary = None
     designer: I18NDictionary = None
     designerURL: I18NDictionary = None
     manufacturer: I18NDictionary = None
     manufacturerURL: I18NDictionary = None
     license: I18NDictionary = None
     licenseURL: I18NDictionary = None
@@ -19,21 +20,29 @@
     typographicSubfamily: I18NDictionary = None
     compatibleFullName: I18NDictionary = None
     sampleText: I18NDictionary = None
     WWSFamilyName: I18NDictionary = None
     WWSSubfamilyName: I18NDictionary = None
     copyright: I18NDictionary = None
     styleMapFamilyName: I18NDictionary = None
+    styleMapStyleName: I18NDictionary = None
+    styleName: I18NDictionary = None
     trademark: I18NDictionary = None
+    preferredSubfamilyName: I18NDictionary = None
 
     def __post_init__(self):
         for k in self.__dataclass_fields__.keys():
             if not getattr(self, k):
                 setattr(self, k, I18NDictionary())
 
     def as_nametable_dict(self):
         rv = {}
-        for k,v in asdict(self).items():
+        ft_names = {
+            "manufacturerURL": "vendorURL",
+            "license": "licenseDescription",
+            "licenseURL": "licenseInfoURL",
+        }
+        for k, v in asdict(self).items():
             if not v:
                 continue
-            rv[k] = v.default_or_dict()
+            rv[ft_names.get(k, k)] = v.default_or_dict()
         return rv
```

### Comparing `babelfont-3.0.1/src/babelfont/Node.py` & `babelfont-3.0.2/src/babelfont/Node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from collections import namedtuple
+from dataclasses import dataclass
 
-_Node = namedtuple("Node", "x,y,type,userdata", defaults=[0, 0, "c", None])
 
+@dataclass
+class Node:
+    x: int = 0
+    y: int = 0
+    type: str = "c"
+    userdata: str = None
 
-class Node(_Node):
     _to_pen_type = {"o": None, "c": "curve", "l": "line", "q": "qcurve"}
     _from_pen_type = {v: k for k, v in _to_pen_type.items()}
 
     def write(self, stream, indent):
         if not self.userdata:
             stream.write(('[%i,%i,"%s"]' % (self.x, self.y, self.type)).encode())
         else:
```

### Comparing `babelfont-3.0.1/src/babelfont/Shape.py` & `babelfont-3.0.2/src/babelfont/Shape.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import math
 from dataclasses import dataclass
-from .BaseObject import BaseObject
+from typing import Optional
+
 from fontTools.misc.transform import Transform
+
+from .BaseObject import BaseObject
 from .Node import Node
-import math
 
 
 @dataclass
 class _ShapeFields:
     ref: str = None
     transform: Transform = None
     nodes: [Node] = None
     closed: bool = True
     direction: int = 1
 
     _layer = None
 
+
 @dataclass
 class Shape(BaseObject, _ShapeFields):
     @property
     def _write_one_line(self):
         return self.is_component
 
     @property
@@ -26,35 +30,34 @@
         return not bool(self.ref)
 
     @property
     def is_component(self):
         return bool(self.ref)
 
     @property
-    def component_layer(self):
+    def component_layer(self) -> Optional["Layer"]:
         if not self.is_component:
             return None
         return self._layer.master.get_glyph_layer(self.ref)
 
     @property
     def pos(self):
         assert self.is_component
         if not self.transform:
-            return (0,0)
+            return (0, 0)
         return tuple(self.transform[4:])
 
     @property
     def angle(self):
         assert self.is_component
         if not self.transform:
             return 0
         return math.atan2(self.transform[1], self.transform[0]) * 180 / math.pi
 
     @property
     def scale(self):
         assert self.is_component
         if not self.transform:
-            return (1,1)
-        print(self.transform)
+            return (1, 1)
         scaleX = math.sqrt(self.transform[0] ** 2 + self.transform[2] ** 2)
         scaleY = math.sqrt(self.transform[1] ** 2 + self.transform[3] ** 2)
         return (scaleX, scaleY)
```

### Comparing `babelfont-3.0.1/src/babelfont/convertors/__init__.py` & `babelfont-3.0.2/src/babelfont/convertors/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,83 @@
 import os
 import sys
 import pkgutil
 import inspect
 import importlib
-from babelfont import Font
+import logging
+
+from babelfont.Font import Font
+
 
 class BaseConvertor:
+    filename: str
+    scratch: object
+    font: Font
+    compile_only: bool
+
     suffix = ".XXX"
 
+    def __init__(self):
+        self.logger = logging.getLogger(self.__class__.__name__)
+
     @classmethod
-    def can_load(self, other, **kwargs):
-        return other.filename.endswith(self.suffix)
+    def can_load(cls, other, **kwargs):
+        return other.filename.endswith(cls.suffix)
 
     @classmethod
-    def can_save(self, other, **kwargs):
-        return other.filename.endswith(self.suffix)
+    def can_save(cls, other, **kwargs):
+        return other.filename.endswith(cls.suffix)
 
     @classmethod
-    def load(cls, convertor):
+    def load(cls, convertor, compile_only=False):
         self = cls()
         self.font = Font()
         # Pass on information to child
         self.filename = convertor.filename
         self.scratch = convertor.scratch
+        self.compile_only = compile_only
+
         return self._load()
 
     @classmethod
     def save(cls, obj, convertor, **kwargs):
         self = cls()
         self.font = obj
         # Pass on information to child
         self.filename = convertor.filename
         self.scratch = convertor.scratch
         return self._save()
 
+    def _load(self):
+        raise NotImplementedError
+
+    def _save(self):
+        raise NotImplementedError
+
+
 class Convert:
     convertors = []
 
     @classmethod
     def _load_convertors(cls):
         if cls.convertors:
             return
         convertorpath = os.path.join(
             os.path.dirname(sys.modules[cls.__module__].__file__)
         )
         # Additional plugin path here?
         loaders = pkgutil.iter_modules([convertorpath])
         for loader, module_name, is_pkg in loaders:
-            if is_pkg:
-                continue
             spec = loader.find_spec(module_name)
             _module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(_module)
             classes = [
                 x[1]
                 for x in inspect.getmembers(_module, inspect.isclass)
-                if issubclass(x[1], BaseConvertor)
+                if issubclass(x[1], BaseConvertor) and x[1] is not BaseConvertor
             ]
             cls.convertors.extend(classes)
 
     def __init__(self, filename):
         self._load_convertors()
         self.filename = filename
         self.scratch = {}
```

### Comparing `babelfont-3.0.1/src/babelfont/convertors/gsobject.py` & `babelfont-3.0.2/src/babelfont/convertors/gsobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from datetime import datetime
-from babelfont import *
-import openstep_plist
-from fontTools.misc.transform import Transform
 from fontFeatures.feaLib import FeaParser
 from babelfont.convertors import BaseConvertor
-import re
-import math
+from babelfont import (
+    Master,
+    Glyph,
+    Layer,
+    Guide,
+    Anchor,
+    Shape,
+    Node,
+    OTValue,
+    Axis,
+    Instance,
+)
 import uuid
-from collections import OrderedDict
 from glyphsLib.glyphdata import get_glyph
-from fontTools.misc.filenames import userNameToFileName
-import os
 
 
 opentype_custom_parameters = {
     "typoAscender": ("OS/2", "sTypoAscender"),
     "typoDescender": ("OS/2", "sTypoDescender"),
     "typoLineGap": ("OS/2", "sTypoLineGap"),
     "winAscent": ("OS/2", "usWinAscent"),
@@ -87,15 +90,15 @@
             axis.min, axis.max, axis.default = (
                 axis.map_backward(axis.min),
                 axis.map_backward(axis.max),
                 axis.map_backward(axis.default),
             )
 
     def _custom_parameter(self, thing, name):
-        for param in (thing.customParameters or []):
+        for param in thing.customParameters or []:
             if param.name == name:
                 return param.value
         return None
 
     def _default_master_id(self):
         # The default master in glyphs is either the first master or the
         # one selected by the Variable Font Origin custom parameter
@@ -116,15 +119,17 @@
         location = gmaster.axes
         metrics = self.gsfont.metrics()
         master = Master(name=gmaster.name, id=gmaster.id, font=self.font)
         metric_types = [m.name or m.typeName() for m in metrics]
         for k, v in zip(metric_types, gmaster.metrics()):
             master.metrics[_glyphs_metrics_to_ours(k)] = v.position
             if v.overshoot:
-                master.metrics["%s overshoot" % _glyphs_metrics_to_ours(k)] = v.overshoot
+                master.metrics[
+                    "%s overshoot" % _glyphs_metrics_to_ours(k)
+                ] = v.overshoot
 
         master.location = {k.tag: v for k, v in zip(self.font.axes, location)}
         master.guides = [self._load_guide(x) for x in gmaster.guides]
         kerntable = self.gsfont.kerning.get(master.id, {})
         master.kerning = self._load_kerning(kerntable)
         # XXX support RTL kerning etc.
 
@@ -136,15 +141,15 @@
         _maybesetformatspecific(master, gmaster, "userData")
         _maybesetformatspecific(master, gmaster, "visible")
         assert master.valid
         return master
 
     def _get_codepoint(self, gglyph):
         if gglyph.unicodes:
-            return [int(x,16) for x in gglyph.unicodes]
+            return [int(x, 16) for x in gglyph.unicodes]
         return []
 
     def _load_glyph(self, gglyph):
         name = gglyph.name
         c = gglyph.category
         sc = gglyph.subCategory
         if sc == "Ligature":
@@ -203,18 +208,18 @@
         if "Background" not in str(type(layer)) and layer.background:
             (background,) = self._load_layer(layer.background, width=l.width)
             # If it doesn't have an ID, we need to generate one
             background.id = str(uuid.uuid1())
             # XXX
             # For some INSANE REASON orjson is serializing this to `True` in json,
             # not `true`.
-            #background.isBackground = True
-            del(background._master)
+            # background.isBackground = True
+            del background._master
 
-            l._background = background.id
+            l.background = background.id
             returns.append(background)
         # TODO backgroundImage, metricTop/Bottom/etc, vertOrigin, vertWidth.
         for r in returns:
             assert r.valid
         return returns
 
     def _load_guide(self, gguide):
@@ -353,15 +358,15 @@
             ast = feaparser.parser.ast
             for name, members in self.font.features.namedClasses.items():
                 glyphclass = ast.GlyphClassDefinition(
                     name, ast.GlyphClass([m for m in members])
                 )
                 feaparser.parser.glyphclasses_.define(name, glyphclass)
             feaparser.parse()
-        except Exception as e:
+        except Exception:
             pass
 
     def _load_shape(self, shape):
         if hasattr(shape, "nodes"):  # It's a path
             return self._load_path(shape)
         else:
             return self._load_component(shape)
@@ -372,34 +377,30 @@
         shape.closed = path.closed
         return shape
 
     def _load_kern_groups(self, glyphs):
         kerngroups = {}
         for g in glyphs:
             if g.leftKerningGroup:
-                kerngroups.setdefault("MMK_L_" + g.leftKerningGroup, []).append(
-                    g.name
-                )
+                kerngroups.setdefault("MMK_L_" + g.leftKerningGroup, []).append(g.name)
             if g.rightKerningGroup:
-                kerngroups.setdefault("MMK_R_" + g.rightKerningGroup, []).append(
-                    g.name
-                )
+                kerngroups.setdefault("MMK_R_" + g.rightKerningGroup, []).append(g.name)
         for k, v in kerngroups.items():
             self.font.features.namedClasses[k] = tuple(v)
 
 
 def _maybesetformatspecific(item, glyphs, key):
     if hasattr(glyphs, key):
         if "com.glyphsapp" not in item._formatspecific:
             item._formatspecific["com.glyphsapp"] = {}
-        value = getattr(glyphs, key) # XXX
+        value = getattr(glyphs, key)  # XXX
         try:
             orjson.dumps(value)
             item._formatspecific["com.glyphsapp"][key] = value
-        except Exception as e:
+        except Exception:
             print("%s.%s cannot be serialized!" % (glyphs, key))
 
 
 def _moveformatspecific(item):
     rv = {}
     if "com.glyphsapp" in item._formatspecific:
         rv = {**item._formatspecific.get("com.glyphsapp", {})}
```

### Comparing `babelfont-3.0.1/src/babelfont/convertors/nfsf.py` & `babelfont-3.0.2/src/babelfont/convertors/nfsf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from datetime import datetime
-from babelfont import *
-from fontTools.misc.transform import Transform
+from babelfont import Glyph, Layer, Node, Shape, Master, Guide, Anchor, Axis, Instance
 from babelfont.convertors import BaseConvertor
 from pathlib import Path
-from lxml import etree
-from fontFeatures import FontFeatures
 import orjson
 import os
 
 
 # One would hope this would be easy.
 
 
@@ -77,32 +74,32 @@
     def _load_metadata(self, info):
         for k in ["note", "upm", "version", "date", "customOpenTypeValues"]:
             if k in info:
                 setattr(self.font, k, info[k])
         self.font.date = datetime.strptime(self.font.date, "%Y-%m-%d %H:%M:%S")
 
     def _load_features(self):
-        path = os.path.join(self.filename, "features.xml")
+        path = os.path.join(self.filename, "features.fea")
         if os.path.isfile(path):
             f = open(path, "r")
-            xml = etree.parse(f)
-            self.font.features = FontFeatures.fromXML(xml.getroot())
+            self.font.features = f.read()
 
     def _save(self):
         path = Path(self.filename)
         path.mkdir(parents=True, exist_ok=True)
 
         with open(path / "info.json", "wb") as f:
             self.font.write(stream=f)
 
         with open(path / "names.json", "wb") as f:
             self.font._write_value(f, "glyphs", self.font.names)
 
-        with open(path / "features.xml", "wb") as f:
-            f.write(etree.tostring(self.font.features.toXML(), pretty_print=True))
+        with open(path / "features.fea", "w") as f:
+            if self.font.features:
+                f.write(self.font.features.to_fea())
 
         with open(path / "glyphs.json", "wb") as f:
             for g in self.font.glyphs:
                 glyphpath = path / "glyphs"
                 glyphpath.mkdir(parents=True, exist_ok=True)
                 with open(path / g.babelfont_filename, "wb") as f2:
                     g._write_value(f2, "layers", g.layers)
```

### Comparing `babelfont-3.0.1/src/babelfont/convertors/truetype.py` & `babelfont-3.0.2/src/babelfont/convertors/truetype.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+import uuid
 from datetime import datetime
-from babelfont import *
+from itertools import chain
+
+from fontFeatures import Attachment
+from fontFeatures.ttLib import unparse
+from fontTools.cu2qu.ufo import glyphs_to_quadratic
 from fontTools.fontBuilder import FontBuilder
-from fontTools.pens.ttGlyphPen import TTGlyphPen
-from fontTools.pens.recordingPen import RecordingPen
-from cu2qu.ufo import glyphs_to_quadratic
+from fontTools.misc.fixedTools import otRound
 from fontTools.misc.timeTools import epoch_diff, timestampSinceEpoch
-from fontTools.ttLib.tables.TupleVariation import TupleVariation
-from babelfont.fontFilters.featureWriters import build_all_features
+from fontTools.pens.recordingPen import RecordingPen
+from fontTools.pens.ttGlyphPen import TTGlyphPen
 from fontTools.ttLib import TTFont
 from fontTools.ttLib.tables._g_l_y_f import GlyphCoordinates
+from fontTools.ttLib.tables.TupleVariation import TupleVariation
 from fontTools.varLib.iup import iup_delta_optimize
-from fontTools.misc.fixedTools import otRound
-from fontFeatures.ttLib import unparse
-from fontFeatures import Attachment
-import uuid
-from itertools import chain
+
+from babelfont.convertors import BaseConvertor
+from babelfont.fontFilters.featureWriters import build_all_features
+from babelfont import Master, Glyph, Layer, Anchor, Shape, Node, Axis, Instance
 
 
-def _categorize_glyph(font,glyphname):
-    if "GDEF" not in font: return None
+def _categorize_glyph(font, glyphname):
+    if "GDEF" not in font:
+        return None
     if not font["GDEF"].table.GlyphClassDef:
         return None
     classdefs = font["GDEF"].table.GlyphClassDef.classDefs
     if glyphname not in classdefs:
         return None
-    if classdefs[glyphname] == 1: return "base"
-    if classdefs[glyphname] == 2: return "ligature"
-    if classdefs[glyphname] == 3: return "mark"
-    if classdefs[glyphname] == 4: return "component"
+    if classdefs[glyphname] == 1:
+        return "base"
+    if classdefs[glyphname] == 2:
+        return "ligature"
+    if classdefs[glyphname] == 3:
+        return "mark"
+    if classdefs[glyphname] == 4:
+        return "component"
+
 
 class TrueType(BaseConvertor):
     suffix = ".ttf"
 
     def _decompose_mixed_layer(self, layer, exportable):
         if (layer.paths and layer.components) or any(
             c.ref not in exportable for c in layer.components
@@ -73,28 +82,39 @@
                     Instance(
                         name=self.tt["name"].getDebugName(instance.subfamilyNameID),
                         location=instance.coordinates,
                     )
                 )
 
     def _load_masters(self):
-        m = Master(location={},name="Default", id=str(uuid.uuid1()) )
+        m = Master(location={}, name="Default", id=str(uuid.uuid1()))
         # Metrics
         m.metrics = {
-            "xHeight": self.tt["OS/2"].sxHeight if hasattr(self.tt["OS/2"], "sxHeight") else None,
-            "capHeight": self.tt["OS/2"].sCapHeight  if hasattr(self.tt["OS/2"], "capHeight") else None,
+            "xHeight": (
+                self.tt["OS/2"].sxHeight
+                if hasattr(self.tt["OS/2"], "sxHeight")
+                else None
+            ),
+            "capHeight": (
+                self.tt["OS/2"].sCapHeight
+                if hasattr(self.tt["OS/2"], "capHeight")
+                else None
+            ),
             "ascender": self.tt["hhea"].ascender,
-            "descender": self.tt["hhea"].descender
+            "descender": self.tt["hhea"].descender,
         }
         m.font = self.font
         self.font.masters = [m]
         if "fvar" in self.tt:
             m.location = {axis.tag: axis.default for axis in self.font.axes}
-            all_masters = [frozenset(x.axes.items()) for x in chain(*self.tt["gvar"].variations.values())]
-            all_masters = [{k:v[1] for k,v in dict(m1).items()} for m1 in all_masters]
+            all_masters = [
+                frozenset(x.axes.items())
+                for x in chain(*self.tt["gvar"].variations.values())
+            ]
+            all_masters = [{k: v[1] for k, v in dict(m1).items()} for m1 in all_masters]
             # Now denormalize.
             # XXX
             pass
 
     def _load_head(self):
         head = self.tt["head"]
         self.font.upm = head.unitsPerEm
@@ -109,30 +129,32 @@
         # XXX
 
     def _load_glyphs(self):
         mapping = self.tt["cmap"].buildReversed()
         glyphs_dict = {}
         for glyph in self.tt.getGlyphOrder():
             category = _categorize_glyph(self.tt, glyph) or "base"
-            glyphs_dict[glyph] = Glyph(name=glyph, codepoints=list(mapping.get(glyph, [])), category=category)
+            glyphs_dict[glyph] = Glyph(
+                name=glyph, codepoints=list(mapping.get(glyph, [])), category=category
+            )
             self.font.glyphs.append(glyphs_dict[glyph])
-            glyphs_dict[glyph].layers = self._load_layers(glyph)
+            glyphs_dict[glyph].layers = self._load_layers(glyph, glyphs_dict[glyph])
         return glyphs_dict
 
-    def _load_layers(self, g):
-        ttglyph = self.tt.getGlyphSet()[g]  # _TTGlyphGlyf object
-        width = self.tt["hmtx"][g][0]
+    def _load_layers(self, glyphname, glyph):
+        ttglyph = self.tt.getGlyphSet()[glyphname]  # _TTGlyphGlyf object
+        width = self.tt["hmtx"][glyphname][0]
         # leftMargin = self.tt["hmtx"][g][1]
-        layer = Layer(width=width, id=str(uuid.uuid1()) )
+        layer = Layer(width=width, id=str(uuid.uuid1()))
         layer._master = self.font.masters[0].id
         layer._font = self.font
+        layer._glyph = glyph
         ttglyph.draw(layer.getPen())
         return [layer]
 
-
     def _load_contour(self, ttglyph, index):
         shape = Shape()
         shape.nodes = []
         endPt = ttglyph.endPtsOfContours[index]
         if index > 0:
             startPt = ttglyph.endPtsOfContours[index - 1] + 1
         else:
@@ -150,20 +172,20 @@
                 else:
                     t = "q"
             else:
                 if len(points) > 1 and points[-1].type == "o":
                     # Double offcurve. Insert implicit oncurve.
                     prevpoint = points[-1]
                     intermediate = Node(
-                        x = (coords[0] + prevpoint.x) / 2,
-                        y = (coords[1] + prevpoint.y) / 2,
-                        type = "q"
+                        x=(coords[0] + prevpoint.x) / 2,
+                        y=(coords[1] + prevpoint.y) / 2,
+                        type="q",
                     )
                     points.append(intermediate)
-            p = Node(x = coords[0], y=coords[1], type=t)
+            p = Node(x=coords[0], y=coords[1], type=t)
             points.append(p)
         shape.nodes = points
         return shape
 
     def _load_component(self, c):
         baseGlyph, transformation = c.getComponentInfo()
         component = Shape(ref=baseGlyph, transform=transformation)
@@ -214,15 +236,15 @@
                 for ix, m in enumerate(f.masters):
                     layer = m.get_glyph_layer(g)
                     pen = TTGlyphPen(m.ttglyphset)
                     layer.draw(pen)
 
                     m.ttglyphset[g] = pen.glyph()
 
-            except Exception as e:
+            except Exception:
                 print(
                     "Problem converting glyph %s to quadratic. (Probably incompatible) "
                     % g
                 )
                 for m in f.masters:
                     m.ttglyphset[g] = TTGlyphPen(m.ttglyphset).glyph()
             done[g] = True
@@ -267,22 +289,24 @@
                     k: axis_map[k].map_backward(v) for k, v in instance.location.items()
                 }
             fb.setupFvar(f.axes, f.instances)
 
             fb.setupGvar(variations)
             fb.setupAvar(f.axes)
         # Move glyph categories to fontfeatures
-        for g in f.glyphs.values():
-            if g.exported:
-                f.features.glyphclasses[g.name] = g.category
+        # if f.features:
+        #     for g in f.glyphs.values():
+        #         if g.exported:
+        #             f.features.classes[g.name] = g.category
 
-        build_all_features(f, fb.font)
+        #     build_all_features(f, fb.font)
         fb.setupPost()
 
-        for table, field, value in f.customOpenTypeValues:
+        for otvalue in f.customOpenTypeValues:
+            table, field, value = otvalue.table, otvalue.field, otvalue.value
             setattr(fb.font[table], field, value)
 
         fb.font.save(self.filename)
 
         # Rename to production
         rename_map = {g.name: g.production_name or g.name for g in f.glyphs}
         if rename_map:
@@ -291,33 +315,35 @@
             if "post" in font and font["post"].formatType == 2.0:
                 font["post"].extraNames = []
                 font["post"].compile(font)
             font.save(self.filename)
 
     def calculate_a_gvar(self, f, model, g, default_width):
         master_layer = f.default_master.get_glyph_layer(g)
-        if not g in f.default_master.ttglyphset:
+        if g not in f.default_master.ttglyphset:
             return None
         default_g = f.default_master.ttglyphset[g]
         all_coords = []
         for m in f.masters:
             layer = m.get_glyph_layer(g)
             basecoords = GlyphCoordinates(m.ttglyphset[g].coordinates)
             if m.ttglyphset[g].isComposite():
                 component_point = GlyphCoordinates(
                     [
                         (otRound(layer_comp.pos[0]), otRound(layer_comp.pos[1]))
                         for layer_comp in layer.components
                     ]
                 )
                 basecoords.extend(component_point)
-            phantomcoords = GlyphCoordinates([(0, 0), (otRound(layer.width), 0), (0, 0), (0, 0)])
+            phantomcoords = GlyphCoordinates(
+                [(0, 0), (otRound(layer.width), 0), (0, 0), (0, 0)]
+            )
             basecoords.extend(phantomcoords)
             all_coords.append(basecoords)
-        for ix,c in enumerate(all_coords):
+        for ix, c in enumerate(all_coords):
             all_ok = True
             if len(c) != len(all_coords[0]):
                 print("Incompatible master %i in glyph %s" % (ix, g))
                 all_ok = False
             if not all_ok:
                 return []
         deltas = model.getDeltas(all_coords)
@@ -328,15 +354,17 @@
             endPts = default_g.endPtsOfContours
 
         for delta, sup in zip(deltas, model.supports):
             if not sup:
                 continue
             var = TupleVariation(sup, round(delta))
             # This assumes we do the default master first, which may not be true
-            delta_opt = iup_delta_optimize(round(delta), round(deltas[0]), endPts, tolerance=0.5)
+            delta_opt = iup_delta_optimize(
+                round(delta), round(deltas[0]), endPts, tolerance=0.5
+            )
             if None in delta_opt:
                 var = TupleVariation(sup, delta_opt)
             gvar_entry.append(var)
         return gvar_entry
 
     def _load_features(self):
         self.font.features = unparse(self.tt)
@@ -376,46 +404,47 @@
     #     y_deltas = np.apply_along_axis(model.getDeltas, 1, base_deltas[:,:,1].transpose())
     #     alldeltas = np.array([x_deltas, y_deltas]).transpose()
     #     gvar_entry = []
     #     for deltaset, sup in zip(alldeltas, model.supports):
     #         gvar_entry.append(TupleVariation(sup, list(map(tuple, deltaset))))
     #     return gvar_entry
 
+
 class OpenType(TrueType):
     suffix = ".otf"
 
     def _load_layers(self, g):
         ttglyph = self.tt.getGlyphSet()[g]
         width = self.tt["hmtx"][g][0]
-        layer = Layer(width=width, id=str(uuid.uuid1()) )
+        layer = Layer(width=width, id=str(uuid.uuid1()))
         layer._master = self.font.masters[0].id
         layer._font = self.font
         pen = RecordingPen()
         ttglyph.draw(pen)
         contours = pen.value
         lastcontour = []
-        startPt = (0,0)
-        lastPt = (0,0)
+        startPt = (0, 0)
+        lastPt = (0, 0)
         index = 0
         for operation, segment in contours:
             if operation == "moveTo":
                 startPt = segment[0]
             elif operation == "closePath":
                 if startPt != lastPt:
-                    lastcontour.append(Node(x=startPt[0], y=startPt[1],type = "l"))
+                    lastcontour.append(Node(x=startPt[0], y=startPt[1], type="l"))
                 contour = Shape()
                 contour.nodes = lastcontour
                 layer.shapes.append(contour)
                 lastcontour = []
             elif operation == "curveTo":
-                lastcontour.append(Node(x=segment[0][0],y=segment[0][1],type = "o"))
-                lastcontour.append(Node(x=segment[1][0],y=segment[1][1],type = "o"))
-                lastcontour.append(Node(x=segment[2][0],y=segment[2][1],type = "c"))
+                lastcontour.append(Node(x=segment[0][0], y=segment[0][1], type="o"))
+                lastcontour.append(Node(x=segment[1][0], y=segment[1][1], type="o"))
+                lastcontour.append(Node(x=segment[2][0], y=segment[2][1], type="c"))
                 lastPt = segment[2]
             elif operation == "lineTo":
-                lastcontour.append(Node(x=segment[0][0],y=segment[0][1],type = "l"))
+                lastcontour.append(Node(x=segment[0][0], y=segment[0][1], type="l"))
                 lastPt = segment[0]
             elif operation == "qCurveTo":
-                lastcontour.append(Node(x=segment[0][0],y=segment[0][1],type = "o"))
-                lastcontour.append(Node(x=segment[1][0],y=segment[1][1],type = "q"))
+                lastcontour.append(Node(x=segment[0][0], y=segment[0][1], type="o"))
+                lastcontour.append(Node(x=segment[1][0], y=segment[1][1], type="q"))
 
         return [layer]
```

### Comparing `babelfont-3.0.1/src/babelfont/fontFilters/featureWriters.py` & `babelfont-3.0.2/src/babelfont/fontFilters/featureWriters.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,35 +20,39 @@
             return [c]
         if c[1:] not in font.features.namedClasses:
             logging.info("Attempted to use undefined kerning class %s" % c)
             return None
         return [x for x in font.features.namedClasses[c[1:]] if font.glyphs[x].exported]
 
     kernroutine = Routine()
-    for (l,r), kern in font._all_kerning.items():
-        l, r = _expand_class(l), _expand_class(r)
-        if l is None or r is None:
+    for (left, right), kern in font._all_kerning.items():
+        left, right = _expand_class(left), _expand_class(right)
+        if left is None or right is None:
             continue
-        kernroutine.rules.append(Positioning(
-            [ l, r ],
-            [ ValueRecord(xAdvance=kern), ValueRecord() ],
-        ))
+        kernroutine.rules.append(
+            Positioning(
+                [left, right],
+                [ValueRecord(xAdvance=kern), ValueRecord()],
+            )
+        )
     font.features.addFeature("kern", [kernroutine])
 
 
 def build_cursive(font):
     anchors = font._all_anchors
     if "entry" in anchors and "exit" in anchors:
         attach = Attachment(
-            "entry", "exit", anchors["entry"], anchors["exit"],
-            flags=(0x8 | 0x1)
+            "entry", "exit", anchors["entry"], anchors["exit"], flags=(0x8 | 0x1)
+        )
+        r = Routine(
+            rules=[attach],
         )
-        r = Routine(rules=[attach], )
         font.features.addFeature("curs", [r])
 
+
 def build_mark_mkmk(font, which="mark", strict=False):
     # Find matching pairs of foo/_foo anchors
     anchors = font._all_anchors
     r = Routine(rules=[])
     if which == "mark":
         basecategory = "base"
     else:
@@ -62,15 +66,16 @@
             k: v
             for k, v in anchors[baseanchor].items()
             if font.glyphs[k].exported and (font.glyphs[k].category == basecategory)
         }
         marks = {
             k: v
             for k, v in anchors[markanchor].items()
-            if font.glyphs[k].exported and (not strict or font.glyphs[k].category == "mark")
+            if font.glyphs[k].exported
+            and (not strict or font.glyphs[k].category == "mark")
         }
         if not (bases and marks):
             continue
         attach = Attachment(baseanchor, markanchor, bases, marks)
         attach.fontfeatures = font.features  # THIS IS A TERRIBLE HACK
         r.rules.append(attach)
     if r.rules:
```

### Comparing `babelfont-3.0.1/PKG-INFO` & `babelfont-3.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: babelfont
-Version: 3.0.1
+Version: 3.0.2
 Summary: Load, examine and save fonts in a variety of formats
-Author: Simon Cozens
-Author-email: simon@simon-cozens.org
-Requires-Python: >=3.8
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: cu2qu (>=1.6.7,<2.0.0)
-Requires-Dist: fontfeatures (>=1.0.6,<2.0.0)
-Requires-Dist: fonttools (>=4.21.1)
-Requires-Dist: glyphsLib (>=5.3.2)
-Requires-Dist: openstep-plist (>=0.2.2)
-Requires-Dist: orjson (>=3.5.1,<4.0.0)
-Requires-Dist: ufoLib2 (>=0.11.1)
+Author-email: Simon Cozens <simon@simon-cozens.org>
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.txt
+Requires-Dist: python>=3.8
+Requires-Dist: orjson~=3.5.1
+Requires-Dist: fonttools>=4.40.0
+Requires-Dist: ufoLib2>=0.11.1
+Requires-Dist: openstep-plist>=0.2.2
+Requires-Dist: glyphsLib>=5.3.2
+Requires-Dist: fontfeatures~=1.0.6
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: defcon; extra == "dev"
 
 # Babelfont: Load, examine and save fonts in a variety of formats
 
 *This describes Babelfont >3.0, which is a complete rewrite from the previous version.*
 
 Babelfont is a utility for loading fonts and examining fonts in a variety
 of formats. It can also be used to *write* fonts in some of these formats,
@@ -53,8 +52,7 @@
 font = load("Myfont.glyphs") # Or .designspace, or whatever
 default_a = font.default_master.get_glyph_layer("A")
 top_anchor = default_a.anchors_dict["top"].x
 print("Top anchor = (%i,%i)" % (top_anchor.x, top_anchor.y))
 print("LSB, RSB = (%i,%i)" % (default_a.lsb, default_a.rsb))
 font.save("Myfont.ttf")
 ```
-
```

