# Comparing `tmp/seatable-api-2.6.8.tar.gz` & `tmp/seatable-api-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatable-api-2.6.8.tar", last modified: Tue Jul 18 02:30:55 2023, max compression
+gzip compressed data, was "dist/seatable-api-2.7.0.tar", last modified: Wed Apr 17 01:48:29 2024, max compression
```

## Comparing `seatable-api-2.6.8.tar` & `seatable-api-2.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.472575 seatable-api-2.6.8/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.8/LICENSE
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-18 02:30:55.471937 seatable-api-2.6.8/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.8/README.md
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.457288 seatable-api-2.6.8/seatable_api/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/column.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/constants.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1338 2023-07-18 02:27:59.000000 seatable-api-2.6.8/seatable_api/context.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    29203 2023-07-18 02:27:59.000000 seatable-api-2.6.8/seatable_api/convert_airtable.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/date_utils.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.8/seatable_api/exception.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    42361 2023-07-14 06:55:21.000000 seatable-api-2.6.8/seatable_api/main.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/message.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/query.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/socket_io.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/utils.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.467387 seatable-api-2.6.8/seatable_api.egg-info/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/requires.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-07-18 02:30:55.473270 seatable-api-2.6.8/setup.cfg
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-07-18 02:29:40.000000 seatable-api-2.6.8/setup.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.469389 seatable-api-2.6.8/tests/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.8/tests/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.8/tests/dateutils_test.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.512951 seatable-api-2.7.0/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-17 01:48:29.512596 seatable-api-2.7.0/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      300 2021-01-29 01:36:12.000000 seatable-api-2.7.0/README.md
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.453836 seatable-api-2.7.0/seatable_api/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      171 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    26810 2024-04-17 01:46:18.000000 seatable-api-2.7.0/seatable_api/api_gateway.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    11418 2021-01-29 01:36:12.000000 seatable-api-2.7.0/seatable_api/column.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1135 2021-12-15 04:05:31.000000 seatable-api-2.7.0/seatable_api/constants.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1338 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/context.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    29203 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/convert_airtable.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    13988 2024-03-21 06:02:17.000000 seatable-api-2.7.0/seatable_api/date_utils.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      235 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/exception.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    49205 2024-04-17 01:44:37.000000 seatable-api-2.7.0/seatable_api/main.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2876 2021-07-17 06:11:15.000000 seatable-api-2.7.0/seatable_api/message.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     3006 2021-01-13 04:11:42.000000 seatable-api-2.7.0/seatable_api/parsetab.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     9400 2021-02-24 08:59:41.000000 seatable-api-2.7.0/seatable_api/query.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2744 2021-07-17 06:11:15.000000 seatable-api-2.7.0/seatable_api/socket_io.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     7276 2024-03-27 08:04:05.000000 seatable-api-2.7.0/seatable_api/utils.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.485168 seatable-api-2.7.0/seatable_api.egg-info/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      591 2024-04-17 01:48:29.000000 seatable-api-2.7.0/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        1 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       47 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       19 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       38 2024-04-17 01:48:29.513113 seatable-api-2.7.0/setup.cfg
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      723 2024-04-17 01:47:54.000000 seatable-api-2.7.0/setup.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.511343 seatable-api-2.7.0/tests/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        0 2023-04-14 03:49:39.000000 seatable-api-2.7.0/tests/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     5261 2023-04-14 03:49:39.000000 seatable-api-2.7.0/tests/dateutils_test.py
```

### Comparing `seatable-api-2.6.8/PKG-INFO` & `seatable-api-2.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.8
+Version: 2.7.0
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
+Description: # seatable-api-python
+        
+        Python client for SeaTable web api
+        
+        English document: <https://seatable.github.io/seatable-scripts/>
+        
+        Chinese document: <https://seatable.github.io/seatable-scripts-cn/>
+        
+        pypi: <https://pypi.org/project/seatable-api/>
+        
+        github: <https://github.com/seatable/seatable-api-python>
+        
 Platform: any
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# seatable-api-python
-
-Python client for SeaTable web api
-
-English document: <https://seatable.github.io/seatable-scripts/>
-
-Chinese document: <https://seatable.github.io/seatable-scripts-cn/>
-
-pypi: <https://pypi.org/project/seatable-api/>
-
-github: <https://github.com/seatable/seatable-api-python>
-
-
```

### Comparing `seatable-api-2.6.8/seatable_api/column.py` & `seatable-api-2.7.0/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/constants.py` & `seatable-api-2.7.0/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/context.py` & `seatable-api-2.7.0/seatable_api/context.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/convert_airtable.py` & `seatable-api-2.7.0/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/date_utils.py` & `seatable-api-2.7.0/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/main.py` & `seatable-api-2.7.0/seatable_api/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,54 +4,39 @@
 from datetime import datetime, timedelta
 from urllib import parse
 from uuid import UUID
 
 # https://requests.readthedocs.io
 import requests
 
