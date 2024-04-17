# Comparing `tmp/panos_upgrade_assurance-0.3.5.tar.gz` & `tmp/panos_upgrade_assurance-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.3.5.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.3.6.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.3.5.tar` & `panos_upgrade_assurance-0.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/LICENSE
--rw-r--r--   0        0        0     1679 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/README.md
--rw-r--r--   0        0        0       76 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    67339 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0     2869 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/exceptions.py
--rw-r--r--   0        0        0    60521 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    31975 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    13150 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0     1370 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-17 01:29:37.581799 panos_upgrade_assurance-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1679 2024-04-17 01:29:37.581799 panos_upgrade_assurance-0.3.6/README.md
+-rw-r--r--   0        0        0       76 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    67339 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2869 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    60578 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31975 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    13150 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1370 2024-04-17 01:29:37.585799 panos_upgrade_assurance-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.3.6/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.3.5/LICENSE` & `panos_upgrade_assurance-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/README.md` & `panos_upgrade_assurance-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/check_firewall.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/exceptions.py` & `panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,14 +694,18 @@
         dict: BGP peers information.
 
         """
 
         response = self.op_parser(cmd="show routing protocol bgp peer")
 
         result = {}
+
+        if response is None:
+            return result
+
         if "entry" in response:
             bgp_peers = response["entry"]
             for peer in bgp_peers if isinstance(bgp_peers, list) else [bgp_peers]:
                 result[
                     f"{peer['@vr'].replace(' ', '-')}_{peer['peer-group'].replace(' ', '-')}_{peer['@peer'].replace(' ', '-')}"
                 ] = dict(peer)
```

### Comparing `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.3.6/panos_upgrade_assurance/utils.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.5/pyproject.toml` & `panos_upgrade_assurance-0.3.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
```

### Comparing `panos_upgrade_assurance-0.3.5/PKG-INFO` & `panos_upgrade_assurance-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

