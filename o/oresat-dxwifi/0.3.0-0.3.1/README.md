# Comparing `tmp/oresat_dxwifi-0.3.0.tar.gz` & `tmp/oresat_dxwifi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_dxwifi-0.3.0.tar", last modified: Sun Apr 14 21:02:49 2024, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.1.tar", last modified: Wed Apr 17 04:16:08 2024, max compression
```

## Comparing `oresat_dxwifi-0.3.0.tar` & `oresat_dxwifi-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.603958 oresat_dxwifi-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/build-deb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.603958 oresat_dxwifi-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/docs/images/hgs-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/docs/images/olaf-browser.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/kill-olaf
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-dxwifi-software-server.service
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-mon-iface.service
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-vcan-iface.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/configs/camera_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/oresat_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/templates/oresat_live.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/configs/transmission_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/startmonitor.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/tx_module.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/start-vcan
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/startmonitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.703329 oresat_dxwifi-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.687329 oresat_dxwifi-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.691329 oresat_dxwifi-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-17 04:16:08.703329 oresat_dxwifi-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.687329 oresat_dxwifi-0.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.691329 oresat_dxwifi-0.3.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.691329 oresat_dxwifi-0.3.1/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.695329 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.703329 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:16:08.703329 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 04:16:08.000000 oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:16:08.703329 oresat_dxwifi-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-17 04:15:59.000000 oresat_dxwifi-0.3.1/startmonitor.sh
```

### Comparing `oresat_dxwifi-0.3.0/.github/workflows/pypi.yaml` & `oresat_dxwifi-0.3.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/.gitignore` & `oresat_dxwifi-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/LICENSE` & `oresat_dxwifi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/PKG-INFO` & `oresat_dxwifi-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.0
+Version: 0.3.1
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oresat-config
+Requires-Dist: oresat-configs
 Requires-Dist: oresat-olaf>=3.0.0
 
 # Table of Contents:
 - [Table of Contents:](#table-of-contents)
 - [oresat-dxwifi-software](#oresat-dxwifi-software)
   - [Install prerequisites on compatible system](#install-prerequisites-on-compatible-system)
   - [Set up source directories](#set-up-source-directories)
```

### Comparing `oresat_dxwifi-0.3.0/README.md` & `oresat_dxwifi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/build-deb.sh` & `oresat_dxwifi-0.3.1/build-deb.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/docs/images/hgs-browser.png` & `oresat_dxwifi-0.3.1/docs/images/hgs-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/docs/images/olaf-browser.png` & `oresat_dxwifi-0.3.1/docs/images/olaf-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/__main__.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/camera/CMakeLists.txt` & `oresat_dxwifi-0.3.1/oresat_dxwifi/camera/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/camera/README.md` & `oresat_dxwifi-0.3.1/oresat_dxwifi/camera/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/camera/frame.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/camera/frame.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/camera/interface.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/camera/interface.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/resources/temperature.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/resources/temperature.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/services/oresat_live.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/services/oresat_live.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif` & `oresat_dxwifi-0.3.1/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/templates/oresat_live.html` & `oresat_dxwifi-0.3.1/oresat_dxwifi/templates/oresat_live.html`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/configs/transmission_configs.yaml` & `oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/configs/transmission_configs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/defaults.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/defaults.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/startmonitor.sh` & `oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/startmonitor.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/transmission.py` & `oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/transmission.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/tx_module.so` & `oresat_dxwifi-0.3.1/oresat_dxwifi/transmission/tx_module.so`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/PKG-INFO` & `oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.0
+Version: 0.3.1
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oresat-config
+Requires-Dist: oresat-configs
 Requires-Dist: oresat-olaf>=3.0.0
 
 # Table of Contents:
 - [Table of Contents:](#table-of-contents)
 - [oresat-dxwifi-software](#oresat-dxwifi-software)
   - [Install prerequisites on compatible system](#install-prerequisites-on-compatible-system)
   - [Set up source directories](#set-up-source-directories)
```

### Comparing `oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/SOURCES.txt` & `oresat_dxwifi-0.3.1/oresat_dxwifi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.0/pyproject.toml` & `oresat_dxwifi-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Embedded Systems",
 ]
 dependencies = [
-    "oresat-config",
+    "oresat-configs",
     "oresat-olaf>=3.0.0",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 oresat-c3 = "oresat_dxwifi.__main__:main"
```

### Comparing `oresat_dxwifi-0.3.0/startmonitor.sh` & `oresat_dxwifi-0.3.1/startmonitor.sh`

 * *Files identical despite different names*

