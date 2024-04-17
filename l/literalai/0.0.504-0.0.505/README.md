# Comparing `tmp/literalai-0.0.504.tar.gz` & `tmp/literalai-0.0.505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.504.tar", last modified: Tue Apr 16 10:19:40 2024, max compression
+gzip compressed data, was "literalai-0.0.505.tar", last modified: Wed Apr 17 09:38:23 2024, max compression
```

## Comparing `literalai-0.0.504.tar` & `literalai-0.0.505.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 10:19:33.000000 literalai-0.0.504/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 10:19:40.664760 literalai-0.0.504/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-16 10:19:33.000000 literalai-0.0.504/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.660760 literalai-0.0.504/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.660760 literalai-0.0.504/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:19:40.664760 literalai-0.0.504/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-16 10:19:33.000000 literalai-0.0.504/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.391110 literalai-0.0.505/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 09:38:13.000000 literalai-0.0.505/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 09:38:23.387110 literalai-0.0.505/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 09:38:13.000000 literalai-0.0.505/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    40395 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:38:23.391110 literalai-0.0.505/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 09:38:13.000000 literalai-0.0.505/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/tests/__init__.py
```

### Comparing `literalai-0.0.504/LICENSE` & `literalai-0.0.505/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/README.md` & `literalai-0.0.505/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/__init__.py` & `literalai-0.0.505/literalai/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     delete_attachment_helper,
     get_attachment_helper,
     update_attachment_helper,
 )
 from .dataset_helpers import (
     add_generation_to_dataset_helper,
     add_step_to_dataset_helper,
-    create_experiment_helper,
-    create_experiment_item_helper,
     create_dataset_helper,
     create_dataset_item_helper,
+    create_experiment_helper,
+    create_experiment_item_helper,
     delete_dataset_helper,
     delete_dataset_item_helper,
     get_dataset_helper,
     get_dataset_item_helper,
     update_dataset_helper,
 )
 from .generation_helpers import create_generation_helper, get_generations_helper
@@ -361,19 +361,21 @@
         return self.gql_helper(*delete_score_helper(id))
 
     # Attachment API
 
     def upload_file(
         self,
         content: Union[bytes, str],
-        thread_id: str,
+        thread_id: Optional[str] = None,
         mime: Optional[str] = "application/octet-stream",
     ) -> Dict:
         id = str(uuid.uuid4())
