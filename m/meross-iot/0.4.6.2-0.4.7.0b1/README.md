# Comparing `tmp/meross_iot-0.4.6.2.tar.gz` & `tmp/meross_iot-0.4.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meross_iot-0.4.6.2.tar", last modified: Mon Feb 12 00:52:51 2024, max compression
+gzip compressed data, was "meross_iot-0.4.7.0b1.tar", last modified: Tue Apr 16 22:16:34 2024, max compression
```

## Comparing `meross_iot-0.4.6.2.tar` & `meross_iot-0.4.7.0b1.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/.version
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.809413 meross_iot-0.4.6.2/meross_iot/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.813413 meross_iot-0.4.6.2/meross_iot/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20292 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.813413 meross_iot-0.4.6.2/meross_iot/controller/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/diffuser_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/diffuser_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/mixins/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/controller/subdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/error_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/http_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53604 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.817412 meross_iot-0.4.6.2/meross_iot/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.817412 meross_iot-0.4.6.2/meross_iot/model/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/http/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/http/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/http/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/http/subdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.817412 meross_iot-0.4.6.2/meross_iot/model/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/plugin/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/plugin/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/plugin/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.817412 meross_iot-0.4.6.2/meross_iot/model/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/online.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/push/unbind.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/model/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.821413 meross_iot-0.4.6.2/meross_iot/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/meross_iot/utilities/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/meross_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-12 00:52:51.000000 meross_iot-0.4.6.2/meross_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_consumptionx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_diffuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_disconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_push_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_togglex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_transport_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/tests/test_valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:51.825413 meross_iot-0.4.6.2/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/utilities/meross_fake_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/utilities/meross_fake_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/utilities/meross_sniffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-12 00:52:34.000000 meross_iot-0.4.6.2/utilities/mixedqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/.version
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.161346 meross_iot-0.4.7.0b1/meross_iot/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.165346 meross_iot-0.4.7.0b1/meross_iot/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.165346 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/subdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/error_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/http_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54525 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/subdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.173346 meross_iot-0.4.7.0b1/meross_iot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/meross_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.173346 meross_iot-0.4.7.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_consumptionx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_diffuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_disconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_push_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_togglex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_transport_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_fake_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_fake_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/mixedqueue.py
```

### Comparing `meross_iot-0.4.6.2/LICENSE` & `meross_iot-0.4.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/PKG-INFO` & `meross_iot-0.4.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.6.2
+Version: 0.4.7.0b1
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -210,19 +210,23 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.6.2
-- Fix dependency specification for paho-mqtt and other libraries
+#### 0.4.7.0b1
+- Added local-lan encryption capabilities to support newest Meross devices
+- Fixed roller shutter mixin not updating initial position after a full async_update() invocation
 
 <details>
     <summary>Older</summary>
+#### 0.4.6.2
+- Fix dependency specification for paho-mqtt and other libraries
+
 #### 0.4.6.0
 - NOTE: this API version breaks backward compatibility with LOGIN method. When upgrading to this version, 
 make sure to pass the new api_base_url value correctly as described in the documentation.
 - Switched the login API to the new signIn path as old /Auth/login is being deprecated
 - Improved CloudCreds to carry also API and MQTT endpoints
 - Handled auto-retry in case of wrong endpoint being used for login
 - Added mac-address attribute to BaseDevice class
```

### Comparing `meross_iot-0.4.6.2/README.md` & `meross_iot-0.4.7.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -187,19 +187,23 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.6.2
-- Fix dependency specification for paho-mqtt and other libraries
+#### 0.4.7.0b1
+- Added local-lan encryption capabilities to support newest Meross devices
+- Fixed roller shutter mixin not updating initial position after a full async_update() invocation
 
 <details>
     <summary>Older</summary>
