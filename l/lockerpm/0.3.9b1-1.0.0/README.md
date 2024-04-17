# Comparing `tmp/lockerpm-0.3.9b1.tar.gz` & `tmp/lockerpm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockerpm-0.3.9b1.tar", last modified: Tue Feb 27 07:15:17 2024, max compression
+gzip compressed data, was "lockerpm-1.0.0.tar", last modified: Wed Apr 17 05:36:27 2024, max compression
```

## Comparing `lockerpm-0.3.9b1.tar` & `lockerpm-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/
--rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-0.3.9b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10888 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     9914 2024-02-19 04:59:40.000000 lockerpm-0.3.9b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.357288 lockerpm-0.3.9b1/docs/
--rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/docs/standard.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/
--rw-rw-r--   0 root         (0) root         (0)      162 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/__about__.json
--rw-rw-r--   0 root         (0) root         (0)      228 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/__about__.py
--rw-rw-r--   0 root         (0) root         (0)     2425 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10317 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     6291 2024-02-15 10:26:50.000000 lockerpm-0.3.9b1/locker/client.py
--rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-0.3.9b1/locker/error.py
--rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-0.3.9b1/locker/logger.py
--rw-rw-r--   0 root         (0) root         (0)    13121 2024-02-08 15:53:14.000000 lockerpm-0.3.9b1/locker/ls_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/ls_resources/
--rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/ls_resources/abstract/
--rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5130 2024-02-08 15:53:14.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/createable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/deletable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/detailable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/listable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/singleton_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/updateable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2548 2024-02-15 10:26:50.000000 lockerpm-0.3.9b1/locker/ls_resources/environment.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/error_object.py
--rw-rw-r--   0 root         (0) root         (0)     2965 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/ls_resources/secret.py
--rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_response.py
--rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/object_classes.py
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/lockerpm.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10888 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/requirements-dev.txt
--rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/requirements-test.txt
--rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-0.3.9b1/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       61 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-23 08:02:16.000000 lockerpm-0.3.9b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1377 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     2636 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_client.py
--rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tests/test_logger.py
--rw-rw-r--   0 root         (0) root         (0)     2788 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_util.py
--rw-rw-r--   0 root         (0) root         (0)     1219 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/
+-rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12566 2024-04-17 05:36:27.188693 lockerpm-1.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    11480 2024-04-08 04:15:59.000000 lockerpm-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.184693 lockerpm-1.0.0/docs/
+-rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-1.0.0/docs/standard.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.184693 lockerpm-1.0.0/locker/
+-rw-rw-r--   0 root         (0) root         (0)      160 2024-04-17 05:35:29.000000 lockerpm-1.0.0/locker/__about__.json
+-rw-rw-r--   0 root         (0) root         (0)      226 2024-04-17 05:35:29.000000 lockerpm-1.0.0/locker/__about__.py
+-rw-rw-r--   0 root         (0) root         (0)     4394 2024-04-07 16:22:07.000000 lockerpm-1.0.0/locker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6458 2024-02-29 03:03:49.000000 lockerpm-1.0.0/locker/atomic_locking.py
+-rw-rw-r--   0 root         (0) root         (0)    10159 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     7073 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/client.py
+-rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-1.0.0/locker/error.py
+-rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-1.0.0/locker/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     1997 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_logger.py
+-rw-rw-r--   0 root         (0) root         (0)    13071 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/locker/ls_resources/
+-rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/locker/ls_resources/abstract/
+-rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5039 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_resources/abstract/api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/createable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/deletable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/detailable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/listable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/singleton_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-1.0.0/locker/ls_resources/abstract/updateable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2548 2024-02-15 10:26:50.000000 lockerpm-1.0.0/locker/ls_resources/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/error_object.py
+-rw-rw-r--   0 root         (0) root         (0)     2965 2024-02-27 07:14:42.000000 lockerpm-1.0.0/locker/ls_resources/secret.py
+-rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_response.py
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/object_classes.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/lockerpm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12566 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1221 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-1.0.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-1.0.0/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-1.0.0/requirements-test.txt
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-1.0.0/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-04-17 05:36:27.192693 lockerpm-1.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4471 2024-04-17 05:35:29.000000 lockerpm-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1377 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     2636 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_client.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tests/test_logger.py
+-rw-rw-r--   0 root         (0) root         (0)     2788 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1219 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tox.ini
```

### Comparing `lockerpm-0.3.9b1/PKG-INFO` & `lockerpm-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: lockerpm
-Version: 0.3.9b1
-Summary: Locker Secret Python SDK
-Home-page: https://locker.io
-Download-URL: 
-Author: CyStack
-Author-email: contact@locker.io
-Keywords: django,vault management,security
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Locker Secret Python SDK
 
 <p align="center">
   <img src="https://cystack.net/images/logo-black.svg" alt="CyStack" width="50%"/>
 </p>
 
  
