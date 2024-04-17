# Comparing `tmp/pih-0.36.7.tar.gz` & `tmp/pih-0.36.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.7.tar", last modified: Tue Apr 16 00:52:55 2024, max compression
+gzip compressed data, was "pih-0.36.8.tar", last modified: Wed Apr 17 06:02:47 2024, max compression
```

## Comparing `pih-0.36.7.tar` & `pih-0.36.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:55.667710 pih-0.36.7/
--rw-rw-rw-   0        0        0      249 2024-04-16 00:52:55.636440 pih-0.36.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:52.924539 pih-0.36.7/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.7/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:53.315150 pih-0.36.7/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.7/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.7/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.7/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.7/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:55.153536 pih-0.36.7/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-16 00:51:44.000000 pih-0.36.7/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.7/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.7/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.7/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.7/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.7/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30004 2024-04-15 23:46:38.000000 pih-0.36.7/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.7/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.7/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.7/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.7/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.7/pih/consts/password.py
--rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.7/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11096 2024-04-10 11:19:30.000000 pih-0.36.7/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.7/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.7/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.7/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.7/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.7/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12162 2024-04-16 00:51:35.000000 pih-0.36.7/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.7/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.7/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.7/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   549057 2024-04-15 02:02:32.000000 pih-0.36.7/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:55.376359 pih-0.36.7/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.7/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.7/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.7/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.7/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:55.518049 pih-0.36.7/pih/tools/
--rw-rw-rw-   0        0        0    51601 2024-04-11 12:03:46.000000 pih-0.36.7/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.7/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.7/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:52:55.596167 pih-0.36.7/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-16 00:52:51.000000 pih-0.36.7/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-16 00:52:51.000000 pih-0.36.7/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 00:52:51.000000 pih-0.36.7/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 00:52:51.000000 pih-0.36.7/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-16 00:52:51.000000 pih-0.36.7/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 00:52:55.683339 pih-0.36.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.363865 pih-0.36.8/
+-rw-rw-rw-   0        0        0      249 2024-04-17 06:02:47.285745 pih-0.36.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:45.126439 pih-0.36.8/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.8/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:45.472782 pih-0.36.8/pih/collections/
+-rw-rw-rw-   0        0        0    28524 2024-04-17 05:26:38.000000 pih-0.36.8/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.8/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.8/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.8/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:46.877888 pih-0.36.8/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-17 06:00:46.000000 pih-0.36.8/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.8/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.8/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.8/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.8/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.8/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30004 2024-04-15 23:46:38.000000 pih-0.36.8/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.8/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.8/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.8/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      187 2024-04-17 05:22:16.000000 pih-0.36.8/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.8/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.8/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.8/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11122 2024-04-16 01:31:15.000000 pih-0.36.8/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.8/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.8/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.8/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.8/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.36.8/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12225 2024-04-17 04:51:50.000000 pih-0.36.8/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.8/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.8/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.8/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   549799 2024-04-17 05:31:22.000000 pih-0.36.8/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.065757 pih-0.36.8/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.8/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.8/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.8/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.8/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.206371 pih-0.36.8/pih/tools/
+-rw-rw-rw-   0        0        0    51621 2024-04-16 02:10:50.000000 pih-0.36.8/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.8/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.8/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.254478 pih-0.36.8/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:02:47.363865 pih-0.36.8/setup.cfg
```

### Comparing `pih-0.36.7/pih/collections/__init__.py` & `pih-0.36.8/pih/collections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,28 @@
 class ZabbixHost:
     id: str | None = None
     name: str | None = None
     host: str | None = None
 
 
 @dataclass
+class IOTDevice:
+    name: str | None = None
+    id: str | None = None
+    key: str | None = None
+    mac: str | None = None
+    uuid: str | None = None
+    sn: str | None = None
+    category: str | None = None
+    product_name: str | None = None
+    product_id: str | None = None
+    biz_type: int | None = None
+
+
+@dataclass
 class ZabbixMetricsValue:
     value: Any | None = None
     clock: datetime | int | None = None
 
 
 @dataclass
 class ZabbixMetrics:
@@ -691,22 +705,22 @@
     name: str | None = None
     start_datetime: str | None = None
     host: str | None = None
     run_from_system_account: bool = False
     run_with_elevetion: bool = False
     live: bool = False
     exclude: bool = False
