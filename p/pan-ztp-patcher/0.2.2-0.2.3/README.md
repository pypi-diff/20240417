# Comparing `tmp/pan_ztp_patcher-0.2.2.tar.gz` & `tmp/pan_ztp_patcher-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.2.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.3.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.2.tar` & `pan_ztp_patcher-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.2/README.md
--rw-r--r--   0        0        0     4518 2024-04-16 17:35:02.987866 pan_ztp_patcher-0.2.2/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.2/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    20240 2024-04-16 17:39:53.108051 pan_ztp_patcher-0.2.2/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      510 2024-04-16 18:15:53.283602 pan_ztp_patcher-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.3/README.md
+-rw-r--r--   0        0        0     4518 2024-04-16 17:35:02.987866 pan_ztp_patcher-0.2.3/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.3/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    20400 2024-04-17 20:12:07.797676 pan_ztp_patcher-0.2.3/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      510 2024-04-17 20:16:00.092902 pan_ztp_patcher-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.3/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.2/README.md` & `pan_ztp_patcher-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.2/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.2.3/pan_ztp_patcher/app.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.2/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.3/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.2/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.3/pan_ztp_patcher/ztp_patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,29 +316,34 @@
             pi_username,
             pi_hostname,
             content_path,
             content_file,
         )
         logger.debug("Sending SCP command: {}".format(scp_command))
         shell.send(scp_command + "\n")
-        time.sleep(2)
+        time.sleep(5)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Check if the host authenticity prompt appears
         logger.debug("Checking for host authenticity prompt...")
-        if "Please type 'yes', 'no' or the fingerprint" in output:
+        if (
+            "Please type 'yes', 'no' or the fingerprint" in output
+            or "Are you sure you want to continue connecting" in output
+        ):  # noqa: E501
             logger.debug("Sending 'yes' to the prompt...")
             shell.send("yes\n")
             time.sleep(2)
             output = shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
 
         # Send the password for pi@
-        logger.debug("Sending password for pi@{}...".format(pi_hostname))
+        logger.debug(
+            "Sending password for {}@{}...".format(pi_username, pi_hostname)
+        )  # noqa: E501
         time.sleep(2)
         shell.send(pi_password + "\n")
         time.sleep(2)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Wait for the completion prompt
@@ -351,15 +356,15 @@
                 )
                 break
             output += shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
             if "already exists" in output:
                 logger.info("Content file already exists on the firewall.")
                 break
-            elif "100%" in output and "ETA" not in output:
+            elif "saved" in output and "ETA" not in output:
                 logger.debug("SCP import content completed successfully.")
                 logger.info("SCP import content completed successfully.")
                 break
             time.sleep(1)
 
         # Close the SSH connection
         client.close()
```

### Comparing `pan_ztp_patcher-0.2.2/PKG-INFO` & `pan_ztp_patcher-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.2
+Version: 0.2.3
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

