# Comparing `tmp/iboxstacksops-0.8.0.tar.gz` & `tmp/iboxstacksops-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.8.0.tar", last modified: Wed Jun  7 11:25:09 2023, max compression
+gzip compressed data, was "iboxstacksops-0.8.1.tar", last modified: Wed Apr 17 08:34:37 2024, max compression
```

## Comparing `iboxstacksops-0.8.0.tar` & `iboxstacksops-0.8.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.8.0/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.936640 iboxstacksops-0.8.0/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.936640 iboxstacksops-0.8.0/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.944640 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.8.0/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.8.0/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.8.0/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4096 2023-05-18 19:50:43.000000 iboxstacksops-0.8.0/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5507 2023-05-19 17:15:37.000000 iboxstacksops-0.8.0/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4204 2023-05-18 19:47:19.000000 iboxstacksops-0.8.0/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.8.0/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.8.0/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.8.0/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.8.0/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6390 2023-05-18 19:46:59.000000 iboxstacksops-0.8.0/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.8.0/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1354 2023-05-18 19:52:27.000000 iboxstacksops-0.8.0/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8720 2023-05-18 19:52:16.000000 iboxstacksops-0.8.0/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17398 2023-06-07 11:12:24.000000 iboxstacksops-0.8.0/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.8.0/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10015 2023-06-06 21:51:44.000000 iboxstacksops-0.8.0/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.8.0/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.8.0/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.8.0/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.8.0/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1563 2023-06-07 11:11:32.000000 iboxstacksops-0.8.0/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.8.0/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.8.0/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.8.0/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.8.0/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-06-07 11:22:43.000000 iboxstacksops-0.8.0/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.122450 iboxstacksops-0.8.1/
+-rw-r--r--   0 mello     (1000) mello     (1000)    10297 2020-02-20 18:59:20.000000 iboxstacksops-0.8.1/LICENSE
+-rw-r--r--   0 mello     (1000) mello     (1000)      854 2024-04-17 08:34:37.122450 iboxstacksops-0.8.1/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.8.1/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.086449 iboxstacksops-0.8.1/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.086449 iboxstacksops-0.8.1/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.098450 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      854 2024-04-17 08:34:36.000000 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      917 2024-04-17 08:34:36.000000 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2024-04-17 08:34:36.000000 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2024-04-17 08:34:36.000000 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2024-04-17 08:34:36.000000 iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.122450 iboxstacksops-0.8.1/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.8.1/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.8.1/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.8.1/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4098 2024-04-17 08:20:41.000000 iboxstacksops-0.8.1/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5598 2024-04-17 08:21:51.000000 iboxstacksops-0.8.1/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4205 2023-06-07 16:27:05.000000 iboxstacksops-0.8.1/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.8.1/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36093 2024-02-05 11:01:26.000000 iboxstacksops-0.8.1/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.8.1/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.8.1/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6420 2023-08-23 09:27:09.000000 iboxstacksops-0.8.1/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.8.1/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1354 2023-05-18 19:52:27.000000 iboxstacksops-0.8.1/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8720 2023-08-02 08:32:12.000000 iboxstacksops-0.8.1/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17556 2024-04-17 08:16:06.000000 iboxstacksops-0.8.1/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.8.1/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10185 2023-06-07 16:21:08.000000 iboxstacksops-0.8.1/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2754 2023-11-06 16:15:41.000000 iboxstacksops-0.8.1/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5237 2024-02-23 14:42:31.000000 iboxstacksops-0.8.1/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.8.1/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.8.1/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1582 2024-02-22 09:09:17.000000 iboxstacksops-0.8.1/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4052 2023-11-06 15:36:35.000000 iboxstacksops-0.8.1/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.8.1/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.8.1/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 08:34:37.122450 iboxstacksops-0.8.1/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.8.1/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2024-04-17 08:34:37.122450 iboxstacksops-0.8.1/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2024-04-17 08:31:35.000000 iboxstacksops-0.8.1/setup.py
```

### Comparing `iboxstacksops-0.8.0/PKG-INFO` & `iboxstacksops-0.8.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.8.0
+Version: 0.8.1
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
-Description: # AwsIBoxStackOps
-        Aws Infrastucture in a Box - Stacks management program.
-        
-        Used to create and update an AWS CloudFormation stack in a simple way.
-        
-        ## Installation ##
-        `pip install iboxstacksops`
-        
-        ## License ##
-        
-        This software is distributed under the terms of the MIT [license](LICENSE).
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: extra
+License-File: LICENSE
+
+# AwsIBoxStackOps
+Aws Infrastucture in a Box - Stacks management program.
+
+Used to create and update an AWS CloudFormation stack in a simple way.
+
+## Installation ##
+`pip install iboxstacksops`
+
+## License ##
+
+This software is distributed under the terms of the MIT [license](LICENSE).
```

### Comparing `iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.8.0
+Version: 0.8.1
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
-Description: # AwsIBoxStackOps
-        Aws Infrastucture in a Box - Stacks management program.
-        
-        Used to create and update an AWS CloudFormation stack in a simple way.
-        
-        ## Installation ##
-        `pip install iboxstacksops`
-        
-        ## License ##
-        
-        This software is distributed under the terms of the MIT [license](LICENSE).
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: extra
+License-File: LICENSE
+
+# AwsIBoxStackOps
+Aws Infrastucture in a Box - Stacks management program.
+
+Used to create and update an AWS CloudFormation stack in a simple way.
+
+## Installation ##
+`pip install iboxstacksops`
+
+## License ##
+
+This software is distributed under the terms of the MIT [license](LICENSE).
```

### Comparing `iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.8.1/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 ./build/lib/iboxstacksops.egg-info/PKG-INFO
 ./build/lib/iboxstacksops.egg-info/SOURCES.txt
 ./build/lib/iboxstacksops.egg-info/dependency_links.txt
 ./build/lib/iboxstacksops.egg-info/requires.txt
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/actions.py` & `iboxstacksops-0.8.1/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/aws.py` & `iboxstacksops-0.8.1/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/cfg.py` & `iboxstacksops-0.8.1/iboxstacksops/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 statistic = "Average"
 statisticresponse = "p95"
 silent = True
 vertical = False
 profile = False
 output = "text"
 disable_rollback = False