-        body = {"fileName": id, "contentType": mime, "threadId": thread_id}
+        body = {"fileName": id, "contentType": mime}
+        if thread_id:
+            body["threadId"] = thread_id
 
         path = "/api/upload/file"
 
         with httpx.Client() as client:
             response = client.post(
                 f"{self.url}{path}",
                 json=body,
@@ -395,15 +397,17 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = (
+            {}
+        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
@@ -971,15 +975,17 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = (
+            {}
+        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
@@ -1201,17 +1207,15 @@
         name: str,
         prompt_id: Optional[str] = None,
         params: Optional[Dict] = None,
     ) -> "DatasetExperiment":
         sync_api = LiteralAPI(self.api_key, self.url)
 
         return await self.gql_helper(
-            *create_experiment_helper(
-                sync_api, dataset_id, name, prompt_id, params
-            )
+            *create_experiment_helper(sync_api, dataset_id, name, prompt_id, params)
         )
 
     async def create_experiment_item(
         self, experiment_item: DatasetExperimentItem
     ) -> DatasetExperimentItem:
         check_scores_finite(experiment_item.scores)
```

### Comparing `literalai-0.0.504/literalai/api/attachment_helpers.py` & `literalai-0.0.505/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/dataset_helpers.py` & `literalai-0.0.505/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/generation_helpers.py` & `literalai-0.0.505/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/gql.py` & `literalai-0.0.505/literalai/api/gql.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/prompt_helpers.py` & `literalai-0.0.505/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/score_helpers.py` & `literalai-0.0.505/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/step_helpers.py` & `literalai-0.0.505/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/thread_helpers.py` & `literalai-0.0.505/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/api/user_helpers.py` & `literalai-0.0.505/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/callback/langchain_callback.py` & `literalai-0.0.505/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/client.py` & `literalai-0.0.505/literalai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from typing import Any, Dict, List, Optional, Union
 
 from literalai.api import AsyncLiteralAPI, LiteralAPI
 from literalai.callback.langchain_callback import get_langchain_callback
+from literalai.callback.llama_index_callback import get_llama_index_callback
 from literalai.context import active_steps_var, active_thread_var
 from literalai.event_processor import EventProcessor
 from literalai.instrumentation.openai import instrument_openai
 from literalai.message import Message
 from literalai.my_types import Attachment
 from literalai.step import (
     MessageStepType,
@@ -72,14 +73,24 @@
         return LangchainTracer(
             self.to_sync(),
             to_ignore=to_ignore,
             to_keep=to_keep,
             **kwargs,
         )
 
+    def llama_index_callback(
+        self,
+        **kwargs: Any,
+    ):
+        LlamaIndexTracer = get_llama_index_callback()
+        return LlamaIndexTracer(
+            self.to_sync(),
+            **kwargs,
+        )
+
     def thread(
         self,
         original_function=None,
         *,
         thread_id: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs,
```

### Comparing `literalai-0.0.504/literalai/dataset.py` & `literalai-0.0.505/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/dataset_experiment.py` & `literalai-0.0.505/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/dataset_item.py` & `literalai-0.0.505/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/event_processor.py` & `literalai-0.0.505/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/filter.py` & `literalai-0.0.505/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/helper.py` & `literalai-0.0.505/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/instrumentation/openai.py` & `literalai-0.0.505/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/message.py` & `literalai-0.0.505/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/my_types.py` & `literalai-0.0.505/literalai/my_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,16 +237,16 @@
     datasetExperimentItemId: Optional[str]
     comment: Optional[str]
     tags: Optional[List[str]]
 
 
 class AttachmentDict(TypedDict, total=False):
     id: Optional[str]
-    threadId: str
-    stepId: str
+    stepId: Optional[str]
+    threadId: Optional[str]
     metadata: Optional[Dict]
     mime: Optional[str]
     name: Optional[str]
     objectKey: Optional[str]
     url: Optional[str]
 
 
@@ -300,40 +300,38 @@
         )
 
         return score
 
 
 @dataclass
 class Attachment:
-    thread_id: str
-    step_id: str
+    step_id: Optional[str] = None
+    thread_id: Optional[str] = None
     id: Optional[str] = Field(default_factory=lambda: str(uuid.uuid4()))
     metadata: Optional[Dict] = Field(default_factory=lambda: {})
     mime: Optional[str] = None
     name: Optional[str] = None
     object_key: Optional[str] = None
     url: Optional[str] = None
 
     def to_dict(self):
         return {
             "id": self.id,
-            "threadId": self.thread_id,
-            "stepId": self.step_id,
             "metadata": self.metadata,
             "mime": self.mime,
             "name": self.name,
             "objectKey": self.object_key,
             "url": self.url,
         }
 
     @classmethod
     def from_dict(cls, attachment_dict: AttachmentDict) -> "Attachment":
         id = attachment_dict.get("id", "")
-        thread_id = attachment_dict.get("threadId", "")
-        step_id = attachment_dict.get("stepId", "")
+        thread_id = attachment_dict.get("threadId", None)
+        step_id = attachment_dict.get("stepId", None)
         metadata = attachment_dict.get("metadata", {})
         mime = attachment_dict.get("mime", "")
         name = attachment_dict.get("name", "")
         object_key = attachment_dict.get("objectKey", "")
         url = attachment_dict.get("url", "")
 
         attachment = cls(
```

### Comparing `literalai-0.0.504/literalai/prompt.py` & `literalai-0.0.505/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/requirements.py` & `literalai-0.0.505/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/step.py` & `literalai-0.0.505/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/thread.py` & `literalai-0.0.505/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai/wrappers.py` & `literalai-0.0.505/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.504/literalai.egg-info/SOURCES.txt` & `literalai-0.0.505/literalai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 literalai/api/prompt_helpers.py
 literalai/api/score_helpers.py
 literalai/api/step_helpers.py
 literalai/api/thread_helpers.py
 literalai/api/user_helpers.py
 literalai/callback/__init__.py
 literalai/callback/langchain_callback.py
+literalai/callback/llama_index_callback.py
 literalai/instrumentation/__init__.py
 literalai/instrumentation/openai.py
 tests/__init__.py
```

