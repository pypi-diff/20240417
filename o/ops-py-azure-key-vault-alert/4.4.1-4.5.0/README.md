# Comparing `tmp/ops-py-azure-key-vault-alert-4.4.1.tar.gz` & `tmp/ops_py_azure_key_vault_alert-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-alert-4.4.1.tar", last modified: Fri Apr 12 13:18:11 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_alert-4.5.0.tar", last modified: Wed Apr 17 08:15:32 2024, max compression
```

## Comparing `ops-py-azure-key-vault-alert-4.4.1.tar` & `ops_py_azure_key_vault_alert-4.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:18:11.266547 ops-py-azure-key-vault-alert-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 13:18:09.000000 ops-py-azure-key-vault-alert-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-12 13:18:11.266547 ops-py-azure-key-vault-alert-4.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:18:11.262547 ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-12 13:18:06.000000 ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7121 2024-04-12 13:18:06.000000 ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7486 2024-04-12 13:18:06.000000 ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/slack_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-12 13:18:06.000000 ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:18:11.266547 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-12 13:18:11.000000 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-12 13:18:11.000000 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:18:11.000000 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 13:18:11.000000 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 13:18:11.000000 ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-12 13:18:09.000000 ops-py-azure-key-vault-alert-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-12 13:18:09.000000 ops-py-azure-key-vault-alert-4.4.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 13:18:06.000000 ops-py-azure-key-vault-alert-4.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:18:11.266547 ops-py-azure-key-vault-alert-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 13:18:09.000000 ops-py-azure-key-vault-alert-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:32.917765 ops_py_azure_key_vault_alert-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 08:15:30.000000 ops_py_azure_key_vault_alert-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-17 08:15:32.917765 ops_py_azure_key_vault_alert-4.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:32.917765 ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-17 08:15:26.000000 ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8621 2024-04-17 08:15:26.000000 ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1648 2024-04-17 08:15:26.000000 ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/slack_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-17 08:15:26.000000 ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:32.917765 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-17 08:15:32.000000 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 08:15:32.000000 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:15:32.000000 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 08:15:32.000000 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 08:15:32.000000 ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 08:15:30.000000 ops_py_azure_key_vault_alert-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 08:15:30.000000 ops_py_azure_key_vault_alert-4.5.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 08:15:26.000000 ops_py_azure_key_vault_alert-4.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:15:32.917765 ops_py_azure_key_vault_alert-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 08:15:30.000000 ops_py_azure_key_vault_alert-4.5.0/setup.py
```

### Comparing `ops-py-azure-key-vault-alert-4.4.1/LICENSE` & `ops_py_azure_key_vault_alert-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.4.1/PKG-INFO` & `ops_py_azure_key_vault_alert-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.4.1
+Version: 4.5.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==4.0.1
+Requires-Dist: ops-py-azure-key-vault-report==5.0.2
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
```

### Comparing `ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/azure_key_vault_alert.py` & `ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,28 +3,33 @@
 import os
 import logging
 import argparse
 import json
 from azure_key_vault_report import azure_key_vault_report
 from azure_key_vault_report import az_cmd
 from message_handler import message_handler
-from .slack_alert import slack_alert
+from .slack_post import slack_post
 from .teams_alert import teams_alert
 
 ########################################################################################################################
 
 
 def main():
     logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
 
     # The list of key vaults to check passed as command line arguments
     parser = argparse.ArgumentParser()
     parser.add_argument("-v", "--vaults", nargs='+',
                         help="List of key vaults to check. E.g. kv-dev kv-test")
 
+    parser.add_argument("-c", "--critical_threshold", type=int,
+                        help="If set then only records that are +/- this value in days till expire/expired "
+                             "will be alerted. Records will be alerted as individual Slack messages. "
+                             "Summary report and other reports will not be posted.")
+
     parser.add_argument("-e", "--expire_threshold", type=int,
                         help="If a value (int) is set. The days to the record's Expiration Date must be above "
                              "this threshold (Default: not set)")
 
     parser.add_argument("-a", "--include_all", action='store_true',
                         help="Include all records in output (verbose) if provided.")
 
@@ -51,14 +56,15 @@
 
     parser.add_argument("-w", "--workflow_output_file", type=str, default="output.json",
                         help="The file where the full json report will be written.")
 
     args = parser.parse_args()
     vaults = args.vaults
     expire_threshold = args.expire_threshold
+    critical_threshold = args.critical_threshold
     include_all = args.include_all
     ignore_no_expiration = args.include_no_expiration
     title = args.title
     record_types = args.record_types
     slack_split_chars = args.slack_split_chars
     teams_max_chars = args.teams_max_chars
     stdout_only = args.stdout_only
@@ -76,14 +82,15 @@
         vaults = [vaults]
 
     # The different kind of alert outputs are initially set to False.
     # Will be updated according to value of WEBHOOK_REPORT
     slack_app = False
     teams_output = False
     msg_handler = None