+#### 0.4.6.2
+- Fix dependency specification for paho-mqtt and other libraries
+
 #### 0.4.6.0
 - NOTE: this API version breaks backward compatibility with LOGIN method. When upgrading to this version, 
 make sure to pass the new api_base_url value correctly as described in the documentation.
 - Switched the login API to the new signIn path as old /Auth/login is being deprecated
 - Improved CloudCreds to carry also API and MQTT endpoints
 - Handled auto-retry in case of wrong endpoint being used for login
 - Added mac-address attribute to BaseDevice class
```

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/device.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -342,14 +342,53 @@
             res = list(filter(lambda c: c.name == channel_id_or_name, self._channels))
         elif isinstance(channel_id_or_name, int):
             res = list(filter(lambda c: c.index == channel_id_or_name, self._channels))
         if len(res) == 1:
             return res[0]
         raise ValueError(f"Could not find channel by id or name = {channel_id_or_name}")
 
+    def support_encryption(self) -> bool:
+        """
+        Returns true if encryption is supported by this device
+        :return:
+        """
+        return False
+
+    def is_encryption_key_set(self) -> bool:
+        """
+        Returns whether an encryption key has been already set
+        :return:
+        """
+        return False
+
+    def set_encryption_key(self, *args, **kwargs):
+        """
+        Sets the encryption key to be used for encryption and decryption
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        pass
+
+    def encrypt(self, message_data_bytes: bytes)->str:
+        """
+        Encrypts the message into a base64 string
+        :param message_data_bytes:
+        :return:
+        """
+        raise NotImplementedError("Encryption not supported by this device")
+
+    def decrypt(self, encrypted_message_bytes: bytes) -> bytes:
+        """
+        Decrypt the message and returns the war decrypted bytes
+        :param encrypted_message_bytes:
+        :return:
+        """
+        raise NotImplementedError("Encryption not supported by this device")
+
 
 class HubDevice(BaseDevice):
     # TODO: provide meaningful comment here describing what this class does
     #  Discvoery?? Bind/unbind?? Online??
     def __init__(self, device_uuid: str, manager, **kwargs):
         super().__init__(device_uuid, manager, **kwargs)
         self._sub_devices = {}
```

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/consumption.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/consumption.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/diffuser_light.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/diffuser_spray.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/dnd.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/electricity.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/garage.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/hub.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/light.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/roller_shutter.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/roller_shutter.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,26 +108,37 @@
         return await self._async_operate(position=position, channel=channel, timeout=timeout, *args, **kwargs)
 
     async def async_update(self, timeout: Optional[float] = None, *args, **kwargs) -> None:
         # Call the super implementation
         await super().async_update(*args, **kwargs)
         # Update the configuration at the same time
         await self.async_fetch_config()
+        await self.async_fetch_position()
 
     async def async_fetch_config(self, timeout: Optional[float] = None, *args, **kwargs) -> None:
         data = await self._execute_command(method="GET",
                                     namespace=Namespace.ROLLER_SHUTTER_CONFIG,
                                     payload={},
                                     timeout=timeout)
         config = data.get('config')
         for d in config:
             channel = d['channel']
             channel_config = d.copy()
             self._shutter__config_by_channel[channel] = channel_config
 
+    async def async_fetch_position(self, timeout: Optional[float] = None, *args, **kwargs) -> None:
+        data = await self._execute_command(method="GET",
+                                    namespace=Namespace.ROLLER_SHUTTER_POSITION,
+                                    payload={},
+                                    timeout=timeout)
+        positions = data.get('position')
+        for p in positions:
+            channel = p['channel']
+            self._shutter__position_by_channel[channel] = p["position"]
+
     def get_open_timer_duration_millis(self, channel: int = 0, *args, **kwargs) -> int:
         self.check_full_update_done()
         return self._shutter__config_by_channel.get(channel).get("signalOpen")
 
     def get_close_timer_duration_millis(self, channel: int = 0, *args, **kwargs) -> int:
         self.check_full_update_done()
         return self._shutter__config_by_channel.get(channel).get("signalClose")
