# Comparing `tmp/alibabacloud_cloud-siem20220616-3.0.4.tar.gz` & `tmp/alibabacloud_cloud-siem20220616-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloud-siem20220616-3.0.4.tar", last modified: Wed Mar 27 07:07:49 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloud-siem20220616-3.0.5.tar", last modified: Wed Apr 17 17:15:00 2024, max compression
```

## Comparing `alibabacloud_cloud-siem20220616-3.0.4.tar` & `alibabacloud_cloud-siem20220616-3.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/
--rw-r--r--   0 root         (0) root         (0)      695 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   357564 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   849185 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2648 2024-03-27 07:07:49.000000 alibabacloud_cloud-siem20220616-3.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/
+-rw-r--r--   0 root         (0) root         (0)      840 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   385500 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   887867 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/setup.py
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/LICENSE` & `alibabacloud_cloud-siem20220616-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/PKG-INFO` & `alibabacloud_cloud-siem20220616-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloud-siem20220616
-Version: 3.0.4
+Version: 3.0.5
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/README-CN.md` & `alibabacloud_cloud-siem20220616-3.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/README.md` & `alibabacloud_cloud-siem20220616-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/client.py` & `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -636,14 +636,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_code):
             body['LogCode'] = request.log_code
         if not UtilClient.is_unset(request.product_code):
             body['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CloseDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -668,14 +672,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_code):
             body['LogCode'] = request.log_code
         if not UtilClient.is_unset(request.product_code):
             body['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CloseDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -712,14 +720,18 @@
     ) -> cloud_siem_20220616_models.DeleteAutomateResponseConfigResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteAutomateResponseConfig',
             version='2022-06-16',
             protocol='HTTPS',
@@ -742,14 +754,18 @@
     ) -> cloud_siem_20220616_models.DeleteAutomateResponseConfigResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteAutomateResponseConfig',
             version='2022-06-16',
             protocol='HTTPS',
@@ -870,14 +886,18 @@
         request: cloud_siem_20220616_models.DeleteCustomizeRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DeleteCustomizeRuleResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_id):
             body['RuleId'] = request.rule_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteCustomizeRule',
@@ -900,14 +920,18 @@
         request: cloud_siem_20220616_models.DeleteCustomizeRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DeleteCustomizeRuleResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_id):
             body['RuleId'] = request.rule_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteCustomizeRule',
@@ -1262,14 +1286,18 @@
     ) -> cloud_siem_20220616_models.DeleteWhiteRuleListResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteWhiteRuleList',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1292,14 +1320,18 @@
     ) -> cloud_siem_20220616_models.DeleteWhiteRuleListResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteWhiteRuleList',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1334,14 +1366,18 @@
         request: cloud_siem_20220616_models.DescribeAggregateFunctionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAggregateFunctionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAggregateFunction',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1362,14 +1398,18 @@
         request: cloud_siem_20220616_models.DescribeAggregateFunctionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAggregateFunctionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAggregateFunction',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1404,14 +1444,18 @@
         request: cloud_siem_20220616_models.DescribeAlertSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAlertSceneResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertScene',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1432,14 +1476,18 @@
         request: cloud_siem_20220616_models.DescribeAlertSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAlertSceneResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertScene',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1476,14 +1524,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertSceneByEventResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSceneByEvent',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1506,14 +1558,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertSceneByEventResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSceneByEvent',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1552,14 +1608,18 @@
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSource',
@@ -1586,14 +1646,18 @@
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSource',
@@ -1632,14 +1696,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertSourceWithEventResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSourceWithEvent',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1662,14 +1730,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertSourceWithEventResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertSourceWithEvent',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1704,14 +1776,20 @@
         request: cloud_siem_20220616_models.DescribeAlertTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAlertTypeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.rule_type):
+            body['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertType',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1732,14 +1810,20 @@
         request: cloud_siem_20220616_models.DescribeAlertTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAlertTypeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.rule_type):
+            body['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertType',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1788,14 +1872,18 @@
             body['IsDefend'] = request.is_defend
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source):
             body['Source'] = request.source
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
@@ -1836,14 +1924,18 @@
             body['IsDefend'] = request.is_defend
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source):
             body['Source'] = request.source
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
@@ -1886,14 +1978,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertsCountResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertsCount',
@@ -1918,14 +2014,18 @@
     ) -> cloud_siem_20220616_models.DescribeAlertsCountResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertsCount',
@@ -1970,14 +2070,18 @@
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertsWithEntity',
@@ -2008,14 +2112,18 @@
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAlertsWithEntity',
@@ -2064,14 +2172,18 @@
             body['IsDefend'] = request.is_defend
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source):
             body['Source'] = request.source
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2108,14 +2220,18 @@
             body['IsDefend'] = request.is_defend
         if not UtilClient.is_unset(request.level):
             body['Level'] = request.level
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source):
             body['Source'] = request.source
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2160,14 +2276,18 @@
             body['AssetName'] = request.asset_name
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAttackTimeLine',
@@ -2196,14 +2316,18 @@
             body['AssetName'] = request.asset_name
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAttackTimeLine',
@@ -2310,14 +2434,18 @@
         request: cloud_siem_20220616_models.DescribeAutomateResponseConfigCounterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAutomateResponseConfigCounterResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigCounter',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2338,14 +2466,18 @@
         request: cloud_siem_20220616_models.DescribeAutomateResponseConfigCounterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeAutomateResponseConfigCounterResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigCounter',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2382,14 +2514,18 @@
     ) -> cloud_siem_20220616_models.DescribeAutomateResponseConfigFeatureResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_response_type):
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigFeature',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2412,14 +2548,18 @@
     ) -> cloud_siem_20220616_models.DescribeAutomateResponseConfigFeatureResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_response_type):
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigFeature',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2458,14 +2598,18 @@
         body = {}
         if not UtilClient.is_unset(request.auto_response_type):
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.entity_type):
             body['EntityType'] = request.entity_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigPlayBooks',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2490,14 +2634,18 @@
         body = {}
         if not UtilClient.is_unset(request.auto_response_type):
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.entity_type):
             body['EntityType'] = request.entity_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeAutomateResponseConfigPlayBooks',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2540,14 +2688,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemAssets',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2576,14 +2728,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemAssets',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2620,14 +2776,18 @@
     ) -> cloud_siem_20220616_models.DescribeCloudSiemAssetsCounterResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemAssetsCounter',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2650,14 +2810,18 @@
     ) -> cloud_siem_20220616_models.DescribeCloudSiemAssetsCounterResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemAssetsCounter',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2694,14 +2858,18 @@
     ) -> cloud_siem_20220616_models.DescribeCloudSiemEventDetailResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemEventDetail',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2724,14 +2892,18 @@
     ) -> cloud_siem_20220616_models.DescribeCloudSiemEventDetailResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCloudSiemEventDetail',
             version='2022-06-16',
             protocol='HTTPS',
@@ -2782,14 +2954,18 @@
             body['Order'] = request.order
         if not UtilClient.is_unset(request.order_field):
             body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.thread_level):
             body['ThreadLevel'] = request.thread_level
         req = open_api_models.OpenApiRequest(
@@ -2832,14 +3008,18 @@
             body['Order'] = request.order
         if not UtilClient.is_unset(request.order_field):
             body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.thread_level):
             body['ThreadLevel'] = request.thread_level
         req = open_api_models.OpenApiRequest(
@@ -3032,14 +3212,18 @@
         request: cloud_siem_20220616_models.DescribeCustomizeRuleCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleCountResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleCount',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3060,14 +3244,18 @@
         request: cloud_siem_20220616_models.DescribeCustomizeRuleCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleCountResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleCount',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3104,14 +3292,18 @@
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleTest',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3134,14 +3326,18 @@
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleTest',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3178,14 +3374,18 @@
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleTestHistogramResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleTestHistogram',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3208,14 +3408,18 @@
     ) -> cloud_siem_20220616_models.DescribeCustomizeRuleTestHistogramResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCustomizeRuleTestHistogram',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3418,14 +3622,18 @@
             body['EntityType'] = request.entity_type
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeDisposeAndPlaybook',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3454,14 +3662,18 @@
             body['EntityType'] = request.entity_type
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeDisposeAndPlaybook',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3498,14 +3710,18 @@
     ) -> cloud_siem_20220616_models.DescribeDisposeStrategyPlaybookResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeDisposeStrategyPlaybook',
@@ -3530,14 +3746,18 @@
     ) -> cloud_siem_20220616_models.DescribeDisposeStrategyPlaybookResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeDisposeStrategyPlaybook',
@@ -3580,14 +3800,18 @@
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.entity_identity):
             body['EntityIdentity'] = request.entity_identity
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEntityInfo',
@@ -3616,14 +3840,18 @@
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.entity_identity):
             body['EntityIdentity'] = request.entity_identity
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEntityInfo',
@@ -3658,16 +3886,24 @@
     def describe_event_count_by_threat_level_with_options(
         self,
         request: cloud_siem_20220616_models.DescribeEventCountByThreatLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeEventCountByThreatLevelResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEventCountByThreatLevel',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3686,16 +3922,24 @@
     async def describe_event_count_by_threat_level_with_options_async(
         self,
         request: cloud_siem_20220616_models.DescribeEventCountByThreatLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeEventCountByThreatLevelResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEventCountByThreatLevel',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3736,14 +3980,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEventDispose',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3770,14 +4018,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeEventDispose',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3960,14 +4212,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_source):
             body['LogSource'] = request.log_source
         if not UtilClient.is_unset(request.log_type):
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogFields',
             version='2022-06-16',
             protocol='HTTPS',
@@ -3992,14 +4248,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_source):
             body['LogSource'] = request.log_source
         if not UtilClient.is_unset(request.log_type):
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogFields',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4036,14 +4296,18 @@
     ) -> cloud_siem_20220616_models.DescribeLogSourceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.log_type):
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogSource',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4066,14 +4330,18 @@
     ) -> cloud_siem_20220616_models.DescribeLogSourceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.log_type):
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogSource',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4178,14 +4446,18 @@
         request: cloud_siem_20220616_models.DescribeLogTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeLogTypeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogType',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4206,14 +4478,18 @@
         request: cloud_siem_20220616_models.DescribeLogTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeLogTypeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeLogType',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4248,14 +4524,18 @@
         request: cloud_siem_20220616_models.DescribeOperatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeOperatorsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.scene_type):
             body['SceneType'] = request.scene_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeOperators',
@@ -4278,14 +4558,18 @@
         request: cloud_siem_20220616_models.DescribeOperatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeOperatorsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.scene_type):
             body['SceneType'] = request.scene_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeOperators',
@@ -4392,14 +4676,18 @@
         request: cloud_siem_20220616_models.DescribeScopeUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeScopeUsersResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeScopeUsers',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4420,14 +4708,18 @@
         request: cloud_siem_20220616_models.DescribeScopeUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeScopeUsersResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeScopeUsers',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4532,14 +4824,18 @@
         request: cloud_siem_20220616_models.DescribeStorageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeStorage',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4560,14 +4856,18 @@
         request: cloud_siem_20220616_models.DescribeStorageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.DescribeStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeStorage',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4678,14 +4978,18 @@
     ) -> cloud_siem_20220616_models.DescribeWafScopeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.entity_id):
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeWafScope',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4708,14 +5012,18 @@
     ) -> cloud_siem_20220616_models.DescribeWafScopeResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.entity_id):
             body['EntityId'] = request.entity_id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeWafScope',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4760,14 +5068,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeWhiteRuleList',
             version='2022-06-16',
             protocol='HTTPS',