@@ -69,42 +44,65 @@
 
 ```
 python setup.py install
 ```
 
 ## Usages
 
-### Set up access key
 
-The SDK needs to be configured with your access key, which is available in your Locker Secret Dashboard. 
-Initialize the `secret_access_key` to its value. 
-You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
+### Configuration access key
+
+The SDK needs to be configured with your access key id and your secret access key, which is available in your 
+Locker Secret Dashboard. These keys must not be disclosed. If you reveal these keys, you need to revoke 
+them immediately. Environment variables are a good solution and they are easy to consume in most programming languages.
+
+**Set up credentials on Linux/MacOS**
+```
+export ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+export SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
+
+**Set up credentials on Windows**
+
+Powershell
+```
+$Env:ACCESS_KEY_ID = '<YOUR_ACCESS_KEY_ID>'
+$Env:SECRET_ACCESS_KEY = '<SECRET_ACCESS_KEY>'
+```
+
+Command Prompt
+```
+set ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+set SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
 
+You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
 If you need to set your custom headers, you also need to set `headers` value in the `options` param:
 
+Now, you can use SDK to get or set values:
 ```
 from locker import Locker
 
-access_key_id = "your_access_key_id..."
-secret_access_key = "your_secret_access_key..."
 api_base = "your_base_api.host"
-headers = {
-    "cf-access-client-id": "",
-    "cf-access-client-secret": ""
-}
-
 locker = Locker(
-    access_key_id=access_key_id, 
-    secret_access_key=secret_access_key, 
     api_base=api_base, 
     options={"headers": headers}
 )
 ```
 
-Now, you can use SDK to get or set values:
+You can also pass parameters in the `Locker()` method or use the shared credential file (`~/.locker/credentials`), 
+but we do not recommend these ways. 
+```
+locker = Locker(
+    access_key_id=os.get_env("<YOUR_ACCESS_KEY_ID>"),
+    secret_access_key=os.get_env("<YOUR_SECRET_ACCESS_KEY>"),
+    api_base=api_base, 
+    options={"headers": headers}
+)
+```
 
 
 ### List secrets
 
 Use `.list()` to get all the secrets in your project. 
 
 ```
@@ -274,21 +272,20 @@
 2. Set `log` when initializing the Locker object:
 
 ```python
 from locker import Locker
 
 locker = Locker(log="debug")
 ```
-
-3. Enable it through Python's logging module:
-
+or 
 ```python
-import logging
-logging.basicConfig()
-logging.getLogger('locker').setLevel(logging.DEBUG)
+from locker import Locker
+
+locker = Locker()
+locker.log = "debug"
 ```
 
 
 ## Examples
 
 See the [examples' folder](/examples).
 
@@ -319,14 +316,55 @@
 ```
 
 Run all tests in a single file:
 ```
 tox -e py3.10 -- tests/test_util.py
 ```
 
