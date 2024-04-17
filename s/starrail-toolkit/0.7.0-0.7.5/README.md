# Comparing `tmp/starrail-toolkit-0.7.0.tar.gz` & `tmp/starrail-toolkit-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.7.0.tar", last modified: Wed Jun 14 13:21:41 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.7.5.tar", last modified: Wed Apr 17 17:36:08 2024, max compression
```

## Comparing `starrail-toolkit-0.7.0.tar` & `starrail-toolkit-0.7.5.tar`

### file list

```diff
@@ -1,80 +1,87 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.878758 starrail-toolkit-0.7.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     6008 2023-06-14 13:21:41.878560 starrail-toolkit-0.7.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     5501 2023-06-14 13:20:38.000000 starrail-toolkit-0.7.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-06-14 13:21:41.878812 starrail-toolkit-0.7.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.868720 starrail-toolkit-0.7.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1939 2023-06-14 09:48:24.000000 starrail-toolkit-0.7.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.869320 starrail-toolkit-0.7.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3827 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.871111 starrail-toolkit-0.7.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/factory.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1164 2023-06-14 07:33:08.000000 starrail-toolkit-0.7.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/migrate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6287 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.871376 starrail-toolkit-0.7.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7233 2023-06-14 09:10:59.000000 starrail-toolkit-0.7.0/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.872320 starrail-toolkit-0.7.0/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      332 2023-06-14 09:10:36.000000 starrail-toolkit-0.7.0/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      679 2023-06-14 08:55:08.000000 starrail-toolkit-0.7.0/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      576 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/common/thread.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.873976 starrail-toolkit-0.7.0/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4456 2023-06-14 13:19:24.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/announcements.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-06-06 06:52:24.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    26369 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-06-13 09:01:52.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/unlock_fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3046 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.874734 starrail-toolkit-0.7.0/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/pie_chart.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.875019 starrail-toolkit-0.7.0/starrail/mihoyo/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-14 09:19:50.000000 starrail-toolkit-0.7.0/starrail/mihoyo/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      241 2023-06-14 09:35:53.000000 starrail-toolkit-0.7.0/starrail/mihoyo/api.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.875559 starrail-toolkit-0.7.0/starrail/unlock/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/service.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.876529 starrail-toolkit-0.7.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2459 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.877353 starrail-toolkit-0.7.0/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5302 2023-06-14 09:04:40.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    10871 2023-06-14 09:35:53.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1349 2023-06-14 10:04:01.000000 starrail-toolkit-0.7.0/starrail/utils/download.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      346 2023-06-14 07:36:34.000000 starrail-toolkit-0.7.0/starrail/utils/misc.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-06-14 13:20:08.000000 starrail-toolkit-0.7.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.878291 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     6008 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1904 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.673571 starrail-toolkit-0.7.5/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6429 2024-04-17 17:36:08.673283 starrail-toolkit-0.7.5/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5599 2024-04-17 17:35:22.000000 starrail-toolkit-0.7.5/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2024-04-17 17:36:08.673623 starrail-toolkit-0.7.5/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.664372 starrail-toolkit-0.7.5/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2068 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.664844 starrail-toolkit-0.7.5/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3827 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.5/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2024-04-13 03:03:06.000000 starrail-toolkit-0.7.5/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.666220 starrail-toolkit-0.7.5/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5240 2024-04-17 17:33:17.000000 starrail-toolkit-0.7.5/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/factory.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1164 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/migrate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6287 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.5/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.666419 starrail-toolkit-0.7.5/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7233 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.667074 starrail-toolkit-0.7.5/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      332 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      685 2024-01-05 08:47:03.000000 starrail-toolkit-0.7.5/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      675 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gui/common/thread.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.668083 starrail-toolkit-0.7.5/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5129 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/announcements.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-06-06 06:52:24.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    26369 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-06-13 09:01:52.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5594 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-06-25 09:04:36.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    11884 2024-04-13 03:06:59.000000 starrail-toolkit-0.7.5/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.668832 starrail-toolkit-0.7.5/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      364 2024-04-13 03:07:16.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/button.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    15816 2024-01-05 09:21:17.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/pie_chart.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.669566 starrail-toolkit-0.7.5/starrail/mihoyo/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/mihoyo/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1784 2024-01-08 17:01:41.000000 starrail-toolkit-0.7.5/starrail/mihoyo/api.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    16347 2024-01-08 17:21:57.000000 starrail-toolkit-0.7.5/starrail/mihoyo/client.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3598 2024-01-08 17:00:36.000000 starrail-toolkit-0.7.5/starrail/mihoyo/dynamic_secret.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      126 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/mihoyo/qrcode.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/mihoyo/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.669905 starrail-toolkit-0.7.5/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.671108 starrail-toolkit-0.7.5/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5030 2024-04-13 03:06:59.000000 starrail-toolkit-0.7.5/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.672159 starrail-toolkit-0.7.5/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6414 2024-01-05 17:14:16.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    12628 2024-04-13 03:06:59.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1349 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/utils/download.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.5/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      915 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1671 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/utils/schedule.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3055 2023-07-22 18:21:50.000000 starrail-toolkit-0.7.5/starrail/utils/security.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2024-04-16 17:06:48.000000 starrail-toolkit-0.7.5/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2024-04-17 17:36:08.672918 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6429 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2102 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)      143 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2024-04-17 17:36:08.000000 starrail-toolkit-0.7.5/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.7.0/LICENSE` & `starrail-toolkit-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/PKG-INFO` & `starrail-toolkit-0.7.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,41 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.7.0
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
-**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
-
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
+|   0.7.5    |    0.7.5     |   0.7.5   |   0.7.5    |
 
 目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 获取官方公告
-- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] ~~支持配置 SToken 用于抽卡导出~~（目前api不支持）
 - [ ] 支持 UP 池计算
 - [ ] 开拓月历
 - [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/iN7870y9o7gb)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwo.lanzouj.com/iyfyP1viohtg)，两种途径的内容相同，可以自行选择下载方式。
 
 ![gui preview gacha](https://s1.ax1x.com/2023/06/01/p9xxdXj.png)
 
+![announcements](https://s1.ax1x.com/2023/06/16/pCMTlxH.png)
+
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
@@ -116,12 +101,12 @@
 
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
-本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。关于账号安全的更多信息，可以访问**[本链接](docs/account-privacy.md)**了解。
 
 ## Credits
 
 本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.7.0/README.md` & `starrail-toolkit-0.7.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,68 @@
+Metadata-Version: 2.1
+Name: starrail-toolkit
+Version: 0.7.5
+Summary: Honkai Star Rail Toolkit
+Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
+Author: LittleNyima
+Author-email: littlenyima@163.com
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: easydict
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: prettytable
+Requires-Dist: PTable
+Requires-Dist: pycryptodomex
+Requires-Dist: PySide6
+Requires-Dist: PySide6_Fluent_Widgets
+Requires-Dist: PySideSix_Frameless_Window
+Requires-Dist: qrcode
+Requires-Dist: requests
+Requires-Dist: setuptools
+
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
-**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
-
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
+|   0.7.5    |    0.7.5     |   0.7.5   |   0.7.5    |
 
 目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 获取官方公告
-- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] ~~支持配置 SToken 用于抽卡导出~~（目前api不支持）
 - [ ] 支持 UP 池计算
 - [ ] 开拓月历
 - [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/iN7870y9o7gb)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwo.lanzouj.com/iyfyP1viohtg)，两种途径的内容相同，可以自行选择下载方式。
 
 ![gui preview gacha](https://s1.ax1x.com/2023/06/01/p9xxdXj.png)
 
+![announcements](https://s1.ax1x.com/2023/06/16/pCMTlxH.png)
+
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
@@ -101,12 +128,12 @@
 
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
-本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。关于账号安全的更多信息，可以访问**[本链接](docs/account-privacy.md)**了解。
 
 ## Credits
 
 本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.7.0/setup.py` & `starrail-toolkit-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/__init__.py` & `starrail-toolkit-0.7.5/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/config.py` & `starrail-toolkit-0.7.5/starrail/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,32 @@
 
 configuration = Configuration(
     cache_dir=srroot,
     db_dir=os.path.join(srroot, 'database'),
     config_path=os.path.join(srroot, 'config.json'),
     account_record_path=os.path.join(srroot, 'accounts.json'),
     res_cache_dir=os.path.join(srroot, 'cache'),
+    user_info_dir=os.path.join(srroot, 'userinfo'),
     check_update=True,
     locale='zhs',
     log_level='DEBUG',
 )
 configuration.set_skip_keys(
     'skip_keys', 'no_flush',
     'cache_dir', 'config_path', 'db_dir', 'account_record_path',
-    'res_cache_dir',
+    'res_cache_dir', 'user_info_dir',
 )
 
 
 def init_config():
 
     os.makedirs(configuration.cache_dir, exist_ok=True)
     os.makedirs(configuration.db_dir, exist_ok=True)
     os.makedirs(configuration.res_cache_dir, exist_ok=True)
+    os.makedirs(configuration.user_info_dir, exist_ok=True)
 
     if os.path.isfile(configuration.config_path):
         with open(configuration.config_path, encoding='utf-8') as fcfg:
             custom_config = json.load(fcfg)
 
         configuration.update(custom_config)
     else:
```

### Comparing `starrail-toolkit-0.7.0/starrail/entry/cli.py` & `starrail-toolkit-0.7.5/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/entry/gui.py` & `starrail-toolkit-0.7.5/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/entry/setup.py` & `starrail-toolkit-0.7.5/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/database.py` & `starrail-toolkit-0.7.5/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/factory.py` & `starrail-toolkit-0.7.5/starrail/gacha/factory.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.7.5/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.7.5/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/migrate.py` & `starrail-toolkit-0.7.5/starrail/gacha/migrate.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/parse.py` & `starrail-toolkit-0.7.5/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/service.py` & `starrail-toolkit-0.7.5/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gacha/url.py` & `starrail-toolkit-0.7.5/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/application.py` & `starrail-toolkit-0.7.5/starrail/gui/application.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/common/config.py` & `starrail-toolkit-0.7.5/starrail/gui/common/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.7.5/starrail/gui/common/stylesheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 
 class StyleSheet(StyleSheetBase, Enum):
     """ Style sheet  """
 
     ANNOUNCEMENT = 'announcement'
     BASE_INTERFACE = 'base_interface'
-    CHECK_UPDATE_DIALOG = 'check_update_dialog'
+    BUTTON = 'button'
     GACHA_RECORD = 'gacha_record'
     HOME_INTERFACE = 'home_interface'
     LINK_CARD = 'link_card'
+    MASK_DIALOG = 'mask_dialog'
     RESULT_TABLE_WIDGET = 'result_table_widget'
     SETTING_INTERFACE = 'setting_interface'
     STAR_RAIL_TOOLKIT = 'star_rail_toolkit'
 
     def path(self, theme=Theme.AUTO):
         theme = qconfig.theme if theme == Theme.AUTO else theme
         return f'resources/qss/{theme.value.lower()}/{self.value}.qss'
```

### Comparing `starrail-toolkit-0.7.0/starrail/gui/common/thread.py` & `starrail-toolkit-0.7.5/starrail/gui/common/thread.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import traceback
 
 from PySide6.QtCore import QThread, Signal
 
-from starrail.utils import babelfish
+from starrail.utils import babelfish, loggings
+
+logger = loggings.get_logger(__file__)
 
 
 class StatefulThread(QThread):
 
     successSignal = Signal(str)
     failureSignal = Signal(str)
 
@@ -14,12 +16,13 @@
         super().__init__(parent=parent)
 
     def run(self):
         try:
             msg = self.work()
             self.successSignal.emit(msg)
         except Exception:
+            logger.error(traceback.format_exc())
             msg = f'{babelfish.ui_traceback()}:\n{traceback.format_exc()}'
             self.failureSignal.emit(msg)
 
     def work(self):
         raise NotImplementedError
```

### Comparing `starrail-toolkit-0.7.0/starrail/gui/common/utils.py` & `starrail-toolkit-0.7.5/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/announcements.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/announcements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 
 import qfluentwidgets as qfw
 from PySide6 import QtCore, QtGui, QtWidgets
 
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.thread import StatefulThread
 from starrail.gui.interfaces.base import BaseInterface
@@ -52,16 +53,18 @@
 
         self.annHBoxLayout = QtWidgets.QHBoxLayout(self.annView)
         self.rightVBoxLayout = QtWidgets.QVBoxLayout(self.annContentView)
 
         self.bannerLabel = QtWidgets.QLabel(text='', parent=self)
         self.annTitleLabel = QtWidgets.QLabel(text='', parent=self)
         self.browser = QtWidgets.QTextBrowser(self)
+        self.browser.anchorClicked.connect(self.onHrefAnchorClicked)
 
         self.updateThread = None
+        self.urlPattern = re.compile(r'^(https?)://[^\s/$.?#].[^\s]*$')
 
         self.__initWidget()
         self.__initLayout()
 
         StyleSheet.ANNOUNCEMENT.apply(self.annView)
         self.updateAnnouncements()
 
@@ -112,14 +115,25 @@
             if success:
                 self.bannerLabel.setPixmap(pixmap)
                 # width = self.browser.width()
                 width = self.width() - self.annList.width() - 72
                 height = int(width * aspectRatio)
                 self.bannerLabel.setFixedSize(width, height)
 
+    def onHrefAnchorClicked(self, qurl: QtCore.QUrl):
+        self.browser.setSource(QtCore.QUrl())
+        url = qurl.toString()
+        jsprefix0 = "javascript:miHoYoGameJSSDK.openInBrowser('"
+        jsprefix1 = "javascript:miHoYoGameJSSDK.openInWebview('"
+        if re.match(self.urlPattern, url):
+            QtGui.QDesktopServices.openUrl(url)
+        elif url.startswith(jsprefix0) or url.startswith(jsprefix1):
+            url = url[len(jsprefix0):].split("'")[0]
+            QtGui.QDesktopServices.openUrl(url)
+
     def resizeEvent(self, e):
         super().resizeEvent(e)
         pixmap = self.bannerLabel.pixmap()
         if pixmap is not None and not pixmap.isNull():
             aspectRatio = pixmap.height() / (pixmap.width() + 1e-6)
             newWidth = self.width() - self.annList.width() - 72
             newHeight = int(newWidth * aspectRatio)
```

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/gacha_sync.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/setting.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from starrail.utils import babelfish
 
 
 class SettingInterface(qfw.ScrollArea):
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
-        self.initialParent = parent
         self.scrollWidget = QWidget()
         self.expandLayout = qfw.ExpandLayout(self.scrollWidget)
 
         self.settingLabel = QLabel(babelfish.ui_settings(), self)
 
         self.personalGroup = qfw.SettingCardGroup(
             title=babelfish.ui_personalization(),
@@ -149,8 +148,8 @@
         )
 
     def __connectSignalToSlot(self):
         qcfg.themeChanged.connect(qfw.setTheme)
         qcfg.appRestartSig.connect(self.__showRestartToolTip)
 
     def checkUpdateAction(self):
-        checkUpdate(parent=self.initialParent, show_success=True)
+        checkUpdate(parent=self.window(), show_success=True)
```

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/unlock_fps.py` & `starrail-toolkit-0.7.5/starrail/gui/interfaces/unlock_fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/interfaces/users.py` & `starrail-toolkit-0.7.5/starrail/gui/widgets/link_card.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,72 @@
-from typing import List
+import qfluentwidgets
+from PySide6.QtCore import Qt, QUrl
+from PySide6.QtGui import QDesktopServices
+from PySide6.QtWidgets import QFrame, QHBoxLayout, QLabel, QVBoxLayout, QWidget
+from qfluentwidgets import FluentIcon, IconWidget, TextWrap
 
-import qfluentwidgets as qfw
-from PySide6 import QtWidgets
+from starrail.gui.common.stylesheet import StyleSheet
 
-from starrail.gui.interfaces.base import BaseInterface
-from starrail.utils import babelfish
-from starrail.utils.accounts import account_record as ar
+AF = Qt.AlignmentFlag
 
 
-class UserItemWidget(QtWidgets.QWidget):
+class LinkCard(QFrame):
 
-    def __init__(self, uid, users, parent=None):
+    def __init__(self, icon, title, content, url, parent=None):
         super().__init__(parent=parent)
-        self.uid = uid
-        self.users = users
-
-        self.hBoxLayout = QtWidgets.QHBoxLayout(self)
-        self.uidLabel = QtWidgets.QLabel(text=uid, parent=self)
-        self.selectedLabel = QtWidgets.QLabel(
-            text=babelfish.ui_current_account(),
-            parent=self,
-        )
-        self.selectButton = qfw.PrimaryPushButton(
-            text=babelfish.ui_switch(),
-            parent=self,
-        )
-        self.selectButton.clicked.connect(self.onSelectButtonClicked)
+        self.url = QUrl(url)
+        self.setFixedSize(198, 220)
+        self.iconWidget = IconWidget(icon, self)
+        self.titleLabel = QLabel(title, self)
+        self.contentLabel = QLabel(TextWrap.wrap(content, 28, False)[0], self)
+        self.urlWidget = IconWidget(FluentIcon.LINK, self)
 
         self.__initWidget()
-        self.__initLayout()
 
     def __initWidget(self):
-        self.setContentsMargins(0, 0, 0, 0)
-        self.hBoxLayout.setContentsMargins(0, 5, 0, 5)
-        self.hBoxLayout.setSpacing(0)
-
-    def __initLayout(self):
-        self.hBoxLayout.addWidget(self.uidLabel)
-        self.hBoxLayout.addSpacing(10)
-        self.hBoxLayout.addWidget(self.selectedLabel)
-        self.hBoxLayout.addStretch(1)
-        self.hBoxLayout.addWidget(self.selectButton)
-
-    def setSelected(self, selected):
-        self.selectButton.setEnabled(not selected)
-        self.selectedLabel.setVisible(selected)
+        self.setCursor(Qt.CursorShape.PointingHandCursor)
 
-    def onSelectButtonClicked(self):
-        selectUser(self, self.users)
-        ar.latest_uid = self.uid
+        self.iconWidget.setFixedSize(54, 54)
+        self.urlWidget.setFixedSize(16, 16)
 
-
-def selectUser(select: UserItemWidget, users: List[UserItemWidget]):
-    for user in users:
-        user.setSelected(user is select)
+        self.vBoxLayout = QVBoxLayout(self)
+        self.vBoxLayout.setSpacing(0)
+        self.vBoxLayout.setContentsMargins(24, 24, 0, 13)
+        self.vBoxLayout.addWidget(self.iconWidget)
+        self.vBoxLayout.addSpacing(16)
+        self.vBoxLayout.addWidget(self.titleLabel)
+        self.vBoxLayout.addSpacing(8)
+        self.vBoxLayout.addWidget(self.contentLabel)
+        self.vBoxLayout.setAlignment(AF.AlignLeft | AF.AlignTop)
+        self.urlWidget.move(170, 192)
+
+        self.titleLabel.setObjectName('titleLabel')
+        self.contentLabel.setObjectName('contentLabel')
+
+    def mouseReleaseEvent(self, e):
+        super().mouseReleaseEvent(e)
+        QDesktopServices.openUrl(self.url)
 
 
-class UserListWidget(QtWidgets.QWidget):
+class LinkCardView(qfluentwidgets.SingleDirectionScrollArea):
+    """ Link card view """
 
     def __init__(self, parent=None):
-        super().__init__(parent=parent)
-
-        self.vBoxLayout = QtWidgets.QVBoxLayout(self)
-        self.vBoxLayout.setSpacing(0)
-        self.vBoxLayout.setContentsMargins(0, 0, 0, 0)
-        self.setContentsMargins(0, 0, 0, 0)
-
-        self.users = []
-
-    def addUserItem(self, uid):
-        userItem = UserItemWidget(uid=uid, users=self.users, parent=self)
-        self.vBoxLayout.addWidget(userItem)
-        self.users.append(userItem)
-        return userItem
-
-    def clear(self):
-        for user in self.users:
-            self.vBoxLayout.removeWidget(user)
-        self.users.clear()
-
-
-class UsersInterface(BaseInterface):
-
-    def __init__(self, title, subtitle, parent):
-        super().__init__(title, subtitle, parent)
-
-        self.userCard = self.addCard('User List')
-        self.userList = UserListWidget(self)
-        self.userCard.addWidget(self.userList)
-
-        self.updateUserList()
-
-    def updateUserList(self):
-        self.userList.clear()
-        latest = ar.latest_uid
-        latestItem = None
-        for account in ar.accounts:
-            item = self.userList.addUserItem(account)
-            if account == latest:
-                latestItem = item
-        selectUser(latestItem, self.userList.users)
+        super().__init__(parent, Qt.Orientation.Horizontal)
+        self.view = QWidget(self)
+        self.hBoxLayout = QHBoxLayout(self.view)
+
+        self.hBoxLayout.setContentsMargins(36, 0, 0, 0)
+        self.hBoxLayout.setSpacing(12)
+        self.hBoxLayout.setAlignment(AF.AlignLeft)
+
+        self.setWidget(self.view)
+        self.setWidgetResizable(True)
+        self.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+
+        self.view.setObjectName('view')
+        StyleSheet.LINK_CARD.apply(self)
+
+    def addCard(self, icon, title, content, url):
+        """ add link card """
+        card = LinkCard(icon, title, content, url, self.view)
+        self.hBoxLayout.addWidget(card, 0, AF.AlignLeft)
```

### Comparing `starrail-toolkit-0.7.0/starrail/gui/widgets/pie_chart.py` & `starrail-toolkit-0.7.5/starrail/gui/widgets/pie_chart.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.7.5/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/unlock/fps.py` & `starrail-toolkit-0.7.5/starrail/unlock/fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/utils/auto_update.py` & `starrail-toolkit-0.7.5/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.7.5/starrail/utils/babelfish/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,26 +17,32 @@
 ui_about = dictionary.ui_about
 ui_about_this = dictionary.ui_about_this
 ui_announcements = dictionary.ui_announcements
 ui_announcements_desc = dictionary.ui_announcements_desc
 ui_arerage_warps_per_5star = dictionary.ui_arerage_warps_per_5star
 ui_auto = dictionary.ui_auto
 ui_average_warps_per_up = dictionary.ui_average_warps_per_up
+ui_cancel = dictionary.ui_cancel
 ui_cancel_update = dictionary.ui_cancel_update
 ui_check_update = dictionary.ui_check_update
 ui_check_update_at_start = dictionary.ui_check_update_at_start
 ui_check_update_at_start_desc = dictionary.ui_check_update_at_start_desc
 ui_check_update_fail = dictionary.ui_check_update_fail
 ui_check_update_success = dictionary.ui_check_update_success
+ui_connect_finish = dictionary.ui_connect_finish
+ui_connect_status = dictionary.ui_connect_status
+ui_connect_to_hoyolab = dictionary.ui_connect_to_hoyolab
+ui_connected = dictionary.ui_connected
 ui_copyright = dictionary.ui_copyright
 ui_curr_fps = dictionary.ui_curr_fps
 ui_current_account = dictionary.ui_current_account
 ui_current_version = dictionary.ui_current_version
 ui_customize_url = dictionary.ui_customize_url
 ui_deduce_uid_fail = dictionary.ui_deduce_uid_fail
+ui_done = dictionary.ui_done
 ui_downloading_gacha = dictionary.ui_downloading_gacha
 ui_en = dictionary.ui_en
 ui_extract_api_fail = dictionary.ui_extract_api_fail
 ui_extract_api_fail_with_msg = dictionary.ui_extract_api_fail_with_msg
 ui_extracting_api_url = dictionary.ui_extracting_api_url
 ui_fine = dictionary.ui_fine
 ui_fine1 = dictionary.ui_fine1
@@ -50,36 +56,48 @@
 ui_gacha_sync_desc = dictionary.ui_gacha_sync_desc
 ui_gacha_true_prob = dictionary.ui_gacha_true_prob
 ui_gacha_type = dictionary.ui_gacha_type
 ui_get_started = dictionary.ui_get_started
 ui_get_started_desc = dictionary.ui_get_started_desc
 ui_github_repo = dictionary.ui_github_repo
 ui_github_repo_desc = dictionary.ui_github_repo_desc
+ui_hoyolab_connect_status = dictionary.ui_hoyolab_connect_status
+ui_hoyolab_unconnect_msg = dictionary.ui_hoyolab_unconnect_msg
+ui_hoyolab_unconnect_title = dictionary.ui_hoyolab_unconnect_title
+ui_html_bold = dictionary.ui_html_bold
+ui_html_font_color = dictionary.ui_html_font_color
 ui_is_latest_version = dictionary.ui_is_latest_version
+ui_last_update_at = dictionary.ui_last_update_at
 ui_load_failure = dictionary.ui_load_failure
 ui_load_gacha = dictionary.ui_load_gacha
 ui_load_success = dictionary.ui_load_success
 ui_load_success_msg = dictionary.ui_load_success_msg
 ui_locale = dictionary.ui_locale
 ui_locale_setting_desc = dictionary.ui_locale_setting_desc
 ui_no_data = dictionary.ui_no_data
+ui_not_connected = dictionary.ui_not_connected
 ui_not_good = dictionary.ui_not_good
+ui_ok = dictionary.ui_ok
 ui_ooops = dictionary.ui_ooops
 ui_open_docs = dictionary.ui_open_docs
 ui_open_issues = dictionary.ui_open_issues
 ui_open_repo = dictionary.ui_open_repo
 ui_open_troubleshooting = dictionary.ui_open_troubleshooting
 ui_operation_zone = dictionary.ui_operation_zone
 ui_personalization = dictionary.ui_personalization
 ui_reset_fps = dictionary.ui_reset_fps
 ui_reset_panel = dictionary.ui_reset_panel
 ui_save_data = dictionary.ui_save_data
 ui_save_failure = dictionary.ui_save_failure
 ui_save_success = dictionary.ui_save_success
 ui_save_success_msg = dictionary.ui_save_success_msg
+ui_scan_code_instr = dictionary.ui_scan_code_instr
+ui_scan_confirmed = dictionary.ui_scan_confirmed
+ui_scan_init = dictionary.ui_scan_init
+ui_scan_scanned = dictionary.ui_scan_scanned
 ui_send_feedback = dictionary.ui_send_feedback
 ui_send_feedback_desc = dictionary.ui_send_feedback_desc
 ui_set_fps_fail_with_msg = dictionary.ui_set_fps_fail_with_msg
 ui_setting_failure = dictionary.ui_setting_failure
 ui_setting_panel = dictionary.ui_setting_panel
 ui_setting_restart_content = dictionary.ui_setting_restart_content
 ui_setting_restart_title = dictionary.ui_setting_restart_title
@@ -93,23 +111,29 @@
 ui_sync_gacha_initial = dictionary.ui_sync_gacha_initial
 ui_sync_gacha_success = dictionary.ui_sync_gacha_success
 ui_synchronizing_gacha = dictionary.ui_synchronizing_gacha
 ui_theme_mode = dictionary.ui_theme_mode
 ui_theme_mode_dark = dictionary.ui_theme_mode_dark
 ui_theme_mode_light = dictionary.ui_theme_mode_light
 ui_theme_mode_settings_desc = dictionary.ui_theme_mode_settings_desc
+ui_time_fmt = dictionary.ui_time_fmt
 ui_title = dictionary.ui_title
 ui_total_warp = dictionary.ui_total_warp
 ui_traceback = dictionary.ui_traceback
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
+ui_unconnect_to_hoyolab = dictionary.ui_unconnect_to_hoyolab
+ui_unknown = dictionary.ui_unknown
 ui_unlock_fps = dictionary.ui_unlock_fps
 ui_unlock_fps_desc = dictionary.ui_unlock_fps_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
 ui_use_customize_url = dictionary.ui_use_customize_url
+ui_user_list = dictionary.ui_user_list
 ui_users = dictionary.ui_users
 ui_users_desc = dictionary.ui_users_desc
+ui_wait_for_connection = dictionary.ui_wait_for_connection
+ui_waiting = dictionary.ui_waiting
 ui_welcome = dictionary.ui_welcome
 ui_zhs = dictionary.ui_zhs
 
 __all__ = ['constants', 'translate']
```

### Comparing `starrail-toolkit-0.7.0/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.7.5/starrail/utils/babelfish/dictionary.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     zhs='五星平均抽数',
 )
 ui_auto = _MS(en='Auto', zhs='跟随系统设置')
 ui_average_warps_per_up = _MS(
     en='Average warps per up',
     zhs='UP 平均抽数',
 )
+ui_cancel = _MS(en='Cancel', zhs='取消')
 ui_cancel_update = _MS(en='Cancel Update', zhs='暂不更新')
 ui_check_update = _MS(en='Check Update', zhs='检查更新')
 ui_check_update_at_start = _MS(
     en='Check Update at Application Start',
     zhs='启动时自动检查更新',
 )
 ui_check_update_at_start_desc = _MS(
@@ -86,14 +87,18 @@
     en='Check update failed. Please check your network connection.',
     zhs='检查更新失败，请检查你的网络连接并重试。（不重试也行，但是你可能没联网）',
 )
 ui_check_update_success = _MS(
     en='Check update finished',
     zhs='检查更新完成',
 )
+ui_connect_finish = _MS(en='Connection done.', zhs='绑定完成。')
+ui_connect_status = _MS(en='Connection Status: {}', zhs='绑定状态：{}')
+ui_connect_to_hoyolab = _MS(en='Connect to HoyoLab', zhs='绑定米游社')
+ui_connected = _MS(en='Connected', zhs='已绑定')
 ui_copyright = _MS(
     en='Copyright © {} LittleNyima.',
     zhs='版权所有 © {} LittleNyima。',
 )
 ui_curr_fps = _MS(
     en='Current FPS in Game Settings: {}.',
     zhs='当前游戏设定帧率：{}。',
@@ -107,14 +112,15 @@
     en='Customize API URL',
     zhs='自定义 API URL',
 )
 ui_deduce_uid_fail = _MS(
     en='Fail to deduce uid. There may be no record. Please check.',
     zhs='检测 UID 失败，账号可能没有抽卡记录，请重试。',
 )
+ui_done = _MS(en='Done', zhs='完成')
 ui_downloading_gacha = _MS(
     en='Downloading page {page} of type {name}',
     zhs='正在导出{name}的第{page}页',
 )
 ui_en = _MS(
     en='English',
     zhs='英语',
@@ -161,29 +167,46 @@
     zhs='学习本工具箱的基本使用方法。',
 )
 ui_github_repo = _MS(en='GitHub Repo', zhs='开源代码')
 ui_github_repo_desc = _MS(
     en='This project is open-resource, licenced under GPLv3. View code here.',
     zhs='本项目代码开源，以 GPLv3 分发。点此查看源代码。',
 )
+ui_hoyolab_connect_status = _MS(en='HoyoLab Connection: {}', zhs='米游社绑定：{}')
+ui_hoyolab_unconnect_msg = _MS(
+    en='Caution: This operation is irreversible!',
+    zhs='注意：这一操作不可撤销！',
+)
+ui_hoyolab_unconnect_title = _MS(
+    en='Unconnect?',
+    zhs='确认取消绑定？',
+)
+ui_html_bold = _MS(en='<b>{}</b>', zhs='<b>{}</b>')
+ui_html_font_color = _MS(
+    en='<font color="{color}">{}</font>',
+    zhs='<font color="{color}">{}</font>',
+)
 ui_is_latest_version = _MS(
     en='Your application is the latest version.',
     zhs='已经是最新版本啦',
 )
+ui_last_update_at = _MS(en='Last Update: {}', zhs='上一次更新于：{}')
 ui_load_failure = _MS(en='Record Load Failed', zhs='加载失败')
 ui_load_gacha = _MS(en='Import from JSON', zhs='导入数据')
 ui_load_success = _MS(en='Record Load Success', zhs='加载成功')
 ui_load_success_msg = _MS(
     en='Successfully loaded {cnt} items for uid {uid}.',
     zhs='成功导入了用户{uid}的{cnt}条记录。',
 )
 ui_locale = _MS(en='Display Language', zhs='显示语言')
 ui_locale_setting_desc = _MS(en='Changing the display language', zhs='改变显示语言')
 ui_no_data = _MS(en='No Data', zhs='暂无数据')
+ui_not_connected = _MS(en='Not Connected', zhs='未绑定')
 ui_not_good = _MS(en='No', zhs='不好')
+ui_ok = _MS(en='OK', zhs='确认')
 ui_ooops = _MS(en='OOOPS!', zhs='出错了！')
 ui_open_docs = _MS(en='Open Documentations', zhs='打开帮助页面')
 ui_open_issues = _MS(en='Open Issue Page', zhs='打开反馈页面')
 ui_open_repo = _MS(en='Open GitHub Repo', zhs='打开代码仓库')
 ui_open_troubleshooting = _MS(en='Open Troubleshooting', zhs='打开常见问题')
 ui_operation_zone = _MS(en='Operations', zhs='操作区')
 ui_personalization = _MS(en='Personalization', zhs='个性化')
@@ -192,14 +215,21 @@
     zhs='重置帧率',
 )
 ui_reset_panel = _MS(en='Reset Panel', zhs='重置面板')
 ui_save_data = _MS(en='Save As', zhs='保存数据')
 ui_save_failure = _MS(en='Data Save Failed', zhs='保存失败')
 ui_save_success = _MS(en='Data Save Success', zhs='保存成功')
 ui_save_success_msg = _MS(en='Data is saved to {}', zhs='数据已保存到{}')
