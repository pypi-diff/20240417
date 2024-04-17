# Comparing `tmp/pairef-1.3.9.tar.gz` & `tmp/pairef-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pairef-1.3.9.tar", last modified: Wed Jun  8 11:44:30 2022, max compression
+gzip compressed data, was "dist/pairef-1.4.0.tar", last modified: Wed Apr 17 10:13:23 2024, max compression
```

## Comparing `pairef-1.3.9.tar` & `pairef-1.4.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/README_images/
--rw-r--r--   0 malyma   (14175) malyma   (14175)    78006 2020-04-30 13:41:20.000000 pairef-1.3.9/README_images/example_head.gif
--rw-r--r--   0 malyma   (14175) malyma   (14175)    51493 2020-06-10 11:16:20.000000 pairef-1.3.9/README_images/example_gui.gif
--rw-r--r--   0 malyma   (14175) malyma   (14175)   114880 2020-04-30 13:41:20.000000 pairef-1.3.9/README_images/example_free_work.gif
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     1762 2021-12-14 10:00:31.000000 pairef-1.3.9/setup.py
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/test/
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     8245 2022-02-03 16:01:50.000000 pairef-1.3.9/test/test_initial.py
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/test/fixtures/
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1044 2020-01-03 15:59:07.000000 pairef-1.3.9/test/fixtures/NK_R00_1-80A.csv
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1131 2020-01-03 15:59:07.000000 pairef-1.3.9/test/fixtures/NK_R00_1-70A.csv
--rw-r--r--   0 malyma   (14175) malyma   (14175)    68380 2019-02-19 11:09:43.000000 pairef-1.3.9/test/fixtures/lysozyme_1-40A.log
--rw-r--r--   0 malyma   (14175) malyma   (14175)      595 2019-02-19 11:09:43.000000 pairef-1.3.9/test/fixtures/A_R-values.csv
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1305 2020-01-03 15:59:07.000000 pairef-1.3.9/test/fixtures/NK_R00_1-50A.csv
--rw-rw-r--   0 malyma   (14175) malyma   (14175)  1432288 2022-01-27 17:15:53.000000 pairef-1.3.9/test/fixtures/mdm2_merged.mtz
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1218 2020-01-03 15:59:07.000000 pairef-1.3.9/test/fixtures/NK_R00_1-60A.csv
--rw-rw-r--   0 malyma   (14175) malyma   (14175)   152901 2022-01-27 17:15:53.000000 pairef-1.3.9/test/fixtures/mdm2_1-60A.pdb
--rw-r--r--   0 malyma   (14175) malyma   (14175)      199 2019-02-19 11:09:43.000000 pairef-1.3.9/test/fixtures/NK_Rgap.csv
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    11342 2022-01-31 13:30:20.000000 pairef-1.3.9/test/test_integration_quick.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    11295 2022-05-27 08:06:38.000000 pairef-1.3.9/test/test_integration_long.py
--rw-r--r--   0 malyma   (14175) malyma   (14175)     4219 2020-05-28 10:35:11.000000 pairef-1.3.9/test/test_graphs.py
--rw-r--r--   0 malyma   (14175) malyma   (14175)     5934 2019-02-19 11:18:25.000000 pairef-1.3.9/test/test_commons.py
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1803 2022-06-08 10:47:32.000000 pairef-1.3.9/test/helper.py
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1312 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/SOURCES.txt
--rw-r--r--   0 malyma   (14175) malyma   (14175)        7 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/top_level.txt
--rw-r--r--   0 malyma   (14175) malyma   (14175)        1 2020-02-26 13:13:55.000000 pairef-1.3.9/pairef.egg-info/not-zip-safe
--rw-r--r--   0 malyma   (14175) malyma   (14175)        1 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/dependency_links.txt
--rw-r--r--   0 malyma   (14175) malyma   (14175)     4522 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/PKG-INFO
--rw-r--r--   0 malyma   (14175) malyma   (14175)       83 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/entry_points.txt
--rw-r--r--   0 malyma   (14175) malyma   (14175)       17 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef.egg-info/requires.txt
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     4522 2022-06-08 11:44:30.000000 pairef-1.3.9/PKG-INFO
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     3130 2021-12-14 10:00:31.000000 pairef-1.3.9/README.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)      181 2020-06-10 13:01:48.000000 pairef-1.3.9/MANIFEST.in
--rw-r--r--   0 malyma   (14175) malyma   (14175)       63 2022-06-08 11:44:30.000000 pairef-1.3.9/setup.cfg
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef/
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/pairef/static/
--rw-r--r--   0 malyma   (14175) malyma   (14175)    12430 2020-04-30 13:41:21.000000 pairef-1.3.9/pairef/static/pairef_logo_64.png
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     2327 2022-01-27 17:15:53.000000 pairef-1.3.9/pairef/static/styles.css
--rw-rw-r--   0 malyma   (14175) malyma   (14175)      183 2022-01-27 17:14:35.000000 pairef-1.3.9/pairef/settings.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)       63 2022-01-27 17:14:35.000000 pairef-1.3.9/pairef/__main__.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     7058 2022-01-27 17:14:35.000000 pairef-1.3.9/pairef/commons.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    46652 2022-06-08 10:32:38.000000 pairef-1.3.9/pairef/graphs.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)       98 2022-06-08 11:35:38.000000 pairef-1.3.9/pairef/__init__.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    50198 2022-06-08 10:32:23.000000 pairef-1.3.9/pairef/refinement.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    56247 2022-06-08 10:32:24.000000 pairef-1.3.9/pairef/preparation.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    31162 2022-06-08 11:33:58.000000 pairef-1.3.9/pairef/gui.py
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    50101 2022-06-08 10:32:26.000000 pairef-1.3.9/pairef/launcher.py
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/docs/
-drwxrwxr-x   0 malyma   (14175) malyma   (14175)        0 2022-06-08 11:44:30.000000 pairef-1.3.9/docs/_static/
--rw-r--r--   0 malyma   (14175) malyma   (14175)    20366 2020-04-30 13:41:20.000000 pairef-1.3.9/docs/_static/example_R-values.png
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    38663 2021-03-16 11:26:10.000000 pairef-1.3.9/docs/_static/phenix_command_prompt.gif
--rw-r--r--   0 malyma   (14175) malyma   (14175)    38533 2020-04-30 13:41:20.000000 pairef-1.3.9/docs/_static/example_CCfree.png
--rw-rw-r--   0 malyma   (14175) malyma   (14175)    33509 2021-03-16 11:24:46.000000 pairef-1.3.9/docs/_static/ccp4console.gif
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1220 2020-04-30 13:41:20.000000 pairef-1.3.9/docs/list_of_functions.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)      810 2019-02-19 14:33:16.000000 pairef-1.3.9/docs/make.bat
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1477 2021-06-03 13:32:19.000000 pairef-1.3.9/docs/gui.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)       24 2019-02-19 11:09:41.000000 pairef-1.3.9/docs/requirements.txt
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     2985 2021-12-14 10:00:31.000000 pairef-1.3.9/docs/index.rst
--rw-rw-r--   0 malyma   (14175) malyma   (14175)     9321 2021-12-14 10:00:31.000000 pairef-1.3.9/docs/installation.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)    17145 2021-03-16 11:51:08.000000 pairef-1.3.9/docs/using.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)      612 2020-04-30 13:41:21.000000 pairef-1.3.9/docs/test.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)      604 2021-11-29 07:45:18.000000 pairef-1.3.9/docs/Makefile
--rw-r--r--   0 malyma   (14175) malyma   (14175)     5485 2021-03-22 11:34:04.000000 pairef-1.3.9/docs/conf.py
--rw-r--r--   0 malyma   (14175) malyma   (14175)     1007 2020-06-10 14:02:34.000000 pairef-1.3.9/docs/credits.rst
--rw-r--r--   0 malyma   (14175) malyma   (14175)     8057 2020-06-10 07:39:18.000000 pairef-1.3.9/LICENSE
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8057 2023-02-28 22:40:52.000000 pairef-1.4.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)      181 2023-02-28 22:40:52.000000 pairef-1.4.0/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4221 2024-04-17 10:13:23.000000 pairef-1.4.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3130 2023-02-28 22:40:52.000000 pairef-1.4.0/README.rst
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/README_images/
+-rw-rw-r--   0 martin    (1000) martin    (1000)   114880 2023-02-28 22:40:52.000000 pairef-1.4.0/README_images/example_free_work.gif
+-rw-rw-r--   0 martin    (1000) martin    (1000)    51493 2023-02-28 22:40:52.000000 pairef-1.4.0/README_images/example_gui.gif
+-rw-rw-r--   0 martin    (1000) martin    (1000)    78006 2023-02-28 22:40:52.000000 pairef-1.4.0/README_images/example_head.gif
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/docs/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      604 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/Makefile
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/docs/_static/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    33509 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/_static/ccp4console.gif
+-rw-rw-r--   0 martin    (1000) martin    (1000)    38533 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/_static/example_CCfree.png
+-rw-rw-r--   0 martin    (1000) martin    (1000)    20366 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/_static/example_R-values.png
+-rw-rw-r--   0 martin    (1000) martin    (1000)    38663 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/_static/phenix_command_prompt.gif
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5485 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/conf.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1007 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/credits.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1477 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/gui.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2985 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/index.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9321 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/installation.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1220 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/list_of_functions.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)      810 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/make.bat
+-rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      612 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/test.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17145 2023-02-28 22:40:52.000000 pairef-1.4.0/docs/using.rst
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       98 2024-04-17 08:41:36.000000 pairef-1.4.0/pairef/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       63 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/__main__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7014 2024-01-12 14:26:34.000000 pairef-1.4.0/pairef/commons.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    48547 2024-04-09 16:45:52.000000 pairef-1.4.0/pairef/graphs.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    31162 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/gui.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    51168 2024-04-17 08:32:56.000000 pairef-1.4.0/pairef/launcher.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    57392 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/preparation.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    57734 2024-04-17 09:31:17.000000 pairef-1.4.0/pairef/refinement.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      183 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/settings.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef/static/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12430 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/static/pairef_logo_64.png
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2327 2023-02-28 22:40:52.000000 pairef-1.4.0/pairef/static/styles.css
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4221 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1341 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       83 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-03-21 14:16:12.000000 pairef-1.4.0/pairef.egg-info/not-zip-safe
+-rw-rw-r--   0 martin    (1000) martin    (1000)       17 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-04-17 10:13:23.000000 pairef-1.4.0/pairef.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       63 2024-04-17 10:13:23.000000 pairef-1.4.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1762 2023-02-28 22:40:52.000000 pairef-1.4.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/test/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-17 10:13:23.000000 pairef-1.4.0/test/fixtures/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      595 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/A_R-values.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1305 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/NK_R00_1-50A.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1218 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/NK_R00_1-60A.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1131 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/NK_R00_1-70A.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1044 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/NK_R00_1-80A.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)      199 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/NK_Rgap.csv
+-rw-rw-r--   0 martin    (1000) martin    (1000)    68380 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/lysozyme_1-40A.log
+-rw-rw-r--   0 martin    (1000) martin    (1000)   152901 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/mdm2_1-60A.pdb
+-rw-rw-r--   0 martin    (1000) martin    (1000)  1432288 2023-02-28 22:40:52.000000 pairef-1.4.0/test/fixtures/mdm2_merged.mtz
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1801 2024-01-12 14:50:35.000000 pairef-1.4.0/test/helper.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2201 2024-03-27 11:32:06.000000 pairef-1.4.0/test/helper.pyc
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3428 2023-03-21 13:02:34.000000 pairef-1.4.0/test/log.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5934 2023-02-28 22:40:52.000000 pairef-1.4.0/test/test_commons.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4245 2023-02-28 22:40:52.000000 pairef-1.4.0/test/test_graphs.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8366 2024-04-08 19:53:55.000000 pairef-1.4.0/test/test_initial.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12041 2024-04-12 15:49:36.000000 pairef-1.4.0/test/test_integration_long.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11453 2024-03-27 13:11:37.000000 pairef-1.4.0/test/test_integration_quick.py
```

### Comparing `pairef-1.3.9/README_images/example_head.gif` & `pairef-1.4.0/README_images/example_head.gif`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/README_images/example_gui.gif` & `pairef-1.4.0/README_images/example_gui.gif`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/README_images/example_free_work.gif` & `pairef-1.4.0/README_images/example_free_work.gif`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/setup.py` & `pairef-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/test_initial.py` & `pairef-1.4.0/test/test_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 def test_file_not_exists(tmp_environ):
     cp = run("--HKLIN " + str(config("foo.mtz")) + ""
              " --XYZIN " + str(config("mdm2_1-60A.pdb")) + ""
              " -i 2" + ""
              " -r " + RES_SHELLS_GOOD + ""
              " -p file_not_exists")
-    assert cp.returncode != 0
+    if sys.platform != 'win32':
+        assert cp.returncode != 0
     # assert not cp.stdout
     # assert cp.stderr == help + "\ncctbx.python -m pairef: error: " \
     #     "The file " + str(config("foo.mtz")) + " does not exist!\n"
     assert cp.stderr == "error: " \
         "The file " + str(config("foo.mtz")) + " does not exist!\n"
 
 
@@ -105,15 +106,16 @@
         shutil.rmtree("pairef_bad_res_shells_setting")
     cp = run("--HKLIN " + str(config("mdm2_merged.mtz")) + ""
              " --XYZIN " + str(config("mdm2_1-60A.pdb")) + ""
              " -i " + res_init + ""
              " -r " + res_shells + ""
              " -p bad_res_shells_setting" + ""
              " -t")
-    assert cp.returncode != 0
+    if sys.platform != 'win32':
+        assert cp.returncode != 0
     # assert not cp.stdout
     assert cp.stderr == error_message
 
 
 def test_valid_args(tmp_environ):
     if os.path.isdir("pairef_valid_args"):
         # Preparation - clean rests from previously examined test that
@@ -189,11 +191,11 @@
     create_workdir("create_workdir")
     assert os.path.isdir("pairef_create_workdir_new")
     os.rmdir("pairef_create_workdir")
     os.rmdir("pairef_create_workdir_new")
 
 
 def test_which():
-    result = bool(which("python") or which("python3"))
+    result = bool(which("python") or which("python3") or which("ccp4-python") or which("cctbx.python"))
     assert result
     result = which("ThisCommandShouldNotExist")
     assert not result
```

