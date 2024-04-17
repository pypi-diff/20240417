# Comparing `tmp/mpl_data_cast-0.6.2.tar.gz` & `tmp/mpl_data_cast-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_data_cast-0.6.2.tar", last modified: Sat Jan  6 13:00:00 2024, max compression
+gzip compressed data, was "mpl_data_cast-0.6.3.tar", last modified: Wed Apr 17 12:08:47 2024, max compression
```

## Comparing `mpl_data_cast-0.6.2.tar` & `mpl_data_cast-0.6.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.454723 mpl_data_cast-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.458723 mpl_data_cast-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.462723 mpl_data_cast-0.6.2/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/MPLDataCast.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/MPLDataCast.ico
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/MPLDataCastLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/MPLDataCastLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/hook-mpl_data_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/macos_MPLDataCast.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/win_MPLDataCast.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/win_make_iss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/build-recipes/win_mpl-data-cast.iss_dummy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.462723 mpl_data_cast-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.462723 mpl_data_cast-0.6.2/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/artwork/mpldc_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/artwork/mpldc_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/artwork/mpldc_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.466723 mpl_data_cast-0.6.2/docs/scrots/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/scrots/make_scrots_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/scrots/ui_main.png
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/scrots/ui_preferences.png
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/sec_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/sec_gui.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/docs/sec_intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.466723 mpl_data_cast-0.6.2/mpl_data_cast/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.466723 mpl_data_cast-0.6.2/mpl_data_cast/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/mpl_data_cast/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/mpl_data_cast/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28754 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/img/mpldc_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/main.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_tree.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_catchall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_oah.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_qlsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/mpl_data_cast/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-06 13:00:00.000000 mpl_data_cast-0.6.2/mpl_data_cast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:00:00.470723 mpl_data_cast-0.6.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   116686 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/data/rcp_rtdc_mask-contour_2018.zip
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/test_gui_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/test_gui_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/test_rcp_catchall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/test_rcp_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-01-06 12:59:50.000000 mpl_data_cast-0.6.2/tests/test_recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.568480 mpl_data_cast-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.572480 mpl_data_cast-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.572480 mpl_data_cast-0.6.3/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCast.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCast.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCastLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCastLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/hook-mpl_data_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_MPLDataCast.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_MPLDataCast.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_make_iss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_mpl-data-cast.iss_dummy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/scrots/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/make_scrots_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/ui_main.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/ui_preferences.png
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_gui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/mpl_data_cast/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/mpl_data_cast/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28754 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/mpldc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_catchall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_oah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_qlsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   116686 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/data/rcp_rtdc_mask-contour_2018.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_gui_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_gui_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_rcp_catchall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_rcp_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_recipe.py
```

### Comparing `mpl_data_cast-0.6.2/.github/workflows/check.yml` & `mpl_data_cast-0.6.3/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/.github/workflows/deploy_github.yml` & `mpl_data_cast-0.6.3/.github/workflows/deploy_github.yml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/.github/workflows/deploy_pypi.yml` & `mpl_data_cast-0.6.3/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/.gitignore` & `mpl_data_cast-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/CHANGELOG` & `mpl_data_cast-0.6.3/CHANGELOG`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.6.3
+ - fix: cleanup temporary directories on startup (#29)
+ - fix: avoid possible name clashes when storing logs in DC output file
+ - enh: warn user when source and target directory are identical (#28)
 0.6.2
  - setup: bump dclab from 0.55.7 to 0.57.0
 0.6.1
  - enh: compute the hash of the input file a second time while waiting
    for the hash of the target file
 0.6.0
  - feat: generalize GUI to use all recipes
```

### Comparing `mpl_data_cast-0.6.2/LICENSE` & `mpl_data_cast-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/PKG-INFO` & `mpl_data_cast-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_data_cast
-Version: 0.6.2
+Version: 0.6.3
 Summary: convert and transfer data to network shares
 Author: Benedikt Hartmann, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL v3
 Project-URL: source, https://github.com/GuckLab/MPL-Data-Cast
 Project-URL: tracker, https://github.com/GuckLab/MPL-Data-Cast/issues
 Project-URL: documentation, https://mpl-data-cast.readthedocs.io
