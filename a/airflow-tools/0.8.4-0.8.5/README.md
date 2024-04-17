# Comparing `tmp/airflow_tools-0.8.4.tar.gz` & `tmp/airflow_tools-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.8.4.tar", max compression
+gzip compressed data, was "airflow_tools-0.8.5.tar", max compression
```

## Comparing `airflow_tools-0.8.4.tar` & `airflow_tools-0.8.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11358 2024-03-15 09:01:15.875283 airflow_tools-0.8.4/LICENSE.txt
--rw-r--r--   0        0        0     8788 2024-04-11 13:00:04.903032 airflow_tools-0.8.4/README.md
--rw-r--r--   0        0        0     1312 2024-04-11 13:41:40.775249 airflow_tools-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.879171 airflow_tools-0.8.4/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-04-11 13:41:49.632435 airflow_tools-0.8.4/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-03-15 09:01:15.879695 airflow_tools-0.8.4/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-03-23 22:52:20.616265 airflow_tools-0.8.4/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-03-15 09:01:15.880246 airflow_tools-0.8.4/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.880736 airflow_tools-0.8.4/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-15 14:21:53.853567 airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-03-23 23:14:28.037837 airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.882284 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     2382 2024-04-11 13:00:04.951649 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-03-24 00:50:06.290603 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-03-25 16:17:00.235954 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-03-24 00:21:54.773711 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-03-24 00:50:06.294839 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-03-24 00:21:54.788482 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-03-15 09:01:15.884092 airflow_tools-0.8.4/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884537 airflow_tools-0.8.4/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884904 airflow_tools-0.8.4/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.885232 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-18 14:38:56.888663 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-03-15 09:01:15.885704 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886187 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886773 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-03-23 22:52:20.625836 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.887444 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.888053 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     6241 2024-04-11 13:40:29.952773 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0     9802 2024-04-11 13:00:04.955252 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
--rw-r--r--   0        0        0      821 2024-04-11 13:00:04.959496 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/tasks.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.890235 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891091 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     9015 2024-04-11 13:00:04.964694 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-03-18 14:38:56.889184 airflow_tools-0.8.4/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891899 airflow_tools-0.8.4/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/LICENSE.txt
+-rw-r--r--   0        0        0     8788 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/README.md
+-rw-r--r--   0        0        0     1315 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0     2382 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1586 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     3877 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     3396 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0     6241 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0    11455 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
+-rw-r--r--   0        0        0      821 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     9015 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10023 1970-01-01 00:00:00.000000 airflow_tools-0.8.5/PKG-INFO
```

### Comparing `airflow_tools-0.8.4/LICENSE.txt` & `airflow_tools-0.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/README.md` & `airflow_tools-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/pyproject.toml` & `airflow_tools-0.8.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.8.4"
+version = "0.8.5"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
@@ -17,15 +17,15 @@
 apache-airflow-providers-amazon = "^8.8.0"
 pendulum = "^2.1.2"
 boto3-stubs = "^1.34.8"
 boto3 = "^1.34.8"
 types-toml = "^0.10.8.7"
 types-jmespath = "^1.0.2.7"
 pandas-stubs = "^2.1.4.231218"
-apache-airflow = "^2.8"
+apache-airflow = "==2.8.*"
 flask-session = "0.5.0"
 apache-airflow-providers-sftp = "^4.8.1"
 databricks-sdk = "^0.21.0"
 databricks-sql-connector = "^2"
 
 [tool.poetry.plugins."apache_airflow_provider"]
 "provider_info" = "airflow_tools.providers.package:get_provider_info"
```

### Comparing `airflow_tools-0.8.4/src/airflow_tools/compression_utils.py` & `airflow_tools-0.8.5/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.8.5/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.8.5/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,41 +13,43 @@
     from airflow.providers.http.operators.http import SimpleHttpOperator as HttpOperator
 
 from airflow.utils.context import Context
 from airflow.utils.helpers import merge_dicts
 from requests import Response
 
 from airflow_tools.compression_utils import CompressionOptions, compress
-from airflow_tools.exceptions import ApiResponseTypeError
 from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
+from airflow_tools.exceptions import ApiResponseTypeError
+
+import logging
+logger = logging.getLogger(__file__)
 
 if TYPE_CHECKING:
     from requests.auth import AuthBase
 
 SaveFormat = Literal['jsonl']
 
 
 class HttpBatchOperator(HttpOperator):
     def execute(
         self, context: Context, use_new_data_parameters_on_pagination=False
     ) -> Any:
         self.log.info("Calling HTTP method")
