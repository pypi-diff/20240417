# Comparing `tmp/pasqal-cloud-0.7.0.tar.gz` & `tmp/pasqal_cloud-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.7.0.tar", last modified: Mon Mar 18 12:03:25 2024, max compression
+gzip compressed data, was "pasqal_cloud-0.7.1.tar", last modified: Wed Apr 17 08:19:11 2024, max compression
```

## Comparing `pasqal-cloud-0.7.0.tar` & `pasqal_cloud-0.7.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.787002 pasqal-cloud-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-03-18 12:03:25.787002 pasqal-cloud-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.779002 pasqal-cloud-0.7.0/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.779002 pasqal-cloud-0.7.0/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.779002 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.779002 pasqal-cloud-0.7.0/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/utils/strenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pasqal_cloud/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-03-18 12:03:25.000000 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-18 12:03:25.000000 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:03:25.000000 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-18 12:03:25.000000 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-18 12:03:25.000000 pasqal-cloud-0.7.0/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-18 12:03:25.787002 pasqal-cloud-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19796 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:25.783002 pasqal-cloud-0.7.0/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_project_renaming_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-03-18 12:03:21.000000 pasqal-cloud-0.7.0/tests/test_workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.668271 pasqal_cloud-0.7.1/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pasqal_cloud/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-17 08:19:11.000000 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-17 08:19:11.000000 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:19:11.000000 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 08:19:11.000000 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 08:19:11.000000 pasqal_cloud-0.7.1/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.672271 pasqal_cloud-0.7.1/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:11.676271 pasqal_cloud-0.7.1/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_project_renaming_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-17 08:19:07.000000 pasqal_cloud-0.7.1/tests/test_workload.py
```

### Comparing `pasqal-cloud-0.7.0/LICENSE` & `pasqal_cloud-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/PKG-INFO` & `pasqal_cloud-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.7.0
+Version: 0.7.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
-Requires-Dist: pydantic<2.0,>=1.10
+Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
-Requires-Dist: mypy==0.982; extra == "dev"
-Requires-Dist: isort==5.12.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: pytest==7.4.0; extra == "dev"
-Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: types-requests==2.31.0.1; extra == "dev"
 Requires-Dist: requests-mock==1.11.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: types-requests==2.31.0.1; extra == "dev"
+Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal-cloud-0.7.0/README.md` & `pasqal_cloud-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/__init__.py` & `pasqal_cloud-0.7.1/pasqal_cloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from datetime import datetime
 import time
-from requests.exceptions import HTTPError
+from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 from warnings import warn
 
+from requests.exceptions import HTTPError
+
 from pasqal_cloud.authentication import TokenProvider
 from pasqal_cloud.batch import Batch, RESULT_POLLING_INTERVAL
 from pasqal_cloud.client import Client, EmptyFilter
 from pasqal_cloud.device import BaseConfig, EmulatorType
 from pasqal_cloud.endpoints import (  # noqa: F401
     AUTH0_CONFIG,
     Auth0Conf,
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/_version.py` & `pasqal_cloud-0.7.1/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/authentication.py` & `pasqal_cloud-0.7.1/pasqal_cloud/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TokenProviderError(Exception):
     pass
 
 
 class TokenProvider(ABC):
-    def __init__(self, *args: list[Any], **kwargs: dict):
-        ...
+    def __init__(self, *args: list[Any], **kwargs: dict): ...
 
     @abstractmethod
     def get_token(self) -> str:
         raise NotImplementedError
 
 
 class ExpiringTokenProvider(TokenProvider, ABC):
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/batch.py` & `pasqal_cloud-0.7.1/pasqal_cloud/batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 from warnings import warn
 
-from pydantic import BaseModel, Extra, root_validator, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    field_validator,
+    model_validator,
+    PrivateAttr,
+    ValidationInfo,
+)
 from requests import HTTPError
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import EmulatorType
 from pasqal_cloud.device.configuration import BaseConfig, EmuFreeConfig, EmuTNConfig
 from pasqal_cloud.errors import (
+    BatchCancellingError,
     BatchFetchingError,
     BatchSetCompleteError,
-    BatchCancellingError,
     JobCreationError,
-    JobFetchingError,
     JobRetryError,
 )
 from pasqal_cloud.job import CreateJob, Job
 
 RESULT_POLLING_INTERVAL = 2  # seconds
 
 
 class Batch(BaseModel):
     """Class to load batch data return by the API.
 
     A batch groups up several jobs with the same sequence. When a batch is assigned to
-    a QPU, all its jobs are ran sequentially and no other batch can be assigned to the
+    a QPU, all its jobs are run sequentially and no other batch can be assigned to the
     device until all its jobs are done and declared complete.
 
     Attributes:
         - complete: Whether the batch has been declared as complete.
         - created_at: Timestamp of the creation of the batch.
         - updated_at: Timestamp of the last update of the batch.
         - device_type: Type of device to run the batch on.
@@ -59,70 +65,81 @@
     updated_at: str
     device_type: str
     project_id: str
     id: str
     user_id: str
     priority: int
     status: str
-    webhook: Optional[str]
-    _client: Client
+    _client: Client = PrivateAttr(default=None)
     sequence_builder: str
-    start_datetime: Optional[str]
-    end_datetime: Optional[str]
-    device_status: Optional[str]
     ordered_jobs: List[Job] = []
     jobs_count: int = 0
     jobs_count_per_status: Dict[str, int] = {}
+    webhook: Optional[str] = None
+    start_datetime: Optional[str] = None
+    end_datetime: Optional[str] = None
+    device_status: Optional[str] = None
     parent_id: Optional[str] = None
     configuration: Union[BaseConfig, Dict[str, Any], None] = None
 
-    class Config:
-        extra = Extra.allow
-        arbitrary_types_allowed = True
-
-    @root_validator(pre=True)
-    def _build_ordered_jobs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """This root validator will modify the 'jobs' attribute which is a list
+    model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
+
+    def __init__(self, **data: Any) -> None:
+        """
+        Workaround to make the private attribute '_client' working
+        like we need with Pydantic V2, more information on:
+        https://docs.pydantic.dev/latest/concepts/models/#private-model-attributes
+        """
+        super().__init__(**data)
+        self._client = data["_client"]
+
+    @model_validator(mode="before")
+    def _build_ordered_jobs(cls, data: Dict[str, Any]) -> Dict[str, Any]:
+        """This root validator will modify the 'jobs' attribute, which is a list
         of jobs dictionaries ordered by creation time before instantiation.
         It will duplicate the value of 'jobs' in a new attribute 'ordered_jobs'
         to keep the jobs ordered by creation time.
         """