-changeset_original = False
+# changeset_original = False
 print_mylog = True
 #
 
 OUT_WIDTH = 1000000
 
 SLACK_CHANNEL = "_cf_deploy"
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/changeset.py` & `iboxstacksops-0.8.1/iboxstacksops/changeset.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 
 # wait until changeset is created
 def _changeset_waiter(istack, changeset_id):
     while True:
         time.sleep(3)
         changeset = istack.client.describe_change_set(
-            ChangeSetName=changeset_id, StackName=istack.name
+            ChangeSetName=changeset_id,
+            StackName=istack.name,
+            IncludePropertyValues=True,
         )
         if changeset["Status"] in istack.cfg.CHANGESET_COMPLETE_STATUS:
             return changeset
 
 
 # parse changeset changes
 def _parse_changeset(changeset):
@@ -145,17 +147,17 @@
     # -wait changeset creation and return it
     changeset = _changeset_waiter(istack, changeset_id)
     # pprint(changeset)
 
     # -parse changeset changes
     changeset_changes, not_replaced = _parse_changeset(changeset)
 
-    # simplify changeset
-    if not istack.cfg.changeset_original:
-        changeset_changes = _simplify_changeset(changeset_changes, not_replaced)
+    # simplify changeset - replaced by IncludePropertyValues
+#    if not istack.cfg.changeset_original:
+#        changeset_changes = _simplify_changeset(changeset_changes, not_replaced)
 
     # -show changeset changes
     _show_changeset_changes(istack, changeset_changes)
 
     # -delete changeset
     _delete_changeset(istack, changeset_id)
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/commands.py` & `iboxstacksops-0.8.1/iboxstacksops/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     if not cfg.compact:
         cfg.OUT_WIDTH = 80
     w_stacks = stacks.get()
     result = concurrent_exec("info", w_stacks, i_stack)
 
     return result
 
