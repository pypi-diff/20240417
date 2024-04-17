# Comparing `tmp/alibabacloud_domain20180208_py2-1.2.0.tar.gz` & `tmp/alibabacloud_domain20180208_py2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_domain20180208_py2-1.2.0.tar", last modified: Mon Mar 25 17:10:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_domain20180208_py2-1.2.1.tar", last modified: Wed Apr 17 03:24:37 2024, max compression
```

## Comparing `alibabacloud_domain20180208_py2-1.2.0.tar` & `alibabacloud_domain20180208_py2-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      195 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33328 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/client.py
--rw-r--r--   0 root         (0) root         (0)   142460 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2919 2024-03-25 17:10:17.000000 alibabacloud_domain20180208_py2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      375 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33328 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/client.py
+-rw-r--r--   0 root         (0) root         (0)   142700 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 03:24:37.000000 alibabacloud_domain20180208_py2-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-17 03:24:36.000000 alibabacloud_domain20180208_py2-1.2.1/setup.py
```

### Comparing `alibabacloud_domain20180208_py2-1.2.0/LICENSE` & `alibabacloud_domain20180208_py2-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208_py2-1.2.0/PKG-INFO` & `alibabacloud_domain20180208_py2-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_domain20180208_py2
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Domains (20180208) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180208_py2-1.2.0/README-CN.md` & `alibabacloud_domain20180208_py2-1.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208_py2-1.2.0/README.md` & `alibabacloud_domain20180208_py2-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/client.py` & `alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208/models.py` & `alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2192,21 +2192,22 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class QueryBookingDomainInfoResponseBody(TeaModel):
     def __init__(self, auction_id=None, book_end_time=None, currency=None, max_bid=None, partner_type=None,
-                 request_id=None, transfer_in_price=None):
+                 request_id=None, snatch_no=None, transfer_in_price=None):
         self.auction_id = auction_id  # type: int
         self.book_end_time = book_end_time  # type: long
         self.currency = currency  # type: str
         self.max_bid = max_bid  # type: float
         self.partner_type = partner_type  # type: str
         self.request_id = request_id  # type: str
+        self.snatch_no = snatch_no  # type: str
         self.transfer_in_price = transfer_in_price  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(QueryBookingDomainInfoResponseBody, self).to_map()
@@ -2222,14 +2223,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AuctionId') is not None:
@@ -2240,14 +2243,16 @@
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
     def __init__(self, headers=None, status_code=None, body=None):
```

### Comparing `alibabacloud_domain20180208_py2-1.2.0/alibabacloud_domain20180208_py2.egg-info/PKG-INFO` & `alibabacloud_domain20180208_py2-1.2.1/alibabacloud_domain20180208_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-domain20180208-py2
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Domains (20180208) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180208_py2-1.2.0/setup.py` & `alibabacloud_domain20180208_py2-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_domain20180208_py2.
 
-Created on 25/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_domain20180208"
 NAME = "alibabacloud_domain20180208_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Domains (20180208) SDK Library for Python2"
```

