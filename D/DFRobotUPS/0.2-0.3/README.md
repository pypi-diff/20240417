# Comparing `tmp/DFRobotUPS-0.2.tar.gz` & `tmp/DFRobotUPS-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.2.tar", last modified: Tue Apr 16 23:00:52 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.3.tar", last modified: Wed Apr 17 00:42:41 2024, max compression
```

## Comparing `DFRobotUPS-0.2.tar` & `DFRobotUPS-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-16 23:00:52.122192 DFRobotUPS-0.2/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-16 23:00:52.092192 DFRobotUPS-0.2/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      177 2024-04-16 22:50:29.000000 DFRobotUPS-0.2/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2911 2024-04-16 22:50:29.000000 DFRobotUPS-0.2/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2886 2024-04-16 22:50:29.000000 DFRobotUPS-0.2/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-16 23:00:52.122192 DFRobotUPS-0.2/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-16 23:00:49.000000 DFRobotUPS-0.2/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-16 23:00:52.000000 DFRobotUPS-0.2/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-16 23:00:49.000000 DFRobotUPS-0.2/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-16 23:00:49.000000 DFRobotUPS-0.2/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-16 23:00:49.000000 DFRobotUPS-0.2/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-16 22:50:37.000000 DFRobotUPS-0.2/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-16 23:00:52.122192 DFRobotUPS-0.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-16 22:50:37.000000 DFRobotUPS-0.2/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-16 23:00:52.132192 DFRobotUPS-0.2/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-16 22:54:10.000000 DFRobotUPS-0.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 00:42:41.175976 DFRobotUPS-0.3/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 00:42:41.145976 DFRobotUPS-0.3/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      193 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3072 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3632 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 00:42:41.175976 DFRobotUPS-0.3/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-17 00:42:38.000000 DFRobotUPS-0.3/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-17 00:42:40.000000 DFRobotUPS-0.3/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-17 00:42:38.000000 DFRobotUPS-0.3/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-17 00:42:38.000000 DFRobotUPS-0.3/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-17 00:42:38.000000 DFRobotUPS-0.3/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-17 00:42:41.175976 DFRobotUPS-0.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-17 00:42:41.185976 DFRobotUPS-0.3/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-17 00:41:12.000000 DFRobotUPS-0.3/setup.py
```

### Comparing `DFRobotUPS-0.2/DFRobotUPS/__main__.py` & `DFRobotUPS-0.3/DFRobotUPS/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # DFRobotUPS.__main__
 
 
 
 import argparse
 import functools
 import os
+import sys
 from time import sleep
 
-from . import __version__, DFRobotUPS, DEFAULT_ADDR, DEFAULT_BUS
+from . import __version__, DFRobotUPS, DEFAULT_ADDR, DEFAULT_BUS, PID
 
 
 
 # --- parse arguments ---
 
 
 
@@ -77,22 +78,29 @@
 
 
 # --- main ---
 
 
 
 if args.debug:
-    print(f"DFRobotUPS HAT at I2C address 0x{args.addr:02x} on bus {args.bus}")
+    print(f"DFRobotUPS HAT on bus {args.bus} at I2C address 0x{args.addr:02x}")
 
 
 # get the UPS object to poll SoC
 
 ups = DFRobotUPS(addr=args.addr, bus=args.bus)
 
 
+# check we do appear to have a UPS HAT at the specified address/bus
+
+if not ups.present:
+    print("error: UPS HAT not found")
+    sys.exit(1)
+
+
 # if we're in shutdown polling mode, do that
 
 if args.shutdown:
     if args.debug:
         print("Polling SoC for shutdown with command:", *args.cmd)
 
     while True:
```

### Comparing `DFRobotUPS-0.2/DFRobotUPS/ups.py` & `DFRobotUPS-0.3/DFRobotUPS/ups.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 
 # the default I2C and SM bus addresses for the UPS HAT
 
 DEFAULT_ADDR = 0x10
 DEFAULT_BUS = 1
 
 
+# the PID for the UPS HAT as returned by an I2C register (below)
+
+PID = 0xdf
+
+
 # the numbers of registers for UPS information, as read using
 # smbus.SMBus.read_byte_data()
 
 REG_ADDR = 0x00
 REG_PID = 0x01
 REG_FWVER = 0x02
 REG_VCELLHI = 0x03
@@ -52,17 +57,26 @@
     def __init__(self, addr=DEFAULT_ADDR, bus=DEFAULT_BUS):
         """Initialise a UPS object at the specified address and SM bus.
         """
 
         self.addr = addr
         self.bus = smbus.SMBus(bus)
 
+        # try to talk to the device for the PID and, if this fails, or
+        # the PID is wrong, set the 'present' flag to False
+        self.present = False
+        try:
+            if self._get_pid() == PID:
+                self.present = True
+        except OSError:
+            pass
+
 
     def _get_pid(self):
-        """Return the product identifier, which should be 0xDF.
+        """Return the product identifier, which should be 0xdf.
         """
 
         return self.bus.read_byte_data(self.addr, REG_PID)
 
 
     def _get_fwver(self):
         """Return the firmware version of the UPS board as tuple with
@@ -94,15 +108,25 @@
 
     def __getattribute__(self, name):
         """Return information about the UPS as attributes.  This is the
         recommended way to retrieve information.
 
         Attributes available are:
 
-        * pid - product identifier (should be 0xDF)
+        * present - whether the UPS HAT appears to be present or not; if
+        False, the remainder of the attributes will be unavailable, save
+        for addr and bus
+
+        * addr - the I2C address of the HAT (as requested for the
+        object, not what is necessarily configured on the HAT)
+
+        * bus - the SMBus requested
+
+        * pid - product identifier (should be 0xdf), else 'present' will
+        be False
 
         * fwver - a tuple containing the firmware version (major, minor)
 
         * vcell - current cell voltage in mV
 
         * soc - state of charge as a floating point percentage
         """
```

### Comparing `DFRobotUPS-0.2/DFRobotUPS.egg-info/PKG-INFO` & `DFRobotUPS-0.3/DFRobotUPS.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.2
+Version: 0.3
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.2/LICENSE` & `DFRobotUPS-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.2/PKG-INFO` & `DFRobotUPS-0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.2
+Version: 0.3
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.2/README.md` & `DFRobotUPS-0.3/README.md`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.2/setup.py` & `DFRobotUPS-0.3/setup.py`

 * *Files identical despite different names*