-        ordered_jobs_list = []
-        jobs_received = values.get("jobs", [])
-        for job in jobs_received:
-            job_dict = {**job, "_client": values["_client"]}
-            ordered_jobs_list.append(job_dict)
-        values["ordered_jobs"] = ordered_jobs_list
-        return values
+        jobs_received = data.get("jobs", [])
+        data["ordered_jobs"] = [
+            {**job, "_client": data["_client"]} for job in jobs_received
+        ]
+        return data
 
     # Ticket (#704), to be removed or updated
     @property
     def jobs(self) -> Dict[str, Job]:
         """Once the 'ordered_jobs' is built, we need to keep the 'jobs' attribute
         for backward compatibility with the code written by the users of the sdk
         """
         warn(
             "'jobs' attribute is deprecated, use 'ordered_jobs' instead",
             DeprecationWarning,
             stacklevel=1,
         )
         return {job.id: job for job in self.ordered_jobs}
 
-    @validator("configuration", pre=True)
+    @jobs.setter
+    def jobs(self, _: Any) -> None:
+        # Override the jobs setter to be a no-op.
+        # `jobs` is a read-only attribute which is derived from the `ordered_jobs` key.
+        pass
+
+    @field_validator("configuration", mode="before")
     def _load_configuration(
         cls,
         configuration: Union[Dict[str, Any], BaseConfig, None],
-        values: Dict[str, Any],
+        info: ValidationInfo,
     ) -> Optional[BaseConfig]:
         if not isinstance(configuration, dict):
             return configuration
         conf_class: Type[BaseConfig] = BaseConfig
-        if values["device_type"] == EmulatorType.EMU_TN.value:
+        if info.data["device_type"] == EmulatorType.EMU_TN.value:
             conf_class = EmuTNConfig