-from seatable_api.exception import AuthExpiredError
+from seatable_api.api_gateway import APIGateway
+from seatable_api.exception import AuthExpiredError, BaseUnauthError
 from seatable_api.message import get_sender_by_account
 from .constants import ROW_FILTER_KEYS, ColumnTypes
 from .constants import RENAME_COLUMN, RESIZE_COLUMN, FREEZE_COLUMN, MOVE_COLUMN, MODIFY_COLUMN_TYPE, DELETE_COLUMN
 from .socket_io import SocketIO
 from .query import QuerySet
-from .utils import convert_db_rows
+from .utils import convert_db_rows, parse_server_url, parse_headers, like_table_id, parse_response
 
 
-def parse_headers(token):
-    return {
-        'Authorization': 'Token ' + token,
-        'Content-Type': 'application/json',
-    }
+def check_auth(func):
 
-
-def parse_server_url(server_url):
-    return server_url.rstrip('/')
-
-
-def parse_response(response):
-    if response.status_code >= 400:
-        try:
-            err_data = json.loads(response.text)
-        except:
-            err_data = {}
-        if err_data.get("error_msg") == "Token expired." and \
-            response.status_code == 403:
-            raise AuthExpiredError
-
-        raise ConnectionError(response.status_code, response.text)
-    else:
-        try:
-            data = json.loads(response.text)
-            return data
-        except:
-            pass
-
-def like_table_id(value):
-    return re.match(r'^[-0-9a-zA-Z]{4}$', value)
+    def wrapper(obj, *args, **kwargs):
+        if not obj.is_authed:
+            raise BaseUnauthError
+        return func(obj, *args, **kwargs)
+    return wrapper
+
+def api_gateway_wrapper(func):
+    def wrapper(obj, *args, **kwargs):
+        if obj.use_api_gateway:
+            new_obj = obj.api_gateway
+            return getattr(new_obj, func.__name__)(*args, **kwargs)
+        return func(obj, *args, **kwargs)
+    return wrapper
 
 
 class SeaTableAPI(object):
     """SeaTable API
     """
 
     def __init__(self, token, server_url):
@@ -67,14 +52,18 @@
         self.jwt_exp = None
         self.headers = None
         self.workspace_id = None
         self.dtable_uuid = None
         self.dtable_name = None
         self.timeout = 30
         self.socketIO = None
+        self.is_authed = False
+
+        self.use_api_gateway = False
+        self.api_gateway = None
 
     def __str__(self):
         return '<SeaTable Base [ %s ]>' % self.dtable_name
 
     def _clone(self):
         clone = self.__class__(self.token, self.server_url)
         clone.dtable_server_url = self.dtable_server_url
@@ -82,14 +71,18 @@
         clone.jwt_token = self.jwt_token
         clone.jwt_exp = self.jwt_exp
         clone.headers = self.headers
         clone.workspace_id = self.workspace_id
         clone.dtable_uuid = self.dtable_uuid
         clone.dtable_name = self.dtable_name
         clone.timeout = self.timeout
+        clone.is_authed = self.is_authed
+
+        clone.use_api_gateway = self.use_api_gateway
+        clone.api_gateway = self.api_gateway
         return clone
 
     def _get_msg_sender_by_account(self, account_name):
         try:
             account = self._get_account_detail(account_name)
             msg_sender = get_sender_by_account(account)
         except:
