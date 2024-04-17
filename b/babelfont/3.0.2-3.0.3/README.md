# Comparing `tmp/babelfont-3.0.2.tar.gz` & `tmp/babelfont-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelfont-3.0.2.tar", last modified: Wed Apr 17 09:51:00 2024, max compression
+gzip compressed data, was "babelfont-3.0.3.tar", last modified: Wed Apr 17 09:55:09 2024, max compression
```

## Comparing `babelfont-3.0.2.tar` & `babelfont-3.0.3.tar`

### file list

```diff
@@ -1,291 +1,291 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 09:50:53.000000 babelfont-3.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.454701 babelfont-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:50:53.000000 babelfont-3.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:50:53.000000 babelfont-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 09:50:53.000000 babelfont-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 09:50:53.000000 babelfont-3.0.2/AUTHORS.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.454701 babelfont-3.0.2/Babelfont.glyphsFileFormat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/MacOS/
--rwxr-xr-x   0 runner    (1001) docker     (127)   120208 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/MacOS/plugin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-17 09:50:53.000000 babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:50:53.000000 babelfont-3.0.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 09:50:53.000000 babelfont-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-17 09:50:53.000000 babelfont-3.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-17 09:51:00.502701 babelfont-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 09:50:53.000000 babelfont-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Anchor.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Axis.md
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Font.md
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Gemfile
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Gemfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Glyph.md
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Instance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Master.md
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Names.md
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/Shape.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.462701 babelfont-3.0.2/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/_data/navigation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    36234 2024-04-17 09:50:53.000000 babelfont-3.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-17 09:50:53.000000 babelfont-3.0.2/makedoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56244 2024-04-17 09:50:53.000000 babelfont-3.0.2/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 09:50:53.000000 babelfont-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:51:00.502701 babelfont-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.458701 babelfont-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.466701 babelfont-3.0.2/src/babelfont/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/BaseObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Font.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Guide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Master.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Names.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/Shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.466701 babelfont-3.0.2/src/babelfont/convertors/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/designspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontforge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/convertors/fontlab/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/fontlab/vfj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/convertors/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26782 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs3.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphspackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/glyphs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/nfsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/truetype.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/convertors/ufo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/src/babelfont/fontFilters/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/anchorPropagation.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/featureWriters.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:50:53.000000 babelfont-3.0.2/src/babelfont/fontFilters/marks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/src/babelfont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 09:51:00.000000 babelfont-3.0.2/src/babelfont.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 09:50:53.000000 babelfont-3.0.2/t.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.470701 babelfont-3.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.474701 babelfont-3.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1118555 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Castoro Roman.vfj
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Glyphs2ManyAxes.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/GlyphsFileFormatv3.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/GlyphsFileFormatv3.vfj
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/LICENSE_MutatorSans
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/LICENSE_UbuTestData.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/NewFont-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Nunito-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (127)   157208 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Nunito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53914 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/SimpleTwoAxis.vfj
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/SimpleTwoAxis3.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.474701 babelfont-3.0.2/tests/data/Test1.roundtrip.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.roundtrip.ufo/features.fea
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/Test1.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/i.glif
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/glyphs/idotless.glif
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Test1.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)   432392 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/Ysabeau[wght].ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/glyphsLib/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestBasic.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFileName.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInactive.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.478701 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.482701 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/order.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/TestReencode.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.482701 babelfont-3.0.2/tests/data/glyphsLib/master_ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:00.502701 babelfont-3.0.2/tests/data/testotfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c2c3fc37b2d4c3cb2ef726c6cdaaabd4b7f3eb9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   125256 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    21160 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    22980 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/HBTest-VF.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/MORXTwentyeight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/TRAK.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   106096 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs2.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_glyphs3_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_otf_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_ufo_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 09:50:53.000000 babelfont-3.0.2/tests/test_vfj_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.081208 babelfont-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 09:54:59.000000 babelfont-3.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.029207 babelfont-3.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.033207 babelfont-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:54:59.000000 babelfont-3.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:54:59.000000 babelfont-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 09:54:59.000000 babelfont-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 09:54:59.000000 babelfont-3.0.3/AUTHORS.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.029207 babelfont-3.0.3/Babelfont.glyphsFileFormat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.033207 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 09:54:59.000000 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.033207 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/MacOS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120208 2024-04-17 09:54:59.000000 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/MacOS/plugin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.033207 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 09:54:59.000000 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-17 09:54:59.000000 babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:54:59.000000 babelfont-3.0.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 09:54:59.000000 babelfont-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-17 09:54:59.000000 babelfont-3.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-17 09:55:09.081208 babelfont-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 09:54:59.000000 babelfont-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.037207 babelfont-3.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Anchor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Axis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Font.md
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Gemfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Glyph.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Instance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Master.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Names.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/Shape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.037207 babelfont-3.0.3/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/_data/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    36234 2024-04-17 09:54:59.000000 babelfont-3.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-17 09:54:59.000000 babelfont-3.0.3/makedoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56244 2024-04-17 09:54:59.000000 babelfont-3.0.3/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 09:54:59.000000 babelfont-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:55:09.081208 babelfont-3.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.029207 babelfont-3.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.037207 babelfont-3.0.3/src/babelfont/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/BaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.041207 babelfont-3.0.3/src/babelfont/convertors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/fontforge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.041207 babelfont-3.0.3/src/babelfont/convertors/fontlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/fontlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/fontlab/vfj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.041207 babelfont-3.0.3/src/babelfont/convertors/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/glyphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26782 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphspackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/glyphs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/nfsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/convertors/ufo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.041207 babelfont-3.0.3/src/babelfont/fontFilters/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/fontFilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/fontFilters/anchorPropagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/fontFilters/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/fontFilters/featureWriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:54:59.000000 babelfont-3.0.3/src/babelfont/fontFilters/marks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.081208 babelfont-3.0.3/src/babelfont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-17 09:55:08.000000 babelfont-3.0.3/src/babelfont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-17 09:55:09.000000 babelfont-3.0.3/src/babelfont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:55:08.000000 babelfont-3.0.3/src/babelfont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 09:55:08.000000 babelfont-3.0.3/src/babelfont.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 09:55:08.000000 babelfont-3.0.3/src/babelfont.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 09:55:08.000000 babelfont-3.0.3/src/babelfont.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 09:54:59.000000 babelfont-3.0.3/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.045207 babelfont-3.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.049208 babelfont-3.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1118555 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Castoro Roman.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Glyphs2ManyAxes.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/GlyphsFileFormatv3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/GlyphsFileFormatv3.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/LICENSE_MutatorSans
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/LICENSE_UbuTestData.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/NewFont-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Nunito-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   157208 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53914 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/SimpleTwoAxis.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/SimpleTwoAxis3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.049208 babelfont-3.0.3/tests/data/Test1.roundtrip.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.roundtrip.ufo/features.fea
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.049208 babelfont-3.0.3/tests/data/Test1.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.049208 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/i.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/glyphs/idotless.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Test1.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)   432392 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/Ysabeau[wght].ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.053207 babelfont-3.0.3/tests/data/glyphsLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestBasic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestFileName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestInactive.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.053207 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.053207 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/order.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/TestReencode.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.053207 babelfont-3.0.3/tests/data/glyphsLib/master_ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:55:09.081208 babelfont-3.0.3/tests/data/testotfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1c2c3fc37b2d4c3cb2ef726c6cdaaabd4b7f3eb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125256 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    21160 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    22980 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/HBTest-VF.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/MORXTwentyeight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/TRAK.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106096 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_glyphs3_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_otf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_ufo_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 09:54:59.000000 babelfont-3.0.3/tests/test_vfj_loader.py
```

### Comparing `babelfont-3.0.2/.github/workflows/ci.yml` & `babelfont-3.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/.gitignore` & `babelfont-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Info.plist` & `babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/MacOS/plugin` & `babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/MacOS/plugin`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf` & `babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py` & `babelfont-3.0.3/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/LICENSE` & `babelfont-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/Makefile` & `babelfont-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/PKG-INFO` & `babelfont-3.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: babelfont
-Version: 3.0.2
+Version: 3.0.3
 Summary: Load, examine and save fonts in a variety of formats
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: python>=3.8
 Requires-Dist: orjson~=3.5.1
 Requires-Dist: fonttools>=4.40.0
 Requires-Dist: ufoLib2>=0.11.1
 Requires-Dist: openstep-plist>=0.2.2
 Requires-Dist: glyphsLib>=5.3.2
 Requires-Dist: fontfeatures~=1.0.6
 Provides-Extra: dev
```

