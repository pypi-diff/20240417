# Comparing `tmp/endaq-device-1.1.1.tar.gz` & `tmp/endaq_device-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endaq-device-1.1.1.tar", last modified: Fri Dec 15 06:01:02 2023, max compression
+gzip compressed data, was "endaq_device-1.2.0.tar", last modified: Wed Apr 17 18:02:22 2024, max compression
```

## Comparing `endaq-device-1.1.1.tar` & `endaq_device-1.2.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.466871 endaq-device-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-15 06:00:55.000000 endaq-device-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2023-12-15 06:01:02.466871 endaq-device-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-15 06:00:55.000000 endaq-device-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.454871 endaq-device-1.1.1/endaq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.458871 endaq-device-1.1.1/endaq/device/
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52073 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   100569 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/command_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    55315 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/configio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/endaq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/hdlc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/response_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.458871 endaq-device-1.1.1/endaq/device/schemata/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/schemata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18426 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/schemata/command-response.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/schemata/flash_package.xml
--rw-r--r--   0 runner    (1001) docker     (127)    51363 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/schemata/mide_config_ui.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27598 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/schemata/mide_manifest.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/slamstick.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.462871 endaq-device-1.1.1/endaq/device/ui_defaults/
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_025G_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_02kG_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_100G_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_500G_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0003_016G.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0003_200G.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0004_02kG_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0004_500G_DC.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/S2_D40D200.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/S2_D8D16.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/S4_D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/S5_E2000D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/S5_E25D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E100D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E2000D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E25D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8324 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E500D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R100D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R2000D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R500D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/W8_E100D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/W8_E2000D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/W8_E25D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/Wx_D40.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/ui_defaults/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2023-12-15 06:00:55.000000 endaq-device-1.1.1/endaq/device/win.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.462871 endaq-device-1.1.1/endaq_device.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2023-12-15 06:01:02.000000 endaq-device-1.1.1/endaq_device.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-15 06:01:02.000000 endaq-device-1.1.1/endaq_device.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 06:01:02.000000 endaq-device-1.1.1/endaq_device.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-15 06:01:02.000000 endaq-device-1.1.1/endaq_device.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-15 06:01:02.000000 endaq-device-1.1.1/endaq_device.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-12-15 06:00:55.000000 endaq-device-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 06:01:02.466871 endaq-device-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-12-15 06:00:55.000000 endaq-device-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:01:02.462871 endaq-device-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-12-15 06:00:55.000000 endaq-device-1.1.1/tests/test__basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-12-15 06:00:55.000000 endaq-device-1.1.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-12-15 06:00:55.000000 endaq-device-1.1.1/tests/test_config_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.518255 endaq_device-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-17 18:02:18.000000 endaq_device-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-17 18:02:22.518255 endaq_device-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 18:02:18.000000 endaq_device-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.506255 endaq_device-1.2.0/endaq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.510255 endaq_device-1.2.0/endaq/device/
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58385 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125059 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/command_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56138 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/configio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/devinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/endaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/hdlc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/response_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.510255 endaq_device-1.2.0/endaq/device/schemata/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/schemata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20988 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/schemata/command-response.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/schemata/flash_package.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    51363 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/schemata/mide_config_ui.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27598 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/schemata/mide_manifest.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/slamstick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.514255 endaq_device-1.2.0/endaq/device/ui_defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_025G_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_02kG_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_100G_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_500G_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0003_016G.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0003_200G.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0004_02kG_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0004_500G_DC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/S2_D40D200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/S2_D8D16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/S4_D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/S5_E2000D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/S5_E25D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_D16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_D8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E100D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E2000D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E25D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E500D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R100D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R2000D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R500D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/W8_E100D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/W8_E2000D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/W8_E25D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/Wx_D40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/ui_defaults/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-17 18:02:18.000000 endaq_device-1.2.0/endaq/device/win.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.514255 endaq_device-1.2.0/endaq_device.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-17 18:02:22.000000 endaq_device-1.2.0/endaq_device.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 18:02:22.000000 endaq_device-1.2.0/endaq_device.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:02:22.000000 endaq_device-1.2.0/endaq_device.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 18:02:22.000000 endaq_device-1.2.0/endaq_device.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 18:02:22.000000 endaq_device-1.2.0/endaq_device.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 18:02:18.000000 endaq_device-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:02:22.518255 endaq_device-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-17 18:02:18.000000 endaq_device-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:02:22.514255 endaq_device-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-17 18:02:18.000000 endaq_device-1.2.0/tests/test__basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-17 18:02:18.000000 endaq_device-1.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-17 18:02:18.000000 endaq_device-1.2.0/tests/test_config_basic.py
```

### Comparing `endaq-device-1.1.1/LICENSE` & `endaq_device-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/PKG-INFO` & `endaq_device-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: endaq-device
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python API for enDAQ data recorders
 Home-page: https://github.com/MideTechnology/endaq-device
 Author: Mide Technology
 Author-email: help@mide.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MideTechnology/endaq-device/issues
 Project-URL: Documentation, https://mide-technology-endaq-device.readthedocs-hosted.com/en/latest/
 Project-URL: Source Code, https://github.com/MideTechnology/endaq-device
 Keywords: endaq configure recorder hardware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `endaq-device-1.1.1/README.md` & `endaq_device-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/__init__.py` & `endaq_device-1.2.0/endaq/device/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,98 @@
 """
 Functions for detecting, identifying, and retrieving information about
 data-logging devices.
 """
 
 __author__ = "David Stokes"
+__copyright__ = "Copyright 2024 Mide Technology Corporation"
 
+import logging
 import os
 from pathlib import Path
 import string
-from typing import List, Optional, Union
+from threading import RLock
+from typing import Dict, List, Optional, Union
+from weakref import WeakValueDictionary
 
 import ebmlite.core
 from idelib.dataset import Dataset
 
 from .base import Recorder, os_specific
+from .command_interfaces import SerialCommandInterface
+from .devinfo import SerialDeviceInfo
 from .exceptions import *
 from .endaq import EndaqS, EndaqW
+from .response_codes import DeviceStatusCode
 from .slamstick import SlamStickX, SlamStickC, SlamStickS
 from .types import Drive, Filename, Epoch
 
-from . import schemata
+logger = logging.getLogger('endaq.device')
+# logger.setLevel(logging.DEBUG)
 
-__version__ = "1.1.1"
+# ============================================================================
+#
+# ============================================================================
+
+__version__ = "1.2.0"
 
 __all__ = ('CommandError', 'ConfigError', 'ConfigVersionError',
            'DeviceError', 'DeviceTimeout', 'UnsupportedFeature',
            'deviceChanged', 'findDevice', 'fromRecording',
            'getDevices', 'getRecorder', 'isRecorder', 'onRecorder',
            'Recorder', 'EndaqS', 'EndaqW', 'SlamStickX', 'SlamStickC',
            'SlamStickS')
 
-#===============================================================================
+# ============================================================================
 # EBML schema path modification
-#===============================================================================
+# ============================================================================
 
 SCHEMA_PATH = "{endaq.device}/schemata"
 
 # Ensure the `idelib` schemata are in the schema path (for idelib <= 3.2.4)
 if "{idelib}/schemata" not in ebmlite.core.SCHEMA_PATH:
     ebmlite.core.SCHEMA_PATH.insert(0, "{idelib}/schemata")
 
 # Add this package's schema to `ebmlite` schema search path, after
 # `idelib`'s. This is a workaround for issue with legacy schema installed by
 # earlier versions (can probably be removed after beta).
 if SCHEMA_PATH not in ebmlite.core.SCHEMA_PATH:
     _idx = ebmlite.core.SCHEMA_PATH.index("{idelib}/schemata") + 1
     ebmlite.core.SCHEMA_PATH.insert(_idx, SCHEMA_PATH)
 
-#===============================================================================
+# ============================================================================
 #
-#===============================================================================
+# ============================================================================
 
 # Known classes or recorder. Checks are performed in the specified order, so
 # put the ones with more general `isRecorder()` methods (i.e. superclasses)
 # after the more specific ones. `SlamStickC` is first, since it is now sold
 # as Sx-D16 but has the old SlamStick hardware, but the naming convention
 # matches that of `EndaqS`. The base `Recorder` should be last.
 RECORDER_TYPES = [SlamStickC, EndaqS, EndaqW, SlamStickS, SlamStickX, Recorder]
 
 # Cache of previously seen recorders, to prevent redundant instantiations.
 # Keyed by the hash of the recorders DEVINFO (or equivalent).
 RECORDERS = {}
 
+# Another cache of recorders, keyed by serial number. Used when discovering
+# remote devices that don't immediately have DEVINFO accessible.
+RECORDERS_BY_SN = WeakValueDictionary()
+
 # Max number of cached recorders. Probably not needed, but just in case.
 RECORDER_CACHE_SIZE = 100
 
-#===============================================================================
-# Platform-specific stuff. 
-#===============================================================================
+# Lock to prevent contention (primarily with the recorder cache). Several
+# classes have their own 'busy' locks as well.
+_module_busy = RLock()
+
 
+# ============================================================================
+# Platform-specific stuff. 
+# ============================================================================
 
 def getRecorder(path: Filename,
                 update: bool = False,
                 strict: bool = True) -> Union[Recorder, None]:
     """ Get a specific recorder by its path.
 
         :param path: The filesystem path to the recorder's root directory.
@@ -81,43 +101,49 @@
             after a device reset).
         :param strict: If `False`, only the directory structure within `path`
             is used to identify a recorder. If `True`, non-FAT file systems
             will be automatically rejected.
         :return: An instance of a :class:`~.endaq.device.Recorder` subclass,
             or `None` if the path is not a recorder.
     """
-    global RECORDERS
+    global RECORDERS, RECORDERS_BY_SN
 
     dev = None
 
-    for rtype in RECORDER_TYPES:
-        if rtype.isRecorder(path, strict=strict):
-            # Get existing recorder if it has already been instantiated.
-            devhash = rtype._getHash(path)
-            dev = RECORDERS.pop(devhash, None)
-            if not dev:
-                dev = rtype(path, strict=strict)
-
-            if devhash:
-                RECORDERS[devhash] = dev
-
-                # Path has changed. Note that the hash does not include
-                # path, in case a device rebooted and remounted with a
-                # different mount point/drive letter.
-                if update and dev.path != path:
-                    dev.path = path
+    with _module_busy:
+        for rtype in RECORDER_TYPES:
+            if rtype.isRecorder(path, strict=strict):
+                # Get existing recorder if it has already been instantiated.
+                devhash = rtype._getHash(path)
+                dev = RECORDERS.pop(devhash, None)
+                if not dev:
+                    dev = rtype(path, strict=strict)
+                else:
+                    # Clear DEVINFO-getter, in case device was previously remote
+                    dev._devinfo = None
+
+                if devhash:
+                    RECORDERS[devhash] = dev
+
+                    # Path has changed. Note that the hash does not include
+                    # path, in case a device rebooted and remounted with a
+                    # different mount point/drive letter.
+                    if update and dev.path != path:
+                        dev.path = path
+
+                RECORDERS_BY_SN[dev.serialInt] = dev
+
+                break
+
+        # Remove old cached devices. Ordered dictionaries assumed!
+        if len(RECORDERS) > RECORDER_CACHE_SIZE:
+            for k in list(RECORDERS.keys())[-RECORDER_CACHE_SIZE:]:
+                del RECORDERS[k]
 
-            break
-
-    # Remove old cached devices. Ordered dictionaries assumed!
-    if len(RECORDERS) > RECORDER_CACHE_SIZE:
-        for k in list(RECORDERS.keys())[:-RECORDER_CACHE_SIZE]:
-            del RECORDERS[k]
-
-    return dev
+        return dev
 
 
 def deviceChanged(recordersOnly: bool = True,
                   clear: bool = False) -> bool:
     """ Returns `True` if a drive has been connected or disconnected since
         the last call to :meth:`~.endaq.device.deviceChanged`.
         
@@ -128,63 +154,78 @@
         :param clear: If `True`, clear the cache of previously-detected
             drives and devices.
     """
     return os_specific.deviceChanged(recordersOnly, RECORDER_TYPES, clear=clear)
 
 
 def getDeviceList(strict: bool = True) -> List[Drive]:
-    """ Get a list of data recorders, as their respective path (or the drive
-        letter under Windows).
+    """ Get a list of local data recorders, as their respective path (or the
+        drive letter under Windows).
 
         :param strict: If `False`, only the directory structure is used
             to identify a recorder. If `True`, non-FAT file systems will
             be automatically rejected.
         :return: A list of `Drive` objects (named tuples containing the
             drive path, label, and other low-level filesystem info).
     """
     return os_specific.getDeviceList(RECORDER_TYPES, strict=strict)
 
 
 def getDevices(paths: Optional[List[Filename]] = None,
-               update: bool = False,
+               unmounted: bool = True,
+               update: bool = True,
                strict: bool = True) -> List[Recorder]:
     """ Get a list of data recorder objects.
     
         :param paths: A list of specific paths to recording devices.
             Defaults to all found devices (as returned by
             :meth:`~.endaq.device.getDeviceList`).
+        :param unmounted: If `True`, include devices connected by USB
+            and responsive to commands but not appearing as drives.
+            Note: Not all devices/firmware versions support this.
         :param update: If `True`, update the path of known devices if they
             have changed (e.g., their drive letter or mount point changed
             after a device reset).
         :param strict: If `False`, only the directory structure is used
             to identify a recorder. If `True`, non-FAT file systems and
             non-removable media will be automatically rejected.
         :return: A list of instances of `Recorder` subclasses.
     """
-    global RECORDERS
+    global RECORDERS, RECORDERS_BY_SN
 
-    if paths is None:
-        paths = getDeviceList(strict=strict)
-    else:
-        if isinstance(paths, (str, bytes, bytearray, Path)):
-            paths = [paths]
-
-    result = []
-
-    for path in paths:
-        dev = getRecorder(path, update=update, strict=strict)
-        if dev is not None:
-            result.append(dev)
+    with _module_busy:
+        if paths is None:
+            paths = getDeviceList(strict=strict)
+        else:
+            if isinstance(paths, (str, bytes, bytearray, Path)):
+                paths = [paths]
+
+        result = set()
+
+        for path in paths:
+            dev = getRecorder(path, update=update, strict=strict)
+            if dev is not None:
+                result.add(dev)
+
+        if unmounted:
+            for dev in getSerialDevices(known=RECORDERS_BY_SN):
+                if not dev.available:
+                    dev.path = None
+                result.add(dev)
+                RECORDERS.pop(hash(dev), None)
+                RECORDERS[hash(dev)] = dev
+                RECORDERS_BY_SN[dev.serialInt] = dev
 
-    return result
+        return sorted(result, key=lambda x: x.path or '\uffff')
 
 
 def findDevice(sn: Optional[Union[str, int]] = None,
                chipId: Optional[Union[str, int]] = None,
                paths: Optional[List[Filename]] = None,
+               unmounted: bool = False,
                update: bool = False,
                strict: bool = True) -> Union[Recorder, None]:
     """ Find a specific recorder by serial number or unique chip ID. One or
         the other must be provided, but not both. Note that early firmware
         versions do not report the device's chip ID.
 
         :param sn: The serial number of the recorder to find. Cannot be used
@@ -194,62 +235,67 @@
             with `sn`. It can be an integer or a hex string. Note that
             `chipId` cannot be used to find SlamStick and older enDAQ S
             devices (prior to hardware revision 2.0), as they do not report
             their chip ID.
         :param paths: A list of specific paths to recording devices.
             Defaults to all found devices (as returned by
             :meth:`~.endaq.device.getDeviceList`).
+        :param unmounted: If `True`, include devices connected by USB
+            and responsive to commands but not appearing as drives.
+            Note: Not all devices/firmware versions support this.
         :param update: If `True`, update the path of known devices if they
             have changed (e.g., their drive letter or mount point changed
             after a device reset).
         :param strict: If `False`, only the directory structure is used
             to identify a recorder. If `True`, non-FAT file systems will
             be automatically rejected.
         :return: An instance of a :class:`~.endaq.device.Recorder` subclass
             representing the device with the specified serial number or chip
             ID, or `None` if it cannot be found.
     """
-    if sn and chipId:
-        raise ValueError('Either a serial number or chip ID is required, not both')
-    elif sn is None and chipId is None:
-        raise ValueError('Either a serial number or chip ID is required')
-
-    if isinstance(sn, str):
-        sn = sn.lstrip(string.ascii_letters+"0")
-        if not sn:
-            sn = 0
-        sn = int(sn)
-
-    if isinstance(chipId, str):
-        chipId = int(chipId, 16)
+    with _module_busy:
+        if sn and chipId:
+            raise ValueError('Either a serial number or chip ID is required, not both')
+        elif sn is None and chipId is None:
+            raise ValueError('Either a serial number or chip ID is required')
+
+        if isinstance(sn, str):
+            sn = sn.lstrip(string.ascii_letters+"0")
+            if not sn:
+                sn = 0
+            sn = int(sn)
+
+        if isinstance(chipId, str):
+            chipId = int(chipId, 16)
+
+        for d in getDevices(paths, update=update, strict=strict, unmounted=unmounted):
+            if d.serialInt == sn or d.chipId == chipId:
+                return d
 
-    for d in getDevices(paths, update=update, strict=strict):
-        if d.serialInt == sn or d.chipId == chipId:
-            return d
-
-    return None
+        return None
 
 
-#===============================================================================
+# ============================================================================
 # 
-#===============================================================================
+# ============================================================================
 
 def isRecorder(path: Filename,
                strict: bool = True) -> bool:
     """ Determine if the given path is a recording device.
 
         :param path: The filesystem path to check.
         :param strict: If `False`, only the directory structure within `path`
             is used to identify a recorder. If `True`, non-FAT file systems
             will be automatically rejected.
     """
-    for t in RECORDER_TYPES:
-        if t.isRecorder(path, strict=strict):
-            return True
-    return False
+    with _module_busy:
+        for t in RECORDER_TYPES:
+            if t.isRecorder(path, strict=strict):
+                return True
+        return False
 
 
 def onRecorder(path: Filename, strict: bool = True) -> bool:
     """ Returns the root directory of a recorder from a path to a directory or
         file on that recorder. It can be used to test whether a file is on
         a recorder. `False` is returned if the path is not on a recorder.
         The test is only whether the path refers to a recorder, not whether
@@ -273,21 +319,80 @@
         path = os.path.dirname(path)
     return False
 
 
 def fromRecording(doc: Dataset) -> Recorder:
     """ Create a 'virtual' recorder from the data contained in a recording
         file.
+
+        :param doc: An imported IDE recording. Note that very old IDE files
+            may not contain the metadata requires to create a `virtual`
+            device.
     """
     productName = doc.recorderInfo.get('ProductName')
     if not productName:
         productName = doc.recorderInfo.get('PartNumber')
     if productName is None:
-        raise TypeError("Could not create virtual recorder from file (no ProductName)")
+        raise TypeError("Could not create virtual recorder from file "
+                        "(no ProductName or PartNumber in metadata)")
     recType = None
     for rec in RECORDER_TYPES:
         if rec._matchName(productName):
             recType = rec
             break
     if recType is None:
         return None
     return recType.fromRecording(doc)
+
+
+# ============================================================================
+# 
+# ============================================================================
+
+def getSerialDevices(known: Optional[Dict[int, Recorder]] = None,
+                     strict: bool = True) -> List[Recorder]:
+    """ Find all recorders with a serial command interface (and firmware
+        that supports retrieving device metadata via that interface).
+
+        :param known: A dictionary of known `Recorder` instances, keyed by
+            device serial number.
+        :param strict: If `True`, check the USB serial port VID and PID to
+            see if they belong to a known type of device.
+        :return: A list of `Recorder` instances found.
+    """
+    if known is None:
+        known = {}
+
+    devices = []
+
+    # Dummy recorder and command interface to retrieve DEVINFO
+    fake = Recorder(None)
+    fake.command = SerialCommandInterface(fake)
+
+    for port, sn in SerialCommandInterface._possibleRecorders(strict=strict):
+        if sn in known:
+            devices.append(known[sn])
+            continue
+
+        fake.command.port = None
+        fake._snInt, fake._sn = sn, str(sn)
+
+        with _module_busy:
+            try:
+                logger.debug(f'Getting info for SN {sn} via serial')
+                info = fake.command._getInfo(0, index=False)
+                if not info:
+                    logger.debug(f'No info returned by SN {sn}, continuing')
+                    continue
+                for devtype in RECORDER_TYPES:
+                    if devtype._isRecorder(info):
+                        device = devtype(None, devinfo=info)
+                        device.command = SerialCommandInterface(device)
+                        device._devinfo = SerialDeviceInfo(device)
+                        devices.append(device)
+                        break
+            except CommandError as err:
+                if err.errno != DeviceStatusCode.ERR_INVALID_COMMAND:
+                    logger.debug(f'Unexpected {type(err).__name__} getting info for {sn}: {err}')
+                continue
+
+    return devices
```