-        elif values["device_type"] == EmulatorType.EMU_FREE.value:
+        elif info.data["device_type"] == EmulatorType.EMU_FREE.value:
             conf_class = EmuFreeConfig
         return conf_class.from_dict(configuration)
 
     def add_jobs(
         self,
         jobs: List[CreateJob],
         wait: bool = False,
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/client.py` & `pasqal_cloud-0.7.1/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/base_config.py` & `pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal_cloud-0.7.1/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/endpoints.py` & `pasqal_cloud-0.7.1/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/errors.py` & `pasqal_cloud-0.7.1/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/job.py` & `pasqal_cloud-0.7.1/pasqal_cloud/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Optional, TypedDict, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 from requests import HTTPError
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.errors import JobCancellingError
 
 
 class Job(BaseModel):
@@ -33,30 +33,37 @@
     """
 
     runs: int
     batch_id: str
     id: str
     project_id: str
     status: str
-    _client: Client
+    _client: Client = PrivateAttr(default=None)
     created_at: str
     updated_at: str
     errors: Optional[List[str]] = None
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
     full_result: Optional[Dict[str, Any]] = None
     variables: Optional[Dict[str, Any]] = None
     # Ticket (#622)
     group_id: Optional[str] = None
     parent_id: Optional[str] = None
 
-    class Config:
-        extra = Extra.allow
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
+
+    def __init__(self, **data: Any) -> None:
+        """
+        Workaround to make the private attribute '_client' working
+        like we need with Pydantic V2, more information on:
+        https://docs.pydantic.dev/latest/concepts/models/#private-model-attributes
+        """
+        super().__init__(**data)
+        self._client = data["_client"]
 
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current job on the PCS."""
         try:
             job_rsp = self._client._cancel_job(self.id)
         except HTTPError as e:
             raise JobCancellingError(e) from e
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/utils/jsend.py` & `pasqal_cloud-0.7.1/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud/workload.py` & `pasqal_cloud-0.7.1/pasqal_cloud/workload.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 import requests
-from pydantic import BaseModel, Extra, validator
+from pydantic import BaseModel, ConfigDict, field_validator, PrivateAttr
+from pydantic_core.core_schema import ValidationInfo
 from requests import HTTPError
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.errors import (
     InvalidWorkloadResultsFormatError,
     WorkloadCancellingError,
     WorkloadResultsConnectionError,
@@ -37,44 +38,53 @@
         - end_timestamp: The timestamp of when the workload finished processing.
         - result: Result of the workload.
     """
 
     id: str
     project_id: str
     status: str
-    _client: Client
+    _client: Client = PrivateAttr(default=None)
     backend: str
     workload_type: str
     config: Dict[str, Any]
     created_at: str
     updated_at: str
     errors: Optional[List[str]] = None
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result_link: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
 
-    class Config:
-        extra = Extra.allow
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(
+        extra="allow", arbitrary_types_allowed=True, validate_default=True
+    )
+
+    def __init__(self, **data: Any) -> None:
+        """
+        Workaround to make the private attribute '_client' working
+        like we need with Pydantic V2, more information on:
+        https://docs.pydantic.dev/latest/concepts/models/#private-model-attributes
+        """
+        super().__init__(**data)
+        self._client = data["_client"]
 
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current job on the PCS."""
         try:
             workload_rsp = self._client._cancel_workload(self.id)
         except HTTPError as e:
             raise WorkloadCancellingError(e) from e
         self.status = workload_rsp.get("status", "CANCELED")
         return workload_rsp
 
-    @validator("result", always=True)
+    @field_validator("result")
     def result_link_to_result(
-        cls, result: Optional[Dict[str, Any]], values: Dict[str, Any]
+        cls, result: Optional[Dict[str, Any]], info: ValidationInfo
     ) -> Optional[Dict[str, Any]]:
-        result_link: Optional[str] = values.get("result_link")
+        result_link: Optional[str] = info.data.get("result_link")
         if result or not result_link:
             return result
         try:
             res = requests.get(result_link)
         except HTTPError as e:
             raise WorkloadResultsDownloadError(e) from e
         except requests.ConnectionError as e:
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud.egg-info/PKG-INFO` & `pasqal_cloud-0.7.1/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.7.0
+Version: 0.7.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
-Requires-Dist: pydantic<2.0,>=1.10
+Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
-Requires-Dist: mypy==0.982; extra == "dev"
-Requires-Dist: isort==5.12.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: pytest==7.4.0; extra == "dev"
-Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: types-requests==2.31.0.1; extra == "dev"
 Requires-Dist: requests-mock==1.11.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: types-requests==2.31.0.1; extra == "dev"
+Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal-cloud-0.7.0/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal_cloud-0.7.1/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/sdk/setup.py` & `pasqal_cloud-0.7.1/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/setup.py` & `pasqal_cloud-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/pasqal-cloud",
     install_requires=[
         "auth0-python >= 3.23.1, <4.0.0",
         "requests>=2.25.1, <3.0.0",
         "pyjwt[crypto]>=2.5.0, <3.0.0",
-        "pydantic>=1.10, <2.0",
+        "pydantic >= 2.6.0, <3.0.0",
     ],
     extras_require={
         "dev": {
             "black==23.3.0",
             "flake8==6.0.0",
             "isort==5.12.0",
-            "mypy==0.982",
+            "mypy==1.9.0",
             "pytest==7.4.0",
             "pytest-cov==4.1.0",
             "types-requests==2.31.0.1",
             "requests-mock==1.11.0",
         }
     },
 )
```

### Comparing `pasqal-cloud-0.7.0/tests/conftest.py` & `pasqal_cloud-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_batch.py` & `pasqal_cloud-0.7.1/tests/test_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     def test_batch_instantiation_with_extra_field(self, batch):
         """Instantiating a batch with an extra field should not raise an error.
 
         This enables us to add new fields in the API response on the batches endpoint
         without breaking compatibility for users with old versions of the SDK where
         the field is not present in the Batch class.
         """
-        batch_dict = batch.dict()  # Batch data expected by the SDK
+        batch_dict = batch.model_dump()  # Batch data expected by the SDK
         # We add an extra field to mimick the API exposing new values to the user
         batch_dict["new_field"] = "any_value"
 
         new_batch = Batch(**batch_dict)  # this should raise no error
         assert (
             new_batch.new_field == "any_value"
         )  # The new value should be stored regardless
```

### Comparing `pasqal-cloud-0.7.0/tests/test_client.py` & `pasqal_cloud-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_cloud_sdk_import.py` & `pasqal_cloud-0.7.1/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_config.py` & `pasqal_cloud-0.7.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_device_specs.py` & `pasqal_cloud-0.7.1/tests/test_device_specs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.sdk = SDK(
             username="me@test.com", password="password", project_id=str(uuid4())
         )
 
     @pytest.mark.usefixtures("mock_request")
     def test_get_device_specs_success(self):
         device_specs_dict = self.sdk.get_device_specs_dict()
-        assert type(device_specs_dict) == dict
+        assert isinstance(device_specs_dict, dict)
         specs = device_specs_dict["FRESNEL"]
         json.loads(specs)
 
     def test_get_device_specs_error(self, mock_request_exception):
         with pytest.raises(DeviceSpecsFetchingError):
             _ = self.sdk.get_device_specs_dict()
         assert mock_request_exception.last_request.method == "GET"
```

### Comparing `pasqal-cloud-0.7.0/tests/test_doubles/authentication.py` & `pasqal_cloud-0.7.1/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_errors.py` & `pasqal_cloud-0.7.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_job.py` & `pasqal_cloud-0.7.1/tests/test_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def test_job_instantiation_with_extra_field(self, job):
         """Instantiating a job with an extra field should not raise an error.
 
         This enables us to add new fields in the API response on the jobs endpoint
         without breaking compatibility for users with old versions of the SDK where
         the field is not present in the Job class.
         """
-        job_dict = job.dict()  # job data expected by the SDK
+        job_dict = job.model_dump()  # job data expected by the SDK
         # We add an extra field to mimick the API exposing new values to the user
         job_dict["new_field"] = "any_value"
 
         new_job = Job(**job_dict)  # this should raise no error
         assert (
             new_job.new_field == "any_value"
         )  # The new value should be stored regardless
```

### Comparing `pasqal-cloud-0.7.0/tests/test_project_renaming_compatibility.py` & `pasqal_cloud-0.7.1/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.7.0/tests/test_workload.py` & `pasqal_cloud-0.7.1/tests/test_workload.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,38 +166,38 @@
     def test_workload_instantiation_with_extra_field(self, workload):
         """Instantiating a workload with an extra field should not raise an error.
 
         This enables us to add new fields in the API response on the workloads endpoint
         without breaking compatibility for users with old versions of the SDK where
         the field is not present in the Batch class.
         """
-        workload_dict = workload.dict()  # Batch data expected by the SDK
+        workload_dict = workload.model_dump()  # Batch data expected by the SDK
         # We add an extra field to mimick the API exposing new values to the user
         workload_dict["new_field"] = "any_value"
 
         new_workload = Workload(**workload_dict)  # this should raise no error
         assert (
             new_workload.new_field == "any_value"
         )  # The new value should be stored regardless
 
     def test_workload_result_raise_connection_error(self, workload):
         """
-        Check that error is raised when improper url is set.
+        Check that error is raised when an improper url is set.
         """
-        workload_dict = workload.dict()
+        workload_dict = workload.model_dump()
         workload_dict.pop("result")
         workload_dict["result_link"] = "http://test.test"
         with pytest.raises(WorkloadResultsConnectionError):
             Workload(**workload_dict)
 
     def tests_workload_result_set(self, workload):
         """
         Check that result is set when only result_link is provided.
         """
-        workload_dict = workload.dict()
+        workload_dict = workload.model_dump()
         workload_dict.pop("result")
         workload_dict["result_link"] = "http://test.test"
         resp = requests.Response()
         resp._content = json.dumps({"some": "data"}).encode("utf-8")
         with patch("requests.get", lambda x: resp):
             res = Workload(**workload_dict)
         assert res.result == {"some": "data"}
```