-    
+
     def clone(
         self,
         job_name: str,
         start_datetime: str | None = None,
         host: str | None = None,
         live: bool | None = None,
-        exclude: bool = False
+        exclude: bool = False,
     ):
         return RobocopyJobDescription(
             job_name,
             start_datetime,
             host or self.host,
             self.run_from_system_account,
             self.run_with_elevetion,
```

### Comparing `pih-0.36.7/pih/collections/service.py` & `pih-0.36.8/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/console_api.py` & `pih-0.36.8/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/console_api_wrapper.py` & `pih-0.36.8/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/__init__.py` & `pih-0.36.8/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.7"
+VERSION: str = "0.36.8"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36.7/pih/consts/ad.py` & `pih-0.36.8/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/addresses.py` & `pih-0.36.8/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/date_time.py` & `pih-0.36.8/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/errors.py` & `pih-0.36.8/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/events.py` & `pih-0.36.8/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/hosts.py` & `pih-0.36.8/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/names.py` & `pih-0.36.8/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/password.py` & `pih-0.36.8/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/paths.py` & `pih-0.36.8/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/polibase.py` & `pih-0.36.8/pih/consts/polibase.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,17 @@
         @staticmethod
         def get_file_name(pin: int, with_extension: bool = False) -> str:
             extension: str = (
                 j((".", POLIBASE.BARCODE.PERSON.IMAGE_FORMAT)) if with_extension else ""
             )
             return j((POLIBASE.BARCODE.NEW_PREFIX, pin, extension))
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST: list[int] = [
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST: list[int] = []
+    """
+    [
         51087,
         24727,
         8846,
         104498,
         97967,
         12411,
         40903,
@@ -220,14 +222,15 @@
         5960,
         111110,
         118252,
         120547,
         120508,
         122658,
     ]
+    """
 
     BONUS_DOCTOR_PERSON_PIN_LIST: list[int] = [
         51087,
         24727,
         8846,
         104498,
         97967,
```

### Comparing `pih-0.36.7/pih/consts/service.py` & `pih-0.36.8/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/consts/service_commands.py` & `pih-0.36.8/pih/consts/service_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     get_settings_value = auto()
     # HeatBeat
     heart_beat = auto()
     # Notifier
     register_polibase_person_information_quest = auto()
     search_polibase_person_information_quests = auto()
     update_polibase_person_information_quest = auto()
-    # Visit Cached
+    # Visit Cached (DS)
     update_polibase_person_visit_to_data_stogare = auto()
     search_polibase_person_visits_in_data_storage = auto()
     # Visit notification
     register_polibase_person_visit_notification = auto()
     search_polibase_person_visit_notifications = auto()
     # Notification confirmation
     search_polibase_person_notification_confirmation = auto()
@@ -193,14 +193,14 @@
     #
     update_person_change_date = auto()
     #
     drop_note_cache = auto()
     #
     get_bonus_list = auto()
     #
-    door_operation = auto()
+    door_command = auto()
     #
     mount_facade_for_linux_host = auto()
     #
     get_event_count = auto()
     #
     get_user_list_by_property = auto()
```

### Comparing `pih-0.36.7/pih/consts/service_roles.py` & `pih-0.36.8/pih/consts/service_roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             ServiceCommands.set_full_name_by_tab_number,
             ServiceCommands.set_telephone_by_tab_number,
             ServiceCommands.check_mark_free,
             ServiceCommands.create_mark,
             ServiceCommands.make_mark_as_free_by_tab_number,
             ServiceCommands.make_mark_as_temporary,
             ServiceCommands.remove_mark_by_tab_number,
-            ServiceCommands.door_operation,
+            ServiceCommands.door_command,
         ),
     )
 
     POLIBASE = ServiceDescription(
         name="Polibase",
         commands=(
             ServiceCommands.get_polibase_person_by_pin,
@@ -259,14 +259,18 @@
         commands=(ServiceCommands.printers_report, ServiceCommands.printer_snmp_call),
     )
     
     
     ZABBIX = ServiceDescription(
         name="Zabbix",
     )
+    
+    IOT = ServiceDescription(
+        name="iot",
+    )
 
     POLIBASE_DATABASE = ServiceDescription(
         name="PolibaseDatabase",
         commands=(ServiceCommands.create_polibase_database_backup,),
     )
 
     SSH = ServiceDescription(
```

### Comparing `pih-0.36.7/pih/consts/settings.py` & `pih-0.36.8/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/pih.py` & `pih-0.36.8/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from pih.consts import *
 from pih.collections import *
 from pih.consts.errors import *
 from pih.consts.polibase import *
 from pih.consts.python import PYTHON
 from pih.consts.events import Events
 from pih.consts.zabbix import ZABBIX
+from pih.consts.iot import IOT
 from pih.consts.settings import SETTINGS
 from pih.consts.ssh_hosts import SSHHosts
 from pih.consts.rpc import RPC as CONST_RPC
 from pih.consts.addresses import ADDRESSES, EMAIL_COLLECTION
 from pih.tools.service import ServiceRoleTool, ServiceTool, ServiceAdminTool
 from pih.consts.service import SUPPORT_NAME_PREFIX, EVENT_LISTENER_NAME_PREFIX
 
@@ -7943,14 +7944,30 @@
         @staticmethod
         def kill_process_by_port(
             value: int,
         ) -> bool | None:
             return PIH.EXECUTOR.kill_process_by_port(value)
 
     class RESULT(ResultTool):
+        
+        class IOTDevices:
+
+            @staticmethod
+            def _call(command: IOT.Commands, parameters: tuple[Any, ...] | None = None) -> bool:
+                return PIH.SERVICE.call_command_for_service(
+                    ServiceRoles.IOT,
+                    ServiceCommands.serve_command,
+                    (command.name, *(parameters or ())),
+                )
+                
+            @staticmethod
+            def devices() -> Result[list[IOTDevice]]:
+                return DataTool.to_result(
+                    PIH.RESULT.IOTDevices._call(IOT.Commands.device_list), IOTDevice
+                ) 
 
         class ZABBIX:
 
             @staticmethod
             def _call(
                 command: ZABBIX.Commands, parameters: tuple[Any, ...] | None = None
             ) -> str | None:
@@ -12911,33 +12928,34 @@
             @staticmethod
             def start_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.start_windows_service(name, computer_name)
 
             @staticmethod
             def stop_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.stop_windows_service(name, computer_name)
+            
 
         class DOOR:
 
             @staticmethod
-            def operation(name: str, operation_name: str) -> bool:
+            def _command(name: str, operation_name: str) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
-                        ServiceCommands.door_operation,
+                        ServiceCommands.door_command,
                         (name, operation_name),
                     )
                 )
 
             @staticmethod
             def open(name: str) -> bool:
-                return PIH.ACTION.DOOR.operation(name, "open")
+                return PIH.ACTION.DOOR._command(name, "open")
 
             @staticmethod
             def close(name: str) -> bool:
-                return PIH.ACTION.DOOR.operation(name, "close")
+                return PIH.ACTION.DOOR._command(name, "close")
 
         class MARK:
 
             @staticmethod
             def create(
                 full_name: FullName,
                 person_division_id: int,
@@ -13175,14 +13193,39 @@
     root = PIH()
 
     NAME = PIH.NAME
 
     IW = root.INPUT_WAIT
 
     R = root.RESULT
+    R_ME = R.MESSAGE
+    R_Z = R.ZABBIX
+    R_R = R.RESOURCES
+    R_RCG = R.RECOGNIZE
+    R_SSH = R.SSH
+    R_IND = R.INDICATIONS
+    R_N = R.NOTES
+    R_E = R.EVENTS
+    R_INV = R.INVENTORY
+    R_WS = R.WORKSTATION
+    R_COMP = R.COMPUTER
+    R_B = R.BACKUP
+    R_DS = R.DATA_STORAGE
+    R_J = R.JOURNALS
+    R_P = R.POLIBASE
+    R_M = R.MARK
+    R_U = R.USER
+    R_F = R.FILES
+    R_TT = R.TIME_TRACKING
+    R_P = R.POLIBASE
+    R_PR = R.PRINTER
+    R_SRVS = R.SERVER
+    R_EM = R.EMAIL
+    R_IOT = R.IOTDevices
+    
     D = root.DATA
     D_V = D.VARIABLE
     D_V_T = D_V.TIMESTAMP
     D_V_T_E = D_V_T.EXPIRED
     D_V_E = D_V.ENVIRONMENT
     D_TN = D.TELEPHONE_NUMBER
     D_MR = D.MATERIALIZED_RESOURCES
@@ -13202,23 +13245,14 @@
     A_QR = A.QR_CODE
     A_IND = A.INDICATION
     A_IND_CT = A_IND.CT
     A_IND_CH = A_IND.CHILLER
     ME = root.MESSAGE
     ME_P = ME.POLIBASE
     A_WS = A.WORKSTATION
-    R_ME = R.MESSAGE
-    R_Z = R.ZABBIX
-    R_R = R.RESOURCES
-    R_RCG = R.RECOGNIZE
-    R_SSH = R.SSH
-    R_IND = R.INDICATIONS
-    R_N = R.NOTES
-    R_E = R.EVENTS
-    R_INV = R.INVENTORY
     #
     A_ME = A.MESSAGE
     A_J = A.JOURNAL
     A_ACT = A.ACTIONS
     A_TT = A.TIME_TRACKING
     A_MIO = A.MOBILE_INPUT_OUTPUT
     R_ME_D = R_ME.DELAYED
@@ -13264,62 +13298,54 @@
     C_J = C.JOURNALS
     C_EML = C.EMAIL
     C_RCG = C.RECOGNIZE
     #
     A_DR = A.DOOR
     A_M = A.MARK
     A_COMP = A.COMPUTER
-    R_M = R.MARK
-    R_U = R.USER
-    R_F = R.FILES
-    R_TT = R.TIME_TRACKING
     A_U = A.USER
     C_U = C.USER
     D_F = D.FORMAT
     D_F_B = D_F.BACKUP
     D_CO = D.CONVERT
     A_P = A.POLIBASE
     A_INV = A.INVENTORY
     C_E = C.EVENTS
     C_P = C.POLIBASE
     C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
-    R_P = R.POLIBASE
-    R_PR = R.PRINTER
-    R_SRVS = R.SERVER
-    R_EM = R.EMAIL
+   
     R_IND_D = R_IND.DEVICE
     #
     A_Z = A.ZABBIX
     A_PTH = A.PATH
     A_P_V = A_P.VISIT
     A_P_V_DS = A_P_V.DATA_STORAGE
     R_P_V = R_P.VISIT
     R_P_V_DS = R_P_V.DATA_STORAGE
     A_P_N = A_P.NOTIFICATION
     A_P_N_C = A_P_N.CONFIRMATION
     R_P_N = R_P.NOTIFICATION
     R_P_N_C = R_P_N.CONFIRMATION
     C_P_N = C_P.NOTIFICATION
     C_P_N_С = C_P_N.CONFIRMATION
-    R_WS = R.WORKSTATION
-    R_COMP = R.COMPUTER
+   
     C_WS = C.WORKSTATION
     A_P_IQ = A_P.INFORMATION_QUEST
     R_P_IQ = R_P.INFORMATION_QUEST
     SRV = root.SERVICE
     SRV_A = SRV.ADMIN
     I = root.input
     I_U = I.user
     A_B = A.BACKUP
-    R_B = R.BACKUP
+
     O = root.output
     SE = root.session
     A_DS = A.DATA_STORAGE
-    R_DS = R.DATA_STORAGE
+    
     V = root.VERSION
     SYS = root.SYS
     U = root.UPDATER
     EXC = root.EXECUTOR
     ER = root.ERROR
     E = root.EVENT
     E_B = E.BUILDER
@@ -13332,15 +13358,15 @@
     PTH_QR = PTH.QR_CODE
     PTH_FNT = PTH.FONTS
     PTH_IND = PTH.INDICATIONS
     PTH_MIO = PTH.MOBILE_HELPER
     PTH_FCD = PTH.FACADE
     PTH_FCD_DIST = PTH_FCD.DITRIBUTIVE
     L = root.LOG
-    R_J = R.JOURNALS
+ 
 
     CT = CONST
     CT_FACADE = FACADE
     CT_PY = PYTHON
     CT_PORT = CONST.PORT
     CT_CMDT = CommandTypes
     CT_LNK = LINK
@@ -13391,15 +13417,15 @@
     CT_I = INDICATIONS
     CT_T = Tags
     CT_CR = CT.CARD_REGISTRY
     C_P_DB = C_P.DATABASE
     CT_PI = PARAM_ITEMS
 
     D_P = D.POLIBASE
-    R_P = R.POLIBASE
+  
 
     CR = root.CARD_REGISTRY
     #
 
     C_V_T_E = D_C.VARIABLE.TIMESTAMP.EXPIRED
```

### Comparing `pih-0.36.7/pih/rpc/__init__.py` & `pih-0.36.8/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.8/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.8/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/tools/__init__.py` & `pih-0.36.8/pih/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1255,22 +1255,22 @@
     def now_time(delta_minutes: int = 0) -> datetime:
         return datetime.combine(date.today(), datetime.now().time()) + timedelta(
             minutes=delta_minutes
         )
 
     @staticmethod
     def datetime_from_string(
-        value: str | None, format: str | None = None
+        value: datetime | None, format: str | None = None
     ) -> datetime | None:
         if e(value):
             return None
         return DataTool.check_not_none(
             format,
-            lambda: datetime.strptime(value, format),
-            lambda: datetime.fromisoformat(value),
+            lambda: datetime.strptime(nnt(value), nnt(format)),
+            lambda: datetime.fromisoformat(nnt(value)),
         )
 
     @staticmethod
     def datetime_or_date_from_string(
         value: str | None, format: str | None = None, as_date: bool = False
     ) -> datetime | date | None:
         if e(value):
```

### Comparing `pih-0.36.7/pih/tools/service.py` & `pih-0.36.8/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih/widgets.py` & `pih-0.36.8/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.7/pih.egg-info/SOURCES.txt` & `pih-0.36.8/pih.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pih/consts/date_time.py
 pih/consts/document.py
 pih/consts/errors.py
 pih/consts/events.py
 pih/consts/facade.py
 pih/consts/file.py
 pih/consts/hosts.py
+pih/consts/iot.py
 pih/consts/names.py
 pih/consts/password.py
 pih/consts/paths.py
 pih/consts/polibase.py
 pih/consts/python.py
 pih/consts/recognize.py
 pih/consts/rpc.py
```