### Comparing `endaq-device-1.1.1/endaq/device/base.py` & `endaq_device-1.2.0/endaq/device/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Items common to all recorder types. Separate from module's `__init__.py` to
 eliminate circular dependencies.
 """
 
 __author__ = "dstokes"
-__copyright__ = "Copyright 2023 Mide Technology Corporation"
 
 from collections import defaultdict
 from datetime import datetime, timedelta
+import errno
 import logging
 import os
 from pathlib import Path
 import re
-import struct
 import sys
 from threading import RLock
 from time import struct_time
-from typing import Any, AnyStr, Callable, Dict, Optional, Tuple, Union
+from typing import Any, AnyStr, Callable, Dict, List, Optional, Tuple, Union
 import warnings
 
-from idelib.dataset import Dataset, Channel
+from idelib.dataset import Dataset, Channel, SubChannel, Sensor
 from idelib import importer
 from idelib.parsers import CalibrationListParser, RecordingPropertiesParser
 from idelib.transforms import Transform
 
 import ebmlite
 from ebmlite import MasterElement, loadSchema
 
@@ -32,30 +31,33 @@
 elif 'win' in sys.platform:
     from . import win as os_specific
 elif sys.platform == 'linux':
     from . import linux as os_specific
 
 from . import config
 from .config import ConfigInterface
+from . import devinfo
+from .devinfo import DeviceInfo, FileDeviceInfo
 from . import measurement
 from .measurement import MeasurementType
 from . import command_interfaces
+from .command_interfaces import CommandInterface
 from .exceptions import *
 from .types import Drive, Filename, Epoch
 
 logger = logging.getLogger('endaq.device')
 
 
 __all__ = ('Recorder', 'os_specific')
 
+
 # ===============================================================================
 #
 # ===============================================================================
 
-
 class Recorder:
     """ A representation of an enDAQ/SlamStick data recorder. Some devices
         will instantiate as a specialized subclass, but the interface remains
         the same.
     """
 
     _INFO_FILE = os.path.join("SYSTEM", "DEV", "DEVINFO")
@@ -75,63 +77,112 @@
     _USERCAL_FILE = os.path.join("SYSTEM", "usercal.dat")
     _FW_UPDATE_FILE = os.path.join('SYSTEM', 'update.pkg')
     _RESPONSE_FILE = os.path.join('SYSTEM', 'DEV', 'RESPONSE')
     _BOOTLOADER_UPDATE_FILE = os.path.join("SYSTEM", 'boot.bin')
     _USERPAGE_UPDATE_FILE = os.path.join("SYSTEM", 'userpage.bin')
     _ESP_UPDATE_FILE = os.path.join('SYSTEM', 'esp32.bin')
 
-    _TIME_PARSER = struct.Struct("<L")
-
-    # TODO: This really belongs in the configuration UI
-    _POST_CONFIG_MSG = ("When ready...\n"
-                        "    1. Disconnect the recorder\n"
-                        "    2. Mount to surface\n"
-                        "    3. Press the recorder's primary button ")
-
     # These should eventually be read from the device
     SN_FORMAT = "%d"
     manufacturer = None
     homepage = None
 
     LIFESPAN = timedelta(2 * 365)
     CAL_LIFESPAN = timedelta(365)
 
     _NAME_PATTERN = re.compile(r'')
 
 
-    def __init__(self, path: Optional[Filename], strict=True):
-        """ Constructor. Typically, instantiation should be done indirectly,
-            using functions such as `endaq.device.getDevices()` or
-            `endaq.device.fromRecording()`. Explicitly instantiating a
-            `Recorder` or `Recorder` subclass is rarely (if ever) necessary.
+    def __init__(self,
+                 path: Optional[Filename],
+                 strict: bool = True,
+                 devinfo: Optional[bytes] = None,
+                 virtual: bool = False):
+        """ A representation of an enDAQ/SlamStick data recorder. Typically,
+            instantiation should be done indirectly, using functions such as
+            `endaq.device.getDevices()` or `endaq.device.fromRecording()`.
+            Explicitly instantiating a `Recorder` or `Recorder` subclass is
+            rarely (if ever) necessary.
 
             :param path: The filesystem path to the recorder, or `None` if
-                it is a 'virtual' device (e.g., constructed from data in a
-                recording).
+                it is a 'virtual' or remote device.
             :param strict: If `True`, only allow real device paths. If
-                `False`, allow any path that contains the standard contents
-                of a recorder's ``SYSTEM`` directory. Primarily for testing.
+                `False`, allow any path that contains a ``SYSTEM`` directory
+                with the standard contents on a device. Primarily for
+                testing.
+            :param devinfo: The necessary data to instantiate a `Recorder`.
+                For creating `Recorder` instances when the hardware isn't
+                physically present on the host computer. If `None`, the
+                data will be read from the device.
+            :param virtual: `True` if the device is not actual hardware
+                (e.g., constructed from data in a recording).
         """
-        # self.mideSchema = loadSchema("mide_ide.xml")
-        # self.manifestSchema = loadSchema("mide_manifest.xml")
-
         self._busy = RLock()
-        self.strict = strict
+        self.strict: bool = strict
 
-        self._command = None
-        self._path = None
-        self.refresh(force=True)
+        self._virtual: bool = virtual
+        self._command: Optional[CommandInterface] = None
+        self._config: Optional[ConfigInterface] = None
+        self._path: Optional[Filename] = None
+        self._devinfo: Optional[DeviceInfo] = None
+        self._rawinfo: Optional[bytes] = devinfo
+        self._info: Optional[Dict] = None
+
+        self._hash: Optional[int] = None
+        self._configData: Optional[Dict] = None
+        self._sn: Optional[str] = None
+        self._snInt: Optional[int] = None
+        self._chipId: Optional[int] = None
+        self._sensors: Optional[Dict[int, Sensor]] = None
+        self._channels: Optional[Dict[int, Channel]] = None
+        self._channelRanges = {}
+        self._propData: Optional[bytes] = None
+        self._manifest: Optional[Dict[str, Any]] = None
+        self._calibration: Optional[Dict[str, Any]] = None
+        self._calData: Optional[bytes] = None
+        self._calPolys: Optional[Dict[int, Any]] = None
+        self._userCalPolys: Optional[Dict] = None
+        self._userCalDict: Optional[Dict] = None
+        self._factoryCalPolys: Optional[Dict] = None
+        self._factoryCalDict: Optional[Dict] = None
+        self._properties: Optional[Dict] = None
+        self._volumeName: Optional[str] = None
+        self._wifi: Optional[str] = None  # Cached name of the manifest's Wi-Fi element
+
+        self.refresh(force=False)
         self.path = path
 
+        # XXX: Make sure this isn't necessary. It caused an infinite loop w/ hasInterface()
+        # self.getInfo()
+
         # The source IDE `Dataset` used for 'virtual' devices.
-        self._source = None
+        self._source: Optional[Dataset] = None
+
+
+    def _getDevinfo(self) -> DeviceInfo:
+        """ Retrieve the appropriate `DeviceInfo` for the `Recorder`.
+        """
+        if self._devinfo is not None:
+            return self._devinfo
+
+        elif self.isVirtual:
+            raise DeviceError('Device information cannot be read from virtual devices')
+
+        for interface in devinfo.INTERFACES:
+            if interface.hasInterface(self):
+                self._devinfo = interface(self)
+
+        if self._devinfo is None:
+            raise DeviceError('Cannot find information reader for device')
+
+        return self._devinfo
 
 
     @property
-    def command(self):
+    def command(self) -> Union[None, command_interfaces.CommandInterface]:
         """ The device's "command interface," the means through which to
             directly control the device. Only applicable to non-virtual
             recorders (i.e., actual hardware, not instantiated from a
             recording).
         """
         # This property provides the appropriate exceptions common to
         # all attempts to send commands if the device is virtual, or
@@ -150,15 +201,15 @@
                 if self._command is None:
                     raise UnsupportedFeature("Device has no command interface")
 
             return self._command
 
 
     @command.setter
-    def command(self, interface):
+    def command(self, interface: Optional[command_interfaces.CommandInterface]):
         with self._busy:
             if interface == self._command:
                 return
             if self._command is not None:
                 with self._busy:
                     self._command.close()
             self._command = interface
@@ -174,165 +225,295 @@
             return bool(self.command)
         except UnsupportedFeature:
             return False
 
 
     @property
     def available(self) -> bool:
-        """ Is the device mounted and available as a drive?
+        """ Is the device mounted and available as a drive? Note: if the
+            device's path or drive letter changed (e.g., after being rebooted
+            or disconnected/reconnected), or the device's firmware or
+            manifest was updated, you may need to call
+            :meth:`~.endaq.device.Recorder.update` first.
         """
         if self.isVirtual or not self.path:
             return False
 
         # Two checks, since former is a property that sets latter
         # and path itself isn't a reliable test in Linux
-        return (os.path.exists(self.path)
-                and os.path.isfile(self.infoFile))
+        if (os.path.exists(self.path) and os.path.isfile(self.infoFile)):
+            # See if the device is mounted in the same place and is unchanged.
+            try:
+                return self._getHash(self.path) == hash(self)
+            except IOError as err:
+                if err.errno == errno.EINVAL:
+                    # Possible race condition: device dismounts after test.
+                    logger.debug('Ignoring expected IOError (EINVAL) getting hash '
+                                 '(device dismounting?)')
+                    return False
+                raise
+
+        return False
+
+
+    def update(self,
+               virtual: bool = False,
+               paths: Optional[List[Filename]] = None,
+               strict: bool = True) -> bool:
+        """ Attempt to update the device's information. Call this method
+            if a device has had its firmware or manifest data updated. This
+            method can also be used to attempt to find the actual hardware
+            corresponding to a 'virtual' device (i.e., instantiated from
+            an IDE recording file).
+
+            :param virtual: If `True` and the recorder is a 'virtual' device,
+                attempt to connect it to the actual hardware (if present).
+            :param paths: A list of specific paths to recording devices.
+                Defaults to all found devices (as returned by
+                :meth:`~.endaq.device.getDeviceList`).
+            :param strict: If `False`, only the directory structure is used
+                to identify a recorder. If `True`, non-FAT file systems will
+                be automatically rejected.
+            :return: `True` if the device had its information updated, or
+                `False` if the device is unchanged or the hardware could
+                not be found.
+        """
+        if not virtual and self.isVirtual:
+            return False
+
+        path = self.path
+
+        # Imported here to avoid circular references.
+        # I don't like doing this, but I think this case is okay.
+        from . import RECORDERS, findDevice, _module_busy
+
+        # See if a device with the same chip ID (or serial number for older
+        # devices) can be found anywhere. This will also update the paths
+        # of known devices.
+        if self.chipId:
+            dev = findDevice(chipId=self.chipId, update=True,
+                             unmounted=True, paths=paths, strict=strict)
+        else:
+            dev = findDevice(sn=self.serialInt, update=True,
+                             unmounted=True, paths=paths, strict=strict)
+
+        if dev and dev != self:
+            # Device's DEVINFO has changed, change in place
+            with _module_busy:
+                RECORDERS[hash(dev)] = self
+                RECORDERS.pop(hash(self), None)
+                self._virtual = False
+                if dev.path != self.path:
+                    self.path = dev.path
+                self.refresh(force=True)
+                return True
+
+        return path != self.path
 
 
-    def __repr__(self):
-        path = self._path or "virtual"
+    def __repr__(self) -> str:
+        """ Return repr(self). """
+        if self.isVirtual:
+            path = "virtual"
+        else:
+            # FUTURE: Show appropriate message for remote devices
+            path = self._path or "unmounted"
+
         if self.name:
             name = '{} "{}"'.format(self.partNumber, self.name)
         else:
             name = self.partNumber
         return '<{} {} SN:{} ({})>'.format(type(self).__name__, name, self.serial, path)
 
 
     @classmethod
-    def _getHash(cls, path: Filename, info=None) -> int:
+    def _getHash(cls,
+                 path: Filename,
+                 info: Optional[bytes] = None) -> int:
         """ Calculate the device's hash. Separated from `__hash__()` so it
             can be used by `getDevices()` to find known recorders.
 
             :param path: The device's filesystem path.
             :param info: The contents of the device's `DEVINFO` file, if
                 previously loaded. For future caching optimization.
         """
-        if path and not info:
-            path = os.path.realpath(path.path if isinstance(path, Drive) else path)
-            infoFile = os.path.join(path, cls._INFO_FILE)
-            if os.path.exists(infoFile):
-                with open(infoFile, 'rb') as f:
-                    info = f.read()
-
+        if not info:
+            info = FileDeviceInfo.readDevinfo(path)
         return hash(info)
 
 
     def __hash__(self) -> int:
         """ Return hash(self). """
         with self._busy:
             if self._hash is None:
                 self.getInfo()
             return self._hash
 
 
-    def refresh(self, force=False):
+    def refresh(self, force: bool = False):
         """ Clear cached device information, ensuring the data is up-to-date.
+
+            :param force: If `True`, reread information from the device,
+                rather than use cached data.
         """
         with self._busy:
-            if self._path and not force:
-                return
+            # Data derived from DEVINFO
+            self._devinfo = None
             self._info = None
             self._hash = None
-            self._config = None
-            self._sn = None
-            self._snInt = None
-            self._chipId = None
-            self._sensors = None
-            self._channels = None
-            self._channelRanges = {}
-            self._manifest = None
-            self._calibration = None
-            self._calData = None  # Note: unlike _manData, _calData is raw
-            self._calPolys = None
-            self._userCalPolys = None
-            self._userCalDict = None
-            self._factoryCalPolys = None
-            self._factoryCalDict = None
-            self._properties = None
-            self._volumeName = None
-            self._wifi = None  # Cached name of the manifest's Wi-Fi element
+
+            if not self.isRemote:
+                # Also from DEVINFO, but required for finding remote devices.
+                # Outside of manufacturing, the device SN shouldn't change.
+                self._sn = None
+                self._snInt = None
+                self._chipId = None
+
+            if not self.isVirtual:
+                # Data derived from things virtual devices can't read; virtual
+                # devices only get a subset of this data upon instantiation
+                if force:
+                    self._rawinfo = None
+
+                self._sensors = None
+                self._channels = None
+                self._channelRanges.clear()
+                self._configData = None
+                self._propData = None
+                self._manifest = None
+                self._calibration = None
+                self._calData = None
+                self._calPolys = None
+                self._userCalPolys = None
+                self._userCalDict = None
+                self._factoryCalPolys = None
+                self._factoryCalDict = None
+                self._properties = None
+                self._volumeName = None
+                self._wifi = None
 
             if self._command:
                 try:
                     self._command.close()
                 except (AttributeError, IOError) as err:
                     logger.debug('Ignoring exception closing {}: '
                                  '{!r}'.format(self._command, err))
                 self._command = None
 
-            self._configInterface = None
+            if self._config:
+                try:
+                    self._config.close()
+                except (AttributeError, IOError) as err:
+                    logger.debug('Ignoring exception closing {}: '
+                                 '{!r}'.format(self._config, err))
+                self._config = None
 
 
     @property
     def path(self) -> Union[str, None]:
+        """ The recorder's filesystem path (e.g., drive letter or mount point).
+        """
         with self._busy:
             return self._path
 
 
     @path.setter
-    def path(self, dev: Union[Filename, None]):
+    def path(self, newpath: Union[Filename, None]):
         """ The recorder's filesystem path (e.g., drive letter or mount point).
         """
         with self._busy:
-            if dev is not None:
-                if self.strict and not self.isRecorder(dev):
+            path = None
+            self._volumeName = ''
+            self.configFile = self.infoFile = None
+            self.clockFile = self.userCalFile = self.configUIFile = None
+            self.recpropFile = self.commandFile = None
+
+            if str(newpath).lower().startswith("mqtt"):
+                path = None
+
+            elif newpath is not None:
+                newpath = newpath.path if isinstance(newpath, Drive) else newpath
+                if self.strict and not self.isRecorder(newpath):
                     raise IOError("Specified path isn't a %s: %r" %
-                                  (self.__class__.__name__, dev))
+                                  (self.__class__.__name__, newpath))
 
-                path = os.path.realpath(dev.path if isinstance(dev, Drive) else dev)
+                path = os.path.realpath(newpath)
                 self.configFile = os.path.join(path, self._CONFIG_FILE)
                 self.infoFile = os.path.join(path, self._INFO_FILE)
                 self.clockFile = os.path.join(path, self._CLOCK_FILE)
                 self.userCalFile = os.path.join(path, self._USERCAL_FILE)
                 self.configUIFile = os.path.join(path, self._CONFIG_UI_FILE)
                 self.recpropFile = os.path.join(path, self._RECPROP_FILE)
                 self.commandFile = os.path.join(path, self._COMMAND_FILE)
                 self._volumeName = None
-            else:
-                path = None
-                self._volumeName = ''
-                self.configFile = self.infoFile = None
-                self.clockFile = self.userCalFile = self.configUIFile = None
-                self.recpropFile = self.commandFile = None
 
             self._path = path
 
 
     @property
     def volumeName(self):
         """ The recorder's user-specified filesystem label. """
-        if self.isVirtual:
+        if self.isVirtual or self.isRemote:
             return False
 