```

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/runtime.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/spray.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/system.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/system.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/thermostat.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/mixins/toggle.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/controller/subdevice.py` & `meross_iot-0.4.7.0b1/meross_iot/controller/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/device_factory.py` & `meross_iot-0.4.7.0b1/meross_iot/device_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from meross_iot.controller.device import BaseDevice, HubDevice, GenericSubDevice
 from meross_iot.controller.mixins.consumption import ConsumptionXMixin, ConsumptionMixin
 from meross_iot.controller.mixins.diffuser_light import DiffuserLightMixin
 from meross_iot.controller.mixins.diffuser_spray import DiffuserSprayMixin
 from meross_iot.controller.mixins.dnd import SystemDndMixin
 from meross_iot.controller.mixins.electricity import ElectricityMixin
+from meross_iot.controller.mixins.encryption import EncryptionSuiteMixin
 from meross_iot.controller.mixins.garage import GarageOpenerMixin
 from meross_iot.controller.mixins.hub import HubMts100Mixin, HubMixn, HubMs100Mixin
 from meross_iot.controller.mixins.light import LightMixin
 from meross_iot.controller.mixins.roller_shutter import RollerShutterTimerMixin
 from meross_iot.controller.mixins.runtime import SystemRuntimeMixin
 from meross_iot.controller.mixins.spray import SprayMixin
 from meross_iot.controller.mixins.system import SystemAllMixin, SystemOnlineMixin
@@ -33,14 +34,17 @@
     # Power plugs abilities
     Namespace.CONTROL_TOGGLEX.value: ToggleXMixin,
     Namespace.CONTROL_TOGGLE.value: ToggleMixin,
     Namespace.CONTROL_CONSUMPTIONX.value: ConsumptionXMixin,
     Namespace.CONTROL_CONSUMPTION.value: ConsumptionMixin,
     Namespace.CONTROL_ELECTRICITY.value: ElectricityMixin,
 
+    # Encryption
+    Namespace.SYSTEM_ENCRYPTION.value: EncryptionSuiteMixin,
+
     # Light abilities
     Namespace.CONTROL_LIGHT.value: LightMixin,
 
     # Garage opener
     Namespace.GARAGE_DOOR_STATE.value: GarageOpenerMixin,
 
     # Roller shutter timer
```

### Comparing `meross_iot-0.4.6.2/meross_iot/error_budget.py` & `meross_iot-0.4.7.0b1/meross_iot/error_budget.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/http_api.py` & `meross_iot-0.4.7.0b1/meross_iot/http_api.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/manager.py` & `meross_iot-0.4.7.0b1/meross_iot/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 _CONNECTION_DROP_UPDATE_SCHEDULE_INTERVAL = 2
 
 T = TypeVar("T", bound=BaseDevice)  # Declare type variable
 ManagerPushNotificationHandlerType = Callable[[GenericPushNotification, List[BaseDevice], 'MerossManager'], Awaitable]
 
 _PENDING_FUTURES = []
 
+_DEFAULT_HEADERS = {"Content-Type": "application/json"}
+
 
 def _mqtt_key_from_domain_port(domain: str, port: int) -> str:
     return f"{domain}:{port}"
 
 
 class TransportMode(Enum):
     MQTT_ONLY = 0
@@ -857,19 +859,36 @@
                                       method: str,
                                       namespace: Union[Namespace,str],
                                       payload: dict,
                                       timeout: float = 10.0):
         # Send the message over the network
         # Build the mqtt message we will send to the broker
         message, message_id = self._build_mqtt_message(method, namespace, payload, destination_device_uuid)
+        device: BaseDevice = self._device_registry.lookup_base_by_uuid(destination_device_uuid)
 
         async with ClientSession() as session:
-            async with session.post(f"http://{device_ip}/config", json=json.loads(message.decode()), timeout=timeout) as response:
-                data = await response.json()
-                return data.get("payload")
+            message_data = message_id
+            decrypt_response = False
+            if device.support_encryption():
+                # Ensure we have correctly set the encryption key. If not, set it right away
+                if not device.is_encryption_key_set():
+                    device.set_encryption_key(uuid=device.uuid, mrskey=self._cloud_creds.key, mac=device.mac_address)
+                # Encrypt the data
+                message_data = device.encrypt(message)
+                decrypt_response = True
+
+            async with session.post(f"http://{device_ip}/config", data=message_data, timeout=timeout, headers=_DEFAULT_HEADERS) as response:
+                response_data = await response.text("utf8")
+
+            if decrypt_response:
+                response_data = device.decrypt(response_data.encode("utf8")).decode("utf8")
+                response_data = response_data.rstrip('\0')
+
+            data = json.loads(response_data)
+            return data.get("payload")
 
     async def async_execute_cmd_client(self,
                                        client: mqtt.Client,
                                        destination_device_uuid: str,
                                        method: str,
                                        namespace: Namespace,
                                        payload: dict,
```

### Comparing `meross_iot-0.4.6.2/meross_iot/model/credentials.py` & `meross_iot-0.4.7.0b1/meross_iot/model/credentials.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/enums.py` & `meross_iot-0.4.7.0b1/meross_iot/model/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     SYSTEM_ALL = 'Appliance.System.All'
     SYSTEM_ABILITY = 'Appliance.System.Ability'
     SYSTEM_ONLINE = 'Appliance.System.Online'
     SYSTEM_REPORT = 'Appliance.System.Report'
     SYSTEM_DEBUG = 'Appliance.System.Debug'
     SYSTEM_RUNTIME = 'Appliance.System.Runtime'
 
+    SYSTEM_ENCRYPTION = 'Appliance.Encrypt.Suite'
+    SYSTEM_ENCRYPTION_ECDHE = 'Appliance.Encrypt.ECDHE'
+
     CONTROL_BIND = 'Appliance.Control.Bind'
     CONTROL_UNBIND = 'Appliance.Control.Unbind'
     CONTROL_TRIGGER = 'Appliance.Control.Trigger'
     CONTROL_TRIGGERX = 'Appliance.Control.TriggerX'
 
     CONFIG_WIFI_LIST = 'Appliance.Config.WifiList'
     CONFIG_TRACE = 'Appliance.Config.Trace'
```

### Comparing `meross_iot-0.4.6.2/meross_iot/model/exception.py` & `meross_iot-0.4.7.0b1/meross_iot/model/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/http/device.py` & `meross_iot-0.4.7.0b1/meross_iot/model/http/device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/http/error_codes.py` & `meross_iot-0.4.7.0b1/meross_iot/model/http/error_codes.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/http/exception.py` & `meross_iot-0.4.7.0b1/meross_iot/model/http/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/http/subdevice.py` & `meross_iot-0.4.7.0b1/meross_iot/model/http/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/plugin/hub.py` & `meross_iot-0.4.7.0b1/meross_iot/model/plugin/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/plugin/light.py` & `meross_iot-0.4.7.0b1/meross_iot/model/plugin/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/plugin/power.py` & `meross_iot-0.4.7.0b1/meross_iot/model/plugin/power.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/push/bind.py` & `meross_iot-0.4.7.0b1/meross_iot/model/push/bind.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/push/common.py` & `meross_iot-0.4.7.0b1/meross_iot/model/push/common.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/push/factory.py` & `meross_iot-0.4.7.0b1/meross_iot/model/push/factory.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/push/online.py` & `meross_iot-0.4.7.0b1/meross_iot/model/push/online.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/model/shared.py` & `meross_iot-0.4.7.0b1/meross_iot/model/shared.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/utilities/conversion.py` & `meross_iot-0.4.7.0b1/meross_iot/utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/utilities/mqtt.py` & `meross_iot-0.4.7.0b1/meross_iot/utilities/mqtt.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot/utilities/stats.py` & `meross_iot-0.4.7.0b1/meross_iot/utilities/stats.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/meross_iot.egg-info/PKG-INFO` & `meross_iot-0.4.7.0b1/meross_iot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.6.2
+Version: 0.4.7.0b1
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -210,19 +210,23 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.6.2
-- Fix dependency specification for paho-mqtt and other libraries
+#### 0.4.7.0b1
+- Added local-lan encryption capabilities to support newest Meross devices
+- Fixed roller shutter mixin not updating initial position after a full async_update() invocation
 
 <details>
     <summary>Older</summary>
+#### 0.4.6.2
+- Fix dependency specification for paho-mqtt and other libraries
+
 #### 0.4.6.0
 - NOTE: this API version breaks backward compatibility with LOGIN method. When upgrading to this version, 
 make sure to pass the new api_base_url value correctly as described in the documentation.
 - Switched the login API to the new signIn path as old /Auth/login is being deprecated
 - Improved CloudCreds to carry also API and MQTT endpoints
 - Handled auto-retry in case of wrong endpoint being used for login
 - Added mac-address attribute to BaseDevice class
```

### Comparing `meross_iot-0.4.6.2/meross_iot.egg-info/SOURCES.txt` & `meross_iot-0.4.7.0b1/meross_iot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 meross_iot/controller/subdevice.py
 meross_iot/controller/mixins/__init__.py
 meross_iot/controller/mixins/consumption.py
 meross_iot/controller/mixins/diffuser_light.py
 meross_iot/controller/mixins/diffuser_spray.py
 meross_iot/controller/mixins/dnd.py
 meross_iot/controller/mixins/electricity.py
+meross_iot/controller/mixins/encryption.py
 meross_iot/controller/mixins/garage.py
 meross_iot/controller/mixins/hub.py
 meross_iot/controller/mixins/light.py
 meross_iot/controller/mixins/roller_shutter.py
 meross_iot/controller/mixins/runtime.py
 meross_iot/controller/mixins/spray.py
 meross_iot/controller/mixins/system.py
```

### Comparing `meross_iot-0.4.6.2/setup.py` & `meross_iot-0.4.7.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_consumptionx.py` & `meross_iot-0.4.7.0b1/tests/test_consumptionx.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_diffuser.py` & `meross_iot-0.4.7.0b1/tests/test_diffuser.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_disconnection.py` & `meross_iot-0.4.7.0b1/tests/test_disconnection.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_dnd.py` & `meross_iot-0.4.7.0b1/tests/test_dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_electricity.py` & `meross_iot-0.4.7.0b1/tests/test_electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_error.py` & `meross_iot-0.4.7.0b1/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_garage.py` & `meross_iot-0.4.7.0b1/tests/test_garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_http.py` & `meross_iot-0.4.7.0b1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_hub.py` & `meross_iot-0.4.7.0b1/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_light.py` & `meross_iot-0.4.7.0b1/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_push_handler.py` & `meross_iot-0.4.7.0b1/tests/test_push_handler.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_roller_shutter.py` & `meross_iot-0.4.7.0b1/tests/test_roller_shutter.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_runtime.py` & `meross_iot-0.4.7.0b1/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_sensor.py` & `meross_iot-0.4.7.0b1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_spray.py` & `meross_iot-0.4.7.0b1/tests/test_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_thermostat.py` & `meross_iot-0.4.7.0b1/tests/test_thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_timeout.py` & `meross_iot-0.4.7.0b1/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_toggle.py` & `meross_iot-0.4.7.0b1/tests/test_toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_togglex.py` & `meross_iot-0.4.7.0b1/tests/test_togglex.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_transport_mode.py` & `meross_iot-0.4.7.0b1/tests/test_transport_mode.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_update.py` & `meross_iot-0.4.7.0b1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/tests/test_valve.py` & `meross_iot-0.4.7.0b1/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/utilities/meross_fake_app.py` & `meross_iot-0.4.7.0b1/utilities/meross_fake_app.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/utilities/meross_fake_device.py` & `meross_iot-0.4.7.0b1/utilities/meross_fake_device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/utilities/meross_sniffer.py` & `meross_iot-0.4.7.0b1/utilities/meross_sniffer.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.6.2/utilities/mixedqueue.py` & `meross_iot-0.4.7.0b1/utilities/mixedqueue.py`

 * *Files identical despite different names*

