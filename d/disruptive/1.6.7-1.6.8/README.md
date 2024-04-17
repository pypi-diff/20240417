# Comparing `tmp/disruptive-1.6.7.tar.gz` & `tmp/disruptive-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disruptive-1.6.7.tar", last modified: Thu Apr 11 09:03:13 2024, max compression
+gzip compressed data, was "disruptive-1.6.8.tar", last modified: Wed Apr 17 07:04:26 2024, max compression
```

## Comparing `disruptive-1.6.7.tar` & `disruptive-1.6.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 09:03:02.000000 disruptive-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-11 09:03:13.544314 disruptive-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-11 09:03:02.000000 disruptive-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.540314 disruptive-1.6.7/disruptive/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68441 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/events/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/eventhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 09:03:02.000000 disruptive-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 09:03:13.544314 disruptive-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 09:03:02.000000 disruptive-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:26.298782 disruptive-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-17 07:04:18.000000 disruptive-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-17 07:04:26.298782 disruptive-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-17 07:04:18.000000 disruptive-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:26.294782 disruptive-1.6.8/disruptive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:26.294782 disruptive-1.6.8/disruptive/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68441 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:26.298782 disruptive-1.6.8/disruptive/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21329 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/eventhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/resources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-17 07:04:18.000000 disruptive-1.6.8/disruptive/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:04:26.294782 disruptive-1.6.8/disruptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-17 07:04:26.000000 disruptive-1.6.8/disruptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-17 07:04:26.000000 disruptive-1.6.8/disruptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:04:26.000000 disruptive-1.6.8/disruptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 07:04:26.000000 disruptive-1.6.8/disruptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 07:04:26.000000 disruptive-1.6.8/disruptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 07:04:18.000000 disruptive-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-17 07:04:26.298782 disruptive-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 07:04:18.000000 disruptive-1.6.8/setup.py
```

### Comparing `disruptive-1.6.7/LICENSE` & `disruptive-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/PKG-INFO` & `disruptive-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.6.7
+Version: 1.6.8
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.6.7/README.md` & `disruptive-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/__init__.py` & `disruptive-1.6.8/disruptive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Metadata
-__version__ = '1.6.7'
+__version__ = '1.6.8'
 
 # If set, logs of chosen level and higher are printed to console.
 # Default value None results in no logs at any level.
 log_level = None
 
 # REST API base URLs of which all endpoints are an expansion.
 base_url = 'https://api.disruptive-technologies.com/v2'
```

### Comparing `disruptive-1.6.7/disruptive/authentication.py` & `disruptive-1.6.8/disruptive/authentication.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/errors.py` & `disruptive-1.6.8/disruptive/errors.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/events/__init__.py` & `disruptive-1.6.8/disruptive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/events/events.py` & `disruptive-1.6.8/disruptive/events/events.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/logging.py` & `disruptive-1.6.8/disruptive/logging.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/outputs.py` & `disruptive-1.6.8/disruptive/outputs.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/requests.py` & `disruptive-1.6.8/disruptive/requests.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/claim.py` & `disruptive-1.6.8/disruptive/resources/claim.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/data_connector.py` & `disruptive-1.6.8/disruptive/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/device.py` & `disruptive-1.6.8/disruptive/resources/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Optional, Any
 
 import disruptive.logging as dtlog
 import disruptive.requests as dtrequests
-import disruptive.events.events as dtevents
+from disruptive.events import events
 import disruptive.outputs as dtoutputs
 from disruptive.errors import TransferDeviceError, LabelUpdateError
 
 
 class Device(dtoutputs.OutputBase):
     """
     Represents Sensors and Cloud Connectors, together referred to as devices.
@@ -76,32 +76,31 @@
         # Unpack attributes from dictionary.
         self.device_id: str = device['name'].split('/')[-1]
         self.project_id: str = device['name'].split('/')[1]
         self.device_type: str = device['type']
         self.labels: dict = device['labels']
 
         # Set display_name if `name` label key exists.
-        self.display_name = None
+        self.display_name: str | None = None
         if 'name' in self.labels:
             self.display_name = self.labels['name']
 
         # Determine if the device is an emulator by checking id prefix.
+        self.is_emulated: bool = False
         if self.device_id.startswith('emu') and len(self.device_id) == 23:
             self.is_emulated = True
-        else:
-            self.is_emulated = False
 
         # If it exists, set the product number.
         # This is not present for emulated devices.
         self.product_number: str = ''
         if 'productNumber' in device:
             self.product_number = device['productNumber']
 
         # If it exists, set the reported object.
-        self.reported = None
+        self.reported: Reported | None = None
         if 'reported' in device:
             self.reported = Reported(device['reported'])
 
     @classmethod
     def get_device(cls,
                    device_id: str,
                    project_id: Optional[str] = None,
@@ -534,42 +533,58 @@
         Object representing reported ethernetStatus event data.
     cellular_status : CellularStatus, None
         Object representing reported cellularStatus event data.
     co2 : Co2, None
         Object representing reported co2 event data.
     pressure : Pressure, None
         Object representing reported pressure event data.
+    motion : Motion, None
+        Object representing reported motion event data.
     desk_occupancy : DeskOccupancy, None
         Object representing reported deskOccupancy event data.
+    contact : Contact, None
+        Object representing reported contact event data.
+    probe_wire_status : ProbeWireStatus, None
+        Object representing reported probeWireStatus event data.
 
     """
 