-        if self._path and self._volumeName is None:
+        if self._path and os.path.exists(self._path) and self._volumeName is None:
             try:
                 self._volumeName = os_specific.getDriveInfo(self.path).label
             except (AttributeError, IOError, TypeError) as err:
                 logger.debug("Getting volumeName raised a possibly-allowed exception: %r" % err)
+
         return self._volumeName
 
 
     def __eq__(self, other) -> bool:
         """ x.__eq__(y) <==> x==y """
         if self is other:
             return True
-        return hash(self) == hash(other)
+        try:
+            return hash(self) == hash(other)
+        except TypeError:
+            return False
 
 
     @classmethod
     def _matchName(cls, name: AnyStr) -> bool:
         """ Does a given product name match this device type?
         """
         if isinstance(name, bytes):
             name = str(name, 'utf8')
         return bool(cls._NAME_PATTERN.match(name))
 
 
     @classmethod
+    def _isRecorder(cls,
+                    info: bytes) -> bool:
+        """ Test whether the given ``DEVINFO`` describes a device matching
+            this class. Used internally by `isRecorder()` and externally when
+            instantiating remote devices.
+
+            :param info: Raw device metadata, as read from a ``DEVINFO``
+                file, retrieved via a command interface, etc.
+            :return: `True` if the info is a match for this `Recorder` class.
+        """
+        try:
+            if not info:
+                return False
+            devinfo = loadSchema('mide_ide.xml').loads(info).dump()
+            name = devinfo['RecordingProperties']['RecorderInfo']['ProductName']
+            if isinstance(name, bytes):
+                # In ebmlite < 3.1, StringElements are read as bytes.
+                name = str(name, 'utf8')
+
+            return cls._matchName(name)
+        except (KeyError, IOError) as err:
+            logger.debug("_isRecorder() raised a possibly-allowed exception: %r" % err)
+            return False
+
+
+    @classmethod
     def isRecorder(cls,
                    path: Filename,
                    strict: bool = True,
                    **kwargs) -> bool:
         """ Test whether a given filesystem path refers to the root directory
             of a data recorder.
 
@@ -349,47 +530,39 @@
 
         try:
             if isinstance(path, Drive):
                 path, _volumeName, _sn, fs, _dtype = path
             else:
                 fs = ''
 
-            path = os.path.realpath(path)
-            infoFile = os.path.join(path, cls._INFO_FILE)
+            realpath = os.path.realpath(path)
+            infoFile = os.path.join(realpath, cls._INFO_FILE)
 
             if strict:
                 if not fs:
-                    info = os_specific.getDriveInfo(path)
+                    info = os_specific.getDriveInfo(realpath)
                     if not info:
                         return False
                     fs = info.fs
                 if "fat" not in fs.lower():
                     return False
 
             if 'info' in kwargs:
-                devinfo = loadSchema('mide_ide.xml').loads(kwargs['info']).dump()
+                devinfo = kwargs['info']
             elif os.path.isfile(infoFile):
-                with loadSchema('mide_ide.xml').load(infoFile) as doc:
-                    devinfo = doc.dump()
+                with open(infoFile, 'rb') as f:
+                    devinfo = f.read()
             else:
                 return False
 
-            props = devinfo['RecordingProperties']['RecorderInfo']
-            name = props['ProductName']
-            if isinstance(name, bytes):
-                # In ebmlite < 3.1, StringElements are read as bytes.
-                name = str(name, 'utf8')
-
-            return cls._matchName(name)
+            return cls._isRecorder(devinfo)
 
         except (KeyError, TypeError, AttributeError, IOError) as err:
             logger.debug("isRecorder() raised a possibly-allowed exception: %r" % err)
-            pass
-
-        return False
+            return False
 
 
     def getInfo(self,
                 name: Optional[str] = None,
                 default=None) -> Any:
         """ Retrieve a recorder's device information. Returns either a single
             item or a dictionary of all device information.
@@ -401,30 +574,34 @@
                 specific item.
             :return: If no `name` is specified, a dictionary containing the
                 device data. If a `name` is specified, the type returned will
                 vary.
         """
         mideSchema = loadSchema("mide_ide.xml")
         with self._busy:
-            if self._info is None:
-                if self.path is not None:
-                    with open(self.infoFile, 'rb') as f:
-                        data = f.read()
-                    self._hash = self._getHash(self.path, data)
-                    infoFile = mideSchema.loads(data)
+            if not self._info:
+                if not self._rawinfo:
+                    try:
+                        self._rawinfo = self._getDevinfo().readDevinfo(self.path)
+                    except DeviceError:
+                        # Serial/MQTT _getInfo() command failed
+                        # TODO: This may not be necessary, depending on how remote devices are handled (in progress)
+                        pass
+                if self._rawinfo:
+                    self._hash = hash(self._rawinfo)
+                    infoFile = mideSchema.loads(self._rawinfo)
                     try:
                         props = infoFile.dump().get('RecordingProperties', '')
-                        if 'RecorderInfo' in props:
-                            self._info = props.get('RecorderInfo', {})
-                            for k, v in self._info.items():
-                                if isinstance(v, bytes):
-                                    # Nothing in the device info should be binary,
-                                    # but as of ebmlite 3.0.1, StringElements are
-                                    # read as bytes. Convert.
-                                    self._info[k] = str(v, 'utf8')
+                        self._info = props.get('RecorderInfo', {})
+                        for k, v in self._info.items():
+                            if isinstance(v, bytes):
+                                # Nothing in the device info should be binary,
+                                # but as of ebmlite 3.0.1, StringElements are
+                                # read as bytes. Convert.
+                                self._info[k] = str(v, 'utf8')
                     except (IOError, KeyError) as err:
                         logger.debug("getInfo() raised a possibly-allowed exception: %r" % err)
                         pass
                     finally:
                         infoFile.close()
 
             if not self._hash:
@@ -443,17 +620,25 @@
             else:
                 return self._info.get(name, default)
 
 
     @property
     def isVirtual(self):
         """ Is this actual hardware, or a virtual recorder? """
-        # NOTE: This will need revision in the future if/when we have
-        #  actual recorders connected remotely by other means.
-        return self.path is None
+        return self._virtual
+
+
+    @property
+    def isRemote(self):
+        """ Is this device not directly connected to this computer? """
+        if self.isVirtual:
+            return False
+        elif not self._path:
+            return True
+        return str(self._path).lower().startswith(('mqtt',))
 
 
     @property
     def name(self) -> str:
         """ The recording device's (user-assigned) name. """
         try:
             return self.config.name
@@ -596,15 +781,15 @@
 
     
     @property
     def postConfigMsg(self) -> str:
         """ The message to be displayed after configuration. """
         if not self.isVirtual and self.config and self.config.postConfigMsg:
             return self.config.postConfigMsg
-        return self._POST_CONFIG_MSG
+        return config._POST_CONFIG_MSG
 
 
     @property
     def canRecord(self) -> bool:
         """ Can the device record on command? """
         if not self.hasCommandInterface:
             return False
@@ -618,15 +803,15 @@
         if not self.hasCommandInterface:
             return False
 
         return self.command.canCopyFirmware
 
 
     @property
-    def hasWifi(self) -> bool:
+    def hasWifi(self) -> Union[str, bool]:
         """ The name of the Wi-Fi hardware type, or `False` if none. The name
             will not be blank, so expressions like `if dev.hasWifi:` will work.
         """
         if not self.hasCommandInterface:
             return False
         if self._wifi is None:
             man = self.getManifest()
@@ -762,15 +947,15 @@
             self._channelRanges[key] = (float("%.2f" % lo), float("%.2f" % hi))
         else:
             self._channelRanges[key] = (lo, hi)
 
         return self._channelRanges[key]
 
 
-    def getAccelAxisChannels(self) -> dict:
+    def getAccelAxisChannels(self) -> Dict[int, List[SubChannel]]:
         """ Retrieve a list of all accelerometer axis subchannels, ordered
             alphabetically (X, Y, Z).
 
             :returns: A dictionary of accelerometer subchannels, keyed by
                 parent channel ID.
         """
         channels = defaultdict(list)
@@ -786,22 +971,24 @@
         """ Read the date/time from the device.
 
             :param epoch: If `True`, return the date/time as integer seconds
                 since the epoch ('Unix time'). If `False`, return a Python
                 `datetime.datetime` object.
             :return: The system time and the device time. Both are UTC.
         """
-        if self.isVirtual or not self.path:
+        if self.isVirtual:
             raise UnsupportedFeature('Virtual devices do not have clocks')
-
-        if self.hasCommandInterface:
-            return self.command.getTime(epoch=epoch)
-        else:
+        elif self.hasCommandInterface:
+            ci = self.command
+        elif self.path and os.path.exists(self.path):
             ci = command_interfaces.FileCommandInterface(self)
-            return ci.getTime(epoch=epoch)
+        else:
+            raise UnsupportedFeature(f'Cannot set time on device {self}')
+
+        return ci.getTime(epoch=epoch)
 
 
     def setTime(self,
                 t: Union[Epoch, datetime, struct_time, tuple, None] = None,
                 pause: bool = True,
                 retries: int = 1) -> Epoch:
         """ Set a recorder's date/time. A variety of standard time types are
@@ -816,22 +1003,24 @@
                 improve accuracy across multiple recorders, but may take up
                 to a second to run. Not applicable if a specific time is
                 provided (i.e. `t` is not `None`).
             :param retries: The number of attempts to make, should the first
                 fail. Random filesystem things can potentially cause hiccups.
             :return: The time that was set, as integer seconds since the epoch.
         """
-        if self.isVirtual or not self.path:
+        if self.isVirtual:
             raise UnsupportedFeature('Virtual devices do not have clocks')
-
-        if self.hasCommandInterface:
-            return self.command.setTime(t=t, pause=pause, retries=retries)
-        else:
+        elif self.hasCommandInterface:
+            ci = self.command
+        elif self.path and os.path.exists(self.path):
             ci = command_interfaces.FileCommandInterface(self)
-            return ci.setTime(t=t, pause=pause, retries=retries)
+        else:
+            raise UnsupportedFeature(f'Cannot set time on device {self}')
+
+        return ci.setTime(t=t, pause=pause, retries=retries)
 
 
     def getClockDrift(self,
                       pause: bool = True,
                       retries: int =1 ) -> float:
         """ Calculate how far the recorder's clock has drifted from the system
             time.
@@ -840,22 +1029,24 @@
                 whole-numbered second before reading the device's clock. This
                 may improve accuracy since the device's realtime clock is in
                 integer seconds.
             :param retries: The number of attempts to make, should the first
                 fail. Random filesystem things can potentially cause hiccups.
             :return: The length of the drift, in seconds.
         """
-        if self.isVirtual or not self.path:
+        if self.isVirtual:
             raise UnsupportedFeature('Virtual devices do not have clocks')
-
-        if self.hasCommandInterface:
-            return self.command.getClockDrift(pause=pause, retries=retries)
-        else:
+        elif self.hasCommandInterface:
+            ci = self.command
+        elif self.path and os.path.exists(self.path):
             ci = command_interfaces.FileCommandInterface(self)
-            return ci.getClockDrift(pause=pause, retries=retries)
+        else:
+            raise UnsupportedFeature(f'Cannot get time on device {self}')
+
+        return ci.getClockDrift(pause=pause, retries=retries)
 
 
     def _parsePolynomials(self, cal: MasterElement) -> Dict[int, Transform]:
         """ Helper method to parse CalibrationList EBML into `Transform`
             objects.
         """
         try:
@@ -865,158 +1056,110 @@
                 calPolys = {p.id: p for p in calPolys if p is not None}
             return calPolys
         except (KeyError, IndexError, ValueError) as err:
             logger.debug("_parsePolynomials() raised a possibly-allowed exception: %r" % err)
             pass
 
 
-    def _readUserpage(self) -> Union[dict, None]:
-        """ Read the device's manifest data from the EFM32 'userpage'. The
-            data is a superset of the information returned by `getInfo()`.
-            Factory calibration and recorder properties are also read
-            and cached, since one or both are in the userpage.
+    def getManifest(self) -> Union[Dict[str, Any], None]:
+        """ Read the device's manifest data. The data is a superset of the
+            information returned by `getInfo()`.
         """
-        if self._manifest is not None:
-            return self._manifest
+        # Note: This method sets `Recorder._propData`, `Recorder._manData`,
+        # `Recorder._calData`, `Recorder._manifest`, and `Recorder._calibration`.
 
-        # Recombine all the 'user page' files
-        data = bytearray()
-        for i in range(4):
-            filename = os.path.join(self.path, self._USERPAGE_FILE % i)
-            with open(filename, 'rb') as fs:
-                data.extend(fs.read())
-
-        (manOffset, manSize,
-         calOffset, calSize,
-         propOffset, propSize) = struct.unpack_from("<HHHHHH", data)
-
-        manData = data[manOffset:manOffset + manSize]
-        calData = data[calOffset:calOffset + calSize]
-
-        # _propData is read and cached here but parsed in `getSensors()`.
-        # New devices use a dynamically-generated properties file, which
-        # overrides any property data in the USERPAGE.
-        if os.path.exists(self.recpropFile):
-            with open(self.recpropFile, 'rb') as f:
-                self._propData = f.read()
-        else:
-            # Zero offset means no property data (very old devices). For new
-            # devices, a size of 1 also means no data (it's a null byte).
-            propSize = 0 if (propOffset == 0 or propSize <= 1) else propSize
-            self._propData = data[propOffset:propOffset + propSize]
-
-        try:
-            self._manData = loadSchema("mide_manifest.xml").loads(manData)
-            self._manifest = self._manData.dump().get('DeviceManifest')
-
-            self._calData = loadSchema("mide_ide.xml").loads(calData)
-            self._calibration = self._calData.dump().get('CalibrationList')
-
-        except (AttributeError, KeyError) as err:
-            logger.debug("_readUserpage() raised a possibly-allowed exception: %r" % err)
-            pass
-
-        return self._manifest
-
-
-    def _readManifest(self) -> Union[dict, None]:
-        """ Read the device's manifest data from the 'MANIFEST' file. The
-            data is a superset of the information returned by `getInfo()`.
+        with self._busy:
+            if self._manifest is not None or self.isVirtual:
+                return self._manifest
 
-            Factory calibration and recorder properties are also read and
-            cached for backwards compatibility, since both are in the older
-            devices' EFM32 'userpage'.
-        """
-        manFile = os.path.join(self.path, self._MANIFEST_FILE)
-        calFile = os.path.join(self.path, self._SYSCAL_FILE)
+            manSchema = loadSchema('mide_manifest.xml')
+            calSchema = loadSchema('mide_ide.xml')
+            manData, calData, propData = self._getDevinfo().readManifest()
 
-        try:
-            with open(manFile, 'rb') as f:
-                self._manData = loadSchema("mide_manifest.xml").loads(f.read())
-            self._manifest = self._manData.dump().get('DeviceManifest')
-        except (FileNotFoundError, AttributeError, KeyError) as err:
-            logger.debug(f"Possibly-allowed exception when reading {manFile}: {err!r}")
+            if manData:
+                self._manData = manData
+                try:
+                    self._manifest = manSchema.loads(manData)[0].dump()
+                except IndexError:
+                    logger.warning(f'No manifest data for {self}!')
+                    self._manifest = None
+            else:
+                logger.warning(f'No manifest data for {self}!')
+                self._manData = self._manifest = None
 
-        try:
-            with loadSchema("mide_ide.xml").load(calFile) as doc:
-                self._calData = doc.schema.loads(doc.getRaw())
-                self._calibration = self._calData[0].dump()
-        except (FileNotFoundError, AttributeError, IndexError) as err:
-            logger.debug(f"Possibly-allowed exception when reading {calFile}: {err!r}")
+            if calData:
+                self._calData = calSchema.loads(calData)
+                try:
+                    self._calibration = self._calData[0].dump()
+                except IndexError:
+                    logger.warning(f'No system calibration for {self}!')
+                    self._calibration = None
+            else:
+                logger.warning(f'No system calibration for {self}!')
+                self._calData = self._calibration = None
 
-        try:
-            # _propData is read and cached here but parsed in `getSensors()`.
-            # Old EFM32 recorders stored this w/ the manifest in the USERPAGE.
-            with open(self.recpropFile, 'rb') as f:
-                self._propData = f.read()
-        except (FileNotFoundError, AttributeError, KeyError) as err:
-            logger.debug(f"Possibly-allowed exception when reading {self.recpropFile}: {err!r}")
+            if propData:
+                self._propData = propData
 
-        return self._manifest
+            return self._manifest
 
 
-    def getManifest(self) -> Union[dict, None]:
-        """ Read the device's manifest data. The data is a superset of the
-            information returned by `getInfo()`.
-        """
-        with self._busy:
-            if self.isVirtual or self._manifest is not None:
-                return self._manifest
+    def _readCalFile(self,
+                     filename: Optional[Filename] = None) -> Optional[MasterElement]:
+        """ Read a file of calibration data.
+        """
+        if filename:
+            with open(filename, 'rb') as f:
+                caldata = f.read()
+        else:
+            caldata = self._getDevinfo().readUserCalibration()
 
-            if os.path.exists(os.path.join(self.path, self._MANIFEST_FILE)):
-                self._readManifest()
-            elif os.path.exists(os.path.join(self.path, self._USERPAGE_FILE % 0)):
-                self._readUserpage()
+        if caldata:
+            return loadSchema("mide_ide.xml").loads(caldata)
 
-            return self._manifest
+        return None
 
 
     def getUserCalibration(self,
-                           filename: Optional[Filename] = None) -> Union[dict, None]:
+                           filename: Optional[Filename] = None) -> Optional[Dict[str, Any]]:
         """ Get the recorder's user-defined calibration data as a dictionary
             of parameters.
         """
-        if self.isVirtual:
+        if self.isVirtual or (self._userCalDict and not filename):
             return self._userCalDict
 
-        filename = self.userCalFile if filename is None else filename
-        if filename is None or not os.path.exists(filename):
-            return None
-        if filename != self.userCalFile:
-            self._userCalDict = None
+        data = self._readCalFile(filename)
+
+        if data:
+            self._userCalDict = data.dump().get('CalibrationList', None)
 
-        if self._userCalDict is None:
-            with open(self.userCalFile, 'rb') as f:
-                d = loadSchema("mide_ide.xml").load(f).dump()
-                self._userCalDict = d.get('CalibrationList', None)
         return self._userCalDict
 
 
     def getUserCalPolynomials(self,
-                              filename: Optional[Filename] = None) -> Union[dict, None]:
+                              filename: Optional[Filename] = None) -> Union[Dict[int, Transform], None]:
         """ Get the recorder's user-defined calibration data as a dictionary
             of `idelib.transforms.Transform` subclass instances, keyed by ID.
 
             :param filename: The name of an alternative user calibration
                 `.dat` file to read (as opposed to the device's standard
                 user calibration).
         """
-        if self.isVirtual and not filename:
-            return None
+        if self.isVirtual or (self._userCalPolys and not filename):
+            return self._userCalPolys
+
+        data = self._readCalFile(filename)
+
+        if data:
+            self._userCalPolys = self._parsePolynomials(data)
 
-        filename = self.userCalFile if filename is None else filename
-        if filename is None or not os.path.exists(filename):
-            return None
-        if self._userCalPolys is None:
-            with loadSchema('mide_ide.xml').load(filename) as doc:
-                self._userCalPolys = self._parsePolynomials(doc)
         return self._userCalPolys
 
 
-    def getCalibration(self, user: bool = True) -> Union[dict, None]:
+    def getCalibration(self, user: bool = True) -> Union[Dict[str, Any], None]:
         """ Get the recorder's current calibration information. User-supplied
             calibration, if present, takes priority (as it is what will be
             applied in recordings).
 
             :param user: If `False`, ignore user calibration and return
                 factory calibration.
         """
@@ -1025,15 +1168,15 @@
             if c is not None:
                 return c
 
         self.getManifest()
         return self._calibration
 
 
-    def getCalPolynomials(self, user: bool = True) -> Union[dict, None]:
+    def getCalPolynomials(self, user: bool = True) -> Union[Dict[int, Transform], None]:
         """ Get the constructed Polynomial objects created from the device's
             current calibration data, as a dictionary of
             `idelib.transform.Transform` subclass instances, keyed by ID.
             User-supplied calibration, if present, takes priority (as it is
             what will be applied in recordings).
 
             :param user: If `False`, ignore user calibration and return
