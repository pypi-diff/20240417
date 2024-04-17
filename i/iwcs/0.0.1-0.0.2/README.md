# Comparing `tmp/iwcs-0.0.1.tar.gz` & `tmp/iwcs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwcs-0.0.1.tar", last modified: Tue Apr 16 16:39:51 2024, max compression
+gzip compressed data, was "iwcs-0.0.2.tar", last modified: Wed Apr 17 15:19:37 2024, max compression
```

## Comparing `iwcs-0.0.1.tar` & `iwcs-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:39:51.694324 iwcs-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 16:39:48.000000 iwcs-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-16 16:39:51.694324 iwcs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-16 16:39:48.000000 iwcs-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:39:51.694324 iwcs-0.0.1/iwcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-16 16:39:48.000000 iwcs-0.0.1/iwcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:39:51.694324 iwcs-0.0.1/iwcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-16 16:39:51.000000 iwcs-0.0.1/iwcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 16:39:51.000000 iwcs-0.0.1/iwcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:39:51.000000 iwcs-0.0.1/iwcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 16:39:51.000000 iwcs-0.0.1/iwcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:39:51.694324 iwcs-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 16:39:48.000000 iwcs-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:19:37.661728 iwcs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 15:19:31.000000 iwcs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-17 15:19:37.661728 iwcs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-17 15:19:31.000000 iwcs-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:19:37.661728 iwcs-0.0.2/iwcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 15:19:31.000000 iwcs-0.0.2/iwcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:19:37.661728 iwcs-0.0.2/iwcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-17 15:19:37.000000 iwcs-0.0.2/iwcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 15:19:37.000000 iwcs-0.0.2/iwcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:19:37.000000 iwcs-0.0.2/iwcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 15:19:37.000000 iwcs-0.0.2/iwcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:19:37.661728 iwcs-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 15:19:31.000000 iwcs-0.0.2/setup.py
```

### Comparing `iwcs-0.0.1/LICENSE` & `iwcs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iwcs-0.0.1/PKG-INFO` & `iwcs-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwcs
-Version: 0.0.1
+Version: 0.0.2
 Summary: iw client stats, get connected wireless client connection statistics
 Home-page: https://github.com/manbehindthemadness/iwcs
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iwcs-0.0.1/README.md` & `iwcs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iwcs-0.0.1/iwcs/__init__.py` & `iwcs-0.0.2/iwcs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import subprocess
 from pathlib import Path
 
 
 if not Path('/sbin/iw').is_file():
     raise FileNotFoundError('command `iw` not found, please run `sudo apt-get install iw`')
 
+
+def mac(mac_address: str, interface: str = 'wlan0') -> dict:
+    """
+    Gather the information in relation to a single sensor by MAC address.
+    """
+    client_info_output = subprocess.check_output(["/sbin/iw", "dev", interface, "station", "get", mac_address]).decode(
+        "utf-8")
+    client_info_lines = client_info_output.split("\n")
+    client_info_dict = {}
+    for line in client_info_lines:
+        if ":" in line:
+            key, value = line.split(":", 1)
+            client_info_dict[key.strip()] = value.strip()
+    return client_info_dict
+
+
 def info(interface: str = 'wlan0') -> dict:
     """
     This will grab the connection stats of the clients connected to the specified interface.
 
     returns: {'<MAC ADDRESS>': {'inactive time': <value>, 'rx bytes': <value>, ...}}
     """
     mac_addresses_output = subprocess.check_output(["/sbin/iw", "dev", interface, "station", "dump"]).decode("utf-8")
     mac_addresses_list = [line.split()[1] for line in mac_addresses_output.split("\n") if "Station" in line]
     clients_info = {}
     for mac_address in mac_addresses_list:
-        client_info_output = subprocess.check_output(["/sbin/iw", "dev", interface, "station", "get", mac_address]).decode("utf-8")
-        client_info_lines = client_info_output.split("\n")
-        client_info_dict = {}
-        for line in client_info_lines:
-            if ":" in line:
-                key, value = line.split(":", 1)
-                client_info_dict[key.strip()] = value.strip()
+        client_info_dict = mac(mac_address, interface)
         clients_info[mac_address] = client_info_dict
     return clients_info
 
 
 def test():
     # Example usage:
     interface = "wlan0"  # Replace with your wireless interface
-    connected_clients_info = get_connected_clients_info(interface)
+    connected_clients_info = info(interface)
     print(connected_clients_info)
```

### Comparing `iwcs-0.0.1/iwcs.egg-info/PKG-INFO` & `iwcs-0.0.2/iwcs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwcs
-Version: 0.0.1
+Version: 0.0.2
 Summary: iw client stats, get connected wireless client connection statistics
 Home-page: https://github.com/manbehindthemadness/iwcs
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iwcs-0.0.1/setup.py` & `iwcs-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='iwcs',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

