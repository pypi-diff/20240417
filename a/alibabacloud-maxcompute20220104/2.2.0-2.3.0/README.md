# Comparing `tmp/alibabacloud_maxcompute20220104-2.2.0.tar.gz` & `tmp/alibabacloud_maxcompute20220104-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_maxcompute20220104-2.2.0.tar", last modified: Wed Feb 28 17:21:38 2024, max compression
+gzip compressed data, was "dist/alibabacloud_maxcompute20220104-2.3.0.tar", last modified: Wed Apr 17 17:13:11 2024, max compression
```

## Comparing `alibabacloud_maxcompute20220104-2.2.0.tar` & `alibabacloud_maxcompute20220104-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/
--rw-r--r--   0 root         (0) root         (0)      655 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/__init__.py
--rw-r--r--   0 root         (0) root         (0)   122733 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/client.py
--rw-r--r--   0 root         (0) root         (0)   428910 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-02-28 17:21:38.000000 alibabacloud_maxcompute20220104-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)      767 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122733 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/client.py
+-rw-r--r--   0 root         (0) root         (0)   429506 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:13:11.000000 alibabacloud_maxcompute20220104-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-17 17:13:10.000000 alibabacloud_maxcompute20220104-2.3.0/setup.py
```

### Comparing `alibabacloud_maxcompute20220104-2.2.0/ChangeLog.md` & `alibabacloud_maxcompute20220104-2.3.0/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-02-28 Version: 2.2.0
+- Support API GetTableInfo.
+
+
+2024-02-28 Version: 2.2.0
+- Support API GetTableInfo.
+
+
 2024-01-08 Version: 2.1.1
 - Generated python 2022-01-04 for MaxCompute.
 
 2023-12-11 Version: 2.1.0
 - Generated python 2022-01-04 for MaxCompute.
 
 2023-12-10 Version: 2.0.4
```

### Comparing `alibabacloud_maxcompute20220104-2.2.0/LICENSE` & `alibabacloud_maxcompute20220104-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-2.2.0/PKG-INFO` & `alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_maxcompute20220104
-Version: 2.2.0
+Name: alibabacloud-maxcompute20220104
+Version: 2.3.0
 Summary: Alibaba Cloud MaxCompute (20220104) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_maxcompute20220104-2.2.0/README-CN.md` & `alibabacloud_maxcompute20220104-2.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-2.2.0/README.md` & `alibabacloud_maxcompute20220104-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/client.py` & `alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104/models.py` & `alibabacloud_maxcompute20220104-2.3.0/alibabacloud_maxcompute20220104/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1624,34 +1624,38 @@
 
 class GetProjectResponseBodyDataProperties(TeaModel):
     def __init__(
         self,
         allow_full_scan: bool = None,
         elder_tunnel_quota: str = None,
         enable_decimal_2: bool = None,
+        enable_fdc_cache_force: bool = None,
         enable_tunnel_quota_route: bool = None,
         encryption: GetProjectResponseBodyDataPropertiesEncryption = None,
+        fdc_quota: str = None,
         retention_days: int = None,
         sql_metering_max: str = None,
         storage_tier_info: GetProjectResponseBodyDataPropertiesStorageTierInfo = None,
         table_lifecycle: GetProjectResponseBodyDataPropertiesTableLifecycle = None,
         timezone: str = None,
         tunnel_quota: str = None,
         type_system: str = None,
     ):
         # Indicates whether a full table scan on the project is enabled.
         self.allow_full_scan = allow_full_scan
         # This operation does not return a value for this parameter.
         self.elder_tunnel_quota = elder_tunnel_quota
         # Indicates whether the DECIMAL data type in MaxCompute V2.0 is enabled.
         self.enable_decimal_2 = enable_decimal_2
+        self.enable_fdc_cache_force = enable_fdc_cache_force
         # Indicates whether tunnel quota routing is enabled.
         self.enable_tunnel_quota_route = enable_tunnel_quota_route
         # The encryption information.
         self.encryption = encryption
+        self.fdc_quota = fdc_quota
         # The number of days for which backup data can be retained.
         self.retention_days = retention_days
         # The upper limit for the resources that are consumed by an SQL statement.
         self.sql_metering_max = sql_metering_max
         # The information about the tiered storage.
         self.storage_tier_info = storage_tier_info
         # The lifecycle of the table in the project.
@@ -1679,18 +1683,22 @@
         result = dict()
         if self.allow_full_scan is not None:
             result['allowFullScan'] = self.allow_full_scan
         if self.elder_tunnel_quota is not None:
             result['elderTunnelQuota'] = self.elder_tunnel_quota
         if self.enable_decimal_2 is not None:
             result['enableDecimal2'] = self.enable_decimal_2
+        if self.enable_fdc_cache_force is not None:
+            result['enableFdcCacheForce'] = self.enable_fdc_cache_force
         if self.enable_tunnel_quota_route is not None:
             result['enableTunnelQuotaRoute'] = self.enable_tunnel_quota_route
         if self.encryption is not None:
             result['encryption'] = self.encryption.to_map()
+        if self.fdc_quota is not None:
+            result['fdcQuota'] = self.fdc_quota
         if self.retention_days is not None:
             result['retentionDays'] = self.retention_days
         if self.sql_metering_max is not None:
             result['sqlMeteringMax'] = self.sql_metering_max
         if self.storage_tier_info is not None:
             result['storageTierInfo'] = self.storage_tier_info.to_map()
         if self.table_lifecycle is not None:
@@ -1707,19 +1715,23 @@
         m = m or dict()
         if m.get('allowFullScan') is not None:
             self.allow_full_scan = m.get('allowFullScan')
         if m.get('elderTunnelQuota') is not None:
             self.elder_tunnel_quota = m.get('elderTunnelQuota')
         if m.get('enableDecimal2') is not None:
             self.enable_decimal_2 = m.get('enableDecimal2')
+        if m.get('enableFdcCacheForce') is not None:
+            self.enable_fdc_cache_force = m.get('enableFdcCacheForce')
         if m.get('enableTunnelQuotaRoute') is not None:
             self.enable_tunnel_quota_route = m.get('enableTunnelQuotaRoute')
         if m.get('encryption') is not None:
             temp_model = GetProjectResponseBodyDataPropertiesEncryption()
             self.encryption = temp_model.from_map(m['encryption'])
+        if m.get('fdcQuota') is not None:
+            self.fdc_quota = m.get('fdcQuota')
         if m.get('retentionDays') is not None:
             self.retention_days = m.get('retentionDays')
         if m.get('sqlMeteringMax') is not None:
             self.sql_metering_max = m.get('sqlMeteringMax')
         if m.get('storageTierInfo') is not None:
             temp_model = GetProjectResponseBodyDataPropertiesStorageTierInfo()
             self.storage_tier_info = temp_model.from_map(m['storageTierInfo'])
```

### Comparing `alibabacloud_maxcompute20220104-2.2.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO` & `alibabacloud_maxcompute20220104-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-maxcompute20220104
-Version: 2.2.0
+Name: alibabacloud_maxcompute20220104
+Version: 2.3.0
 Summary: Alibaba Cloud MaxCompute (20220104) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_maxcompute20220104-2.2.0/setup.py` & `alibabacloud_maxcompute20220104-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_maxcompute20220104.
 
-Created on 28/02/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_maxcompute20220104"
 NAME = "alibabacloud_maxcompute20220104" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MaxCompute (20220104) SDK Library for Python"
```