### Comparing `pairef-1.3.9/test/fixtures/NK_R00_1-80A.csv` & `pairef-1.4.0/test/fixtures/NK_R00_1-80A.csv`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/NK_R00_1-70A.csv` & `pairef-1.4.0/test/fixtures/NK_R00_1-70A.csv`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/lysozyme_1-40A.log` & `pairef-1.4.0/test/fixtures/lysozyme_1-40A.log`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/A_R-values.csv` & `pairef-1.4.0/test/fixtures/A_R-values.csv`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/NK_R00_1-50A.csv` & `pairef-1.4.0/test/fixtures/NK_R00_1-50A.csv`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/mdm2_merged.mtz` & `pairef-1.4.0/test/fixtures/mdm2_merged.mtz`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/NK_R00_1-60A.csv` & `pairef-1.4.0/test/fixtures/NK_R00_1-60A.csv`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/fixtures/mdm2_1-60A.pdb` & `pairef-1.4.0/test/fixtures/mdm2_1-60A.pdb`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/test_integration_quick.py` & `pairef-1.4.0/test/test_integration_quick.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         # hklin_unmerged = os.path.join(os.environ.get("CCP4"), "lib",
         #     python_path, "site-packages/ccp4i2/demo_data/mdm2/mdm2_unmerged.mtz")
     elif platform.python_version_tuple()[0] == "2":  # CCP4 7
         hklin_unmerged = os.path.join(os.environ.get("CCP4"),
             "share/ccp4i2/demo_data/mdm2/mdm2_unmerged.mtz")
 
 dir_project = "pairef_test_quick_mdm2"
-if which("refmac5") and os.path.isfile(hklin_unmerged):
+if (which("refmac5") or which("refmacat")) and os.path.isfile(hklin_unmerged):
     def test_integration_quick_mdm2(tmp_environ):
         print("\nPerforming a quick integration test using mdm2 demo data"
               ", please wait...\n")
         if os.path.isdir(dir_project):
             # Preparation - clean rests from previously examined test that
             # has been interrupted
             shutil.rmtree(dir_project)
@@ -78,23 +78,23 @@
         expected_stdout_3 = """Refinement using REFMAC5:
 
    * Calculating initial statistics at 1.60 A resolution...
        Collecting statistics from logfiles...
 
    * Refining using data up to 1.55 A resolution...
        Running command:
-       refmac5 HKLIN mdm2_merged.mtz XYZIN test_quick_mdm2_R00_1-60A.pdb HKLOUT test_quick_mdm2_R00_1-55A.mtz XYZOUT test_quick_mdm2_R00_1-55A.pdb LIBOUT test_quick_mdm2_R00_1-55A.cif
+       refmacat HKLIN mdm2_merged.mtz XYZIN test_quick_mdm2_R00_1-60A.pdb HKLOUT test_quick_mdm2_R00_1-55A.mtz XYZOUT test_quick_mdm2_R00_1-55A.pdb LIBOUT test_quick_mdm2_R00_1-55A.cif
        Calculating statistics of the refined structure model... . . .
        Collecting statistics from logfiles...
        Updating graphs...
        Preliminary suggested cutoff: 1.XX A
 
    * Refining using data up to 1.50 A resolution...
        Running command:
-       refmac5 HKLIN mdm2_merged.mtz XYZIN test_quick_mdm2_R00_1-55A.pdb HKLOUT test_quick_mdm2_R00_1-50A.mtz XYZOUT test_quick_mdm2_R00_1-50A.pdb LIBOUT test_quick_mdm2_R00_1-50A.cif
+       refmacat HKLIN mdm2_merged.mtz XYZIN test_quick_mdm2_R00_1-55A.pdb HKLOUT test_quick_mdm2_R00_1-50A.mtz XYZOUT test_quick_mdm2_R00_1-50A.pdb LIBOUT test_quick_mdm2_R00_1-50A.cif
        Calculating statistics of the refined structure model... . . . .
        Collecting statistics from logfiles...
        Updating graphs...
        Preliminary suggested cutoff: 1.XX A
 
      * Calculating merging statistics... . . . . . . . .
        Using labels=I,SIGI
@@ -231,17 +231,18 @@
         assert "Calculations are still in progress" not in htmlfile_content
         assert "</html>" in htmlfile_content
 
         # Clean up
         os.chdir("..")
         shutil.rmtree(dir_project)
         
-elif not which("refmac5"):
+elif not (which("refmac5") or which("refmacat")):
     warnings.warn(UserWarning("Integration test could not be performed.\n"
-                              "refmac5: Command not found."))
+                              "refmac5: Command not found.\n"
+                              "refmacat: Command not found."))
 else:
     warnings.warn(UserWarning(
         "Integration test could not be performed.\n"
         "Unmerged demo data ccp4i2/demo_data/mdm2_unmerged.mtz "
         "could not be found.\n"
         "For this test, the CCP4 Suite must be installed and the relating "
         "paths must be set correctly."))
```

### Comparing `pairef-1.3.9/test/test_integration_long.py` & `pairef-1.4.0/test/test_integration_long.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 # mdm2 - normal run using refmac, quite fast calculation
 # CDO - normal run using refmac
 # POLI - run using refmac with --TLSIN and --weight
 # BO - run using refmac with --libin and --comfile
 # TL - run with free flag No.2 with input mmcif - refmac
 #                                               - phenix.refine
 # hse11 - normal run using phenix.refine, quite fast calculation, low resolution ~2.9 A
+# 8OLA_five_letter - run using refmac --libin five-letter-code restraint --prerefinement-ncyc 10
 
 
 if which("refmac5"):
     @pytest.mark.parametrize(  # res_i requires two decimals, others requires refin. programe to be specified
     "project, files, res_i, res_r, others",
     [("mdm2_0-10A", {"xyzin": "mdm2_1-60A.pdb", "hklin_unmerged": "mdm2_unmerged.mtz", "hklin": "mdm2_merged.mtz"}, "1.60", "1.5,1.4,1.3", "--refmac"),
      ("CDO_0-10A", {"xyzin": "CDO_2B5H_edit_refmac1.pdb", "hklin": "CDO_R.mtz", "hklin_unmerged": "CDO_XDS_ASCII.HKL"}, "2.00", "1.9,1.8,1.7,1.6,1.5,1.42", "--refmac"),
      ("POLI_TLS", {"xyzin": "poli67_edit12_refmac1.pdb", "hklin": "poli67_R.mtz", "hklin_unmerged": "poli67_XDS_ASCII.HKL", "tlsin": "poli67_edit12_refmac1_TLS+Biso.tlsin"}, "2.30", "2.2,2.1,2.0,1.9", "--refmac --weight 0.06 --tlsin poli67_edit12_refmac1_TLS+Biso.tlsin --TLS-ncyc 5"),
      ("BO_LIB", {"xyzin": "BO_edit94_refmac1.pdb", "hklin": "BO_R.mtz", "hklin_unmerged": "BO_XDS_ASCII.HKL", "libin": "BO_TRP-HIS_FC6.cif", "comin": "BO_setting.com"}, "2.59", "2.50", "--refmac --libin BO_TRP-HIS_FC6.cif --comfile BO_setting.com"),
      ("TL_cif_refmac", {"xyzin": "TL_3n21_edit05_refmac1_shaken.mmcif", "hklin": "TL_AUTOMATIC_DEFAULT_free_R.mtz"}, "1.80", "1.70,1.60,1.50", "--refmac --flag 2"),
      ("TL_cif_phenix", {"xyzin": "TL_3n21_edit05_refmac1_shaken.cif", "hklin": "TL_AUTOMATIC_DEFAULT_free_R.mtz", "defin": "TL_setting.def"}, "1.80", "1.70,1.60,1.50", "--phenix --flag 2 --def TL_setting.def"),
-     ("hse11", {"xyzin": "hse11_2-90A.pdb", "hklin": "hse11_2-45A.mtz", "hklin_unmerged": "hse11_XDS_ASCII.HKL"}, "2.90", "2.70,2.45", "--phenix")],
-     ids=["mdm2_0-10A", "CDO_0-10A", "POLI_TLS", "BO_LIB", "TL_cif_refmac", "TL_cif_phenix", "hse11"])
+     ("hse11", {"xyzin": "hse11_2-90A.pdb", "hklin": "hse11_2-45A.mtz", "hklin_unmerged": "hse11_XDS_ASCII.HKL"}, "2.90", "2.70,2.45", "--phenix"),
+     ("8OLA_five_letter", {"xyzin": "8OLA_ADP15.mmcif", "hklin": "8OLA-sf.mtz", "libin": "8OLA_A1H69.cif", "hklin_unmerged": None}, "1.60", "1.40", "--libin 8OLA_A1H69.cif --prerefinement-ncyc 10 --refmac")],
+     ids=["mdm2_0-10A", "CDO_0-10A", "POLI_TLS", "BO_LIB", "TL_cif_refmac", "TL_cif_phenix", "hse11", "8OLA_five_letter"])
     def test_integration(project, files, res_i, res_r, others, tmp_environ):
         if "--phenix" in others and not which("phenix.refine"):
             warnings.warn(UserWarning("phenix.refine was not found in executables.\n"))
             pytest.skip("Skipping tests for phenix.refine.")
         print("\nPerforming integration tests, please wait...\n")
         dir_project = "pairef_" + project
         if os.path.isdir(dir_project):
@@ -46,42 +48,43 @@
             urllib_wget = urllib.request.urlretrieve
         except ImportError:  # Python 2
             import urllib
             urllib_wget = urllib.urlretrieve
 
         url_prefix = "https://raw.githubusercontent.com/MartinMalyMM/pairef_test_data/main/"
         for f in files.values():
-            filename, log = urllib_wget(url_prefix + f, f)
-            # try:
-            #    filename, log = urllib_wget(url_prefix + f, f)
-            #except urllib.error.HTTPError:        # Python 3
-            #    filename, log = urllib_wget(url_prefix_alt + f, f)
-            ## print(url_prefix + f)
-            ## print(bool("Content-Length: 14" in str(log)))
-            ## print(str(log))
-            #if "Content-Length: 14" in str(log):  # Python 2
-            #    print(url_prefix + f + " not found")
-            #    print("trying alt")
-            #    filename, log = urllib_wget(url_prefix_alt + f, f)
-            assert os.path.isfile(f)
+            if f:
+                filename, log = urllib_wget(url_prefix + f, f)
+                # try:
+                #    filename, log = urllib_wget(url_prefix + f, f)
+                #except urllib.error.HTTPError:        # Python 3
+                #    filename, log = urllib_wget(url_prefix_alt + f, f)
+                ## print(url_prefix + f)
+                ## print(bool("Content-Length: 14" in str(log)))
+                ## print(str(log))
+                #if "Content-Length: 14" in str(log):  # Python 2
+                #    print(url_prefix + f + " not found")
+                #    print("trying alt")
+                #    filename, log = urllib_wget(url_prefix_alt + f, f)
+                assert os.path.isfile(f)
         if "TL_cif" in project:
             filename, log = urllib_wget(
                 "https://pairef.fjfi.cvut.cz/docs/publication_examples/3-2_TL/pairef_TL_step0-10A/"
                 "AUTOMATIC_DEFAULT_scaled_unmerged.mtz",
                 "TL_AUTOMATIC_DEFAULT_scaled_unmerged.mtz")
             files["hklin_unmerged"] = "TL_AUTOMATIC_DEFAULT_scaled_unmerged.mtz"
             assert os.path.isfile("TL_AUTOMATIC_DEFAULT_scaled_unmerged.mtz")
         xyzin = files["xyzin"]
         hklin = files["hklin"]
         hklin_unmerged = files["hklin_unmerged"]
 
         arguments = "--HKLIN " + hklin + \
-            " --XYZIN " + xyzin + \
-            " -u " + hklin_unmerged + \
-            " -i " + res_i + \
+            " --XYZIN " + xyzin
+        if hklin_unmerged: arguments += " -u " + hklin_unmerged
+        arguments += " -i " + res_i + \
             " -r " + res_r + \
             " -p " + project + \
             " " + others
         cp = run(arguments)
         assert cp.returncode == 0
         # assert not cp.stderr
         if cp.stderr:
@@ -106,21 +109,24 @@
 """
         if "--phenix" in others:
             expected_stdout += " * Refinement software: phenix.refine\n"
         elif "--refmac" in others:
             expected_stdout += " * Refinement software: REFMAC5\n"
         expected_stdout += " * XYZIN: " + xyzin + "\n"
         expected_stdout += " * HKLIN: " + hklin + "\n"
-        expected_stdout += " * HKLIN unmerged: " + hklin_unmerged + "\n"
+        if hklin_unmerged:
+            expected_stdout += " * HKLIN unmerged: " + hklin_unmerged + "\n"
         if "--libin" in others:
             expected_stdout += " * LIBIN: " + files["libin"] + "\n"
         if "--tlsin" in others:
             expected_stdout += " * TLSIN: " + files["tlsin"] + "\n"
         expected_stdout += " * Project name: " + project + "\n"
         expected_stdout += " * Resolution shells: " + res_r + "\n"
+        if "--prerefinement-ncyc 10" in others:
+            expected_stdout += " * Number of pre-refinement cycles that will be performed before the paired refinement protocol: 10\n"
         if "--comfile" in others:
             expected_stdout += " * Com file for REFMAC5: " + files["comin"] + "\n"
         if "--def" in others:
             expected_stdout += " * Keyword file for phenix.refine: " + files["defin"] + "\n"
         if "--weight" in others:
             expected_stdout += " * Weight matrix: 0.06\n"  # POLI
         if "--TLS-ncyc" in others:                         # POLI
@@ -160,38 +166,40 @@
                 calculation_ended = True
         assert calculation_ended
 
         res_i_name = res_i.replace(".", "-")
         files_out = \
             [xyzin,
              hklin,
-             hklin_unmerged,
              "PAIREF_cutoff.txt",
              "PAIREF_out.log",
              "PAIREF_" + project + ".html",
              "styles.css",
              project + "_CCfree.png",
-             project + "_CC.png",
              project + "_CCwork.png",
-             project + "_Comp_Mult.png",
-             project + "_Intensities.png",
-             project + "_merging_stats.csv",
-             project + "_No_reflections.png",
              project + "_No_work_free_reflections.png",
              project + "_Optical_resolution.csv",
              project + "_Optical_resolution.png",
              project + "_R" + flag + "_Rgap.csv",
              project + "_R" + flag + "_R-values.csv",
              project + "_Rfree.png",
              project + "_Rgap.csv",
              project + "_Rgap.png",
-             project + "_Rmerge_Rmeas_Rpim.png",
              project + "_R-values.csv",
              project + "_R-values.png",
              project + "_Rwork.png"]