@@ -13,18 +13,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click>=8
-Requires-Dist: dclab>=0.57.0
+Requires-Dist: dclab>=0.58.2
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: hdf5plugin
 Requires-Dist: numpy>=1.21
+Requires-Dist: psutil
 Requires-Dist: pyqt6
 Requires-Dist: tifffile==2022.3.16
 
 |MPL-Data-Cast|
 ===============
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
```

### Comparing `mpl_data_cast-0.6.2/README.rst` & `mpl_data_cast-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/MPLDataCast.icns` & `mpl_data_cast-0.6.3/build-recipes/MPLDataCast.icns`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/MPLDataCast.ico` & `mpl_data_cast-0.6.3/build-recipes/MPLDataCast.ico`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/Readme.md` & `mpl_data_cast-0.6.3/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/hook-mpl_data_cast.py` & `mpl_data_cast-0.6.3/build-recipes/hook-mpl_data_cast.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/macos_MPLDataCast.spec` & `mpl_data_cast-0.6.3/build-recipes/macos_MPLDataCast.spec`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/macos_build_app.sh` & `mpl_data_cast-0.6.3/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/win_MPLDataCast.spec` & `mpl_data_cast-0.6.3/build-recipes/win_MPLDataCast.spec`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/win_make_iss.py` & `mpl_data_cast-0.6.3/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/build-recipes/win_mpl-data-cast.iss_dummy` & `mpl_data_cast-0.6.3/build-recipes/win_mpl-data-cast.iss_dummy`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/artwork/mpldc_icon.svg` & `mpl_data_cast-0.6.3/docs/artwork/mpldc_icon.svg`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/artwork/mpldc_splash.png` & `mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/artwork/mpldc_splash.svg` & `mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.svg`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/conf.py` & `mpl_data_cast-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/scrots/ui_main.png` & `mpl_data_cast-0.6.3/docs/scrots/ui_main.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/scrots/ui_preferences.png` & `mpl_data_cast-0.6.3/docs/scrots/ui_preferences.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/sec_gui.rst` & `mpl_data_cast-0.6.3/docs/sec_gui.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/docs/sec_intro.rst` & `mpl_data_cast-0.6.3/docs/sec_intro.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/cli/cli.py` & `mpl_data_cast-0.6.3/mpl_data_cast/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/__main__.py` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/img/mpldc_icon.png` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/img/mpldc_icon.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/main.py` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
         # Recipe selection
         self.comboBox_recipe.currentIndexChanged.connect(
             self.on_recipe_changed)
 
         self.show()
         self.raise_()
+
+        # Clean up stale temporary data
+        mpldc_recipe.cleanup_tmp_dirs()
         splash.splash_close()
 
     @property
     def current_recipe(self):
         name = self.comboBox_recipe.currentData()
         return mpldc_recipe.map_recipe_name_to_class(name)
 
@@ -143,14 +146,29 @@
                                         "Input directory error",
                                         "Input directory does not exist!")
         if not self.widget_output.path.exists():
             QtWidgets.QMessageBox.error(self,
                                         "Output directory error",
                                         "Output directory does not exist!")
 
+        # Warn the user when input and output directories are identical.
+        if self.widget_input.path.samefile(self.widget_output.path):
+            ret = QtWidgets.QMessageBox.question(
+                self,
+                "Output and input directories are identical",
+                "You have selected an output directory that is identical to "
+                "the input directory. If you continue, then the files in this "
+                "directory will be <b>replaced</b> according to the recipe "
+                "you chose.<br><br>"
+                "Are you absolutely sure you would like to continue?"
+            )
+            if ret != QtWidgets.QMessageBox.StandardButton.Yes:
+                # Abort
+                return
+
         self.pushButton_transfer.setEnabled(False)
         rp = self.current_recipe(self.widget_input.path,
                                  self.widget_output.path)
 
         tree_counter = self.widget_input.tree_counter
         with CastingCallback(self, tree_counter) as path_callback:
             # run the casting operation in a separate thread
