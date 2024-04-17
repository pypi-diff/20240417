# Comparing `tmp/broadlink-0.8.tar.gz` & `tmp/broadlink-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/broadlink-0.8.tar", last modified: Sun Mar 18 22:13:03 2018, max compression
+gzip compressed data, was "dist/broadlink-0.9.tar", last modified: Tue Apr 24 15:33:17 2018, max compression
```

## Comparing `broadlink-0.8.tar` & `broadlink-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-03-18 22:13:03.000000 broadlink-0.8/
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/dependency_links.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2016-12-03 22:37:41.000000 broadlink-0.8/broadlink.egg-info/not-zip-safe
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      540 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/PKG-INFO
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       10 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/top_level.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       27 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/requires.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      236 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink.egg-info/SOURCES.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      540 2018-03-18 22:13:03.000000 broadlink-0.8/PKG-INFO
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       38 2018-03-18 22:13:03.000000 broadlink-0.8/setup.cfg
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-03-18 22:13:03.000000 broadlink-0.8/broadlink/
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)    29123 2018-03-18 22:12:30.000000 broadlink-0.8/broadlink/__init__.py
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)     1873 2017-11-27 20:08:06.000000 broadlink-0.8/README.md
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      983 2018-03-18 22:12:44.000000 broadlink-0.8/setup.py
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-04-24 15:33:17.000000 broadlink-0.9/
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2016-12-03 22:37:41.000000 broadlink-0.9/broadlink.egg-info/not-zip-safe
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      540 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/PKG-INFO
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       10 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/top_level.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       27 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/requires.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      236 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      540 2018-04-24 15:33:17.000000 broadlink-0.9/PKG-INFO
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       38 2018-04-24 15:33:17.000000 broadlink-0.9/setup.cfg
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-04-24 15:33:17.000000 broadlink-0.9/broadlink/
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)    30398 2018-04-24 15:32:33.000000 broadlink-0.9/broadlink/__init__.py
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)     2021 2018-04-24 15:32:33.000000 broadlink-0.9/README.md
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      983 2018-04-24 15:32:59.000000 broadlink-0.9/setup.py
```

### Comparing `broadlink-0.8/broadlink.egg-info/PKG-INFO` & `broadlink-0.9/broadlink.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: broadlink
-Version: 0.8
+Version: 0.9
 Summary: Python API for controlling Broadlink IR controllers
 Home-page: http://github.com/mjg59/python-broadlink
 Author: Matthew Garrett
 Author-email: mjg59@srcf.ucam.org
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `broadlink-0.8/PKG-INFO` & `broadlink-0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: broadlink
-Version: 0.8
+Version: 0.9
 Summary: Python API for controlling Broadlink IR controllers
 Home-page: http://github.com/mjg59/python-broadlink
 Author: Matthew Garrett
 Author-email: mjg59@srcf.ucam.org
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `broadlink-0.8/broadlink/__init__.py` & `broadlink-0.9/broadlink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2719 or devtype == 0x7919 or devtype == 0x271a or devtype == 0x791a: # Honeywell SP2
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2720: # SPMini
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x753e: # SP3
     return sp2(host=host, mac=mac, devtype=devtype)
+  elif devtype == 0x7D00: # OEM branded SP3
+    return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x947a or devtype == 0x9479: # SP3S
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2728: # SPMini2
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2733 or devtype == 0x273e: # OEM branded SPMini
     return sp2(host=host, mac=mac, devtype=devtype)
   elif devtype >= 0x7530 and devtype <= 0x7918: # OEM branded SPMini2