@@ -1124,37 +1267,37 @@
         data = self.getCalibration(user=user)
         if data:
             return data.get('CalibrationSerialNumber', None)
         return None
 
 
     @property
-    def transforms(self) -> Union[dict, None]:
+    def transforms(self) -> Union[Dict[int, Transform], None]:
         """ The recorder's calibration polynomials, a dictionary of
             `idelib.transform.Transform` subclass instances keyed by ID. For
             compatibility with `idelib.dataset.Dataset`; results are the
             same as `Recorder.getCalPolynomials()`.
         """
         return self.getCalPolynomials()
 
 
-    def getProperties(self) -> dict:
+    def getProperties(self) -> Dict[str, Any]:
         """ Get the raw Recording Properties from the device.
         """
         if self.isVirtual or self._properties is not None:
             return self._properties
 
         self.getManifest()
         props = loadSchema("mide_ide.xml").loads(self._propData).dump()
 
         self._properties = props.get('RecordingProperties', {})
         return self._properties
 
 
-    def getSensors(self) -> dict:
+    def getSensors(self) -> Dict[int, Sensor]:
         """ Get the recorder sensor description data.
         """
         self.getManifest()
 
         if self._sensors is not None:
             return self._sensors
 
@@ -1184,40 +1327,48 @@
             logger.debug("getSensors() raised a possibly-allowed exception: %r" % err)
             pass
 
         return self._sensors
 
 
     @property
-    def sensors(self) -> dict:
+    def sensors(self) -> Dict[int, Sensor]:
+        """ The device's sensors; a dictionary of `Sensor` objects keyed by
+            sensor ID. For compatibility with `idelib.dataset.Dataset`; results
+            are the same as `Recorder.getSensors()`.
+        """
         return self.getSensors()
 
 
     @property
-    def channels(self) -> dict:
+    def channels(self) -> Dict[int, Channel]:
+        """ The devices recording channels; a dictionary of `Channel` objects
+            keyed by channel ID. For compatibility with `idelib.dataset.Dataset`;
+            results are the same as `Recorder.getChannels(mtype=None)`.
+        """
         self.getSensors()
         return self._channels.copy()
 
 
-    def getChannels(self, mtype: Union[MeasurementType, str, None] = None) -> dict:
+    def getChannels(self, mtype: Union[MeasurementType, str, None] = None) -> Dict[int, Channel]:
         """ Get the recorder channel description data.
 
             :param mtype: An optional measurement type, to filter results.
             :return: A dictionary of `Channel` objects, keyed by channel ID.
         """
         # `getSensors()` does all the real work
         self.getSensors()
         if mtype:
             channels = measurement.filter_channels(self._channels, mtype)
             return {ch.id: ch for ch in channels}
         else:
             return self._channels.copy()
 
 
-    def getSubchannels(self, mtype: Union[MeasurementType, str, None] = None) -> dict:
+    def getSubchannels(self, mtype: Union[MeasurementType, str, None] = None) -> List[SubChannel]:
         """ Get the recorder subchannel description data.
 
             :param mtype: An optional measurement type, to filter results. See
                 `endaq.device.measurement`.
             :return: A list of `SubChannel` objects.
         """
         # `getSensors()` does all the real work
@@ -1230,15 +1381,15 @@
             channels = measurement.filter_channels(channels, mtype)
 
         return channels
 
 
     @classmethod
     def generateCalEbml(cls,
-                        transforms: dict,
+                        transforms: Union[List[Transform], Dict[int, Transform]],
                         date: Optional[int] = None,
                         expires: Optional[int] = None,
                         calSerial: int = 0) -> ebmlite.Document:
         """ Generate binary calibration data (EBML). For the keyword arguments,
             a value of `False` will simply not write the corresponding element.
 
             :param transforms: A dictionary or list of `idelib.calibration`
@@ -1265,31 +1416,33 @@
         if isinstance(calSerial, int):
             data['CalibrationSerialNumber'] = calSerial
 
         return loadSchema('mide_ide.xml').encodes({'CalibrationList': data})
 
 
     def writeUserCal(self,
-                     transforms: dict,
+                     transforms: Union[List[Transform], Dict[int, Transform]],
                      filename: Union[str, Path, None] = None):
-        """ Write user calibration to the SSX.
+        """ Write user calibration to the device.
 
             :param transforms: A dictionary or list of `idelib.calibration`
                 objects.
             :param filename: An alternate file to which to write the data,
                 instead of the standard user calibration file.
         """
         if self.isVirtual:
             raise ConfigError('Could not write user calibration data: '
                               'Not a real recorder!')
 
-        filename = self.userCalFile if filename is None else filename
         cal = self.generateCalEbml(transforms)
-        with open(filename, 'wb') as f:
-            f.write(cal)
+        if filename:
+            with open(filename, 'wb') as f:
+                f.write(cal)
+        else:
+            self._getDevinfo().writeUserCal(cal)
 
 
     # ===========================================================================
     #
     # ===========================================================================
 
     def startRecording(self,
@@ -1318,31 +1471,31 @@
 
     @property
     def config(self) -> ConfigInterface:
         """ The device's "configuration interface," the means through which to
             read and/or write device config.
         """
         with self._busy:
-            if self._configInterface is None:
+            if self._config is None:
                 for interface in config.INTERFACES:
                     if interface.hasInterface(self):
                         # logger.debug('Instantiating config interface: {!r}'.format(interface))
-                        self._configInterface = interface(self)
+                        self._config = interface(self)
                         break
 
-                if self._configInterface is None:
+                if self._config is None:
                     raise UnsupportedFeature("Device has no configuration interface")
 
-            return self._configInterface
+            return self._config
 
 
     @config.setter
     def config(self, interface: ConfigInterface):
         with self._busy:
-            self._configInterface = interface
+            self._config = interface
 
 
     @property
     def hasConfigInterface(self) -> bool:
         """ Does the device have the ability to execute commands?
         """
         try:
@@ -1356,36 +1509,43 @@
     # ===========================================================================
 
     @classmethod
     def fromRecording(cls, dataset: Dataset) -> "Recorder":
         """ Create a 'virtual' recorder from the recorder description in a
             recording.
         """
-        dev = cls(None)
-        dev._source = dataset
-        dev._info = dataset.recorderInfo.copy()
-        dev._calPolys = dataset.transforms.copy()
-        dev._channels = dataset.channels.copy()
-        dev._warnings = dataset.warningRanges.copy()
-        dev._sensors = dataset.sensors.copy()
+        rawinfo = None
+        config = configUi = None
 
         # Crawl the Dataset's EBML document for config-related data.
         # Usually pretty quick.
         for el in dataset.ebmldoc:
             if el.name.endswith('DataBlock'):
                 # End of the metadata
                 break
+            elif el.name == 'RecordingProperties':
+                rawinfo = el.getRaw()
             elif el.name.startswith('RecorderConfiguration'):
                 # This will eventually be unnecessary; see issue:
                 # https://github.com/MideTechnology/idelib/issues/112
-                dev._config = dataset.ebmldoc.schema.loads(el.getRaw())
+                config = dataset.ebmldoc.schema.loads(el.getRaw())
             elif el.name == 'ConfigUI':
                 # Proposed, but not yet in IDE files.
                 # No longer strictly required due to `ui_defaults`.
-                dev._configUi = loadSchema('mide_config_ui.xml').loads(el.value)
+                configUi = loadSchema('mide_config_ui.xml').loads(el.value)
+
+        dev = cls(None, virtual=True, devinfo=rawinfo)
+        dev._source = dataset
+        dev._devinfo = None
+        dev._calPolys = dataset.transforms.copy()
+        dev._channels = dataset.channels.copy()
+        dev._warnings = dataset.warningRanges.copy()
+        dev._sensors = dataset.sensors.copy()
+        dev._configUi = configUi
+        dev._configData = config
 
         # Datasets merge calibration info into recorderInfo; separate them.
         dev._calibration = {}
         for k in ('CalibrationDate',
                   'CalibrationExpiry',
                   'CalibrationSerialNumber'):
             v = dev._info.pop(k, None)
```

### Comparing `endaq-device-1.1.1/endaq/device/command_interfaces.py` & `endaq_device-1.2.0/endaq/device/command_interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,40 +5,44 @@
 
 import calendar
 from copy import deepcopy
 from datetime import datetime
 import errno
 import os.path
 import shutil
+import string
+import struct
 import sys
 from time import sleep, time, struct_time
-from typing import Any, AnyStr, ByteString, Dict, Optional, Tuple, Union, Callable, TYPE_CHECKING
+from typing import Any, AnyStr, Dict, Generator, List, Optional, Tuple, Union, Callable
+from uuid import uuid4
 import warnings
 
 import logging
 logger = logging.getLogger('endaq.device')
 
 from ebmlite import loadSchema
 import serial
 import serial.tools.list_ports
 
-from .exceptions import DeviceError, CommandError, DeviceTimeout, UnsupportedFeature
+from .exceptions import DeviceError, CommandError, CommunicationError, DeviceTimeout, UnsupportedFeature
 from .hdlc import hdlc_decode, hdlc_encode, HDLC_BREAK_CHAR
 from .exceptions import CRCError
-from .types import Epoch
+from .types import Epoch, Filename
 from . import response_codes
 from .response_codes import *
 
 if sys.platform == 'darwin':
     from . import macos as os_specific
 elif 'win' in sys.platform:
     from . import win as os_specific
 elif sys.platform == 'linux':
     from . import linux as os_specific
 
+from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .base import Recorder
 
 
 # ===========================================================================
 #
 # ===========================================================================
@@ -57,14 +61,16 @@
         status message string (optional).
     """
 
     # Default maximum encoded command length (bytes). Only applicable to
     # certain interfaces.
     DEFAULT_MAX_COMMAND_SIZE = None
 
+    _TIME_PARSER = struct.Struct("<L")
+
 
     def __init__(self,
                  device: "Recorder"):
         """ `CommandInterface` instances are rarely (if ever) explicitly
             created; the parent `Recorder` object will create an instance of
             the appropriate `CommandInterface` subclass when its `command`
             property is first accessed.
@@ -84,14 +90,17 @@
 
         # Last reported device status. Not available on all interfaces.
         self.status: Tuple[Optional[int], Optional[str]] = (None, None)
 
         # Some interfaces (i.e. serial) have a maximum packet size.
         self.maxCommandSize = self.DEFAULT_MAX_COMMAND_SIZE
 
+        # This host's LockID. Typically generated by `setLockID()`.
+        self.hostId: bytes = uuid4().bytes
+
 
     def __del__(self):
         # Destructor; does a bit of cleanup. Just in case.
         self.close()
 
 
     @classmethod
@@ -144,35 +153,49 @@
         :return: `True` if the connection was reset (or the interface type
             has no persistent connection).
         """
         return True
 
 
     def _encode(self, data: dict,
-                checkSize: bool = True) -> Union[bytearray, bytes]:
+                checkSize: bool = True) -> bytes:
         """
         Prepare a packet of command data for transmission, doing any
         preparation required by the interface's medium.
 
         :param data: The unencoded command `dict`.
         :param checkSize: If `False`, skip the check that the length of the
             encoded command is not greater than the device's maximum.
         :return: The encoded command data, with any class-specific
             wrapping or other preparations.
         """
         ebml = self.schema.encodes(data, headers=False)
 
-        if checkSize and self.maxCommandSize is not None and len(ebml) > self.maxCommandSize:
+        if checkSize and self.maxCommandSize and len(ebml) > self.maxCommandSize:
             raise CommandError("Command too large ({}); max size is {}".format(
                     len(ebml), self.maxCommandSize))
 
         return ebml
 
 
-    def _decode(self, packet: ByteString) -> dict:
+    def _encodeResponse(self, data: dict) -> bytearray:
+        """
+        Encode a packet of response data in the manner typically received
+        from devices, doing any preparation required by the interface's
+        medium. Only used in some special cases; not generally used in
+        ordinary "Recorder" communication.
+
+        :param data: The unencoded command `dict`.
+        :return: The encoded command data, with any class-specific
+            wrapping or other preparations.
+        """
+        return CommandInterface._encode(self, data, checkSize=False)
+
+
+    def _decode(self, packet: Union[bytearray, bytes]) -> dict:
         """
         Translate a response packet (EBML) into a dictionary.
 
         :param packet: A packet of response data, in EBML with possibly
             additional coding (varying by interface type).
         :return: The response, as nested dictionaries.
         """
@@ -183,15 +206,28 @@
         # raise IOError exceptions
         # FUTURE: Catch correct exception type after ebmlite changes (as proposed)
         except IOError as err:
             # Most common bad data error: invalid ID length
             if 'Invalid length' not in str(err):
                 raise
 
-            raise CommandError('Response from device could not be decoded ({})'.format(err))
+            raise CommunicationError('Response from device could not be decoded '
+                                     f'({err})')
+
+
+    def _decodeCommand(self, packet:Union[bytearray, bytes]) -> Dict[str, Any]:
+        """ Translate a command packet (EBML) into a dictionary. Only used in
+            some special cases; not generally used in ordinary "Recorder"
+            communication.
+
+            :param packet: A packet of command data, in EBML with possibly
+                additional coding (varying by interface type).
+            :return: The response, as nested dictionaries.
+        """
+        return CommandInterface._decode(self, packet)
 
 
     # =======================================================================
     # The actual command sending and response receiving.
     # =======================================================================
 
     def _encodeResponseCodes(self,
@@ -216,15 +252,15 @@
             except (AttributeError, TypeError):
                 logger.debug('Received unknown {}: {}'.format(name, code))
                 pass
 
         return response
 
 
-    def _writeCommand(self, packet: ByteString) -> int:
+    def _writeCommand(self, packet: Union[bytearray, bytes]) -> int:
         """
         Send an encoded EBMLCommand element. This is a low-level write; the
         data should include any transport-specific packaging. It generally
         should not be used directly.
 
         :param packet: An encoded EBMLCommand element.
         :return: The number of bytes written.
@@ -452,26 +488,41 @@
                                 callback=callback)
 
 
     def startRecording(self,
                        timeout: Union[int, float] = 5,
                        callback: Optional[Callable] = None) -> bool:
         """ Start the device recording, if supported.
-            Must be implemented in every subclass.
 
             :param timeout: Time (in seconds) to wait for a response before
                 raising a `DeviceTimeout` exception. `None` or -1 will wait
                 indefinitely.
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a
                 response will be cancelled. The callback function should
                 require no arguments.
             :returns: `True` if the command was successful.
         """
-        raise NotImplementedError
+        raise UnsupportedFeature(self, self.startRecording)
+
+
+    def stopRecording(self,
+                      timeout: Union[int, float] = 5,
+                      callback: Optional[Callable] = None):
+        """ Stop a device that is recording, if supported.
+
+            :param timeout: Time (in seconds) to wait for the recorder to
+                respond. 0 will return immediately.
+            :param callback: A function to call each response-checking
+                cycle. If the callback returns `True`, the wait for a response
+                will be cancelled. The callback function should require no
+                arguments.
+            :returns: `True` if the command was successful.
+        """
+        raise UnsupportedFeature(self, self.stopRecording)
 
 
     def reset(self,
               timeout: Union[int, float] = 5,
               callback: Optional[Callable] = None) -> bool:
         """ Reset (reboot) the recorder.
             Must be implemented in every subclass.
@@ -519,15 +570,15 @@
             support the command.
         """
         # Only interfaces that support this method will implement it.
         raise UnsupportedFeature(self, self.getBatteryStatus)
 
 
     def ping(self,
-             data: Optional[ByteString] = None,
+             data: Union[bytearray, bytes, None] = None,
              timeout: Union[int, float] = 5,
              callback: Optional[Callable] = None) -> bytes:
         """ Verify the recorder is present and responding. Not supported on
             all devices.
 
             :param data: An optional binary payload, returned by the recorder
                 verbatim.
@@ -626,26 +677,37 @@
                 sleep(0.1)
 
             timeoutMsg = timeoutMsg or "Timed out waiting for device to disconnect"
             raise DeviceTimeout(timeoutMsg)
 
 
     def awaitRemount(self,
+                     update: bool = False,
+                     paths: Optional[List[Filename]] = None,
+                     strict: bool = True,
                      timeout: Optional[Union[int, float]] = None,
-                     timeoutMsg: Optional[str] = None,
+                     interval: float = 0.125,
                      callback: Optional[Callable] = None) -> bool:
         """ Wait for the device to reappear as a drive, indicating it has
             been reconnected, completed a recording, finished firmware
             application, etc.
 
+            :param update: If `True`, attempt to update the device's
+                information. This may be required if the device has had its
+                firmware or userpage updated.
+            :param paths: For use with `update`. A list of specific paths to
+                search for the updated recording device.
+            :param strict: For use with `update`. If `True`, non-FAT file
+                systems will be automatically rejected when searching for the
+                updated recording device.
             :param timeout: Time (in seconds) to wait for the recorder to
                 respond. 0 will return immediately; `None` or -1 will wait
                 indefinitely.
-            :param timeoutMsg: A command-specific message to use when raising
-                a `DeviceTimeout` exception.
+            :param interval: Time (in seconds) between checks for the
+                remounted device.
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a
                 response will be cancelled. The callback function should
                 require no arguments.
             :return: `True` if the device reappeared. `False` if it is a
                 virtual device, or the wait was cancelled by the callback.
         """
@@ -657,20 +719,21 @@
 
         with self.device._busy:
             timeout = -1 if timeout is None else timeout
             deadline = time() + timeout
             while timeout < 0 or time() < deadline:
                 if callback is not None and callback():
                     return False
-                elif self.device.available:
+                if update:
+                    self.device.update(paths=paths, strict=strict)
+                if self.device.available:
                     return True
-                sleep(0.1)
+                sleep(interval)
 
-            timeoutMsg = timeoutMsg or "Timed out waiting for device to remount"
-            raise DeviceTimeout(timeoutMsg)
+            raise DeviceTimeout("Timed out waiting for device to remount")
 
 
     def _updateAll(self,
                    secure: True,
                    wait: bool = True,
                    timeout: Union[int, float] = 10,
                    callback: Optional[Callable] = None) -> bool:
@@ -812,15 +875,16 @@
 
             # Use 'secure' if the device FW update is a .pkg, or it has keys installed.
             secure = bool(isPkg or keyRev)
 
             return self._updateAll(secure=secure, timeout=timeout, callback=callback)
 
 
-    def setKeys(self, keys: ByteString,
+    def setKeys(self,
+                keys: Union[bytearray, bytes],
                 timeout: Union[int, float] = 5,
                 callback: Optional[Callable] = None):
         """ Update the device's key bundle
 
             :param keys: The key data.
             :param timeout: Time (in seconds) to wait for the recorder to
                 respond. 0 will return immediately. `None` or -1 will wait