```

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/main.ui` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/main.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/preferences.py` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/preferences.ui` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_tree.py` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/gui/widget_tree.ui` & `mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/helper.py` & `mpl_data_cast-0.6.3/mpl_data_cast/helper.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_catchall.py` & `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_catchall.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_oah.py` & `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_oah.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_qlsi.py` & `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_qlsi.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/mod_recipes/rcp_rtdc.py` & `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_rtdc.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,26 @@
         # first compress the .rtdc file
         dclab.cli.compress(path_out=temp_path, path_in=path_list[0])
         # the rest of the files should be log files
         cmp_kw = hdf5plugin.Zstd(clevel=5)
         if len(path_list) > 1:
             with dclab.RTDCWriter(temp_path, compression_kwargs=cmp_kw) as hw:
                 for pp in path_list[1:]:
-                    lines = pp.read_text().split("\n")
-                    lines = [ll.rstrip() for ll in lines]
-                    hw.store_log(pp.name, lines)
+                    while True:
+                        # avoid name clashes
+                        ii = 0
+                        log_name = pp.name + f"-{ii}" if ii else pp.name
+                        if log_name in hw.h5file.get("logs", {}):
+                            ii += 1
+                            continue
+                        # write the log file
+                        lines = pp.read_text().split("\n")
+                        lines = [ll.rstrip() for ll in lines]
+                        hw.store_log(log_name, lines)
+                        break
 
     def get_raw_data_iterator(self):
         """Get list of .rtdc files including associated files"""
         for pp in self.path_raw.rglob("*.rtdc"):
             path_list = [pp]
             # search for matching SoftwareSettings.ini files
             if pp.name.startswith("M"):
```

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/recipe.py` & `mpl_data_cast-0.6.3/mpl_data_cast/recipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import hashlib
 from abc import ABC, abstractmethod
 import atexit
+import logging
+import os
 import pathlib
 import shutil
 import tempfile
 import traceback
 import uuid
 from typing import Type, Callable, List
 
+import psutil
+
 from .util import HasherThread, hashfile, copyhashfile
 
 
+logger = logging.getLogger(__name__)
+
+
 #: Files that are not copied (unless specified explicitly by a recipe)
 IGNORED_FILE_NAMES = [
     ".DS_Store",
     "._.DS_Store",
     "Thumbs.db",
 ]
 
@@ -40,16 +47,23 @@
         self.format = self.__class__.__name__
         #: Path to raw data tree
         self.path_raw = pathlib.Path(path_raw)
         #: path to target data tree
         self.path_tar = pathlib.Path(path_tar)
         if not self.path_raw.exists():
             raise ValueError(f"Raw data path '{self.path_raw}' doesn't exist!")
+        temp_root = pathlib.Path(tempfile.gettempdir()) / "MPL-Data-Cast"
+        temp_root.mkdir(exist_ok=True, parents=True)
         #: Temporary directory (will be deleted upon application exit)