@@ -63,15 +65,15 @@
   elif devtype == 0x278f: # RM Mini Shate
     return rm(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2714: # A1
     return a1(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x4EB5 or devtype == 0x4EF7: # MP1: 0x4eb5, honyar oem mp1: 0x4ef7
     return mp1(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x4EAD: # Hysen controller
-    return hysen(host=host, mac=mac)
+    return hysen(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x2722: # S1 (SmartOne Alarm Kit)
     return S1C(host=host, mac=mac, devtype=devtype)
   elif devtype == 0x4E4D: # Dooya DT360E (DOOYA_CURTAIN_V2)
     return dooya(host=host, mac=mac, devtype=devtype)
   else:
     return device(host=host, mac=mac, devtype=devtype)
 
@@ -411,32 +413,44 @@
     """Returns the power state of the smart plug."""
     packet = bytearray(16)
     packet[0] = 1
     response = self.send_packet(0x6a, packet)
     err = response[0x22] | (response[0x23] << 8)
     if err == 0:
       payload = self.decrypt(bytes(response[0x38:]))
-      if ord(payload[0x4]) == 1 or ord(payload[0x4]) == 3:
-        state = True
+      if type(payload[0x4]) == int:
+        if payload[0x4] == 1 or payload[0x4] == 3:
+          state = True
+        else:
+          state = False
       else:
-        state = False
+        if ord(payload[0x4]) == 1 or ord(payload[0x4]) == 3:
+          state = True
+        else:
+          state = False
       return state
 
   def check_nightlight(self):
     """Returns the power state of the smart plug."""
     packet = bytearray(16)
     packet[0] = 1
     response = self.send_packet(0x6a, packet)
     err = response[0x22] | (response[0x23] << 8)
     if err == 0:
       payload = self.decrypt(bytes(response[0x38:]))
-      if ord(payload[0x4]) == 2 or ord(payload[0x4]) == 3:
-        state = True
+      if type(payload[0x4]) == int:
+        if payload[0x4] == 2 or payload[0x4] == 3:
+          state = True
+        else:
+          state = False
       else:
-        state = False
+        if ord(payload[0x4]) == 2 or ord(payload[0x4]) == 3:
+          state = True
+        else:
+          state = False
       return state
 
   def get_energy(self):
     packet = bytearray([8, 0, 254, 1, 5, 1, 0, 0, 0, 45])
     response = self.send_packet(0x6a, packet)
     err = response[0x22] | (response[0x23] << 8)
     if err == 0:
@@ -678,14 +692,23 @@
   # loop_mode = 2 ("1234567") means every day (including Saturday and Sunday) follows the "weekday" schedule
   # The sensor command is currently experimental
   def set_mode(self, auto_mode, loop_mode,sensor=0):
     mode_byte = ( (loop_mode + 1) << 4) + auto_mode
     # print 'Mode byte: 0x'+ format(mode_byte, '02x')
     self.send_request(bytearray([0x01,0x06,0x00,0x02,mode_byte,sensor]))
 
+  # Advanced settings
+  # Sensor mode (SEN) sensor = 0 for internal sensor, 1 for external sensor, 2 for internal control temperature, external limit temperature. Factory default: 0.
+  # Set temperature range for external sensor (OSV) osv = 5..99. Factory default: 42C
+  # Deadzone for floor temprature (dIF) dif = 1..9. Factory default: 2C
+  # Upper temperature limit for internal sensor (SVH) svh = 5..99. Factory default: 35C
+  # Lower temperature limit for internal sensor (SVL) svl = 5..99. Factory default: 5C
+  # Actual temperature calibration (AdJ) adj = -0.5. Prescision 0.1C
+  # Anti-freezing function (FrE) fre = 0 for anti-freezing function shut down, 1 for anti-freezing function open. Factory default: 0
+  # Power on memory (POn) poweron = 0 for power on memory off, 1 for power on memory on. Factory default: 0
   def set_advanced(self, loop_mode, sensor, osv, dif, svh, svl, adj, fre, poweron):
     input_payload = bytearray([0x01,0x10,0x00,0x02,0x00,0x05,0x0a, loop_mode, sensor, osv, dif, svh, svl, (int(adj*2)>>8 & 0xff), (int(adj*2) & 0xff), fre, poweron])
     self.send_request(input_payload)
 
   # For backwards compatibility only.  Prefer calling set_mode directly.  Note this function invokes loop_mode=0 and sensor=0.
   def switch_to_auto(self):
     self.set_mode(auto_mode=1, loop_mode=0)
```

### Comparing `broadlink-0.8/README.md` & `broadlink-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Python control for Broadlink RM2 IR controllers
 ===============================================
 
-A simple Python API for controlling IR controllers from [Broadlink](http://www.ibroadlink.com/rm/). At present, only RM Pro (referred to as RM2 in the codebase) and A1 sensor platform devices are supported. There is currently no support for the cloud API.
+A simple Python API for controlling IR controllers from [Broadlink](http://www.ibroadlink.com/rm/). At present, the following devices are currently supported:
+
+* RM Pro (referred to as RM2 in the codebase)
+* A1 sensor platform devices are supported
+* RM3 mini IR blaster
+
+There is currently no support for the cloud API.
 
 Example use
 -----------
 
 Setup a new device on your local wireless network:
 
 1. Put the device into AP Mode
@@ -64,16 +70,21 @@
 ```
 
 Check power state on a SmartPlug:
 ```
 state = devices[0].check_power()
 ```
 
+Check energy consumption on a SmartPlug:
+```
+state = devices[0].get_energy()
+```
+
 Set power state for S1 on a SmartPowerStrip MP1:
 ```
 devices[0].set_power(1, True)
 ```
 
 Check power state on a SmartPowerStrip:
 ```
 state = devices[0].check_power()
-```
+```
```

### Comparing `broadlink-0.8/setup.py` & `broadlink-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     dynamic_requires = ["pyaes==1.6.0"]
 except ImportError as e:
     dynamic_requires = ['pycryptodome==3.4.11']
 
 # For Hysen thermostatic heating controller
 dynamic_requires.append('PyCRC')
 
-version = 0.8
+version = 0.9
 
 setup(
     name='broadlink',
-    version=0.8,
+    version=0.9,
     author='Matthew Garrett',
     author_email='mjg59@srcf.ucam.org',
     url='http://github.com/mjg59/python-broadlink',
     packages=find_packages(),
     scripts=[],
     install_requires=dynamic_requires,
     description='Python API for controlling Broadlink IR controllers',
```

