# Comparing `tmp/alibabacloud_emr20210320_py2-1.4.2.tar.gz` & `tmp/alibabacloud_emr20210320_py2-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr20210320_py2-1.4.2.tar", last modified: Tue Mar 26 17:11:04 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr20210320_py2-1.5.0.tar", last modified: Wed Apr 17 17:11:57 2024, max compression
```

## Comparing `alibabacloud_emr20210320_py2-1.4.2.tar` & `alibabacloud_emr20210320_py2-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     2600 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103517 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/client.py
--rw-r--r--   0 root         (0) root         (0)  1659822 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-03-26 17:11:04.000000 alibabacloud_emr20210320_py2-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2667 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109730 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/client.py
+-rw-r--r--   0 root         (0) root         (0)  1678468 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/setup.py
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/ChangeLog.md` & `alibabacloud_emr20210320_py2-1.5.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-26 Version: 1.4.2
+- Generated python2 2021-03-20 for Emr.
+
 2024-03-15 Version: 1.4.1
 - Update API GetAutoScalingPolicy: update response param.
 
 
 2024-03-14 Version: 1.4.0
 - Support API GetApplication.
 - Support API ListComponentInstances.
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/LICENSE` & `alibabacloud_emr20210320_py2-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.4.2/PKG-INFO` & `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_emr20210320_py2
-Version: 1.4.2
+Name: alibabacloud-emr20210320-py2
+Version: 1.5.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/README-CN.md` & `alibabacloud_emr20210320_py2-1.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.4.2/README.md` & `alibabacloud_emr20210320_py2-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/client.py` & `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,66 @@
         @param request: DecreaseNodesRequest
 
         @return: DecreaseNodesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.decrease_nodes_with_options(request, runtime)
 
+    def delete_api_template_with_options(self, request, runtime):
+        """
+        创建集群模板
+        
+
+        @param request: DeleteApiTemplateRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.DeleteApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_api_template(self, request):
+        """
+        创建集群模板
+        
+
+        @param request: DeleteApiTemplateRequest
+
+        @return: DeleteApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.delete_api_template_with_options(request, runtime)
+
     def delete_cluster_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -229,14 +281,44 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_cluster(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_cluster_with_options(request, runtime)
 
+    def get_api_template_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.GetApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_api_template(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_api_template_with_options(request, runtime)
+
     def get_application_with_options(self, request, runtime):
         """
         查询应用详情。
         
 
         @param request: GetApplicationRequest
 
@@ -1291,14 +1373,56 @@
             self.call_api(params, req, runtime)
         )
 
     def join_resource_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.join_resource_group_with_options(request, runtime)
 
+    def list_api_templates_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.template_ids):
+            query['TemplateIds'] = request.template_ids
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListApiTemplates',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.ListApiTemplatesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_api_templates(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_api_templates_with_options(request, runtime)
+
     def list_application_configs_with_options(self, request, runtime):
         """
         查询应用配置。
         
 
         @param request: ListApplicationConfigsRequest
 
@@ -2675,14 +2799,66 @@
             self.call_api(params, req, runtime)
         )
 
     def remove_auto_scaling_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_auto_scaling_policy_with_options(request, runtime)
 
+    def run_api_template_with_options(self, request, runtime):
+        """
+        执行集群模板
+        
+
+        @param request: RunApiTemplateRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RunApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RunApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.RunApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def run_api_template(self, request):
+        """
+        执行集群模板
+        
+
+        @param request: RunApiTemplateRequest
+
+        @return: RunApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.run_api_template_with_options(request, runtime)
+
     def run_application_action_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.action_name):
             query['ActionName'] = request.action_name
         if not UtilClient.is_unset(request.batch_size):
             query['BatchSize'] = request.batch_size
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320/models.py` & `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,14 +310,76 @@
         if m.get('Taints') is not None:
             for k in m.get('Taints'):
                 temp_model = AckNodeSelectorTaints()
                 self.taints.append(temp_model.from_map(k))
         return self
 
 
