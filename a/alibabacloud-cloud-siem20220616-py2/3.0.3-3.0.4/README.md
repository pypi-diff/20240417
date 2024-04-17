# Comparing `tmp/alibabacloud_cloud-siem20220616_py2-3.0.3.tar.gz` & `tmp/alibabacloud_cloud-siem20220616_py2-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloud-siem20220616_py2-3.0.3.tar", last modified: Wed Mar 27 07:07:41 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloud-siem20220616_py2-3.0.4.tar", last modified: Wed Apr 17 17:12:44 2024, max compression
```

## Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3.tar` & `alibabacloud_cloud-siem20220616_py2-3.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/
--rw-r--r--   0 root         (0) root         (0)      554 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142898 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   854745 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2024-03-27 07:07:41.000000 alibabacloud_cloud-siem20220616_py2-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/
+-rw-r--r--   0 root         (0) root         (0)      699 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   156866 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   893445 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/setup.py
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/ChangeLog.md` & `alibabacloud_cloud-siem20220616_py2-3.0.4/ChangeLog.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-27 Version: 3.0.3
+- Update API BatchJobCheck: update response param.
+- Update API DescribeCloudSiemEventDetail: update response param.
+
+
 2024-02-22 Version: 3.0.2
 - Update API DescribeCloudSiemEventDetail: update response param.
 
 
 2024-01-18 Version: 3.0.1
 - Generated python2 2022-06-16 for cloud-siem.
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/LICENSE` & `alibabacloud_cloud-siem20220616_py2-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/PKG-INFO` & `alibabacloud_cloud-siem20220616_py2-3.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloud-siem20220616_py2
-Version: 3.0.3
+Version: 3.0.4
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/README-CN.md` & `alibabacloud_cloud-siem20220616_py2-3.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/README.md` & `alibabacloud_cloud-siem20220616_py2-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/client.py` & `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -279,14 +279,18 @@
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
@@ -309,14 +313,18 @@
     def delete_automate_response_config_with_options(self, request, runtime):
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
@@ -373,14 +381,18 @@
         return self.delete_bind_account_with_options(request, runtime)
 
     def delete_customize_rule_with_options(self, request, runtime):
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
@@ -535,14 +547,18 @@
     def delete_white_rule_list_with_options(self, request, runtime):
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
@@ -563,14 +579,18 @@
         return self.delete_white_rule_list_with_options(request, runtime)
 
     def describe_aggregate_function_with_options(self, request, runtime):
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
@@ -591,14 +611,18 @@
         return self.describe_aggregate_function_with_options(request, runtime)
 
     def describe_alert_scene_with_options(self, request, runtime):
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
@@ -621,14 +645,18 @@
     def describe_alert_scene_by_event_with_options(self, request, runtime):
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
@@ -653,14 +681,18 @@
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
@@ -685,14 +717,18 @@
     def describe_alert_source_with_event_with_options(self, request, runtime):
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
@@ -713,14 +749,20 @@
         return self.describe_alert_source_with_event_with_options(request, runtime)
 
     def describe_alert_type_with_options(self, request, runtime):
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
@@ -755,14 +797,18 @@
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
@@ -791,14 +837,18 @@
     def describe_alerts_count_with_options(self, request, runtime):
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
@@ -829,14 +879,18 @@
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
@@ -871,14 +925,18 @@
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
@@ -909,14 +967,18 @@
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
@@ -967,14 +1029,18 @@
         return self.describe_auth_with_options(request, runtime)
 
     def describe_automate_response_config_counter_with_options(self, request, runtime):
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
@@ -997,14 +1063,18 @@
     def describe_automate_response_config_feature_with_options(self, request, runtime):
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
@@ -1029,14 +1099,18 @@
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
@@ -1065,14 +1139,18 @@
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
@@ -1095,14 +1173,18 @@
     def describe_cloud_siem_assets_counter_with_options(self, request, runtime):
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
@@ -1125,14 +1207,18 @@
     def describe_cloud_siem_event_detail_with_options(self, request, runtime):
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
@@ -1169,14 +1255,18 @@
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
@@ -1265,14 +1355,18 @@
         return self.describe_customize_rule_with_options(request, runtime)
 
     def describe_customize_rule_count_with_options(self, request, runtime):
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
@@ -1295,14 +1389,18 @@
     def describe_customize_rule_test_with_options(self, request, runtime):
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
@@ -1325,14 +1423,18 @@
     def describe_customize_rule_test_histogram_with_options(self, request, runtime):
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
@@ -1427,14 +1529,18 @@
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
@@ -1457,14 +1563,18 @@
     def describe_dispose_strategy_playbook_with_options(self, request, runtime):
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
@@ -1493,14 +1603,18 @@
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
@@ -1521,16 +1635,24 @@
     def describe_entity_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_entity_info_with_options(request, runtime)
 
     def describe_event_count_by_threat_level_with_options(self, request, runtime):
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
@@ -1557,14 +1679,18 @@
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
@@ -1647,14 +1773,18 @@
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
@@ -1677,14 +1807,18 @@
     def describe_log_source_with_options(self, request, runtime):
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
@@ -1733,14 +1867,18 @@
         return self.describe_log_store_with_options(request, runtime)
 
     def describe_log_type_with_options(self, request, runtime):
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
@@ -1761,14 +1899,18 @@
         return self.describe_log_type_with_options(request, runtime)
 
     def describe_operators_with_options(self, request, runtime):
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
@@ -1819,14 +1961,18 @@
         return self.describe_prod_count_with_options(request, runtime)
 
     def describe_scope_users_with_options(self, request, runtime):
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
@@ -1875,14 +2021,18 @@
         return self.describe_service_status_with_options(request, runtime)
 
     def describe_storage_with_options(self, request, runtime):
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
@@ -1935,14 +2085,18 @@
     def describe_waf_scope_with_options(self, request, runtime):
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
@@ -1973,14 +2127,18 @@
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
@@ -2071,16 +2229,22 @@
     def do_self_delegate(self, request):
         runtime = util_models.RuntimeOptions()
         return self.do_self_delegate_with_options(request, runtime)
 
     def enable_access_for_cloud_siem_with_options(self, request, runtime):
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
@@ -2129,14 +2293,18 @@
         return self.enable_service_for_cloud_siem_with_options(request, runtime)
 
     def get_capacity_with_options(self, request, runtime):
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
@@ -2263,14 +2431,18 @@
         return self.get_quick_query_with_options(request, runtime)
 
     def get_storage_with_options(self, request, runtime):
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
@@ -2327,14 +2499,18 @@
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
@@ -2355,14 +2531,18 @@
         return self.list_accounts_by_log_with_options(request, runtime)
 
     def list_all_prods_with_options(self, request, runtime):
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
@@ -2395,14 +2575,18 @@
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
@@ -2497,18 +2681,26 @@
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
@@ -2539,24 +2731,38 @@
         return self.list_cloud_siem_customize_rules_with_options(request, runtime)
 
     def list_cloud_siem_predefined_rules_with_options(self, request, runtime):
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
@@ -2593,14 +2799,18 @@
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
@@ -2685,14 +2895,18 @@
         return self.list_data_source_types_with_options(request, runtime)
 
     def list_delivery_with_options(self, request, runtime):
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
@@ -2735,14 +2949,18 @@
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
@@ -2771,14 +2989,18 @@
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
@@ -3109,14 +3331,18 @@
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
@@ -3147,14 +3373,18 @@
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
@@ -3181,14 +3411,16 @@
     def post_customize_rule_with_options(self, request, runtime):
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
@@ -3201,14 +3433,18 @@
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
@@ -3243,14 +3479,18 @@
     def post_customize_rule_test_with_options(self, request, runtime):
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
@@ -3283,14 +3523,18 @@
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
@@ -3315,14 +3559,18 @@
     def post_event_whiterule_list_with_options(self, request, runtime):
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
@@ -3347,14 +3595,18 @@
     def post_finish_customize_rule_test_with_options(self, request, runtime):
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
@@ -3379,14 +3631,18 @@
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
@@ -3409,14 +3665,18 @@
         return self.post_rule_status_change_with_options(request, runtime)
 
     def restore_capacity_with_options(self, request, runtime):
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
@@ -3471,14 +3731,18 @@
     def set_storage_with_options(self, request, runtime):
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
@@ -3601,14 +3865,18 @@
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
@@ -3633,14 +3901,18 @@
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

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616/models.py` & `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1554,15 +1554,15 @@
         if m.get('body') is not None:
             temp_model = BindAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CloseDeliveryRequest(TeaModel):
-    def __init__(self, log_code=None, product_code=None, region_id=None):
+    def __init__(self, log_code=None, product_code=None, region_id=None, role_for=None, role_type=None):
         # The log code of the cloud service, such as the code of the process log for Security Center. You can obtain the log code from the response of the ListDelivery operation.
         self.log_code = log_code  # type: str
         # The code of the cloud service. Valid values:
         # 
         # *   qcloud_waf
         # *   qlcoud_cfw
         # *   hcloud_waf
@@ -1588,14 +1588,16 @@
         # *   polardb
         self.product_code = product_code  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CloseDeliveryRequest, self).to_map()
         if _map is not None:
@@ -1604,24 +1606,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, data=None, request_id=None):
         # Indicates whether the threat analysis feature was disabled. Valid values:
         # 
@@ -1688,44 +1698,54 @@
         if m.get('body') is not None:
             temp_model = CloseDeliveryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteAutomateResponseConfigRequest(TeaModel):
-    def __init__(self, id=None, region_id=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None):
         # The ID of the rule.
         self.id = id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAutomateResponseConfigRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
         # The HTTP status code.
         self.code = code  # type: int
@@ -1960,39 +1980,49 @@
         if m.get('body') is not None:
             temp_model = DeleteBindAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteCustomizeRuleRequest(TeaModel):
-    def __init__(self, region_id=None, rule_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None, rule_id=None):
         # The region in which the service is deployed.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The ID of the rule.
         self.rule_id = rule_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteCustomizeRuleRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
@@ -2588,44 +2618,54 @@
         if m.get('body') is not None:
             temp_model = DeleteUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteWhiteRuleListRequest(TeaModel):
-    def __init__(self, id=None, region_id=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None):
         # The unique ID of the whitelist rule.
         self.id = id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteWhiteRuleListRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
         # The HTTP status code.
         self.code = code  # type: int
@@ -2710,38 +2750,48 @@
         if m.get('body') is not None:
             temp_model = DeleteWhiteRuleListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAggregateFunctionRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAggregateFunctionRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAggregateFunctionResponseBodyData(TeaModel):
     def __init__(self, function=None, function_name=None):
         # The aggregate function.
         self.function = function  # type: str
@@ -2865,38 +2915,48 @@
         if m.get('body') is not None:
             temp_model = DescribeAggregateFunctionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertSceneRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAlertSceneRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAlertSceneResponseBodyDataTargets(TeaModel):
     def __init__(self, name=None, type=None, value=None, values=None):
         # The display name of the attribute for the entity.
         self.name = name  # type: str
@@ -3102,44 +3162,54 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertSceneResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertSceneByEventRequest(TeaModel):
-    def __init__(self, incident_uuid=None, region_id=None):
+    def __init__(self, incident_uuid=None, region_id=None, role_for=None, role_type=None):
         # The ID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAlertSceneByEventRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, name=None, type=None, value=None, values=None):
         # The display name of the entity attribute field that can be added to the whitelist.
         self.name = name  # type: str
@@ -3345,28 +3415,30 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertSceneByEventResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertSourceRequest(TeaModel):
-    def __init__(self, end_time=None, level=None, region_id=None, start_time=None):
+    def __init__(self, end_time=None, level=None, region_id=None, role_for=None, role_type=None, start_time=None):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The risk levels. The value is a JSON array. Valid values:
         # 
         # *   serious: high
         # *   suspicious: medium
         # *   remind: low
         self.level = level  # type: list[str]
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3377,26 +3449,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, source=None, source_name=None):
@@ -3522,44 +3602,54 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertSourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertSourceWithEventRequest(TeaModel):
-    def __init__(self, incident_uuid=None, region_id=None):
+    def __init__(self, incident_uuid=None, region_id=None, role_for=None, role_type=None):
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAlertSourceWithEventRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, source=None, source_name=None):
         # The internal code of the alert data source.
         self.source = source  # type: str
@@ -3683,38 +3773,53 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertSourceWithEventResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertTypeRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None, rule_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
+        self.rule_type = rule_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAlertTypeRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, alert_type=None, alert_type_mds=None):
         # The type of the risk.
         self.alert_type = alert_type  # type: str
@@ -3839,15 +3944,16 @@
             temp_model = DescribeAlertTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertsRequest(TeaModel):
     def __init__(self, alert_title=None, alert_uuid=None, current_page=None, end_time=None, is_defend=None,
-                 level=None, page_size=None, region_id=None, source=None, start_time=None, sub_user_id=None):
+                 level=None, page_size=None, region_id=None, role_for=None, role_type=None, source=None, start_time=None,
+                 sub_user_id=None):
         # The title of the alert.
         self.alert_title = alert_title  # type: str
         # The UUID of the alert.
         self.alert_uuid = alert_uuid  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The end of the time range to query. Unit: milliseconds.
@@ -3866,14 +3972,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The source of the alert.
         self.source = source  # type: str
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
         # The ID of the Alibaba Cloud account within which the alert is generated.
         self.sub_user_id = sub_user_id  # type: str
 
@@ -3898,14 +4006,18 @@
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
@@ -3924,14 +4036,18 @@
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
@@ -4375,22 +4491,24 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertsCountRequest(TeaModel):
-    def __init__(self, end_time=None, region_id=None, start_time=None):
+    def __init__(self, end_time=None, region_id=None, role_for=None, role_type=None, start_time=None):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4399,24 +4517,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, all=None, high=None, low=None, medium=None, product_num=None):
@@ -4555,28 +4681,30 @@
             temp_model = DescribeAlertsCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertsWithEntityRequest(TeaModel):
     def __init__(self, current_page=None, entity_id=None, incident_uuid=None, page_size=None, region_id=None,
-                 sophon_task_id=None):
+                 role_for=None, role_type=None, sophon_task_id=None):
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The ID of the entity.
         self.entity_id = entity_id  # type: long
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The ID of the SOAR handing policy.
         self.sophon_task_id = sophon_task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4591,14 +4719,18 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CurrentPage') is not None:
@@ -4607,14 +4739,18 @@
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
     def __init__(self, current_page=None, page_size=None, total_count=None):
@@ -5055,15 +5191,15 @@
             temp_model = DescribeAlertsWithEntityResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertsWithEventRequest(TeaModel):
     def __init__(self, alert_title=None, current_page=None, incident_uuid=None, is_defend=None, level=None,
-                 page_size=None, region_id=None, source=None, sub_user_id=None):
+                 page_size=None, region_id=None, role_for=None, role_type=None, source=None, sub_user_id=None):
         # The title of the alert.
         self.alert_title = alert_title  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The ID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # Specifies whether an attack is defended. Valid values:
@@ -5080,14 +5216,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The data source of the alert.
         self.source = source  # type: str
         # The ID of the account within which the alert is generated.
         self.sub_user_id = sub_user_id  # type: long
 
     def validate(self):
         pass
@@ -5108,14 +5246,18 @@
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
 
     def from_map(self, m=None):
@@ -5130,14 +5272,18 @@
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
 
 
@@ -5216,16 +5362,17 @@
 
 
 class DescribeAlertsWithEventResponseBodyDataResponseData(TeaModel):
     def __init__(self, alert_desc=None, alert_desc_code=None, alert_desc_en=None, alert_detail=None,
                  alert_info_list=None, alert_level=None, alert_name=None, alert_name_code=None, alert_name_en=None,
                  alert_src_prod=None, alert_src_prod_module=None, alert_title=None, alert_title_en=None, alert_type=None,
                  alert_type_code=None, alert_type_en=None, alert_uuid=None, asset_list=None, att_ck=None, cloud_code=None,
-                 end_time=None, gmt_create=None, gmt_modified=None, id=None, incident_uuid=None, is_defend=None,
-                 log_time=None, log_uuid=None, main_user_id=None, occur_time=None, start_time=None, sub_user_id=None):
+                 end_time=None, entity_list=None, gmt_create=None, gmt_modified=None, id=None, incident_uuid=None,
+                 is_defend=None, log_time=None, log_uuid=None, main_user_id=None, occur_time=None, start_time=None,
+                 sub_user_id=None):
         # The description of the alert.
         self.alert_desc = alert_desc  # type: str
         # The internal code of the alert description.
         self.alert_desc_code = alert_desc_code  # type: str
         # The alert description in English.
         self.alert_desc_en = alert_desc_en  # type: str
         # The details of the alert.
@@ -5268,14 +5415,15 @@
         # 
         # *   aliyun: Alibaba Cloud
         # *   qcloud: Tencent Cloud
         # *   hcloud: Huawei Cloud
         self.cloud_code = cloud_code  # type: str
         # The time when the alert was closed.
         self.end_time = end_time  # type: str
+        self.entity_list = entity_list  # type: str
         # The time when the alert was received.
         self.gmt_create = gmt_create  # type: str
         # The time when the alert was last updated.
         self.gmt_modified = gmt_modified  # type: str
         # The unique ID of the alert.
         self.id = id  # type: long
         # The UUID of the event.
@@ -5350,14 +5498,16 @@
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
@@ -5421,14 +5571,16 @@
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
@@ -5579,26 +5731,29 @@
         if m.get('body') is not None:
             temp_model = DescribeAlertsWithEventResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAttackTimeLineRequest(TeaModel):
-    def __init__(self, asset_name=None, end_time=None, incident_uuid=None, region_id=None, start_time=None):
+    def __init__(self, asset_name=None, end_time=None, incident_uuid=None, region_id=None, role_for=None,
+                 role_type=None, start_time=None):
         # The name of the asset.
         self.asset_name = asset_name  # type: str
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The ID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5611,28 +5766,36 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, alert_level=None, alert_name=None, alert_name_code=None, alert_name_en=None,
@@ -5975,38 +6138,48 @@
         if m.get('body') is not None:
             temp_model = DescribeAuthResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAutomateResponseConfigCounterRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAutomateResponseConfigCounterRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeAutomateResponseConfigCounterResponseBodyData(TeaModel):
     def __init__(self, all=None, online=None):
         # The total number of rules.
         self.all = all  # type: long
@@ -6124,47 +6297,57 @@
         if m.get('body') is not None:
             temp_model = DescribeAutomateResponseConfigCounterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAutomateResponseConfigFeatureRequest(TeaModel):
-    def __init__(self, auto_response_type=None, region_id=None):
+    def __init__(self, auto_response_type=None, region_id=None, role_for=None, role_type=None):
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAutomateResponseConfigFeatureRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, value=None, value_mds=None):
         # The enumerated value of the right operand.
         self.value = value  # type: str
@@ -6419,15 +6602,15 @@
         if m.get('body') is not None:
             temp_model = DescribeAutomateResponseConfigFeatureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAutomateResponseConfigPlayBooksRequest(TeaModel):
-    def __init__(self, auto_response_type=None, entity_type=None, region_id=None):
+    def __init__(self, auto_response_type=None, entity_type=None, region_id=None, role_for=None, role_type=None):
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type  # type: str
         # The entity type of the playbook. Valid values:
         # 
@@ -6436,14 +6619,16 @@
         # *   file
         self.entity_type = entity_type  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAutomateResponseConfigPlayBooksRequest, self).to_map()
         if _map is not None:
@@ -6452,24 +6637,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, description=None, display_name=None, name=None, param_type=None, uuid=None):
         # The description of the playbook.
         self.description = description  # type: str
@@ -6615,15 +6808,16 @@
         if m.get('body') is not None:
             temp_model = DescribeAutomateResponseConfigPlayBooksResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCloudSiemAssetsRequest(TeaModel):
-    def __init__(self, asset_type=None, current_page=None, incident_uuid=None, page_size=None, region_id=None):
+    def __init__(self, asset_type=None, current_page=None, incident_uuid=None, page_size=None, region_id=None,
+                 role_for=None, role_type=None):
         # The type of the asset. Valid values:
         # 
         # *   ip
         # *   domain
         # *   url
         # *   process
         # *   file
@@ -6636,14 +6830,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCloudSiemAssetsRequest, self).to_map()
         if _map is not None:
@@ -6656,28 +6852,36 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, current_page=None, page_size=None, total_count=None):
         # The current page number.
         self.current_page = current_page  # type: int
@@ -6992,44 +7196,54 @@
         if m.get('body') is not None:
             temp_model = DescribeCloudSiemAssetsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCloudSiemAssetsCounterRequest(TeaModel):
-    def __init__(self, incident_uuid=None, region_id=None):
+    def __init__(self, incident_uuid=None, region_id=None, role_for=None, role_type=None):
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCloudSiemAssetsCounterRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, asset_num=None, asset_type=None):
         # The number of assets.
         self.asset_num = asset_num  # type: int
@@ -7160,44 +7374,54 @@
         if m.get('body') is not None:
             temp_model = DescribeCloudSiemAssetsCounterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCloudSiemEventDetailRequest(TeaModel):
-    def __init__(self, incident_uuid=None, region_id=None):
+    def __init__(self, incident_uuid=None, region_id=None, role_for=None, role_type=None):
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCloudSiemEventDetailRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, alert_num=None, aliuid=None, asset_num=None, att_ck_labels=None, data_sources=None,
                  description=None, description_en=None, ext_content=None, gmt_create=None, gmt_modified=None,
                  incident_name=None, incident_name_en=None, incident_uuid=None, refer_account=None, remark=None, status=None,
@@ -7423,16 +7647,16 @@
             temp_model = DescribeCloudSiemEventDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCloudSiemEventsRequest(TeaModel):
     def __init__(self, asset_id=None, current_page=None, end_time=None, event_name=None, incident_uuid=None,
-                 order=None, order_field=None, page_size=None, region_id=None, start_time=None, status=None,
-                 thread_level=None):
+                 order=None, order_field=None, page_size=None, region_id=None, role_for=None, role_type=None,
+                 start_time=None, status=None, thread_level=None):
         # The ID of the asset that is associated with the event.
         self.asset_id = asset_id  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The name of the event.
@@ -7452,14 +7676,16 @@
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handling
         # *   5: handling failed
@@ -7495,14 +7721,18 @@
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
@@ -7523,14 +7753,18 @@
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
@@ -7572,16 +7806,16 @@
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeCloudSiemEventsResponseBodyDataResponseData(TeaModel):
     def __init__(self, alert_num=None, aliuid=None, asset_num=None, att_ck_labels=None, data_sources=None,
                  description=None, description_en=None, ext_content=None, gmt_create=None, gmt_modified=None,
-                 incident_name=None, incident_name_en=None, incident_uuid=None, remark=None, status=None, threat_level=None,
-                 threat_score=None):
+                 incident_name=None, incident_name_en=None, incident_uuid=None, refer_account=None, remark=None, status=None,
+                 threat_level=None, threat_score=None):
         # The number of alerts that are associated with the event.
         self.alert_num = alert_num  # type: int
         # The ID of the Alibaba Cloud account to which the event belongs.
         self.aliuid = aliuid  # type: long
         # The number of assets that are associated with the event.
         self.asset_num = asset_num  # type: int
         # The tags of the ATT\&CK attack.
@@ -7600,14 +7834,15 @@
         self.gmt_modified = gmt_modified  # type: str
         # The name of the event.
         self.incident_name = incident_name  # type: str
         # The event name in English.
         self.incident_name_en = incident_name_en  # type: str
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
+        self.refer_account = refer_account  # type: str
         # The remarks of the event.
         self.remark = remark  # type: str
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handling
         # *   5: handling failed
@@ -7653,14 +7888,16 @@
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
@@ -7691,14 +7928,16 @@
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
@@ -8243,81 +8482,133 @@
         if m.get('body') is not None:
             temp_model = DescribeCustomizeRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCustomizeRuleCountRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCustomizeRuleCountRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeCustomizeRuleCountResponseBodyData(TeaModel):
-    def __init__(self, high_rule_num=None, in_use_rule_num=None, low_rule_num=None, medium_rule_num=None):
+    def __init__(self, aggregation_rule_num=None, customize_rule_num=None, expert_rule_num=None,
+                 graph_computing_rule_num=None, high_rule_num=None, in_use_rule_num=None, low_rule_num=None, medium_rule_num=None,
+                 predefined_rule_num=None, single_alert_rule_num=None, total_rule_num=None, un_event_rule_num=None):
+        self.aggregation_rule_num = aggregation_rule_num  # type: int
+        self.customize_rule_num = customize_rule_num  # type: int
+        self.expert_rule_num = expert_rule_num  # type: int
+        self.graph_computing_rule_num = graph_computing_rule_num  # type: int
         # The number of rules that are used to identify high-risk threats.
         self.high_rule_num = high_rule_num  # type: int
         # The total number of rules.
         self.in_use_rule_num = in_use_rule_num  # type: int
         # The number of rules that are used to identify low-risk threats.
         self.low_rule_num = low_rule_num  # type: int
         # The number of rules that are used to identify medium-risk threats.
         self.medium_rule_num = medium_rule_num  # type: int
+        self.predefined_rule_num = predefined_rule_num  # type: int
+        self.single_alert_rule_num = single_alert_rule_num  # type: int
+        self.total_rule_num = total_rule_num  # type: int
+        self.un_event_rule_num = un_event_rule_num  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCustomizeRuleCountResponseBodyData, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
         # The HTTP status code that is returned.
         self.code = code  # type: int
@@ -8404,44 +8695,54 @@
         if m.get('body') is not None:
             temp_model = DescribeCustomizeRuleCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCustomizeRuleTestRequest(TeaModel):
-    def __init__(self, id=None, region_id=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None):
         # The ID of the rule.
         self.id = id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCustomizeRuleTestRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, id=None, simulate_data=None, status=None):
         # The ID of the rule.
         self.id = id  # type: long
@@ -8571,44 +8872,54 @@
         if m.get('body') is not None:
             temp_model = DescribeCustomizeRuleTestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCustomizeRuleTestHistogramRequest(TeaModel):
-    def __init__(self, id=None, region_id=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None):
         # The ID of the rule.
         self.id = id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCustomizeRuleTestHistogramRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, count=None, from_=None, to=None):
         # The number of alerts that are generated in the query time range.
         self.count = count  # type: long
@@ -9233,15 +9544,16 @@
         if m.get('body') is not None:
             temp_model = DescribeDataSourceParametersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDisposeAndPlaybookRequest(TeaModel):
-    def __init__(self, current_page=None, entity_type=None, incident_uuid=None, page_size=None, region_id=None):
+    def __init__(self, current_page=None, entity_type=None, incident_uuid=None, page_size=None, region_id=None,
+                 role_for=None, role_type=None):
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The entity type. Valid values:
         # 
         # *   ip
         # *   process
         # *   file
@@ -9251,14 +9563,16 @@
         # The number of entries to return on each page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDisposeAndPlaybookRequest, self).to_map()
         if _map is not None:
@@ -9271,28 +9585,36 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, current_page=None, page_size=None, total_count=None):
         # The current page number.
         self.current_page = current_page  # type: int
@@ -9608,22 +9930,24 @@
         if m.get('body') is not None:
             temp_model = DescribeDisposeAndPlaybookResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDisposeStrategyPlaybookRequest(TeaModel):
-    def __init__(self, end_time=None, region_id=None, start_time=None):
+    def __init__(self, end_time=None, region_id=None, role_for=None, role_type=None, start_time=None):
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9632,24 +9956,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, playbook_name=None, playbook_uuid=None):
@@ -9775,27 +10107,29 @@
         if m.get('body') is not None:
             temp_model = DescribeDisposeStrategyPlaybookResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEntityInfoRequest(TeaModel):
-    def __init__(self, entity_id=None, entity_identity=None, incident_uuid=None, region_id=None,
-                 sophon_task_id=None):
+    def __init__(self, entity_id=None, entity_identity=None, incident_uuid=None, region_id=None, role_for=None,
+                 role_type=None, sophon_task_id=None):
         # The logical ID of the entity.
         self.entity_id = entity_id  # type: long
         # The feature value of the entity. Fuzzy match is supported.
         self.entity_identity = entity_identity  # type: str
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The ID of the SOAR handling policy.
         self.sophon_task_id = sophon_task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9808,28 +10142,36 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, entity_id=None, entity_info=None, entity_type=None, tip_info=None):
@@ -9968,38 +10310,58 @@
         if m.get('body') is not None:
             temp_model = DescribeEntityInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEventCountByThreatLevelRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, end_time=None, region_id=None, role_for=None, role_type=None, start_time=None):
+        self.end_time = end_time  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
+        self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEventCountByThreatLevelRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, event_num=None, high_level_event_num=None, low_level_event_num=None,
                  medium_level_event_num=None, undeal_event_num=None):
         # The total number of events.
@@ -10136,26 +10498,29 @@
         if m.get('body') is not None:
             temp_model = DescribeEventCountByThreatLevelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEventDisposeRequest(TeaModel):
-    def __init__(self, current_page=None, incident_uuid=None, page_size=None, region_id=None):
+    def __init__(self, current_page=None, incident_uuid=None, page_size=None, region_id=None, role_for=None,
+                 role_type=None):
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The number of entries to return on each page. Maximum value: 500.
         self.page_size = page_size  # type: int
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEventDisposeRequest, self).to_map()
         if _map is not None:
@@ -10166,26 +10531,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, channel=None, gmt_create=None, gmt_modified=None, id=None, incident_uuid=None,
                  message_title=None, receiver=None, status=None):
         # The channel of the contact information. Valid values:
@@ -10864,24 +11237,26 @@
         if m.get('body') is not None:
             temp_model = DescribeJobStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeLogFieldsRequest(TeaModel):
-    def __init__(self, log_source=None, log_type=None, region_id=None):
+    def __init__(self, log_source=None, log_type=None, region_id=None, role_for=None, role_type=None):
         # The log source of the rule.
         self.log_source = log_source  # type: str
         # The log type of the rule.
         self.log_type = log_type  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeLogFieldsRequest, self).to_map()
         if _map is not None:
@@ -10890,24 +11265,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, activity_name=None, field_desc=None, field_name=None, field_type=None, log_code=None):
         # The type of the log to which the field belongs.
         self.activity_name = activity_name  # type: str
@@ -11052,44 +11435,54 @@
         if m.get('body') is not None:
             temp_model = DescribeLogFieldsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeLogSourceRequest(TeaModel):
-    def __init__(self, log_type=None, region_id=None):
+    def __init__(self, log_type=None, region_id=None, role_for=None, role_type=None):
         # The log type of the rule.
         self.log_type = log_type  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeLogSourceRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, log_source=None, log_source_name=None):
         # The log source of the rule.
         self.log_source = log_source  # type: str
@@ -11381,38 +11774,48 @@
         if m.get('body') is not None:
             temp_model = DescribeLogStoreResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeLogTypeRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeLogTypeRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeLogTypeResponseBodyData(TeaModel):
     def __init__(self, log_type=None, log_type_name=None):
         # The log type of the rule.
         self.log_type = log_type  # type: str
@@ -11536,20 +11939,22 @@
         if m.get('body') is not None:
             temp_model = DescribeLogTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeOperatorsRequest(TeaModel):
-    def __init__(self, region_id=None, scene_type=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None, scene_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The type of the scenario in which the operator is used. Valid values:
         # 
         # *   If you do not specify this parameter, the default scenario is used.
         # *   AGGREGATE: AGGREGATE scenario.
         self.scene_type = scene_type  # type: str
 
     def validate(self):
@@ -11559,22 +11964,30 @@
         _map = super(DescribeOperatorsRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, index=None, operator=None, operator_desc_cn=None, operator_desc_en=None, operator_name=None,
@@ -11865,79 +12278,99 @@
         if m.get('body') is not None:
             temp_model = DescribeProdCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeScopeUsersRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeScopeUsersRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeScopeUsersResponseBodyData(TeaModel):
-    def __init__(self, ali_uid=None, domains=None, instance_id=None, user_name=None):
+    def __init__(self, ali_uid=None, cloud_code=None, domains=None, instance_id=None, user_id=None, user_name=None):
         # The ID of the security information and event management (SIEM) user.
         self.ali_uid = ali_uid  # type: long
+        self.cloud_code = cloud_code  # type: str
         # An array consisting of the domain names that are protected by the WAF instance.
         self.domains = domains  # type: list[str]
         # The ID of the Web Application Firewall (WAF) instance.
         self.instance_id = instance_id  # type: str
+        self.user_id = user_id  # type: str
         # The username.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeScopeUsersResponseBodyData, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
@@ -12130,38 +12563,48 @@
         if m.get('body') is not None:
             temp_model = DescribeServiceStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeStorageRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeStorageRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeStorageResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
         # Indicates whether the projects and Logstores that are created for the threat analysis feature exist in Simple Log Service. Valid values:
         # 
@@ -12263,16 +12706,16 @@
         if m.get('SubUserId') is not None:
             self.sub_user_id = m.get('SubUserId')
         return self
 
 
 class DescribeUserBuyStatusResponseBodyData(TeaModel):
     def __init__(self, can_buy=None, capacity=None, duration_days=None, end_time=None, main_user_id=None,
-                 main_user_name=None, master_user_id=None, master_user_name=None, sas_instance_id=None, sub_user_id=None,
-                 sub_user_name=None):
+                 main_user_name=None, master_user_id=None, master_user_name=None, rd_order=None, sas_instance_id=None,
+                 sub_user_id=None, sub_user_name=None):
         # Indicates whether the logon Alibaba Cloud account can be used to place orders for the threat analysis feature, such as purchase, upgrade, and specifications change orders. Valid values:
         # 
         # *   true
         # *   false
         self.can_buy = can_buy  # type: bool
         # The log storage capacity that is purchased for the threat analysis feature. Unit: GB.
         self.capacity = capacity  # type: int
@@ -12284,14 +12727,15 @@
         self.main_user_id = main_user_id  # type: long
         # The username of the Alibaba Cloud account that is used to purchase the threat analysis feature.
         self.main_user_name = main_user_name  # type: str
         # The ID of the management account of the resource directory.
         self.master_user_id = master_user_id  # type: long
         # The display name of the management account of the resource directory.
         self.master_user_name = master_user_name  # type: str
+        self.rd_order = rd_order  # type: int
         # The instance ID of Security Center.
         self.sas_instance_id = sas_instance_id  # type: str
         # The ID of the logon Alibaba Cloud account.
         self.sub_user_id = sub_user_id  # type: long
         # The username of the logon Alibaba Cloud account.
         self.sub_user_name = sub_user_name  # type: str
 
@@ -12316,14 +12760,16 @@
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
@@ -12342,14 +12788,16 @@
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
@@ -12421,44 +12869,54 @@
         if m.get('body') is not None:
             temp_model = DescribeUserBuyStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeWafScopeRequest(TeaModel):
-    def __init__(self, entity_id=None, region_id=None):
+    def __init__(self, entity_id=None, region_id=None, role_for=None, role_type=None):
         # The ID of the entity.
         self.entity_id = entity_id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeWafScopeRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, aliuid=None, domains=None, instance_id=None):
         # The ID of the Alibaba Cloud account in SIEM.
         self.aliuid = aliuid  # type: long
@@ -12589,15 +13047,15 @@
             temp_model = DescribeWafScopeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeWhiteRuleListRequest(TeaModel):
     def __init__(self, alert_name=None, alert_type=None, current_page=None, incident_uuid=None, page_size=None,
-                 region_id=None):
+                 region_id=None, role_for=None, role_type=None):
         # The name of the alert.
         self.alert_name = alert_name  # type: str
         # The type of the alert.
         self.alert_type = alert_type  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The UUID of the event.
@@ -12605,14 +13063,16 @@
         # The number of entries per page. Valid values: 1 to 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeWhiteRuleListRequest, self).to_map()
         if _map is not None:
@@ -12627,14 +13087,18 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AlertName') is not None:
             self.alert_name = m.get('AlertName')
         if m.get('AlertType') is not None:
@@ -12643,14 +13107,18 @@
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
     def __init__(self, current_page=None, page_size=None, total_count=None):
         # The current page number.
         self.current_page = current_page  # type: int
@@ -13465,38 +13933,53 @@
         if m.get('body') is not None:
             temp_model = DoSelfDelegateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableAccessForCloudSiemRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, auto_submit=None, region_id=None, role_for=None, role_type=None):
+        self.auto_submit = auto_submit  # type: int
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(EnableAccessForCloudSiemRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, data=None, request_id=None):
         # The data returned.
         self.data = data  # type: bool
@@ -13658,38 +14141,48 @@
         if m.get('body') is not None:
             temp_model = EnableServiceForCloudSiemResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetCapacityRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetCapacityRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class GetCapacityResponseBodyData(TeaModel):
     def __init__(self, exist_log_store=None, preserved_capacity=None, used_capacity=None):
         # Indicates whether the Logstores for the threat analysis feature exist on the user side. Valid values:
         # 
@@ -14400,38 +14893,48 @@
         if m.get('body') is not None:
             temp_model = GetQuickQueryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetStorageRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetStorageRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class GetStorageResponseBodyData(TeaModel):
     def __init__(self, can_operate=None, display_region=None, region=None, ttl=None):
         # Indicates whether the storage region can be changed for once. Default value: false Valid values:
         # 
@@ -14748,15 +15251,16 @@
         if m.get('body') is not None:
             temp_model = ListAccountAccessIdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAccountsByLogRequest(TeaModel):
-    def __init__(self, cloud_code=None, log_codes=None, prod_code=None, region_id=None):
+    def __init__(self, cloud_code=None, log_codes=None, prod_code=None, region_id=None, role_for=None,
+                 role_type=None):
         # The code that is used for multi-cloud environments.
         # 
         # Valid values:
         # 
         # *   qcloud
         # *   hcloud
         # *   aliyun
@@ -14766,14 +15270,16 @@
         # The code of the service.
         self.prod_code = prod_code  # type: str
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListAccountsByLogRequest, self).to_map()
         if _map is not None:
@@ -14784,26 +15290,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, account_id=None, account_name=None, imported=None, log_code=None, main_user_id=None,
                  prod_code=None, sub_user_id=None):
         # The ID of the cloud account.
@@ -14937,38 +15451,48 @@
         if m.get('body') is not None:
             temp_model = ListAccountsByLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAllProdsRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListAllProdsRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListAllProdsResponseBodyDataProdList(TeaModel):
     def __init__(self, cloud_code=None, imported_log_count=None, modify_time=None, prod_code=None,
                  total_log_count=None):
         # The code of the cloud service provider. Valid values:
@@ -15140,15 +15664,15 @@
             temp_model = ListAllProdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAutomateResponseConfigsRequest(TeaModel):
     def __init__(self, action_type=None, auto_response_type=None, current_page=None, id=None, page_size=None,
-                 playbook_uuid=None, region_id=None, rule_name=None, status=None, sub_user_id=None):
+                 playbook_uuid=None, region_id=None, role_for=None, role_type=None, rule_name=None, status=None, sub_user_id=None):
         # The type of the handling action. Valid values:
         # 
         # *   doPlaybook: runs a playbook.
         # *   changeEventStatus: changes the status of an event.
         # *   changeThreatLevel: changes the risk level of an event.
         self.action_type = action_type  # type: str
         # The type of the automated response rule. Valid values:
@@ -15165,14 +15689,16 @@
         # The UUID of the playbook.
         self.playbook_uuid = playbook_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The name of the automated response rule.
         self.rule_name = rule_name  # type: str
         # The status of the rule. Valid values:
         # 
         # *   0: disabled
         # *   100: enabled
         self.status = status  # type: int
@@ -15198,14 +15724,18 @@
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
@@ -15222,14 +15752,18 @@
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
@@ -15269,15 +15803,15 @@
             self.page_size = m.get('PageSize')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class ListAutomateResponseConfigsResponseBodyDataResponseData(TeaModel):
-    def __init__(self, action_config=None, action_type=None, aliuid=None, auto_response_type=None,
+    def __init__(self, action_config=None, action_type=None, aliuid=None, auto_response_type=None, data_type=None,
                  execution_condition=None, gmt_create=None, gmt_modified=None, id=None, rule_name=None, status=None, sub_user_id=None):
         # The configuration of the action that is performed after the rule is hit. The value is in JSON format.
         self.action_config = action_config  # type: str
         # The type of the handling action. Multiple types are separated by commas (,). Valid values:
         # 
         # *   doPlaybook: runs a playbook.
         # *   changeEventStatus: changes the status of an event.
@@ -15286,14 +15820,15 @@
         # The ID of the Alibaba Cloud account that is associated with the rule in SIEM.
         self.aliuid = aliuid  # type: long
         # The type of the automated response rule. Valid values:
         # 
         # *   event
         # *   alert
         self.auto_response_type = auto_response_type  # type: str
+        self.data_type = data_type  # type: int
         # The trigger condition of the rule. The value is in the JSON format.
         self.execution_condition = execution_condition  # type: str
         # The creation time.
         self.gmt_create = gmt_create  # type: str
         # The update time.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the automated response rule.
@@ -15321,14 +15856,16 @@
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
@@ -15347,14 +15884,16 @@
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
@@ -15885,31 +16424,36 @@
         if m.get('body') is not None:
             temp_model = ListBindDataSourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListCloudSiemCustomizeRulesRequest(TeaModel):
-    def __init__(self, alert_type=None, current_page=None, end_time=None, id=None, page_size=None, region_id=None,
-                 rule_name=None, rule_type=None, start_time=None, status=None, threat_level=None):
+    def __init__(self, alert_type=None, current_page=None, end_time=None, id=None, order=None, order_field=None,
+                 page_size=None, region_id=None, role_for=None, role_type=None, rule_name=None, rule_type=None,
+                 start_time=None, status=None, threat_level=None):
         # The alert type.
         self.alert_type = alert_type  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
         # The ID of the custom rule.
         self.id = id  # type: str
+        self.order = order  # type: str
+        self.order_field = order_field  # type: str
         # The number of entries per page. The value can be up to 100.
         self.page_size = page_size  # type: int
         # The data management center of the threat analysis feature. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   **cn-hangzhou**: Your assets reside in regions in China.
         # *   **ap-southeast-1**: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The name of the rule. The name can contain letters, digits, underscores (\_), and periods (.).
         self.rule_name = rule_name  # type: str
         # The type of the rule. Valid values:
         # 
         # *   **predefine**\
         # *   **customize**\
         self.rule_type = rule_type  # type: str
@@ -15943,18 +16487,26 @@
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
@@ -15969,18 +16521,26 @@
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
@@ -16024,24 +16584,27 @@
             self.page_size = m.get('PageSize')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class ListCloudSiemCustomizeRulesResponseBodyDataResponseData(TeaModel):
-    def __init__(self, alert_type=None, alert_type_mds=None, aliuid=None, event_transfer_ext=None,
-                 event_transfer_switch=None, event_transfer_type=None, gmt_create=None, gmt_modified=None, id=None, log_source=None,
-                 log_source_mds=None, log_type=None, log_type_mds=None, query_cycle=None, rule_condition=None, rule_desc=None,
-                 rule_group=None, rule_name=None, rule_threshold=None, rule_type=None, status=None, threat_level=None):
+    def __init__(self, alert_type=None, alert_type_mds=None, aliuid=None, att_ck=None, data_type=None,
+                 event_transfer_ext=None, event_transfer_switch=None, event_transfer_type=None, gmt_create=None, gmt_modified=None,
+                 id=None, log_source=None, log_source_mds=None, log_type=None, log_type_mds=None, query_cycle=None,
+                 rule_condition=None, rule_desc=None, rule_group=None, rule_name=None, rule_threshold=None, rule_type=None,
+                 status=None, threat_level=None):
         # The threat type.
         self.alert_type = alert_type  # type: str
         # The internal code of the threat type.
         self.alert_type_mds = alert_type_mds  # type: str
         # The ID of the Alibaba Cloud account in SIEM.
         self.aliuid = aliuid  # type: long
+        self.att_ck = att_ck  # type: str
+        self.data_type = data_type  # type: int
         # The extended information about event generation. If the value of **eventTransferType** is **allToSingle**, the value of this parameter indicates the length and unit of the alert aggregation window. The HTML escape characters are reversed.
         self.event_transfer_ext = event_transfer_ext  # type: str
         # Indicates whether the system generates an event for the alert. Valid values:
         # 
         # *   **0**: no.
         # *   **1**: yes.
         self.event_transfer_switch = event_transfer_switch  # type: int
@@ -16108,14 +16671,18 @@
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
@@ -16156,14 +16723,18 @@
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
@@ -16330,31 +16901,39 @@
         if m.get('body') is not None:
             temp_model = ListCloudSiemCustomizeRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListCloudSiemPredefinedRulesRequest(TeaModel):
-    def __init__(self, alert_type=None, current_page=None, end_time=None, id=None, page_size=None, region_id=None,
-                 rule_name=None, rule_type=None, start_time=None, status=None, threat_level=None):
+    def __init__(self, alert_type=None, att_ck=None, current_page=None, end_time=None, event_transfer_type=None,
+                 id=None, log_source=None, order=None, order_field=None, page_size=None, region_id=None, role_for=None,
+                 role_type=None, rule_name=None, rule_type=None, start_time=None, status=None, threat_level=None):
         # The alert type.
         self.alert_type = alert_type  # type: str
+        self.att_ck = att_ck  # type: str
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The end of the time range to query. Unit: milliseconds.
         self.end_time = end_time  # type: long
+        self.event_transfer_type = event_transfer_type  # type: str
         # The ID of the rule.
         self.id = id  # type: str
+        self.log_source = log_source  # type: str
+        self.order = order  # type: str
+        self.order_field = order_field  # type: str
         # The number of entries per page. Maximum value: 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The name of the rule. The name can contain letters, digits, underscores (\_), and periods (.).
         self.rule_name = rule_name  # type: str
         # The type of the rule. Valid values:
         # 
         # *   predefine
         # *   customize
         self.rule_type = rule_type  # type: str
@@ -16382,24 +16961,38 @@
         _map = super(ListCloudSiemPredefinedRulesRequest, self).to_map()
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
@@ -16408,24 +17001,38 @@
             result['ThreatLevel'] = self.threat_level
         return result
 
     def from_map(self, m=None):
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
@@ -16469,28 +17076,33 @@
             self.page_size = m.get('PageSize')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class ListCloudSiemPredefinedRulesResponseBodyDataResponseData(TeaModel):
-    def __init__(self, alert_type=None, gmt_create=None, gmt_modified=None, id=None, rule_desc_mds=None,
-                 rule_name=None, rule_name_mds=None, source=None, status=None, threat_level=None):
+    def __init__(self, alert_type=None, att_ck=None, event_transfer_type=None, gmt_create=None, gmt_modified=None,
+                 id=None, rule_desc_mds=None, rule_name=None, rule_name_cn=None, rule_name_en=None, rule_name_mds=None,
+                 source=None, status=None, threat_level=None):
         # The type of the risk.
         self.alert_type = alert_type  # type: str
+        self.att_ck = att_ck  # type: str
+        self.event_transfer_type = event_transfer_type  # type: str
         # The time when the rule was created.
         self.gmt_create = gmt_create  # type: str
         # The time when the rule was modified.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the predefined rule.
         self.id = id  # type: long
         # The internal code of the rule description.
         self.rule_desc_mds = rule_desc_mds  # type: str
         # The name of the rule.
         self.rule_name = rule_name  # type: str
+        self.rule_name_cn = rule_name_cn  # type: str
+        self.rule_name_en = rule_name_en  # type: str
         # The internal code of the rule name.
         self.rule_name_mds = rule_name_mds  # type: str
         # The log source of the rule.
         self.source = source  # type: str
         # The status of the predefined rule. Valid values:
         # 
         # *   0: The rule is in the initial state.
@@ -16510,48 +17122,64 @@
         _map = super(ListCloudSiemPredefinedRulesResponseBodyDataResponseData, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -16688,26 +17316,28 @@
         if m.get('body') is not None:
             temp_model = ListCloudSiemPredefinedRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListCustomizeRuleTestResultRequest(TeaModel):
-    def __init__(self, current_page=None, id=None, page_size=None, region_id=None):
+    def __init__(self, current_page=None, id=None, page_size=None, region_id=None, role_for=None, role_type=None):
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The ID of the rule.
         self.id = id  # type: long
         # The number of entries per page. Valid values: 1 to 100.
         self.page_size = page_size  # type: int
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListCustomizeRuleTestResultRequest, self).to_map()
         if _map is not None:
@@ -16718,26 +17348,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, current_page=None, page_size=None, total_count=None):
         # The current page number.
         self.current_page = current_page  # type: int
@@ -17454,38 +18092,48 @@
         if m.get('body') is not None:
             temp_model = ListDataSourceTypesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListDeliveryRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListDeliveryRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class ListDeliveryResponseBodyDataProductListLogListExtraParameters(TeaModel):
     def __init__(self, key=None, value=None):
         # The ID of the extended parameter.
         self.key = key  # type: str
@@ -17824,15 +18472,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListDisposeStrategyRequest(TeaModel):
     def __init__(self, current_page=None, effective_status=None, end_time=None, entity_identity=None,
                  entity_type=None, order=None, order_field=None, page_size=None, playbook_name=None, playbook_types=None,
-                 playbook_uuid=None, region_id=None, sophon_task_id=None, start_time=None):
+                 playbook_uuid=None, region_id=None, role_for=None, role_type=None, sophon_task_id=None, start_time=None):
         # The page number. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The status of the policy. Valid values:
         # 
         # *   0: invalid
         # *   1: valid
         self.effective_status = effective_status  # type: int
@@ -17872,14 +18520,16 @@
         # The UUID of the playbook.
         self.playbook_uuid = playbook_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The ID of the SOAR handling policy.
         self.sophon_task_id = sophon_task_id  # type: str
         # The beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
@@ -17910,14 +18560,18 @@
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
 
     def from_map(self, m=None):
@@ -17942,14 +18596,18 @@
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
 
 
@@ -18285,28 +18943,30 @@
         if m.get('body') is not None:
             temp_model = ListDisposeStrategyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListImportedLogsByProdRequest(TeaModel):
-    def __init__(self, cloud_code=None, prod_code=None, region_id=None):
+    def __init__(self, cloud_code=None, prod_code=None, region_id=None, role_for=None, role_type=None):
         # The code of the cloud service provider. Valid values:
         # 
         # *   qcloud: Tencent Cloud
         # *   aliyun: Alibaba Cloud
         # *   hcloud: Huawei Cloud
         self.cloud_code = cloud_code  # type: str
         # The code of the cloud service.
         self.prod_code = prod_code  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListImportedLogsByProdRequest, self).to_map()
         if _map is not None:
@@ -18315,30 +18975,39 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, auto_imported=None, cloud_code=None, imported=None, imported_user_count=None, log_code=None,
-                 log_mds_code=None, modify_time=None, prod_code=None, total_user_count=None, un_imported_user_count=None):
+                 log_mds_code=None, log_type=None, modify_time=None, prod_code=None, total_user_count=None,
+                 un_imported_user_count=None):
         # Indicates whether the log is automatically added to the threat analysis feature within newly added accounts. Valid values:
         # 
         # *   1: yes
         # *   0: no
         self.auto_imported = auto_imported  # type: int
         # The code of the cloud service provider. Valid values:
         # 
@@ -18353,14 +19022,15 @@
         self.imported = imported  # type: int
         # The number of users who have added the log.
         self.imported_user_count = imported_user_count  # type: int
         # The log code.
         self.log_code = log_code  # type: str
         # The display log code.
         self.log_mds_code = log_mds_code  # type: str
+        self.log_type = log_type  # type: int
         # The time when the log was last added.
         self.modify_time = modify_time  # type: str
         # The code of the cloud service to which the log belongs.
         self.prod_code = prod_code  # type: str
         # The total number of users who have the log.
         self.total_user_count = total_user_count  # type: int
         # The number of users who have not added the log.
@@ -18383,14 +19053,16 @@
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
@@ -18407,14 +19079,16 @@
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
@@ -20075,15 +20749,15 @@
         if m.get('body') is not None:
             temp_model = ModifyDataSourceLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class OpenDeliveryRequest(TeaModel):
-    def __init__(self, log_code=None, product_code=None, region_id=None):
+    def __init__(self, log_code=None, product_code=None, region_id=None, role_for=None, role_type=None):
         # The log code of the cloud service, such as the code of the process log for Security Center. If you leave this parameter empty, operations are performed on all logs of the cloud service.
         self.log_code = log_code  # type: str
         # The code of the cloud service. Valid values:
         # 
         # *   qcloud_waf
         # *   qlcoud_cfw
         # *   hcloud_waf
@@ -20109,14 +20783,16 @@
         # *   polardb
         self.product_code = product_code  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(OpenDeliveryRequest, self).to_map()
         if _map is not None:
@@ -20125,24 +20801,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, data=None, request_id=None):
         # Indicates whether the log delivery feature is enabled. Valid values:
         # 
@@ -20210,15 +20894,15 @@
             temp_model = OpenDeliveryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostAutomateResponseConfigRequest(TeaModel):
     def __init__(self, action_config=None, action_type=None, auto_response_type=None, execution_condition=None,
-                 id=None, region_id=None, rule_name=None, sub_user_id=None):
+                 id=None, region_id=None, role_for=None, role_type=None, rule_name=None, sub_user_id=None):
         # The action configuration of the automated response rule. The value is in the JSON format.
         self.action_config = action_config  # type: str
         # The type of the handling action. Multiple types are separated by commas (,). Valid values:
         # 
         # *   **doPlaybook**: runs the playbook.
         # *   **changeEventStatus**: changes the event status.
         # *   **changeThreatLevel**: changes the threat level of the event.
@@ -20233,14 +20917,16 @@
         # The rule ID.
         self.id = id  # type: long
         # The data management center of the threat analysis feature. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   **cn-hangzhou**: Your assets reside in regions in China.
         # *   **ap-southeast-1**: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The rule name.
         self.rule_name = rule_name  # type: str
         # The ID of the user who created the rule.
         self.sub_user_id = sub_user_id  # type: long
 
     def validate(self):
         pass
@@ -20259,14 +20945,18 @@
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
 
     def from_map(self, m=None):
@@ -20279,14 +20969,18 @@
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
 
 
@@ -20375,22 +21069,23 @@
         if m.get('body') is not None:
             temp_model = PostAutomateResponseConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostCustomizeRuleRequest(TeaModel):
-    def __init__(self, alert_type=None, alert_type_mds=None, event_transfer_ext=None, event_transfer_switch=None,
-                 event_transfer_type=None, id=None, log_source=None, log_source_mds=None, log_type=None, log_type_mds=None,
-                 query_cycle=None, region_id=None, rule_condition=None, rule_desc=None, rule_group=None, rule_name=None,
-                 rule_threshold=None, threat_level=None):
+    def __init__(self, alert_type=None, alert_type_mds=None, att_ck=None, event_transfer_ext=None,
+                 event_transfer_switch=None, event_transfer_type=None, id=None, log_source=None, log_source_mds=None, log_type=None,
+                 log_type_mds=None, query_cycle=None, region_id=None, role_for=None, role_type=None, rule_condition=None,
+                 rule_desc=None, rule_group=None, rule_name=None, rule_threshold=None, threat_level=None):
         # The risk type.
         self.alert_type = alert_type  # type: str
         # The internal code of the risk type.
         self.alert_type_mds = alert_type_mds  # type: str
+        self.att_ck = att_ck  # type: str
         # The extended information about event generation. If eventTransferType is set to allToSingle, the value of this parameter indicates the length and unit of the alert aggregation window.
         self.event_transfer_ext = event_transfer_ext  # type: str
         # Specifies whether to convert an alert to an event. Valid values:
         # 
         # *   0: no
         # *   1: yes
         self.event_transfer_switch = event_transfer_switch  # type: int
@@ -20413,14 +21108,16 @@
         # The window length of the rule.
         self.query_cycle = query_cycle  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The query condition of the rule. The value is in the JSON format.
         self.rule_condition = rule_condition  # type: str
         # The description of the rule.
         self.rule_desc = rule_desc  # type: str
         # The log aggregation field of the rule. The value is a JSON string.
         self.rule_group = rule_group  # type: str
         # The name of the rule.
@@ -20443,14 +21140,16 @@
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
@@ -20463,14 +21162,18 @@
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
@@ -20483,14 +21186,16 @@
 
     def from_map(self, m=None):
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
@@ -20503,14 +21208,18 @@
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
@@ -20519,24 +21228,27 @@
             self.rule_threshold = m.get('RuleThreshold')
         if m.get('ThreatLevel') is not None:
             self.threat_level = m.get('ThreatLevel')
         return self
 
 
 class PostCustomizeRuleResponseBodyData(TeaModel):
-    def __init__(self, alert_type=None, alert_type_mds=None, aliuid=None, event_transfer_ext=None,
-                 event_transfer_switch=None, event_transfer_type=None, gmt_create=None, gmt_modified=None, id=None, log_source=None,
-                 log_source_mds=None, log_type=None, log_type_mds=None, query_cycle=None, rule_condition=None, rule_desc=None,
-                 rule_group=None, rule_name=None, rule_threshold=None, rule_type=None, status=None, threat_level=None):
+    def __init__(self, alert_type=None, alert_type_mds=None, aliuid=None, att_ck=None, data_type=None,
+                 event_transfer_ext=None, event_transfer_switch=None, event_transfer_type=None, gmt_create=None, gmt_modified=None,
+                 id=None, log_source=None, log_source_mds=None, log_type=None, log_type_mds=None, query_cycle=None,
+                 rule_condition=None, rule_desc=None, rule_group=None, rule_name=None, rule_threshold=None, rule_type=None,
+                 status=None, threat_level=None):
         # The risk type.
         self.alert_type = alert_type  # type: str
         # The internal code of the risk type.
         self.alert_type_mds = alert_type_mds  # type: str
         # The ID of the Alibaba Cloud account that is used to purchase the threat analysis feature.
         self.aliuid = aliuid  # type: long
+        self.att_ck = att_ck  # type: str
+        self.data_type = data_type  # type: int
         # The extended information about event generation. If eventTransferType is set to allToSingle, the value of this parameter indicates the length and unit of the alert aggregation window. The HTML escape characters are reversed.
         self.event_transfer_ext = event_transfer_ext  # type: str
         # Indicates whether the system generates an event for the alert. Valid values:
         # 
         # *   0: no
         # *   1: yes
         self.event_transfer_switch = event_transfer_switch  # type: int
@@ -20603,14 +21315,18 @@
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
@@ -20651,14 +21367,18 @@
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
@@ -20783,22 +21503,24 @@
         if m.get('body') is not None:
             temp_model = PostCustomizeRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostCustomizeRuleTestRequest(TeaModel):
-    def __init__(self, id=None, region_id=None, simulated_data=None, test_type=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None, simulated_data=None, test_type=None):
         # The ID of the rule.
         self.id = id  # type: long
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The simulation data for the test. This parameter is available only when TestType is set to simulate.
         self.simulated_data = simulated_data  # type: str
         # The test type. Valid values:
         # 
         # *   simulate: simulation data test
         # *   business: business data test
         self.test_type = test_type  # type: str
@@ -20812,26 +21534,34 @@
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
 
     def from_map(self, m=None):
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
 
 
@@ -20921,28 +21651,30 @@
             temp_model = PostCustomizeRuleTestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostEventDisposeAndWhiteruleListRequest(TeaModel):
     def __init__(self, event_dispose=None, incident_uuid=None, receiver_info=None, region_id=None, remark=None,
-                 status=None):
+                 role_for=None, role_type=None, status=None):
         # The configuration of event handling. The value is a JSON object.
         self.event_dispose = event_dispose  # type: str
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The configuration of the alert recipient. The value is a JSON object.
         self.receiver_info = receiver_info  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
         # The remarks of the event.
         self.remark = remark  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The status of the event. Valid values:
         # 
         # *   0: unhandled
         # *   1: handing
         # *   5: handling failed
         # *   10: handled
         self.status = status  # type: int
@@ -20962,14 +21694,18 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('EventDispose') is not None:
@@ -20978,14 +21714,18 @@
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
@@ -21072,22 +21812,24 @@
         if m.get('body') is not None:
             temp_model = PostEventDisposeAndWhiteruleListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostEventWhiteruleListRequest(TeaModel):
-    def __init__(self, incident_uuid=None, region_id=None, whiterule_list=None):
+    def __init__(self, incident_uuid=None, region_id=None, role_for=None, role_type=None, whiterule_list=None):
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The alert whitelist rule. The value is a JSON object.
         self.whiterule_list = whiterule_list  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -21096,24 +21838,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
@@ -21200,44 +21950,54 @@
         if m.get('body') is not None:
             temp_model = PostEventWhiteruleListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostFinishCustomizeRuleTestRequest(TeaModel):
-    def __init__(self, id=None, region_id=None):
+    def __init__(self, id=None, region_id=None, role_for=None, role_type=None):
         # The ID of the rule.
         self.id = id  # type: long
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PostFinishCustomizeRuleTestRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
         # The HTTP status code.
         self.code = code  # type: int
@@ -21322,27 +22082,29 @@
         if m.get('body') is not None:
             temp_model = PostFinishCustomizeRuleTestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostRuleStatusChangeRequest(TeaModel):
-    def __init__(self, ids=None, in_use=None, region_id=None, rule_type=None):
+    def __init__(self, ids=None, in_use=None, region_id=None, role_for=None, role_type=None, rule_type=None):
         # The rule IDs. The value is a JSON array.
         self.ids = ids  # type: str
         # Specifies whether to enable the rule. Valid values:
         # 
         # *   true
         # *   false
         self.in_use = in_use  # type: bool
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The type of the rule. Valid values:
         # 
         # *   predefine
         # *   customize
         self.rule_type = rule_type  # type: str
 
     def validate(self):
@@ -21356,26 +22118,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
@@ -21462,38 +22232,48 @@
         if m.get('body') is not None:
             temp_model = PostRuleStatusChangeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RestoreCapacityRequest(TeaModel):
-    def __init__(self, region_id=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None):
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in the Chinese mainland or in the China (Hong Kong) region.
         # *   ap-southeast-1: Your assets reside in regions outside the Chinese mainland, excluding the China (Hong Kong) region.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RestoreCapacityRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         return self
 
 
 class RestoreCapacityResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
         # Indicates whether the release command has been sent. Valid values:
         # 
@@ -21670,26 +22450,28 @@
         if m.get('body') is not None:
             temp_model = SaveQuickQueryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetStorageRequest(TeaModel):
-    def __init__(self, region=None, region_id=None, ttl=None):
+    def __init__(self, region=None, region_id=None, role_for=None, role_type=None, ttl=None):
         # The storage region of logs.
         # 
         # If the data management center is **cn-hangzhou**, the default value of **Region** is cn-shanghai, which specifies the China (Shanghai) region. If the data management center is **ap-southeast-1**, the default value of **Region** is ap-southeast-1, which specifies the Singapore region.
         # 
         # The region for log storage cannot be changed. To change the region, contact the technical support of threat analysis.
         self.region = region  # type: str
         # The data management center of the threat analysis feature. Specify this parameter based on the region where your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The storage duration of logs. Default value: 180. Minimum value: 30. Maximum value: 3000. Unit: days.
         self.ttl = ttl  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -21698,24 +22480,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, data=None, request_id=None):
@@ -22186,27 +22976,29 @@
         if m.get('body') is not None:
             temp_model = SubmitJobsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAutomateResponseConfigStatusRequest(TeaModel):
-    def __init__(self, ids=None, in_use=None, region_id=None):
+    def __init__(self, ids=None, in_use=None, region_id=None, role_for=None, role_type=None):
         # The IDs of the automatic response rules. The value is a JSON array.
         self.ids = ids  # type: str
         # Specifies whether the rule is enabled. Valid values:
         # 
         # *   true
         # *   false
         self.in_use = in_use  # type: bool
         # The data management center of the threat analysis feature. Specify this parameter based on the region in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions inside China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateAutomateResponseConfigStatusRequest, self).to_map()
         if _map is not None:
@@ -22215,24 +23007,32 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
         # The HTTP status code that is returned.
         self.code = code  # type: int
@@ -22317,24 +23117,27 @@
         if m.get('body') is not None:
             temp_model = UpdateAutomateResponseConfigStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateWhiteRuleListRequest(TeaModel):
-    def __init__(self, expression=None, incident_uuid=None, region_id=None, white_rule_id=None):
+    def __init__(self, expression=None, incident_uuid=None, region_id=None, role_for=None, role_type=None,
+                 white_rule_id=None):
         # The alert whitelist rule. The value is a JSON object.
         self.expression = expression  # type: str
         # The UUID of the event.
         self.incident_uuid = incident_uuid  # type: str
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The unique ID of the whitelist rule.
         self.white_rule_id = white_rule_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -22345,26 +23148,34 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO` & `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloud-siem20220616-py2
-Version: 3.0.3
+Version: 3.0.4
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.3/setup.py` & `alibabacloud_cloud-siem20220616_py2-3.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloud-siem20220616_py2.
 
-Created on 27/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloud_siem20220616"
 NAME = "alibabacloud_cloud-siem20220616_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloud-siem (20220616) SDK Library for Python2"
```