@@ -4798,14 +5110,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeWhiteRuleList',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5010,16 +5326,22 @@
     def enable_access_for_cloud_siem_with_options(
         self,
         request: cloud_siem_20220616_models.EnableAccessForCloudSiemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.EnableAccessForCloudSiemResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.auto_submit):
+            body['AutoSubmit'] = request.auto_submit
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='EnableAccessForCloudSiem',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5038,16 +5360,22 @@
     async def enable_access_for_cloud_siem_with_options_async(
         self,
         request: cloud_siem_20220616_models.EnableAccessForCloudSiemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.EnableAccessForCloudSiemResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.auto_submit):
+            body['AutoSubmit'] = request.auto_submit
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='EnableAccessForCloudSiem',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5152,14 +5480,18 @@
         request: cloud_siem_20220616_models.GetCapacityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.GetCapacityResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetCapacity',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5180,14 +5512,18 @@
         request: cloud_siem_20220616_models.GetCapacityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.GetCapacityResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetCapacity',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5476,14 +5812,18 @@
         request: cloud_siem_20220616_models.GetStorageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.GetStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetStorage',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5504,14 +5844,18 @@
         request: cloud_siem_20220616_models.GetStorageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.GetStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetStorage',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5626,14 +5970,18 @@
             body['CloudCode'] = request.cloud_code
         if not UtilClient.is_unset(request.log_codes):
             body['LogCodes'] = request.log_codes
         if not UtilClient.is_unset(request.prod_code):
             body['ProdCode'] = request.prod_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListAccountsByLog',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5660,14 +6008,18 @@
             body['CloudCode'] = request.cloud_code
         if not UtilClient.is_unset(request.log_codes):
             body['LogCodes'] = request.log_codes
         if not UtilClient.is_unset(request.prod_code):
             body['ProdCode'] = request.prod_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListAccountsByLog',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5702,14 +6054,18 @@
         request: cloud_siem_20220616_models.ListAllProdsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListAllProdsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListAllProds',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5730,14 +6086,18 @@
         request: cloud_siem_20220616_models.ListAllProdsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListAllProdsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListAllProds',
             version='2022-06-16',
             protocol='HTTPS',
@@ -5784,14 +6144,18 @@
             body['Id'] = request.id
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.playbook_uuid):
             body['PlaybookUuid'] = request.playbook_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
@@ -5830,14 +6194,18 @@
             body['Id'] = request.id
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.playbook_uuid):
             body['PlaybookUuid'] = request.playbook_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
@@ -6036,18 +6404,26 @@
             body['AlertType'] = request.alert_type
         if not UtilClient.is_unset(request.current_page):
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
+        if not UtilClient.is_unset(request.order):
+            body['Order'] = request.order
+        if not UtilClient.is_unset(request.order_field):
+            body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
@@ -6084,18 +6460,26 @@
             body['AlertType'] = request.alert_type
         if not UtilClient.is_unset(request.current_page):
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
+        if not UtilClient.is_unset(request.order):
+            body['Order'] = request.order
+        if not UtilClient.is_unset(request.order_field):
+            body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
@@ -6140,24 +6524,38 @@
         request: cloud_siem_20220616_models.ListCloudSiemPredefinedRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListCloudSiemPredefinedRulesResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alert_type):
             body['AlertType'] = request.alert_type
+        if not UtilClient.is_unset(request.att_ck):
+            body['AttCk'] = request.att_ck
         if not UtilClient.is_unset(request.current_page):
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.event_transfer_type):
+            body['EventTransferType'] = request.event_transfer_type
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
+        if not UtilClient.is_unset(request.log_source):
+            body['LogSource'] = request.log_source
+        if not UtilClient.is_unset(request.order):
+            body['Order'] = request.order
+        if not UtilClient.is_unset(request.order_field):
+            body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
@@ -6188,24 +6586,38 @@
         request: cloud_siem_20220616_models.ListCloudSiemPredefinedRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListCloudSiemPredefinedRulesResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alert_type):
             body['AlertType'] = request.alert_type
+        if not UtilClient.is_unset(request.att_ck):
+            body['AttCk'] = request.att_ck
         if not UtilClient.is_unset(request.current_page):
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.event_transfer_type):
+            body['EventTransferType'] = request.event_transfer_type
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
+        if not UtilClient.is_unset(request.log_source):
+            body['LogSource'] = request.log_source
+        if not UtilClient.is_unset(request.order):
+            body['Order'] = request.order
+        if not UtilClient.is_unset(request.order_field):
+            body['OrderField'] = request.order_field
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
@@ -6256,14 +6668,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListCustomizeRuleTestResult',
             version='2022-06-16',
             protocol='HTTPS',
@@ -6290,14 +6706,18 @@
             body['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListCustomizeRuleTestResult',
             version='2022-06-16',
             protocol='HTTPS',
@@ -6488,14 +6908,18 @@
         request: cloud_siem_20220616_models.ListDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListDeliveryResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -6516,14 +6940,18 @@
         request: cloud_siem_20220616_models.ListDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListDeliveryResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -6580,14 +7008,18 @@
             body['PlaybookName'] = request.playbook_name
         if not UtilClient.is_unset(request.playbook_types):
             body['PlaybookTypes'] = request.playbook_types
         if not UtilClient.is_unset(request.playbook_uuid):
             body['PlaybookUuid'] = request.playbook_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -6634,14 +7066,18 @@
             body['PlaybookName'] = request.playbook_name
         if not UtilClient.is_unset(request.playbook_types):
             body['PlaybookTypes'] = request.playbook_types
         if not UtilClient.is_unset(request.playbook_uuid):
             body['PlaybookUuid'] = request.playbook_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.sophon_task_id):
             body['SophonTaskId'] = request.sophon_task_id
         if not UtilClient.is_unset(request.start_time):
             body['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -6684,14 +7120,18 @@
         body = {}
         if not UtilClient.is_unset(request.cloud_code):
             body['CloudCode'] = request.cloud_code
         if not UtilClient.is_unset(request.prod_code):
             body['ProdCode'] = request.prod_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListImportedLogsByProd',
             version='2022-06-16',
             protocol='HTTPS',
@@ -6716,14 +7156,18 @@
         body = {}
         if not UtilClient.is_unset(request.cloud_code):
             body['CloudCode'] = request.cloud_code
         if not UtilClient.is_unset(request.prod_code):
             body['ProdCode'] = request.prod_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListImportedLogsByProd',
             version='2022-06-16',
             protocol='HTTPS',
@@ -7500,14 +7944,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_code):
             body['LogCode'] = request.log_code
         if not UtilClient.is_unset(request.product_code):
             body['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='OpenDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -7532,14 +7980,18 @@
         body = {}
         if not UtilClient.is_unset(request.log_code):
             body['LogCode'] = request.log_code
         if not UtilClient.is_unset(request.product_code):
             body['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='OpenDelivery',
             version='2022-06-16',
             protocol='HTTPS',
@@ -7584,14 +8036,18 @@
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.execution_condition):
             body['ExecutionCondition'] = request.execution_condition
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7626,14 +8082,18 @@
             body['AutoResponseType'] = request.auto_response_type
         if not UtilClient.is_unset(request.execution_condition):
             body['ExecutionCondition'] = request.execution_condition
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_name):
             body['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.sub_user_id):
             body['SubUserId'] = request.sub_user_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7674,14 +8134,16 @@
     ) -> cloud_siem_20220616_models.PostCustomizeRuleResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alert_type):
             body['AlertType'] = request.alert_type
         if not UtilClient.is_unset(request.alert_type_mds):
             body['AlertTypeMds'] = request.alert_type_mds
+        if not UtilClient.is_unset(request.att_ck):
+            body['AttCk'] = request.att_ck
         if not UtilClient.is_unset(request.event_transfer_ext):
             body['EventTransferExt'] = request.event_transfer_ext
         if not UtilClient.is_unset(request.event_transfer_switch):
             body['EventTransferSwitch'] = request.event_transfer_switch
         if not UtilClient.is_unset(request.event_transfer_type):
             body['EventTransferType'] = request.event_transfer_type
         if not UtilClient.is_unset(request.id):
@@ -7694,14 +8156,18 @@
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.log_type_mds):
             body['LogTypeMds'] = request.log_type_mds
         if not UtilClient.is_unset(request.query_cycle):
             body['QueryCycle'] = request.query_cycle
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_condition):
             body['RuleCondition'] = request.rule_condition
         if not UtilClient.is_unset(request.rule_desc):
             body['RuleDesc'] = request.rule_desc
         if not UtilClient.is_unset(request.rule_group):
             body['RuleGroup'] = request.rule_group
         if not UtilClient.is_unset(request.rule_name):
@@ -7736,14 +8202,16 @@
     ) -> cloud_siem_20220616_models.PostCustomizeRuleResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alert_type):
             body['AlertType'] = request.alert_type
         if not UtilClient.is_unset(request.alert_type_mds):
             body['AlertTypeMds'] = request.alert_type_mds
+        if not UtilClient.is_unset(request.att_ck):
+            body['AttCk'] = request.att_ck
         if not UtilClient.is_unset(request.event_transfer_ext):
             body['EventTransferExt'] = request.event_transfer_ext
         if not UtilClient.is_unset(request.event_transfer_switch):
             body['EventTransferSwitch'] = request.event_transfer_switch
         if not UtilClient.is_unset(request.event_transfer_type):
             body['EventTransferType'] = request.event_transfer_type
         if not UtilClient.is_unset(request.id):
@@ -7756,14 +8224,18 @@
             body['LogType'] = request.log_type
         if not UtilClient.is_unset(request.log_type_mds):
             body['LogTypeMds'] = request.log_type_mds
         if not UtilClient.is_unset(request.query_cycle):
             body['QueryCycle'] = request.query_cycle
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_condition):
             body['RuleCondition'] = request.rule_condition
         if not UtilClient.is_unset(request.rule_desc):
             body['RuleDesc'] = request.rule_desc
         if not UtilClient.is_unset(request.rule_group):
             body['RuleGroup'] = request.rule_group
         if not UtilClient.is_unset(request.rule_name):
