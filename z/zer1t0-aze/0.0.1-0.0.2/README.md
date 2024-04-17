# Comparing `tmp/zer1t0-aze-0.0.1.tar.gz` & `tmp/zer1t0_aze-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0-aze-0.0.1.tar", last modified: Wed Apr 10 18:29:52 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.2.tar", last modified: Wed Apr 17 18:21:55 2024, max compression
```

## Comparing `zer1t0-aze-0.0.1.tar` & `zer1t0_aze-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,73 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-10 18:29:52.321418 zer1t0-aze-0.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-10 18:25:45.000000 zer1t0-aze-0.0.1/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-10 18:28:36.000000 zer1t0-aze-0.0.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1102 2024-04-10 18:29:52.321418 zer1t0-aze-0.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      707 2024-04-10 18:14:32.000000 zer1t0-aze-0.0.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-10 18:29:52.321418 zer1t0-aze-0.0.1/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-10 18:04:59.000000 zer1t0-aze-0.0.1/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-10 18:09:35.000000 zer1t0-aze-0.0.1/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-10 18:08:35.000000 zer1t0-aze-0.0.1/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-10 18:29:52.321418 zer1t0-aze-0.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-10 18:00:05.000000 zer1t0-aze-0.0.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-10 18:29:52.321418 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1102 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      447 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-10 18:29:52.000000 zer1t0-aze-0.0.1/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     1666 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1246 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.497674 zer1t0_aze-0.0.2/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10018 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1261 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     1666 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     2329 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-get-login-info
+-rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-inspect-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-login-with-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-tenant-id
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-whoami
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.509674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.513674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.513674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/
+-rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
+-rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 user      (1000) user      (1000)      457 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0-aze-0.0.1/LICENSE` & `zer1t0_aze-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/README.md` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 - **az-get-login-info**: Retrieve login information about an Azure domain.
 - **az-inspect-token**: Show access token (jwt) payload in json format.
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
 - **az-tenant-id**: Retrieves the tenant id from tenant domain.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
+## Install
+
+```
+pip install zer1t0-aze
+```
+
 ## Development
 
 To probe in a development scenario:
 ```
 cd aze/
 pip install -e .
 ```
```

### Comparing `zer1t0-aze-0.0.1/aze/az_get_login_info.py` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/aze/az_inspect_token.py` & `zer1t0_aze-0.0.2/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/aze/az_login_with_token.py` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_login_with_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/aze/az_tenant_id.py` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/aze/read_in.py` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/aze/utils.py` & `zer1t0_aze-0.0.2/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0-aze-0.0.1/setup.py` & `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/setup.py`

 * *Files identical despite different names*