+        if hklin_unmerged:
+            files_out += \
+                [hklin_unmerged,
+                 project + "_merging_stats.csv",
+                 project + "_CC.png",
+                 project + "_Comp_Mult.png",
+                 project + "_No_reflections.png",
+                 project + "_Intensities.png",
+                 project + "_Rmerge_Rmeas_Rpim.png"]
         if "--refmac" in others:
             files_out += \
                 [project + "_R" + flag + "_" + res_i_name + "A_comparison_at_" + res_i_name + "A.log",
                  project + "_R" + flag + "_" + res_i_name + "A_comparison_at_" + res_i_name + "A.mtz",
                  project + "_R" + flag + "_" + res_i_name + "A.csv",
                  project + "_R" + flag + "_" + res_i_name + "A.log",
                  project + "_R" + flag + "_" + res_i_name + "A.mmcif",
@@ -220,14 +228,15 @@
             htmlfile_content = htmlfile.read()
         assert "Calculations are still in progress" not in htmlfile_content
         assert "</html>" in htmlfile_content
 
         # Clean up a bit
         os.chdir("..")
         for f in files.values():
-            if os.path.isfile(f):
-                os.remove(f)
+            if f:
+                if os.path.isfile(f):
+                    os.remove(f)
         # shutil.rmtree(dir_project)
 
 else:
     warnings.warn(UserWarning("Integration test could not be performed.\n"
                               "refmac5: Command not found."))
```

### Comparing `pairef-1.3.9/test/test_graphs.py` & `pairef-1.4.0/test/test_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     args.no_modification = None
     args.prerefinement_ncyc = None
     args.reset_bfactor = None
     args.add_to_bfactor = None
     args.set_bfactor = None
     args.shake_sites = None
     args.constant_grid = None
+    args.ccp4cloud = None
     shutil.copy2(config("A_R-values.csv"), tempfile.gettempdir())
     shells_ready_with_res_init = (1.8, 1.7, 1.6)
     shells = (1.8, 1.7, 1.6, 1.5)
     flag_sets = range(20)
     htmlfilename_in_progress = write_log_html(
         shells, shells_ready_with_res_init, args, versions_dict, flag_sets)
     assert os.path.isfile(htmlfilename_in_progress)
```

### Comparing `pairef-1.3.9/test/test_commons.py` & `pairef-1.4.0/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/test/helper.py` & `pairef-1.4.0/test/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     #     pass
     if sys.platform == 'win32':
         posix_bool = False
         shell_bool = True
     else:
         posix_bool = True
         shell_bool = False
-    print('\n$ cctbx.python -m pairef', line)
+    print('\n$ ccp4-python -m pairef', line)
     # print('\n$ python -m', MODULE, line)
-    command = ["cctbx.python", '-m', "pairef"] + shlex.split(line, posix=posix_bool)
+    command = ["ccp4-python", '-m', "pairef"] + shlex.split(line, posix=posix_bool)
     # return subprocess.run(command,
     process = subprocess.Popen(command,
                                stdout=subprocess.PIPE,
                                stderr=subprocess.PIPE,
                                universal_newlines=True,
                                shell=shell_bool,
                                **kwargs)
```

### Comparing `pairef-1.3.9/pairef.egg-info/SOURCES.txt` & `pairef-1.4.0/pairef.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 pairef.egg-info/entry_points.txt
 pairef.egg-info/not-zip-safe
 pairef.egg-info/requires.txt
 pairef.egg-info/top_level.txt
 pairef/static/pairef_logo_64.png
 pairef/static/styles.css
 test/helper.py
+test/helper.pyc
+test/log.txt
 test/test_commons.py
 test/test_graphs.py
 test/test_initial.py
 test/test_integration_long.py
 test/test_integration_quick.py
 test/fixtures/A_R-values.csv
 test/fixtures/NK_R00_1-50A.csv
```

### Comparing `pairef-1.3.9/pairef.egg-info/PKG-INFO` & `pairef-1.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pairef
-Version: 1.3.9
+Version: 1.4.0
 Summary: Automatic PAIRed REFinement protocol
 Home-page: https://pairef.fjfi.cvut.cz/
 Author: Martin Maly
 Author-email: martin.maly@fjfi.cvut.cz
 License: GNU Lesser General Public License v3 (LGPLv3)
-Description: *PAIREF*
-        ========
-        
-        *Automatic PAIRed REFinement protocol*
-        
-        *PAIREF* is a tool for macromolecular crystallographers that performs the *PAIRed REFinement protocol* [1]_ automatically to estimate the optimal high-resolution cutoff. It is developed in Python and can be installed as a module into the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_. It provides graphical and command-line interface that executes all the needed calculations. Parameters of refinement can be specified in detail to put all the calculations under full control of the user. Obtained results are presented as plots and tables in HTML log file. *PAIREF* supports `REFMAC5 <http://www.ccp4.ac.uk/html/refmac5.html>`_ (part of the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_) and `phenix.refine <https://www.phenix-online.org/documentation/reference/refinement.html>`_ (part of the `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_) for structure model refinement.
-        
-        .. image:: README_images/example_gui.gif
-        
-        .. image:: README_images/example_head.gif
-        
-        .. image:: README_images/example_free_work.gif
-        
-        .. [1] `P.A. Karplus, K. Diederichs: "Linking crystallographic model and data quality." (2012) Science, 336(6084):1030-3. <https://science.sciencemag.org/content/336/6084/1030>`_
-        
-        Installation and system requirements
-        ------------------------------------
-        
-        *PAIREF* depends on the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_ or `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_. Both contain the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_ with Python and `pip <https://pip.pypa.io/en/stable/>`_). *PAIREF* works with both Python 2 and Python 3.
-        
-        *PAIREF* can be easily installed running command :code:`cctbx.python -m pip install pairef --user --no-deps` in terminal (GNU/Linux, macOS) or CCP4Console (Windows). More information are available in `documentation <https://pairef.fjfi.cvut.cz/docs/installation.html>`_. Check also the *PAIREF* homepage at `<https://pairef.fjfi.cvut.cz/>`_ and `PyPI repository <https://pypi.org/project/pairef/>`_.
-        
-        Example
-        -------
-        
-        To run paired refinement of a model (previously refined at 1.81 Å) for a series of cutoffs (1.7, 1.6, and 1.5 Å), execute a following command:
-        
-        .. code ::
-        
-           cctbx.python -m pairef --XYZIN model_1-81A.pdb --HKLIN data_1-5A.mtz --HKLIN_UNMERGED data_1-5A_unmerged.mtz -i 1.81 -r 1.7,1.6,1.5
-        
-        For detailed information about other program parameters, read the documentation available at `<http://pairef.fjfi.cvut.cz/docs>`_.
-        
-        Credits and contact
-        -------------------
-        
-        Please refer: M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko: `Paired refinement under the control of PAIREF <https://journals.iucr.org/m/issues/2020/04/00/mf5044/index.html>`_ (2020) *IUCrJ* **7**
-        
-        *PAIREF* is developed by Martin Malý in collaboration of Czech Technical University, Czech Academy of Sciences, and University of Konstanz. In case of any questions or problems, please do not hesitate and write us: `martin.maly@fjfi.cvut.cz <mailto:martin.maly@fjfi.cvut.cz>`_.
-        
 Keywords: macromolecular crystallography,research
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
@@ -59,7 +19,50 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+*PAIREF*
+========
+
+*Automatic PAIRed REFinement protocol*
+
+*PAIREF* is a tool for macromolecular crystallographers that performs the *PAIRed REFinement protocol* [1]_ automatically to estimate the optimal high-resolution cutoff. It is developed in Python and can be installed as a module into the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_. It provides graphical and command-line interface that executes all the needed calculations. Parameters of refinement can be specified in detail to put all the calculations under full control of the user. Obtained results are presented as plots and tables in HTML log file. *PAIREF* supports `REFMAC5 <http://www.ccp4.ac.uk/html/refmac5.html>`_ (part of the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_) and `phenix.refine <https://www.phenix-online.org/documentation/reference/refinement.html>`_ (part of the `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_) for structure model refinement.
+
+.. image:: README_images/example_gui.gif
+
+.. image:: README_images/example_head.gif
+
+.. image:: README_images/example_free_work.gif
+
+.. [1] `P.A. Karplus, K. Diederichs: "Linking crystallographic model and data quality." (2012) Science, 336(6084):1030-3. <https://science.sciencemag.org/content/336/6084/1030>`_
+
+Installation and system requirements
+------------------------------------
+
+*PAIREF* depends on the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_ or `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_. Both contain the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_ with Python and `pip <https://pip.pypa.io/en/stable/>`_). *PAIREF* works with both Python 2 and Python 3.
+
+*PAIREF* can be easily installed running command :code:`cctbx.python -m pip install pairef --user --no-deps` in terminal (GNU/Linux, macOS) or CCP4Console (Windows). More information are available in `documentation <https://pairef.fjfi.cvut.cz/docs/installation.html>`_. Check also the *PAIREF* homepage at `<https://pairef.fjfi.cvut.cz/>`_ and `PyPI repository <https://pypi.org/project/pairef/>`_.
+
+Example
+-------
+
+To run paired refinement of a model (previously refined at 1.81 Å) for a series of cutoffs (1.7, 1.6, and 1.5 Å), execute a following command:
+
+.. code ::
+
+   cctbx.python -m pairef --XYZIN model_1-81A.pdb --HKLIN data_1-5A.mtz --HKLIN_UNMERGED data_1-5A_unmerged.mtz -i 1.81 -r 1.7,1.6,1.5
+
+For detailed information about other program parameters, read the documentation available at `<http://pairef.fjfi.cvut.cz/docs>`_.
+
+Credits and contact
+-------------------
+
+Please refer: M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko: `Paired refinement under the control of PAIREF <https://journals.iucr.org/m/issues/2020/04/00/mf5044/index.html>`_ (2020) *IUCrJ* **7**
+
+*PAIREF* is developed by Martin Malý in collaboration of Czech Technical University, Czech Academy of Sciences, and University of Konstanz. In case of any questions or problems, please do not hesitate and write us: `martin.maly@fjfi.cvut.cz <mailto:martin.maly@fjfi.cvut.cz>`_.
+
+
```

### Comparing `pairef-1.3.9/PKG-INFO` & `pairef-1.4.0/pairef.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pairef
-Version: 1.3.9
+Version: 1.4.0
 Summary: Automatic PAIRed REFinement protocol
 Home-page: https://pairef.fjfi.cvut.cz/
 Author: Martin Maly
 Author-email: martin.maly@fjfi.cvut.cz
 License: GNU Lesser General Public License v3 (LGPLv3)
-Description: *PAIREF*
-        ========
-        
-        *Automatic PAIRed REFinement protocol*
-        
-        *PAIREF* is a tool for macromolecular crystallographers that performs the *PAIRed REFinement protocol* [1]_ automatically to estimate the optimal high-resolution cutoff. It is developed in Python and can be installed as a module into the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_. It provides graphical and command-line interface that executes all the needed calculations. Parameters of refinement can be specified in detail to put all the calculations under full control of the user. Obtained results are presented as plots and tables in HTML log file. *PAIREF* supports `REFMAC5 <http://www.ccp4.ac.uk/html/refmac5.html>`_ (part of the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_) and `phenix.refine <https://www.phenix-online.org/documentation/reference/refinement.html>`_ (part of the `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_) for structure model refinement.
-        
-        .. image:: README_images/example_gui.gif
-        
-        .. image:: README_images/example_head.gif
-        
-        .. image:: README_images/example_free_work.gif
-        
-        .. [1] `P.A. Karplus, K. Diederichs: "Linking crystallographic model and data quality." (2012) Science, 336(6084):1030-3. <https://science.sciencemag.org/content/336/6084/1030>`_
-        
-        Installation and system requirements
-        ------------------------------------
-        
-        *PAIREF* depends on the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_ or `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_. Both contain the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_ with Python and `pip <https://pip.pypa.io/en/stable/>`_). *PAIREF* works with both Python 2 and Python 3.
-        
-        *PAIREF* can be easily installed running command :code:`cctbx.python -m pip install pairef --user --no-deps` in terminal (GNU/Linux, macOS) or CCP4Console (Windows). More information are available in `documentation <https://pairef.fjfi.cvut.cz/docs/installation.html>`_. Check also the *PAIREF* homepage at `<https://pairef.fjfi.cvut.cz/>`_ and `PyPI repository <https://pypi.org/project/pairef/>`_.
-        
-        Example
-        -------
-        
-        To run paired refinement of a model (previously refined at 1.81 Å) for a series of cutoffs (1.7, 1.6, and 1.5 Å), execute a following command:
-        
-        .. code ::
-        
-           cctbx.python -m pairef --XYZIN model_1-81A.pdb --HKLIN data_1-5A.mtz --HKLIN_UNMERGED data_1-5A_unmerged.mtz -i 1.81 -r 1.7,1.6,1.5
-        
-        For detailed information about other program parameters, read the documentation available at `<http://pairef.fjfi.cvut.cz/docs>`_.
-        
-        Credits and contact
-        -------------------
-        
-        Please refer: M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko: `Paired refinement under the control of PAIREF <https://journals.iucr.org/m/issues/2020/04/00/mf5044/index.html>`_ (2020) *IUCrJ* **7**
-        
-        *PAIREF* is developed by Martin Malý in collaboration of Czech Technical University, Czech Academy of Sciences, and University of Konstanz. In case of any questions or problems, please do not hesitate and write us: `martin.maly@fjfi.cvut.cz <mailto:martin.maly@fjfi.cvut.cz>`_.
-        
 Keywords: macromolecular crystallography,research
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
@@ -59,7 +19,50 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+*PAIREF*
+========
+
+*Automatic PAIRed REFinement protocol*
+
+*PAIREF* is a tool for macromolecular crystallographers that performs the *PAIRed REFinement protocol* [1]_ automatically to estimate the optimal high-resolution cutoff. It is developed in Python and can be installed as a module into the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_. It provides graphical and command-line interface that executes all the needed calculations. Parameters of refinement can be specified in detail to put all the calculations under full control of the user. Obtained results are presented as plots and tables in HTML log file. *PAIREF* supports `REFMAC5 <http://www.ccp4.ac.uk/html/refmac5.html>`_ (part of the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_) and `phenix.refine <https://www.phenix-online.org/documentation/reference/refinement.html>`_ (part of the `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_) for structure model refinement.
+
+.. image:: README_images/example_gui.gif
+
+.. image:: README_images/example_head.gif
+
+.. image:: README_images/example_free_work.gif
+
+.. [1] `P.A. Karplus, K. Diederichs: "Linking crystallographic model and data quality." (2012) Science, 336(6084):1030-3. <https://science.sciencemag.org/content/336/6084/1030>`_
+
+Installation and system requirements
+------------------------------------
+
+*PAIREF* depends on the `CCP4 Software Suite <http://www.ccp4.ac.uk/>`_ or `PHENIX <https://www.phenix-online.org/documentation/reference/refinement.html>`_. Both contain the `Computational Crystallography Toolbox <https://cci.lbl.gov/cctbx_docs/index.html>`_ with Python and `pip <https://pip.pypa.io/en/stable/>`_). *PAIREF* works with both Python 2 and Python 3.
+
+*PAIREF* can be easily installed running command :code:`cctbx.python -m pip install pairef --user --no-deps` in terminal (GNU/Linux, macOS) or CCP4Console (Windows). More information are available in `documentation <https://pairef.fjfi.cvut.cz/docs/installation.html>`_. Check also the *PAIREF* homepage at `<https://pairef.fjfi.cvut.cz/>`_ and `PyPI repository <https://pypi.org/project/pairef/>`_.
+
+Example
+-------
+
+To run paired refinement of a model (previously refined at 1.81 Å) for a series of cutoffs (1.7, 1.6, and 1.5 Å), execute a following command:
+
+.. code ::
+
+   cctbx.python -m pairef --XYZIN model_1-81A.pdb --HKLIN data_1-5A.mtz --HKLIN_UNMERGED data_1-5A_unmerged.mtz -i 1.81 -r 1.7,1.6,1.5
+
+For detailed information about other program parameters, read the documentation available at `<http://pairef.fjfi.cvut.cz/docs>`_.
+
+Credits and contact
+-------------------
+
+Please refer: M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko: `Paired refinement under the control of PAIREF <https://journals.iucr.org/m/issues/2020/04/00/mf5044/index.html>`_ (2020) *IUCrJ* **7**
+
+*PAIREF* is developed by Martin Malý in collaboration of Czech Technical University, Czech Academy of Sciences, and University of Konstanz. In case of any questions or problems, please do not hesitate and write us: `martin.maly@fjfi.cvut.cz <mailto:martin.maly@fjfi.cvut.cz>`_.
+
+
```

### Comparing `pairef-1.3.9/README.rst` & `pairef-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/pairef/static/pairef_logo_64.png` & `pairef-1.4.0/pairef/static/pairef_logo_64.png`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/pairef/static/styles.css` & `pairef-1.4.0/pairef/static/styles.css`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/pairef/commons.py` & `pairef-1.4.0/pairef/commons.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,16 +203,16 @@
         values_free_list.append(float(line.split()[6]))
     except ValueError:
         values_free_list.append(None)
     if errors:  # return also standard error of mean
         try:
             errors_work_list.append(float(line.split()[9]))
         except ValueError:
-            errors_work_list.append(float('nan'))            
+            errors_work_list.append(0)            
         try:
             errors_free_list.append(float(line.split()[10]))
         except ValueError:
-            errors_free_list.append(float('nan'))
+            errors_free_list.append(0)
     else:
-        errors_work_list.append(float('nan'))
-        errors_free_list.append(float('nan'))
+        errors_work_list.append(0)
+        errors_free_list.append(0)
     return values_work_list, values_free_list, errors_work_list, errors_free_list, continue_sign
```

### Comparing `pairef-1.3.9/pairef/graphs.py` & `pairef-1.4.0/pairef/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         depth (int)
 
     Returns:
         list: containing labels for a graph - compressed
     """
     if len(list) > 88:
         return list  # long lists cause problems
-    if len([label for label in list if label is not ""]) >= n_max:
+    if len([label for label in list if label != ""]) >= n_max:
         if len(list) % 2 == 0:
             i = int(pow(2, depth - 1) + 1)  # i = 2 in case of depth == 1
             list[1] = ""
         else:
             i = int(pow(2, depth - 1))  # i = 1 in case of depth == 1
         erase = True
         while i < len(list) - 1:
@@ -42,15 +42,15 @@
                 list[i] = ""
                 erase = False
             else:
                 erase = True
             i = i + 1 * depth
         list[- depth - 1] = ""
     # If it was not enough, do it again, recursively
-    if len([label for label in list if label is not ""]) >= n_max:
+    if len([label for label in list if label != ""]) >= n_max:
         list = xticklabels_compress(list=list, n_max=n_max, depth=2*depth)
     return list
 
 
 def matplotlib_bar(args, values="R-values", flag_sets=[], ready_shells=[]):
     """Plots and saves a bar chart using `matplotlib`.
 
@@ -608,14 +608,15 @@
 
     import getpass
     import socket
     import html
 
     page = """<!DOCTYPE html>
 <head>
+    <meta charset="utf-8">
     <title>PAIREF - results """ + args.project + """</title>
     <link rel="stylesheet" type="text/css" href="styles.css">\n"""
     if not done:
         page += """\t<meta http-equiv="refresh" content="15">\n"""
     page += """</head>
 <body>
     <div id="header">
@@ -647,29 +648,29 @@
         if done:
             page += "\t<h2>VERDICT - suggested cutoff: "
         else:
             page += "\t<h2>Preliminary suggested cutoff: "
         if cutoff[0] == cutoff[1]:
             page += twodec(cutoff[0])
         else:
-            page += "strict: " + twodec(cutoff[0]) + " A; benevolent: "  + twodec(cutoff[1])
-        page += " A</h2>\n"
+            page += "strict: " + twodec(cutoff[0]) + " &#8491;; benevolent: "  + twodec(cutoff[1])
+        page += " &#8491;</h2>\n"
         page += "\t\t<table class='suggestion'>\n"
         page += "\t\t<tr><th>Shell</th><th>Accepted?</th><th>Reason</th></tr>\n"
         for i, shell in enumerate(ready_shells[1:]):
             if not accepted[i][1] and not accepted[i][0]:
                 page += "\t\t<tr class='rejected'>\n"
             elif "lowNfree" + twodec(shell) in warning_dict:
                 page += "\t\t<tr class='lowNfree'>\n"
             elif accepted[i][1] and not accepted[i][0]:
                 page += "\t\t<tr class='benevolent'>\n"
             else:  # elif accepted[i][0]:
                 page += "\t\t<tr class='accepted'>\n"
             page += "\t\t\t<td>"
-            page += twodec(shells[i]) + "-" + twodec(shell) + " A</td>\n"
+            page += twodec(shells[i]) + "-" + twodec(shell) + " &#8491;</td>\n"
             page += "\t\t\t<td>"
             if accepted[i][0]:
                 page += "Yes"
             elif accepted[i][1] and not accepted[i][0]:
                 page += "Warning"
             else:
                 page += "No"
@@ -784,73 +785,92 @@
                     "mtzdump", "binning", "flags", "amb_labels"]
     page = warning_orangebox(warning_keys, page)
     if ready_shells:
         if len(ready_shells) >= 2:
             page += '\t<h2>Overall values</h2>\n'
             page = warning_orangebox(["overall_R"], page)
             page += '\t\t<div class="wrap">\n'
-            page += '\t\t\t<div class="column">\n'
-            page += '\t\t\t\t<a href="' + args.project + '_R-values.png">'
+            page += '\t\t\t<div class="column">\n\t\t\t\t'
+            if not args.ccp4cloud:
+                page += '<a href="' + args.project + '_R-values.png">'
             page += '<img src="' + args.project + '_R-values.png' \
                 '?shell=' + twodecname(ready_shells[-1]) + '" ' \
                 'alt="R-values"></a><br />\n'
+            if not args.ccp4cloud:
+                page += '</a>'
+            page += '<br />\n'
             page += '\t\t\t\tRaw data: <a href="' + args.project + '' \
                 '_R-values.csv">' + args.project + '_R-values.csv' \
                 '</a><br />\n'
             page += '\t\t\t\t<pre>\n'
             with open(args.project + "_R-values.csv", "r") as csvfile:
                 page += html.escape(csvfile.read())
             page += '</pre>'
             page += '\n\t\t\t\t<p class="note">Note: For each incremental ' \
                 'step of resolution from X->Y, the <i>R</i>-values were ' \
                 'calculated at resolution X.'
             if args.complete_cross_validation:
                 page += ' Standard error of mean is shown in orange.'
             page += '</p>\n'
             page += '\t\t\t</div>\n'
-            page += '\t\t\t<div class="column">\n'
-            page += '\t\t\t\t<a href="' + args.project + '_Rgap.png">' \
-                '<img src="' + args.project + '_Rgap.png' \
+            page += '\t\t\t<div class="column">\n\t\t\t\t'
+            if not args.ccp4cloud:
+                page += '<a href="' + args.project + '_Rgap.png">'
+            page += '<img src="' + args.project + '_Rgap.png' \
                 '?shell=' + twodecname(ready_shells[-1]) + '" ' \
-                'alt="Rgap"></a><br />\n'
+                'alt="Rgap">'
+            if not args.ccp4cloud:
+                page += '</a>'
+            page += '<br />\n'
             page += '\t\t\t\tRaw data: <a href="' \
                 '' + args.project + '_Rgap.csv">' + args.project + '' \
                 '_Rgap.csv</a>\n'
             page += '\t\t\t\t<p class="note">Note: The R-values were ' \
                 'calculated at ' + twodec(shells[0]) + ' &#8491; resolution.' \
                 '</p>\n'
             page += '\t\t\t</div>\n'
             page += '\t\t</div>\n'
 
             if args.complete_cross_validation:
-                for shell in ready_shells[1:]:  # exclude the initial difr. l.
-                    page += '\t\t<a href="' + args.project + '_R-values_com' \
-                        'plete_' + twodecname(shell) + 'A.png">' \
-                        '<img src="' + args.project + '_R-values_complete' \
+                for shell in ready_shells[1:]:  # exclude the initial diffr. l.
+                    page += '\t\t'
+                    if not args.ccp4cloud:
+                        page += '<a href="' + args.project + '_R-values_complete_' + twodecname(shell) + 'A.png">'
+                    page += '<img src="' + args.project + '_R-values_complete' \
                         '_' + twodecname(shell) + 'A.png' \
                         '?shell=' + twodecname(shell) + '' \
                         '" alt="R-values (complete cross-validation, ' \
-                        '' + twodec(shell) + ' A)"></a>\n'
+                        '' + twodec(shell) + ' A)">'
+                    if not args.ccp4cloud:
+                        page += '</a>'
+                    page += '<br />\n'
 
         # "Rfree", "CCfree", "Rwork", "CCwork", "No_work_free_refl." graphs
         if not args.complete_cross_validation:
             page += '\t<h2>Model statistics - binned values</h2>\n'
             # Show relating warnings if there are some
-            warning_keys = ["Nfree", "high_R", "low_R", "low_CC"]
+            warning_keys = ["Nfree", "high_R", "low_R", "low_CC", "noI"]
             page = warning_orangebox(warning_keys, page)
             # Show "Rfree", "CCfree", "Rwork", "CCwork" graphs
-            graphs = ["Rfree", "CCfree", "Rwork", "CCwork"]
+            if "noI" in warning_dict:
+                graphs = ["Rfree", "Rwork"]
+            else:
+                graphs = ["Rfree", "CCfree", "Rwork", "CCwork"]
             for i, graph in enumerate(graphs):
                 pngfilename = args.project + "_" + graph + ".png"
                 if os.path.isfile(pngfilename):
-                    page += '\t\t<a href="' + args.project + '_' + graph + '' \
-                        '.png">' \
-                        '<img src="' + args.project + '_' + graph + '.png' \
+                    page += '\t\t'
+                    if not args.ccp4cloud:
+                        page += '<a href="' + args.project + '_' + graph + '.png">'
+                    page += '<img src="' + args.project + '_' + graph + '.png' \
                         '?shell=' + twodecname(ready_shells[-1]) + '' \
-                        '" alt="' + graph + '"></a>\n'
+                        '" alt="' + graph + '">'
+                    if not args.ccp4cloud:
+                        page += '</a>'
+                    page += '\n'
                 if i % 2 == 1:  # Display max. 2 graphs in row
                     page += "\t\t<br />\n"
             # Link to raw data
             page += '\t\tRaw data:\n'
             page += '\t\t<ul>\n'
             for shell in ready_shells:
                 page += '\t\t\t<li><a href="' + args.project + '_' \
@@ -859,45 +879,57 @@
                     'R' + str(args.flag).zfill(2) + '_' \
                     '' + twodecname(shell) + 'A.csv</a></li>\n'
             page += '\t\t</ul>\n'
             # Show No. work free reflections graph
             graph = "No_work_free_reflections"
             pngfilename = args.project + "_" + graph + ".png"
             if os.path.isfile(pngfilename):
-                page += '\t\t<a href="' + args.project + '_' + graph + '' \
-                    '.png">' \
-                    '<img src="' + args.project + '_' + graph + '.png' \
+                page += '\t\t'
+                if not args.ccp4cloud:
+                    page += '<a href="' + args.project + '_' + graph + '.png">'
+                page += '<img src="' + args.project + '_' + graph + '.png' \
                     '?shell=' + twodecname(ready_shells[-1]) + '' \
-                    '" alt="' + graph + '"></a>\n'
+                    '" alt="' + graph + '">'
+                if not args.ccp4cloud:
+                    page += '</a>'
+                page += '\n'
 
     # Optical resolution
     pngfilename = args.project + "_Optical_resolution.png"
     csvfilename = args.project + "_Optical_resolution.csv"
     if os.path.isfile(pngfilename):
         page += "\t<h2>Optical resolution</h2>\n"
-        page += '\t\t<a href="' + pngfilename + '">' \
-            '<img src="' + pngfilename + \
+        if not args.ccp4cloud:
+            page += '\t\t<a href="' + pngfilename + '">'
+        page += '<img src="' + pngfilename + \
             '?shell=' + twodecname(ready_shells[-1]) + '" ' \
-            'alt="Optical resolution"></a><br />\n'
+            'alt="Optical resolution">'
+        if not args.ccp4cloud:
+            page += '</a>'
+        page += '<br />\n'
         page += '\t\tRaw data: <a href="' + csvfilename + '">' + \
             csvfilename + '</a>\n'
 
     csvfilename = args.project + "_merging_stats.csv"
     if args.hklin_unmerged and ready_merging_statistics \
             and os.path.isfile(csvfilename):
         graphs = ["CC", "Intensities", "Comp_Mult", "Rmerge_Rmeas_Rpim",
                   "No_reflections"]
         page += "\t<h2>Merging statistics</h2>\n"
         warning_keys = ["merging_stats", "CC*"]
         page = warning_orangebox(warning_keys, page)
         for graph in graphs:
-            page += '\t\t<a href="' + args.project + '_' + graph + '' \
-                '.png">' \
-                '<img src="' + args.project + '_' + graph + '.png" alt="' \
-                '' + graph + '"></a>\n'
+            page += '\t\t'
+            if not args.ccp4cloud:
+                page += '<a href="' + args.project + '_' + graph + '.png">'
+            page += '<img src="' + args.project + '_' + graph + '.png" alt="' \
+                '' + graph + '">'
+            if not args.ccp4cloud:
+                page += '</a>'
+            page += '\n'
         page += '\t\t<p>Raw data: <a href="' + args.project + '' \
             '_merging_stats.csv">' \
             '' + args.project + '_merging_stats.csv</a></p>\n'
         page += '\t\t<pre>\n'
         with open(args.project + "_merging_stats.csv", "r") as csvfile:
             page += html.escape(csvfile.read())
         page += '\t\t</pre>\n'
@@ -922,60 +954,70 @@
                     ciffilename = prefix + '_001.cif'
                 else:  # refmac
                     logfilename = prefix + '.log'
                     pdbfilename = prefix + '.pdb'
                     ciffilename = prefix + '.mmcif'
                 if os.path.isfile(pngfilename):
                     page += '\t\t\t<div class="column">\n'
-                    page += '\t\t\t\t<a href="' + pngfilename + '">' \
-                        '<img src="' + pngfilename + '" alt="' \
+                    page += '\t\t\t\t'
+                    if not args.ccp4cloud:
+                        page += '<a href="' + pngfilename + '">'
+                    page += '<img src="' + pngfilename + '" alt="' \
                         '' + twodec(shell) + 'A statistics vs. cycle, ' \
-                        'flag ' + str(flag).zfill(2) + '"></a><br />\n'
+                        'flag ' + str(flag).zfill(2) + '">'
+                    if not args.ccp4cloud:
+                        page += '</a>'
+                    page += '<br />\n'
                     page += '\t\t\t\t<a href="' + logfilename + '">' \
                         'Log file</a> from refinement at ' \
                         '' + twodec(shell) + ' &#8491;<br />\n'
                     page += '\t\t\t\t' \
                         'Structure model refined at ' + twodec(shell) + ' ' \
                         '&#8491; <a href="' + pdbfilename + '">PDB</a> ' \
                         '<a href="' + ciffilename + '">mmCIF</a>\n'
                     page += '\t\t\t</div>\n'
             page += '\t\t</div>\n'
             page += '\t\t</div>\n'
     page += """
 \t<h2>References</h2>
 \t\tPlease cite the used software:
 \t\t<ul>
-\t\t<li>Paired refinement under the control of <i>PAIREF</i>. M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko (2020) <i>IUCrJ</i> <b>7</b></li>
+\t\t<li>Paired refinement under the control of <i>PAIREF</i>. M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko (2020) <i>IUCrJ</i> <b>7</b>:681-692, DOI: <a href='https://doi.org/10.1107/S2052252520005916'>10.1107/S2052252520005916</a></li>
 """
     if not args.phenix or "ccp4" in sys.executable.lower():
-        page += "\t\t<li>Overview of the <i>CCP</i>4 suite and current developments. Collaborative Computational Project, Number 4 (2011) <i>Acta Cryst.</i> D<b>67</b>:235-242</li>\n"
+        page += "\t\t<li>The <i>CCP</i>4 suite: integrative software for macromolecular crystallography. J. Agirre <i>et al</i>. (2023) <i>Acta Cryst. D</i> <b>79</b>(6):449-461, DOI: 10.1107/S2059798323003595</li>\n"
     if args.phenix:
-        page += "\t\t<li>Macromolecular structure determination using X-rays, neutrons and electrons: recent developments in <i>Phenix</i>. D. Liebschner, P.V. Afonine, M.L. Baker, G. Bunkóczi, V.B. Chen, T.I. Croll, B. Hintze, L.W. Hung, S. Jain, A.J. McCoy, N.W. Moriarty, R.D. Oeffner, B.K. Poon, M.G. Prisant, R.J. Read, J.S. Richardson, D.C. Richardson, M.D. Sammito, O.V. Sobolev, D.H. Stockwell, T.C. Terwilliger, A.G. Urzhumtsev, L.L. Videau, C.J. Williams, P.D. Adams (2019) <i>Acta Cryst.</i> D<b>75</b>:861-877</li>\n"
-        page += "\t\t<li>Towards automated crystallographic structure refinement with <i>phenix.refine</i>. P.V. Afonine, R.W. Grosse-Kunstleve, N. Echols, J.J. Headd, N.W. Moriarty, M. Mustyakimov, T.C. Terwilliger, A. Urzhumtsev, P.H. Zwart, P.D. Adams (2012) <i>Acta Cryst.</i> D<b>68</b>:352-67</li>\n"
+        page += "\t\t<li><i>PAIREF</i>: paired refinement also for Phenix users. M. Maly, K. Diederichs, J. Dohnalek, P. Kolenko (2021) <i>Acta Cryst. F</i><b>77</b>:226-229, DOI: <a href='https://doi.org/10.1107/s2053230x21006129'>10.1107/s2053230x21006129</a></li>\n"
+        page += "\t\t<li>Macromolecular structure determination using X-rays, neutrons and electrons: recent developments in <i>Phenix</i>. D. Liebschner, P.V. Afonine, M.L. Baker, G. Bunkóczi, V.B. Chen, T.I. Croll, B. Hintze, L.W. Hung, S. Jain, A.J. McCoy, N.W. Moriarty, R.D. Oeffner, B.K. Poon, M.G. Prisant, R.J. Read, J.S. Richardson, D.C. Richardson, M.D. Sammito, O.V. Sobolev, D.H. Stockwell, T.C. Terwilliger, A.G. Urzhumtsev, L.L. Videau, C.J. Williams, P.D. Adams (2019) <i>Acta Cryst. D</i><b>75</b>:861-877</li>\n"
+        page += "\t\t<li>Towards automated crystallographic structure refinement with <i>phenix.refine</i>. P.V. Afonine, R.W. Grosse-Kunstleve, N. Echols, J.J. Headd, N.W. Moriarty, M. Mustyakimov, T.C. Terwilliger, A. Urzhumtsev, P.H. Zwart, P.D. Adams (2012) <i>Acta Cryst. D</i><b>68</b>:352-67</li>\n"
     else:
-        page += "\t\t<li><i>REFMAC</i>5 for the refinement of macromolecular ""crystal structures. G.N. Murshudov, P. Skubak, A.A. Lebedev, N.S. Pannu, R.A. Steiner, R.A. Nicholls, M.D. Winn, F. Long, A.A. Vagin (2011) <i>Acta Cryst.</i> D<b>67</b>:355-367</li>\n"
+        page += "\t\t<li><i>REFMAC</i>5 for the refinement of macromolecular ""crystal structures. G.N. Murshudov, P. Skubak, A.A. Lebedev, N.S. Pannu, R.A. Steiner, R.A. Nicholls, M.D. Winn, F. Long, A.A. Vagin (2011) <i>Acta Cryst. D</i><b>67</b>:355-367</li>\n"
     if which("sfcheck"):
-        page += "\t\t<li><i>SFCHECK</i>: a unified set of procedures for evaluating the quality of macromolecular structure-factor data and their agreement with the atomic model. A.A. Vaguine, J. Richelle, S.J. Wodak (1999) <i>Acta Cryst.</i> D<b>55</b>:191-205</li>\n"
+        page += "\t\t<li><i>SFCHECK</i>: a unified set of procedures for evaluating the quality of macromolecular structure-factor data and their agreement with the atomic model. A.A. Vaguine, J. Richelle, S.J. Wodak (1999) <i>Acta Cryst. D</i><b>55</b>:191-205</li>\n"
     page += """
 \t\t<li>The <i>Computational Crystallography Toolbox</i>: crystallographic algorithms in a reusable software framework. R.W. Grosse-Kunstleve, N.K. Sauter, N.W. Moriarty, P.D. Adams (2002) <i>J. Appl. Crystallogr.</i> <b>35</b>:126-136</li>
 \t\t</ul>
 \t\t&nbsp;
 \t\t<ul>
-\t\t<li>Linking crystallographic model and data quality.  P.A. Karplus & K. Diederichs (2012) <i>Science</i> <b>336</b>:1030-3</li>
+\t\t<li>Linking crystallographic model and data quality.  P.A. Karplus & K. Diederichs (2012) <i>Science</i> <b>336</b>:1030-1033</li>
 \t\t<li>Assessing and maximizing data quality in macromolecular crystallography. P.A. Karplus & K. Diederichs (2015) <i>Cur. Op. in Str. Biology</i> <b>34</b>:60-68</li>
 \t\t<li>Better models by discarding data? P.A. Karplus & K. Diederichs (2013) <i>Acta Cryst.</i> D<b>59</b>:1215-1222</li>
 \t\t</ul>
 
 
 </body>
 </html>"""
 
     htmlfilename = "PAIREF_" + args.project + ".html"
-    with open(htmlfilename, "w") as htmlfile:
-        htmlfile.write(page)
+    if int(platform.python_version_tuple()[0]) == 2:
+        with open(htmlfilename, "w") as htmlfile:
+            htmlfile.write(page)
+    else:  # Python 3
+        with open(htmlfilename, "w", encoding="utf-8") as htmlfile:
+            htmlfile.write(page)
 
     # Styles
     cssfilepath = str(os.path.dirname(os.path.abspath(__file__))) + \
         "/static/styles.css"
     if os.path.isfile(cssfilepath):
         shutil.copy2(cssfilepath, ".")
```

### Comparing `pairef-1.3.9/pairef/refinement.py` & `pairef-1.4.0/pairef/refinement.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import subprocess
 import shutil
 from math import sqrt
 from .settings import warning_dict, settings
 from .commons import twodec, twodecname, fourdec, extract_from_file, warning_my
 from .commons import Popen_my
+from .preparation import which
 
 
 def refinement_refmac(res_cur,
                       res_prev,
                       res_high,
                       args,
                       n_bins_low,
@@ -113,15 +114,15 @@
             com = comfile.read()   # com is str (modified content of the file)
         re_end = re.compile(re.escape("end"), re.IGNORECASE)
         com = re_end.sub("", com)
         # com = re.sub("(?i)end","", com) # case-insensitive
         com += "\n refi reso " + reso + " \n"
         if not any(["ncyc" in line.lower() for line in com.splitlines()]) \
            and not args.ncyc:
-            args.ncyc = 10
+            args.ncyc = 20
     prefix = args.project + "_R" + str(flag).zfill(2) + "_" \
         "" + twodecname(res_cur) + "A"
     if mode == "comp":
         print(" .", end="")
         # print("       Calculating statistics of the refined structure model."
         ncyc_not_zero = False
         prefix += "_comparison" \
@@ -162,15 +163,15 @@
     elif mode == "refine":
         prefix += ""
         com += "\n bins " + str(n_bins_low)
         ncyc_not_zero = True
         if args.ncyc:
             com += "\n ncyc " + str(args.ncyc)
         elif not args.comin:
-            com += "\n ncyc 10"
+            com += "\n ncyc 20"
         if args.quick:
             com += "\n ncyc 1"
     if bfac_set:
         com += "\n BFACtor SET " + twodec(bfac_set)
     if args.weight:
         com += "\n weight matrix " + fourdec(args.weight)
     # Shannon factor
@@ -197,16 +198,20 @@
     logout = prefix + ".log"
     if mode == "refine":
         xyzin = args.project + "_R" + str(flag).zfill(2) + "_" + \
             twodecname(res_prev) + "A" + settings["pdbORmmcif"]
     elif mode == "comp" or mode == "prev_pair":
         xyzin = args.project + "_R" + str(flag).zfill(2) + "_" + \
             twodecname(res_cur) + "A" + settings["pdbORmmcif"]
-    command = ["refmac5", "HKLIN", args.hklin, "XYZIN", xyzin, "HKLOUT",
-               hklout, "XYZOUT", xyzout, "LIBOUT", libout]
+    if which("refmacat"):
+        refmac_executable = "refmacat"
+    else:
+        refmac_executable = "refmac5"
+    command = [refmac_executable, "HKLIN", args.hklin, "XYZIN", xyzin,
+               "HKLOUT", hklout, "XYZOUT", xyzout, "LIBOUT", libout]
     # Optional LIBIN
     if args.libin:
         command.append("LIBIN")
         command.append(args.libin)
     # Optional TLSIN (and TLSOUT)
     if args.tlsin:
         if ncyc_not_zero:
@@ -234,15 +239,15 @@
                              "the details.\nAborting.\n")
             sys.exit(1)
     # Copy log and tls while running REFMAC5 at the starting resolution
     if mode == "first":
         prefix_copy = prefix + "_comparison_at_" + twodecname(res_high) + "A"
         shutil.copy2(logout, prefix_copy + ".log")
         shutil.copy2(hklout, prefix_copy + ".mtz")
-    version = extract_from_file(logout, "version", 0, 1, nth_word=5,
+    version = extract_from_file(logout, "  version", 0, 1, nth_word=5,
                                 get_first=True)
     results = {"HKLOUT": hklout, "XYZOUT": xyzout, "LOGOUT": logout,
                "version": version}
     if mode == "comp" or mode == "prev_pair":
         files_to_be_removed = [xyzout, xyzout_secondary, libout]
         if "tlsout" in vars():
             to_be_removed += [tlsout]
@@ -335,17 +340,43 @@
         "" + twodecname(res_cur) + "A"
     if mode == "refine":
         xyzin = args.project + "_R" + str(flag).zfill(2) + "_" + \
             twodecname(res_prev) + "A_001" + settings["pdbORmmcif"]
     elif mode == "comp" or mode == "prev_pair":
         xyzin = args.project + "_R" + str(flag).zfill(2) + "_" + \
             twodecname(res_cur) + "A_001" + settings["pdbORmmcif"]
-    com = "refinement.input.xray_data.high_resolution=" + twodec(res_high)
+    if settings["phenix_subversion"] >= 21:
+        com = "data_manager {"
+        com += "\n  fmodel {"
+        com += "\n    xray_data {"
+        com += "\n      high_resolution=" + twodec(res_high)
+    else:
+        com = "refinement.input.xray_data.high_resolution=" + twodec(res_high)
     if res_low:
-        com += "\nrefinement.input.xray_data.low_resolution=" + twodec(res_low)
+        if settings["phenix_subversion"] >= 21:
+            com += "\n      low_resolution=" + twodec(res_low)
+        else:
+            com += "\nrefinement.input.xray_data.low_resolution=" + twodec(res_low)
+    if settings["phenix_subversion"] >= 21:
+        com += "\n      r_free_flags.test_flag_value=" + str(flag)
+    else:
+        com += "\nrefinement.input.xray_data.r_free_flags.test_flag_value=" + str(flag)
+    if settings["phenix_subversion"] >= 21:
+        com += "\n    }"
+        com += "\n  }"
+    if hasattr(args, "label"):  # always false for the very first mode="refine"
+        if settings["phenix_subversion"] >= 21:
+            com += "\n  miller_array {"
+            com += "\n    file=" + args.hklin
+            com += "\n    labels.name='" + args.label.split(":")[1] + "'"
+            com += "\n  }"
+        else:
+            com += "\nrefinement.input.xray_data.labels=" + args.label
+    if settings["phenix_subversion"] >= 21:
+        com += "\n}"
     if args.defin:
         with open(args.defin, "r") as deffile:
             deff = deffile.read()
             if not any(["number_of_macro_cycle" in line for line in deff.splitlines()]) \
                and not args.ncyc:
                 args.ncyc = 3
 
@@ -398,30 +429,32 @@
         ncyc_not_zero = True
         if args.ncyc:
             com += "\nrefinement.main.number_of_macro_cycles=" + str(args.ncyc)
         elif not args.defin:
             com += "\nrefinement.main.number_of_macro_cycles=3"
         if args.quick:
             com += "\nrefinement.main.number_of_macro_cycles=1"
-    com += "\nrefinement.gui.base_output_dir=None"
-    com += "\nrefinement.gui.tmp_dir=None"
-    com += "\nrefinement.gui.notify_email=None"
-    com += "\nrefinement.output.n_resolution_bins=" + str(n_bins)
-    com += "\nrefinement.output.prefix=" + prefix
-    com += "\nrefinement.output.serial=None"
-    com += "\nrefinement.output.serial_format='%03d'"
+    if settings["phenix_subversion"] >= 21:
+        # com += "\nrefinement.main.max_number_of_resolution_bins=" + str(n_bins)
+        com += "\noutput.prefix=" + prefix
+        com += "\noutput.serial=None"
+        com += "\noutput.serial_format='%03d'"
+    else:
+        com += "\nrefinement.output.n_resolution_bins=" + str(n_bins)
+        com += "\nrefinement.output.prefix=" + prefix
+        com += "\nrefinement.output.serial=None"
+        com += "\nrefinement.output.serial_format='%03d'"
+        com += "\nrefinement.gui.base_output_dir=None"
+        com += "\nrefinement.gui.tmp_dir=None"
+        com += "\nrefinement.gui.notify_email=None"
     # com += "\nrefinement.input.pdb.filename=" + xyzin
     # com += "\nrefinement.input.xray_data.filename=" + args.hklin
     # com += "\nrefinement.input.xray_data.r_free_flags.filename=" + args.hklin
     # com += "\nrefinement.input.monomers.file_name=None"
     # com += "\nrefinement.input.sequence.file_name=None"
-    com += "\nrefinement.input.xray_data.r_free_flags.test_flag_value=" + \
-        str(flag)
-    if hasattr(args, "label"):  # always false for the very first mode="refine"
-        com += "\nrefinement.input.xray_data.labels=" + args.label
     # Output filenames
     if "cif" in settings["pdbORmmcif"]:
         xyzout = prefix + "_001" + settings["pdbORmmcif"]
         xyzout_secondary = prefix + "_001" + ".pdb"
     else:  # pdb
         xyzout = prefix + "_001" + settings["pdbORmmcif"]
         xyzout_secondary = prefix + "_001" + ".cif"
@@ -430,18 +463,22 @@
     geoout = prefix + "_001.geo"
     outout = prefix + "_001.out"
     params = prefix + "_001.params"
     command = ["phenix.refine", args.hklin, xyzin]
     if args.libin:
         command.append(args.libin)
     if args.defin:
-        command.append(args.defin)
+        if settings["phenix_subversion"] >= 21:
+            com += "\ndata_manager.phil_files=" + args.defin
+        else:
+            command.append(args.defin)
     with open(params, "w") as pars:
         pars.write(com)
     command.append(params)
+    # command.append("output.overwrite=True")
 
     if (mode == "refine" or
             (mode == "first" and args.complete_cross_validation)):
         if args.complete_cross_validation:
             print("     – FreeRflag set " + str(flag))
         print("       Running command:")
         print("       " + " ".join(command))
@@ -482,20 +519,19 @@
                                  "\nAborting.\n")
                 sys.exit(1)
     # Copy log and tls while running phenix.refine at the starting resolution
     if mode == "first":
         pdbout = prefix + "_001" + ".pdb"
         prefix_copy = prefix + "_comparison_at_" + twodecname(res_high) + "A"
         shutil.copy2(pdbout, prefix_copy + "_001.pdb")
-    version = extract_from_file(logout, "Version", 0, 1, nth_word=1,
-                                get_first=True)
-    results = {"HKLOUT": hklout, "XYZOUT": xyzout, "LOGOUT": logout,
-               "version": version}
+        shutil.copy2(hklout, prefix_copy + "_001.mtz")
+    results = {"HKLOUT": hklout, "XYZOUT": xyzout, "LOGOUT": logout}
+    #           "version": version}
     if mode == "comp" or mode == "prev_pair":
-        files_to_be_removed = [hklout, geoout]
+        files_to_be_removed = [geoout]
         if "tlsout" in vars():
             to_be_removed += [tlsout]
         for filename in files_to_be_removed:
             if os.path.exists(filename):
                 os.remove(filename)
     return results
 
@@ -536,17 +572,17 @@
     return label, labels_all
 
 
 def collect_stat_BINNED(shells, project, hklin, n_bins_low, flag,
                         res_low, refinement="refmac"):
     """Collects statistics of a particular structure model depending on
     resolution (*e. i.* values are binned) and saves them in a CSV file.
-    Statistics are picked from a REFMAC5 logfile relating to the model
-    `project_RXX_twodecname(shells[-1])A.pdb`, where `XX` is a number
-    of a flag.
+    For REFMAC5, statistics are picked from a logfile relating to the model
+    `project_RXX_twodecname(shells[-1])A`, where `XX` is a number
+    of a flag. For Phenix, statistics are calculated using CCTBX from MTZ.
 
     This function is called by the function `main()` in file `launcher.py`.
 
     Args:
         shells (list) - Contains high resolution diffraction limits
                         from the initial to the last which were used
                         for that model (float).
@@ -581,24 +617,31 @@
             collect_stat_overall_refmac(prefix + ".log", flag)
         overall_CCwork, overall_CCfree = calculate_correlation(mtzfilename,
                                                                hklin, flag)
         overall_CCwork = fourdec(overall_CCwork)
         overall_CCfree = fourdec(overall_CCfree)
     elif refinement == "phenix":
         # Pick statistics for `n_bins_low` res. shells up to initial diffr. limit
-        pdbfilename = prefix + "_comparison" \
-            "_at_" + twodecname(shells[0]) + "A_001.pdb"
+        # pdbfilename = prefix + "_comparison" \
+        #     "_at_" + twodecname(shells[0]) + "A_001.pdb"
+        mtzfilename = prefix + "_comparison" \
+            "_at_" + twodecname(shells[0]) + "A_001.mtz"
+        fobs, fmodel, flags = get_f_cctbx(mtzfilename)
         bin_res_low, bin_res_high, bin_Nwork, bin_Nfree, \
             bin_Rwork, bin_Rfree, bin_CCwork, bin_CCfree = \
-            collect_stat_binned_phenix_low(pdbfilename, n_bins_low, res_low)
+            calculate_stats_cctbx(fobs, fmodel, flags, n_bins=n_bins_low)
+        #   collect_stat_binned_phenix_low(pdbfilename, n_bins_low, res_low)
         # Pick overall values for data up to previous diffraction limit
         # (to be comparable pairwisely)
-        pdbfilename = prefix + "_001.pdb"
+        # pdbfilename = prefix + "_001.pdb"
+        mtzfilename = prefix + "_001.mtz"
+        fobs, fmodel, flags = get_f_cctbx(mtzfilename)
         overall_Rwork, overall_Rfree = \
-            collect_stat_overall_phenix(pdbfilename)
+            calculate_stats_cctbx(fobs, fmodel, flags, n_bins=1, overall=True)
+        #   collect_stat_overall_phenix(pdbfilename)
         overall_CCwork = "N/A"
         overall_CCfree = "N/A"
         overall_CCavg = "N/A"
     # Write the statistics to a csv file
     csvfilename = prefix + ".csv"
     with open(csvfilename, "w") as csvfile:
         csvfile.write("# Statistics of refined structure model calculated "
@@ -614,29 +657,33 @@
                       "Rfree   CCwork  CCfree \n")
     collect_stat_write(csvfilename, bin_res_low, bin_res_high,
                               bin_Nwork, bin_Nfree,
                               bin_Rwork, bin_Rfree,
                               bin_CCwork, bin_CCfree)
     # Pick stats. for the high resolution shells and write them to the CSV file
     for i in range(len(shells) - 1):
+        bin_res_low = [twodec(shells[i])]
+        bin_res_high = [twodec(shells[i + 1])]
         if refinement == "refmac":
-            bin_res_low = [twodec(shells[i])]
-            bin_res_high = [twodec(shells[i + 1])]
             logfilename = prefix + "_comparison" \
                 "_at_" + twodecname(shells[i + 1]) + "A.log"
             mtzfilename = prefix + ".mtz"
             bin_Nwork, bin_Nfree, bin_Rwork, bin_Rfree, bin_CCwork, \
                 bin_CCfree = collect_stat_binned_refmac_high(
                     logfilename, mtzfilename, hklin, n_bins_low,
                     float(twodec(shells[i])), float(twodec(shells[i + 1])), flag)
         elif refinement == "phenix":
-            pdbfilename = prefix + "_comparison" \
-                "_at_" + twodecname(shells[i + 1]) + "A_001.pdb"
-            bin_res_low, bin_res_high, bin_Nwork, bin_Nfree, bin_Rwork, bin_Rfree, \
-                bin_CCwork, bin_CCfree = collect_stat_binned_phenix_high(pdbfilename, n_bins_low)
+            # pdbfilename = prefix + "_comparison" \
+            #     "_at_" + twodecname(shells[i + 1]) + "A_001.pdb"
+            mtzfilename = prefix + "_comparison" \
+                "_at_" + twodecname(shells[i + 1]) + "A_001.mtz"
+            fobs, fmodel, flags = get_f_cctbx(mtzfilename)
+            _bin_res_low, _bin_res_high, bin_Nwork, bin_Nfree, bin_Rwork, bin_Rfree, \
+                bin_CCwork, bin_CCfree = calculate_stats_cctbx(fobs, fmodel, flags, n_bins=1)
+            #                          = collect_stat_binned_phenix_high(pdbfilename, n_bins_low)
         collect_stat_write(
             csvfilename, bin_res_low, bin_res_high, bin_Nwork, bin_Nfree,
             bin_Rwork, bin_Rfree, bin_CCwork, bin_CCfree,
             shell_number=n_bins_low + 1 + i)
     return csvfilename
 
 
@@ -758,22 +805,24 @@
     except IndexError:
         bin_Nfree = ["N/A"]
     return(bin_Nwork, bin_Nfree, bin_Rwork, bin_Rfree,
            bin_CCwork, bin_CCfree)
 
 
 def collect_stat_binned_phenix_low(pdbfilename, n_bins_low, res_low=999):
-    """Picks and returns statistics values in the given `REFMAC5` logfile.
+    """This function is deprecated and not used now, it does not work
+    for Phenix 1.21 and newer. Function calculate_stats_cctbx() is used instead.
+    Picks and returns statistics values in the given PDB.
     Logfile supposed to contain information from `n_bins_low` shells.
 
     This function is called by the function `collect_stat_BINNED()`
     from this file and `main()` from file `launcher.py`.
 
     Args:
-        pdbfilename (str): Name of a `REFMAC5` logfile
+        pdbfilename (str): Name of a PDB
         n_bins_low (int): Number of low resolution bins
 
     Returns:
         (tuple): tuple containing statistics
         values `bin_Nwork`, `bin_Nfree`, `bin_Rwork`,
         `bin_Rfree`, `bin_CCwork`, and `bin_CCfree` (all are `str`)
     """
@@ -786,28 +835,32 @@
     bin_CCwork = []
     bin_CCfree = []
     # # Definition of bins, numbers of reflections, R-values
     pdbfile_lines = extract_from_file(
         pdbfilename, "REMARK   3   BIN  RESOLUTION RANGE  COMPL.    "
         "NWORK NFREE   RWORK  RFREE  CCWORK CCFREE", 1, n_bins_low)
     for i in range(n_bins_low):
+        print(pdbfile_lines[i])####################
+        print(pdbfile_lines[i].split())
         bin_res_low.append(pdbfile_lines[i].split()[3])
         bin_res_high.append(pdbfile_lines[i].split()[5])
         bin_Nwork.append(pdbfile_lines[i].split()[7])
         bin_Nfree.append(pdbfile_lines[i].split()[8])
         bin_Rwork.append(pdbfile_lines[i].split()[9])
         bin_Rfree.append(pdbfile_lines[i].split()[10])
         bin_CCwork.append(pdbfile_lines[i].split()[11])
         bin_CCfree.append(pdbfile_lines[i].split()[12])
     return(bin_res_low, bin_res_high, bin_Nwork, bin_Nfree,
            bin_Rwork, bin_Rfree, bin_CCwork, bin_CCfree)
 
 
 def collect_stat_binned_phenix_high(pdbfilename, n_bins_low):
-    """Picks and returns statistics values in the given `REFMAC5` logfile.
+    """This function is deprecated and not used now, it does not work
+    for Phenix 1.21 and newer. Function calculate_stats_cctbx() is used instead.
+    Picks and returns statistics values in the given `REFMAC5` logfile.
     Logfile supposed to contain information from 1 shells.
 
     This function is called by the function `collect_stat_BINNED()`.
 
     Args:
         logfilename (str): Name of a `REFMAC5` logfile
         n_bins_low (int): Number of low resolution bins
@@ -850,16 +903,16 @@
 
     Returns:
         str: Filename of the created CSV file.
     """
     with open(csvfilename, "a") as csvfile:
         for i in range(len(bin_Rwork)):
             csvfile.write(
-                str(shell_number).zfill(2) + "        " + bin_res_low[i] + ""
-                " - " + bin_res_high[i] + "         " + bin_Nwork[i] + "     "
+                str(shell_number).zfill(2) + "        " + str(bin_res_low[i]) + ""
+                " - " + str(bin_res_high[i]) + "         " + bin_Nwork[i] + "     "
                 "" + bin_Nfree[i] + "     " + bin_Rwork[i] + "     "
                 "" + bin_Rfree[i] + "     " + bin_CCwork[i] + "     "
                 "" + bin_CCfree[i] + "\n")
             if float(bin_Nfree[i]) < 50:
                 warning_my("Nfree", "There are only " + str(bin_Nfree[i]) + ""
                            " < 50 free reflections in the resolution shell "
                            "" + twodec(bin_res_low[i]) + "-"
@@ -869,17 +922,17 @@
                            "thicker resolution shells.")
             shell_number = shell_number + 1
     return csvfilename
 
 
 def collect_stat_OVERALL(shells, args, flag, refinement="refmac"):
     """Collects overall statistics of a particular structure model
-    from a REFMAC5 logfile or from PDB file (phenix.refine).
-    Model which is dealing with: `project_RXX_twodecname(shells[-1])A.pdb`
-    (REFMAC5) or `project_RXX_twodecname(shells[-1])A_001.pdb` (phenix.refine),
+    from a REFMAC5 logfile or using CCTBX (phenix.refine).
+    File which is dealing with: `project_RXX_twodecname(shells[-1])A.pdb`
+    (REFMAC5) or `project_RXX_twodecname(shells[-1])A_001.mtz` (phenix.refine),
     where `XX` is a number of a flag.
 
     This function is called by the function `main()` in file `launcher.py`.
 
     Args:
         shells (list):  Contains high resolution diffraction limits
                         from the initial to the last which were used
@@ -907,21 +960,28 @@
             Rwork_after, Rfree_after = \
                 collect_stat_overall_refmac(filename_prefix + ".log", flag)
             mtzfilename = prefix + "_" + twodecname(shells[-1]) + "A.mtz"
             CCwork_after, CCfree_after = calculate_correlation(
                 mtzfilename, args.hklin, flag, res_high=float(shells[-2]))  # floats
         elif refinement == "phenix":
             # get Rwork, Rfree                (not CCwork, CCfree, CCavg)
-            pdbfilename = prefix + "_" + twodecname(shells[-2]) + "A_001.pdb"
+            # pdbfilename = prefix + "_" + twodecname(shells[-2]) + "A_001.pdb"
+            mtzfilename = prefix + "_" + twodecname(shells[-2]) + "A_001.mtz"
+            fobs, fmodel, flags = get_f_cctbx(mtzfilename)
             Rwork_before, Rfree_before = \
-                collect_stat_overall_phenix(pdbfilename)
-            pdbfilename = prefix + "_" + twodecname(shells[-1]) + "A_comparison" \
-                "_at_" + twodecname(shells[-2]) + "A_prev_pair_001.pdb"
+                calculate_stats_cctbx(fobs, fmodel, flags, n_bins=1, overall=True)
+            #     collect_stat_overall_phenix(pdbfilename)
+            # pdbfilename = prefix + "_" + twodecname(shells[-1]) + "A_comparison" \
+            #     "_at_" + twodecname(shells[-2]) + "A_prev_pair_001.pdb"
+            mtzfilename = prefix + "_" + twodecname(shells[-1]) + "A_comparison" \
+                "_at_" + twodecname(shells[-2]) + "A_prev_pair_001.mtz"
+            fobs, fmodel, flags = get_f_cctbx(mtzfilename)
             Rwork_after, Rfree_after = \
-                collect_stat_overall_phenix(pdbfilename)
+                calculate_stats_cctbx(fobs, fmodel, flags, n_bins=1, overall=True)
+            #   collect_stat_overall_phenix(pdbfilename)
 
         # Rwork, Rfree
         Rwork_change = fourdec(float(Rwork_after) - float(Rwork_before))
         Rfree_change = fourdec(float(Rfree_after) - float(Rfree_before))
         #
         csvfilename = prefix + "_R-values.csv"
         csvfilenames.append(csvfilename)
@@ -948,17 +1008,21 @@
     # Pick overall values of the current structure model
     # and find Rfree-Rwork gap (at the initial resolution)
     if refinement == "refmac":     # get Rwork, Rfree
         logfilename = prefix + "_" + twodecname(shells[-1]) + "A" \
             "_comparison_at_" + twodecname(shells[0]) + "A.log"
         Rwork, Rfree = collect_stat_overall_refmac(logfilename, flag)
     elif refinement == "phenix":   # get Rwork, Rfree
-        pdbfilename = prefix + "_" + twodecname(shells[-1]) + "A" \
-            "_comparison_at_" + twodecname(shells[0]) + "A_001.pdb"
-        Rwork, Rfree = collect_stat_overall_phenix(pdbfilename)
+        # pdbfilename = prefix + "_" + twodecname(shells[-1]) + "A" \
+        #     "_comparison_at_" + twodecname(shells[0]) + "A_001.pdb"
+        # Rwork, Rfree = collect_stat_overall_phenix(pdbfilename)
+        mtzfilename = prefix + "_" + twodecname(shells[-1]) + "A" \
+            "_comparison_at_" + twodecname(shells[0]) + "A_001.mtz"
+        fobs, fmodel, flags = get_f_cctbx(mtzfilename)
+        Rwork, Rfree = calculate_stats_cctbx(fobs, fmodel, flags, overall=True)
     Rgap = fourdec(float(Rfree) - float(Rwork))
     csvfilename_gap = prefix + "_Rgap.csv"
     # Write the begining of the csv file if it does not exist yet
     if not os.path.isfile(csvfilename_gap):
         with open(csvfilename_gap, "w") as csvfile:
             csvfile.write("# Resolution   Rwork   Rfree   Rfree-Rwork\n")
     with open(csvfilename_gap, "a") as csvfile:
@@ -1015,15 +1079,16 @@
     for i, column in enumerate(miller_arrays):
         if column.is_xray_intensity_array() and \
                 column.anomalous_flag() == False:
             i_obs_label = str(column.info()).split(".mtz:")[1].split(",")[0]
             i_obs = column
             break
     if not i_obs:
-        print("Error - intensities were not found in " + hklin)  # TO DO
+        warning_my("noI", "Intensities were not found in " + hklin + ". "
+                   "CCwork and CCfree values cannot be calculated.")
         return "N/A", "N/A"
 
     # prepare sftools command and run
     if res_low and res_high:  # else: full resolution of MTZ file
         com_resolution = " resolution " + fourdec(res_low) + " " + fourdec(res_high)
     elif res_high:
         com_resolution = " resolution 999 " + fourdec(res_high)
@@ -1044,18 +1109,18 @@
     output, err = p.communicate(com)
 
     # pick values
     CCwork = None
     CCfree = None
     output_lines = output.splitlines()
     for i in range(len(output.splitlines())):
-        if "WARNING" in output.splitlines()[i]:
-            print(output.splitlines()[i])
-            return "N/A", "N/A"
-        elif " $TABLE: Correlation vs. resolution:" in output.splitlines()[i] and \
+        # if "WARNING" in output.splitlines()[i]:
+        #     print(output.splitlines()[i]) #####
+        #     # return "N/A", "N/A"
+        if " $TABLE: Correlation vs. resolution:" in output.splitlines()[i] and \
                 "$$" in output.splitlines()[i + 2] and \
                 "$$" in output.splitlines()[i + 4] and \
                 "$$" in output.splitlines()[i + 6] and \
                 "NSHELL  DMIN    DMAX    RFACT   CORREL    <F1>    <F2>    NREF $$" in output.splitlines()[i + 3]:
             if not CCfree:
                 try:
                     CCfree = float(output.splitlines()[i + 5].split()[4])
@@ -1074,15 +1139,17 @@
         CCfree = "N/A"
     if not CCwork:
         CCwork = "N/A"
     return CCwork, CCfree
 
     
 def collect_stat_overall_phenix(pdbfilename):
-    """Picks and returns overall Rwork, Rfree values from a given PDB file 
+    """This function is deprecated and not used now, it does not work
+    for Phenix 1.21 and newer. Function calculate_stats_cctbx() is used instead.
+    Picks and returns overall Rwork, Rfree values from a given PDB file 
     refined in phenix.refine.
 
     This function is called by the functions `collect_stat_OVERALL()`
     and `collect_stat_BINNED()`.
 
     Args:
         pdbfilename (str): Filename of a PDB structure model refined in \
@@ -1097,14 +1164,98 @@
         "REMARK   3   R VALUE            (WORKING SET) : ", 0, 1, -1)
     Rfree = extract_from_file(
         pdbfilename,
         "REMARK   3   FREE R VALUE                     : ", 0, 1, -1)
     return Rwork, Rfree
 
 
+def get_f_cctbx(mtzfilename, d_max=0, d_min=0):
+    from iotbx.reflection_file_utils import get_r_free_flags_scores
+    from iotbx.file_reader import any_file
+    mtz_in = any_file(mtzfilename)
+    ma = mtz_in.file_server.miller_arrays
+    flags = fmodel = fobs = None
+    # select the output arrays from phenix.refine
+    for array in ma :
+        labels = array.info().label_string()
+        if labels.startswith("R-free-flags"):
+            flags = array
+        elif labels.startswith("F-model"):
+            fmodel = abs(array)
+        elif labels.startswith("F-obs-filtered"):
+            fobs = array
+    if (None in [flags, fobs, fmodel]):
+        raise RuntimeError("Not a valid phenix.refine output file")
+    scores = get_r_free_flags_scores([flags], None)
+    test_flag_value = scores.test_flag_values[0]
+    flags = flags.customized_copy(data=flags.data()==test_flag_value)
+    fmodel = fmodel.resolution_filter(d_max=d_max, d_min=d_min)
+    fmodel, fobs = fmodel.common_sets(other=fobs)
+    fmodel, flags = fmodel.common_sets(other=flags)
+    return fobs, fmodel, flags
+
+
+def calculate_stats_cctbx(fobs, fmodel, flags, n_bins=10, overall=False, bins=False):
+    """Based on iotbx/examples/recalculate_phenix_refine_r_factors.py"""
+    fmodel, fobs = fmodel.common_sets(other=fobs)
+    fmodel, flags = fmodel.common_sets(other=flags)
+    fc_work = fmodel.select(~(flags.data()))
+    fo_work = fobs.select(~(flags.data()))
+    fc_test = fmodel.select(flags.data())
+    fo_test = fobs.select(flags.data())
+    r_work = str(round(fo_work.r1_factor(fc_work), 4))
+    r_free = str(round(fo_test.r1_factor(fc_test), 4))
+    # print("r_work = %.4f" % r_work)
+    # print("r_free = %.4f" % r_free)
+    if overall:
+        return r_work, r_free
+    flags.setup_binner(n_bins=n_bins)
+    fo_work.use_binning_of(flags)
+    fc_work.use_binner_of(fo_work)
+    fo_test.use_binning_of(fo_work)
+    fc_test.use_binning_of(fo_work)
+    bin_res_low = []
+    bin_res_high = []
+    bin_Nwork = []
+    bin_Nfree = []
+    bin_Rwork = []
+    bin_Rfree = []
+    bin_CCwork = []
+    bin_CCfree = []
+    for i_bin in fo_work.binner().range_all():
+        sel_work = fo_work.binner().selection(i_bin)
+        sel_test = fo_test.binner().selection(i_bin)
+        fo_work_bin = fo_work.select(sel_work)
+        fc_work_bin = fc_work.select(sel_work)
+        fo_test_bin = fo_test.select(sel_test)
+        fc_test_bin = fc_test.select(sel_test)
+        if fc_test_bin.size() == 0 : continue
+        _bin_res_low, _bin_res_high = fo_work_bin.d_max_min()
+        bin_res_low.append(str(round(_bin_res_low, 2)))
+        if bins: continue
+        bin_res_high.append(str(round(_bin_res_high, 2)))
+        bin_Nwork.append(str(fo_work_bin.size()))
+        bin_Nfree.append(str(fo_test_bin.size()))
+        bin_Rwork.append(str(round(fo_work_bin.r1_factor(other=fc_work_bin,
+            assume_index_matching=True), 4)))
+        bin_Rfree.append(str(round(fo_test_bin.r1_factor(other=fc_test_bin,
+            assume_index_matching=True), 4)))
+        bin_CCwork.append(str(round(fo_work_bin.correlation(fc_work_bin).coefficient(), 4)))
+        bin_CCfree.append(str(round(fo_test_bin.correlation(fc_test_bin).coefficient(), 4)))
+        # legend = flags.binner().bin_legend(i_bin, show_counts=False)
+        # print("%s  %8d %8d  %.4f %.4f  %.3f %.3f" % (legend, fo_work_bin.size(),
+        #   fo_test_bin.size(), r_work_bin, r_free_bin, cc_work_bin, cc_free_bin))
+    # print(bin_res_low, bin_res_high, bin_Nwork, bin_Nfree,
+    #        bin_Rwork, bin_Rfree, bin_CCwork, bin_CCfree)
+    if bins:
+        return bin_res_low
+    return(bin_res_low, bin_res_high, bin_Nwork, bin_Nfree,
+           bin_Rwork, bin_Rfree, bin_CCwork, bin_CCfree)
+
+
 def collect_stat_OVERALL_AVG(shells, project, flag_sets):
     """Calculates and saves average overall values from CSV files prepared by
     the function `collect_stat_OVERALL()`.
 
     This function is called by the function `main()` in file `launcher.py`.
 
     Args:
@@ -1169,16 +1320,19 @@
                       "     " + space_Rwork + Rwork_diff_avg + "        "
                       "" + Rfree_init_avg + "     " + Rfree_fin_avg + "     "
                       "" + space_Rfree + Rfree_diff_avg + "         "
                       "" + Rwork_stdev + "       " + Rfree_stdev + "     "
                       "" + Rwork_diff_sem + "       " + Rfree_diff_sem + "\n")
 
     # === Rgap ===
-    Rgap_avg = fourdec(float(Rfree_fin_avg) - float(Rwork_fin_avg))
+    Rgap_fin_avg = fourdec(float(Rfree_fin_avg) - float(Rwork_fin_avg))
     csvfilename_gap = project + "_Rgap.csv"
     if not os.path.isfile(csvfilename_gap):
         with open(csvfilename_gap, "w") as csvfile:
+            Rgap_init_avg = fourdec(float(Rfree_init_avg) - float(Rwork_init_avg))
             csvfile.write("# Resolution   Rwork   Rfree   Rfree-Rwork\n")
+            csvfile.write(twodec(shells[0]) + "          " + Rwork_init_avg + "   "
+                          "" + Rfree_init_avg + "   " + Rgap_init_avg + "\n")
     with open(csvfilename_gap, "a") as csvfile:
         csvfile.write(twodec(shells[-1]) + "          " + Rwork_fin_avg + "   "
-                      "" + Rfree_fin_avg + "   " + Rgap_avg + "\n")
+                      "" + Rfree_fin_avg + "   " + Rgap_fin_avg + "\n")
     return csvfilename, csvfilename_gap
```

### Comparing `pairef-1.3.9/pairef/preparation.py` & `pairef-1.4.0/pairef/preparation.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,20 +199,21 @@
         (tuple):
             * shells (*list*)
             * n_bins_low (*int*)
             * n_flag_sets (*int*)
             * default_shells_definition (*bool*)
     """
     # If the resolution of input model == resolution of diffr. data, abort
-    if twodec(args.res_init) == twodec(res_high_mtz):
-        sys.stderr.write("ERROR: The given input structure model "
-                         "" + args.xyzin + " was refined at the same "
-                         "resolution as the given diffraction data "
-                         "" + args.hklin + " have. Nothing to do."
-                         "\nAborting.\n")
+    if twodec(args.res_init) <= twodec(res_high_mtz):
+        sys.stderr.write(
+            "ERROR: Given input MTZ file " + args.hklin + " contain data "
+            "only up to resolution " + twodec(res_high_mtz) + " A that is "
+            "the same or lower than the initial high-resolution diffraction "
+            "limit " + twodec(args.res_init) + " A. Nothing to do.\n"
+            "Aborting.\n")
         sys.exit(1)
     # Estimation of
     #   1. a number of low resolution bins and
     #   2. a number of free reflection sets
     # If not successful, just divide into 12 resolution bins
     # and consider 20 free reflection sets.
     n_i_obs = 0
@@ -340,14 +341,18 @@
                         "ERROR: Explicit definition of high "
                         "resolution shells (option -r) is not correct. ")
                     sys.stderr.write(
                         "Values must be set in the decreasing order "
                         "(e.g. 2.1,2.0,1.9).")
                     sys.stderr.write("\nAborting.\n")
                     sys.exit(1)
+        for i in range(len(shells_high)):
+            if twodec(shells_high[i]) <= twodec(res_high_mtz):
+                shells_high = shells_high[:i] + [round(float(res_high_mtz), 2)]
+                break
         if shells_high[0] >= args.res_init:
             sys.stderr.write(
                 "ERROR: Explicit definition of high "
                 "resolution shells (option -r) is not correct. ")
             sys.stderr.write(
                 "Resolution of the first shell (" + twodec(shells_high[0]) + ""
                 " A), "
@@ -370,16 +375,24 @@
                              " - ( " + str(args.step) + " * "
                              "" + str(args.n_shells) + ""
                              " ) = " + twodec(res_fin) + " < 0")
             sys.stderr.write("\nAborting.\n")
             sys.exit(1)
         shells_high = []
         for i in range(args.n_shells):
-            shells_high.append(args.res_init - (i + 1) * args.step)
-
+            new_shell = args.res_init - (i + 1) * args.step
+            if twodec(new_shell) >= twodec(res_high_mtz):
+                shells_high.append(args.res_init - (i + 1) * args.step)
+            elif i == 0:  # and new_shell < res_high_mtz:
+                shells_high = round(float(twodec(res_high_mtz)), 2)
+                break
+            else:  # i >= 1 and new_shell < res_high_mtz:
+                if twodec(res_high_mtz) != twodec(shells_high[i - 1]):
+                    shells_high.append(round(float(twodec(res_high_mtz)), 2))
+                break
     else:
         # Default setting - 0.05A wide high resolution shells
         shell_width = 0.05
         default_shells_definition = True
         shells_high = []
         res_cur = args.res_init - shell_width
         while round(res_cur, 3) >= round(res_high_mtz, 3):
@@ -420,15 +433,22 @@
                 # "ERROR: Definition of high resolution shells  using mtzdump "
                 # "was not successful. Is the MTZ file OK?")
             # sys.stderr.write(
                 # "Use manual definition of the high resolution shells to "
                 # "overcome this problem (option -r).")
             # sys.stderr.write("\nAborting.\n")
             # sys.exit(1)
-
+    if shells_high == []:
+        sys.stderr.write(
+            "ERROR: The given definition of high-resolution shells requires "
+            "more data in high resolution than are available in the given "
+            "input MTZ file " + args.hklin + " that contain data "
+            "only up to resolution " + twodec(res_high_mtz) + " A. Nothing to do.\n"
+            "Aborting.\n")
+        sys.exit(1)
     shells = [args.res_init] + shells_high
     return shells, n_bins_low, n_flag_sets, default_shells_definition
 
 
 def res_high_from_xyzin(xyzin, format=".pdb"):
     """Finds a line containing `RESOLUTION RANGE HIGH` in the file `xyzin`,
     picks the last word of the line (that should be the high resolution)
```

### Comparing `pairef-1.3.9/pairef/gui.py` & `pairef-1.4.0/pairef/gui.py`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/pairef/launcher.py` & `pairef-1.4.0/pairef/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from .settings import warning_dict, settings
 from .preparation import welcome, create_workdir, output_log, def_res_shells
 from .preparation import which, res_high_from_xyzin, res_from_mtz, res_opt
 from .preparation import calculate_merging_stats, run_pdbtools
 from .preparation import res_from_hklin_unmerged, check_refinement_software
 from .preparation import suggest_cutoff
 from .commons import twodec, twodecname, warning_my, try_symlink, Popen_my
-from .refinement import collect_stat_OVERALL
-from .refinement import collect_stat_OVERALL_AVG
+from .commons import extract_from_file
+from .refinement import collect_stat_OVERALL, collect_stat_OVERALL_AVG
 from .refinement import collect_stat_BINNED
+from .refinement import calculate_stats_cctbx, get_f_cctbx
 from .graphs import matplotlib_bar, matplotlib_line, write_log_html
 
 
 RES_LOW = 50
 
 
 class MyArgumentParser(argparse.ArgumentParser):
@@ -263,14 +264,17 @@
     # const=0.25 sets the default when there are 0 arguments
     group3.add_argument(
         '--prerefinement-no-modification', dest='no_modification',
         help="do not modify the input structure model before the complete "
         "cross-validation protocol", action='store_true')
 
     parser.add_argument(
+        '--ccp4cloud', dest='ccp4cloud', help=argparse.SUPPRESS,
+        action='store_true')
+    parser.add_argument(
         '-t', dest='test', help=argparse.SUPPRESS, action='store_true')
     parser.add_argument(
         '-q', dest='quick', help=argparse.SUPPRESS, action='store_true')
 
     # If the arguments are not set correctly, show help and exit
     if (input_args == [__file__]) or \
        (input_args == [os.path.basename(__file__)]) or \
@@ -414,24 +418,29 @@
         sys.exit(1)
 
     # Decide which refinement software will be used
     if args.phenix:
         refinement = "phenix"
         refinement_name = "phenix.refine"
         from .refinement import refinement_phenix
-        from .refinement import collect_stat_binned_phenix_low
+        # from .refinement import collect_stat_binned_phenix_low
     else:
         refinement = "refmac"  # REFMAC5 as default
         refinement_name = "REFMAC5"
         from .refinement import refinement_refmac
         from .refinement import collect_stat_binned_refmac_low
     settings["sh"] = False
     if args.phenix and platform.system() == 'Windows':
         settings["sh"] = True
 
+    versions_dict = {"refmac_version": "N/A",  # It will be found later
+                     "phenix_version": "N/A",  # It will be found now
+                     "phenix_subversion": "N/A",  # It will be found now
+                     "pairef_version": __version__}
+
     # Check of the needed executables - works only on Linux or Windows
     if platform.system() == 'Linux' or platform.system() == 'Windows':
         if refinement == "refmac":  # CCP4 & REFMAC5
             cryst_package = "CCP4 Software Suite"
             required_executables = ["refmac5", "baverage", "mtzdump", "sfcheck"]
             ## if args.update_waters:
             ##     required_executables.append("findwaters")
@@ -439,14 +448,21 @@
             cryst_package = "PHENIX software suite"
             if platform.system() == 'Linux':
                 required_executables = ["phenix.refine"]
             else:
                 required_executables = []  # just skip the check
             # modules: from xia2.Wrappers.CCP4.Mtzdump import Mtzdump
             #          iotbx
+            #
+            with open("phenix_version.txt", 'w') as out:
+                p = Popen_my(["phenix.version"], stdout=out, stderr=out, shell=settings["sh"])
+                p.communicate()
+            versions_dict["phenix_version"] = extract_from_file(
+                "phenix_version.txt", "ersion", 0, 1, nth_word=-1)
+            settings["phenix_subversion"] = int(versions_dict["phenix_version"].split(".")[1])
         for required_executable in required_executables:
             if not which(required_executable) and not args.test:
                 sys.stderr.write("ERROR: PAIREF requires installed `"
                                  "" + required_executable + "` (a part "
                                  "of the " + cryst_package + ") but it is not "
                                  "executable."
                                  "\nAborting.\n")
@@ -469,18 +485,14 @@
     # Create new working directory (name related to the project)
     workdir = create_workdir(args.project)
 
     # Set to write STDOUT to screen and file
     writer = output_log(sys.stdout, workdir + '/PAIREF_out.log')
     sys.stdout = writer
 
-    versions_dict = {"refmac_version": "N/A",  # It will be found later
-                     "phenix_version": "N/A",  # It will be found later
-                     "pairef_version": __version__}
-
     # Show information about the module and input parameters
     welcome(args, versions_dict["pairef_version"])
 
     # Find resolution range of merged data
     res_low, res_high_mtz = res_from_mtz(args.hklin)  # uses CCTBX
     if not res_high_mtz:
         sys.stderr.write("ERROR: High-resolution limit of data "
@@ -651,15 +663,15 @@
                                         args=args,
                                         n_bins=n_bins_low,
                                         mode="first",
                                         res_low=res_low,
                                         res_highest=shells[-1],
                                         flag=flag,
                                         xyzin_start=xyzin_start)
-            versions_dict["phenix_version"] = results["version"]
+            # versions_dict["phenix_version"] = results["version"]
         collect_stat_OVERALL([res_cur], args, flag, refinement)
         if args.complete_cross_validation or args.prerefinement_ncyc:
             matplotlib_line(
                 shells=[shells[0]],
                 project=args.project,
                 statistics=["Rwork_cyc", "Rfree_cyc"],
                 n_bins_low=n_bins_low,
@@ -699,18 +711,25 @@
             "_at_" + twodecname(shells[0]) + "A.log"
         mtzfilename = \
             args.project + "_R" + str(flag_sets[0]).zfill(2) + "_" \
             "" + twodecname(shells[0]) + "A.mtz"
         bins_low = collect_stat_binned_refmac_low(
             logfilename, mtzfilename, args.hklin, n_bins_low, res_low, flag)[1]
     elif refinement == "phenix":
-        pdbfilename = args.project + "_R" + str(flag_sets[0]).zfill(2) + "_" \
-            "" + twodecname(shells[0]) + "A_comparison" \
-            "_at_" + twodecname(shells[0]) + "A_001.pdb"
-        bins_low = collect_stat_binned_phenix_low(pdbfilename, n_bins_low)[0]
+        mtzfilename = \
+            args.project + "_R" + str(flag_sets[0]).zfill(2) + "_" \
+            "" + twodecname(shells[0]) + "A_001.mtz"
+        fobs, fmodel, flags = get_f_cctbx(mtzfilename)
+        bins_low = \
+                calculate_stats_cctbx(fobs, fmodel, flags, n_bins=n_bins_low, bins=True)
+        # pdbfilename = args.project + "_R" + str(flag_sets[0]).zfill(2) + "_" \
+        #     "" + twodecname(shells[0]) + "A_comparison" \
+        #     "_at_" + twodecname(shells[0]) + "A_001.pdb"
+        # bins_low = collect_stat_binned_phenix_low(pdbfilename, n_bins_low)[0]
+        # bins_low = [float(bin) for bin in bins_low]
     bins_low = [float(bin) for bin in bins_low]
     if not args.complete_cross_validation:
         collect_stat_BINNED([res_cur], args.project, args.hklin,
                                    n_bins_low, flag, res_low, refinement)
         if which("sfcheck"):
             res_opt(shells[0], args, refinement)
             matplotlib_line(shells=[shells[0]],
```

### Comparing `pairef-1.3.9/docs/_static/example_R-values.png` & `pairef-1.4.0/docs/_static/example_R-values.png`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/_static/phenix_command_prompt.gif` & `pairef-1.4.0/docs/_static/phenix_command_prompt.gif`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/_static/example_CCfree.png` & `pairef-1.4.0/docs/_static/example_CCfree.png`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/_static/ccp4console.gif` & `pairef-1.4.0/docs/_static/ccp4console.gif`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/list_of_functions.rst` & `pairef-1.4.0/docs/list_of_functions.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/make.bat` & `pairef-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/gui.rst` & `pairef-1.4.0/docs/gui.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/index.rst` & `pairef-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/installation.rst` & `pairef-1.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/using.rst` & `pairef-1.4.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/test.rst` & `pairef-1.4.0/docs/test.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/Makefile` & `pairef-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/conf.py` & `pairef-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/docs/credits.rst` & `pairef-1.4.0/docs/credits.rst`

 * *Files identical despite different names*

### Comparing `pairef-1.3.9/LICENSE` & `pairef-1.4.0/LICENSE`

 * *Files identical despite different names*