### Comparing `babelfont-3.0.2/README.md` & `babelfont-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Anchor.md` & `babelfont-3.0.3/docs/Anchor.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Axis.md` & `babelfont-3.0.3/docs/Axis.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Font.md` & `babelfont-3.0.3/docs/Font.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Gemfile.lock` & `babelfont-3.0.3/docs/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Glyph.md` & `babelfont-3.0.3/docs/Glyph.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Guide.md` & `babelfont-3.0.3/docs/Guide.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Instance.md` & `babelfont-3.0.3/docs/Instance.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Layer.md` & `babelfont-3.0.3/docs/Layer.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Master.md` & `babelfont-3.0.3/docs/Master.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Names.md` & `babelfont-3.0.3/docs/Names.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/Shape.md` & `babelfont-3.0.3/docs/Shape.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/docs/index.md` & `babelfont-3.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/makedoc.py` & `babelfont-3.0.3/makedoc.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/poetry.lock` & `babelfont-3.0.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/pyproject.toml` & `babelfont-3.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 description = "Load, examine and save fonts in a variety of formats"
 authors = [
     { name = "Simon Cozens", email= "simon@simon-cozens.org" }
 ]
 readme = "README.md"
 
 dependencies = [
-    "python >=3.8",
     "orjson ~= 3.5.1",
     "fonttools >=4.40.0",
     "ufoLib2 >=0.11.1",
     "openstep-plist >=0.2.2",
     "glyphsLib >=5.3.2",
     "fontfeatures ~= 1.0.6",
 ]