-        self.tempdir = pathlib.Path(tempfile.mkdtemp(prefix="MPL-Data-Cast_"))
+        self.tempdir = pathlib.Path(
+            # Use the current PID as an identifier for the temp dir
+            tempfile.mkdtemp(
+                prefix=f"PID-{os.getpid()}-{self.format}_",
+                dir=temp_root))
+        # Make sure everything is removed in the end.
         atexit.register(shutil.rmtree, self.tempdir, ignore_errors=True)
 
     def cast(self, path_callback: Callable = None, **kwargs) -> dict:
         """Cast the entire data tree to the target directory
 
         Parameters
         ----------
@@ -250,14 +264,44 @@
                 # deleting it.
                 target_path.unlink(missing_ok=True)
         if success and delete_after:
             temp_path.unlink(missing_ok=True)
         return success
 
 
+def cleanup_tmp_dirs():
+    """Removes stale temporary recipe directories"""
+    # In versions <=0.6.2 of MPL-Data-Cast, the temporary files were located
+    # here (If a user installed a newer version of MPL-Data-Cast, then
+    # we can in any case safely remove these directories):
+    for pp in pathlib.Path(tempfile.gettempdir()).glob("MPL-Data-Cast_*"):
+        if pp.is_dir():
+            shutil.rmtree(pp, ignore_errors=True)
+
+    # New versions of MPL-Data-Cast, we have this temporary directory for
+    # recipes:
+    temp_dir = pathlib.Path(tempfile.gettempdir()) / "MPL-Data-Cast"
+    if temp_dir.is_dir():
+        for pp in temp_dir.glob("PID-*"):
+            try:
+                if pp.is_dir():
+                    # Every subdirectory is named according to PID of its
+                    # process. If the process does not exist anymore, we
+                    # may delete it.
+                    pid = int(pp.name.split("-")[1])
+                    print(pp, pid, psutil.pid_exists(pid))
+                    if not psutil.pid_exists(pid):
+                        shutil.rmtree(pp, ignore_errors=True)
+            except BaseException:
+                logger.warning(
+                    f"Could not remove stale data {pp} from PID {pid}:\n"
+                    f"{traceback.format_exc()}"
+                )
+
+
 def get_available_recipe_names() -> list[str]:
     names = []
     for cls in Recipe.__subclasses__():
         names.append(map_class_to_recipe_name(cls))
     return sorted(names)
```

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast/util.py` & `mpl_data_cast-0.6.3/mpl_data_cast/util.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast.egg-info/PKG-INFO` & `mpl_data_cast-0.6.3/mpl_data_cast.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_data_cast
-Version: 0.6.2
+Version: 0.6.3
 Summary: convert and transfer data to network shares
 Author: Benedikt Hartmann, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL v3
 Project-URL: source, https://github.com/GuckLab/MPL-Data-Cast
 Project-URL: tracker, https://github.com/GuckLab/MPL-Data-Cast/issues
 Project-URL: documentation, https://mpl-data-cast.readthedocs.io
@@ -13,18 +13,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click>=8
-Requires-Dist: dclab>=0.57.0
+Requires-Dist: dclab>=0.58.2
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: hdf5plugin
 Requires-Dist: numpy>=1.21
+Requires-Dist: psutil
 Requires-Dist: pyqt6
 Requires-Dist: tifffile==2022.3.16
 
 |MPL-Data-Cast|
 ===============
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
```

### Comparing `mpl_data_cast-0.6.2/mpl_data_cast.egg-info/SOURCES.txt` & `mpl_data_cast-0.6.3/mpl_data_cast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/pyproject.toml` & `mpl_data_cast-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,19 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Intended Audience :: Science/Research',
 ]
 license = {text = "GPL v3"}
 dependencies = [
     "click>=8",
-    "dclab>=0.57.0",
+    "dclab>=0.58.2",
     "h5py>=3.8.0",
     "hdf5plugin",  # compression
     "numpy>=1.21",  # CVE-2021-33430
+    "psutil",
     "pyqt6",
     "tifffile==2022.3.16",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 mpldc-gui = "mpl_data_cast.gui.__main__:main"
```

### Comparing `mpl_data_cast-0.6.2/tests/data/rcp_rtdc_mask-contour_2018.zip` & `mpl_data_cast-0.6.3/tests/data/rcp_rtdc_mask-contour_2018.zip`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/tests/test_gui_basic.py` & `mpl_data_cast-0.6.3/tests/test_gui_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/tests/test_gui_rtdc.py` & `mpl_data_cast-0.6.3/tests/test_gui_rtdc.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,35 +31,37 @@
     """Check that data is transfered when clicking on the button 'Transfer'."""
     mw = MPLDataCast()
     qtbot.addWidget(mw)
     QtWidgets.QApplication.setActiveWindow(mw)
     QtTest.QTest.qWait(100)
 
     data = retrieve_data("rcp_rtdc_mask-contour_2018.zip")
-    test_file = data / "M001_data.rtdc"
-    test_file_dst = tmp_path / "M001_data.rtdc"
-    shutil.copy(test_file, test_file_dst)
-    tmp_dir = tf.TemporaryDirectory()
-    path_out = pathlib.Path(tmp_dir.name)
-    assert tmp_path.exists()
-    assert path_out.exists()
+    tmp_in = tmp_path / "in"
+    tmp_in.mkdir()
+    tmp_out = tmp_path / "out"
+    tmp_out.mkdir()
 
-    mw.widget_input.path = tmp_path
-    mw.widget_output.path = path_out
+    shutil.copytree(data, tmp_in, dirs_exist_ok=True)
+
+    assert tmp_in.is_dir()
+    assert tmp_out.is_dir()
+
+    mw.widget_input.path = tmp_in
+    mw.widget_output.path = tmp_out
 
     bt = mw.pushButton_transfer
 
     # Monkeypatch message box to always return OK
     monkeypatch.setattr(QtWidgets.QMessageBox,
                         "information",
                         lambda *args: QtWidgets.QMessageBox.StandardButton.Ok)
     qtbot.mouseClick(bt, QtCore.Qt.MouseButton.LeftButton)
 
-    assert (path_out / "M001_data.rtdc").exists()
-    tmp_dir.cleanup()
+    assert (tmp_out / "M001_data.rtdc").exists()
+
     mw.close()
     QtTest.QTest.qWait(100)
     QtWidgets.QApplication.processEvents(
         QtCore.QEventLoop.ProcessEventsFlag.AllEvents, 5000)
 
 
 def test_transfer_data_advanced(qtbot, tmp_path, monkeypatch):
```

### Comparing `mpl_data_cast-0.6.2/tests/test_rcp_catchall.py` & `mpl_data_cast-0.6.3/tests/test_rcp_catchall.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/tests/test_rcp_rtdc.py` & `mpl_data_cast-0.6.3/tests/test_rcp_rtdc.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.2/tests/test_recipe.py` & `mpl_data_cast-0.6.3/tests/test_recipe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import atexit
 import hashlib
+import os
 import pathlib
+import shutil
 import tempfile
+import uuid
 
-from mpl_data_cast import Recipe
+from mpl_data_cast import Recipe, cleanup_tmp_dirs
 
 
 def make_example_data():
     td = pathlib.Path(tempfile.mkdtemp())
     d1 = td / "hans" / "peter"
     d1.mkdir(parents=True, exist_ok=True)
     d2 = td / "fliege"
@@ -36,14 +40,48 @@
             if pp.is_dir():
                 files = sorted(pp.rglob("*.txt"))
                 if files:
                     data_list.append(files)
         return sorted(data_list)
 
 
+def test_cleanup_recipes_new():
+    td = pathlib.Path(tempfile.gettempdir()) / "MPL-Data-Cast"
+    mypid = os.getpid()
+
+    dir1 = td / f"PID-{mypid}-Something_else"
+    dir2 = td / "PID-32769-Something_else"
+
+    atexit.register(shutil.rmtree, dir1, ignore_errors=True)
+    atexit.register(shutil.rmtree, dir2, ignore_errors=True)
+
+    dir1.mkdir(exist_ok=True, parents=True)
+    path1 = dir1 / "a.txt"
+    path1.write_text("should not be deleted")
+
+    dir2.mkdir(exist_ok=True, parents=True)
+    path2 = dir2 / "a.txt"
+    path2.write_text("should be deleted")
+
+    cleanup_tmp_dirs()
+
+    assert path1.exists()
+    assert not path2.exists()
+
+
+def test_cleanup_recipes_old():
+    td = pathlib.Path(tempfile.gettempdir()) / f"MPL-Data-Cast_{uuid.uuid4()}"
+    td.mkdir(parents=True, exist_ok=True)
+    path = td / "data.dat"
+    path.write_text("hello world")
+    assert path.exists()
+    cleanup_tmp_dirs()
+    assert not path.exists()
+
+
 def test_pipeline_init():
     path_raw = make_example_data()
     path_tar = pathlib.Path(tempfile.mkdtemp()) / "test"
     pl = DummyRecipe(path_raw, path_tar)
     assert pl.tempdir.exists()
     assert pl.format == "DummyRecipe"
     assert not path_tar.exists()
```