@@ -7812,14 +8284,18 @@
     ) -> cloud_siem_20220616_models.PostCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.simulated_data):
             body['SimulatedData'] = request.simulated_data
         if not UtilClient.is_unset(request.test_type):
             body['TestType'] = request.test_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7846,14 +8322,18 @@
     ) -> cloud_siem_20220616_models.PostCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.simulated_data):
             body['SimulatedData'] = request.simulated_data
         if not UtilClient.is_unset(request.test_type):
             body['TestType'] = request.test_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7900,14 +8380,18 @@
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.receiver_info):
             body['ReceiverInfo'] = request.receiver_info
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
             body['Remark'] = request.remark
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostEventDisposeAndWhiteruleList',
@@ -7938,14 +8422,18 @@
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.receiver_info):
             body['ReceiverInfo'] = request.receiver_info
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
             body['Remark'] = request.remark
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostEventDisposeAndWhiteruleList',
@@ -7984,14 +8472,18 @@
     ) -> cloud_siem_20220616_models.PostEventWhiteruleListResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.whiterule_list):
             body['WhiteruleList'] = request.whiterule_list
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostEventWhiteruleList',
@@ -8016,14 +8508,18 @@
     ) -> cloud_siem_20220616_models.PostEventWhiteruleListResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.whiterule_list):
             body['WhiteruleList'] = request.whiterule_list
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostEventWhiteruleList',
@@ -8062,14 +8558,18 @@
     ) -> cloud_siem_20220616_models.PostFinishCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostFinishCustomizeRuleTest',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8092,14 +8592,18 @@
     ) -> cloud_siem_20220616_models.PostFinishCustomizeRuleTestResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostFinishCustomizeRuleTest',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8138,14 +8642,18 @@
         body = {}
         if not UtilClient.is_unset(request.ids):
             body['Ids'] = request.ids
         if not UtilClient.is_unset(request.in_use):
             body['InUse'] = request.in_use
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostRuleStatusChange',
@@ -8172,14 +8680,18 @@
         body = {}
         if not UtilClient.is_unset(request.ids):
             body['Ids'] = request.ids
         if not UtilClient.is_unset(request.in_use):
             body['InUse'] = request.in_use
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.rule_type):
             body['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostRuleStatusChange',
@@ -8216,14 +8728,18 @@
         request: cloud_siem_20220616_models.RestoreCapacityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.RestoreCapacityResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='RestoreCapacity',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8244,14 +8760,18 @@
         request: cloud_siem_20220616_models.RestoreCapacityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.RestoreCapacityResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='RestoreCapacity',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8366,14 +8886,18 @@
     ) -> cloud_siem_20220616_models.SetStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region):
             body['Region'] = request.region
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.ttl):
             body['Ttl'] = request.ttl
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='SetStorage',
@@ -8398,14 +8922,18 @@
     ) -> cloud_siem_20220616_models.SetStorageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region):
             body['Region'] = request.region
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.ttl):
             body['Ttl'] = request.ttl
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='SetStorage',
@@ -8680,14 +9208,18 @@
         body = {}
         if not UtilClient.is_unset(request.ids):
             body['Ids'] = request.ids
         if not UtilClient.is_unset(request.in_use):
             body['InUse'] = request.in_use
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateAutomateResponseConfigStatus',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8712,14 +9244,18 @@
         body = {}
         if not UtilClient.is_unset(request.ids):
             body['Ids'] = request.ids
         if not UtilClient.is_unset(request.in_use):
             body['InUse'] = request.in_use
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateAutomateResponseConfigStatus',
             version='2022-06-16',
             protocol='HTTPS',
@@ -8758,14 +9294,18 @@
         body = {}
         if not UtilClient.is_unset(request.expression):
             body['Expression'] = request.expression
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.white_rule_id):
             body['WhiteRuleId'] = request.white_rule_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateWhiteRuleList',