+## Troubleshooting
+
+This section provides solutions to problems you might encounter when using the SDK. 
+
+### Using with gunicorn
+
+If the Locker object is declared at the same time as your gunicorn application and gunicorn's number of workers 
+is greater than 1, you must use gunicorn's `--preload` parameter to load the application code before the worker process 
+is forked.
+
+```
+gunicorn --preload -w 5 -b 0.0.0.0:8000 your_project.wsgi:application
+```
+
+### Using in multiple-thread
+
+When using Locker in multi-threading, you should place the Locker declaration in a mutex lock to prevent 
+race conditions
+
+Example:
+
+```
+from threading import Lock
+
+# create a lock
+lock = Lock()
+# acquire the lock
+lock.acquire()
+# Declare Locker object Here
+locker = Locker(
+    access_key_id=access_key_id, 
+    secret_access_key=secret_access_key
+)
+locker.get(YOUR_SECRET_KEY)
+# release the lock
+lock.release()
+```
+
+<!-- ### Upgrading the version -->
+
+
 
 ## Reporting security issues
 
 We take the security and our users' trust very seriously. If you found a security issue in Locker SDK Python, please 
 report the issue by contacting us at <contact@locker.io>. Do not file an issue on the tracker.
```

### Comparing `lockerpm-0.3.9b1/README.md` & `lockerpm-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: lockerpm
+Version: 1.0.0
+Summary: Locker Secret Python SDK
+Home-page: https://locker.io
+Download-URL: 
+Author: CyStack
+Author-email: contact@locker.io
+Keywords: django,vault management,security
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Locker Secret Python SDK
 
 <p align="center">
   <img src="https://cystack.net/images/logo-black.svg" alt="CyStack" width="50%"/>
 </p>
 
  
@@ -44,42 +71,65 @@
 
 ```
 python setup.py install
 ```
 
 ## Usages
 
-### Set up access key
 
-The SDK needs to be configured with your access key, which is available in your Locker Secret Dashboard. 
-Initialize the `secret_access_key` to its value. 
-You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
+### Configuration access key
+
+The SDK needs to be configured with your access key id and your secret access key, which is available in your 
+Locker Secret Dashboard. These keys must not be disclosed. If you reveal these keys, you need to revoke 
+them immediately. Environment variables are a good solution and they are easy to consume in most programming languages.
+
+**Set up credentials on Linux/MacOS**
+```
+export ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+export SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
+
+**Set up credentials on Windows**
+
+Powershell
+```
+$Env:ACCESS_KEY_ID = '<YOUR_ACCESS_KEY_ID>'
+$Env:SECRET_ACCESS_KEY = '<SECRET_ACCESS_KEY>'
+```
+
+Command Prompt
+```
+set ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+set SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
 
+You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
 If you need to set your custom headers, you also need to set `headers` value in the `options` param:
 
+Now, you can use SDK to get or set values:
 ```
 from locker import Locker
 
-access_key_id = "your_access_key_id..."
-secret_access_key = "your_secret_access_key..."
 api_base = "your_base_api.host"
-headers = {
-    "cf-access-client-id": "",
-    "cf-access-client-secret": ""
-}
-
 locker = Locker(
-    access_key_id=access_key_id, 
-    secret_access_key=secret_access_key, 
     api_base=api_base, 
     options={"headers": headers}
 )
 ```
 
-Now, you can use SDK to get or set values:
+You can also pass parameters in the `Locker()` method or use the shared credential file (`~/.locker/credentials`), 
+but we do not recommend these ways. 
+```
+locker = Locker(
+    access_key_id=os.get_env("<YOUR_ACCESS_KEY_ID>"),
+    secret_access_key=os.get_env("<YOUR_SECRET_ACCESS_KEY>"),
+    api_base=api_base, 
+    options={"headers": headers}
+)
+```
 
 
 ### List secrets
 
 Use `.list()` to get all the secrets in your project. 
 
 ```
@@ -249,21 +299,20 @@
 2. Set `log` when initializing the Locker object:
 
 ```python
 from locker import Locker
 
 locker = Locker(log="debug")
 ```
-
-3. Enable it through Python's logging module:
-
+or 
 ```python