-
         response = self.hook.run(
             self.endpoint, self.data, self.headers, self.extra_options
         )
         yield self.process_response(context=context, response=response)
         for response in self.paginate_sync(
             response=response,
             use_new_data_parameters_on_pagination=use_new_data_parameters_on_pagination,
         ):
             yield self.process_response(context=context, response=response)
 
     def paginate_sync(
-        self, response: Response, use_new_data_parameters_on_pagination=False
+        self, response: Response, use_new_data_parameters_on_pagination: bool = False
     ) -> Response | list[Response]:
         if not self.pagination_function:
             return None
 
         while True:
             next_page_params = self.pagination_function(response)
             if not next_page_params:
@@ -94,70 +96,63 @@
             headers=merge_dicts(self.headers, next_page_params.get("headers", {})),
             extra_options=merge_dicts(
                 self.extra_options, next_page_params.get("extra_options", {})
             ),
         )
 
 
-class HttpToFilesystem(BaseOperator):
+class HttpToDataLake(BaseOperator):
     template_fields = list(HttpOperator.template_fields) + [
-        'filesystem_path',
-        'filesystem_conn_id',
+        'data_lake_path',
+        'data_lake_conn_id',
         'jmespath_expression',
         'save_format',
     ]
     template_fields_renderers = HttpOperator.template_fields_renderers
 
     json_response_save_format = ['json', 'jsonl']
-    binary_response_save_format = ['parquet']
 
     def __init__(
         self,
         http_conn_id: str,
-        filesystem_conn_id: str,
-        filesystem_path: str,
+        data_lake_conn_id: str,
+        data_lake_path: str,
         save_format: SaveFormat = 'jsonl',
         compression: CompressionOptions = None,
         endpoint: str | None = None,
         method: str = "POST",
         data: Any = None,
         headers: dict[str, str] | None = None,
         auth_type: type['AuthBase'] | None = None,
         jmespath_expression: str | None = None,
         pagination_function: Callable | None = None,
         use_new_data_parameters_on_pagination: bool = False,
-        create_file_on_success: str | None = None,
         *args,
         **kwargs,
     ):
+        logger.warning(
+            "HttpToDataLake is deprecated and will be removed in a future version. "
+            "Please use HttpToFilesystem instead."
+        )
         super().__init__(*args, **kwargs)
         self.http_conn_id = http_conn_id
-        self.filesystem_conn_id = filesystem_conn_id
-        self.filesystem_path = filesystem_path
+        self.data_lake_conn_id = data_lake_conn_id
+        self.data_lake_path = data_lake_path
         self.save_format = save_format
         self.compression = compression
         self.endpoint = endpoint
         self.method = method
         self.data = data
         self.headers = headers
         self.auth_type = auth_type
         self.jmespath_expression = jmespath_expression
         self.pagination_function = pagination_function
         self.use_new_data_parameters_on_pagination = (
             use_new_data_parameters_on_pagination
         )
-        self.create_file_on_success = create_file_on_success
-
-        if (
-            self.save_format in self.binary_response_save_format
-            and self.compression is not None
-        ):
-            raise ValueError(
-                f'Compression is not supported for binary response save formats: {self.binary_response_save_format}'
-            )
 
     def execute(self, context: 'Context') -> Any:
         http_batch_operator = HttpBatchOperator(
             task_id='http-operator',
             http_conn_id=self.http_conn_id,
             endpoint=self.endpoint,
             method=self.method,
@@ -171,32 +166,23 @@
             http_batch_operator.execute(
                 context,
                 use_new_data_parameters_on_pagination=self.use_new_data_parameters_on_pagination,
             ),
             start=1,
         ):
             filesystem_protocol = FilesystemFactory.get_data_lake_filesystem(
-                connection=BaseHook.get_connection(self.filesystem_conn_id),
+                connection=BaseHook.get_connection(self.data_lake_conn_id),
             )
 
-            file_path = self.filesystem_path.rstrip('/') + '/' + self._file_name(i)
+            file_path = self.data_lake_path.rstrip('/') + '/' + self._file_name(i)
 
             filesystem_protocol.write(data, file_path)
 
-            if self.create_file_on_success is not None and isinstance(
-                self.create_file_on_success, str
-            ):
-                success_file_path = (
-                    self.filesystem_path.rstrip('/') + '/' + self.create_file_on_success
-                )
-                filesystem_protocol.write(BytesIO(), success_file_path)
-
     def _file_name(self, n_part) -> str:
         file_name = f'part{n_part:04}.{self.save_format}'
