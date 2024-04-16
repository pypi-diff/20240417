# Comparing `tmp/napalm_fsos_ssh-1.1.0.tar.gz` & `tmp/napalm_fsos_ssh-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_fsos_ssh-1.1.0.tar", max compression
+gzip compressed data, was "napalm_fsos_ssh-1.2.0.tar", max compression
```

## Comparing `napalm_fsos_ssh-1.1.0.tar` & `napalm_fsos_ssh-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    22294 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/LICENSE
--rw-r--r--   0        0        0    23504 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/LICENSE.fr
--rw-r--r--   0        0        0     2057 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/README.md
--rw-r--r--   0        0        0      319 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/__init__.py
--rw-r--r--   0        0        0    25366 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/fsos.py
--rw-r--r--   0        0        0     1601 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/index
--rw-r--r--   0        0        0      313 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/ping.textfsm
--rw-r--r--   0        0        0      151 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_arp.textfsm
--rw-r--r--   0        0        0      242 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      835 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm
--rw-r--r--   0        0        0      225 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      331 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_route.textfsm
--rw-r--r--   0        0        0      180 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      196 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      270 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_route.textfsm
--rw-r--r--   0        0        0      175 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor.textfsm
--rw-r--r--   0        0        0      395 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor_interface.textfsm
--rw-r--r--   0        0        0      135 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_memory.textfsm
--rw-r--r--   0        0        0       71 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_ntp.textfsm
--rw-r--r--   0        0        0      190 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server.textfsm
--rw-r--r--   0        0        0       95 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server_engine_id.textfsm
--rw-r--r--   0        0        0      432 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_system.textfsm
--rw-r--r--   0        0        0      418 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_transceiver.textfsm
--rw-r--r--   0        0        0      107 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_users.textfsm
--rw-r--r--   0        0        0      163 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_version.textfsm
--rw-r--r--   0        0        0     1049 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm
--rw-r--r--   0        0        0      221 2024-04-11 17:49:19.240029 napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/traceroute.textfsm
--rw-r--r--   0        0        0     1099 2024-04-11 17:49:39.759933 napalm_fsos_ssh-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 napalm_fsos_ssh-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    22294 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/LICENSE
+-rw-r--r--   0        0        0    23504 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/LICENSE.fr
+-rw-r--r--   0        0        0     2057 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/README.md
+-rw-r--r--   0        0        0      319 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/__init__.py
+-rw-r--r--   0        0        0    25366 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/fsos.py
+-rw-r--r--   0        0        0     1601 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/index
+-rw-r--r--   0        0        0      313 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/ping.textfsm
+-rw-r--r--   0        0        0      151 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_arp.textfsm
+-rw-r--r--   0        0        0      242 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      835 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm
+-rw-r--r--   0        0        0      225 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      331 2024-04-16 23:11:20.864227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ip_route.textfsm
+-rw-r--r--   0        0        0      180 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      196 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      270 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      175 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor.textfsm
+-rw-r--r--   0        0        0      395 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_lldp_neighbor_interface.textfsm
+-rw-r--r--   0        0        0      135 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_memory.textfsm
+-rw-r--r--   0        0        0       71 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_ntp.textfsm
+-rw-r--r--   0        0        0      190 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server.textfsm
+-rw-r--r--   0        0        0       95 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_snmp_server_engine_id.textfsm
+-rw-r--r--   0        0        0      432 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_system.textfsm
+-rw-r--r--   0        0        0      418 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_transceiver.textfsm
+-rw-r--r--   0        0        0      107 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_users.textfsm
+-rw-r--r--   0        0        0      163 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_version.textfsm
+-rw-r--r--   0        0        0     1049 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm
+-rw-r--r--   0        0        0      221 2024-04-16 23:11:20.868227 napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/traceroute.textfsm
+-rw-r--r--   0        0        0     1145 2024-04-16 23:11:43.259954 napalm_fsos_ssh-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 napalm_fsos_ssh-1.2.0/PKG-INFO
```

### Comparing `napalm_fsos_ssh-1.1.0/LICENSE` & `napalm_fsos_ssh-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/LICENSE.fr` & `napalm_fsos_ssh-1.2.0/LICENSE.fr`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/README.md` & `napalm_fsos_ssh-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/fsos.py` & `napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/fsos.py`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/index` & `napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/index`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm` & `napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_interfaces_counters.textfsm`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm` & `napalm_fsos_ssh-1.2.0/napalm_fsos_ssh/utils/textfsm_templates/show_vlan_all.textfsm`

 * *Files identical despite different names*

### Comparing `napalm_fsos_ssh-1.1.0/pyproject.toml` & `napalm_fsos_ssh-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "napalm-fsos-ssh"
-version = "v1.1.0"
+version = "v1.2.0"
 description = "Napalm driver for FSOS through SSH"
 authors = ["Ludovic Ortega <ludovic.ortega@adminafk.fr>"]
 license = "CeCILL"
 readme = "README.md"
 homepage = "https://github.com/napalm-automation-community/napalm-fsos-ssh"
 repository = "https://github.com/napalm-automation-community/napalm-fsos-ssh"
 keywords = ["napalm", "fsos", "netmiko"]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
     "Topic :: Utilities",
 ]
 include = [
     "LICENSE",
     "LICENSE.fr",
 ]
 
 [tool.poetry.dependencies]
-python = ">3.8,<3.12"
+python = ">3.8,<3.13"
 napalm = ">=4.0,<5.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.4,<8.2.0"
 ruff = ">=0.1.11,<0.4.0"
 
 [build-system]
```

### Comparing `napalm_fsos_ssh-1.1.0/PKG-INFO` & `napalm_fsos_ssh-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: napalm-fsos-ssh
-Version: 1.1.0
+Version: 1.2.0
 Summary: Napalm driver for FSOS through SSH
 Home-page: https://github.com/napalm-automation-community/napalm-fsos-ssh
 License: CeCILL
 Keywords: napalm,fsos,netmiko
 Author: Ludovic Ortega
 Author-email: ludovic.ortega@adminafk.fr
-Requires-Python: >3.8,<3.12
+Requires-Python: >3.8,<3.13
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Dist: napalm (>=4.0,<5.1)
 Project-URL: Repository, https://github.com/napalm-automation-community/napalm-fsos-ssh
 Description-Content-Type: text/markdown
 
 Napalm driver for FSOS using SSH
```