+class ApiTemplate(TeaModel):
+    def __init__(self, api_name=None, content=None, region_id=None, resource_group_id=None, status=None,
+                 template_id=None, template_name=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 模版接口参数。
+        self.content = content  # type: str
+        # 区域ID。
+        self.region_id = region_id  # type: str
+        # 资源组ID。
+        self.resource_group_id = resource_group_id  # type: str
+        # 模板状态。
+        self.status = status  # type: str
+        # 模板ID。
+        self.template_id = template_id  # type: str
+        # 模板ID。
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ApiTemplate, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
 class Application(TeaModel):
     def __init__(self, application_name=None):
         # 应用名称。从EMR控制台集群创建页面可查看到指定发行版的应用名称列表。
         self.application_name = application_name  # type: str
 
     def validate(self):
         pass
@@ -6722,14 +6784,123 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DecreaseNodesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteApiTemplateRequest(TeaModel):
+    def __init__(self, api_name=None, region_id=None, resource_group_id=None, template_id=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 区域ID。
+        self.region_id = region_id  # type: str
+        # 资源组ID。
+        self.resource_group_id = resource_group_id  # type: str
+        # 集群模板id。
+        self.template_id = template_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteApiTemplateRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class DeleteApiTemplateResponseBody(TeaModel):
+    def __init__(self, request_id=None, success=None):
+        # 请求ID。
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteApiTemplateResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteApiTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteApiTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteApiTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteClusterRequest(TeaModel):
     def __init__(self, cluster_id=None, region_id=None):
         # The ID of the cluster.
         self.cluster_id = cluster_id  # type: str
         # The ID of the region in which you want to create the instance.
         self.region_id = region_id  # type: str
 
@@ -6820,14 +6991,113 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetApiTemplateRequest(TeaModel):
+    def __init__(self, region_id=None, template_id=None):
+        # 区域ID。
+        self.region_id = region_id  # type: str
+        # 集群模板id。
+        self.template_id = template_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetApiTemplateRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class GetApiTemplateResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ApiTemplate
+        # 请求ID。
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetApiTemplateResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ApiTemplate()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetApiTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetApiTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetApiTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetApplicationRequest(TeaModel):
     def __init__(self, application_name=None, cluster_id=None, region_id=None):
         # 应用名称。
         self.application_name = application_name  # type: str
         # 集群ID。
         self.cluster_id = cluster_id  # type: str
         # 地域ID。
@@ -25518,14 +25788,174 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = JoinResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListApiTemplatesRequest(TeaModel):
+    def __init__(self, api_name=None, max_results=None, next_token=None, region_id=None, resource_group_id=None,
+                 template_id=None, template_ids=None, template_name=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 一次获取的最大记录数。
+        self.max_results = max_results  # type: int
+        # 标记当前开始读取的位置，置空表示从头开始。
+        self.next_token = next_token  # type: str
+        # 区域ID。
+        self.region_id = region_id  # type: str
+        # 资源组ID。
+        self.resource_group_id = resource_group_id  # type: str
+        # 集群模板id。
+        self.template_id = template_id  # type: str
+        # 集群模板id列表。
+        self.template_ids = template_ids  # type: list[str]
+        # 集群模板名字。
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListApiTemplatesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_ids is not None:
+            result['TemplateIds'] = self.template_ids
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateIds') is not None:
+            self.template_ids = m.get('TemplateIds')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class ListApiTemplatesResponseBody(TeaModel):
+    def __init__(self, api_templates=None, max_results=None, next_token=None, request_id=None, total_count=None):
+        self.api_templates = api_templates  # type: list[ApiTemplate]
+        # 本次请求所返回的最大记录条数。
+        self.max_results = max_results  # type: int
+        # 返回读取到的数据位置，空代表数据已经读取完毕。
+        self.next_token = next_token  # type: str
+        # 请求ID。
+        self.request_id = request_id  # type: str
+        # 本次请求条件下的数据总量。
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.api_templates:
+            for k in self.api_templates:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListApiTemplatesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ApiTemplates'] = []
+        if self.api_templates is not None:
+            for k in self.api_templates:
+                result['ApiTemplates'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.api_templates = []
+        if m.get('ApiTemplates') is not None:
+            for k in m.get('ApiTemplates'):
+                temp_model = ApiTemplate()
+                self.api_templates.append(temp_model.from_map(k))
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListApiTemplatesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListApiTemplatesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListApiTemplatesResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListApiTemplatesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListApplicationConfigsRequest(TeaModel):
     def __init__(self, application_name=None, cluster_id=None, config_file_name=None, config_item_key=None,
                  config_item_value=None, max_results=None, next_token=None, node_group_id=None, node_id=None, region_id=None):
         # The name of the application.
         self.application_name = application_name  # type: str
         # The cluster ID.
         self.cluster_id = cluster_id  # type: str
@@ -40478,14 +40908,123 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveAutoScalingPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RunApiTemplateRequest(TeaModel):
+    def __init__(self, api_name=None, client_token=None, region_id=None, template_id=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 幂等客户端TOKEN。
+        self.client_token = client_token  # type: str
+        # 地域ID。
+        self.region_id = region_id  # type: str
+        # 集群模板id。
+        self.template_id = template_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RunApiTemplateRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class RunApiTemplateResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: str
+        # 请求ID。
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RunApiTemplateResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RunApiTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RunApiTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RunApiTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RunApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RunApplicationActionRequest(TeaModel):
     def __init__(self, action_name=None, batch_size=None, cluster_id=None, component_instance_selector=None,
                  description=None, execute_strategy=None, interval=None, region_id=None, rolling_execute=None):
         # The name of the action. Valid values:
         # 
         # *   start
         # *   stop
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/alibabacloud_emr20210320_py2.egg-info/PKG-INFO` & `alibabacloud_emr20210320_py2-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-emr20210320-py2
-Version: 1.4.2
+Name: alibabacloud_emr20210320_py2
+Version: 1.5.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320_py2-1.4.2/setup.py` & `alibabacloud_emr20210320_py2-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr20210320_py2.
 
-Created on 26/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr20210320"
 NAME = "alibabacloud_emr20210320_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Emr (20210320) SDK Library for Python2"
```