@@ -109,25 +102,41 @@
         self.dtable_db_url = parse_server_url(data.get('dtable_db', ''))
         self.jwt_token = data.get('access_token')
         self.headers = parse_headers(self.jwt_token)
         self.workspace_id = data.get('workspace_id')
         self.dtable_uuid = data.get('dtable_uuid')
         self.dtable_name = data.get('dtable_name')
 
+        # api gateway entry
+        self.use_api_gateway = data.get('use_api_gateway')
+        if self.use_api_gateway:
+            self.api_gateway = APIGateway(
+                token = self.token,
+                api_gateway_url=self.server_url + '/api-gateway',
+                server_url=self.server_url,
+                headers=self.headers,
+                dtable_uuid=self.dtable_uuid
+            )
+
         if with_socket_io is True:
             base = self._clone()
             self.socketIO = SocketIO(base)
             self.socketIO._connect()
 
+        self.is_authed = True
+
     def _metadata_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/metadata/'
 
     def _table_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/tables/'
 
+    def _view_server_url(self):
+        return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/views/'
+
     def _row_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/rows/'
 
     def _batch_row_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/batch-append-rows/'
 
     def _batch_update_row_server_url(self):
@@ -159,14 +168,17 @@
 
     def _app_custom_upload_link_url(self):
         return self.server_url + '/api/v2.1/dtable/custom/app-upload-link/'
 
     def _app_upload_link_url(self):
         return self.server_url + '/api/v2.1/dtable/app-upload-link/'
 
+    def _app_user_info_url(self):
+        return self.server_url + '/api/v2.1/dtable/app-user-info/'
+
     def _column_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/columns/'
 
     def _column_options_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/column-options/'
 
     def _column_cascade_setting_server_url(self):
@@ -209,35 +221,56 @@
         }
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
 
         data = parse_response(response)
         return data.get('account')
 
+    @check_auth
     def send_email(self, account_name, msg,  **kwargs):
         msg_sender = self._get_msg_sender_by_account(account_name)
         if not msg_sender or msg_sender.msg_type != 'email':
             raise ValueError('Email message sender does not configered.')
         msg_sender.send_msg(msg, **kwargs)
 
+    @check_auth
     def send_wechat_msg(self, account_name, msg):
         msg_sender = self._get_msg_sender_by_account(account_name)
         if not msg_sender or msg_sender.msg_type != 'wechat':
             raise ValueError('Wechat message sender does not configered.')
         msg_sender.send_msg(msg)
 