-import logging
-logging.basicConfig()
-logging.getLogger('locker').setLevel(logging.DEBUG)
+from locker import Locker
+
+locker = Locker()
+locker.log = "debug"
 ```
 
 
 ## Examples
 
 See the [examples' folder](/examples).
 
@@ -294,14 +343,55 @@
 ```
 
 Run all tests in a single file:
 ```
 tox -e py3.10 -- tests/test_util.py
 ```
 
+## Troubleshooting
+
+This section provides solutions to problems you might encounter when using the SDK. 
+
+### Using with gunicorn
+
+If the Locker object is declared at the same time as your gunicorn application and gunicorn's number of workers 
+is greater than 1, you must use gunicorn's `--preload` parameter to load the application code before the worker process 
+is forked.
+
+```
+gunicorn --preload -w 5 -b 0.0.0.0:8000 your_project.wsgi:application
+```
+
+### Using in multiple-thread
+
+When using Locker in multi-threading, you should place the Locker declaration in a mutex lock to prevent 
+race conditions
+
+Example:
+
+```
+from threading import Lock
+
+# create a lock
+lock = Lock()
+# acquire the lock
+lock.acquire()
+# Declare Locker object Here
+locker = Locker(
+    access_key_id=access_key_id, 
+    secret_access_key=secret_access_key
+)
+locker.get(YOUR_SECRET_KEY)
+# release the lock
+lock.release()
+```
+
+<!-- ### Upgrading the version -->
+
+
 
 ## Reporting security issues
 
 We take the security and our users' trust very seriously. If you found a security issue in Locker SDK Python, please 
 report the issue by contacting us at <contact@locker.io>. Do not file an issue on the tracker.
```

### Comparing `lockerpm-0.3.9b1/docs/standard.md` & `lockerpm-1.0.0/docs/standard.md`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/binary_adapter.py` & `lockerpm-1.0.0/locker/binary_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         return binary_file_path
 
     def call(
         self,
         cli,
         params=None,
         asjson=True,
-        shell=True,
         timeout=DEFAULT_TIMEOUT,
         skip_cli_lines=0
     ):
         binary_file = self.get_binary_file()
         my_access_key_id = self.access_key_id
         my_secret_access_key = self.secret_access_key
         # if my_access_key_id is None or my_secret_access_key is None:
@@ -258,12 +257,7 @@
             )
         else:
             return error.LockerError(
                 error_data.get("message"),
                 http_body=error_data,
                 code="locker_error"
             )
-
-            # return error.APIError(
-            #     error_data.get("message"),
-            #     http_body=error_data
-            # )
```

### Comparing `lockerpm-0.3.9b1/locker/client.py` & `lockerpm-1.0.0/locker/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import copy
+import logging
+import os
+import socket
 from typing import Dict, Any
 
 from locker.ls_resources import Secret, Environment
-from locker.logger import Logger
+
+
+LOCKER_LOG = os.environ.get("LOCKER_LOG")
 
 
 class Locker:
     DEFAULT_OPTIONS = {
         "access_key_id": None,
         "secret_access_key": None,
         "api_base": "https://api.locker.io/locker_secrets",
@@ -30,22 +35,24 @@
         proxy: Any = None,
         log: str = None,
         max_network_retries: int = 0,
         resttime: int = 120,
         fetch: bool = False,
         options: Dict = None,
     ):
+        # self.download_binary()
         if options is None:
             options = {}
         if api_base:
             options["api_base"] = api_base
         if api_version:
             options["api_version"] = api_version
         if proxy:
             options["proxy"] = proxy
+        log = log or LOCKER_LOG
         if log:
             options["log"] = log
         assert resttime >= -1
         options["resttime"] = resttime
         options["fetch"] = fetch
 
         if max_network_retries:
@@ -63,15 +70,16 @@
         else:
             headers = {}
 
         self._options.update(options)
         self._options["headers"].update(headers)
 
         # Set Logger