-
         if self.compression:
             file_name += f'.{self.compression}'
         return file_name
 
     def _response_filter(self, response) -> BytesIO:
         if (
             self.jmespath_expression
@@ -211,16 +197,14 @@
             raise ApiResponseTypeError(
                 'JMESPath expression is only supported for json and jsonl save formats'
             )
 
         elif self.save_format in self.json_response_save_format:
             self.data = response.json()
 
-        elif self.save_format in self.binary_response_save_format:
-            self.data = response.content
         else:
             self.data = response.text
 
         match self.save_format:
             case 'json':
                 return json_to_binary(self.data, self.compression)
 
@@ -231,42 +215,39 @@
                     )
                 return list_to_jsonl(self.data, self.compression)
 
             case 'xml':
                 return xml_to_binary(self.data, self.compression)
 
             case 'parquet':
-                return self.data
-
-            case 'csv':
-                return csv_to_binary(self.data, self.compression)
+                return parquet_to_binary(self.data, self.compression)
 
             case _:
                 raise NotImplementedError(f'Unknown save_format: {self.save_format}')
 
 
 def list_to_jsonl(data: list[dict], compression: 'CompressionOptions') -> BytesIO:
-    out = StringIO()
     df = pd.DataFrame(data)
+    out = BytesIO()
     df.to_json(out, orient='records', lines=True, compression=compression)
     out.seek(0)
-    return BytesIO(out.getvalue().encode())
+    return out
 
 
 def json_to_binary(data: dict, compression: 'CompressionOptions') -> BytesIO:
     json_string = json.dumps(data).encode()
     compressed_json = compress(compression, json_string)
     out = BytesIO(compressed_json)
     return out
 
 
-def csv_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
-    csv_df = pd.read_csv(StringIO(data), sep=',')
+def parquet_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
+    parquet_df = pd.DataFrame(StringIO(data))
     out = BytesIO()
-    csv_df.to_csv(out, compression=compression, index=False)
+    parquet_df.to_parquet(out, compression=compression)
     out.seek(0)
     return out
 
 
 def xml_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
     compressed_xml = compress(compression, data.encode())
     out = BytesIO(compressed_xml)