```

### Comparing `babelfont-3.0.2/src/babelfont/Axis.py` & `babelfont-3.0.3/src/babelfont/Axis.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/BaseObject.py` & `babelfont-3.0.3/src/babelfont/BaseObject.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Features.py` & `babelfont-3.0.3/src/babelfont/Features.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Font.py` & `babelfont-3.0.3/src/babelfont/Font.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Glyph.py` & `babelfont-3.0.3/src/babelfont/Glyph.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Instance.py` & `babelfont-3.0.3/src/babelfont/Instance.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Layer.py` & `babelfont-3.0.3/src/babelfont/Layer.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Master.py` & `babelfont-3.0.3/src/babelfont/Master.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Names.py` & `babelfont-3.0.3/src/babelfont/Names.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Node.py` & `babelfont-3.0.3/src/babelfont/Node.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/Shape.py` & `babelfont-3.0.3/src/babelfont/Shape.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/__init__.py` & `babelfont-3.0.3/src/babelfont/__init__.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/__main__.py` & `babelfont-3.0.3/src/babelfont/__main__.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/__init__.py` & `babelfont-3.0.3/src/babelfont/convertors/__init__.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/designspace.py` & `babelfont-3.0.3/src/babelfont/convertors/designspace.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/fontforge.py` & `babelfont-3.0.3/src/babelfont/convertors/fontforge.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/fontlab/vfj.py` & `babelfont-3.0.3/src/babelfont/convertors/fontlab/vfj.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs2.py` & `babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphs2.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphs3.py` & `babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphs3.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/glyphs/glyphspackage.py` & `babelfont-3.0.3/src/babelfont/convertors/glyphs/glyphspackage.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/glyphs/utils.py` & `babelfont-3.0.3/src/babelfont/convertors/glyphs/utils.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/gsobject.py` & `babelfont-3.0.3/src/babelfont/convertors/gsobject.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/nfsf.py` & `babelfont-3.0.3/src/babelfont/convertors/nfsf.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/truetype.py` & `babelfont-3.0.3/src/babelfont/convertors/truetype.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/convertors/ufo.py` & `babelfont-3.0.3/src/babelfont/convertors/ufo.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/fontFilters/anchorPropagation.py` & `babelfont-3.0.3/src/babelfont/fontFilters/anchorPropagation.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont/fontFilters/featureWriters.py` & `babelfont-3.0.3/src/babelfont/fontFilters/featureWriters.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/src/babelfont.egg-info/PKG-INFO` & `babelfont-3.0.3/src/babelfont.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: babelfont
-Version: 3.0.2
+Version: 3.0.3
 Summary: Load, examine and save fonts in a variety of formats
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: python>=3.8
 Requires-Dist: orjson~=3.5.1
 Requires-Dist: fonttools>=4.40.0
 Requires-Dist: ufoLib2>=0.11.1
 Requires-Dist: openstep-plist>=0.2.2
 Requires-Dist: glyphsLib>=5.3.2
 Requires-Dist: fontfeatures~=1.0.6
 Provides-Extra: dev