@@ -971,15 +1035,15 @@
 
         if response is None:
             return None
 
         return self._encodeResponseCodes(response.get('QueryWiFiResponse'))
 
 
-    def scanWifi(self, 
+    def scanWifi(self,
                  timeout: Union[int, float] = 10,
                  interval: float = .25,
                  callback: Optional[Callable] = None) -> Union[None, list]:
         """ Initiate a scan for Wi-Fi access points (APs). Applicable only
             to devices with Wi-Fi hardware.
 
             The resluts are returned as a list of dictionaries, one for each
@@ -1180,14 +1244,124 @@
             except (TypeError, ValueError) as err:
                 warnings.warn("{} parsing IP address: {}"
                               .format(type(err).__name__, err))
 
         return mac, ip
 
 
+    # =======================================================================
+    # Lock ID: A weakly-enforced means of claiming exclusive use of a device.
+    # =======================================================================
+
+    def getLockID(self, timeout: Union[int, float] = 5) -> Union[bytearray, bytes, None]:
+        """ Get the device's current lock ID, if any. Not supported by all
+            device types or firmware versions.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param timeout: Time (in seconds) to wait for a response.
+            :returns: The device's current lock ID, if any.
+        """
+        raise UnsupportedFeature(self, self.getLockID)
+
+
+    def setLockID(self,
+                  current: Union[bytearray, bytes, None] = None,
+                  new: Union[bytearray, bytes, None] = None,
+                  timeout: Union[int, float] = 5) -> Union[bytearray, bytes]:
+        """ Set a unique 'lock' ID on the device, requesting exclusive use of
+            the device.  Not supported by all devices/firmware.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param current: The lock ID currently on the device; for use if
+                the device already has a lock ID set.
+            :param new: The new lock ID. It defaults to the command
+                interface's `lockId` (generated when the `CommandInterface`
+                was instantiated, and unique to this instance).
+            :param timeout: Time (in seconds) to wait for a response.
+            :returns: The new lock ID.
+        """
+        raise UnsupportedFeature(self, self.setLockID)
+
+
+    def clearLockID(self,
+                    current: Union[bytearray, bytes, None] = None,
+                    timeout: Union[int, float] = 5) -> bool:
+        """ Clear the lock ID on the device.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param current: The lock ID currently on the device. Defaults to
+                this command interface's current lock ID (if any), but one
+                can be supplied to force a device with a different ID to
+                clear it.
+            :param timeout: Time (in seconds) to wait for a response.
+        """
+        # Same as setting with new=b'\x00\x00\x00\x00', but more user-friendly
+        raise UnsupportedFeature(self, self.clearLockID)
+
+
+    # =======================================================================
+    # General device info getting/setting
+    # =======================================================================
+
+    def _getInfo(self,
+                 index: int,
+                 timeout: Union[int, float] = 10,
+                 interval: float = .25,
+                 callback: Optional[Callable] = None,
+                  **kwargs) -> bytes:
+        """ Retrieve device system information. For 'local' devices, this
+            is retrieved via the filesystem. This method is called indirectly
+            by methods in `Recorder`. Different subclasses may have
+            additional keyword arguments.
+
+            :param index: The index of the information to retrieve.
+            :param timeout: Time (in seconds) to wait for a response before
+                raising a :class:`~.endaq.device.DeviceTimeout` exception.
+                `None` or -1 will wait indefinitely.
+            :param interval: Time (in seconds) between checks for a response.
+            :param callback: A function to call each response-checking cycle.
+                If the callback returns `True`, the wait for a response will
+                be cancelled. The callback function should require no arguments.
+            :return: The raw info, as unparsed EBML binary data. It is up to
+                the caller to know how to process the results (e.g., choose
+                the correct schema, etc.).
+        """
+        raise UnsupportedFeature(self, self._getInfo)
+
+
+    def _setInfo(self,
+                 index: int,
+                 payload: Union[bytearray, bytes],
+                 timeout: Union[int, float] = 10,
+                 interval: float = .25,
+                 callback: Optional[Callable] = None):
+        """ Write device system information. This method is called indirectly
+            by methods in `Recorder`.
+
+            :param index: The index of the information to write.
+            :param timeout: Time (in seconds) to wait for a response before
+                raising a :class:`~.endaq.device.DeviceTimeout` exception.
+                `None` or -1 will wait indefinitely.
+            :param interval: Time (in seconds) between checks for a response.
+            :param callback: A function to call each response-checking cycle.
+                If the callback returns `True`, the wait for a response will
+                be cancelled. The callback function should require no arguments.
+        """
+        raise UnsupportedFeature(self, self._setInfo)
+
+
 # ===========================================================================
 #
 # ===========================================================================
 
 class SerialCommandInterface(CommandInterface):
     """
     A mechanism for sending commands to a recorder via a serial port.
@@ -1248,14 +1422,16 @@
     @classmethod
     def hasInterface(cls, device: "Recorder") -> bool:
         """ Determine if a device supports this `CommandInterface` type.
 
             :param device: The recorder to check.
             :return: `True` if the device supports the interface.
         """
+        # Virtual devices have no CommandInterface.
+        # Remote devices get theirs through another method.
         if device.isVirtual:
             return False
 
         # If the DEVINFO explicitly indicates a serial command interface,
         # trust it.
         if device.getInfo('SerialCommandInterface') is not None:
             return True
@@ -1278,56 +1454,93 @@
         except CommandError as err:
             if 'No serial port found' in str(err):
                 return False
             raise
 
 
     @classmethod
-    def findSerialPort(cls, device: "Recorder") -> Union[None, str]:
+    def _possibleRecorders(cls,
+                           strict: bool = True) -> Generator[Tuple[str, int], None, None]:
+        """ Find all serial ports that might be `Recorder` serial command
+            interfaces.
+
+            :param strict: If `True`, check the USB serial port VID and PID
+                to see if they belong to a known type of device.
+            :yields: Tuples of port name and serial number.
+        """
+        # Find valid USB/serial device by vendor/product ID
+        for port in serial.tools.list_ports.comports():
+            sn = port.serial_number
+            if not sn or len(sn) != 8:
+               continue
+            try:
+                if strict and (port.vid, port.pid) not in cls.USB_IDS:
+                    continue
+                yield port.device, int(sn)
+            except ValueError as err:
+                # Probably text in serial number, ignore if so
+                if 'invalid literal' not in str(err).lower():
+                    raise
+
+
+    @classmethod
+    def findSerialPort(cls,
+                       device: Union["Recorder", int, str],
+                       strict: bool = True) -> Union[None, str]:
         """ Find the path/name/number of a serial port corresponding to a
             given serial number.
 
-            :param device: The recorder to check.
+            :param device: The `Recorder` to check, or a recorder serial
+                number.
+            :param strict: If `True`, check the USB serial port VID and PID
+                to see if they belong to a known type of device. If `False`,
+                only the serial number is checked.
             :return: The corresponding serial port path/name/number, or
                 `None` if no matching port is found.
         """
-        if device.isVirtual:
-            return None
+        try:
+            if device.isVirtual:
+                return None
+            devSerial = device.serialInt
+        except AttributeError:
+            if isinstance(device, int):
+                devSerial = device
+            elif isinstance(device, str):
+                sn = device.lstrip(string.ascii_letters+"0")
+                devSerial = int(sn) if sn else 0
+            else:
+                raise
 
-        for p in serial.tools.list_ports.comports():
-            # Find valid USB/serial device by vendor/product ID
-            # if (p.vid, p.pid) not in cls.USB_IDS:
-            #     continue
-            try:
-                if not p.serial_number:
-                    continue
-                sn = int(p.serial_number)
-                if sn == device.serialInt:
-                    return p.device
-            except ValueError as err:
-                # Probably text in serial number, ignore if so
-                if 'invalid literal' not in str(err).lower():
-                    raise
+        for port, sn in cls._possibleRecorders(strict=strict):
+            if sn == devSerial:
+                return port
 
 
     def getSerialPort(self,
                       reset: bool = False,
-                      **kwargs) -> Union[None, serial.Serial]:
+                      timeout: Union[int, float] = 1,
+                      kwargs: Optional[Dict[str, Any]] = None) -> Union[None, serial.Serial]:
         """
         Connect to a device's serial port.
 
         :param reset: If `True`, reset the serial connection if already open.
             Use if the path/number to the device's serial port has changed.
+        :param timeout: Time (in seconds) to get the serial port.
+        :param kwargs: Additional keyword arguments to be used when opening
+            the port. Note: these will be ignored if the port has already
+            been created and `reset` is `False`.
         :return: A `serial.Serial` instance, or `None` if no port matching
             the device can be found.
-
-        Additional keyword arguments will be used when opening the port. Note:
-        these will be ignored if the port has already been created and `reset`
-        is `False`.
         """
+        timeout = -1 if timeout is None else timeout
+        kwargs = kwargs or {}
+        kwargs.setdefault('timeout', self.timeout)
+        params = self.SERIAL_PARAMS.copy()
+        params.update(kwargs)
+
         if self.port:
             try:
                 if reset:
                     self.port.close()
                 else:
                     if not self.port.is_open:
                         self.port.open()
@@ -1337,26 +1550,42 @@
 
                     return self.port
 
             except (IOError, OSError, serial.SerialException):
                 # Disconnected device can cause this. Ignore in this case.
                 pass
 
-        portname = self.findSerialPort(self.device)
+        deadline = time() + timeout
 
-        if not portname:
-            self.port = None
-            raise CommandError('No serial port found for {}'.format(self.device))
+        while timeout < 0 or time() < deadline:
+            try:
+                portname = self.findSerialPort(self.device)
 
-        kwargs.setdefault('timeout', self.timeout)
-        params = self.SERIAL_PARAMS.copy()
-        params.update(kwargs)
+                if portname:
+                    self.port = serial.Serial(portname, **params)
+                    return self.port
+
+            except (IOError, serial.SerialException) as err:
+                # A ClearComError/PermissionError comes up while device resets
+                # (the driver doesn't immediately recognize the device is gone?)
+                # It clears after a couple of seconds; ignore it.
+                if 'ClearCommError' not in repr(err):
+                    logger.debug("Ignoring exception when opening {} (probably okay): "
+                                 "{!r}".format(type(self).__name__, err))
+
+            sleep(0.1)
+            continue
+
+        self.port = None
 
-        self.port = serial.Serial(portname, **params)
-        return self.port
+        if sys.platform == 'linux':
+            raise CommandError('No serial port found for device '
+                               "('sudo' may be required to access serial ports)")
+        else:
+            raise CommandError('No serial port found for device')
 
 
     # =======================================================================
     # The methods below are the ones shared across subclasses
     # =======================================================================
 
     def resetConnection(self) -> bool:
@@ -1376,16 +1605,20 @@
         """
         try:
             if self.port and self.port.is_open:
                 self.port.close()
                 return not self.port.is_open
         except (IOError, OSError, serial.SerialException) as err:
             # Disconnected device can cause this.
-            logger.debug("Ignoring exception when closing {} (probably okay): "
-                         "{!r}".format(type(self).__name__, err))
+            # A ClearComError/PermissionError comes up while device resets
+            # (the driver doesn't immediately recognize the device is gone?)
+            # It clears after a couple of seconds; ignore it.
+            if 'ClearCommError' not in repr(err):
+                logger.debug("Ignoring exception when closing {} (probably okay): "
+                             "{!r}".format(type(self).__name__, err))
         return True
 
 
     def _encode(self,
                 data: dict,
                 checkSize: bool = True) -> bytearray:
         """
@@ -1402,64 +1635,124 @@
         # Header: address 0 (broadcast), EBML data, immediate write.
         packet = bytearray([0x80, 0x26, 0x00, 0x0A])
         packet.extend(ebml)
         packet = hdlc_encode(packet, crc=self.make_crc)
         return packet
 
 
-    def _decode(self,
-                packet: ByteString) -> dict:
+    def _encodeResponse(self, packet: dict) -> bytearray:
         """
-            Translate a response packet into a dictionary. Removes additional
+        Encode a packet of response data in the manner typically received
+        from devices, doing any preparation required by the interface's
+        medium. Only used in some special cases; not generally used in
+        ordinary "Recorder" communication.
+
+        Note that the encoded results may not exactly match those generated
+        by a device, as the enDAQ firmware uses fixed lengths for element
+        size indicators some cases.
+
+        :param packet: The unencoded command `dict`.
+        :return: The encoded command data, with any class-specific
+            wrapping or other preparations.
+        """
+        ebml = super()._encodeResponse(packet)
+        responseCode = 0
+
+        # Header: address 1 (host), EBML data, immediate write.
+        packet = bytearray([0x81, 0x00, responseCode])
+        packet.extend(ebml)
+        packet = hdlc_encode(packet, crc=self.make_crc)
+        return packet
+
+
+    def _decode(self,
+                packet: bytearray) -> Dict[str, Any]:
+        """ Translate a response packet into a dictionary. Removes additional
             header data and checks the CRC (if the interface's `ignore_crc`
             attribue is `False`) before parsing the binary EBML contents.
 
             :param packet: A packet of response data.
             :return: The response, as nested dictionaries.
         """
-        # Testing note: because response headers differ from commands, this
-        # method cannot directly decode a packet created by `encode()`.
-
         # Messages are Corbus packets:
         # HDLC escaped short header, payload, crc16
         packet = hdlc_decode(packet, ignore_crc=self.ignore_crc)
         if packet.startswith(b'\x81\x00'):
             resultcode = packet[2]
             if resultcode == 0:
                 return super()._decode(packet[3:-2])
             else:
                 errname = {0x01: "Corbus command failed",
                            0x07: "bad Corbus command"}.get(resultcode, "unknown error")
-                raise CommandError("Response header indicated an error (0x{:02x}: {})".format(resultcode, errname))
+                raise CommandError(f"Response header indicated an error "
+                                   f"(0x{resultcode:02x}: {errname})")
         else:
-            raise CommandError('Response was corrupted or incomplete; did not have expected Corbus header')
+            raise CommunicationError('Response was corrupted or incomplete; '
+                                     'did not have expected Corbus header')
+
+
+    def _decodeCommand(self, packet: Union[bytearray, bytes]) -> Dict[str, Any]:
+        """ Translate a command packet (EBML) into a dictionary. Only used in
+            some special cases; not generally used in ordinary "Recorder"
+            communication.
+
+            :param packet: A packet of command data, in EBML with possibly
+                additional coding (varying by interface type).
+            :return: The command, as nested dictionaries.
+        """
+        packet = hdlc_decode(packet, ignore_crc=self.ignore_crc)
+        if packet.startswith(b'\x80\x26\x00\x0A'):
+            return super()._decodeCommand(packet[4:-2])
+        else:
+            raise CommunicationError('Received command was corrupted or incomplete; '
+                                     'did not have expected Corbus header')
 
 
     def _writeCommand(self,
-                      packet: ByteString) -> int:
+                      packet: Union[bytearray, bytes],
+                      timeout: Union[int, float] = 0.5) -> int:
         """ Transmit a fully formed packet (addressed, HDLC encoded, etc.)
             via serial. This is a low-level write to the medium and does not
             do the additional housekeeping that `sendCommand()` does;
             typically, it should not be used directly.
 
             :param packet: The encoded, packetized, binary `EBMLCommand`
                 data.
             :return: The number of bytes written.
         """
-        port = self.getSerialPort()
+        timeout = -1 if timeout is None else timeout
+        deadline = time() + timeout
 
-        if port.in_waiting:
-            logger.debug('Flushing {} bytes from serial input'.format(port.in_waiting))
-            port.flushInput()
+        while timeout < 0 or time() < deadline:
+            try:
+                port = self.getSerialPort()
+
+                if port.in_waiting:
+                    logger.debug('Flushing {} bytes from serial input'.format(port.in_waiting))
+                    port.reset_input_buffer()
+
+                return port.write(packet)
+
+            except (IOError, OSError, serial.SerialException) as err:
+                # A ClearComError/PermissionError comes up while device resets
+                # (the driver doesn't immediately recognize the device is gone?)
+                # It clears after a couple of seconds; ignore it.
+                if 'ClearCommError' not in repr(err):
+                    logger.debug("Ignoring exception when closing {} (probably okay): "
+                                 "{!r}".format(type(self).__name__, err))
 
-        return port.write(packet)
+            sleep(0.1)
+            continue
+
+        return None
+        # raise TimeoutError("Timed out attempting to send command via serial")
 
 
     def _readResponse(self,
-                      timeout: Optional[float] = None,
+                      timeout: Optional[float] = 0.5,
                       callback: Optional[Callable] = None) -> Union[None, dict]:
         """
         Wait for and retrieve the response to a serial command. Does not do
         any processing other than (attempting to) decode the EBML payload.
 
         :param timeout: Time to wait for a valid response. `None` or -1 will
             wait indefinitely.
@@ -1474,42 +1767,54 @@
         deadline = time() + timeout
 
         buf = b''
 
         while timeout < 0 or time() < deadline:
             if callback is not None and callback():
                 return
-            if self.port.in_waiting:
-                buf += self.port.read()
-                self._lastbuf = buf
-                if HDLC_BREAK_CHAR in buf:
-                    packet, _, buf = buf.partition(HDLC_BREAK_CHAR)
-                    if packet.startswith(b'\x81\x00'):
-                        response = self._decode(packet)
-                        self._response = time(), response
-                        if 'EBMLResponse' not in response:
-                            logger.warning('Response did not contain an EBMLResponse element')
-                        return response.get('EBMLResponse', response)
-                    else:
-                        # In the future, there might be other devices on the
-                        # bus, so a wrong header might be for a different
-                        # address. Ignore.
-                        logger.debug("Packet incomplete or has wrong header, ignoring")
-            else:
-                sleep(.01)
+            try:
+                if self.port.in_waiting:
+                    buf += self.port.read()
+                    self._lastbuf = buf
+                    if HDLC_BREAK_CHAR in buf:
+                        packet, _, buf = buf.partition(HDLC_BREAK_CHAR)
+                        if packet.startswith(b'\x81\x00'):
+                            response = self._decode(packet)
+                            self._response = time(), response
+                            if 'EBMLResponse' not in response:
+                                logger.warning('Response did not contain an EBMLResponse element')
+                            return response.get('EBMLResponse', response)
+                        else:
+                            # In the future, there might be other devices on the
+                            # bus, so a wrong header might be for a different
+                            # address. Ignore.
+                            logger.debug("Packet incomplete or has wrong header, ignoring")
+                else:
+                    sleep(.01)
 
-        raise TimeoutError("Timeout waiting for response to serial command")
+            except (IOError, OSError, serial.SerialException) as err:
+                # A ClearComError/PermissionError comes up while device resets
+                # (the driver doesn't immediately recognize the device is gone?)
+                # It clears after a couple of seconds; ignore it.
+                if 'ClearCommError' not in repr(err):
+                    logger.debug("Ignoring exception when reading response (probably okay): "
+                                 "{!r}".format(err))
+                sleep(0.1)
+
+        return None
+        # raise TimeoutError("Timeout waiting for response to serial command")
 
 
     def _sendCommand(self,
                      cmd: dict,
                      response: bool = True,
                      timeout: Union[int, float] = 10,
                      interval: float = .25,
                      index: bool = True,
+                     lock: bool = False,
                      callback: Optional[Callable] = None) -> Union[None, dict]:
         """ Send a command to the device and (optionally) retrieve the
             response.
 
             :param cmd: The command data, as a `dict` that can be encoded as
                 EBML data.
             :param response: If `True`, return a response. All serial