-        self._options["logger"] = Logger(log_level=self._options.get("log"))
+        logger = self._set_stream_logger(level=self._options.get('log'))
+        self._options["logger"] = logger
 
         # Rip off trailing slash since all urls depend on that
         assert isinstance(self._options["api_base"], str)
         if self._options["api_base"].endswith("/"):
             self._options["api_base"] = self._options["api_base"][:-1]
 
         # if access_key_basic_auth:
@@ -112,15 +120,31 @@
     @property
     def log(self):
         return self._options.get("log")
 
     @log.setter
     def log(self, log_value):
         self._options.update({"log": log_value})
-        self._options["logger"] = Logger(log_level=self._options.get("log"))
+        logger = self._set_stream_logger(level=log_value)
+        self._options["logger"] = logger
+
+    @staticmethod
+    def _set_stream_logger(level, name='locker'):
+        assert level in ["debug", "info", "warning", "error"], "The log level is not valid"
+        level = level.upper()
+        format_string = '%(asctime)s {hostname} %(levelname)s %(message)s'.format(**{'hostname': socket.gethostname()})
+
+        logger = logging.getLogger(name)
+        logger.setLevel(level)
+        handler = logging.StreamHandler()
+        handler.setLevel(level)
+        formatter = logging.Formatter(format_string)
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+        return logger
 
     @property
     def resttime(self):
         return self._options.get("resttime")
 
     @resttime.setter
     def resttime(self, resttime_value):
```

### Comparing `lockerpm-0.3.9b1/locker/error.py` & `lockerpm-1.0.0/locker/error.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/logger.py` & `lockerpm-1.0.0/locker/logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_object.py` & `lockerpm-1.0.0/locker/ls_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,22 +195,22 @@
             super().__setitem__(
                 k,
                 util.convert_to_ls_object(v, access_key_id, secret_access_key, api_base, api_version),
             )
 
         self._previous = values
 
-    def call(self, cli, asjson=True, shell=True, timeout=DEFAULT_TIMEOUT, params=None):
+    def call(self, cli, asjson=True, timeout=DEFAULT_TIMEOUT, params=None):
         return LSObject._call(
-            self, cli, asjson=asjson, shell=shell, timeout=timeout, params=params
+            self, cli, asjson=asjson, timeout=timeout, params=params
         )
 
     # The 'cli_' is suffixed with an underscore to avoid conflicting with request parameters in `params`
     def _call(self, cli_, access_key_id=None, secret_access_key=None, api_base=None, api_version=None,
-              asjson=True, shell=True, timeout=DEFAULT_TIMEOUT, params=None):
+              asjson=True, timeout=DEFAULT_TIMEOUT, params=None):
         params = None if params is None else params.copy()
 
         access_key_id = util.read_special_variable(params, "access_key_id", access_key_id)
         secret_access_key = util.read_special_variable(params, "secret_access_key", secret_access_key)
         api_base = util.read_special_variable(params, "api_base", api_base)
         api_version = util.read_special_variable(params, "api_version", api_version)
         headers = util.read_special_variable(params, "headers", None)
@@ -232,15 +232,15 @@
             api_version=api_version,
             headers=headers,
             logger=logger,
             resttime=resttime,
             fetch=fetch,
         )
         res_data = binary_executor.call(
-            cli=cli_, params=params, asjson=asjson, shell=shell, timeout=timeout, skip_cli_lines=skip_cli_lines
+            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines
         )
         return util.convert_to_ls_object(
             res_data, access_key_id, secret_access_key, api_base, api_version, params
         )
 
     def __repr__(self):
         ident_parts = [type(self).__name__]