+    touch: events.Touch | None = None
+    temperature: events.Temperature | None = None
+    object_present: events.ObjectPresent | None = None
+    humidity: events.Humidity | None = None
+    object_present_count: events.ObjectPresentCount | None = None
+    touch_count: events.TouchCount | None = None
+    water_present: events.WaterPresent | None = None
+    network_status: events.NetworkStatus | None = None
+    battery_status: events.BatteryStatus | None = None
+    connection_status: events.ConnectionStatus | None = None
+    ethernet_status: events.EthernetStatus | None = None
+    cellular_status: events.CellularStatus | None = None
+    co2: events.Co2 | None = None
+    pressure: events.Pressure | None = None
+    motion: events.Motion | None = None
+    desk_occupancy: events.DeskOccupancy | None = None
+    contact: events.Contact | None = None
+    probe_wire_status: events.ProbeWireStatus | None = None
+
     def __init__(self, reported: dict) -> None:
         """
         Constructs the Reported object by unpacking each event in the field.
 
         Parameters
         ----------
         reported : dict
             Dictionary of the reported field for a device.
 
         """
 
         # Inherit parent Event class init.
         dtoutputs.OutputBase.__init__(self, reported)
 
-        # Set default attribute values.
-        for key in dtevents._EVENTS_MAP._api_names:
-            # Skip labelsChanged as it does not exist in reported.
-            if key == 'labelsChanged':
-                continue
-
-            # Set attribute to None.
-            setattr(self, dtevents._EVENTS_MAP._api_names[key].attr_name, None)
-
         # Unpack the reported dictionary data.
         self.__unpack()
 
     def __unpack(self) -> None:
         """
         Iterates each field in the raw dictionary and set the
         related attribute to the appropriate _EventData child object.
@@ -583,19 +598,19 @@
             if self._raw[key] is None:
                 continue
 
             # Repack the data field in expected format.
             repacked = {key: self._raw[key]}
 
             # Check if key exists in map of known events.
-            if key in dtevents._EVENTS_MAP._api_names:
+            if key in events._EVENTS_MAP._api_names:
                 # Initialize appropriate data instance.
-                data = dtevents._EventData.from_event_type(repacked, key)
+                data = events._EventData.from_event_type(repacked, key)
 
                 # Set attribute according to event type.
                 setattr(
                     self,
-                    dtevents._EVENTS_MAP._api_names[key].attr_name,
+                    events._EVENTS_MAP._api_names[key].attr_name,
                     data,
                 )
             else:
                 dtlog.warning('Skipping unknown reported type {}.'.format(key))
```

### Comparing `disruptive-1.6.7/disruptive/resources/emulator.py` & `disruptive-1.6.8/disruptive/resources/emulator.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/eventhistory.py` & `disruptive-1.6.8/disruptive/resources/eventhistory.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/organization.py` & `disruptive-1.6.8/disruptive/resources/organization.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/project.py` & `disruptive-1.6.8/disruptive/resources/project.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/role.py` & `disruptive-1.6.8/disruptive/resources/role.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/service_account.py` & `disruptive-1.6.8/disruptive/resources/service_account.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/resources/stream.py` & `disruptive-1.6.8/disruptive/resources/stream.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive/transforms.py` & `disruptive-1.6.8/disruptive/transforms.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/disruptive.egg-info/PKG-INFO` & `disruptive-1.6.8/disruptive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.6.7
+Version: 1.6.8
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.6.7/disruptive.egg-info/SOURCES.txt` & `disruptive-1.6.8/disruptive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.7/setup.cfg` & `disruptive-1.6.8/setup.cfg`

 * *Files identical despite different names*

