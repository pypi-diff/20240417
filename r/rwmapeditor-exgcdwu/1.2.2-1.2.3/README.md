# Comparing `tmp/rwmapeditor_exgcdwu-1.2.2.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.2.2.tar", last modified: Wed Apr 17 17:02:27 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.2.3.tar", last modified: Wed Apr 17 17:09:18 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.2.2.tar` & `rwmapeditor_exgcdwu-1.2.3.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.363682 rwmapeditor_exgcdwu-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42677 2024-04-17 17:02:27.363682 rwmapeditor_exgcdwu-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.323681 rwmapeditor_exgcdwu-1.2.2/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.323681 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.323681 rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.323681 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.323681 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.331682 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.355682 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16202 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/water2deepwater_flat.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.355682 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/units.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_one.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/default_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tile_group_grid/tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tobject_group_COP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/rwmap/data/tobject_group_COP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:02:27.359682 rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42677 2024-04-17 17:02:27.000000 rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-17 17:02:27.000000 rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:02:27.000000 rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 17:02:27.000000 rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 17:02:27.363682 rwmapeditor_exgcdwu-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 17:02:08.000000 rwmapeditor_exgcdwu-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42677 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.486514 rwmapeditor_exgcdwu-1.2.3/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.486514 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.486514 rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.486514 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.486514 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.494514 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.522514 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16202 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/water2deepwater_flat.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.522514 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/units.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.522514 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.522514 rwmapeditor_exgcdwu-1.2.3/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/rwmap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/default_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tile_group_grid/tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tobject_group_COP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/rwmap/data/tobject_group_COP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:09:18.526514 rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42677 2024-04-17 17:09:18.000000 rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-17 17:09:18.000000 rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:09:18.000000 rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 17:09:18.000000 rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 17:09:18.530514 rwmapeditor_exgcdwu-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 17:09:01.000000 rwmapeditor_exgcdwu-1.2.3/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.2.2/LICENSE` & `rwmapeditor_exgcdwu-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.2
+Version: 1.2.3
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.2.2/README.md` & `rwmapeditor_exgcdwu-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_case/_tileset.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self, properties:frame.ElementProperties, tileset_list:list[case.TileSet],
                   layer_list:list[case.Layer], objectGroup_list:list[case.ObjectGroup])->None:
         super().__init__(properties)
         self._tileset_list = tileset_list
         self._layer_list = layer_list
         self._objectGroup_list = objectGroup_list
     @classmethod
-    def init_mapfile(cls, map_file:str, rwmaps_dir:str = RWMAP_DIR + "/_maps")->None:
+    def init_mapfile(cls, map_file:str, rwmaps_dir:str = RWMAP_DIR + "/_maps/")->None:
         xmlTree:et.ElementTree = et.ElementTree(file=map_file)
         root:et.Element = xmlTree.getroot()
         properties = frame.ElementProperties.init_etElement(root)
 
         tileset_list = [case.TileSet(frame.ElementProperties("tileset", {"firstgid": "0", "name": "empty"}), frame.Coordinate(1, 1))]
         tileset_list = tileset_list + [case.TileSet.init_etElement(tileset, rwmaps_dir) for tileset in root if tileset.tag == "tileset"]
         layer_list = [case.Layer.init_etElement(layer) for layer in root if layer.tag == "layer"]
```

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/misc.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/ridges/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/ridges/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_maps/units.tsx` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_one.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_one.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_pos.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_object/_object_pro.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_object/_object_pro.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.2.3/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.2
+Version: 1.2.3
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.2.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.2.3/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.2/setup.py` & `rwmapeditor_exgcdwu-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.2.2'
+__version__ = '1.2.3'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 setup(
     name = 'rwmapeditor_exgcdwu',
```

