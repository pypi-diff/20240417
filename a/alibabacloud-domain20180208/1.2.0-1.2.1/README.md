# Comparing `tmp/alibabacloud_domain20180208-1.2.0.tar.gz` & `tmp/alibabacloud_domain20180208-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_domain20180208-1.2.0.tar", last modified: Mon Mar 25 17:12:24 2024, max compression
+gzip compressed data, was "dist/alibabacloud_domain20180208-1.2.1.tar", last modified: Wed Apr 17 03:25:09 2024, max compression
```

## Comparing `alibabacloud_domain20180208-1.2.0.tar` & `alibabacloud_domain20180208-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      194 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2423 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1192 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82269 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/client.py
--rw-r--r--   0 root         (0) root         (0)   141718 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2423 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2627 2024-03-25 17:12:24.000000 alibabacloud_domain20180208-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82269 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/client.py
+-rw-r--r--   0 root         (0) root         (0)   141960 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 03:25:09.000000 alibabacloud_domain20180208-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-04-17 03:25:08.000000 alibabacloud_domain20180208-1.2.1/setup.py
```

### Comparing `alibabacloud_domain20180208-1.2.0/LICENSE` & `alibabacloud_domain20180208-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208-1.2.0/PKG-INFO` & `alibabacloud_domain20180208-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_domain20180208
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Domains (20180208) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180208-1.2.0/README-CN.md` & `alibabacloud_domain20180208-1.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208-1.2.0/README.md` & `alibabacloud_domain20180208-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/client.py` & `alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208/models.py` & `alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2515,22 +2515,24 @@
         self,
         auction_id: int = None,
         book_end_time: int = None,
         currency: str = None,
         max_bid: float = None,
         partner_type: str = None,
         request_id: str = None,
+        snatch_no: str = None,
         transfer_in_price: float = None,
     ):
         self.auction_id = auction_id
         self.book_end_time = book_end_time
         self.currency = currency
         self.max_bid = max_bid
         self.partner_type = partner_type
         self.request_id = request_id
+        self.snatch_no = snatch_no
         self.transfer_in_price = transfer_in_price
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2546,14 +2548,16 @@
             result['Currency'] = self.currency
         if self.max_bid is not None:
             result['MaxBid'] = self.max_bid
         if self.partner_type is not None:
             result['PartnerType'] = self.partner_type
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.snatch_no is not None:
+            result['SnatchNo'] = self.snatch_no
         if self.transfer_in_price is not None:
             result['TransferInPrice'] = self.transfer_in_price
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AuctionId') is not None:
@@ -2564,14 +2568,16 @@
             self.currency = m.get('Currency')
         if m.get('MaxBid') is not None:
             self.max_bid = m.get('MaxBid')
         if m.get('PartnerType') is not None:
             self.partner_type = m.get('PartnerType')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('SnatchNo') is not None:
+            self.snatch_no = m.get('SnatchNo')
         if m.get('TransferInPrice') is not None:
             self.transfer_in_price = m.get('TransferInPrice')
         return self
 
 
 class QueryBookingDomainInfoResponse(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_domain20180208-1.2.0/alibabacloud_domain20180208.egg-info/PKG-INFO` & `alibabacloud_domain20180208-1.2.1/alibabacloud_domain20180208.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-domain20180208
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Domains (20180208) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180208-1.2.0/setup.py` & `alibabacloud_domain20180208-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_domain20180208.
 
-Created on 25/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_domain20180208"
 NAME = "alibabacloud_domain20180208" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Domains (20180208) SDK Library for Python"
```

