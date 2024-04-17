# Comparing `tmp/rhdzmota_extension_streamlit_webapps-0.5.2.tar.gz` & `tmp/rhdzmota_extension_streamlit_webapps-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota_extension_streamlit_webapps-0.5.2.tar", last modified: Tue Apr  9 04:56:06 2024, max compression
+gzip compressed data, was "rhdzmota_extension_streamlit_webapps-0.6.0.tar", last modified: Wed Apr 17 00:55:09 2024, max compression
```

## Comparing `rhdzmota_extension_streamlit_webapps-0.5.2.tar` & `rhdzmota_extension_streamlit_webapps-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.989374 rhdzmota_extension_streamlit_webapps-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.989374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.989374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/components/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps_version
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 04:55:51.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:06.993374 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 04:56:06.000000 rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.926442 rhdzmota_extension_streamlit_webapps-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-17 00:55:09.926442 rhdzmota_extension_streamlit_webapps-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:55:09.926442 rhdzmota_extension_streamlit_webapps-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.922442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_gatekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_temp_acl_via_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps_version
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 00:54:54.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:55:09.926442 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:55:09.000000 rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/top_level.txt
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/PKG-INFO` & `rhdzmota_extension_streamlit_webapps-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota_extension_streamlit_webapps
-Version: 0.5.2
+Version: 0.6.0
 Summary: RHDZMOTA Extension App: streamlit_webapps
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/README.md` & `rhdzmota_extension_streamlit_webapps-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/setup.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/backend.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/backend.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/cli.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/cli.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/page_view.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/page_view.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota/ext/streamlit_webapps/runner.py` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota/ext/streamlit_webapps/runner.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota-extension-streamlit-webapps
-Version: 0.5.2
+Version: 0.6.0
 Summary: RHDZMOTA Extension App: streamlit_webapps
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.2/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt` & `rhdzmota_extension_streamlit_webapps-0.6.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,19 @@
 src/main/rhdzmota/ext/streamlit_webapps/page_view.py
 src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
 src/main/rhdzmota/ext/streamlit_webapps/runner.py
 src/main/rhdzmota/ext/streamlit_webapps/settings.py
 src/main/rhdzmota/ext/streamlit_webapps/components/__init__.py
 src/main/rhdzmota/ext/streamlit_webapps/components/catalog.py
 src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py
+src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_temp_acl_via_jwt.py
+src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/__init__.py
+src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_failure.py
+src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_gatekeeper.py
+src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/comp_email_acl_success.py
+src/main/rhdzmota/ext/streamlit_webapps/components/collection_email_acl_via_token/utils.py
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/dependency_links.txt
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/not-zip-safe
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/requires.txt
 src/main/rhdzmota_extension_streamlit_webapps.egg-info/top_level.txt
```