```

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/tasks.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/tasks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from io import BytesIO, StringIO
-from typing import TYPE_CHECKING, Any, Callable, Literal
+from typing import TYPE_CHECKING, Any, Callable, Literal, Optional, Protocol
 
 import jmespath
 import pandas as pd
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator
 
 try:
@@ -13,43 +13,46 @@
     from airflow.providers.http.operators.http import SimpleHttpOperator as HttpOperator
 
 from airflow.utils.context import Context
 from airflow.utils.helpers import merge_dicts
 from requests import Response
 
 from airflow_tools.compression_utils import CompressionOptions, compress
-from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
 from airflow_tools.exceptions import ApiResponseTypeError
-
-import logging
-logger = logging.getLogger(__file__)
+from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
 
 if TYPE_CHECKING:
     from requests.auth import AuthBase
 
 SaveFormat = Literal['jsonl']
 
 
+class Transformation(Protocol):
+    def __call__(self, data: bytes, **kwargs) -> bytes:
+        ...
+
+
 class HttpBatchOperator(HttpOperator):
     def execute(
         self, context: Context, use_new_data_parameters_on_pagination=False
     ) -> Any:
         self.log.info("Calling HTTP method")
+
         response = self.hook.run(
             self.endpoint, self.data, self.headers, self.extra_options
         )
         yield self.process_response(context=context, response=response)
         for response in self.paginate_sync(
             response=response,
             use_new_data_parameters_on_pagination=use_new_data_parameters_on_pagination,
         ):
             yield self.process_response(context=context, response=response)
 
     def paginate_sync(
-        self, response: Response, use_new_data_parameters_on_pagination: bool = False
+        self, response: Response, use_new_data_parameters_on_pagination=False
     ) -> Response | list[Response]:
         if not self.pagination_function:
             return None
 
         while True:
             next_page_params = self.pagination_function(response)
             if not next_page_params:
@@ -96,63 +99,91 @@
             headers=merge_dicts(self.headers, next_page_params.get("headers", {})),
             extra_options=merge_dicts(
                 self.extra_options, next_page_params.get("extra_options", {})
             ),
         )
 
 
-class HttpToDataLake(BaseOperator):
+class HttpToFilesystem(BaseOperator):
     template_fields = list(HttpOperator.template_fields) + [
-        'data_lake_path',
-        'data_lake_conn_id',
+        'filesystem_path',
+        'filesystem_conn_id',
         'jmespath_expression',
         'save_format',
+        'source_format',
     ]
     template_fields_renderers = HttpOperator.template_fields_renderers
 
-    json_response_save_format = ['json', 'jsonl']
+    json_response_source_format = ['json', 'jsonl']
+    binary_response_source_format = ['parquet']
 
     def __init__(
         self,
         http_conn_id: str,
-        data_lake_conn_id: str,
-        data_lake_path: str,
+        filesystem_conn_id: str,
+        filesystem_path: str,
         save_format: SaveFormat = 'jsonl',
+        source_format: SaveFormat = None,
         compression: CompressionOptions = None,
         endpoint: str | None = None,
         method: str = "POST",
         data: Any = None,
         headers: dict[str, str] | None = None,
         auth_type: type['AuthBase'] | None = None,
         jmespath_expression: str | None = None,
         pagination_function: Callable | None = None,
         use_new_data_parameters_on_pagination: bool = False,
+        create_file_on_success: str | None = None,
+        data_transformation: Optional[Transformation] = None,
+        data_transformation_kwargs: dict[str, Any] | None = None,
         *args,
         **kwargs,
     ):
-        logger.warning(
-            "HttpToDataLake is deprecated and will be removed in a future version. "
-            "Please use HttpToFilesystem instead."
-        )
         super().__init__(*args, **kwargs)
         self.http_conn_id = http_conn_id
-        self.data_lake_conn_id = data_lake_conn_id
-        self.data_lake_path = data_lake_path
-        self.save_format = save_format
+        self.filesystem_conn_id = filesystem_conn_id
+        self.filesystem_path = filesystem_path
         self.compression = compression
         self.endpoint = endpoint
         self.method = method
         self.data = data
         self.headers = headers
         self.auth_type = auth_type
         self.jmespath_expression = jmespath_expression
         self.pagination_function = pagination_function
         self.use_new_data_parameters_on_pagination = (
             use_new_data_parameters_on_pagination
         )
+        self.create_file_on_success = create_file_on_success
+        self.data_transformation = data_transformation
+        self.data_transformation_kwargs = data_transformation_kwargs
+
+        self.save_format = save_format
+        self.source_format = source_format if source_format else save_format
+        self.kwargs = kwargs
+
+        if (
+            self.save_format in self.binary_response_source_format
+            and self.compression is not None
+        ):
+            raise ValueError(
+                f'Compression is not supported for binary response save formats: {self.binary_response_source_format}'
+            )
+
+        if self.data_transformation and not callable(self.data_transformation):
+            raise ValueError('data_transformation must be a callable')
+
+        if self.data_transformation is None and self.source_format != self.save_format:
+            raise ValueError(
+                'data_transformation must be provided if source_format is different from save_format'
+            )
+        if self.data_transformation_kwargs and self.data_transformation is None:
+            raise ValueError(
+                'data_transformation must be provided if data_transformation_kwargs is provided'
+            )
 
     def execute(self, context: 'Context') -> Any:
         http_batch_operator = HttpBatchOperator(
             task_id='http-operator',
             http_conn_id=self.http_conn_id,
             endpoint=self.endpoint,
             method=self.method,
@@ -166,88 +197,111 @@
             http_batch_operator.execute(
                 context,
                 use_new_data_parameters_on_pagination=self.use_new_data_parameters_on_pagination,
             ),
             start=1,
         ):
             filesystem_protocol = FilesystemFactory.get_data_lake_filesystem(
-                connection=BaseHook.get_connection(self.data_lake_conn_id),
+                connection=BaseHook.get_connection(self.filesystem_conn_id),
             )
 
-            file_path = self.data_lake_path.rstrip('/') + '/' + self._file_name(i)
+            file_path = self.filesystem_path.rstrip('/') + '/' + self._file_name(i)
 
             filesystem_protocol.write(data, file_path)
 
+            if self.create_file_on_success is not None and isinstance(
+                self.create_file_on_success, str
+            ):
+                success_file_path = (
+                    self.filesystem_path.rstrip('/') + '/' + self.create_file_on_success
+                )
+                filesystem_protocol.write(BytesIO(), success_file_path)
+
     def _file_name(self, n_part) -> str:
         file_name = f'part{n_part:04}.{self.save_format}'
+
         if self.compression:
             file_name += f'.{self.compression}'
         return file_name
 
     def _response_filter(self, response) -> BytesIO:
         if (
             self.jmespath_expression
-            and self.save_format in self.json_response_save_format
+            and self.source_format in self.json_response_source_format
         ):
             self.data = jmespath.search(self.jmespath_expression, response.json())
 
         elif (
             self.jmespath_expression
-            and self.save_format not in self.json_response_save_format
+            and self.source_format not in self.json_response_source_format
         ):
             raise ApiResponseTypeError(
                 'JMESPath expression is only supported for json and jsonl save formats'
             )
-
-        elif self.save_format in self.json_response_save_format:
+        elif self.source_format in self.json_response_source_format:
             self.data = response.json()
 
+        elif self.source_format in self.binary_response_source_format:
+            self.data = response.content
         else:
             self.data = response.text
 
-        match self.save_format:
+        # Check if we have a custom data transformation
+        if self.data_transformation and self.data_transformation_kwargs:
+            return self.data_transformation(self.data, self.data_transformation_kwargs)
+        elif self.data_transformation:
+            return self.data_transformation(self.data)
+
+        # If we don't have a custom data transformation, use the default one based on the source_format
+
+        match self.source_format:
             case 'json':
                 return json_to_binary(self.data, self.compression)
 
             case 'jsonl':
                 if not isinstance(self.data, list):
                     raise ApiResponseTypeError(
                         'Expected response can\'t be transformed to jsonl. It is not  list[dict]'
                     )
                 return list_to_jsonl(self.data, self.compression)
 
             case 'xml':
                 return xml_to_binary(self.data, self.compression)
 
             case 'parquet':
-                return parquet_to_binary(self.data, self.compression)
+                return self.data
+
+            case 'csv':
+                return csv_to_binary(self.data, self.compression)
 
             case _:
-                raise NotImplementedError(f'Unknown save_format: {self.save_format}')
+                raise NotImplementedError(
+                    f'Unknown source_format/save_format: {self.source_format}'
+                )
 
 
 def list_to_jsonl(data: list[dict], compression: 'CompressionOptions') -> BytesIO:
+    out = StringIO()
     df = pd.DataFrame(data)
-    out = BytesIO()
     df.to_json(out, orient='records', lines=True, compression=compression)
     out.seek(0)
-    return out
+    return BytesIO(out.getvalue().encode())
 
 
 def json_to_binary(data: dict, compression: 'CompressionOptions') -> BytesIO:
     json_string = json.dumps(data).encode()
     compressed_json = compress(compression, json_string)
     out = BytesIO(compressed_json)
     return out
 
 
-def parquet_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
-    parquet_df = pd.DataFrame(StringIO(data))
+def csv_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
+    csv_df = pd.read_csv(StringIO(data), sep=',')
     out = BytesIO()
-    parquet_df.to_parquet(out, compression=compression)
+    csv_df.to_csv(out, compression=compression, index=False)
     out.seek(0)
     return out
 
 
 def xml_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
     compressed_xml = compress(compression, data.encode())
     out = BytesIO(compressed_xml)
```