```

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/__init__.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/api_resource.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/api_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,27 +56,25 @@
         self,
         cli_,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
         asjson=True,
-        shell=True,
         timeout=DEFAULT_TIMEOUT,
         params=None,
     ):
         obj = LSObject._call(
             self,
             cli_,
             access_key_id,
             secret_access_key,
             api_base,
             api_version,
             asjson,
-            shell,
             timeout,
             params,
         )
 
         if type(self) is type(obj):
             self.refresh_from(obj)
             return self
@@ -87,35 +85,34 @@
     def _call_and_refresh(
         self,
         cli,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
-        asjson=True, shell=True, timeout=DEFAULT_TIMEOUT, params=None
+        asjson=True, timeout=DEFAULT_TIMEOUT, params=None
     ):
         obj = LSObject._call(
             self,
             cli, access_key_id, secret_access_key, api_base, api_version,
-            asjson, shell, timeout, params
+            asjson, timeout, params
         )
         self.refresh_from(obj)
         return self
 
     # The 'cli_' is suffixed with an underscore to avoid conflicting with request parameters in `params`
     @classmethod
     def _static_call(
         cls,
         cli_,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
         asjson=True,
-        shell=True,
         timeout=DEFAULT_TIMEOUT,
         params=None,
     ):
         params = None if params is None else params.copy()
         access_key_id = util.read_special_variable(params, "access_key_id", access_key_id)
         secret_access_key = util.read_special_variable(params, "secret_access_key", secret_access_key)
         api_base = util.read_special_variable(params, "api_base", api_base)
@@ -133,13 +130,13 @@
             api_version=api_version,
             headers=headers,
             logger=logger,
             resttime=resttime,
             fetch=fetch
         )
         res_data = binary_executor.call(
-            cli=cli_, params=params, asjson=asjson, shell=shell, timeout=timeout, skip_cli_lines=skip_cli_lines
+            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines
         )
         return util.convert_to_ls_object(
             res_data, access_key_id, secret_access_key, api_base, api_version, params
         )
```

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/createable_api_resource.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/deletable_api_resource.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/listable_api_resource.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/abstract/singleton_api_resource.py` & `lockerpm-1.0.0/locker/ls_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/environment.py` & `lockerpm-1.0.0/locker/ls_resources/environment.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/error_object.py` & `lockerpm-1.0.0/locker/ls_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_resources/secret.py` & `lockerpm-1.0.0/locker/ls_resources/secret.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/ls_response.py` & `lockerpm-1.0.0/locker/ls_response.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/locker/util.py` & `lockerpm-1.0.0/locker/util.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/lockerpm.egg-info/PKG-INFO` & `lockerpm-1.0.0/lockerpm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: lockerpm
-Version: 0.3.9b1
+Version: 1.0.0
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Locker Secret Python SDK
 
 <p align="center">
   <img src="https://cystack.net/images/logo-black.svg" alt="CyStack" width="50%"/>
@@ -69,42 +71,65 @@
 
 ```
 python setup.py install
 ```
 
 ## Usages
 
-### Set up access key
 
-The SDK needs to be configured with your access key, which is available in your Locker Secret Dashboard. 
-Initialize the `secret_access_key` to its value. 
-You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
+### Configuration access key
+
+The SDK needs to be configured with your access key id and your secret access key, which is available in your 
+Locker Secret Dashboard. These keys must not be disclosed. If you reveal these keys, you need to revoke 
+them immediately. Environment variables are a good solution and they are easy to consume in most programming languages.
+
+**Set up credentials on Linux/MacOS**
+```
+export ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+export SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
+
+**Set up credentials on Windows**
+
+Powershell
+```
+$Env:ACCESS_KEY_ID = '<YOUR_ACCESS_KEY_ID>'
+$Env:SECRET_ACCESS_KEY = '<SECRET_ACCESS_KEY>'
+```
+
+Command Prompt
+```
+set ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
+set SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
+```
 
+You also need to set `api_base` value (default is `https://api.locker.io/locker_secrets`).
 If you need to set your custom headers, you also need to set `headers` value in the `options` param:
 
+Now, you can use SDK to get or set values:
 ```
 from locker import Locker
 
-access_key_id = "your_access_key_id..."
-secret_access_key = "your_secret_access_key..."
 api_base = "your_base_api.host"
-headers = {
-    "cf-access-client-id": "",
-    "cf-access-client-secret": ""
-}
-
 locker = Locker(
-    access_key_id=access_key_id, 
-    secret_access_key=secret_access_key, 
     api_base=api_base, 
     options={"headers": headers}
 )
 ```
 