@@ -1519,14 +1824,16 @@
             :param timeout: Time (in seconds) to wait for a response before
                 raising a :class:`~.endaq.device.DeviceTimeout` exception.
                 `None` or -1 will wait indefinitely.
             :param interval: Time (in seconds) between checks for a
                 response. Not used by the serial interface.
             :param index: If `True` (default), include an incrementing
                 'command index' (for matching responses to commands).
+            :param lock: If `True`, include the current `hostId` in the
+                command, as some `SetInfo` commands require.
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a
                 response will be cancelled. The callback function should
                 require no arguments.
             :return: The response dictionary, or `None` if `response` is
                 `False`.
 
@@ -1535,22 +1842,25 @@
         timeout = -1 if timeout is None else timeout
         deadline = time() + timeout
 
         with self.device._busy:
             self.getSerialPort()
             try:
                 while True:
-                    if 'EBMLCommand' in cmd and index:
-                        self.index += 1
-                        cmd['EBMLCommand']['CommandIdx'] = self.index
+                    if 'EBMLCommand' in cmd:
+                        if index:
+                            self.index += 1
+                            cmd['EBMLCommand']['CommandIdx'] = self.index
+                        if lock:
+                            cmd['EBMLCommand']['LockID'] = self.hostId or (b'\x00' * 16)
 
                     packet = self._encode(cmd)
                     self.lastCommand = time(), deepcopy(cmd)
                     self._writeCommand(packet)
-            
+
                     if timeout == 0:
                         return None
 
                     try:
                         resp = self._readResponse(timeout, callback=callback)
                     except (IOError, serial.SerialException) as err:
                         # Commands that reset can cause the device to close the
@@ -1587,15 +1897,15 @@
                             EXC = CommandError if -30 <= code <= -20 else DeviceError
                             raise EXC(code, msg, self.lastCommand[1])
 
                         if queueDepth == 0:
                             logger.debug('Command queue full, retrying.')
                         else:
                             respIdx = resp.get('ResponseIdx')
-                            if respIdx == self.index:
+                            if not index or respIdx == self.index:
                                 return resp if response else None
                             else:
                                 logger.debug('Bad ResponseIdx; expected {}, got {}. '
                                              'Retrying.'.format(self.index, respIdx))
                     else:
                         queueDepth = 1
 
@@ -1645,17 +1955,17 @@
             if pause:
                 while int(t) == int(sysTime):
                     sysTime = time()
 
             response = self._sendCommand(command, timeout=timeout)
             try:
                 dt = response['ClockTime']
-                devTime = self.device._TIME_PARSER.unpack_from(dt)[0]
+                devTime = self._TIME_PARSER.unpack_from(dt)[0]
             except KeyError:
-                raise CommandError("GetClock response did not contain ClockTime")
+                raise DeviceError("GetClock response did not contain ClockTime")
 
         return sysTime, devTime
 
 
     def _setTime(self,
                  t: Optional[int] = None,
                  pause: bool = True) -> Tuple[Epoch, Epoch]:
@@ -1680,29 +1990,29 @@
             if pause:
                 # `pause` will set the time on the next second
                 t += 1
         else:
             pause = False
 
         t = int(t)
-        payload = self.device._TIME_PARSER.pack(t)
+        payload = self._TIME_PARSER.pack(t)
 
         t0 = time()
         if pause:
             while t0 < t:
                 t0 = time()
 
         self._sendCommand({'EBMLCommand': {'SetClock': payload}},
                           response=False)
 
         return t0, t
 
 
     def ping(self,
-             data: Optional[ByteString] = None,
+             data: Union[bytearray, bytes, None] = None,
              timeout: Union[int, float] = 10,
              interval: float = .25,
              callback: Optional[Callable] = None) -> dict:
         """ Verify the recorder is present and responding. Not supported on
             all devices.
 
             :param data: Optional data, which will be returned verbatim.
@@ -1718,15 +2028,15 @@
                 data sent.
         """
         cmd = {'EBMLCommand': {'SendPing': b'' if data is None else data}}
         response = self._sendCommand(cmd, timeout=timeout, interval=interval,
                                      callback=callback)
 
         if 'PingReply' not in response:
-            raise CommandError('Ping response did not contain a PingReply')
+            raise DeviceError('Ping response did not contain a PingReply')
 
         return response['PingReply']
 
 
     def blink(self,
               duration: int = 3,
               priority: int = 0,
@@ -1736,16 +2046,16 @@
             specific recorder when multiple are plugged into one computer.
             Not supported on all devices.
 
             Blinking will alternate between patterns `a` and `b` every 0.5
             seconds, continuing for the specified duration. `a` and `b`
             are unsigned 8 bit integers, in which each bit represents one
             of the recorder's LEDs:
-                * Bit 0 (LSB): Red
-                * Bit 1: Green
+                * Bit 0 (LSB): Green
+                * Bit 1: Red
                 * Bit 2: Blue
                 * Bits 3-7: Reserved for future use.
 
             :param duration: The total duration (in seconds) of the blinking,
                 maximum 255. 0 will blink without time limit, stopping when
                 the device is disconnected from USB, or when a recording is
                 started (trigger or button press).
@@ -1830,14 +2140,42 @@
                                       statusCode=DeviceStatusCode.START_PENDING,
                                       timeoutMsg="Timed out waiting for recording to start",
                                       wait=wait,
                                       timeout=timeout,
                                       callback=callback)
 
 
+    def stopRecording(self,
+                      wait: bool = True,
+                      timeout: Union[int, float] = 5,
+                      callback: Optional[Callable] = None):
+        """ Stop a device that is recording.
+
+            :param wait: If `True`, wait for the recorer to respond and/or
+                remount, indicating the recording has started.
+            :param timeout: Time (in seconds) to wait for the recorder to
+                respond. 0 will return immediately.
+            :param callback: A function to call each response-checking
+                cycle. If the callback returns `True`, the wait for a response
+                will be cancelled. The callback function should require no
+                arguments.
+            :returns: `True` if the command was successful.
+        """
+        response = self._sendCommand({'EBMLCommand': {'RecStop': {}}},
+                                     response=False,
+                                     timeout=timeout,
+                                     callback=callback)
+
+        if response is not None or not wait:
+            return True
+
+        self.awaitRemount(timeout, callback=callback)
+        return True
+
+
     def reset(self,
               wait: bool = True,
               timeout: Union[int, float] = 5,
               callback: Optional[Callable] = None) -> bool:
         """ Reset (reboot) the recorder.
 
             :param wait: If `True`, wait for the recorer to respond and/or
@@ -1930,25 +2268,214 @@
                 raise IOError('SerialCommandInterface.scanWifi() failed, and '
                               'device does not support alternative '
                               'FileCommandInterface')
 
         return self._fileinterface.scanWifi(timeout, interval, callback)
 
 
+    # =======================================================================
+    # Lock ID: A weakly-enforced means of claiming exclusive use of a device.
+    # =======================================================================
+
+    def getLockID(self,
+                  timeout: Union[int, float] = 5) -> Union[bytearray, bytes, None]:
+        """ Get the device's current lock ID, if any. Not supported by all
+            device types or firmware versions.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param timeout: Time (in seconds) to wait for a response.
+            :returns: The device's current lock ID, if any.
+        """
+        with self.device._busy:
+            cmd = {'EBMLCommand': {'GetLockID': {}}}
+
+            try:
+                response = self._sendCommand(cmd,
+                                             response=True,
+                                             timeout=timeout)
+            except CommandError as err:
+                # Older FW returns wrong status code
+                if err.errno == DeviceStatusCode.ERR_INVALID_COMMAND:
+                    raise CommandError(DeviceStatusCode.ERR_UNKNOWN_COMMAND,
+                                       *err.args[1:])
+                raise
+
+            if not response:
+                logger.debug('GetLockID did not get a response!')
+                return None
+
+            lockId = response.get('LockID', None)
+            
+            if isinstance(lockId, (bytearray, bytes)) and not any(lockId):
+                # All zeros; lock not set.
+                return None
+            elif not lockId:
+                logger.debug('GetLockID response did not contain LockID!')
+                return None
+
+            return lockId
+
+
+    def setLockID(self,
+                  current: Union[bytearray, bytes, None] = None,
+                  new: Union[bytearray, bytes, None] = None,
+                  timeout: Union[int, float] = 5) -> bool:
+        """ Set a unique 'lock' ID on the device, requesting exclusive use of
+            the device.  Not supported by all devices/firmware.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param current: The lock ID currently on the device; for use if
+                the device already has a lock ID set.
+            :param new: The new lock ID. It defaults to the command
+                interface's `lockId` (generated when the `CommandInterface`
+                was instantiated, and unique to this instance).
+            :param timeout: Time (in seconds) to wait for a response.
+            :returns: The new lock ID.
+        """
+        lockId = new or self.hostId
+        with self.device._busy:
+            cmd = {'EBMLCommand':
+                       {'SetLockID':
+                            {'CurrentLockID': current or (b'\x00' * 16),
+                             'NewLockID': lockId}}}
+
+            try:
+                self._sendCommand(cmd,
+                                  response=True,
+                                  timeout=timeout)
+            except CommandError as err:
+                # Older FW returns wrong status code
+                if err.errno == DeviceStatusCode.ERR_INVALID_COMMAND:
+                    raise CommandError(DeviceStatusCode.ERR_UNKNOWN_COMMAND,
+                                       *err.args[1:])
+                raise
+
+            return True
+
+
+    def clearLockID(self,
+                    current: Union[bytearray, bytes, None] = None,
+                    timeout: Union[int, float] = 5) -> bool:
+        """ Clear the lock ID on the device.
+
+            Lock IDs are a weakly-enforced means of requesting exclusive use
+            of a device. If a device has a lock ID set, commands sent without
+            that ID will generate an error.
+
+            :param current: The lock ID currently on the device. Defaults to
+                this command interface's current lock ID, but one
+                can be supplied to force a device with a different ID to
+                clear it.
+            :param timeout: Time (in seconds) to wait for a response.
+        """
+        # Same as setting with new=b'\x00\x00\x00...', but more user-friendly
+        with self.device._busy:
+            new = b'\00' * 16
+            current = current or self.hostId
+            result = bool(self.setLockID(new=new, current=current))
+            return result
+
+
+    # =======================================================================
+    # General device info getting/setting
+    # =======================================================================
+
+    def _getInfo(self,
+                 infoIdx: int,
+                 timeout: Union[int, float] = 10,
+                 interval: float = .25,
+                 lock: bool = False,
+                 index: bool = True,
+                 callback: Optional[Callable] = None) -> bytes:
+        """ Retrieve device system information. For 'local' devices, this
+            is retrieved via the filesystem. This method is called indirectly
+            by methods in `Recorder`.
+
+            :param infoIdx: The index of the information to retrieve.
+            :param timeout: Time (in seconds) to wait for a response before
+                raising a :class:`~.endaq.device.DeviceTimeout` exception.
+                `None` or -1 will wait indefinitely.
+            :param interval: Time (in seconds) between checks for a response.
+            :param callback: A function to call each response-checking cycle.
+                If the callback returns `True`, the wait for a response will
+                be cancelled. The callback function should require no arguments.
+            :param lock: If `True`, include the current `hostId` in the
+                command, as some `SetInfo` commands require.
+            :param index: If `True`, include a ``CommandIdx`` in the command,
+                and use it to validate the response (if any).
+            :return: The raw info, as unparsed EBML binary data. It is up to
+                the caller to know how to process the results (e.g., choose
+                the correct schema, etc.).
+        """
+        # Note: Reading config or user calibration requires a LockID
+        # lock = index in (5, 6)
+        cmd = {'EBMLCommand': {'GetInfo': infoIdx}}
+        response = self._sendCommand(cmd,
+                                     response=True,
+                                     timeout=timeout,
+                                     lock=lock,
+                                     index=index,
+                                     callback=callback)
+
+        try:
+            info = response['GetInfoResponse']['InfoPayload']
+        except KeyError:
+            if 'GetInfoResponse' in response:
+                raise DeviceError('Response did not contain expected GetInfoResponse element')
+            else:
+                raise DeviceError('Response did not contain a payload of information')
+
+        try:
+            return bytes(info)
+        except ValueError:
+            logger.debug('_getInfo() got unexpected payload: '
+                         f"{response['GetInfoResponse']['InfoPayload']!r}")
+            return info
+
+
+    def _setInfo(self,
+                 infoIdx: int,
+                 payload: Union[bytearray, bytes],
+                 timeout: Union[int, float] = 10,
+                 interval: float = .25,
+                 callback: Optional[Callable] = None):
+        """ Write device system information. This method is called indirectly
+            by methods in `Recorder`.
+
+            :param infoIdx: The index of the information to write.
+            :param timeout: Time (in seconds) to wait for a response before
+                raising a :class:`~.endaq.device.DeviceTimeout` exception.
+                `None` or -1 will wait indefinitely.
+            :param interval: Time (in seconds) between checks for a response.
+            :param callback: A function to call each response-checking cycle.
+                If the callback returns `True`, the wait for a response will
+                be cancelled. The callback function should require no arguments.
+        """
+        # TODO: Implement `SerialCommandInterface._setInfo()`!
+        #  Send command with lock=True
+        raise NotImplementedError
+
+
 # ===========================================================================
 #
 # ===========================================================================
 
 class FileCommandInterface(CommandInterface):
     """
     A mechanism for sending commands to a recorder via the `COMMAND` file.
     """
 
     def _writeCommand(self,
-                      packet: Union[AnyStr, ByteString]) -> int:
+                      packet: Union[AnyStr, bytearray]) -> int:
         """
         Send an encoded EBMLCommand element. This is a low-level write; the
         data should include any transport-specific packaging. It generally
         should not be used directly.
 
         :param packet: An encoded EBMLCommand element.
         :return: The number of bytes written.
@@ -1963,15 +2490,15 @@
     @classmethod
     def hasInterface(cls, device) -> bool:
         """ Determine if a device supports this `CommandInterface` type.
 
             :param device: The recorder to check.
             :return: `True` if the device supports the interface.
         """
-        if device.isVirtual or not device.path:
+        if device.isVirtual or device.isRemote or not device.path:
             return False
 
         # Old SlamStick devices may not support COMMAND. They should get
         # the `LegacyFileCommandInterface` because it is checked first,
         # but check anyway, just to make sure.
         if (not device.getInfo('McuType', '').startswith(('EFM32GG11', 'STM32'))
                 and device.firmwareVersion <= 19):
@@ -2044,15 +2571,15 @@
         """
         with self.device._busy:
             if pause:
                 t = int(time())
                 while int(time()) == t:
                     pass
             sysTime, devTime = os_specific.readRecorderClock(self.device.clockFile)
-            devTime = self.device._TIME_PARSER.unpack_from(devTime)[0]
+            devTime = self._TIME_PARSER.unpack_from(devTime)[0]
 
         return sysTime, devTime
 
 
     def _setTime(self,
                  t: Optional[int] = None,
                  pause: bool = True) -> Tuple[Epoch, Epoch]:
@@ -2076,15 +2603,15 @@
             t = time()
             if pause:
                 t += 1
         else:
             pause = False
 
         t = int(t)
-        payload = self.device._TIME_PARSER.pack(t)
+        payload = self._TIME_PARSER.pack(t)
 
         t0 = time()
         with open(self.device.clockFile, 'wb') as f:
             if pause:
                 while t0 < t:
                     t0 = time()
             f.write(payload)
@@ -2105,14 +2632,16 @@
             :param cmd: The raw EBML representing the command.
             :param response: If `True`, wait for and return a response.
             :param timeout: Time (in seconds) to wait for a response before
                 raising a `DeviceTimeout` exception. `None` or -1 will wait
                 indefinitely.
             :param interval: Time (in seconds) between checks for a
                 response.
+            :param index: If `True`, include a ``CommandIdx`` in the command,
+                and use it to validate the response (if any).
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a response
                 will be cancelled. The callback function should require no
                 arguments.
 
             :raise: DeviceTimeout
         """
@@ -2310,14 +2839,17 @@
     @classmethod
     def hasInterface(cls, device) -> bool:
         """ Determine if a device supports this `CommandInterface` type.
 
             :param device: The recorder to check.
             :return: `True` if the device supports the interface.
         """
+        if device.isRemote:
+            return False
+
         if device.getInfo('McuType', "EFM32GG330") != "EFM32GG330":
             return False
 
         return 17 <= device.firmwareVersion <= 19
 
 
     @property
```

### Comparing `endaq-device-1.1.1/endaq/device/config.py` & `endaq_device-1.2.0/endaq/device/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,24 @@
 logger = logging.getLogger('endaq.device')
 
 
 # ===========================================================================
 #
 # ===========================================================================
 
+# Default post-configuration message. Will (eventually) be in CONFIG.UI data.
+_POST_CONFIG_MSG = ("When ready...\n"
+                    "    1. Disconnect the recorder\n"
+                    "    2. Mount to surface\n"
+                    "    3. Press the recorder's primary button ")
+
+# ===========================================================================
+#
+# ===========================================================================
+
 class ConfigItem:
     """ A single configuration item/field, read from Config UI data, e.g., a
         device's ``CONFIG.UI`` file. It keeps track of the item's data type
         and handles conversion between internal and real-world units where
         applicable. It can also perform basic validation (minimum, maximum,
         specific valid options, etc.) if the ``CONFIG.UI`` data provides the
         required information.
@@ -455,14 +465,25 @@
         self.validate = True
 
         # The format version of the last config data read.
         self.configVersionRead = None
         self._supportedConfigVersions = None
 
 
+    def close(self) -> bool:
+        """
+        Close the interface. Only applicable to subclasses with a persistent
+        connection. Fails silently.
+
+        :return: `True` if the connection was reset (or the interface type
+            has no persistent connection).
+        """
+        return True
+
+
     @property
     def supportedConfigVersions(self):
         """ A tuple of configuration data format versions supported by
             the interface. 1 is the original SlamStick version, only
             supported on old hardware/firmware. The current version is 2.
         """
         return (2,)
@@ -497,14 +518,16 @@
     @classmethod
     def hasInterface(cls, device: "Recorder") -> bool:
         """ Determine if a device supports this `ConfigInterface` type.
 
             :param device: The Recorder to check.
             :return: `True` if the device supports the interface.
         """
+        if device.isRemote:
+            return False
         if getattr(device, "_config", None) is not None:
             return True
         return ui_defaults.getDefaultConfigUI(device) is not None
 
 
     @property
     def available(self) -> bool:
@@ -575,16 +598,16 @@
 
             :param origConfig: The unprocessed dictionary dumped from a
                 configuration EBML file.
             :param default: A dictionary of default config values.
         """
         config = {} if default is None else default.copy()
 