+    success = False
 
     if not WEBHOOK_REPORT:
         logging.warning("'WEBHOOK_REPORT' not provided. Report will not be posted to message handler.")
     else:
         if "slack.com/services" in WEBHOOK_REPORT:
             logging.info("Slack services webhook detected.")
             slack_app = True
@@ -100,32 +107,16 @@
     # If argument 'include_no_expiration' is not provided, then the variable 'ignore_no_expiration' is then set to True
     kv_report = azure_key_vault_report.AzureKeyVaultReport(az_results)
     kv_report.parse_results()
     kv_report.add_summary()
     kv_report.add_report(expire_threshold=expire_threshold,
                          ignore_no_expiration=ignore_no_expiration,
                          include_all=include_all,
-                         teams_json=teams_output)
-
-    # Initializes the Message Handler
-    if WEBHOOK_REPORT:
-        msg_handler = message_handler.MessageHandler(WEBHOOK_REPORT)
-
-    if teams_output:
-        success = teams_alert(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
-    else:
-        success = slack_alert(title, kv_report, max_chars=slack_split_chars, slack_app=slack_app,
-                              stdout_only=stdout_only, msg_handler=msg_handler)
-
-    # If success and 'WEBHOOK_NOTIFY' is provided
-    # an additional notify will be posted to the 'WEBHOOK_NOTIFY' webhook
-    if success and WEBHOOK_NOTIFY:
-        logging.info(f"Trigger additional alert about new report message(s)...")
-        alert = message_handler.MessageHandler(WEBHOOK_NOTIFY)
-        alert.post_payload()
+                         teams_json=teams_output,
+                         critical_threshold=critical_threshold)
 
     # Get the full report which will be logged for future references.
     # Azure resource information are added.
     report_full = kv_report.get_report_full()
     if isinstance(report_full, dict):
         workflow_output_name = str(WORKFLOW_OUTPUT_NAME).strip().lower().replace(" ", "_")[:40]
         report_full["name"] = workflow_output_name
@@ -136,14 +127,54 @@
         # Write full report as json to file
         if not isinstance(workflow_output_file, str):
             workflow_output_file = "output.json"
 
         with open(workflow_output_file, 'w') as f:
             json.dump(report_full, f)
 
+    if stdout_only:
+        report = kv_report.get_report_summary_markdown()
+        print(title)
+        print(report)
+        return
+
+    # Initializes the Message Handler
+    if WEBHOOK_REPORT:
+        msg_handler = message_handler.MessageHandler(WEBHOOK_REPORT)
+
+    if teams_output and not success:
+        success = teams_alert(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
+
+    if msg_handler and not teams_output and not success:
+        if slack_app and not success:
+            if not isinstance(critical_threshold, int):
+                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, md=False)
+            else:
+                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars)
+            if payloads:
+                success = slack_post(msg_handler, payloads=payloads)
+
+        if not slack_app and not isinstance(critical_threshold, int) and not success:
+            posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False, md=False)
+            if posts:
+                success = slack_post(msg_handler, posts=posts)
+
+        if isinstance(critical_threshold, int) and not slack_app and not success:
+            error_msg = "Posting individual critical messages to Slack Workflow is not supported."
+            logging.error(error_msg)
+            success = slack_post(msg_handler, posts=[(f"ERROR - {title}", error_msg)])
+
+    # If success and 'WEBHOOK_NOTIFY' is provided
+    # an additional notify will be posted to the 'WEBHOOK_NOTIFY' webhook
+    if success and WEBHOOK_NOTIFY:
+        logging.info(f"Trigger additional alert about new report message(s)...")
+        alert = message_handler.MessageHandler(WEBHOOK_NOTIFY)
+        alert.post_payload()
+
+
 ########################################################################################################################
 
 
 if __name__ == '__main__':
     # The actual report will be posted to the webhook exported in
     # the following environment variable
     WEBHOOK_REPORT = os.getenv("WEBHOOK_REPORT")
```

### Comparing `ops-py-azure-key-vault-alert-4.4.1/azure_key_vault_alert/teams_alert.py` & `ops_py_azure_key_vault_alert-4.5.0/azure_key_vault_alert/teams_alert.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.4.1
+Version: 4.5.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==4.0.1
+Requires-Dist: ops-py-azure-key-vault-report==5.0.2
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
```

### Comparing `ops-py-azure-key-vault-alert-4.4.1/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops_py_azure_key_vault_alert-4.5.0/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jaraco.context==5.3.0
 jaraco.functools==4.0.0
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==4.0.1
+ops-py-azure-key-vault-report==5.0.2
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
 Pygments==2.17.2
 pyproject_hooks==1.0.0
```

### Comparing `ops-py-azure-key-vault-alert-4.4.1/readme.md` & `ops_py_azure_key_vault_alert-4.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.4.1/requirements.txt` & `ops_py_azure_key_vault_alert-4.5.0/requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jaraco.context==5.3.0
 jaraco.functools==4.0.0
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==4.0.1
+ops-py-azure-key-vault-report==5.0.2
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
 Pygments==2.17.2
 pyproject_hooks==1.0.0
```

