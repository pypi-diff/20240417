# Comparing `tmp/tenzir_platform-0.3.1.tar.gz` & `tmp/tenzir_platform-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenzir_platform-0.3.1.tar", max compression
+gzip compressed data, was "tenzir_platform-0.3.2.tar", max compression
```

## Comparing `tenzir_platform-0.3.1.tar` & `tenzir_platform-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/README.md
--rw-r--r--   0        0        0      878 2024-04-16 08:17:04.609817 tenzir_platform-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/auth_rule.py
--rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/cache.py
--rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/client.py
--rw-r--r--   0        0        0      817 2024-04-16 08:17:04.609817 tenzir_platform-0.3.1/tenzir_platform/helpers/environment.py
--rw-r--r--   0        0        0     5908 2024-04-16 08:17:07.433819 tenzir_platform-0.3.1/tenzir_platform/helpers/oidc.py
--rw-r--r--   0        0        0     6232 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/subcommand_admin.py
--rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/subcommand_auth.py
--rw-r--r--   0        0        0     5654 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/subcommand_node.py
--rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.3.1/tenzir_platform/subcommand_workspace.py
--rw-r--r--   0        0        0     1787 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/tenzir_platform.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/README.md
+-rw-r--r--   0        0        0      878 2024-04-17 10:01:10.615745 tenzir_platform-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/auth_rule.py
+-rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/cache.py
+-rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/client.py
+-rw-r--r--   0        0        0      818 2024-04-17 10:00:10.402949 tenzir_platform-0.3.2/tenzir_platform/helpers/environment.py
+-rw-r--r--   0        0        0     5908 2024-04-17 09:59:52.870718 tenzir_platform-0.3.2/tenzir_platform/helpers/oidc.py
+-rw-r--r--   0        0        0     6232 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/subcommand_admin.py
+-rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/subcommand_auth.py
+-rw-r--r--   0        0        0     5654 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/subcommand_node.py
+-rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.3.2/tenzir_platform/subcommand_workspace.py
+-rw-r--r--   0        0        0     1787 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/tenzir_platform.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.3.2/PKG-INFO
```

### Comparing `tenzir_platform-0.3.1/pyproject.toml` & `tenzir_platform-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenzir-platform"
-version = "0.3.1"
+version = "0.3.2"
 description = "Tenzir CLI"
 authors = ["Tenzir <engineering@tenzir.com>"]
 readme = "README.md"
 packages = [{ include = "tenzir_platform" }]
 
 [tool.poetry.scripts]
 tenzir-platform = "tenzir_platform.tenzir_platform:main"
```

### Comparing `tenzir_platform-0.3.1/tenzir_platform/helpers/auth_rule.py` & `tenzir_platform-0.3.2/tenzir_platform/helpers/auth_rule.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/helpers/cache.py` & `tenzir_platform-0.3.2/tenzir_platform/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/helpers/client.py` & `tenzir_platform-0.3.2/tenzir_platform/helpers/client.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/helpers/environment.py` & `tenzir_platform-0.3.2/tenzir_platform/helpers/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic_settings import BaseSettings
 
 
 API_ENDPOINT = "https://rest.tenzir.app/production-v1"
-OIDC_ISSUER_URL = "https://tenzir.eu.auth0.com"
+OIDC_ISSUER_URL = "https://tenzir.eu.auth0.com/"
 OIDC_CLIENT_ID = "vzRh8grIVu1bwutvZbbpBDCOvSzN8AXh"
 
 
 class PlatformEnvironment(BaseSettings):
     # The remote API endpoint of the platform.
     api_endpoint: str = API_ENDPOINT
```

### Comparing `tenzir_platform-0.3.1/tenzir_platform/helpers/oidc.py` & `tenzir_platform-0.3.2/tenzir_platform/helpers/oidc.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/subcommand_admin.py` & `tenzir_platform-0.3.2/tenzir_platform/subcommand_admin.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/subcommand_auth.py` & `tenzir_platform-0.3.2/tenzir_platform/subcommand_auth.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/subcommand_node.py` & `tenzir_platform-0.3.2/tenzir_platform/subcommand_node.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/subcommand_workspace.py` & `tenzir_platform-0.3.2/tenzir_platform/subcommand_workspace.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/tenzir_platform/tenzir_platform.py` & `tenzir_platform-0.3.2/tenzir_platform/tenzir_platform.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.1/PKG-INFO` & `tenzir_platform-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenzir-platform
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tenzir CLI
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