+
 def show_resources():
     w_stacks = stacks.get()
     result = concurrent_exec("show_resources", w_stacks, i_stack)
 
 
 def log():
     name = cfg.stack[0]
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/common.py` & `iboxstacksops-0.8.1/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/dashboard.py` & `iboxstacksops-0.8.1/iboxstacksops/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
             AutoScalingGroupName=res[AutoScalingGroupName],
             PolicyNames=[polname],
         )
 
         return response["ScalingPolicies"][0]["TargetTrackingConfiguration"]
 
     def get_policy_ecs(res):
+        if "ScalingPolicyTrackingsApp" not in res:
+            return {}
         resname = "/".join(res["ScalingPolicyTrackingsApp"].split("/")[2:5]).split(":")[
             0
         ]
         client = istack.boto3.client("application-autoscaling")
         response = client.describe_scaling_policies(
             PolicyNames=list(istack.cfg.SCALING_POLICY_TRACKINGS_NAMES.keys()),
             ResourceId=resname,
@@ -87,15 +89,15 @@
                 color = "#1f77b4"
             if n == "ServiceName":
                 conf = get_policy_ecs(res)
                 l_type = "ECS"
                 color = "#36dc52"
 
             stat = "Average"
-            value = conf["TargetValue"]
+            value = conf.get("TargetValue", 0)
             if (
                 "CustomizedMetricSpecification" in conf
                 and "Statistic" in conf["CustomizedMetricSpecification"]
             ):
                 stat = conf["CustomizedMetricSpecification"]["Statistic"]
 
             ret.append(
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/events.py` & `iboxstacksops-0.8.1/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/i_region.py` & `iboxstacksops-0.8.1/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/i_stack.py` & `iboxstacksops-0.8.1/iboxstacksops/i_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 
     def stackset_update(self):
         cfg.fields = cfg.STACKSET_INSTANCES_SHOW_TABLE_FIELDS
         self.exports = self.cfg.exports
         self.template = template.get_template(self, stackset=True)
         self.stack = True
         parameters.process(self)
+        resolve.process(self)
         result = actions.stackset_update(self)
         if result:
             return {self.name: None}
 
     def stackset_info(self):
         self.exports = self.cfg.exports
         self.template = template.get_template(self, stackset=True)
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/msg.py` & `iboxstacksops-0.8.1/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/outputs.py` & `iboxstacksops-0.8.1/iboxstacksops/outputs.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/parameters.py` & `iboxstacksops-0.8.1/iboxstacksops/parameters.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/parser.py` & `iboxstacksops-0.8.1/iboxstacksops/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
             "Modify,Replace",
             "Delete,Replace",
         ],
     )
     parser.add_argument(
         "-n", "--nochangeset", help="No ChangeSet", required=False, action="store_true"
     )
-    parser.add_argument(
-        "-C",
-        "--changeset-original",
-        help="Do not simply ChangeSet",
-        required=False,
-        action="store_true",
-    )
+#    parser.add_argument(
+#        "-C",
+#        "--changeset-original",
+#        help="Do not simply ChangeSet",
+#        required=False,
+#        action="store_true",
+#    )
     parser.add_argument("--dryrun", help="Show changeset and exit", action="store_true")
     parser.add_argument(
         "-T", "--showtags", help="Show tags changes in changeset", action="store_true"
     )
     parser.add_argument(
         "-D",
         "--dashboard",
@@ -110,15 +110,19 @@
     )
 
 
 def get_show_parser(subparser, parents=[]):
     parser = subparser.add_parser("show", parents=parents, help="Show Stacks table")
 
     parser.add_argument(
-        "-F", "--fields", nargs="+", type=str, default=cfg.SHOW_TABLE_FIELDS,
+        "-F",
+        "--fields",
+        nargs="+",
+        type=str,
+        default=cfg.SHOW_TABLE_FIELDS,
         help="Can use syntax 'Name=DisplayName' to use custom table heading",
     )
     parser.add_argument(
         "-O", "--output", type=str, default="text", choices=["text", "html", "bare"]
     )
 
     return parser