@@ -8792,14 +9332,18 @@
         body = {}
         if not UtilClient.is_unset(request.expression):
             body['Expression'] = request.expression
         if not UtilClient.is_unset(request.incident_uuid):
             body['IncidentUuid'] = request.incident_uuid
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.white_rule_id):
             body['WhiteRuleId'] = request.white_rule_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateWhiteRuleList',
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616/models.py` & `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1750,14 +1750,16 @@
 
 class CloseDeliveryRequest(TeaModel):
     def __init__(
         self,
         log_code: str = None,
         product_code: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The log code of the cloud service, such as the code of the process log for Security Center. You can obtain the log code from the response of the ListDelivery operation.
         self.log_code = log_code
         # The code of the cloud service. Valid values:
         # 
         # *   qcloud_waf
         # *   qlcoud_cfw
@@ -1784,14 +1786,16 @@
         # *   polardb
         self.product_code = product_code
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1800,24 +1804,32 @@
         result = dict()
         if self.log_code is not None:
             result['LogCode'] = self.log_code
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('LogCode') is not None:
             self.log_code = m.get('LogCode')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class CloseDeliveryResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
@@ -1897,44 +1909,56 @@
 
 
 class DeleteAutomateResponseConfigRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the rule.
         self.id = id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DeleteAutomateResponseConfigResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -2203,40 +2227,52 @@
         return self
 
 
 class DeleteCustomizeRuleRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_id: int = None,
     ):
         # The region in which the service is deployed.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The ID of the rule.
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_id is not None:
             result['RuleId'] = self.rule_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class DeleteCustomizeRuleResponseBody(TeaModel):
     def __init__(
@@ -2911,44 +2947,56 @@
 
 
 class DeleteWhiteRuleListRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The unique ID of the whitelist rule.
         self.id = id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DeleteWhiteRuleListResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -3048,38 +3096,50 @@
         return self
 
 
 class DescribeAggregateFunctionRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAggregateFunctionResponseBodyData(TeaModel):
     def __init__(
         self,
         function: str = None,
@@ -3222,38 +3282,50 @@
         return self
 
 
 class DescribeAlertSceneRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAlertSceneResponseBodyDataTargets(TeaModel):
     def __init__(
         self,
         name: str = None,
@@ -3489,44 +3561,56 @@
 
 
 class DescribeAlertSceneByEventRequest(TeaModel):
     def __init__(
         self,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAlertSceneByEventResponseBodyDataTargets(TeaModel):
     def __init__(
         self,
         name: str = None,
@@ -3763,14 +3847,16 @@
 
 class DescribeAlertSourceRequest(TeaModel):
     def __init__(
         self,
         end_time: int = None,
         level: List[str] = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         start_time: int = None,
     ):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
         # The risk levels. The value is a JSON array. Valid values:
         # 
         # *   serious: high
@@ -3778,14 +3864,16 @@
         # *   remind: low
         self.level = level
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3796,26 +3884,34 @@
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.level is not None:
             result['Level'] = self.level
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('Level') is not None:
             self.level = m.get('Level')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAlertSourceResponseBodyData(TeaModel):
     def __init__(
@@ -3961,44 +4057,56 @@
 
 
 class DescribeAlertSourceWithEventRequest(TeaModel):
     def __init__(
         self,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAlertSourceWithEventResponseBodyData(TeaModel):
     def __init__(
         self,
         source: str = None,
@@ -4141,38 +4249,56 @@
         return self
 
 
 class DescribeAlertTypeRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
+        rule_type: str = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
+        self.rule_type = rule_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
+        if self.rule_type is not None:
+            result['RuleType'] = self.rule_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
+        if m.get('RuleType') is not None:
+            self.rule_type = m.get('RuleType')
         return self
 
 
 class DescribeAlertTypeResponseBodyData(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
@@ -4322,14 +4448,16 @@
         alert_uuid: str = None,
         current_page: int = None,
         end_time: int = None,
         is_defend: str = None,
         level: List[str] = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         source: str = None,
         start_time: int = None,
         sub_user_id: str = None,
     ):
         # The title of the alert.
         self.alert_title = alert_title
         # The UUID of the alert.
@@ -4352,14 +4480,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The source of the alert.
         self.source = source
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
         # The ID of the Alibaba Cloud account within which the alert is generated.
         self.sub_user_id = sub_user_id
 
@@ -4384,14 +4514,18 @@
             result['IsDefend'] = self.is_defend
         if self.level is not None:
             result['Level'] = self.level
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.source is not None:
             result['Source'] = self.source
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.sub_user_id is not None:
             result['SubUserId'] = self.sub_user_id
         return result
@@ -4410,14 +4544,18 @@
             self.is_defend = m.get('IsDefend')
         if m.get('Level') is not None:
             self.level = m.get('Level')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('Source') is not None:
             self.source = m.get('Source')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         return self
@@ -4920,23 +5058,27 @@
 
 
 class DescribeAlertsCountRequest(TeaModel):
     def __init__(
         self,
         end_time: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         start_time: int = None,
     ):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4945,24 +5087,32 @@
             return _map
 
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAlertsCountResponseBodyData(TeaModel):
     def __init__(
@@ -5126,14 +5276,16 @@
     def __init__(
         self,
         current_page: int = None,
         entity_id: int = None,
         incident_uuid: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         sophon_task_id: str = None,
     ):
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The ID of the entity.
         self.entity_id = entity_id
         # The UUID of the event.
@@ -5141,14 +5293,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The ID of the SOAR handing policy.
         self.sophon_task_id = sophon_task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5163,14 +5317,18 @@
             result['EntityId'] = self.entity_id
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.sophon_task_id is not None:
             result['SophonTaskId'] = self.sophon_task_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CurrentPage') is not None:
@@ -5179,14 +5337,18 @@
             self.entity_id = m.get('EntityId')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SophonTaskId') is not None:
             self.sophon_task_id = m.get('SophonTaskId')
         return self
 
 
 class DescribeAlertsWithEntityResponseBodyDataPageInfo(TeaModel):
     def __init__(
@@ -5690,14 +5852,16 @@
         alert_title: str = None,
         current_page: int = None,
         incident_uuid: str = None,
         is_defend: str = None,
         level: List[str] = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         source: str = None,
         sub_user_id: int = None,
     ):
         # The title of the alert.
         self.alert_title = alert_title
         # The page number. Pages start from page 1.
         self.current_page = current_page
@@ -5717,14 +5881,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The data source of the alert.
         self.source = source
         # The ID of the account within which the alert is generated.
         self.sub_user_id = sub_user_id
 
     def validate(self):
         pass
@@ -5745,14 +5911,18 @@
             result['IsDefend'] = self.is_defend
         if self.level is not None:
             result['Level'] = self.level
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.source is not None:
             result['Source'] = self.source
         if self.sub_user_id is not None:
             result['SubUserId'] = self.sub_user_id
         return result
 
     def from_map(self, m: dict = None):
@@ -5767,14 +5937,18 @@
             self.is_defend = m.get('IsDefend')
         if m.get('Level') is not None:
             self.level = m.get('Level')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('Source') is not None:
             self.source = m.get('Source')
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         return self
 
 
@@ -5882,14 +6056,15 @@
         alert_type_code: str = None,
         alert_type_en: str = None,
         alert_uuid: str = None,
         asset_list: str = None,
         att_ck: str = None,
         cloud_code: str = None,
         end_time: str = None,
+        entity_list: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         incident_uuid: str = None,
         is_defend: str = None,
         log_time: str = None,
         log_uuid: str = None,
@@ -5944,14 +6119,15 @@
         # 
         # *   aliyun: Alibaba Cloud
         # *   qcloud: Tencent Cloud
         # *   hcloud: Huawei Cloud
         self.cloud_code = cloud_code
         # The time when the alert was closed.
         self.end_time = end_time
+        self.entity_list = entity_list
         # The time when the alert was received.
         self.gmt_create = gmt_create
         # The time when the alert was last updated.
         self.gmt_modified = gmt_modified
         # The unique ID of the alert.
         self.id = id
         # The UUID of the event.
@@ -6026,14 +6202,16 @@
             result['AssetList'] = self.asset_list
         if self.att_ck is not None:
             result['AttCk'] = self.att_ck
         if self.cloud_code is not None:
             result['CloudCode'] = self.cloud_code
         if self.end_time is not None:
             result['EndTime'] = self.end_time
+        if self.entity_list is not None:
+            result['EntityList'] = self.entity_list
         if self.gmt_create is not None:
             result['GmtCreate'] = self.gmt_create
         if self.gmt_modified is not None:
             result['GmtModified'] = self.gmt_modified
         if self.id is not None:
             result['Id'] = self.id
         if self.incident_uuid is not None:
@@ -6097,14 +6275,16 @@
             self.asset_list = m.get('AssetList')
         if m.get('AttCk') is not None:
             self.att_ck = m.get('AttCk')
         if m.get('CloudCode') is not None:
             self.cloud_code = m.get('CloudCode')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
+        if m.get('EntityList') is not None:
+            self.entity_list = m.get('EntityList')
         if m.get('GmtCreate') is not None:
             self.gmt_create = m.get('GmtCreate')
         if m.get('GmtModified') is not None:
             self.gmt_modified = m.get('GmtModified')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('IncidentUuid') is not None:
@@ -6277,27 +6457,31 @@
 class DescribeAttackTimeLineRequest(TeaModel):
     def __init__(
         self,
         asset_name: str = None,
         end_time: int = None,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         start_time: int = None,
     ):
         # The name of the asset.
         self.asset_name = asset_name
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
         # The ID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6310,28 +6494,36 @@
             result['AssetName'] = self.asset_name
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AssetName') is not None:
             self.asset_name = m.get('AssetName')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAttackTimeLineResponseBodyData(TeaModel):
     def __init__(
@@ -6720,38 +6912,50 @@
         return self
 
 
 class DescribeAutomateResponseConfigCounterRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAutomateResponseConfigCounterResponseBodyData(TeaModel):
     def __init__(
         self,
         all: int = None,
@@ -6889,47 +7093,59 @@
 
 
 class DescribeAutomateResponseConfigFeatureRequest(TeaModel):
     def __init__(
         self,
         auto_response_type: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auto_response_type is not None:
             result['AutoResponseType'] = self.auto_response_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoResponseType') is not None:
             self.auto_response_type = m.get('AutoResponseType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAutomateResponseConfigFeatureResponseBodyDataRightValueEnums(TeaModel):
     def __init__(
         self,
         value: str = None,
@@ -7220,14 +7436,16 @@
 
 class DescribeAutomateResponseConfigPlayBooksRequest(TeaModel):
     def __init__(
         self,
         auto_response_type: str = None,
         entity_type: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type
         # The entity type of the playbook. Valid values:
@@ -7237,14 +7455,16 @@
         # *   file
         self.entity_type = entity_type
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7253,24 +7473,32 @@
         result = dict()
         if self.auto_response_type is not None:
             result['AutoResponseType'] = self.auto_response_type
         if self.entity_type is not None:
             result['EntityType'] = self.entity_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoResponseType') is not None:
             self.auto_response_type = m.get('AutoResponseType')
         if m.get('EntityType') is not None:
             self.entity_type = m.get('EntityType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAutomateResponseConfigPlayBooksResponseBodyData(TeaModel):
     def __init__(
         self,
         description: str = None,
@@ -7442,14 +7670,16 @@
     def __init__(
         self,
         asset_type: str = None,
         current_page: int = None,
         incident_uuid: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The type of the asset. Valid values:
         # 
         # *   ip
         # *   domain
         # *   url
         # *   process
@@ -7463,14 +7693,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7483,28 +7715,36 @@
             result['CurrentPage'] = self.current_page
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AssetType') is not None:
             self.asset_type = m.get('AssetType')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCloudSiemAssetsResponseBodyDataPageInfo(TeaModel):
     def __init__(
         self,
         current_page: int = None,
@@ -7861,44 +8101,56 @@
 
 
 class DescribeCloudSiemAssetsCounterRequest(TeaModel):
     def __init__(
         self,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCloudSiemAssetsCounterResponseBodyData(TeaModel):
     def __init__(
         self,
         asset_num: int = None,
@@ -8049,44 +8301,56 @@
 
 
 class DescribeCloudSiemEventDetailRequest(TeaModel):
     def __init__(
         self,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCloudSiemEventDetailResponseBodyData(TeaModel):
     def __init__(
         self,
         alert_num: int = None,
@@ -8351,14 +8615,16 @@
         end_time: int = None,
         event_name: str = None,
         incident_uuid: str = None,
         order: str = None,
         order_field: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         start_time: int = None,
         status: int = None,
         thread_level: List[str] = None,
     ):
         # The ID of the asset that is associated with the event.
         self.asset_id = asset_id
         # The page number. Pages start from page 1.
@@ -8382,14 +8648,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handling
         # *   5: handling failed
@@ -8425,14 +8693,18 @@
             result['Order'] = self.order
         if self.order_field is not None:
             result['OrderField'] = self.order_field
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.status is not None:
             result['Status'] = self.status
         if self.thread_level is not None:
             result['ThreadLevel'] = self.thread_level
         return result
@@ -8453,14 +8725,18 @@
             self.order = m.get('Order')
         if m.get('OrderField') is not None:
             self.order_field = m.get('OrderField')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('ThreadLevel') is not None:
             self.thread_level = m.get('ThreadLevel')
         return self
@@ -8520,14 +8796,15 @@
         description_en: str = None,
         ext_content: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         incident_name: str = None,
         incident_name_en: str = None,
         incident_uuid: str = None,
+        refer_account: str = None,
         remark: str = None,
         status: int = None,
         threat_level: str = None,
         threat_score: float = None,
     ):
         # The number of alerts that are associated with the event.
         self.alert_num = alert_num
@@ -8551,14 +8828,15 @@
         self.gmt_modified = gmt_modified
         # The name of the event.
         self.incident_name = incident_name
         # The event name in English.
         self.incident_name_en = incident_name_en
         # The UUID of the event.
         self.incident_uuid = incident_uuid
+        self.refer_account = refer_account
         # The remarks of the event.
         self.remark = remark
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handling
         # *   5: handling failed
@@ -8604,14 +8882,16 @@
             result['GmtModified'] = self.gmt_modified
         if self.incident_name is not None:
             result['IncidentName'] = self.incident_name
         if self.incident_name_en is not None:
             result['IncidentNameEn'] = self.incident_name_en
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
+        if self.refer_account is not None:
+            result['ReferAccount'] = self.refer_account
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.status is not None:
             result['Status'] = self.status
         if self.threat_level is not None:
             result['ThreatLevel'] = self.threat_level
         if self.threat_score is not None:
@@ -8642,14 +8922,16 @@
             self.gmt_modified = m.get('GmtModified')
         if m.get('IncidentName') is not None:
             self.incident_name = m.get('IncidentName')
         if m.get('IncidentNameEn') is not None:
             self.incident_name_en = m.get('IncidentNameEn')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
+        if m.get('ReferAccount') is not None:
+            self.refer_account = m.get('ReferAccount')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('ThreatLevel') is not None:
             self.threat_level = m.get('ThreatLevel')
         if m.get('ThreatScore') is not None:
@@ -9264,87 +9546,147 @@
         return self
 
 
 class DescribeCustomizeRuleCountRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCustomizeRuleCountResponseBodyData(TeaModel):
     def __init__(
         self,
+        aggregation_rule_num: int = None,
+        customize_rule_num: int = None,
+        expert_rule_num: int = None,
+        graph_computing_rule_num: int = None,
         high_rule_num: int = None,
         in_use_rule_num: int = None,
         low_rule_num: int = None,
         medium_rule_num: int = None,
-    ):
+        predefined_rule_num: int = None,
+        single_alert_rule_num: int = None,
+        total_rule_num: int = None,
+        un_event_rule_num: int = None,
+    ):
+        self.aggregation_rule_num = aggregation_rule_num
+        self.customize_rule_num = customize_rule_num
+        self.expert_rule_num = expert_rule_num
+        self.graph_computing_rule_num = graph_computing_rule_num
         # The number of rules that are used to identify high-risk threats.
         self.high_rule_num = high_rule_num
         # The total number of rules.
         self.in_use_rule_num = in_use_rule_num
         # The number of rules that are used to identify low-risk threats.
         self.low_rule_num = low_rule_num
         # The number of rules that are used to identify medium-risk threats.
         self.medium_rule_num = medium_rule_num
+        self.predefined_rule_num = predefined_rule_num
+        self.single_alert_rule_num = single_alert_rule_num
+        self.total_rule_num = total_rule_num
+        self.un_event_rule_num = un_event_rule_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.aggregation_rule_num is not None:
+            result['AggregationRuleNum'] = self.aggregation_rule_num
+        if self.customize_rule_num is not None:
+            result['CustomizeRuleNum'] = self.customize_rule_num
+        if self.expert_rule_num is not None:
+            result['ExpertRuleNum'] = self.expert_rule_num
+        if self.graph_computing_rule_num is not None:
+            result['GraphComputingRuleNum'] = self.graph_computing_rule_num
         if self.high_rule_num is not None:
             result['HighRuleNum'] = self.high_rule_num
         if self.in_use_rule_num is not None:
             result['InUseRuleNum'] = self.in_use_rule_num
         if self.low_rule_num is not None:
             result['LowRuleNum'] = self.low_rule_num
         if self.medium_rule_num is not None:
             result['MediumRuleNum'] = self.medium_rule_num
+        if self.predefined_rule_num is not None:
+            result['PredefinedRuleNum'] = self.predefined_rule_num
+        if self.single_alert_rule_num is not None:
+            result['SingleAlertRuleNum'] = self.single_alert_rule_num
+        if self.total_rule_num is not None:
+            result['TotalRuleNum'] = self.total_rule_num
+        if self.un_event_rule_num is not None:
+            result['UnEventRuleNum'] = self.un_event_rule_num
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AggregationRuleNum') is not None:
+            self.aggregation_rule_num = m.get('AggregationRuleNum')
+        if m.get('CustomizeRuleNum') is not None:
+            self.customize_rule_num = m.get('CustomizeRuleNum')
+        if m.get('ExpertRuleNum') is not None:
+            self.expert_rule_num = m.get('ExpertRuleNum')
+        if m.get('GraphComputingRuleNum') is not None:
+            self.graph_computing_rule_num = m.get('GraphComputingRuleNum')
         if m.get('HighRuleNum') is not None:
             self.high_rule_num = m.get('HighRuleNum')
         if m.get('InUseRuleNum') is not None:
             self.in_use_rule_num = m.get('InUseRuleNum')
         if m.get('LowRuleNum') is not None:
             self.low_rule_num = m.get('LowRuleNum')
         if m.get('MediumRuleNum') is not None:
             self.medium_rule_num = m.get('MediumRuleNum')
+        if m.get('PredefinedRuleNum') is not None:
+            self.predefined_rule_num = m.get('PredefinedRuleNum')
+        if m.get('SingleAlertRuleNum') is not None:
+            self.single_alert_rule_num = m.get('SingleAlertRuleNum')
+        if m.get('TotalRuleNum') is not None:
+            self.total_rule_num = m.get('TotalRuleNum')
+        if m.get('UnEventRuleNum') is not None:
+            self.un_event_rule_num = m.get('UnEventRuleNum')
         return self
 
 
 class DescribeCustomizeRuleCountResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -9447,44 +9789,56 @@
 
 
 class DescribeCustomizeRuleTestRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the rule.
         self.id = id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCustomizeRuleTestResponseBodyData(TeaModel):
     def __init__(
         self,
         id: int = None,
@@ -9635,44 +9989,56 @@
 
 
 class DescribeCustomizeRuleTestHistogramRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the rule.
         self.id = id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCustomizeRuleTestHistogramResponseBodyData(TeaModel):
     def __init__(
         self,
         count: int = None,
@@ -10377,14 +10743,16 @@
     def __init__(
         self,
         current_page: int = None,
         entity_type: str = None,
         incident_uuid: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The entity type. Valid values:
         # 
         # *   ip
         # *   process
@@ -10395,14 +10763,16 @@
         # The number of entries to return on each page. Maximum value: 100.
         self.page_size = page_size
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -10415,28 +10785,36 @@
             result['EntityType'] = self.entity_type
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('EntityType') is not None:
             self.entity_type = m.get('EntityType')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeDisposeAndPlaybookResponseBodyDataPageInfo(TeaModel):
     def __init__(
         self,
         current_page: int = None,
@@ -10795,23 +11173,27 @@
 
 
 class DescribeDisposeStrategyPlaybookRequest(TeaModel):
     def __init__(
         self,
         end_time: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         start_time: int = None,
     ):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -10820,24 +11202,32 @@
             return _map
 
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDisposeStrategyPlaybookResponseBodyData(TeaModel):
     def __init__(
@@ -10985,27 +11375,31 @@
 class DescribeEntityInfoRequest(TeaModel):
     def __init__(
         self,
         entity_id: int = None,
         entity_identity: str = None,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         sophon_task_id: str = None,
     ):
         # The logical ID of the entity.
         self.entity_id = entity_id
         # The feature value of the entity. Fuzzy match is supported.
         self.entity_identity = entity_identity
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The ID of the SOAR handling policy.
         self.sophon_task_id = sophon_task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11018,28 +11412,36 @@
             result['EntityId'] = self.entity_id
         if self.entity_identity is not None:
             result['EntityIdentity'] = self.entity_identity
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.sophon_task_id is not None:
             result['SophonTaskId'] = self.sophon_task_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EntityId') is not None:
             self.entity_id = m.get('EntityId')
         if m.get('EntityIdentity') is not None:
             self.entity_identity = m.get('EntityIdentity')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SophonTaskId') is not None:
             self.sophon_task_id = m.get('SophonTaskId')
         return self
 
 
 class DescribeEntityInfoResponseBodyData(TeaModel):
     def __init__(
@@ -11198,39 +11600,63 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEventCountByThreatLevelRequest(TeaModel):
     def __init__(
         self,
+        end_time: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
+        start_time: int = None,
     ):
+        self.end_time = end_time
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
+        self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeEventCountByThreatLevelResponseBodyData(TeaModel):
     def __init__(
         self,
         event_num: int = None,
@@ -11391,26 +11817,30 @@
 class DescribeEventDisposeRequest(TeaModel):
     def __init__(
         self,
         current_page: int = None,
         incident_uuid: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The number of entries to return on each page. Maximum value: 500.
         self.page_size = page_size
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -11421,26 +11851,34 @@
             result['CurrentPage'] = self.current_page
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeEventDisposeResponseBodyDataReceiverInfo(TeaModel):
     def __init__(
         self,
         channel: str = None,
@@ -12208,24 +12646,28 @@
 
 class DescribeLogFieldsRequest(TeaModel):
     def __init__(
         self,
         log_source: str = None,
         log_type: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The log source of the rule.
         self.log_source = log_source
         # The log type of the rule.
         self.log_type = log_type
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -12234,24 +12676,32 @@
         result = dict()
         if self.log_source is not None:
             result['LogSource'] = self.log_source
         if self.log_type is not None:
             result['LogType'] = self.log_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('LogSource') is not None:
             self.log_source = m.get('LogSource')
         if m.get('LogType') is not None:
             self.log_type = m.get('LogType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeLogFieldsResponseBodyData(TeaModel):
     def __init__(
         self,
         activity_name: str = None,
@@ -12419,44 +12869,56 @@
 
 
 class DescribeLogSourceRequest(TeaModel):
     def __init__(
         self,
         log_type: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The log type of the rule.
         self.log_type = log_type
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.log_type is not None:
             result['LogType'] = self.log_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('LogType') is not None:
             self.log_type = m.get('LogType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeLogSourceResponseBodyData(TeaModel):
     def __init__(
         self,
         log_source: str = None,
@@ -12787,38 +13249,50 @@
         return self
 
 
 class DescribeLogTypeRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeLogTypeResponseBodyData(TeaModel):
     def __init__(
         self,
         log_type: str = None,
@@ -12961,21 +13435,25 @@
         return self
 
 
 class DescribeOperatorsRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         scene_type: str = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The type of the scenario in which the operator is used. Valid values:
         # 
         # *   If you do not specify this parameter, the default scenario is used.
         # *   AGGREGATE: AGGREGATE scenario.
         self.scene_type = scene_type
 
     def validate(self):
@@ -12985,22 +13463,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.scene_type is not None:
             result['SceneType'] = self.scene_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SceneType') is not None:
             self.scene_type = m.get('SceneType')
         return self
 
 
 class DescribeOperatorsResponseBodyData(TeaModel):
     def __init__(
@@ -13331,85 +13817,109 @@
         return self
 
 
 class DescribeScopeUsersRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeScopeUsersResponseBodyData(TeaModel):
     def __init__(
         self,
         ali_uid: int = None,
+        cloud_code: str = None,
         domains: List[str] = None,
         instance_id: str = None,
+        user_id: str = None,
         user_name: str = None,
     ):
         # The ID of the security information and event management (SIEM) user.
         self.ali_uid = ali_uid
+        self.cloud_code = cloud_code
         # An array consisting of the domain names that are protected by the WAF instance.
         self.domains = domains
         # The ID of the Web Application Firewall (WAF) instance.
         self.instance_id = instance_id
+        self.user_id = user_id
         # The username.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.ali_uid is not None:
             result['AliUid'] = self.ali_uid
+        if self.cloud_code is not None:
+            result['CloudCode'] = self.cloud_code
         if self.domains is not None:
             result['Domains'] = self.domains
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
         if self.user_name is not None:
             result['UserName'] = self.user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AliUid') is not None:
             self.ali_uid = m.get('AliUid')
+        if m.get('CloudCode') is not None:
+            self.cloud_code = m.get('CloudCode')
         if m.get('Domains') is not None:
             self.domains = m.get('Domains')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeScopeUsersResponseBody(TeaModel):
     def __init__(
@@ -13629,38 +14139,50 @@
         return self
 
 
 class DescribeStorageRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeStorageResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
@@ -13784,14 +14306,15 @@
         capacity: int = None,
         duration_days: int = None,
         end_time: int = None,
         main_user_id: int = None,
         main_user_name: str = None,
         master_user_id: int = None,
         master_user_name: str = None,
+        rd_order: int = None,
         sas_instance_id: str = None,
         sub_user_id: int = None,
         sub_user_name: str = None,
     ):
         # Indicates whether the logon Alibaba Cloud account can be used to place orders for the threat analysis feature, such as purchase, upgrade, and specifications change orders. Valid values:
         # 
         # *   true
@@ -13807,14 +14330,15 @@
         self.main_user_id = main_user_id
         # The username of the Alibaba Cloud account that is used to purchase the threat analysis feature.
         self.main_user_name = main_user_name
         # The ID of the management account of the resource directory.
         self.master_user_id = master_user_id
         # The display name of the management account of the resource directory.
         self.master_user_name = master_user_name
+        self.rd_order = rd_order
         # The instance ID of Security Center.
         self.sas_instance_id = sas_instance_id
         # The ID of the logon Alibaba Cloud account.
         self.sub_user_id = sub_user_id
         # The username of the logon Alibaba Cloud account.
         self.sub_user_name = sub_user_name
 
@@ -13839,14 +14363,16 @@
             result['MainUserId'] = self.main_user_id
         if self.main_user_name is not None:
             result['MainUserName'] = self.main_user_name
         if self.master_user_id is not None:
             result['MasterUserId'] = self.master_user_id
         if self.master_user_name is not None:
             result['MasterUserName'] = self.master_user_name
+        if self.rd_order is not None:
+            result['RdOrder'] = self.rd_order
         if self.sas_instance_id is not None:
             result['SasInstanceId'] = self.sas_instance_id
         if self.sub_user_id is not None:
             result['SubUserId'] = self.sub_user_id
         if self.sub_user_name is not None:
             result['SubUserName'] = self.sub_user_name
         return result
@@ -13865,14 +14391,16 @@
             self.main_user_id = m.get('MainUserId')
         if m.get('MainUserName') is not None:
             self.main_user_name = m.get('MainUserName')
         if m.get('MasterUserId') is not None:
             self.master_user_id = m.get('MasterUserId')
         if m.get('MasterUserName') is not None:
             self.master_user_name = m.get('MasterUserName')
+        if m.get('RdOrder') is not None:
+            self.rd_order = m.get('RdOrder')
         if m.get('SasInstanceId') is not None:
             self.sas_instance_id = m.get('SasInstanceId')
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         if m.get('SubUserName') is not None:
             self.sub_user_name = m.get('SubUserName')
         return self
@@ -13957,44 +14485,56 @@
 
 
 class DescribeWafScopeRequest(TeaModel):
     def __init__(
         self,
         entity_id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the entity.
         self.entity_id = entity_id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.entity_id is not None:
             result['EntityId'] = self.entity_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EntityId') is not None:
             self.entity_id = m.get('EntityId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeWafScopeResponseBodyData(TeaModel):
     def __init__(
         self,
         aliuid: int = None,
@@ -14149,14 +14689,16 @@
         self,
         alert_name: str = None,
         alert_type: str = None,
         current_page: int = None,
         incident_uuid: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The name of the alert.
         self.alert_name = alert_name
         # The type of the alert.
         self.alert_type = alert_type
         # The page number. Pages start from page 1.
         self.current_page = current_page
@@ -14165,14 +14707,16 @@
         # The number of entries per page. Valid values: 1 to 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -14187,14 +14731,18 @@
             result['CurrentPage'] = self.current_page
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlertName') is not None:
             self.alert_name = m.get('AlertName')
         if m.get('AlertType') is not None:
@@ -14203,14 +14751,18 @@
             self.current_page = m.get('CurrentPage')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeWhiteRuleListResponseBodyDataPageInfo(TeaModel):
     def __init__(
         self,
         current_page: int = None,
@@ -15130,39 +15682,57 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableAccessForCloudSiemRequest(TeaModel):
     def __init__(
         self,
+        auto_submit: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
+        self.auto_submit = auto_submit
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.auto_submit is not None:
+            result['AutoSubmit'] = self.auto_submit
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AutoSubmit') is not None:
+            self.auto_submit = m.get('AutoSubmit')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class EnableAccessForCloudSiemResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
@@ -15348,38 +15918,50 @@
         return self
 
 
 class GetCapacityRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class GetCapacityResponseBodyData(TeaModel):
     def __init__(
         self,
         exist_log_store: bool = None,
@@ -16184,38 +16766,50 @@
         return self
 
 
 class GetStorageRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class GetStorageResponseBodyData(TeaModel):
     def __init__(
         self,
         can_operate: bool = None,
@@ -16577,14 +17171,16 @@
 class ListAccountsByLogRequest(TeaModel):
     def __init__(
         self,
         cloud_code: str = None,
         log_codes: List[str] = None,
         prod_code: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The code that is used for multi-cloud environments.
         # 
         # Valid values:
         # 
         # *   qcloud
         # *   hcloud
@@ -16595,14 +17191,16 @@
         # The code of the service.
         self.prod_code = prod_code
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -16613,26 +17211,34 @@
             result['CloudCode'] = self.cloud_code
         if self.log_codes is not None:
             result['LogCodes'] = self.log_codes
         if self.prod_code is not None:
             result['ProdCode'] = self.prod_code
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CloudCode') is not None:
             self.cloud_code = m.get('CloudCode')
         if m.get('LogCodes') is not None:
             self.log_codes = m.get('LogCodes')
         if m.get('ProdCode') is not None:
             self.prod_code = m.get('ProdCode')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListAccountsByLogResponseBodyData(TeaModel):
     def __init__(
         self,
         account_id: str = None,
@@ -16786,38 +17392,50 @@
         return self
 
 
 class ListAllProdsRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListAllProdsResponseBodyDataProdList(TeaModel):
     def __init__(
         self,
         cloud_code: str = None,
@@ -17018,14 +17636,16 @@
         action_type: str = None,
         auto_response_type: str = None,
         current_page: int = None,
         id: int = None,
         page_size: int = None,
         playbook_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_name: str = None,
         status: int = None,
         sub_user_id: int = None,
     ):
         # The type of the handling action. Valid values:
         # 
         # *   doPlaybook: runs a playbook.
@@ -17046,14 +17666,16 @@
         # The UUID of the playbook.
         self.playbook_uuid = playbook_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The name of the automated response rule.
         self.rule_name = rule_name
         # The status of the rule. Valid values:
         # 
         # *   0: disabled
         # *   100: enabled
         self.status = status
@@ -17079,14 +17701,18 @@
             result['Id'] = self.id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.playbook_uuid is not None:
             result['PlaybookUuid'] = self.playbook_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.status is not None:
             result['Status'] = self.status
         if self.sub_user_id is not None:
             result['SubUserId'] = self.sub_user_id
         return result
@@ -17103,14 +17729,18 @@
             self.id = m.get('Id')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PlaybookUuid') is not None:
             self.playbook_uuid = m.get('PlaybookUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         return self
@@ -17161,14 +17791,15 @@
 class ListAutomateResponseConfigsResponseBodyDataResponseData(TeaModel):
     def __init__(
         self,
         action_config: str = None,
         action_type: str = None,
         aliuid: int = None,
         auto_response_type: str = None,
+        data_type: int = None,
         execution_condition: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         rule_name: str = None,
         status: int = None,
         sub_user_id: int = None,
@@ -17184,14 +17815,15 @@
         # The ID of the Alibaba Cloud account that is associated with the rule in SIEM.
         self.aliuid = aliuid
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type
+        self.data_type = data_type
         # The trigger condition of the rule. The value is in the JSON format.
         self.execution_condition = execution_condition
         # The creation time.
         self.gmt_create = gmt_create
         # The update time.
         self.gmt_modified = gmt_modified
         # The ID of the automated response rule.
@@ -17219,14 +17851,16 @@
             result['ActionConfig'] = self.action_config
         if self.action_type is not None:
             result['ActionType'] = self.action_type
         if self.aliuid is not None:
             result['Aliuid'] = self.aliuid
         if self.auto_response_type is not None:
             result['AutoResponseType'] = self.auto_response_type
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.execution_condition is not None:
             result['ExecutionCondition'] = self.execution_condition
         if self.gmt_create is not None:
             result['GmtCreate'] = self.gmt_create
         if self.gmt_modified is not None:
             result['GmtModified'] = self.gmt_modified
         if self.id is not None:
@@ -17245,14 +17879,16 @@
             self.action_config = m.get('ActionConfig')
         if m.get('ActionType') is not None:
             self.action_type = m.get('ActionType')
         if m.get('Aliuid') is not None:
             self.aliuid = m.get('Aliuid')
         if m.get('AutoResponseType') is not None:
             self.auto_response_type = m.get('AutoResponseType')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('ExecutionCondition') is not None:
             self.execution_condition = m.get('ExecutionCondition')
         if m.get('GmtCreate') is not None:
             self.gmt_create = m.get('GmtCreate')
         if m.get('GmtModified') is not None:
             self.gmt_modified = m.get('GmtModified')
         if m.get('Id') is not None:
@@ -17851,37 +18487,45 @@
 class ListCloudSiemCustomizeRulesRequest(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
         current_page: int = None,
         end_time: int = None,
         id: str = None,
+        order: str = None,
+        order_field: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_name: str = None,
         rule_type: str = None,
         start_time: int = None,
         status: int = None,
         threat_level: List[str] = None,
     ):
         # The alert type.
         self.alert_type = alert_type
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
         # The ID of the custom rule.
         self.id = id
+        self.order = order
+        self.order_field = order_field
         # The number of entries per page. The value can be up to 100.
         self.page_size = page_size
         # The data management center of the threat analysis feature. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   **cn-hangzhou**: Your assets reside in regions in China.
         # *   **ap-southeast-1**: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The name of the rule. The name can contain letters, digits, underscores (\_), and periods (.).
         self.rule_name = rule_name
         # The type of the rule. Valid values:
         # 
         # *   **predefine**\
         # *   **customize**\
         self.rule_type = rule_type
@@ -17915,18 +18559,26 @@
             result['AlertType'] = self.alert_type
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.id is not None:
             result['Id'] = self.id
+        if self.order is not None:
+            result['Order'] = self.order
+        if self.order_field is not None:
+            result['OrderField'] = self.order_field
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.rule_type is not None:
             result['RuleType'] = self.rule_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.status is not None:
@@ -17941,18 +18593,26 @@
             self.alert_type = m.get('AlertType')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('Id') is not None:
             self.id = m.get('Id')
+        if m.get('Order') is not None:
+            self.order = m.get('Order')
+        if m.get('OrderField') is not None:
+            self.order_field = m.get('OrderField')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('RuleType') is not None:
             self.rule_type = m.get('RuleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('Status') is not None:
@@ -18006,14 +18666,16 @@
 
 class ListCloudSiemCustomizeRulesResponseBodyDataResponseData(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
         alert_type_mds: str = None,
         aliuid: int = None,
+        att_ck: str = None,
+        data_type: int = None,
         event_transfer_ext: str = None,
         event_transfer_switch: int = None,
         event_transfer_type: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         log_source: str = None,
@@ -18032,14 +18694,16 @@
     ):
         # The threat type.
         self.alert_type = alert_type
         # The internal code of the threat type.
         self.alert_type_mds = alert_type_mds
         # The ID of the Alibaba Cloud account in SIEM.
         self.aliuid = aliuid
+        self.att_ck = att_ck
+        self.data_type = data_type
         # The extended information about event generation. If the value of **eventTransferType** is **allToSingle**, the value of this parameter indicates the length and unit of the alert aggregation window. The HTML escape characters are reversed.
         self.event_transfer_ext = event_transfer_ext
         # Indicates whether the system generates an event for the alert. Valid values:
         # 
         # *   **0**: no.
         # *   **1**: yes.
         self.event_transfer_switch = event_transfer_switch
@@ -18106,14 +18770,18 @@
         result = dict()
         if self.alert_type is not None:
             result['AlertType'] = self.alert_type
         if self.alert_type_mds is not None:
             result['AlertTypeMds'] = self.alert_type_mds
         if self.aliuid is not None:
             result['Aliuid'] = self.aliuid
+        if self.att_ck is not None:
+            result['AttCk'] = self.att_ck
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.event_transfer_ext is not None:
             result['EventTransferExt'] = self.event_transfer_ext
         if self.event_transfer_switch is not None:
             result['EventTransferSwitch'] = self.event_transfer_switch
         if self.event_transfer_type is not None:
             result['EventTransferType'] = self.event_transfer_type
         if self.gmt_create is not None:
@@ -18154,14 +18822,18 @@
         m = m or dict()
         if m.get('AlertType') is not None:
             self.alert_type = m.get('AlertType')
         if m.get('AlertTypeMds') is not None:
             self.alert_type_mds = m.get('AlertTypeMds')
         if m.get('Aliuid') is not None:
             self.aliuid = m.get('Aliuid')
+        if m.get('AttCk') is not None:
+            self.att_ck = m.get('AttCk')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('EventTransferExt') is not None:
             self.event_transfer_ext = m.get('EventTransferExt')
         if m.get('EventTransferSwitch') is not None:
             self.event_transfer_switch = m.get('EventTransferSwitch')
         if m.get('EventTransferType') is not None:
             self.event_transfer_type = m.get('EventTransferType')
         if m.get('GmtCreate') is not None:
@@ -18347,40 +19019,54 @@
         return self
 
 
 class ListCloudSiemPredefinedRulesRequest(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
+        att_ck: str = None,
         current_page: int = None,
         end_time: int = None,
+        event_transfer_type: str = None,
         id: str = None,
+        log_source: str = None,
+        order: str = None,
+        order_field: str = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_name: str = None,
         rule_type: str = None,
         start_time: int = None,
         status: int = None,
         threat_level: List[str] = None,
     ):
         # The alert type.
         self.alert_type = alert_type
+        self.att_ck = att_ck
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time
+        self.event_transfer_type = event_transfer_type
         # The ID of the rule.
         self.id = id
+        self.log_source = log_source
+        self.order = order
+        self.order_field = order_field
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The name of the rule. The name can contain letters, digits, underscores (\_), and periods (.).
         self.rule_name = rule_name
         # The type of the rule. Valid values:
         # 
         # *   predefine
         # *   customize
         self.rule_type = rule_type
@@ -18408,24 +19094,38 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.alert_type is not None:
             result['AlertType'] = self.alert_type
+        if self.att_ck is not None:
+            result['AttCk'] = self.att_ck
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.end_time is not None:
             result['EndTime'] = self.end_time
+        if self.event_transfer_type is not None:
+            result['EventTransferType'] = self.event_transfer_type
         if self.id is not None:
             result['Id'] = self.id
+        if self.log_source is not None:
+            result['LogSource'] = self.log_source
+        if self.order is not None:
+            result['Order'] = self.order
+        if self.order_field is not None:
+            result['OrderField'] = self.order_field
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.rule_type is not None:
             result['RuleType'] = self.rule_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.status is not None:
@@ -18434,24 +19134,38 @@
             result['ThreatLevel'] = self.threat_level
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlertType') is not None:
             self.alert_type = m.get('AlertType')
+        if m.get('AttCk') is not None:
+            self.att_ck = m.get('AttCk')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
+        if m.get('EventTransferType') is not None:
+            self.event_transfer_type = m.get('EventTransferType')
         if m.get('Id') is not None:
             self.id = m.get('Id')
+        if m.get('LogSource') is not None:
+            self.log_source = m.get('LogSource')
+        if m.get('Order') is not None:
+            self.order = m.get('Order')
+        if m.get('OrderField') is not None:
+            self.order_field = m.get('OrderField')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('RuleType') is not None:
             self.rule_type = m.get('RuleType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('Status') is not None:
@@ -18503,36 +19217,44 @@
         return self
 
 
 class ListCloudSiemPredefinedRulesResponseBodyDataResponseData(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
+        att_ck: str = None,
+        event_transfer_type: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         rule_desc_mds: str = None,
         rule_name: str = None,
+        rule_name_cn: str = None,
+        rule_name_en: str = None,
         rule_name_mds: str = None,
         source: str = None,
         status: int = None,
         threat_level: str = None,
     ):
         # The type of the risk.
         self.alert_type = alert_type
+        self.att_ck = att_ck
+        self.event_transfer_type = event_transfer_type
         # The time when the rule was created.
         self.gmt_create = gmt_create
         # The time when the rule was modified.
         self.gmt_modified = gmt_modified
         # The ID of the predefined rule.
         self.id = id
         # The internal code of the rule description.
         self.rule_desc_mds = rule_desc_mds
         # The name of the rule.
         self.rule_name = rule_name
+        self.rule_name_cn = rule_name_cn
+        self.rule_name_en = rule_name_en
         # The internal code of the rule name.
         self.rule_name_mds = rule_name_mds
         # The log source of the rule.
         self.source = source
         # The status of the predefined rule. Valid values:
         # 
         # *   0: The rule is in the initial state.
@@ -18552,48 +19274,64 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.alert_type is not None:
             result['AlertType'] = self.alert_type
+        if self.att_ck is not None:
+            result['AttCk'] = self.att_ck
+        if self.event_transfer_type is not None:
+            result['EventTransferType'] = self.event_transfer_type
         if self.gmt_create is not None:
             result['GmtCreate'] = self.gmt_create
         if self.gmt_modified is not None:
             result['GmtModified'] = self.gmt_modified
         if self.id is not None:
             result['Id'] = self.id
         if self.rule_desc_mds is not None:
             result['RuleDescMds'] = self.rule_desc_mds
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
+        if self.rule_name_cn is not None:
+            result['RuleNameCn'] = self.rule_name_cn
+        if self.rule_name_en is not None:
+            result['RuleNameEn'] = self.rule_name_en
         if self.rule_name_mds is not None:
             result['RuleNameMds'] = self.rule_name_mds
         if self.source is not None:
             result['Source'] = self.source
         if self.status is not None:
             result['Status'] = self.status
         if self.threat_level is not None:
             result['ThreatLevel'] = self.threat_level
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlertType') is not None:
             self.alert_type = m.get('AlertType')
+        if m.get('AttCk') is not None:
+            self.att_ck = m.get('AttCk')
+        if m.get('EventTransferType') is not None:
+            self.event_transfer_type = m.get('EventTransferType')
         if m.get('GmtCreate') is not None:
             self.gmt_create = m.get('GmtCreate')
         if m.get('GmtModified') is not None:
             self.gmt_modified = m.get('GmtModified')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RuleDescMds') is not None:
             self.rule_desc_mds = m.get('RuleDescMds')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
+        if m.get('RuleNameCn') is not None:
+            self.rule_name_cn = m.get('RuleNameCn')
+        if m.get('RuleNameEn') is not None:
+            self.rule_name_en = m.get('RuleNameEn')
         if m.get('RuleNameMds') is not None:
             self.rule_name_mds = m.get('RuleNameMds')
         if m.get('Source') is not None:
             self.source = m.get('Source')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('ThreatLevel') is not None:
@@ -18752,26 +19490,30 @@
 class ListCustomizeRuleTestResultRequest(TeaModel):
     def __init__(
         self,
         current_page: int = None,
         id: int = None,
         page_size: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The ID of the rule.
         self.id = id
         # The number of entries per page. Valid values: 1 to 100.
         self.page_size = page_size
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -18782,26 +19524,34 @@
             result['CurrentPage'] = self.current_page
         if self.id is not None:
             result['Id'] = self.id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListCustomizeRuleTestResultResponseBodyDataPageInfo(TeaModel):
     def __init__(
         self,
         current_page: int = None,
@@ -19608,38 +20358,50 @@
         return self
 
 
 class ListDeliveryRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListDeliveryResponseBodyDataProductListLogListExtraParameters(TeaModel):
     def __init__(
         self,
         key: str = None,
@@ -20025,14 +20787,16 @@
         order: str = None,
         order_field: str = None,
         page_size: int = None,
         playbook_name: str = None,
         playbook_types: str = None,
         playbook_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         sophon_task_id: str = None,
         start_time: int = None,
     ):
         # The page number. Pages start from page 1.
         self.current_page = current_page
         # The status of the policy. Valid values:
         # 
@@ -20075,14 +20839,16 @@
         # The UUID of the playbook.
         self.playbook_uuid = playbook_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The ID of the SOAR handling policy.
         self.sophon_task_id = sophon_task_id
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
     def validate(self):
         pass
@@ -20113,14 +20879,18 @@
             result['PlaybookName'] = self.playbook_name
         if self.playbook_types is not None:
             result['PlaybookTypes'] = self.playbook_types
         if self.playbook_uuid is not None:
             result['PlaybookUuid'] = self.playbook_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.sophon_task_id is not None:
             result['SophonTaskId'] = self.sophon_task_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
@@ -20145,14 +20915,18 @@
             self.playbook_name = m.get('PlaybookName')
         if m.get('PlaybookTypes') is not None:
             self.playbook_types = m.get('PlaybookTypes')
         if m.get('PlaybookUuid') is not None:
             self.playbook_uuid = m.get('PlaybookUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SophonTaskId') is not None:
             self.sophon_task_id = m.get('SophonTaskId')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
@@ -20534,28 +21308,32 @@
 
 class ListImportedLogsByProdRequest(TeaModel):
     def __init__(
         self,
         cloud_code: str = None,
         prod_code: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The code of the cloud service provider. Valid values:
         # 
         # *   qcloud: Tencent Cloud
         # *   aliyun: Alibaba Cloud
         # *   hcloud: Huawei Cloud
         self.cloud_code = cloud_code
         # The code of the cloud service.
         self.prod_code = prod_code
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -20564,36 +21342,45 @@
         result = dict()
         if self.cloud_code is not None:
             result['CloudCode'] = self.cloud_code
         if self.prod_code is not None:
             result['ProdCode'] = self.prod_code
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CloudCode') is not None:
             self.cloud_code = m.get('CloudCode')
         if m.get('ProdCode') is not None:
             self.prod_code = m.get('ProdCode')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListImportedLogsByProdResponseBodyData(TeaModel):
     def __init__(
         self,
         auto_imported: int = None,
         cloud_code: str = None,
         imported: int = None,
         imported_user_count: int = None,
         log_code: str = None,
         log_mds_code: str = None,
+        log_type: int = None,
         modify_time: str = None,
         prod_code: str = None,
         total_user_count: int = None,
         un_imported_user_count: int = None,
     ):
         # Indicates whether the log is automatically added to the threat analysis feature within newly added accounts. Valid values:
         # 
@@ -20613,14 +21400,15 @@
         self.imported = imported
         # The number of users who have added the log.
         self.imported_user_count = imported_user_count
         # The log code.
         self.log_code = log_code
         # The display log code.
         self.log_mds_code = log_mds_code
+        self.log_type = log_type
         # The time when the log was last added.
         self.modify_time = modify_time
         # The code of the cloud service to which the log belongs.
         self.prod_code = prod_code
         # The total number of users who have the log.
         self.total_user_count = total_user_count
         # The number of users who have not added the log.
@@ -20643,14 +21431,16 @@
             result['Imported'] = self.imported
         if self.imported_user_count is not None:
             result['ImportedUserCount'] = self.imported_user_count
         if self.log_code is not None:
             result['LogCode'] = self.log_code
         if self.log_mds_code is not None:
             result['LogMdsCode'] = self.log_mds_code
+        if self.log_type is not None:
+            result['LogType'] = self.log_type
         if self.modify_time is not None:
             result['ModifyTime'] = self.modify_time
         if self.prod_code is not None:
             result['ProdCode'] = self.prod_code
         if self.total_user_count is not None:
             result['TotalUserCount'] = self.total_user_count
         if self.un_imported_user_count is not None:
@@ -20667,14 +21457,16 @@
             self.imported = m.get('Imported')
         if m.get('ImportedUserCount') is not None:
             self.imported_user_count = m.get('ImportedUserCount')
         if m.get('LogCode') is not None:
             self.log_code = m.get('LogCode')
         if m.get('LogMdsCode') is not None:
             self.log_mds_code = m.get('LogMdsCode')
+        if m.get('LogType') is not None:
+            self.log_type = m.get('LogType')
         if m.get('ModifyTime') is not None:
             self.modify_time = m.get('ModifyTime')
         if m.get('ProdCode') is not None:
             self.prod_code = m.get('ProdCode')
         if m.get('TotalUserCount') is not None:
             self.total_user_count = m.get('TotalUserCount')
         if m.get('UnImportedUserCount') is not None:
@@ -22542,14 +23334,16 @@
 
 class OpenDeliveryRequest(TeaModel):
     def __init__(
         self,
         log_code: str = None,
         product_code: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The log code of the cloud service, such as the code of the process log for Security Center. If you leave this parameter empty, operations are performed on all logs of the cloud service.
         self.log_code = log_code
         # The code of the cloud service. Valid values:
         # 
         # *   qcloud_waf
         # *   qlcoud_cfw
@@ -22576,14 +23370,16 @@
         # *   polardb
         self.product_code = product_code
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -22592,24 +23388,32 @@
         result = dict()
         if self.log_code is not None:
             result['LogCode'] = self.log_code
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('LogCode') is not None:
             self.log_code = m.get('LogCode')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class OpenDeliveryResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
@@ -22693,14 +23497,16 @@
         self,
         action_config: str = None,
         action_type: str = None,
         auto_response_type: str = None,
         execution_condition: str = None,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_name: str = None,
         sub_user_id: int = None,
     ):
         # The action configuration of the automated response rule. The value is in the JSON format.
         self.action_config = action_config
         # The type of the handling action. Multiple types are separated by commas (,). Valid values:
         # 
@@ -22718,14 +23524,16 @@
         # The rule ID.
         self.id = id
         # The data management center of the threat analysis feature. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   **cn-hangzhou**: Your assets reside in regions in China.
         # *   **ap-southeast-1**: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The rule name.
         self.rule_name = rule_name
         # The ID of the user who created the rule.
         self.sub_user_id = sub_user_id
 
     def validate(self):
         pass
@@ -22744,14 +23552,18 @@
             result['AutoResponseType'] = self.auto_response_type
         if self.execution_condition is not None:
             result['ExecutionCondition'] = self.execution_condition
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.sub_user_id is not None:
             result['SubUserId'] = self.sub_user_id
         return result
 
     def from_map(self, m: dict = None):
@@ -22764,14 +23576,18 @@
             self.auto_response_type = m.get('AutoResponseType')
         if m.get('ExecutionCondition') is not None:
             self.execution_condition = m.get('ExecutionCondition')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         return self
 
 
@@ -22876,35 +23692,39 @@
 
 
 class PostCustomizeRuleRequest(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
         alert_type_mds: str = None,
+        att_ck: str = None,
         event_transfer_ext: str = None,
         event_transfer_switch: int = None,
         event_transfer_type: str = None,
         id: int = None,
         log_source: str = None,
         log_source_mds: str = None,
         log_type: str = None,
         log_type_mds: str = None,
         query_cycle: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_condition: str = None,
         rule_desc: str = None,
         rule_group: str = None,
         rule_name: str = None,
         rule_threshold: str = None,
         threat_level: str = None,
     ):
         # The risk type.
         self.alert_type = alert_type
         # The internal code of the risk type.
         self.alert_type_mds = alert_type_mds
+        self.att_ck = att_ck
         # The extended information about event generation. If eventTransferType is set to allToSingle, the value of this parameter indicates the length and unit of the alert aggregation window.
         self.event_transfer_ext = event_transfer_ext
         # Specifies whether to convert an alert to an event. Valid values:
         # 
         # *   0: no
         # *   1: yes
         self.event_transfer_switch = event_transfer_switch
@@ -22927,14 +23747,16 @@
         # The window length of the rule.
         self.query_cycle = query_cycle
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The query condition of the rule. The value is in the JSON format.
         self.rule_condition = rule_condition
         # The description of the rule.
         self.rule_desc = rule_desc
         # The log aggregation field of the rule. The value is a JSON string.
         self.rule_group = rule_group
         # The name of the rule.
@@ -22957,14 +23779,16 @@
             return _map
 
         result = dict()
         if self.alert_type is not None:
             result['AlertType'] = self.alert_type
         if self.alert_type_mds is not None:
             result['AlertTypeMds'] = self.alert_type_mds
+        if self.att_ck is not None:
+            result['AttCk'] = self.att_ck
         if self.event_transfer_ext is not None:
             result['EventTransferExt'] = self.event_transfer_ext
         if self.event_transfer_switch is not None:
             result['EventTransferSwitch'] = self.event_transfer_switch
         if self.event_transfer_type is not None:
             result['EventTransferType'] = self.event_transfer_type
         if self.id is not None:
@@ -22977,14 +23801,18 @@
             result['LogType'] = self.log_type
         if self.log_type_mds is not None:
             result['LogTypeMds'] = self.log_type_mds
         if self.query_cycle is not None:
             result['QueryCycle'] = self.query_cycle
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_condition is not None:
             result['RuleCondition'] = self.rule_condition
         if self.rule_desc is not None:
             result['RuleDesc'] = self.rule_desc
         if self.rule_group is not None:
             result['RuleGroup'] = self.rule_group
         if self.rule_name is not None:
@@ -22997,14 +23825,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlertType') is not None:
             self.alert_type = m.get('AlertType')
         if m.get('AlertTypeMds') is not None:
             self.alert_type_mds = m.get('AlertTypeMds')
+        if m.get('AttCk') is not None:
+            self.att_ck = m.get('AttCk')
         if m.get('EventTransferExt') is not None:
             self.event_transfer_ext = m.get('EventTransferExt')
         if m.get('EventTransferSwitch') is not None:
             self.event_transfer_switch = m.get('EventTransferSwitch')
         if m.get('EventTransferType') is not None:
             self.event_transfer_type = m.get('EventTransferType')
         if m.get('Id') is not None:
@@ -23017,14 +23847,18 @@
             self.log_type = m.get('LogType')
         if m.get('LogTypeMds') is not None:
             self.log_type_mds = m.get('LogTypeMds')
         if m.get('QueryCycle') is not None:
             self.query_cycle = m.get('QueryCycle')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleCondition') is not None:
             self.rule_condition = m.get('RuleCondition')
         if m.get('RuleDesc') is not None:
             self.rule_desc = m.get('RuleDesc')
         if m.get('RuleGroup') is not None:
             self.rule_group = m.get('RuleGroup')
         if m.get('RuleName') is not None:
@@ -23038,14 +23872,16 @@
 
 class PostCustomizeRuleResponseBodyData(TeaModel):
     def __init__(
         self,
         alert_type: str = None,
         alert_type_mds: str = None,
         aliuid: int = None,
+        att_ck: str = None,
+        data_type: int = None,
         event_transfer_ext: str = None,
         event_transfer_switch: int = None,
         event_transfer_type: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         log_source: str = None,
@@ -23064,14 +23900,16 @@
     ):
         # The risk type.
         self.alert_type = alert_type
         # The internal code of the risk type.
         self.alert_type_mds = alert_type_mds
         # The ID of the Alibaba Cloud account that is used to purchase the threat analysis feature.
         self.aliuid = aliuid
+        self.att_ck = att_ck
+        self.data_type = data_type
         # The extended information about event generation. If eventTransferType is set to allToSingle, the value of this parameter indicates the length and unit of the alert aggregation window. The HTML escape characters are reversed.
         self.event_transfer_ext = event_transfer_ext
         # Indicates whether the system generates an event for the alert. Valid values:
         # 
         # *   0: no
         # *   1: yes
         self.event_transfer_switch = event_transfer_switch
@@ -23138,14 +23976,18 @@
         result = dict()
         if self.alert_type is not None:
             result['AlertType'] = self.alert_type
         if self.alert_type_mds is not None:
             result['AlertTypeMds'] = self.alert_type_mds
         if self.aliuid is not None:
             result['Aliuid'] = self.aliuid
+        if self.att_ck is not None:
+            result['AttCk'] = self.att_ck
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.event_transfer_ext is not None:
             result['EventTransferExt'] = self.event_transfer_ext
         if self.event_transfer_switch is not None:
             result['EventTransferSwitch'] = self.event_transfer_switch
         if self.event_transfer_type is not None:
             result['EventTransferType'] = self.event_transfer_type
         if self.gmt_create is not None:
@@ -23186,14 +24028,18 @@
         m = m or dict()
         if m.get('AlertType') is not None:
             self.alert_type = m.get('AlertType')
         if m.get('AlertTypeMds') is not None:
             self.alert_type_mds = m.get('AlertTypeMds')
         if m.get('Aliuid') is not None:
             self.aliuid = m.get('Aliuid')
+        if m.get('AttCk') is not None:
+            self.att_ck = m.get('AttCk')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('EventTransferExt') is not None:
             self.event_transfer_ext = m.get('EventTransferExt')
         if m.get('EventTransferSwitch') is not None:
             self.event_transfer_switch = m.get('EventTransferSwitch')
         if m.get('EventTransferType') is not None:
             self.event_transfer_type = m.get('EventTransferType')
         if m.get('GmtCreate') is not None:
@@ -23334,24 +24180,28 @@
 
 
 class PostCustomizeRuleTestRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         simulated_data: str = None,
         test_type: str = None,
     ):
         # The ID of the rule.
         self.id = id
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The simulation data for the test. This parameter is available only when TestType is set to simulate.
         self.simulated_data = simulated_data
         # The test type. Valid values:
         # 
         # *   simulate: simulation data test
         # *   business: business data test
         self.test_type = test_type
@@ -23365,26 +24215,34 @@
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.simulated_data is not None:
             result['SimulatedData'] = self.simulated_data
         if self.test_type is not None:
             result['TestType'] = self.test_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SimulatedData') is not None:
             self.simulated_data = m.get('SimulatedData')
         if m.get('TestType') is not None:
             self.test_type = m.get('TestType')
         return self
 
 
@@ -23492,14 +24350,16 @@
     def __init__(
         self,
         event_dispose: str = None,
         incident_uuid: str = None,
         receiver_info: str = None,
         region_id: str = None,
         remark: str = None,
+        role_for: int = None,
+        role_type: int = None,
         status: int = None,
     ):
         # The configuration of event handling. The value is a JSON object.
         self.event_dispose = event_dispose
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The configuration of the alert recipient. The value is a JSON object.
@@ -23507,14 +24367,16 @@
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
         # The remarks of the event.
         self.remark = remark
+        self.role_for = role_for
+        self.role_type = role_type
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handing
         # *   5: handling failed
         # *   10: handled
         self.status = status
@@ -23534,14 +24396,18 @@
             result['IncidentUuid'] = self.incident_uuid
         if self.receiver_info is not None:
             result['ReceiverInfo'] = self.receiver_info
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.remark is not None:
             result['Remark'] = self.remark
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EventDispose') is not None:
@@ -23550,14 +24416,18 @@
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('ReceiverInfo') is not None:
             self.receiver_info = m.get('ReceiverInfo')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class PostEventDisposeAndWhiteruleListResponseBody(TeaModel):
     def __init__(
@@ -23660,23 +24530,27 @@
 
 
 class PostEventWhiteruleListRequest(TeaModel):
     def __init__(
         self,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         whiterule_list: str = None,
     ):
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The alert whitelist rule. The value is a JSON object.
         self.whiterule_list = whiterule_list
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -23685,24 +24559,32 @@
             return _map
 
         result = dict()
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.whiterule_list is not None:
             result['WhiteruleList'] = self.whiterule_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('WhiteruleList') is not None:
             self.whiterule_list = m.get('WhiteruleList')
         return self
 
 
 class PostEventWhiteruleListResponseBody(TeaModel):
     def __init__(
@@ -23805,44 +24687,56 @@
 
 
 class PostFinishCustomizeRuleTestRequest(TeaModel):
     def __init__(
         self,
         id: int = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The ID of the rule.
         self.id = id
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class PostFinishCustomizeRuleTestResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -23944,28 +24838,32 @@
 
 class PostRuleStatusChangeRequest(TeaModel):
     def __init__(
         self,
         ids: str = None,
         in_use: bool = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         rule_type: str = None,
     ):
         # The rule IDs. The value is a JSON array.
         self.ids = ids
         # Specifies whether to enable the rule. Valid values:
         # 
         # *   true
         # *   false
         self.in_use = in_use
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The type of the rule. Valid values:
         # 
         # *   predefine
         # *   customize
         self.rule_type = rule_type
 
     def validate(self):
@@ -23979,26 +24877,34 @@
         result = dict()
         if self.ids is not None:
             result['Ids'] = self.ids
         if self.in_use is not None:
             result['InUse'] = self.in_use
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.rule_type is not None:
             result['RuleType'] = self.rule_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Ids') is not None:
             self.ids = m.get('Ids')
         if m.get('InUse') is not None:
             self.in_use = m.get('InUse')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('RuleType') is not None:
             self.rule_type = m.get('RuleType')
         return self
 
 
 class PostRuleStatusChangeResponseBody(TeaModel):
     def __init__(
@@ -24100,38 +25006,50 @@
         return self
 
 
 class RestoreCapacityRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class RestoreCapacityResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
@@ -24335,27 +25253,31 @@
 
 
 class SetStorageRequest(TeaModel):
     def __init__(
         self,
         region: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         ttl: int = None,
     ):
         # The storage region of logs.
         # 
         # If the data management center is **cn-hangzhou**, the default value of **Region** is cn-shanghai, which specifies the China (Shanghai) region. If the data management center is **ap-southeast-1**, the default value of **Region** is ap-southeast-1, which specifies the Singapore region.
         # 
         # The region for log storage cannot be changed. To change the region, contact the technical support of threat analysis.
         self.region = region
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The storage duration of logs. Default value: 180. Minimum value: 30. Maximum value: 3000. Unit: days.
         self.ttl = ttl
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -24364,24 +25286,32 @@
             return _map
 
         result = dict()
         if self.region is not None:
             result['Region'] = self.region
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.ttl is not None:
             result['Ttl'] = self.ttl
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Region') is not None:
             self.region = m.get('Region')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('Ttl') is not None:
             self.ttl = m.get('Ttl')
         return self
 
 
 class SetStorageResponseBody(TeaModel):
     def __init__(
@@ -24913,27 +25843,31 @@
 
 class UpdateAutomateResponseConfigStatusRequest(TeaModel):
     def __init__(
         self,
         ids: str = None,
         in_use: bool = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
     ):
         # The IDs of the automatic response rules. The value is a JSON array.
         self.ids = ids
         # Specifies whether the rule is enabled. Valid values:
         # 
         # *   true
         # *   false
         self.in_use = in_use
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -24942,24 +25876,32 @@
         result = dict()
         if self.ids is not None:
             result['Ids'] = self.ids
         if self.in_use is not None:
             result['InUse'] = self.in_use
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Ids') is not None:
             self.ids = m.get('Ids')
         if m.get('InUse') is not None:
             self.in_use = m.get('InUse')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class UpdateAutomateResponseConfigStatusResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -25061,25 +26003,29 @@
 
 class UpdateWhiteRuleListRequest(TeaModel):
     def __init__(
         self,
         expression: str = None,
         incident_uuid: str = None,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         white_rule_id: int = None,
     ):
         # The alert whitelist rule. The value is a JSON object.
         self.expression = expression
         # The UUID of the event.
         self.incident_uuid = incident_uuid
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The unique ID of the whitelist rule.
         self.white_rule_id = white_rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -25090,26 +26036,34 @@
         result = dict()
         if self.expression is not None:
             result['Expression'] = self.expression
         if self.incident_uuid is not None:
             result['IncidentUuid'] = self.incident_uuid
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.white_rule_id is not None:
             result['WhiteRuleId'] = self.white_rule_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Expression') is not None:
             self.expression = m.get('Expression')
         if m.get('IncidentUuid') is not None:
             self.incident_uuid = m.get('IncidentUuid')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('WhiteRuleId') is not None:
             self.white_rule_id = m.get('WhiteRuleId')
         return self
 
 
 class UpdateWhiteRuleListResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO` & `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloud-siem20220616
-Version: 3.0.4
+Version: 3.0.5
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.4/setup.py` & `alibabacloud_cloud-siem20220616-3.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloud-siem20220616.
 
-Created on 27/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloud_siem20220616"
 NAME = "alibabacloud_cloud-siem20220616" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloud-siem (20220616) SDK Library for Python"
```