-Now, you can use SDK to get or set values:
+You can also pass parameters in the `Locker()` method or use the shared credential file (`~/.locker/credentials`), 
+but we do not recommend these ways. 
+```
+locker = Locker(
+    access_key_id=os.get_env("<YOUR_ACCESS_KEY_ID>"),
+    secret_access_key=os.get_env("<YOUR_SECRET_ACCESS_KEY>"),
+    api_base=api_base, 
+    options={"headers": headers}
+)
+```
 
 
 ### List secrets
 
 Use `.list()` to get all the secrets in your project. 
 
 ```
@@ -274,21 +299,20 @@
 2. Set `log` when initializing the Locker object:
 
 ```python
 from locker import Locker
 
 locker = Locker(log="debug")
 ```
-
-3. Enable it through Python's logging module:
-
+or 
 ```python
-import logging
-logging.basicConfig()
-logging.getLogger('locker').setLevel(logging.DEBUG)
+from locker import Locker
+
+locker = Locker()
+locker.log = "debug"
 ```
 
 
 ## Examples
 
 See the [examples' folder](/examples).
 
@@ -319,14 +343,55 @@
 ```
 
 Run all tests in a single file:
 ```
 tox -e py3.10 -- tests/test_util.py
 ```
 
+## Troubleshooting
+
+This section provides solutions to problems you might encounter when using the SDK. 
+
+### Using with gunicorn
+
+If the Locker object is declared at the same time as your gunicorn application and gunicorn's number of workers 
+is greater than 1, you must use gunicorn's `--preload` parameter to load the application code before the worker process 
+is forked.
+
+```
+gunicorn --preload -w 5 -b 0.0.0.0:8000 your_project.wsgi:application
+```
+
+### Using in multiple-thread
+
+When using Locker in multi-threading, you should place the Locker declaration in a mutex lock to prevent 
+race conditions
+
+Example:
+
+```
+from threading import Lock
+
+# create a lock
+lock = Lock()
+# acquire the lock
+lock.acquire()
+# Declare Locker object Here
+locker = Locker(
+    access_key_id=access_key_id, 
+    secret_access_key=secret_access_key
+)
+locker.get(YOUR_SECRET_KEY)
+# release the lock
+lock.release()
+```
+
+<!-- ### Upgrading the version -->
+
+
 
 ## Reporting security issues
 
 We take the security and our users' trust very seriously. If you found a security issue in Locker SDK Python, please 
 report the issue by contacting us at <contact@locker.io>. Do not file an issue on the tracker.
```

### Comparing `lockerpm-0.3.9b1/lockerpm.egg-info/SOURCES.txt` & `lockerpm-1.0.0/lockerpm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 setup.cfg
 setup.py
 tox.ini
 docs/standard.md
 locker/__about__.json
 locker/__about__.py
 locker/__init__.py
+locker/atomic_locking.py
 locker/binary_adapter.py
 locker/client.py
 locker/error.py
 locker/logger.py
+locker/ls_logger.py
 locker/ls_object.py
 locker/ls_response.py
 locker/object_classes.py
 locker/util.py
 locker/ls_resources/__init__.py
 locker/ls_resources/environment.py
 locker/ls_resources/error_object.py
```

### Comparing `lockerpm-0.3.9b1/setup.py` & `lockerpm-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,38 @@
 
 def _requirements_test():
     # download_binary()
     with open('requirements-test.txt', 'r') as f:
         return [name.strip() for name in f.readlines()]
 
 