@@ -276,14 +280,17 @@
         parents=parents,
         help="Create RecordSet Aliases looking at stack R53 resources",
     )
     parser.set_defaults(func=r53)
 
     parser.add_argument("--dryrun", help="Show changes and exit", action="store_true")
     parser.add_argument(
+        "--safe", help="Create only internal and regional records", action="store_true"
+    )
+    parser.add_argument(
         "--noorigin", help="Do not create Origin Record", action="store_true"
     )
     parser.add_argument(
         "--suffix",
         help='Suffix to add to RecordSet Name, prepended with "-"',
         default="",
         type=str,
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/replica.py` & `iboxstacksops-0.8.1/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/resolve.py` & `iboxstacksops-0.8.1/iboxstacksops/resolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,16 +242,22 @@
                     pass
                 istack.t_resources[v["Type"]] = r
                 istack.r_resources[r] = _recursive_resolve(r, v)
 
                 if v["Type"] == "AWS::Lambda::Function":
                     _check_lambda(r)
 
+    def _process_metadata():
+        istack.metadata = _recursive_resolve(
+            "Metadata", istack.template.get("Metadata", {})
+        )
+
     _process_conditions()
     _process_resources()
+    _process_metadata()
 
 
 def _check_s3_files(istack):
     for f in istack.s3_files:
         bucket = f[0]
         key = f[1]
         try:
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/resources.py` & `iboxstacksops-0.8.1/iboxstacksops/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 if res_lid in [
                     "ListenerHttpsExternalRules1",
                     "ListenerHttpsExternalRules2",
                     "ListenerHttpExternalRules1",
                     "ListenerHttpInternalRules1",
                 ]:
                     res_pid = "/".join(res_pid.split("/")[1:4])
-                if res_lid in ["Service", "ServiceSpot"]:
+                if res_lid in ["Service", "ServiceSpot"] and res_pid != "null":
                     res_pid_arr = res_pid.split("/")
                     if len(res_pid_arr) == 3:
                         res_pid = res_pid_arr[2]
                     else:
                         res_pid = res_pid_arr[1]
                 if res_lid in [
                     "LoadBalancerApplicationExternal",
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/route53.py` & `iboxstacksops-0.8.1/iboxstacksops/route53.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,28 +99,28 @@
             )
             record_origin = "%s.origin.%s" % (record["role"], record["domain"])
             record_cf = "%s.%s" % (record["role"], record["domain"])
             map_record = {
                 record_region: v,
             }
 
-            if "RecordSetCloudFront" not in res:
+            if "RecordSetCloudFront" not in res and not istack.cfg.safe:
                 map_record[record_cf] = record_region
 
-            if not istack.cfg.noorigin:
+            if not istack.cfg.noorigin and not istack.cfg.safe:
                 map_record[record_origin] = record_region
 
         if r.startswith("RecordSetInternal"):
             record = _get_rec_info(v, "internal")
             record_internal = record["role"] + "." + record["domain"]
             map_record = {
                 record_internal: v,
             }
 
-        if r == "RecordSetCloudFront":
+        if r == "RecordSetCloudFront" and not istack.cfg.safe:
             record = _get_rec_info(v, "cf")
             record_cf = record["role"] + "." + record["domain"]
             map_record = {
                 record_cf: v,
             }
 
         if r.startswith("ServiceDiscoveryService"):
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/ssm.py` & `iboxstacksops-0.8.1/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/stacks.py` & `iboxstacksops-0.8.1/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/table.py` & `iboxstacksops-0.8.1/iboxstacksops/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                 else f"{n[i]} *"
                 if i in parameter_not_empty
                 else n[i]
                 for i in table_data
             ]
         )
 
