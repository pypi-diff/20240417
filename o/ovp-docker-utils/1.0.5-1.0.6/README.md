# Comparing `tmp/ovp_docker_utils-1.0.5.tar.gz` & `tmp/ovp_docker_utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.5.tar", last modified: Mon Apr 15 20:16:57 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.6.tar", last modified: Wed Apr 17 00:16:55 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.5.tar` & `ovp_docker_utils-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.819455 ovp_docker_utils-1.0.5/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      380 2024-04-15 20:16:57.818456 ovp_docker_utils-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.787455 ovp_docker_utils-1.0.5/ovp_docker_utils/
--rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-15 20:16:15.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33479 2024-04-15 20:14:29.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.817456 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 20:16:57.819455 ovp_docker_utils-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.653143 ovp_docker_utils-1.0.6/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-04-17 00:16:55.652145 ovp_docker_utils-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.613147 ovp_docker_utils-1.0.6/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-15 20:43:27.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    33397 2024-04-17 00:10:52.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.650143 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 00:16:55.653143 ovp_docker_utils-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/setup.py
```

### Comparing `ovp_docker_utils-1.0.5/LICENSE` & `ovp_docker_utils-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/README.md` & `ovp_docker_utils-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.6/ovp_docker_utils/docker_compose_instance.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.6/ovp_docker_utils/oem_logging.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.6/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,35 +322,33 @@
 
     @property
     def vpu_name(self):
         return self.vpu_config["device"]["info"]["name"]
 
     def connect(self,) -> bool:
 
+        
         if not USING_IFM3DPY:
             logger.info("ifm3dpy unavailable")
         if USING_IFM3DPY:
-            if not possible_initial_ip_addresses:
-                possible_initial_ip_addresses = []
-            possible_initial_ip_addresses = list(
-                set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
-            if len(possible_initial_ip_addresses) > 1:
+            if len(self.config.possible_initial_ip_addresses_to_try) ==0:
+                VPU_config = ifm3dpy.O3R(self.config.IP).get()
+                logger.info(f"Connected to {self.config.IP}")
+                self._connected = True
+            else:
+                possible_initial_ip_addresses = list(
+                    set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
                 logger.info(
                     f"Trying to connect to VPU at any of the following addresses: {possible_initial_ip_addresses}")
 
                 for temp_IP in possible_initial_ip_addresses:
-                    try:
-                        VPU_config = ifm3dpy.O3R(temp_IP).get()
-                        logger.info(f"Connected to {temp_IP}")
-                        self._connected = True
-                        break
-                    except Exception as e:
-                        if "XMLRPC Timeout" in str(e):
-                            continue
-                        raise e
+                    VPU_config = ifm3dpy.O3R(temp_IP).get()
+                    logger.info(f"Connected to {temp_IP}")
+                    self._connected = True
+                    break
                 if not self._connected:
                     logger.info(
                         f"VPU could not be found at any of the following addresses: {possible_initial_ip_addresses}")
                 elif temp_IP != self.config.IP:
                     logger.info(
                         f"Updating IP address from {temp_IP} to {self.config.IP}")
                     gateway = ".".join(
@@ -365,14 +363,15 @@
                     ifm3dpy.O3R(temp_IP).reboot()
                     wait_period = 80
                     logger.info(f"Waiting 80s for VPU to reboot.")
                     heartbeat_rate = 2
                     for x in range(int(wait_period/heartbeat_rate)):
                         print(".", end="")
                         time.sleep(heartbeat_rate)
+        
         if USING_IFM3DPY and self._connected:
             self._o3r = ifm3dpy.O3R(self.config.IP)
             self._fw_version = ".".join(self.vpu_config["device"]["swVersion"]["firmware"].split(
                 "-")[0].split(".")[:3])  # get the first 3 parts of the version number
 
             logger.info(f"Device firmware version: {self._fw_version}")
```

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_file_utils.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_key_gen.py` & `ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_key_gen.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.5/setup.py` & `ovp_docker_utils-1.0.6/setup.py`

 * *Files identical despite different names*