-        root = origConfig.get('RecorderConfigurationList', None)
-        if root is None:
+        root = origConfig.get('RecorderConfigurationList', {})
+        if not root:
             return None
 
         for item in root.get('RecorderConfigurationItem', []):
             configId = item.get('ConfigID', None)
             if not configId:
                 continue
 
@@ -1201,15 +1224,15 @@
 
 
     def getConfig(self) -> Union[Document, MasterElement]:
         """ Low-level method that retrieves the device's config EBML (e.g.,
             the contents of a real device's ``config.cfg`` file), if any.
         """
         # This will have been cached when Recorder.fromRecording() was called
-        return self.device._config
+        return self.device._configData
 
 
     def applyConfig(self, **kwargs):
         """ Apply modified configuration data to the device. Not supported on
             virtual devices!
         """
         raise UnsupportedFeature("Virtual devices cannot be configured")
@@ -1252,15 +1275,15 @@
     def hasInterface(cls, device: "Recorder") -> bool:
         """
         Determine if a device supports this `ConfigInterface` type.
 
         :param device: The Recorder to check.
         :return: `True` if the device supports the interface.
         """
-        if device.isVirtual:
+        if device.isVirtual or device.isRemote:
             return False
 
         # Very simple initial check: is there a CONFIG.UI file?
         # Unlikely to fail, but in a `try` just in case.
         try:
             if os.path.isfile(device.configUIFile):
                 return True
```

### Comparing `endaq-device-1.1.1/endaq/device/configio.py` & `endaq_device-1.2.0/endaq/device/configio.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/endaq.py` & `endaq_device-1.2.0/endaq/device/endaq.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,35 +180,30 @@
             raise UnsupportedFeature('Device has no command interface')
 
         return self.command.scanWifi(timeout=timeout, interval=interval, callback=callback)
 
 
     def updateESP32(self,
                     firmware: str,
-                    destination: Optional[str] = None,
                     timeout: float = 10,
                     callback: Optional[Callable] = None):
         """ Update the ESP32 firmware.
 
             Note: This method is deprecated. Use `recorder.command.updateESP32()`
             instead.
 
             :param firmware: The name of the ESP32 firmware package (.bin).
-            :param destination: The name of the firmware package after being
-                copied to the device, an alternative to the default.
-                Optional; primarily for testing purposes.
             :param timeout: Time (in seconds) to wait for the recorder to
                 respond. 0 will return immediately.
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a response
                 will be cancelled. The callback function should take no
                 arguments.
             :return:
         """
         # FUTURE: Remove EndaqW.updateESP32()
         warnings.warn("Direct control moved to `command` attribute; use "
                       "recorder.command.updateESP32()", DeprecationWarning)
 
         return self.command.updateESP32(firmware=firmware,
-                                        destination=destination,
                                         timeout=timeout,
                                         callback=callback)
```

### Comparing `endaq-device-1.1.1/endaq/device/exceptions.py` & `endaq_device-1.2.0/endaq/device/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 """
 Exceptions raised when interacting with a recording device.
 """
 
-__all__ = ('CommandError', 'ConfigError', 'ConfigVersionError',
-           'DeviceError', 'DeviceTimeout', 'UnsupportedFeature')
+__all__ = ('CommandError', 'CommunicationError', 'ConfigError',
+           'ConfigVersionError', 'DeviceError', 'DeviceTimeout',
+           'UnsupportedFeature')
 
 
 class DeviceError(Exception):
     """ Base class for device-related exceptions. """
+    @property
+    def errno(self):
+        if len(self.args) > 1:
+            return self.args[0]
+        return None
+
+
+class CommandError(RuntimeError, DeviceError):
+    """ Exception raised by a failure to process a command. """
+
+
+class CommunicationError(RuntimeError, DeviceError):
+    """ Exception raised by a failure to communicate. """
 
 
 class ConfigError(ValueError, DeviceError):
     """ Exception raised when configuration data is invalid.
     """
 
 
@@ -23,34 +37,33 @@
 
 class DeviceTimeout(TimeoutError, DeviceError):
     """ Exception raised when a device fails to respond within an expected
         length of time.
     """
 
 
-class CommandError(RuntimeError, DeviceError):
-    """ Exception raised by a failure to communicate. """
-
-
 class UnsupportedFeature(DeviceError):
     """ Exception raised when a device does not support a given feature
         (e.g., attempting to execute Wi-Fi commands on a device without
         Wi-Fi, or executing a command exclusive to the serial command
         interface over the file-based interface).
 
         Intended to be instantiated with either a single argument (a message
         string) or with two (the object raising the exception, and the
         offending method).
     """
+    @property
+    def errno(self):
+        return None
 
     def __str__(self):
         try:
             if len(self.args) == 2:
-                return "{} does not support {}".format(type(self.args[0]).__name__,
-                                                       self.args[1].__name__)
+                return "{}.{}".format(type(self.args[0]).__name__,
+                                      self.args[1].__name__)
         except (AttributeError, IndexError, TypeError):
             pass
 
         return super().__str__()
 
 
 class CRCError(ValueError):
```

### Comparing `endaq-device-1.1.1/endaq/device/hdlc.py` & `endaq_device-1.2.0/endaq/device/hdlc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 HDLC encoding and checksum-related code.
 
 In this application, 'HDLC encoding' amounts to using HDLC escaping and
 break characters.
 """
-from typing import ByteString, Union
+from typing import Union
 
 from logging import getLogger
 logger = getLogger('endaq.device')
 
 from .exceptions import CRCError
 
 
@@ -139,15 +139,15 @@
             out_payload.append(i)
 
     out_payload.append(HDLC_BREAK)  # add end-of-packet break char
 
     return out_payload
 
 
-def hdlc_decode(in_payload: ByteString,
+def hdlc_decode(in_payload: Union[bytearray, bytes],
                 ignore_crc: bool = False) -> bytearray:
     """ Decode an HDLC-encoded packet into raw data.
 
         :param in_payload: The HDLC-encoded packet payload.
         :param ignore_crc: If `True`, do not perform a CRC check.
         :returns: The decoded data (including the CRC, if any).
     """
```

### Comparing `endaq-device-1.1.1/endaq/device/legacy.py` & `endaq_device-1.2.0/endaq/device/legacy.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/linux.py` & `endaq_device-1.2.0/endaq/device/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import errno
 import logging
 import os
 import mmap
 import math
 import re
 from time import time
-from typing import ByteString, Tuple, Union
+from typing import Tuple, Union
 import warnings
 
 import psutil
 
 from .types import Drive, Epoch, Filename
 
 logger = logging.getLogger('endaq.device')
@@ -69,15 +69,15 @@
         label = None
     else:
         label = labels[partName]
 
     return Drive(path=dev, label=label, sn=serial, fs=disk.fstype, type=None)
 
 
-def readUncachedFile(filename: Filename) -> ByteString:
+def readUncachedFile(filename: Filename) -> bytes:
     """ Read a file, circumventing the disk cache. Returns the data read.
     """
     filename = os.path.realpath(filename)
     root = os.path.dirname(filename)
 
     if not os.path.isfile(filename):
         raise IOError(errno.ENOENT, 'No such file', filename)
```

### Comparing `endaq-device-1.1.1/endaq/device/macos.py` & `endaq_device-1.2.0/endaq/device/macos.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/measurement.py` & `endaq_device-1.2.0/endaq/device/measurement.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/response_codes.py` & `endaq_device-1.2.0/endaq/device/response_codes.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,24 +14,30 @@
            "CurrentWiFiStatus", "WiFiConnectionError")
 
 
 class DeviceStatusCode(IntEnum):
     """ The device status, returned in the response to a command. Negative
         values denote errors.
     """
-    IDLE = 0  #: Device idle, message successful.
+    IDLE = 0  #: Device idle, message successful. It is implied the device is mounted as a drive.
+    IDLE_UNMOUNTED = 1  #: Device idle, not mounted as a drive. *For future use.*
     RECORDING = 10  #: Device is currently recording.
     RESET_PENDING = 20  #: Reset pending: the device will reset soon after this response is received.
     START_PENDING = 30  #: Recording start pending: the device will start recording soon after this response is received.
+    TRIGGERING = 40 #: Device is currently triggering.
+    SLEEPING = 100  #: Device is currently in sleep mode, or will enter sleep mode soon after this response is received. *For future use.*
 
     ERR_BUSY = -10  #: Communication channel is busy
     ERR_INVALID_COMMAND = -20  #: Badly formed command
+    ERR_BAD_LOCK_ID = -21 #: Command Lock ID invalid
+    ERR_BAD_INFO_INDEX = -22  #: Unknown GetInfo/SetInfo index, or info is read or write only.
     ERR_UNKNOWN_COMMAND = -30  #: Command not recognized
     ERR_BAD_PAYLOAD = -40  #: Command payload is bad
     ERR_BAD_EBML = -50  #: Command EBML is malformed
+    ERR_RESPONSE_TOO_LARGE = -51  #: Internal device error, EBML command response too large
     ERR_BAD_CHECKSUM = -60  #: Command checksum failed (error transmitting packet)
     ERR_BAD_PACKET = -70  #: Content of command packet bad/damaged
 
 
 class WiFiConnectionStatus(IntEnum):
     """ The status of the Wi-Fi connection, returned when querying Wi-Fi.
     """
@@ -74,13 +80,40 @@
     ERR_GROUP_CIPHER_INVALID = 18
     ERR_PAIRWISE_CIPHER_INVALID = 19
     ERR_AKMP_INVALID = 20
     ERR_UNSUPP_RSN_IE_VERSION = 21
     ERR_INVALID_RSN_IE_CAP = 22
     ERR_802_1X_AUTH_FAILED = 23
     ERR_CIPHER_SUITE_REJECTED = 24
+    ERR_TDLS_PEER_UNREACHABLE = 25
+    ERR_TDLS_UNSPECIFIED = 26
+    ERR_SSP_REQUESTED_DISASSOC = 27
+    ERR_NO_SSP_ROAMING_AGREEMENT = 28
+    ERR_BAD_CIPHER_OR_AKM = 29
+    ERR_NOT_AUTHORIZED_THIS_LOCATION = 30
+    ERR_SERVICE_CHANGE_PERCLUDES_TS = 31
+    ERR_UNSPECIFIED_QOS = 32
+    ERR_NOT_ENOUGH_BANDWIDTH = 33
+    ERR_MISSING_ACKS = 34
+    ERR_EXCEEDED_TXOP = 35
+    ERR_STA_LEAVING = 36
+    ERR_END_BA = 37
+    ERR_UNKNOWN_BA = 38
+    ERR_TIMEOUT = 39
+    ERR_PEER_INITIATED = 46
+    ERR_AP_INITIATED = 47
+    ERR_INVALID_FT_ACTION_FRAME_COUNT = 48
+    ERR_INVALID_PMKID = 49
+    ERR_INVALID_MDE = 50
+    ERR_INVALID_FTE = 51
+    ERR_TRANSMISSION_LINK_ESTABLISH_FAILED = 67
+    ERR_ALTERATIVE_CHANNEL_OCCUPIED = 68
     ERR_BEACON_TIMEOUT = 200
     ERR_NO_AP_FOUND = 201
     ERR_AUTH_FAIL = 202
     ERR_ASSOC_FAIL = 203
     ERR_HANDSHAKE_TIMEOUT = 204
     ERR_CONNECTION_FAIL = 205
+    ERR_AP_TSF_RESET = 206
+    ERR_ROAMING = 207
+    ERR_ASSOC_COMEBACK_TIME_TOO_LONG = 208
+    ERR_SA_QUERY_TIMEOUT = 209
```

### Comparing `endaq-device-1.1.1/endaq/device/schemata/command-response.xml` & `endaq_device-1.2.0/endaq/device/schemata/command-response.xml`

 * *Files 4% similar despite different names*

#### Comparing `endaq-device-1.1.1/endaq/device/schemata/command-response.xml` & `endaq_device-1.2.0/endaq/device/schemata/command-response.xml`

```diff
@@ -50,14 +50,15 @@
     <BinaryElement name="KeyVals" id="0x6B76" mandatory="0" multiple="0">Process a key stream and apply it if it is valid</BinaryElement>
   </MasterElement>
   <MasterElement name="EBMLCommand" id="0x80" mandatory="0" multiple="0">
     An EBML formatted command directive
     <UIntegerElement name="CommandIdx" id="0x88" multiple="0" mandatory="1">Incrementing index, will bump by one for each update to this data structure, starting at 0 after device reset</UIntegerElement>
     <!-- Legacy commands, duplicated within EBMLCommand for serial use (which requires the outer EBMLCommand element) -->
     <MasterElement name="RecStart" id="0x7273" mandatory="0" multiple="0">&quot;rs&quot; Initiate a recording as if button was pressed</MasterElement>
+    <MasterElement name="RecStop" id="0x7275" mandatory="0" multiple="0">&quot;ru&quot; Stop a recording as if button was pressed</MasterElement>
     <MasterElement name="LegacyFW" id="0x6677" mandatory="0" multiple="0">&quot;fw&quot; Update App FW (legacy interface)</MasterElement>
     <MasterElement name="LegacyBL" id="0x626C" mandatory="0" multiple="0">&quot;bl&quot; Update Bootloader Image (legacy)</MasterElement>
     <MasterElement name="LegacyAll" id="0x7561" mandatory="0" multiple="0">&quot;ua&quot; Update FW, userpage, and bootloader (legacy)</MasterElement>
     <MasterElement name="FlashPackage" id="0x706B" mandatory="0" multiple="0">&quot;pk&quot; Flash meta-package (arbitrary flash segments)</MasterElement>
     <MasterElement name="LegacyUP" id="0x7570" mandatory="0" multiple="0">&quot;up&quot; Update User Page (legacy)</MasterElement>
     <MasterElement name="LegacyESP" id="0x7577" mandatory="0" multiple="0">&quot;uw&quot; Flash an image to ESP32</MasterElement>
     <MasterElement name="SecureUpdateAll" id="0x7361" mandatory="0" multiple="0">&quot;sa&quot; Securely update FW, userpage, and bootloader</MasterElement>
@@ -86,14 +87,35 @@
     <MasterElement name="QueryWiFi" id="0x85" multiple="0" mandatory="0">Get a response for current Wi-Fi State</MasterElement>
     <MasterElement name="NetworkStatus" id="0x87" multiple="0" mandatory="0">Get network identifiers</MasterElement>
     <BinaryElement name="SetClock" id="0x5510" multiple="0" mandatory="0">Serial only. Set the real time clock. Expects a 10 byte value. Comparable to writing to the CLOCK file.</BinaryElement>
     <MasterElement name="GetClock" id="0x5500" multiple="0" mandatory="0">Serial only. Request RTC clock time. Comparable to reading the CLOCK file.</MasterElement>
     <MasterElement name="GetBattery" id="0x5600" multiple="0" mandatory="0">Serial only. Request the battery state.</MasterElement>
     <BinaryElement name="SendPing" id="0x5700" multiple="0" mandatory="0">Serial only. Request the device echo the enclosed data.</BinaryElement>
     <BinaryElement name="Blink" id="0x5800" multiple="0" mandatory="0">Serial only. Blinks LEDs on device for recognition purposes</BinaryElement>
+    <MasterElement name="GetLockID" id="0x90" mandatory="0" multiple="0">Get the current Lock ID on the device</MasterElement>
+    <MasterElement name="SetLockID" id="0x91" mandatory="0" multiple="0">
+      Set the current Lock ID on the device
+      <BinaryElement name="CurrentLockID" id="0x5A01" mandatory="1" multiple="0"/>
+      <BinaryElement name="NewLockID" id="0x5A02" mandatory="1" multiple="0"/>
+    </MasterElement>
+    <BinaryElement name="LockID" id="0x5A00" mandatory="0" multiple="0">Serial Only, optional LockID</BinaryElement>
+    <IntegerElement name="GetInfo" id="0x5B00" mandatory="0" multiple="0">Serial Only, Get device Info. The value corresponds to:
+            0: DEVINFO - Read Only
+            1: DEVPROPS - Read Only
+            2: CONFIG.UI - Read Only
+            3: MANIFEST - Read Only
+            4: SYSCAL - Read Only
+            5: config.cfg - Read / Write - requires LockID
+            6: usercal.dat - Read / Write - requires LockID
+            7: update.pkg - Write Only - requires LockID
+            8: update.pkg.sig - Write Only - requires LockID</IntegerElement>
+    <MasterElement name="SetInfo" id="0x5B07" mandatory="0" multiple="0">
+      <IntegerElement name="InfoIndex" id="0x5B02" mandatory="1" multiple="0">See GetInfo for index value</IntegerElement>
+      <BinaryElement name="InfoPayload" id="0x5B03" mandatory="1" multiple="0">Payload</BinaryElement>
+    </MasterElement>
   </MasterElement>
   <MasterElement name="EBMLResponse" id="0x86" multiple="0" mandatory="0">
     Response payload to above EBML command payload. Not all commands generate a response
     <UIntegerElement name="ResponseIdx" id="0x5000" multiple="0" mandatory="1">Incrementing index, will bump by one for each update to this data structure, starting at 0 after device reset</UIntegerElement>
     <UIntegerElement name="CMDQueueDepth" id="0x5100" multiple="0" mandatory="1">Available space in command queue on device, a value of 0 means any new commands issued will be dropped</UIntegerElement>
     <MasterElement name="WiFiScanResult" id="0x5200" multiple="0" mandatory="0">
       <UIntegerElement name="ScanVersion" id="0x5201" multiple="0" mandatory="1">Will default to 1 if not present</UIntegerElement>
@@ -138,26 +160,37 @@
             Bit 9: Battery charging
             Bit 8: Level report mode
               == 0: 3-state approximate report (value 0 == empty, 255 == full, any other value is 'some' charge)
               == 1: Approximate charge level 0-255
             Bits 7-0: Charge level (uint8) (percentage = value * 0.39216)</UIntegerElement>
     <BinaryElement name="PingReply" id="0x5701" multiple="0" mandatory="0">Serial only. Contains the echo to a Ping command.</BinaryElement>
     <IntegerElement name="DeviceStatusCode" id="0x5801" multiple="0" mandatory="0">Serial only, mandatory for serial. int16. Negative values are errors.
+            100: Device is currently in sleep mode, or will enter sleep mode soon after this response is received.
+            40: Device Triggering (i.e. waiting for a trigger)
             30: Recording start pending (device will start recording soon after this message is sent)
             20: Reset pending (device will reset soon after this message is sent)
             10: Device recording
-            0: Device idle, message successful.
+            1: Device idle, unmounted.
+            0: Device idle, message successful. It is presumed the device is mounted as an MSD.
             -10: Communication busy
             -20: Command not valid
+            -21: Command Lock ID invalid
+            -22: Command Info Index Unknown / Invalid
             -30: Unknown command
             -40: Bad payload
             -50: EBML invalid
+            -51: Response too large, internal device error
             -60: Bad checksum
             -70: Preamble (CorBus packet header) invalid</IntegerElement>
     <UnicodeElement name="DeviceStatusMessage" id="0x5901" multiple="0" mandatory="0">Serial only. Optional code for device status, including error message</UnicodeElement>
+    <BinaryElement name="LockID" id="0x5A00" mandatory="0" multiple="0">Serial Only, optional current LockID of device</BinaryElement>
+    <MasterElement name="GetInfoResponse" id="0x5B01" mandatory="0" multiple="0">
+      <IntegerElement name="InfoIndex" id="0x5B02" mandatory="1" multiple="0">See GetInfo in EBMLCommand for index value</IntegerElement>
+      <BinaryElement name="InfoPayload" id="0x5B03" mandatory="1" multiple="0">Payload</BinaryElement>
+    </MasterElement>
   </MasterElement>
   <!--
 Attributes: a way to insert an arbitrary key/value into a structure, without revising (and potentially bloating) the
 schema itself. This data is typically non-critical. Strictly speaking, this may be considered an abuse of EBML, but it
 is flexible and moderately clean. This is used in several Mide schemata.
 -->
   <MasterElement name="Attribute" id="0x6110" global="1" multiple="1">
```

### Comparing `endaq-device-1.1.1/endaq/device/schemata/flash_package.xml` & `endaq_device-1.2.0/endaq/device/schemata/flash_package.xml`

 * *Files 10% similar despite different names*

#### Comparing `endaq-device-1.1.1/endaq/device/schemata/flash_package.xml` & `endaq_device-1.2.0/endaq/device/schemata/flash_package.xml`

```diff
@@ -40,14 +40,22 @@
     <UIntegerElement name="MinFWRev" id="0xF3" multiple="0" mandatory="0">Minimum firmware version that can receive this update (in case of interface changes)</UIntegerElement>
     <IntegerElement name="KeySlot" id="0xF4" multiple="0" mandatory="1">AES Key slot used to encrypt payload (-1 for unencrypted payload)</IntegerElement>
     <IntegerElement name="PayloadLen" id="0xF5" multiple="0" mandatory="1">Length of following encrypted payload  of the following format: 1 or more of (uint16 byte offset || uint16 length || [length] bytes of binary data to flash)</IntegerElement>
     <StringElement name="TargetProcessor" id="0xF6" multiple="0" mandatory="1">Processor the attached update is intended for. Values include &quot;EFM32GG11B820F2048GL120&quot;, &quot;STM32U585AII6&quot;, or &quot;ANY&quot; for non-firmware updates</StringElement>
     <StringElement name="FWRevString" id="0xF7" multiple="0" mandatory="0">Human readable firmware revision</StringElement>
     <StringElement name="UpdateNotes" id="0xF8" multiple="0" mandatory="0">Human readable notes regarding the update</StringElement>
     <MasterElement name="NonCriticalElements" global="1" id="0xE0" multiple="0" mandatory="0">The device may skip elements inside NonCriticalElements without stopping the update. Any other unrecognized elements will kill the firmware update.</MasterElement>
+    <!-- Additional element for NCP (EFM currently) information. Not strictly necessary but for newer models allows simultaneous updating of the NCP -->
+    <MasterElement name="NcpUpdate" id="0x80" mandatory="0" multiple="0">
+      <StringElement name="NcpType" id="0x86" multiple="0" mandatory="1">NCP chip type the update is meant for</StringElement>
+      <UIntegerElement name="NcpFwRev" id="0x82" multiple="0" mandatory="1">NCP firmware vers. single digit format</UIntegerElement>
+      <StringElement name="NcpFwRevString" id="0x87" multiple="0" mandatory="0">NCP firmware vers. triple digit format</StringElement>
+      <IntegerElement name="NcpKeySlot" id="0x84" multiple="0" mandatory="1">Encryption key used to decrypt NCP file</IntegerElement>
+      <IntegerElement name="NcpPayloadLen" id="0x85" multiple="0" mandatory="1">Length of NCP encrypted payload of the following format: 1 or more of (uint16 byte offset || uint16 length || [length] bytes of binary data to flash)</IntegerElement>
+    </MasterElement>
     <!-- UpdatePkg -->
   </MasterElement>
   <!-- UpdatePkg -->
   <!-- Not part of the schema officially, but there is a binary blob appended to the end of this "header" that carries the payload described by the tags above -->
   <!--
 Attributes: a way to insert an arbitrary key/value into a structure, without revising (and potentially bloating) the
 schema itself. This data is typically non-critical. Strictly speaking, this may be considered an abuse of EBML, but it
```

### Comparing `endaq-device-1.1.1/endaq/device/schemata/mide_config_ui.xml` & `endaq_device-1.2.0/endaq/device/schemata/mide_config_ui.xml`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/schemata/mide_manifest.xml` & `endaq_device-1.2.0/endaq/device/schemata/mide_manifest.xml`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/slamstick.py` & `endaq_device-1.2.0/endaq/device/slamstick.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,34 +24,27 @@
     SN_FORMAT = "SSX%07d"
 
     # Match all Slam Sticks; this should be last in the list of types to find.
     _NAME_PATTERN = re.compile(r"^Slam Stick.*")
 
     _FW_UPDATE_FILE = os.path.join("SYSTEM", 'firmware.bin')
 
-    # TODO: This really belongs in the configuration UI
-    _POST_CONFIG_MSG = ('When ready...\n'
-                        '    1. Disconnect the recorder\n'
-                        '    2. Mount to surface\n'
-                        '    3. Press the recorder\'s "X" button ')
-
     manufacturer = "Midé Technology Corporation"
     homepage = "https://endaq.com/collections/endaq-shock-recorders-vibration-data-logger-sensors"
 
 
 #===============================================================================
 #
 #===============================================================================
 
 class SlamStickC(SlamStickX):
     """ A Slam Stick C data recorder from Mide Technology Corporation. Also
         sold as enDAQ Sx-D16.
     """
     SN_FORMAT = "SSC%07d"
-    _POST_CONFIG_MSG = SlamStickX._POST_CONFIG_MSG.replace(' "X" ', ' "C" ')
     _NAME_PATTERN = re.compile(r"(^Slam Stick C.*)|(^S[234]-D16)")
 
     @property
     def serial(self) -> str:
         """ The recorder's manufacturer-issued serial number (as string). """
         # Hacky bit to provide Sx-D16 the enDAQ S serial number format.
         if self._sn is None:
@@ -84,9 +77,8 @@
 #
 # ===============================================================================
 
 class SlamStickS(SlamStickX):
     """ A Slam Stick S data recorder from Mide Technology Corporation.
     """
     SN_FORMAT = "SSS%07d"
-    _POST_CONFIG_MSG = SlamStickX._POST_CONFIG_MSG.replace(' "X" ', ' "S" ')
     _NAME_PATTERN = re.compile("^Slam Stick S.*")
```

### Comparing `endaq-device-1.1.1/endaq/device/types.py` & `endaq_device-1.2.0/endaq/device/types.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_025G_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_025G_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_02kG_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_02kG_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_100G_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_100G_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0002_500G_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0002_500G_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0003_016G.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0003_016G.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0003_200G.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0003_200G.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0004_02kG_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0004_02kG_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/LOG_0004_500G_DC.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/LOG_0004_500G_DC.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/S2_D40D200.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/S2_D40D200.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/S2_D8D16.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/S2_D8D16.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/S4_D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/S4_D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/S5_E2000D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/S5_E2000D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/S5_E25D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/S5_E25D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E100D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E100D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E2000D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E2000D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E25D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E25D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_E500D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_E500D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R100D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R100D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R2000D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R2000D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Sx_R500D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Sx_R500D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/W8_E100D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/W8_E100D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/W8_E2000D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/W8_E2000D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/W8_E25D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/W8_E25D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/Wx_D40.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/Wx_D40.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/__init__.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/__init__.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/ui_defaults/default.py` & `endaq_device-1.2.0/endaq/device/ui_defaults/default.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/util.py` & `endaq_device-1.2.0/endaq/device/util.py`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/endaq/device/win.py` & `endaq_device-1.2.0/endaq/device/win.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import ctypes
 import errno
 import logging
 import os
 from pathlib import Path
 import sys
 from time import time
-from typing import ByteString, List, Optional, Tuple
+from typing import List, Optional, Tuple
 import warnings
 
 from .types import Drive, Epoch, Filename
 
 logger = logging.getLogger('endaq.device')
 
 # ==============================================================================
@@ -71,15 +71,15 @@
     except AttributeError:
         fs = None
 
     return Drive(path=dev, label=volumeNameBuffer.value, sn=sn,
                  fs=fs, type=win32file.GetDriveType(dev))
     
 
-def readUncachedFile(filename: Filename) -> ByteString:
+def readUncachedFile(filename: Filename) -> bytes:
     """ Read a file, circumventing the disk cache. Returns the data read.
     """
     if isinstance(filename, Path):
         filename = str(filename)
 
     filename = os.path.realpath(filename)
     root = os.path.dirname(filename)
@@ -180,20 +180,23 @@
                 # First cut: only consider removable drives
                 if devtype == win32file.DRIVE_REMOVABLE or not strict:
                     info = getDriveInfo(driveLetter)
                     for t in types:
                         if t.isRecorder(info, strict=strict):
                             result.append(info)
                             break
+
         except IOError as err:
-            # Rare error, may be caused by flaky device or USB.
-            msg = ("getDeviceList(): Could not access {}:/ ({}); "
-                   "ignoring error and continuing".format(letter, err))
-            warnings.warn(msg)
-            logger.error(msg)
+            # WindowsError 433 is not uncommon for devices that just started recording.
+            # Ignore it, warn about any others.
+            if getattr(err, 'winerror', None) != 433:
+                msg = ("getDeviceList(): Could not access {}:/ ({}); "
+                       "ignoring error and continuing".format(letter, err))
+                warnings.warn(msg)
+                logger.error(msg)
 
         drivebits >>= 1
     return result
 
 
 # Module-level globals for caching last discovered logical drives and recorders
 _LAST_DEVICES = 0       # Bitmap of logical drives (Z...A)
```

### Comparing `endaq-device-1.1.1/endaq_device.egg-info/PKG-INFO` & `endaq_device-1.2.0/endaq_device.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: endaq-device
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python API for enDAQ data recorders
 Home-page: https://github.com/MideTechnology/endaq-device
 Author: Mide Technology
 Author-email: help@mide.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MideTechnology/endaq-device/issues
 Project-URL: Documentation, https://mide-technology-endaq-device.readthedocs-hosted.com/en/latest/
 Project-URL: Source Code, https://github.com/MideTechnology/endaq-device
 Keywords: endaq configure recorder hardware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `endaq-device-1.1.1/endaq_device.egg-info/SOURCES.txt` & `endaq_device-1.2.0/endaq_device.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 ./endaq/device/__init__.py
 ./endaq/device/base.py
 ./endaq/device/command_interfaces.py
 ./endaq/device/config.py
 ./endaq/device/configio.py
+./endaq/device/devinfo.py
 ./endaq/device/endaq.py
 ./endaq/device/exceptions.py
 ./endaq/device/hdlc.py
 ./endaq/device/legacy.py
 ./endaq/device/linux.py
 ./endaq/device/macos.py
 ./endaq/device/measurement.py
@@ -33,15 +34,17 @@
 ./endaq/device/ui_defaults/LOG_0004_02kG_DC.py
 ./endaq/device/ui_defaults/LOG_0004_500G_DC.py
 ./endaq/device/ui_defaults/S2_D40D200.py
 ./endaq/device/ui_defaults/S2_D8D16.py
 ./endaq/device/ui_defaults/S4_D40.py
 ./endaq/device/ui_defaults/S5_E2000D40.py
 ./endaq/device/ui_defaults/S5_E25D40.py
+./endaq/device/ui_defaults/Sx_D16.py
 ./endaq/device/ui_defaults/Sx_D40.py
+./endaq/device/ui_defaults/Sx_D8.py
 ./endaq/device/ui_defaults/Sx_E100D40.py
 ./endaq/device/ui_defaults/Sx_E2000D40.py
 ./endaq/device/ui_defaults/Sx_E25D40.py
 ./endaq/device/ui_defaults/Sx_E500D40.py
 ./endaq/device/ui_defaults/Sx_R100D40.py
 ./endaq/device/ui_defaults/Sx_R2000D40.py
 ./endaq/device/ui_defaults/Sx_R500D40.py
```

### Comparing `endaq-device-1.1.1/endaq_device.egg-info/requires.txt` & `endaq_device-1.2.0/endaq_device.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/pyproject.toml` & `endaq_device-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `endaq-device-1.1.1/setup.py` & `endaq_device-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         long_description=read('README.md'),
         long_description_content_type='text/markdown',
         url='https://github.com/MideTechnology/endaq-device',
         license='MIT',
         classifiers=['Development Status :: 5 - Production/Stable',
                      'License :: OSI Approved :: MIT License',
                      'Natural Language :: English',
-                     'Programming Language :: Python :: 3.7',
                      'Programming Language :: Python :: 3.8',
                      'Programming Language :: Python :: 3.9',
                      'Programming Language :: Python :: 3.10',
                      'Programming Language :: Python :: 3.11',
                      'Programming Language :: Python :: 3.12',
                      ],
         keywords='endaq configure recorder hardware',
```

### Comparing `endaq-device-1.1.1/tests/test__basics.py` & `endaq_device-1.2.0/tests/test__basics.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,19 +55,23 @@
 
 
 def test_getDevices():
     """ Test of `getDevices()`, comparing found device paths to the list of
         fake recorder directories.
     """
     endaq.device.RECORDERS.clear()
-    devs = endaq.device.getDevices(paths=fake_recorders.RECORDER_PATHS, strict=False)
+    devs = endaq.device.getDevices(paths=fake_recorders.RECORDER_PATHS,
+                                   strict=False,
+                                   unmounted=False)
     assert sorted(dev.path for dev in devs) == sorted(fake_recorders.RECORDER_PATHS)
 
     # Just one path provided should return just one device
-    devs = endaq.device.getDevices(paths=fake_recorders.RECORDER_PATHS[0], strict=False)
+    devs = endaq.device.getDevices(paths=fake_recorders.RECORDER_PATHS[0],
+                                   strict=False,
+                                   unmounted=False)
     assert len(devs) == 1
 
 
 @pytest.mark.parametrize("path", RECORDER_PATHS)
 def test_onRecorder(path):
     """ Test checking if a file is on a recorder (its path corresponds
         to a recorder's path).
@@ -81,8 +85,7 @@
 def test_findDevice(path):
     """ Test finding recorders by serial number.
     """
     dev = endaq.device.getRecorder(path, strict=False)
     endaq.device.RECORDERS.clear()
     assert endaq.device.findDevice(dev.serialInt, paths=fake_recorders.RECORDER_PATHS, strict=False)
     assert endaq.device.findDevice(dev.serial, paths=fake_recorders.RECORDER_PATHS, strict=False)
-
```

### Comparing `endaq-device-1.1.1/tests/test_command.py` & `endaq_device-1.2.0/tests/test_command.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,45 @@
 
 from copy import deepcopy
 import os.path
 import pytest
 
 import endaq.device
 from endaq.device import getRecorder, UnsupportedFeature
-from endaq.device.command_interfaces import CommandInterface, FileCommandInterface, SerialCommandInterface, LegacyFileCommandInterface
+from endaq.device.command_interfaces import CommandInterface, FileCommandInterface, SerialCommandInterface
 
 from .fake_recorders import RECORDER_PATHS
 from .mock_hardware import applyMockCommandIO, MockCommandSerialIO
 
 # Clear any cached devices, just to be safe
 endaq.device.RECORDERS.clear()
 
 # Create parameters, mainly to provide an ID, making the results readable
 DEVICES = [pytest.param(getRecorder(path, strict=False), id=os.path.basename(path)) for path in RECORDER_PATHS]
-FILE_DEVICES = [param for param in DEVICES if param[0][0].hasCommandInterface and isinstance(param[0][0].command, FileCommandInterface)]
-SERIAL_DEVICES = [param for param in DEVICES if param[0][0].hasCommandInterface and isinstance(param[0][0].command, SerialCommandInterface)]
 NO_COMMAND_DEVICES = [param for param in DEVICES if not param[0][0].hasCommandInterface]
+COMMAND_DEVICES = [param for param in DEVICES if param[0][0].hasCommandInterface]
+FILE_DEVICES = [param for param in COMMAND_DEVICES if isinstance(param[0][0].command, FileCommandInterface)]
+SERIAL_DEVICES = [param for param in COMMAND_DEVICES if isinstance(param[0][0].command, SerialCommandInterface)]
 
 # NOTE: This should be changed to get devices from DEVICES - see note in fake_recorders.py
 WIFI_DEVICES = [param for param in SERIAL_DEVICES if param[0][0].hasWifi]
 
+# Simple example command
+TEST_COMMAND = {
+    'EBMLCommand': {
+        'SendPing': b'hello world',
+        'CommandIdx': 2}}
+
+# Simple example response to simple example command
+TEST_RESPONSE = {
+    'EBMLResponse': {
+        'ResponseIdx': 2,
+        'CMDQueueDepth': 1,
+        'DeviceStatusCode': 0,
+        'PingReply': b'hello world'}}
 
 # Response to a `scanWifi()` command
 WIFI_SCAN = {'EBMLResponse': {
                   'CMDQueueDepth': 1,
                   'DeviceStatusCode': 0,
                   'ResponseIdx': 1,
                   'WiFiScanResult': {'AP': [{'AuthType': 3,
@@ -73,14 +87,25 @@
     if dev.hasCommandInterface:
         assert isinstance(dev.command, CommandInterface)
     else:
         with pytest.raises(UnsupportedFeature):
             _ = dev.command
 
 
+@pytest.mark.parametrize("dev", COMMAND_DEVICES)
+def test_command_encoding(dev):
+    """ Test basic encoding and decoding of command messages.
+    """
+    command = dev.command._encode(TEST_COMMAND)
+    response = dev.command._encodeResponse(TEST_RESPONSE)
+
+    assert dev.command._decodeCommand(command) == TEST_COMMAND
+    assert dev.command._decode(response) == TEST_RESPONSE
+
+
 @pytest.mark.parametrize("dev", SERIAL_DEVICES)
 def test_command_ping(dev):
     """ Test the `ping()` command on devices that support it.
     """
     mock_io = applyMockCommandIO(dev)
     mock_io.response = mock_io.encodeResponse({'EBMLResponse':
                                                {'ResponseIdx': dev.command.index + 1,
```

### Comparing `endaq-device-1.1.1/tests/test_config_basic.py` & `endaq_device-1.2.0/tests/test_config_basic.py`

 * *Files identical despite different names*