-    table.sortby = fields[0]
+    if fields:
+        table.sortby = fields[0]
     table.reversesort = True
     table.align = "l"
 
     if cfg.output == "html":
         table.format = True
 
         return table.get_html_string(fields=fields)
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/tags.py` & `iboxstacksops-0.8.1/iboxstacksops/tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     tags_remove = {}
 
     # unchanged tags
     tags_default = {}
 
     # changed tags - same value as corresponding stack param
     tags_changed = {}
+
+    # metadata tags - found inside template Metadata Section
+    tags_metadata = {}
+
     final_tags = []
 
     for tag in stack_tags:
         key = tag["Key"]
         current_value = tag["Value"]
 
         # Skip LastUpdate and EnvApp1Version Tag
@@ -51,37 +55,67 @@
             if len(value) == 0:
                 value = "empty"
 
             tags_default[key] = value
 
         final_tags.append({"Key": key, "Value": value})
 
-    # Add cmd tags that do not have as Value REMOVE
-    for key, value in cmd_tags.items():
-        if value != "REMOVE":
-            final_tags.append({"Key": key, "Value": value})
-            tags_cmd[key] = value
+    final_tags_keys = [n["Key"] for n in final_tags]
+
+    upsert_tags_cfg = [
+        # Command line tags
+        (cmd_tags, tags_cmd),
+        # Metadata tags found inside template Metadata Section
+        (istack.template.get("Metadata", {}).get("Tags", {}), tags_metadata),
+    ]
+
+    # Add or Update Tags
+    for n in upsert_tags_cfg:
+        for key, value in n[0].items():
+            if key not in tags_remove:
+                # Tag must not be removed
+                tag = {"Key": key, "Value": value}
+                if tag in final_tags:
+                    # Tag already exist, skip it
+                    pass
+                elif key in final_tags_keys:
+                    # Tag Key already exist but with different Value, update it
+                    loc = final_tags_keys.index(key)
+                    tags_changed[key] = "%s => %s" % (
+                        final_tags[loc]["Value"],
+                        value,
+                    )
+                    final_tags[loc] = tag
+                    tags_default.pop(key, None)
+                else:
+                    # Tag Key do not exist, add/append it
+                    final_tags.append(tag)
+                    n[1][key] = value
 
     # Add LastUpdate Tag with current time
     # Currently disabled:
     # Some resource, like CloudFormation Distribution, take time to be updated.
     # Does it make sense to have a tag with LastUpdateTime even if resource properties are not changed at all ?
     # If a resource is created by CloudFormation i can simply look at Stack LastUpdateTime
     # to have the same information derived by tagging it (i know that with tagging is simpler to do this).
     # final_tags.append({"Key": "LastUpdate", "Value": str(datetime.now())})
 
     if tags_default:
         istack.mylog(
-            "DEFAULT - STACK TAGS\n%s\n" % pformat(tags_default, width=1000000)
+            "CURRENT - STACK TAGS\n%s\n" % pformat(tags_default, width=1000000)
         )
     if tags_changed:
         istack.mylog(
             "CHANGED - STACK TAGS\n%s\n" % pformat(tags_changed, width=1000000)
         )
     if tags_cmd:
         istack.mylog(
             "COMMAND LINE - STACK TAGS\n%s\n" % pformat(tags_cmd, width=1000000)
         )
+    if tags_metadata:
+        istack.mylog(
+            "METADATA - STACK TAGS\n%s\n" % pformat(tags_metadata, width=1000000)
+        )
     if tags_remove:
         istack.mylog("REMOVE - STACK TAGS\n%s\n" % pformat(tags_remove, width=1000000))
 
     return final_tags
```

### Comparing `iboxstacksops-0.8.0/iboxstacksops/template.py` & `iboxstacksops-0.8.1/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/iboxstacksops/tools.py` & `iboxstacksops-0.8.1/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.8.0/setup.py` & `iboxstacksops-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.8.0",
+    version="0.8.1",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