+ui_scan_code_instr = _MS(
+    en='Scan QR code with HoyoLab client to login. Current Status: {}.',
+    zhs='用米游社手机客户端扫描二维码以登陆。扫描状态：{}。',
+)
+ui_scan_confirmed = _MS(en='Confirmed', zhs='已确认')
+ui_scan_init = _MS(en='Not Scanned', zhs='未扫描')
+ui_scan_scanned = _MS(en='Scanned', zhs='已扫描')
 ui_send_feedback = _MS(en='Send Feedback', zhs='提交反馈')
 ui_send_feedback_desc = _MS(
     en='Feedback is welcome if you encounter problems or have suggestions.',
     zhs='如果你遇到问题，或对本项目有更多建议，欢迎提交反馈。',
 )
 ui_set_fps_fail_with_msg = _MS(
     en='Setting FPS failed. Failed with: {}',
@@ -243,22 +273,25 @@
 ui_theme_mode = _MS(en='Theme Mode', zhs='应用主题')
 ui_theme_mode_dark = _MS(en='Dark', zhs='深色')
 ui_theme_mode_light = _MS(en='Light', zhs='浅色')
 ui_theme_mode_settings_desc = _MS(
     en='Changing the appearance of application',
     zhs='改变应用外观',
 )
+ui_time_fmt = _MS(en='%Y/%m/%d %H:%M:%S', zhs='%Y/%m/%d %H:%M:%S')
 ui_title = _MS(en='Honkai: Star Rail Toolkit', zhs='崩坏：星穹铁道工具箱')
 ui_total_warp = _MS(en='Total Warp', zhs='总抽数')
 ui_traceback = _MS(en='Traceback', zhs='报错信息')
 ui_troubleshooting = _MS(en='TroubleShooting', zhs='常见问题')
 ui_troubleshooting_desc = _MS(
     en='Click here to view FAQ.',
     zhs='点此查看常见问题解答。',
 )
+ui_unconnect_to_hoyolab = _MS(en='Unconnect', zhs='解除绑定')
+ui_unknown = _MS(en='unkown', zhs='未知')
 ui_unlock_fps = _MS(
     en='Unlock FPS Settings',
     zhs='解锁帧率',
 )
 ui_unlock_fps_desc = _MS(
     en=(
         'First set the frame rate in the game at least once, and then use the '
@@ -279,16 +312,22 @@
     ),
     zhs=(
         '崩坏：星穹铁道工具箱有新的可用版本，更新日志：{}\n 请更新到最新版本以使用全新'
         '功能。如果你对GitHub的连接不稳定，请从网盘下载最新版本。'
     ),
 )
 ui_use_customize_url = _MS(en='Use Customize URL', zhs='使用自定义URL')
+ui_user_list = _MS(en='Users List', zhs='用户列表')
 ui_users = _MS(en='Users', zhs='用户管理')
 ui_users_desc = _MS(en='Multi-user management', zhs='如果有多个账号可以用这个切换')
+ui_wait_for_connection = _MS(
+    en='Connecting to HoyoLab, please wait...',
+    zhs='正在绑定，请等待...',
+)
+ui_waiting = _MS(en='Waiting', zhs='等待中')
 ui_welcome = _MS(
     en='Welcome to HKSR Toolkit!',
     zhs='欢迎登车！',
 )
 ui_zhs = _MS(
     en='Simplified Chinese',
     zhs='简体中文',
```

### Comparing `starrail-toolkit-0.7.0/starrail/utils/babelfish/locale.py` & `starrail-toolkit-0.7.5/starrail/utils/babelfish/locale.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.7.5/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/utils/download.py` & `starrail-toolkit-0.7.5/starrail/utils/download.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail/utils/loggings.py` & `starrail-toolkit-0.7.5/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.7.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.7.5/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.7.0
+Version: 0.7.5
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: easydict
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: prettytable
+Requires-Dist: PTable
+Requires-Dist: pycryptodomex
+Requires-Dist: PySide6
+Requires-Dist: PySide6_Fluent_Widgets
+Requires-Dist: PySideSix_Frameless_Window
+Requires-Dist: qrcode
+Requires-Dist: requests
+Requires-Dist: setuptools
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
-**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
-
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
+|   0.7.5    |    0.7.5     |   0.7.5   |   0.7.5    |
 
 目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 获取官方公告
-- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] ~~支持配置 SToken 用于抽卡导出~~（目前api不支持）
 - [ ] 支持 UP 池计算
 - [ ] 开拓月历
 - [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/iN7870y9o7gb)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwo.lanzouj.com/iyfyP1viohtg)，两种途径的内容相同，可以自行选择下载方式。
 
 ![gui preview gacha](https://s1.ax1x.com/2023/06/01/p9xxdXj.png)
 
+![announcements](https://s1.ax1x.com/2023/06/16/pCMTlxH.png)
+
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
@@ -116,12 +128,12 @@
 
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
-本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。关于账号安全的更多信息，可以访问**[本链接](docs/account-privacy.md)**了解。
 
 ## Credits
 
 本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.7.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.7.5/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,29 +32,36 @@
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/unlock_fps.py
 starrail/gui/interfaces/users.py
 starrail/gui/widgets/__init__.py
+starrail/gui/widgets/button.py
 starrail/gui/widgets/dialog.py
 starrail/gui/widgets/link_card.py
 starrail/gui/widgets/pie_chart.py
 starrail/gui/widgets/title_bar.py
 starrail/mihoyo/__init__.py
 starrail/mihoyo/api.py
+starrail/mihoyo/client.py
+starrail/mihoyo/dynamic_secret.py
+starrail/mihoyo/qrcode.py
+starrail/mihoyo/service.py
 starrail/unlock/__init__.py
 starrail/unlock/fps.py
 starrail/unlock/service.py
 starrail/utils/__init__.py
 starrail/utils/accounts.py
 starrail/utils/auto_update.py
 starrail/utils/download.py
 starrail/utils/loggings.py
 starrail/utils/misc.py
+starrail/utils/schedule.py
+starrail/utils/security.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
 starrail/utils/babelfish/translate.py
 starrail_toolkit.egg-info/PKG-INFO
```

