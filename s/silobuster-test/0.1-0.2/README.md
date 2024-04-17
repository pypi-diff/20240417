# Comparing `tmp/silobuster_test-0.1.tar.gz` & `tmp/silobuster_test-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster_test-0.1.tar", last modified: Tue Apr 16 23:49:24 2024, max compression
+gzip compressed data, was "silobuster_test-0.2.tar", last modified: Wed Apr 17 00:16:29 2024, max compression
```

## Comparing `silobuster_test-0.1.tar` & `silobuster_test-0.2.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.337817 silobuster_test-0.1/
--rw-r--r--   0 jhom       (502) staff       (20)      138 2024-04-16 23:49:24.336669 silobuster_test-0.1/PKG-INFO
--rw-r--r--   0 jhom       (502) staff       (20)     6246 2024-04-16 23:01:26.000000 silobuster_test-0.1/README.md
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.142672 silobuster_test-0.1/deduper/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/admin.py
--rw-r--r--   0 jhom       (502) staff       (20)      140 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/apps.py
--rw-r--r--   0 jhom       (502) staff       (20)      383 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/asgi.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.234204 silobuster_test-0.1/deduper/deduplicate/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/admin.py
--rw-r--r--   0 jhom       (502) staff       (20)      154 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/apps.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.239236 silobuster_test-0.1/deduper/deduplicate/migrations/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/migrations/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/models.py
--rw-r--r--   0 jhom       (502) staff       (20)     6946 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/process_requests.py
--rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/tests.py
--rw-r--r--   0 jhom       (502) staff       (20)      387 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/urls.py
--rw-r--r--   0 jhom       (502) staff       (20)     3424 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/deduplicate/views.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.290160 silobuster_test-0.1/deduper/logs/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/admin.py
--rw-r--r--   0 jhom       (502) staff       (20)      140 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/apps.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.292961 silobuster_test-0.1/deduper/logs/migrations/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/migrations/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/models.py
--rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/tests.py
--rw-r--r--   0 jhom       (502) staff       (20)      206 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/urls.py
--rw-r--r--   0 jhom       (502) staff       (20)     2075 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/logs/views.py
--rwxr-xr-x   0 jhom       (502) staff       (20)      655 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/manage.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.295792 silobuster_test-0.1/deduper/migrations/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/migrations/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/models.py
--rw-r--r--   0 jhom       (502) staff       (20)     4078 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/settings.py
--rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/tests.py
--rw-r--r--   0 jhom       (502) staff       (20)      999 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/urls.py
--rw-r--r--   0 jhom       (502) staff       (20)     1324 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/views.py
--rw-r--r--   0 jhom       (502) staff       (20)      391 2024-04-16 23:01:26.000000 silobuster_test-0.1/deduper/wsgi.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.307216 silobuster_test-0.1/manglers/
--rw-r--r--   0 jhom       (502) staff       (20)       93 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)     1367 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/mangle_org_name.py
--rw-r--r--   0 jhom       (502) staff       (20)     3860 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/mangle_url.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.318782 silobuster_test-0.1/manglers/tests/
--rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/tests/__init__.py
--rw-r--r--   0 jhom       (502) staff       (20)     5417 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/tests/test_mangle_org.py
--rw-r--r--   0 jhom       (502) staff       (20)     9549 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/tests/test_mangle_url.py
--rw-r--r--   0 jhom       (502) staff       (20)     1128 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/tests/testing.py
--rw-r--r--   0 jhom       (502) staff       (20)      978 2024-04-16 23:01:26.000000 silobuster_test-0.1/manglers/tld_swap_prob_dict.py
--rw-r--r--   0 jhom       (502) staff       (20)       38 2024-04-16 23:49:24.338263 silobuster_test-0.1/setup.cfg
--rw-r--r--   0 jhom       (502) staff       (20)      425 2024-04-16 23:47:31.000000 silobuster_test-0.1/setup.py
-drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-16 23:49:24.333193 silobuster_test-0.1/silobuster_test.egg-info/
--rw-r--r--   0 jhom       (502) staff       (20)      138 2024-04-16 23:49:23.000000 silobuster_test-0.1/silobuster_test.egg-info/PKG-INFO
--rw-r--r--   0 jhom       (502) staff       (20)     1138 2024-04-16 23:49:23.000000 silobuster_test-0.1/silobuster_test.egg-info/SOURCES.txt
--rw-r--r--   0 jhom       (502) staff       (20)        1 2024-04-16 23:49:23.000000 silobuster_test-0.1/silobuster_test.egg-info/dependency_links.txt
--rw-r--r--   0 jhom       (502) staff       (20)       13 2024-04-16 23:49:23.000000 silobuster_test-0.1/silobuster_test.egg-info/requires.txt
--rw-r--r--   0 jhom       (502) staff       (20)       17 2024-04-16 23:49:23.000000 silobuster_test-0.1/silobuster_test.egg-info/top_level.txt
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:29.054219 silobuster_test-0.2/
+-rw-r--r--   0 jhom       (502) staff       (20)      138 2024-04-17 00:16:29.052737 silobuster_test-0.2/PKG-INFO
+-rw-r--r--   0 jhom       (502) staff       (20)     6246 2024-04-16 23:01:26.000000 silobuster_test-0.2/README.md
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.771934 silobuster_test-0.2/deduper/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/admin.py
+-rw-r--r--   0 jhom       (502) staff       (20)      140 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/apps.py
+-rw-r--r--   0 jhom       (502) staff       (20)      383 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/asgi.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.823639 silobuster_test-0.2/deduper/deduplicate/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/admin.py
+-rw-r--r--   0 jhom       (502) staff       (20)      154 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/apps.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.829024 silobuster_test-0.2/deduper/deduplicate/migrations/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/migrations/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/models.py
+-rw-r--r--   0 jhom       (502) staff       (20)     6946 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/process_requests.py
+-rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/tests.py
+-rw-r--r--   0 jhom       (502) staff       (20)      387 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/urls.py
+-rw-r--r--   0 jhom       (502) staff       (20)     3424 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/deduplicate/views.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.861953 silobuster_test-0.2/deduper/logs/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       63 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/admin.py
+-rw-r--r--   0 jhom       (502) staff       (20)      140 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/apps.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.867145 silobuster_test-0.2/deduper/logs/migrations/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/migrations/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/models.py
+-rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/tests.py
+-rw-r--r--   0 jhom       (502) staff       (20)      206 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/urls.py
+-rw-r--r--   0 jhom       (502) staff       (20)     2075 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/logs/views.py
+-rwxr-xr-x   0 jhom       (502) staff       (20)      655 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/manage.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.871162 silobuster_test-0.2/deduper/migrations/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/migrations/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)       57 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/models.py
+-rw-r--r--   0 jhom       (502) staff       (20)     4078 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/settings.py
+-rw-r--r--   0 jhom       (502) staff       (20)       60 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/tests.py
+-rw-r--r--   0 jhom       (502) staff       (20)      999 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/urls.py
+-rw-r--r--   0 jhom       (502) staff       (20)     1324 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/views.py
+-rw-r--r--   0 jhom       (502) staff       (20)      391 2024-04-16 23:01:26.000000 silobuster_test-0.2/deduper/wsgi.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.882631 silobuster_test-0.2/libs/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-17 00:12:53.000000 silobuster_test-0.2/libs/__init__.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.901608 silobuster_test-0.2/libs/connector/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-17 00:13:10.000000 silobuster_test-0.2/libs/connector/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)     3065 2024-04-16 23:17:47.000000 silobuster_test-0.2/libs/connector/base_connector.py
+-rw-r--r--   0 jhom       (502) staff       (20)     1449 2024-04-16 23:01:26.000000 silobuster_test-0.2/libs/connector/dataframe_connector.py
+-rw-r--r--   0 jhom       (502) staff       (20)     6855 2024-04-16 23:01:26.000000 silobuster_test-0.2/libs/connector/generic_connector.py
+-rw-r--r--   0 jhom       (502) staff       (20)    17352 2024-04-16 23:40:22.000000 silobuster_test-0.2/libs/connector/postgres_connector.py
+-rw-r--r--   0 jhom       (502) staff       (20)      586 2024-04-16 23:01:26.000000 silobuster_test-0.2/libs/uuid.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.922569 silobuster_test-0.2/manglers/
+-rw-r--r--   0 jhom       (502) staff       (20)       93 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)     1367 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/mangle_org_name.py
+-rw-r--r--   0 jhom       (502) staff       (20)     3860 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/mangle_url.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:28.939994 silobuster_test-0.2/manglers/tests/
+-rw-r--r--   0 jhom       (502) staff       (20)        0 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/tests/__init__.py
+-rw-r--r--   0 jhom       (502) staff       (20)     5417 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/tests/test_mangle_org.py
+-rw-r--r--   0 jhom       (502) staff       (20)     9549 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/tests/test_mangle_url.py
+-rw-r--r--   0 jhom       (502) staff       (20)     1128 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/tests/testing.py
+-rw-r--r--   0 jhom       (502) staff       (20)      978 2024-04-16 23:01:26.000000 silobuster_test-0.2/manglers/tld_swap_prob_dict.py
+-rw-r--r--   0 jhom       (502) staff       (20)       38 2024-04-17 00:16:29.055355 silobuster_test-0.2/setup.cfg
+-rw-r--r--   0 jhom       (502) staff       (20)      425 2024-04-17 00:16:06.000000 silobuster_test-0.2/setup.py
+drwxr-xr-x   0 jhom       (502) staff       (20)        0 2024-04-17 00:16:29.050211 silobuster_test-0.2/silobuster_test.egg-info/
+-rw-r--r--   0 jhom       (502) staff       (20)      138 2024-04-17 00:16:28.000000 silobuster_test-0.2/silobuster_test.egg-info/PKG-INFO
+-rw-r--r--   0 jhom       (502) staff       (20)     1339 2024-04-17 00:16:28.000000 silobuster_test-0.2/silobuster_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jhom       (502) staff       (20)        1 2024-04-17 00:16:28.000000 silobuster_test-0.2/silobuster_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jhom       (502) staff       (20)       13 2024-04-17 00:16:28.000000 silobuster_test-0.2/silobuster_test.egg-info/requires.txt
+-rw-r--r--   0 jhom       (502) staff       (20)       22 2024-04-17 00:16:28.000000 silobuster_test-0.2/silobuster_test.egg-info/top_level.txt
```

### Comparing `silobuster_test-0.1/README.md` & `silobuster_test-0.2/README.md`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/deduplicate/process_requests.py` & `silobuster_test-0.2/deduper/deduplicate/process_requests.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/deduplicate/views.py` & `silobuster_test-0.2/deduper/deduplicate/views.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/logs/views.py` & `silobuster_test-0.2/deduper/logs/views.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/manage.py` & `silobuster_test-0.2/deduper/manage.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/settings.py` & `silobuster_test-0.2/deduper/settings.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/urls.py` & `silobuster_test-0.2/deduper/urls.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/deduper/views.py` & `silobuster_test-0.2/deduper/views.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/mangle_org_name.py` & `silobuster_test-0.2/manglers/mangle_org_name.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/mangle_url.py` & `silobuster_test-0.2/manglers/mangle_url.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/tests/test_mangle_org.py` & `silobuster_test-0.2/manglers/tests/test_mangle_org.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/tests/test_mangle_url.py` & `silobuster_test-0.2/manglers/tests/test_mangle_url.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/tests/testing.py` & `silobuster_test-0.2/manglers/tests/testing.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/manglers/tld_swap_prob_dict.py` & `silobuster_test-0.2/manglers/tld_swap_prob_dict.py`

 * *Files identical despite different names*

### Comparing `silobuster_test-0.1/silobuster_test.egg-info/SOURCES.txt` & `silobuster_test-0.2/silobuster_test.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 deduper/logs/apps.py
 deduper/logs/models.py
 deduper/logs/tests.py
 deduper/logs/urls.py
 deduper/logs/views.py
 deduper/logs/migrations/__init__.py
 deduper/migrations/__init__.py
+libs/__init__.py
+libs/uuid.py
+libs/connector/__init__.py
+libs/connector/base_connector.py
+libs/connector/dataframe_connector.py
+libs/connector/generic_connector.py
+libs/connector/postgres_connector.py
 manglers/__init__.py
 manglers/mangle_org_name.py
 manglers/mangle_url.py
 manglers/tld_swap_prob_dict.py
 manglers/tests/__init__.py
 manglers/tests/test_mangle_org.py
 manglers/tests/test_mangle_url.py
```