```

### Comparing `babelfont-3.0.2/src/babelfont.egg-info/SOURCES.txt` & `babelfont-3.0.3/src/babelfont.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Castoro Roman.vfj` & `babelfont-3.0.3/tests/data/Castoro Roman.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Glyphs2ManyAxes.glyphs` & `babelfont-3.0.3/tests/data/Glyphs2ManyAxes.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/GlyphsFileFormatv3.glyphs` & `babelfont-3.0.3/tests/data/GlyphsFileFormatv3.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/GlyphsFileFormatv3.vfj` & `babelfont-3.0.3/tests/data/GlyphsFileFormatv3.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/LICENSE_MutatorSans` & `babelfont-3.0.3/tests/data/LICENSE_MutatorSans`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/LICENSE_UbuTestData.txt` & `babelfont-3.0.3/tests/data/LICENSE_UbuTestData.txt`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/NewFont-Regular.ttf` & `babelfont-3.0.3/tests/data/NewFont-Regular.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Nunito-Regular.otf` & `babelfont-3.0.3/tests/data/Nunito-Regular.otf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Nunito-Regular.ttf` & `babelfont-3.0.3/tests/data/Nunito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/SimpleTwoAxis.vfj` & `babelfont-3.0.3/tests/data/SimpleTwoAxis.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/SimpleTwoAxis3.glyphs` & `babelfont-3.0.3/tests/data/SimpleTwoAxis3.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.glyphs` & `babelfont-3.0.3/tests/data/Test1.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.ufo/fontinfo.plist` & `babelfont-3.0.3/tests/data/Test1.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.ufo/glyphs/A_.glif` & `babelfont-3.0.3/tests/data/Test1.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.ufo/glyphs/B_.glif` & `babelfont-3.0.3/tests/data/Test1.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif` & `babelfont-3.0.3/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Test1.ufo/lib.plist` & `babelfont-3.0.3/tests/data/Test1.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/Ysabeau[wght].ttf` & `babelfont-3.0.3/tests/data/Ysabeau[wght].ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestBasic.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestBasic.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestFileName.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestFileName.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInactive.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestInactive.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph` & `babelfont-3.0.3/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/TestReencode.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/TestReencode.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace` & `babelfont-3.0.3/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf` & `babelfont-3.0.3/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf` & `babelfont-3.0.3/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf` & `babelfont-3.0.3/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf` & `babelfont-3.0.3/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf` & `babelfont-3.0.3/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf` & `babelfont-3.0.3/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf` & `babelfont-3.0.3/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf` & `babelfont-3.0.3/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf` & `babelfont-3.0.3/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf` & `babelfont-3.0.3/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf` & `babelfont-3.0.3/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf` & `babelfont-3.0.3/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf` & `babelfont-3.0.3/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf` & `babelfont-3.0.3/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf` & `babelfont-3.0.3/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf` & `babelfont-3.0.3/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf` & `babelfont-3.0.3/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf` & `babelfont-3.0.3/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf` & `babelfont-3.0.3/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf` & `babelfont-3.0.3/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf` & `babelfont-3.0.3/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf` & `babelfont-3.0.3/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf` & `babelfont-3.0.3/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf` & `babelfont-3.0.3/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf` & `babelfont-3.0.3/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf` & `babelfont-3.0.3/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf` & `babelfont-3.0.3/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf` & `babelfont-3.0.3/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf` & `babelfont-3.0.3/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf` & `babelfont-3.0.3/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf` & `babelfont-3.0.3/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf` & `babelfont-3.0.3/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf` & `babelfont-3.0.3/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf` & `babelfont-3.0.3/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf` & `babelfont-3.0.3/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf` & `babelfont-3.0.3/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf` & `babelfont-3.0.3/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf` & `babelfont-3.0.3/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf` & `babelfont-3.0.3/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf` & `babelfont-3.0.3/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf` & `babelfont-3.0.3/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf` & `babelfont-3.0.3/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf` & `babelfont-3.0.3/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf` & `babelfont-3.0.3/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf` & `babelfont-3.0.3/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf` & `babelfont-3.0.3/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf` & `babelfont-3.0.3/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf` & `babelfont-3.0.3/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf` & `babelfont-3.0.3/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf` & `babelfont-3.0.3/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf` & `babelfont-3.0.3/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf` & `babelfont-3.0.3/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf` & `babelfont-3.0.3/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf` & `babelfont-3.0.3/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf` & `babelfont-3.0.3/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf` & `babelfont-3.0.3/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf` & `babelfont-3.0.3/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf` & `babelfont-3.0.3/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf` & `babelfont-3.0.3/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf` & `babelfont-3.0.3/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf` & `babelfont-3.0.3/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf` & `babelfont-3.0.3/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf` & `babelfont-3.0.3/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf` & `babelfont-3.0.3/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf` & `babelfont-3.0.3/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf` & `babelfont-3.0.3/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf` & `babelfont-3.0.3/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf` & `babelfont-3.0.3/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf` & `babelfont-3.0.3/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf` & `babelfont-3.0.3/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf` & `babelfont-3.0.3/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf` & `babelfont-3.0.3/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf` & `babelfont-3.0.3/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf` & `babelfont-3.0.3/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf` & `babelfont-3.0.3/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf` & `babelfont-3.0.3/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf` & `babelfont-3.0.3/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf` & `babelfont-3.0.3/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf` & `babelfont-3.0.3/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf` & `babelfont-3.0.3/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf` & `babelfont-3.0.3/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf` & `babelfont-3.0.3/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf` & `babelfont-3.0.3/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf` & `babelfont-3.0.3/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf` & `babelfont-3.0.3/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/HBTest-VF.ttf` & `babelfont-3.0.3/tests/data/testotfs/HBTest-VF.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/MORXTwentyeight.ttf` & `babelfont-3.0.3/tests/data/testotfs/MORXTwentyeight.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/TRAK.ttf` & `babelfont-3.0.3/tests/data/testotfs/TRAK.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf` & `babelfont-3.0.3/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf` & `babelfont-3.0.3/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf` & `babelfont-3.0.3/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf` & `babelfont-3.0.3/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf` & `babelfont-3.0.3/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf` & `babelfont-3.0.3/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf` & `babelfont-3.0.3/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf` & `babelfont-3.0.3/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf` & `babelfont-3.0.3/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf` & `babelfont-3.0.3/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf` & `babelfont-3.0.3/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf` & `babelfont-3.0.3/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf` & `babelfont-3.0.3/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf` & `babelfont-3.0.3/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf` & `babelfont-3.0.3/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf` & `babelfont-3.0.3/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf` & `babelfont-3.0.3/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf` & `babelfont-3.0.3/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf` & `babelfont-3.0.3/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf` & `babelfont-3.0.3/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf` & `babelfont-3.0.3/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf` & `babelfont-3.0.3/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf` & `babelfont-3.0.3/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf` & `babelfont-3.0.3/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf` & `babelfont-3.0.3/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf` & `babelfont-3.0.3/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf` & `babelfont-3.0.3/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf` & `babelfont-3.0.3/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf` & `babelfont-3.0.3/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf` & `babelfont-3.0.3/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf` & `babelfont-3.0.3/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf` & `babelfont-3.0.3/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf` & `babelfont-3.0.3/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf` & `babelfont-3.0.3/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf` & `babelfont-3.0.3/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf` & `babelfont-3.0.3/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf` & `babelfont-3.0.3/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf` & `babelfont-3.0.3/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf` & `babelfont-3.0.3/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf` & `babelfont-3.0.3/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf` & `babelfont-3.0.3/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf` & `babelfont-3.0.3/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/test_features.py` & `babelfont-3.0.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/test_glyphs3_roundtrip.py` & `babelfont-3.0.3/tests/test_glyphs3_roundtrip.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.2/tests/test_otf_loader.py` & `babelfont-3.0.3/tests/test_otf_loader.py`

 * *Files identical despite different names*