+    @check_auth
+    @api_gateway_wrapper
     def get_metadata(self):
         """
         :return: dict
         """
         url = self._metadata_server_url()
         response = requests.get(url, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('metadata')
 
+
+    @check_auth
+    @api_gateway_wrapper
+    def list_tables(self):
+        meta = self.get_metadata()
+        return meta.get('tables') or []
+
+    @check_auth
+    @api_gateway_wrapper
+    def get_table_by_name(self, table_name):
+        tables = self.list_tables()
+        for t in tables:
+            if t.get('name') == table_name:
+                return t
+
+    @check_auth
+    @api_gateway_wrapper
     def add_table(self, table_name, lang='en', columns=[]):
         """
         :param table_name: str
         :param lang: str, currently 'en' for English, and 'zh-cn' for Chinese
         :param columns: list
         """
         url = self._table_server_url()
@@ -246,14 +279,100 @@
             'lang': lang,
         }
         if columns:
             json_data['columns'] = columns
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
+    def rename_table(self, table_name, new_table_name):
+        url = self._table_server_url()
+        json_data = {
+            'table_name': table_name,
+            'new_table_name': new_table_name
+        }
+        response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def delete_table(self, table_name):
+        url = self._table_server_url()
+        json_data = {
+            'table_name': table_name,
+        }
+        response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def list_views(self, table_name):
+        url = self._view_server_url()
+        params = {
+            'table_name': table_name
+        }
+        response = requests.get(url, params=params, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def get_view_by_name(self, table_name, view_name):
+        url = self._view_server_url()
+        view_url = '%(url)s/%(view_name)s/?table_name=%(table_name)s' % ({
+            "url": url.rstrip('/'),
+            'view_name': view_name,
+            'table_name': table_name
+        })
+        response = requests.get(view_url, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def add_view(self, table_name, view_name):
+        url = self._view_server_url()
+        view_url = '%(url)s/?table_name=%(table_name)s' % ({
+            "url": url.rstrip('/'),
+            'table_name': table_name
+        })
+        json_data = {
+            'name': view_name
+        }
+        response = requests.post(view_url, json=json_data, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def rename_view(self, table_name, view_name, new_view_name):
+        url = self._view_server_url()
+        view_url = '%(url)s/%(view_name)s/?table_name=%(table_name)s' % ({
+            "url": url.rstrip('/'),
+            'view_name': view_name,
+            'table_name': table_name
+        })
+        json_data = {
+            'name': new_view_name
+        }
+        response = requests.put(view_url, json=json_data, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
+    def delete_view(self, table_name, view_name):
+        url = self._view_server_url()
+        view_url = '%(url)s/%(view_name)s/?table_name=%(table_name)s' % ({
+            "url": url.rstrip('/'),
+            'view_name': view_name,
+            'table_name': table_name
+        })
+        response = requests.delete(view_url, headers=self.headers, timeout=self.timeout)
+        return parse_response(response)
+
+    @check_auth
+    @api_gateway_wrapper
     def list_rows(self, table_name, view_name=None, order_by=None, desc=False, start=None, limit=None):
         """
         :param table_name: str
         :param view_name: str
         :param order_by: str
         :param desc: boolean
         :param start: int
@@ -276,14 +395,17 @@
             params['start'] = start
         if limit:
             params['limit'] = limit
         response = requests.get(url, params=params, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('rows')
 
+
+    @check_auth
+    @api_gateway_wrapper
     def get_row(self, table_name, row_id):
         """
         :param table_name: str
         :param row_id: str
         :return: dict
         """
         url = self._row_server_url() + row_id + '/'
@@ -293,61 +415,75 @@
 
         if like_table_id(table_name):
             params['table_id'] = table_name
         response = requests.get(url, params=params, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
-    def append_row(self, table_name, row_data):
+    @check_auth
+    @api_gateway_wrapper
+    def append_row(self, table_name, row_data, apply_default=None):
         """
         :param table_name: str
         :param row_data: dict
         """
         url = self._row_server_url()
         json_data = {
             'table_name': table_name,
             'row': row_data,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
+        if apply_default is not None:
+            json_data['apply_default'] = apply_default
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
-    def batch_append_rows(self, table_name, rows_data):
+    @check_auth
+    @api_gateway_wrapper
+    def batch_append_rows(self, table_name, rows_data, apply_default=None):
         """
         :param table_name: str
         :param rows_data: dict
         """
         url = self._batch_row_server_url()
         json_data = {
             'table_name': table_name,
             'rows': rows_data,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
+        if apply_default is not None:
+            json_data['apply_default'] = apply_default
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
-    def insert_row(self, table_name, row_data, anchor_row_id):
+    @check_auth
+    @api_gateway_wrapper
+    def insert_row(self, table_name, row_data, anchor_row_id, apply_default=None):
         """
         :param table_name: str
         :param row_data: dict
         :param anchor_row_id: str
         """
         url = self._row_server_url()
         json_data = {
             'table_name': table_name,
             'row': row_data,
             'anchor_row_id': anchor_row_id,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
+        if apply_default is not None:
+            json_data['apply_default'] = apply_default
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def update_row(self, table_name, row_id, row_data):
         """
         :param table_name: str
         :param row_id: str
         :param row_data: dict
         """
         url = self._row_server_url()
@@ -357,14 +493,16 @@
             'row': row_data,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def batch_update_rows(self, table_name, rows_data):
         """
         :param table_name: str
         :param rows_data: list
         :return:
         """
         url = self._batch_update_row_server_url()
@@ -373,14 +511,16 @@
             'updates': rows_data,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def delete_row(self, table_name, row_id):
         """
         :param table_name: str
         :param row_id: str
         """
         url = self._row_server_url()
         json_data = {
@@ -388,14 +528,16 @@
             'row_id': row_id,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def batch_delete_rows(self, table_name, row_ids):
         """
         :param table_name: str
         :param row_ids: list
         """
         url = self._batch_delete_row_server_url()
         json_data = {
@@ -403,14 +545,16 @@
             'row_ids': row_ids,
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def filter_rows(self, table_name, filters, view_name=None, filter_conjunction='And'):
         """
         :param table_name: str
         :param view_name: str
         :param filters: list
         :param filter_conjunction: str, 'And' or 'Or'
         :return: list
@@ -445,36 +589,40 @@
 
         url = self._filtered_rows_server_url()
         response = requests.get(
             url, json=json_data, params=params, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('rows')
 
+    @check_auth
     def get_file_download_link(self, path):
         """
         :param path: str
         :return: str
         """
         url = self._app_download_link_url()
         params = {'path': path}
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('download_link')
 
+    @check_auth
     def get_file_upload_link(self):
         """
         :return: dict
         """
         url = self._app_upload_link_url()
         headers = parse_headers(self.token)
         response = requests.get(url, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def add_link(self, link_id, table_name, other_table_name, row_id, other_row_id):
         """
         :param link_id: str
         :param table_name: str
         :param other_table_name: str
         :param row_id: str
         :param other_row_id: str
@@ -490,14 +638,16 @@
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         if like_table_id(other_table_name):
             json_data['other_table_id'] = other_table_name
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def remove_link(self, link_id, table_name, other_table_name, row_id, other_row_id):
         """
         :param link_id: str
         :param table_name: str
         :param other_table_name: str
         :param row_id: str
         :param other_row_id: str
@@ -513,14 +663,16 @@
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         if like_table_id(other_table_name):
             json_data['other_table_id'] = other_table_name
         response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def update_link(self, link_id, table_name, other_table_name, row_id, other_rows_ids):
         """
         :param link_id: str
         :param table_name: str
         :param other_table_name: str
         :param row_id: str
         :param other_rows_ids: list
@@ -538,14 +690,16 @@
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         if like_table_id(other_table_name):
             json_data['other_table_id'] = other_table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def batch_update_links(self, link_id, table_name, other_table_name, row_id_list, other_rows_ids_map):
         """
         :param link_id: str
         :param table_name: str
         :param other_table_name: str
         :param row_id_list: []
         :param other_rows_ids_map: dict
@@ -563,14 +717,15 @@
             json_data['table_id'] = table_name
         if like_table_id(other_table_name):
             json_data['other_table_id'] = other_table_name
 
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
     def get_linked_records(self, table_id, link_column_key, rows):
         """
         :param table_id:  str
         :param link_column_key: str
         :param rows: list
         """
         url = self._dtable_db_linked_records_url()
@@ -578,14 +733,16 @@
             'table_id': table_id,
             'link_column': link_column_key,
             'rows': rows,
         }
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
+    @check_auth
+    @api_gateway_wrapper
     def list_columns(self, table_name, view_name=None):
         """
         :param table_name: str
         :param view_name: str
         :return: list
         """
         url = self._column_server_url()
@@ -596,21 +753,43 @@
             params['table_id'] = table_name
         if view_name:
             params['view_name'] = view_name
         response = requests.get(url, params=params, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('columns')
 
-    def get_column_link_id(self, table_name, column_name, view_name=None):
-        columns = self.list_columns(table_name, view_name)
+    @check_auth
+    @api_gateway_wrapper
+    def get_column_link_id(self, table_name, column_name):
+        columns = self.list_columns(table_name)
         for column in columns:
             if column.get('name') == column_name and column.get('type') == 'link':
                 return column.get('data', {}).get('link_id')
-        raise ValueError('link type column "%s" does not exist in current view' % column_name)
+        raise ValueError('link type column "%s" does not exist in current table' % column_name)
+
+    @check_auth
+    @api_gateway_wrapper
+    def get_column_by_name(self, table_name, column_name):
+        columns = self.list_columns(table_name)
+        for col in columns:
+            if col.get('name') == column_name:
+                return col
+
+    @check_auth
+    @api_gateway_wrapper
+    def get_columns_by_type(self, table_name, column_type:ColumnTypes):
+        if column_type not in ColumnTypes:
+            raise ValueError("type %s invalid!" % (column_type,))
+        columns = self.list_columns(table_name)
+        cols_results = [col for col in columns if col.get('type') == column_type.value]
+        return cols_results
+
 
+    @check_auth
+    @api_gateway_wrapper
     def insert_column(self, table_name, column_name, column_type, column_key=None, column_data=None):
         """
         :param table_name: str
         :param column_name: str
         :param column_type: ColumnType enum
         :param column_key: str, which you want to insert after
         :param column_data: dict, config information of column
@@ -630,14 +809,16 @@
             json_data['anchor_column'] = column_key
         if column_data:
             json_data['column_data'] = column_data
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def rename_column(self, table_name, column_key, new_column_name):
         """
         :param table_name: str
         :param column_key: str
         :param new_column_name: str
         :return: dict
         """
@@ -650,14 +831,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def resize_column(self, table_name, column_key, new_column_width):
         """
         :param table_name: str
         :param column_key: str
         :param old_column_width: int
         :param new_column_width: int
         :return: dict
@@ -671,14 +854,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def freeze_column(self, table_name, column_key, frozen):
         """
         :param table_name: str
         :param column_key: str
         :param frozen: bool
         :return: dict
         """
@@ -691,14 +876,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def move_column(self, table_name, column_key, target_column_key):
         """
         :param table_name: str
         :param column_key: str
         :param target_column_key: bool
         :return: dict
         """
@@ -711,14 +898,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def modify_column_type(self, table_name, column_key, new_column_type):
         """
         :param table_name: str
         :param column_key: str
         :param new_column_type: str
         :return: dict
         """
@@ -733,14 +922,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def add_column_options(self, table_name, column, options):
         """
         :param table_name: str
         :param column: str
         :param options: list
         """
         url = self._column_options_server_url()
@@ -751,14 +942,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def add_column_cascade_settings(self, table_name, child_column, parent_column, cascade_settings):
         """
 
         :param table_name:  str
         :param child_column: str
         :param parent_column: str
         :param cascade_settings: dict
@@ -773,14 +966,16 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    @api_gateway_wrapper
     def delete_column(self, table_name, column_key):
         """
         :param table_name: str
         :param column_key: str
         :return: None
         """
         url = self._column_server_url()
@@ -790,25 +985,27 @@
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
     def download_file(self, url, save_path):
         if not str(UUID(self.dtable_uuid)) in url:
             raise Exception('url invalid.')
         path = url.split(str(UUID(self.dtable_uuid)))[-1].strip('/')
         download_link = self.get_file_download_link(parse.unquote(path))
         response = requests.get(download_link, timeout=self.timeout)
         if response.status_code != 200:
             raise Exception('download file error')
         with open(save_path, 'wb') as f:
             f.write(response.content)
 
+    @check_auth
     def upload_bytes_file(self, name, content: bytes, relative_path=None, file_type=None, replace=False):
         """
         relative_path: relative path for upload, if None, default {file_type}s/{date of this month} eg: files/2020-09
         file_type: if relative is None, file type must in ['image', 'file'], default 'file'
         return: info dict of uploaded file
         """
         upload_link_dict = self.get_file_upload_link()
@@ -841,14 +1038,15 @@
         return {
             'type': file_type,
             'size': d.get('size'),
             'name': d.get('name'),
             'url': url
         }
 
+    @check_auth
     def upload_local_file(self, file_path, name=None, relative_path=None, file_type=None, replace=False):
         """
         relative_path: relative path for upload, if None, default {file_type}s/{date of today}, eg: files/2020-09
         file_type: if relative is None, file type must in ['image', 'file'], default 'file'
         return: info dict of uploaded file
         """
         if file_type not in ['image', 'file']:
@@ -885,28 +1083,31 @@
         return {
             'type': file_type,
             'size': d.get('size'),
             'name': d.get('name'),
             'url': url
         }
 
+    @check_auth
     def filter(self, table_name, conditions='', view_name=None):
         """
         :param table_name: str
         :param conditions: str
         :return: queryset
         """
         base = self._clone()
         queryset = QuerySet(base, table_name)
         queryset.raw_rows = self.list_rows(table_name, view_name)
         queryset.raw_columns = self.list_columns(table_name, view_name)
         queryset.conditions = conditions
         queryset._execute_conditions()
         return queryset
 
+    @check_auth
+    @api_gateway_wrapper
     def query(self, sql, convert=True):
         """
         :param sql: str
         :param convert: bool
         :return: list
         """
         if not sql:
@@ -921,86 +1122,95 @@
         results = data.get('results')
         if convert:
             converted_results = convert_db_rows(metadata, results)
             return converted_results
         else:
             return results
 
+    @check_auth
     def get_related_users(self):
         response = requests.get(self._get_related_users_url(), headers=self.headers)
         return parse_response(response)['user_list']
 
+    @check_auth
+    @api_gateway_wrapper
     def send_toast_notification(self, username, msg, toast_type='success'):
         url = self._send_toast_notification_url()
         requests.post(url, json={
             'to_user': username,
             'toast_type': toast_type,
             'detail': {
                 'msg': str(msg)
             }
         }, headers=self.headers)
 
+    @check_auth
     def add_workflow_task(self, workflow_token, row_data, initiator=None, link_rows=None, new_linked_rows=None):
         url = self._add_workflow_task_url(workflow_token)
         headers = {'Authorization': 'Token ' + self.jwt_token}
         response = requests.post(url, data={
             'row_data': json.dumps(row_data),
             'initiator': initiator,
             'link_rows': json.dumps(link_rows or []),
             'new_linked_rows': json.dumps(new_linked_rows or [])
         }, headers=headers)
         return parse_response(response)['task']
 
+    @check_auth
     def add_workflow_task_with_existed_row(self, workflow_token, row_id, initiator=None):
         url = self._add_workflow_task_url(workflow_token)
         headers = {'Authorization': 'Token ' + self.jwt_token}
         response = requests.post(url, data={'row_id': row_id, 'initiator': initiator}, headers=headers)
         return parse_response(response)['task']
 
-
+    @check_auth
+    @api_gateway_wrapper
     def big_data_insert_rows(self, table_name, rows_data):
         url = self._dtable_db_insert_rows_url()
         json_data = {
             'table_name': table_name,
             'rows': rows_data,
         }
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
 
     ####   custom assets ######
+    @check_auth
     def get_custom_file_download_link(self, path):
         """
         :param path: str
         :return: str
         """
         url = self._app_custom_download_link_url()
         params = {'path': path}
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         return data.get('download_link')
 
+    @check_auth
     def get_custom_file_upload_link(self, path):
         url = self._app_custom_upload_link_url()
         params = {'path': path}
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
-
+    @check_auth
     def download_custom_file(self, path, save_path):
         download_link = self.get_custom_file_download_link(parse.unquote(path))
         response = requests.get(download_link, timeout=self.timeout)
         if response.status_code != 200:
             raise Exception('download file error')
         with open(save_path, 'wb') as f:
             f.write(response.content)
 
+    @check_auth
     def upload_local_file_to_custom_folder(self, local_path, custom_folder_path = None, name=None, ):
         if not name:
             name = local_path.strip('/').split('/')[-1]
         if not custom_folder_path:
             custom_folder_path = '/'
 
         upload_link_dict = self.get_custom_file_upload_link(parse.unquote(custom_folder_path))
@@ -1016,15 +1226,15 @@
             'file': (name, open(local_path, 'rb'))
         }, timeout=self.timeout)
         d = response.json()[0]
 
         file_name = d.get('name')
         return self.get_custom_file_info(custom_folder_path, file_name)
 
-
+    @check_auth
     def get_custom_file_info(self, path, name):
         url = self._app_custom_asset_file_url()
         params = {'path': path, 'name': name}
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         d = data['dirent']
@@ -1035,22 +1245,32 @@
         return {
             'type': 'file',
             'size': d.get('file_size'),
             'name': d.get('obj_name'),
             'url': 'custom-asset://%s.%s' % (asset_uuid, file_name_ext)
         }
 
+    @check_auth
     def list_custom_assets(self, path):
         url = self._app_custom_asset_dir_url()
         params = {'path': path}
         headers = parse_headers(self.token)
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
         data = parse_response(response)
         return data
 
+    @check_auth
+    def get_user_info(self, username):
+        url = self._app_user_info_url()
+        params = {'username': username}
+        headers = parse_headers(self.token)
+        response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        data = parse_response(response)
+        return data
+
 
 
 class Account(object):
     def __init__(self, login_name, password, server_url):
         self.login_name = login_name
         self.username = None
         self.password = password
```

### Comparing `seatable-api-2.6.8/seatable_api/message.py` & `seatable-api-2.7.0/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/query.py` & `seatable-api-2.7.0/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/socket_io.py` & `seatable-api-2.7.0/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.8/seatable_api/utils.py` & `seatable-api-2.7.0/seatable_api/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import json
+import re
 from datetime import datetime
 
+from seatable_api.exception import AuthExpiredError
+
 
 def _get_row(data):
     op_type = data['op_type']
     if op_type == 'insert_row':
         row = data['row_data']
     elif op_type == 'modify_row':
         row = data['updated']
@@ -180,7 +183,41 @@
                 else:
                     item[column_name] = value
             else:
                 item[column_key] = value
         converted_results.append(item)
 
     return converted_results
+
+
+def parse_headers(token):
+    return {
+        'Authorization': 'Token ' + token,
+        'Content-Type': 'application/json',
+    }
+
+
+def parse_server_url(server_url):
+    return server_url.rstrip('/')
+
+
+def parse_response(response):
+    if response.status_code >= 400:
+        try:
+            err_data = json.loads(response.text)
+        except:
+            err_data = {}
+        if err_data.get("error_msg") == "Token expired." and \
+                response.status_code == 403:
+            raise AuthExpiredError
+
+        raise ConnectionError(response.status_code, response.text)
+    else:
+        try:
+            data = json.loads(response.text)
+            return data
+        except:
+            pass
+
+
+def like_table_id(value):
+    return re.match(r'^[-0-9a-zA-Z]{4}$', value)
```

### Comparing `seatable-api-2.6.8/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.7.0/seatable_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.8
+Version: 2.7.0
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
+Description: # seatable-api-python
+        
+        Python client for SeaTable web api
+        
+        English document: <https://seatable.github.io/seatable-scripts/>
+        
+        Chinese document: <https://seatable.github.io/seatable-scripts-cn/>
+        
+        pypi: <https://pypi.org/project/seatable-api/>
+        
+        github: <https://github.com/seatable/seatable-api-python>
+        
 Platform: any
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# seatable-api-python
-
-Python client for SeaTable web api
-
-English document: <https://seatable.github.io/seatable-scripts/>
-
-Chinese document: <https://seatable.github.io/seatable-scripts-cn/>
-
-pypi: <https://pypi.org/project/seatable-api/>
-
-github: <https://github.com/seatable/seatable-api-python>
-
-
```

### Comparing `seatable-api-2.6.8/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.7.0/seatable_api.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-LICENSE
 README.md
 setup.py
 seatable_api/__init__.py
+seatable_api/api_gateway.py
 seatable_api/column.py
 seatable_api/constants.py
 seatable_api/context.py
 seatable_api/convert_airtable.py
 seatable_api/date_utils.py
 seatable_api/exception.py
 seatable_api/main.py
 seatable_api/message.py
+seatable_api/parsetab.py
 seatable_api/query.py
 seatable_api/socket_io.py
 seatable_api/utils.py
 seatable_api.egg-info/PKG-INFO
 seatable_api.egg-info/SOURCES.txt
 seatable_api.egg-info/dependency_links.txt
 seatable_api.egg-info/requires.txt
```

### Comparing `seatable-api-2.6.8/setup.py` & `seatable-api-2.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.6.8'
+__version__ = '2.7.0'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.6.8/tests/dateutils_test.py` & `seatable-api-2.7.0/tests/dateutils_test.py`

 * *Files identical despite different names*