### Comparing `airflow_tools-0.8.4/src/airflow_tools/providers/package.py` & `airflow_tools-0.8.5/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.4/PKG-INFO` & `airflow_tools-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.8.4
+Version: 0.8.5
 Summary: 
 Author: Biel Llobera
 Author-email: biel_llobera@dkl.digital
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: apache-airflow (>=2.8,<3.0)
+Requires-Dist: apache-airflow (==2.8.*)
 Requires-Dist: apache-airflow-providers-amazon (>=8.8.0,<9.0.0)
 Requires-Dist: apache-airflow-providers-microsoft-azure (>=8.0.0,<9.0.0)
 Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
 Requires-Dist: apache-airflow-providers-slack (>=8.5.1,<9.0.0)
 Requires-Dist: boto3 (>=1.34.8,<2.0.0)
 Requires-Dist: boto3-stubs (>=1.34.8,<2.0.0)
 Requires-Dist: databricks-sdk (>=0.21.0,<0.22.0)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.4 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.5 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
-airflow (>=2.8,<3.0) Requires-Dist: apache-airflow-providers-amazon
+airflow (==2.8.*) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
 Requires-Dist: apache-airflow-providers-slack (>=8.5.1,<9.0.0) Requires-Dist:
 boto3 (>=1.34.8,<2.0.0) Requires-Dist: boto3-stubs (>=1.34.8,<2.0.0) Requires-
 Dist: databricks-sdk (>=0.21.0,<0.22.0) Requires-Dist: databricks-sql-connector
 (>=2,<3) Requires-Dist: flask-session (==0.5.0) Requires-Dist: jmespath
 (>=1.0.1,<2.0.0) Requires-Dist: pandas (>=2.1.1,<3.0.0) Requires-Dist: pandas-
```