+def _classifiers():
+    classifiers = [
+        "Intended Audience :: Developers",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.6",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ]
+    if "b1" in __version__:
+        classifiers += ["Development Status :: 3 - Alpha"]
+    else:
+        classifiers += ["Development Status :: 5 - Production/Stable"]
+    return classifiers
+
+
 class PyTest(TestCommand):
     def finalize_options(self):
         TestCommand.finalize_options(self)
         self.test_args = []
         self.test_suite = True
 
     def run_tests(self):
@@ -40,44 +64,44 @@
         sys.exit(errno)
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
-def download_binary():
-    home_dir = os.path.expanduser("~")
-    locker_dir = os.path.join(home_dir, ".locker")
-    binary_file_path = os.path.join(locker_dir, f"locker_binary-{binary_version}")
-
-    if sys.platform == "darwin":
-        if platform.processor() == "arm":
-            binary_url = f"https://s.locker.io/download/locker-cli-mac-arm64-{binary_version}"
-        else:
-            binary_url = f"https://s.locker.io/download/locker-cli-mac-x64-{binary_version}"
-    elif sys.platform == "win32":
-        binary_url = f"https://s.locker.io/download/locker-cli-win-x64-{binary_version}.exe"
-        binary_file_path = os.path.join(locker_dir, f"locker_binary-{binary_version}.exe")
-    else:
-        binary_url = f"https://s.locker.io/download/locker-cli-linux-x64-{binary_version}"
-
-    # Check if the .locker directory exists, and create it if not
-    if not os.path.exists(locker_dir):
-        os.makedirs(locker_dir)
-
-    # Download binary file
-    if not os.path.exists(binary_file_path):
-        # req = urllib.request.urlopen(binary_url)
-
-        try:
-            urllib.request.urlretrieve(binary_url, binary_file_path)
-            print("saving to", os.path.abspath(binary_file_path))
-        except Exception as e:
-            print(f"Download failed: {e}")
-            raise e
+# def download_binary():
+#     home_dir = os.path.expanduser("~")
+#     locker_dir = os.path.join(home_dir, ".locker")
+#     binary_file_path = os.path.join(locker_dir, f"locker_binary-{binary_version}")
+#
+#     if sys.platform == "darwin":
+#         if platform.processor() == "arm":
+#             binary_url = f"https://s.locker.io/download/locker-cli-mac-arm64-{binary_version}"
+#         else:
+#             binary_url = f"https://s.locker.io/download/locker-cli-mac-x64-{binary_version}"
+#     elif sys.platform == "win32":
+#         binary_url = f"https://s.locker.io/download/locker-cli-win-x64-{binary_version}.exe"
+#         binary_file_path = os.path.join(locker_dir, f"locker_binary-{binary_version}.exe")
+#     else:
+#         binary_url = f"https://s.locker.io/download/locker-cli-linux-x64-{binary_version}"
+#
+#     # Check if the .locker directory exists, and create it if not
+#     if not os.path.exists(locker_dir):
+#         os.makedirs(locker_dir)
+#
+#     # Download binary file
+#     if not os.path.exists(binary_file_path):
+#         # req = urllib.request.urlopen(binary_url)
+#
+#         try:
+#             urllib.request.urlretrieve(binary_url, binary_file_path)
+#             print("saving to", os.path.abspath(binary_file_path))
+#         except Exception as e:
+#             print(f"Download failed: {e}")
+#             raise e
 
 
 def main():
     setup(
         name="lockerpm",
         version=__version__,
         author="CyStack",
@@ -107,27 +131,13 @@
         ),
         python_requires=">=3.6",
         install_requires=_requirements(),
         tests_require=_requirements_test(),
         cmdclass={
             'test': PyTest,
         },
-        classifiers=[
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Developers",
-            "Operating System :: OS Independent",
-            "Programming Language :: Python",
-            "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3 :: Only",
-            "Programming Language :: Python :: 3.10",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.6",
-            "Topic :: Software Development :: Libraries :: Application Frameworks",
-            "Topic :: Software Development :: Libraries :: Python Modules",
-        ]
+        classifiers=_classifiers(),
     )
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `lockerpm-0.3.9b1/tests/test_binary_adapter.py` & `lockerpm-1.0.0/tests/test_binary_adapter.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/tests/test_client.py` & `lockerpm-1.0.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/tests/test_logger.py` & `lockerpm-1.0.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/tests/test_util.py` & `lockerpm-1.0.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.9b1/tox.ini` & `lockerpm-1.0.0/tox.ini`

 * *Files identical despite different names*

