# Comparing `tmp/splunktalib-3.0.4.tar.gz` & `tmp/splunktalib-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunktalib-3.0.4.tar", max compression
+gzip compressed data, was "splunktalib-3.0.5.tar", max compression
```

## Comparing `splunktalib-3.0.4.tar` & `splunktalib-3.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11342 2023-05-26 12:30:49.211469 splunktalib-3.0.4/LICENSE
--rw-r--r--   0        0        0     1104 2023-05-26 12:31:21.624237 splunktalib-3.0.4/pyproject.toml
--rw-r--r--   0        0        0      598 2023-05-26 12:31:21.620237 splunktalib-3.0.4/splunktalib/__init__.py
--rw-r--r--   0        0        0      575 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/__init__.py
--rw-r--r--   0        0        0      594 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/consts.py
--rw-r--r--   0        0        0     4951 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/log.py
--rw-r--r--   0        0        0     1599 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/pattern.py
--rw-r--r--   0        0        0     3922 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/util.py
--rw-r--r--   0        0        0     2251 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/common/xml_dom_parser.py
--rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/__init__.py
--rw-r--r--   0        0        0     3497 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/concurrent_executor.py
--rw-r--r--   0        0        0     2247 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/process_pool.py
--rw-r--r--   0        0        0    10691 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/thread_pool.py
--rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/__init__.py
--rw-r--r--   0        0        0     6088 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/conf_endpoints.py
--rw-r--r--   0        0        0     9206 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/conf_manager.py
--rw-r--r--   0        0        0     7195 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/data_input_endpoints.py
--rw-r--r--   0        0        0     3467 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/property_endpoints.py
--rw-r--r--   0        0        0     1796 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/request.py
--rw-r--r--   0        0        0     6892 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/ta_conf_manager.py
--rw-r--r--   0        0        0    12871 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/credentials.py
--rw-r--r--   0        0        0     5830 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/event_writer.py
--rw-r--r--   0        0        0     2358 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/file_monitor.py
--rw-r--r--   0        0        0     7444 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/kv_client.py
--rw-r--r--   0        0        0     5207 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/modinput.py
--rw-r--r--   0        0        0     2586 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/orphan_process_monitor.py
--rw-r--r--   0        0        0     3001 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/rest.py
--rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/job.py
--rw-r--r--   0        0        0     4637 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/scheduler.py
--rw-r--r--   0        0        0      667 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/setting.conf
--rw-r--r--   0        0        0     2336 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/splunk_cluster.py
--rw-r--r--   0        0        0     1906 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/splunk_platform.py
--rw-r--r--   0        0        0     9147 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/state_store.py
--rw-r--r--   0        0        0     2617 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/timer.py
--rw-r--r--   0        0        0     4779 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/timer_queue.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 splunktalib-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-04-17 14:19:14.491882 splunktalib-3.0.5/LICENSE
+-rw-r--r--   0        0        0     1104 2024-04-17 14:19:47.727918 splunktalib-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0      598 2024-04-17 14:19:47.723919 splunktalib-3.0.5/splunktalib/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/consts.py
+-rw-r--r--   0        0        0     4951 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/log.py
+-rw-r--r--   0        0        0     1599 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/pattern.py
+-rw-r--r--   0        0        0     3922 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/util.py
+-rw-r--r--   0        0        0     2251 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/common/xml_dom_parser.py
+-rw-r--r--   0        0        0      575 2024-04-17 14:19:14.491882 splunktalib-3.0.5/splunktalib/concurrent/__init__.py
+-rw-r--r--   0        0        0     3497 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/concurrent/concurrent_executor.py
+-rw-r--r--   0        0        0     2247 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/concurrent/process_pool.py
+-rw-r--r--   0        0        0    10691 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/concurrent/thread_pool.py
+-rw-r--r--   0        0        0      575 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/__init__.py
+-rw-r--r--   0        0        0     6088 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/conf_endpoints.py
+-rw-r--r--   0        0        0     9206 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/conf_manager.py
+-rw-r--r--   0        0        0     7195 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/data_input_endpoints.py
+-rw-r--r--   0        0        0     3467 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/property_endpoints.py
+-rw-r--r--   0        0        0     1796 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/request.py
+-rw-r--r--   0        0        0     6892 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/conf_manager/ta_conf_manager.py
+-rw-r--r--   0        0        0    12871 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/credentials.py
+-rw-r--r--   0        0        0     5830 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/event_writer.py
+-rw-r--r--   0        0        0     2358 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/file_monitor.py
+-rw-r--r--   0        0        0     7444 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/kv_client.py
+-rw-r--r--   0        0        0     5207 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/modinput.py
+-rw-r--r--   0        0        0     2586 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/orphan_process_monitor.py
+-rw-r--r--   0        0        0     3001 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/rest.py
+-rw-r--r--   0        0        0      575 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/schedule/__init__.py
+-rw-r--r--   0        0        0     3065 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/schedule/job.py
+-rw-r--r--   0        0        0     4637 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/schedule/scheduler.py
+-rw-r--r--   0        0        0      667 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/setting.conf
+-rw-r--r--   0        0        0     2336 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/splunk_cluster.py
+-rw-r--r--   0        0        0     1906 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/splunk_platform.py
+-rw-r--r--   0        0        0     9147 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/state_store.py
+-rw-r--r--   0        0        0     2617 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/timer.py
+-rw-r--r--   0        0        0     4779 2024-04-17 14:19:14.495882 splunktalib-3.0.5/splunktalib/timer_queue.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 splunktalib-3.0.5/PKG-INFO
```

### Comparing `splunktalib-3.0.4/LICENSE` & `splunktalib-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/pyproject.toml` & `splunktalib-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "splunktalib"
-version = "3.0.4"
+version = "3.0.5"
 description = "Supporting library for Splunk Add-ons"
 authors = ["rfaircloth-splunk <rfaircloth@splunk.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/splunk/addonfactory-ta-library-python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `splunktalib-3.0.4/splunktalib/__init__.py` & `splunktalib-3.0.5/splunktalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "3.0.4"
+__version__ = "3.0.5"
```

### Comparing `splunktalib-3.0.4/splunktalib/common/__init__.py` & `splunktalib-3.0.5/splunktalib/common/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/common/consts.py` & `splunktalib-3.0.5/splunktalib/common/consts.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/common/log.py` & `splunktalib-3.0.5/splunktalib/common/log.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/common/pattern.py` & `splunktalib-3.0.5/splunktalib/common/pattern.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/common/util.py` & `splunktalib-3.0.5/splunktalib/common/util.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/common/xml_dom_parser.py` & `splunktalib-3.0.5/splunktalib/common/xml_dom_parser.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/concurrent/__init__.py` & `splunktalib-3.0.5/splunktalib/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/concurrent/concurrent_executor.py` & `splunktalib-3.0.5/splunktalib/concurrent/concurrent_executor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/concurrent/process_pool.py` & `splunktalib-3.0.5/splunktalib/concurrent/process_pool.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/concurrent/thread_pool.py` & `splunktalib-3.0.5/splunktalib/concurrent/thread_pool.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/__init__.py` & `splunktalib-3.0.5/splunktalib/conf_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/conf_endpoints.py` & `splunktalib-3.0.5/splunktalib/conf_manager/conf_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/conf_manager.py` & `splunktalib-3.0.5/splunktalib/conf_manager/conf_manager.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/data_input_endpoints.py` & `splunktalib-3.0.5/splunktalib/conf_manager/data_input_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/property_endpoints.py` & `splunktalib-3.0.5/splunktalib/conf_manager/property_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/request.py` & `splunktalib-3.0.5/splunktalib/conf_manager/request.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/conf_manager/ta_conf_manager.py` & `splunktalib-3.0.5/splunktalib/conf_manager/ta_conf_manager.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/credentials.py` & `splunktalib-3.0.5/splunktalib/credentials.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/event_writer.py` & `splunktalib-3.0.5/splunktalib/event_writer.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/file_monitor.py` & `splunktalib-3.0.5/splunktalib/file_monitor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/kv_client.py` & `splunktalib-3.0.5/splunktalib/kv_client.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/modinput.py` & `splunktalib-3.0.5/splunktalib/modinput.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/orphan_process_monitor.py` & `splunktalib-3.0.5/splunktalib/orphan_process_monitor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/rest.py` & `splunktalib-3.0.5/splunktalib/rest.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/schedule/__init__.py` & `splunktalib-3.0.5/splunktalib/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/schedule/job.py` & `splunktalib-3.0.5/splunktalib/schedule/job.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/schedule/scheduler.py` & `splunktalib-3.0.5/splunktalib/schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/setting.conf` & `splunktalib-3.0.5/splunktalib/setting.conf`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/splunk_cluster.py` & `splunktalib-3.0.5/splunktalib/splunk_cluster.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/splunk_platform.py` & `splunktalib-3.0.5/splunktalib/splunk_platform.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/state_store.py` & `splunktalib-3.0.5/splunktalib/state_store.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/timer.py` & `splunktalib-3.0.5/splunktalib/timer.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/splunktalib/timer_queue.py` & `splunktalib-3.0.5/splunktalib/timer_queue.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.4/PKG-INFO` & `splunktalib-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splunktalib
-Version: 3.0.4
+Version: 3.0.5
 Summary: Supporting library for Splunk Add-ons
 Home-page: https://github.com/splunk/addonfactory-ta-library-python
 License: Apache-2.0
 Author: rfaircloth-splunk
 Author-email: rfaircloth@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

