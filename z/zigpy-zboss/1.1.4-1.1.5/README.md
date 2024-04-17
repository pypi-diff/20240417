# Comparing `tmp/zigpy-zboss-1.1.4.tar.gz` & `tmp/zigpy_zboss-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-zboss-1.1.4.tar", last modified: Fri Apr  5 10:49:36 2024, max compression
+gzip compressed data, was "zigpy_zboss-1.1.5.tar", last modified: Wed Apr 17 14:32:18 2024, max compression
```

## Comparing `zigpy-zboss-1.1.4.tar` & `zigpy_zboss-1.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.921142 zigpy-zboss-1.1.4/zigpy_zboss/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/af.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/aps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/ncp_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/nwk_mgmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/zdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/nvram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/factory_reset_ncp.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/get_ncp_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/types/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/named.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/nvids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/uart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.810403 zigpy_zboss-1.1.5/zigpy_zboss/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.810403 zigpy_zboss-1.1.5/zigpy_zboss/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/aps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/ncp_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/nwk_mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/commands/zdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/nvram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.810403 zigpy_zboss-1.1.5/zigpy_zboss/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/tools/factory_reset_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/tools/get_ncp_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/zigpy_zboss/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/nvids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/types/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/zigpy_zboss/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25356 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/zigbee/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-17 14:32:11.000000 zigpy_zboss-1.1.5/zigpy_zboss/zigbee/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:32:18.814403 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-17 14:32:18.000000 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-17 14:32:18.000000 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:32:18.000000 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 14:32:18.000000 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 14:32:18.000000 zigpy_zboss-1.1.5/zigpy_zboss.egg-info/top_level.txt
```

### Comparing `zigpy-zboss-1.1.4/COPYING` & `zigpy_zboss-1.1.5/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/LICENSE` & `zigpy_zboss-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/PKG-INFO` & `zigpy_zboss-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `zigpy-zboss-1.1.4/README.md` & `zigpy_zboss-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/pyproject.toml` & `zigpy_zboss-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/setup.cfg` & `zigpy_zboss-1.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/api.py` & `zigpy_zboss-1.1.5/zigpy_zboss/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/checksum.py` & `zigpy_zboss-1.1.5/zigpy_zboss/checksum.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/__init__.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/af.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/af.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/aps.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/aps.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/ncp_config.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/ncp_config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/security.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/commands/zdo.py` & `zigpy_zboss-1.1.5/zigpy_zboss/commands/zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/config.py` & `zigpy_zboss-1.1.5/zigpy_zboss/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/debug.py` & `zigpy_zboss-1.1.5/zigpy_zboss/debug.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/frames.py` & `zigpy_zboss-1.1.5/zigpy_zboss/frames.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/logger.py` & `zigpy_zboss-1.1.5/zigpy_zboss/logger.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/nvram.py` & `zigpy_zboss-1.1.5/zigpy_zboss/nvram.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/tools/config.py` & `zigpy_zboss-1.1.5/zigpy_zboss/tools/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/tools/factory_reset_ncp.py` & `zigpy_zboss-1.1.5/zigpy_zboss/tools/factory_reset_ncp.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/tools/get_ncp_version.py` & `zigpy_zboss-1.1.5/zigpy_zboss/tools/get_ncp_version.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/basic.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/commands.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,12 +699,23 @@
 
     Mains = 1 << 0
     RechargeableBattery = 1 << 1
     DisposableBattery = 1 << 2
     Reserved = 1 << 3
 
 
+class Relationship(t.enum8):
+    """Enum class for Relationship."""
+
+    Parent = 0x00
+    Child = 0x01
+    Sibling = 0x02
+    NoneOfTheAbove = 0x03
+    PreviousChild = 0x04
+    Unauthenticated = 0x05
+
+
 STATUS_SCHEMA = (
     t.Param("TSN", t.uint8_t, "Transmit Sequence Number"),
     t.Param("StatusCat", StatusCategory, "Status category code"),
     t.Param("StatusCode", t.uint8_t, "Status code inside category"),
 )
```

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/cstruct.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/cstruct.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/named.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/nvids.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/nvids.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/types/structs.py` & `zigpy_zboss-1.1.5/zigpy_zboss/types/structs.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/uart.py` & `zigpy_zboss-1.1.5/zigpy_zboss/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/utils.py` & `zigpy_zboss-1.1.5/zigpy_zboss/utils.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/zigbee/application.py` & `zigpy_zboss-1.1.5/zigpy_zboss/zigbee/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,16 @@
         map = await self._api.nvram.read(
                 t_zboss.DatasetId.ZB_NVRAM_ADDR_MAP,
                 t_zboss.DSNwkAddrMap
             )
         for rec in map:
             if rec.nwk_addr == 0x0000:
                 continue
