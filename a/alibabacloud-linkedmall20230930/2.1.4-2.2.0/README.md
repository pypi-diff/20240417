# Comparing `tmp/alibabacloud_linkedmall20230930-2.1.4.tar.gz` & `tmp/alibabacloud_linkedmall20230930-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.1.4.tar", last modified: Fri Apr 12 05:36:11 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.2.0.tar", last modified: Wed Apr 17 02:54:43 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930-2.1.4.tar` & `alibabacloud_linkedmall20230930-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/
--rw-r--r--   0 root         (0) root         (0)      527 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63190 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   157477 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65926 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   159384 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/setup.py
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/ChangeLog.md` & `alibabacloud_linkedmall20230930-2.2.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-12 Version: 2.1.4
+- Generated python 2023-09-30 for linkedmall.
+
 2024-04-08 Version: 2.1.3
 - Generated python 2023-09-30 for linkedmall.
 
 2024-03-29 Version: 2.1.2
 - Update API GetSelectionProduct: update param divisionCode.
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/LICENSE` & `alibabacloud_linkedmall20230930-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.4/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_linkedmall20230930
-Version: 2.1.4
+Name: alibabacloud-linkedmall20230930
+Version: 2.2.0
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/README-CN.md` & `alibabacloud_linkedmall20230930-2.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.4/README.md` & `alibabacloud_linkedmall20230930-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1590,7 +1590,77 @@
     async def render_refund_order_async(
         self,
         request: linkedmall_20230930_models.RenderRefundOrderRequest,
     ) -> linkedmall_20230930_models.RenderRefundOrderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.render_refund_order_with_options_async(request, headers, runtime)
+
+    def split_purchase_order_with_options(
+        self,
+        request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        UtilClient.validate_model(request)
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(request.body)
+        )
+        params = open_api_models.Params(
+            action='SplitPurchaseOrder',
+            version='2023-09-30',
+            protocol='HTTPS',
+            pathname=f'/opensaas-s2b/opensaas-s2b-biz-trade/v2/purchaseOrders/commands/split',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            linkedmall_20230930_models.SplitPurchaseOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def split_purchase_order_with_options_async(
+        self,
+        request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        UtilClient.validate_model(request)
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(request.body)
+        )
+        params = open_api_models.Params(
+            action='SplitPurchaseOrder',
+            version='2023-09-30',
+            protocol='HTTPS',
+            pathname=f'/opensaas-s2b/opensaas-s2b-biz-trade/v2/purchaseOrders/commands/split',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            linkedmall_20230930_models.SplitPurchaseOrderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def split_purchase_order(
+        self,
+        request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
+    ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.split_purchase_order_with_options(request, headers, runtime)
+
+    async def split_purchase_order_async(
+        self,
+        request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
+    ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.split_purchase_order_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4936,7 +4936,77 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RefundRenderResult()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SplitPurchaseOrderRequest(TeaModel):
+    def __init__(
+        self,
+        body: PurchaseOrderRenderQuery = None,
+    ):
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('body') is not None:
+            temp_model = PurchaseOrderRenderQuery()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SplitPurchaseOrderResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PurchaseOrderRenderResult = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = PurchaseOrderRenderResult()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-linkedmall20230930
-Version: 2.1.4
+Name: alibabacloud_linkedmall20230930
+Version: 2.2.0
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.4/setup.py` & `alibabacloud_linkedmall20230930-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930.
 
-Created on 12/04/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python"
```