-            self.state.network_info.children.append(rec.ieee_addr)
+            if rec.ieee_addr not in self.state.network_info.children:
+                self.state.network_info.children.append(rec.ieee_addr)
             self.state.network_info.nwk_addresses[rec.ieee_addr] = rec.nwk_addr
 
         keys = await self._api.nvram.read(
             t_zboss.DatasetId.ZB_NVRAM_APS_SECURE_DATA,
             t_zboss.DSApsSecureKeys
         )
         for key_entry in keys:
@@ -494,14 +495,21 @@
         except asyncio.TimeoutError:
             return False
         else:
             return device_config
         finally:
             zboss.close()
 
+    async def _watchdog_feed(self):
+        """Watchdog loop to periodically test if ZBOSS is still running."""
+        await self._api.request(
+            c.NcpConfig.GetZigbeeRole.Req(TSN=self.get_sequence()),
+            timeout=15
+        )
+
     # Overwrites zigpy because of custom ZDO layer required for ZBOSS.
     def add_device(self, ieee: t.EUI64, nwk: t.NWK):
         """Create zigpy `Device` object with the provided IEEE and NWK addr."""
         assert isinstance(ieee, t.EUI64)
         # TODO: Shut down existing device
 
         dev = ZbossDevice(self, ieee, nwk)
@@ -549,16 +557,15 @@
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
         elif msg.Status == t_zboss.DeviceUpdateStatus.unsecured_join:
             # 0x000 as parent device, currently unused
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
         elif msg.Status == t_zboss.DeviceUpdateStatus.device_left:
-            pass
-            # self.handle_leave(msg.Nwk, msg.IEEE)
+            self.handle_leave(msg.Nwk, msg.IEEE)
         elif msg.Status == t_zboss.DeviceUpdateStatus.tc_rejoin:
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
 
     def on_apsde_indication(self, msg):
         """APSDE-DATA.indication handler."""
         is_broadcast = bool(msg.FrameFC & t_zboss.APSFrameFC.Broadcast)
```

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss/zigbee/device.py` & `zigpy_zboss-1.1.5/zigpy_zboss/zigbee/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,47 +245,50 @@
             self,
             packet: t.ZigbeePacket,
             zdo_hdr: zdo_t.ZDOHeader,
             zdo_args: tuple[Any]) -> None:
         """Send ZDO IEEE addr request and handle the response."""
         tsn = zdo_hdr.tsn
         nwki, req_type, index = zdo_args
-        res = await self._api.request(
+        res = await self._device._application._api.request(
             c.ZDO.IeeeAddrReq.Req(
                 TSN=tsn,
                 DstNWK=packet.dst.address,
                 NWKtoMatch=nwki,
                 RequestType=req_type,
                 StartIndex=index,
-                )
+                ),
+            timeout=70,
         )
 
         if res.StatusCode:
             # ZDO command failed, use dummy values.
             ieee = t.EUI64([0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff])
             nwki = t.NWK(0xffff)
+            src_ad = t.NWK(0x0000)
         else:
             ieee = res.RemoteDevIEEE
             nwki = res.RemoteDevNWK
+            src_ad = res.RemoteDevNWK
 
         status = zdo_t.Status(res.StatusCode)
         data = tsn.serialize() \
             + status.serialize() \
             + ieee.serialize() \
             + nwki.serialize()
 
         packet = t.ZigbeePacket(
             src=t.AddrModeAddress(
                 addr_mode=t.AddrMode.NWK,
-                address=res.RemoteDevNWK,
+                address=src_ad,
             ),
             src_ep=0,
             dst=t.AddrModeAddress(
                 addr_mode=t.AddrMode.NWK,
-                address=self.state.node_info.nwk,
+                address=t.NWK(0x0000),
             ),
             dst_ep=0,
             tsn=tsn,
             profile_id=0,
             cluster_id=zdo_t.ZDOCmd.IEEE_addr_rsp,
             data=t.SerializableBytes(data),
             tx_options=t.TransmitOptions.NONE,
```

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss.egg-info/PKG-INFO` & `zigpy_zboss-1.1.5/zigpy_zboss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `zigpy-zboss-1.1.4/zigpy_zboss.egg-info/SOURCES.txt` & `zigpy_zboss-1.1.5/zigpy_zboss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

