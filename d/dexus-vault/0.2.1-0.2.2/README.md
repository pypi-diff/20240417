# Comparing `tmp/dexus_vault-0.2.1.tar.gz` & `tmp/dexus_vault-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexus_vault-0.2.1.tar", last modified: Mon Apr 15 20:55:33 2024, max compression
+gzip compressed data, was "dexus_vault-0.2.2.tar", last modified: Wed Apr 17 10:05:58 2024, max compression
```

## Comparing `dexus_vault-0.2.1.tar` & `dexus_vault-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/dex_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/vault_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/client_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/dex_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/vault_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/dexus_vault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/client_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/dexus_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/setup.py
```

### Comparing `dexus_vault-0.2.1/LICENSE` & `dexus_vault-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/PKG-INFO` & `dexus_vault-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.1
+Version: 0.2.2
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dexus_vault-0.2.1/README.md` & `dexus_vault-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/__main__.py` & `dexus_vault-0.2.2/dexus_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/client.py` & `dexus_vault-0.2.2/dexus_vault/client.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py` & `dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py` & `dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/src/dex_processor.py` & `dexus_vault-0.2.2/dexus_vault/src/dex_processor.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/src/vault_processor.py` & `dexus_vault-0.2.2/dexus_vault/src/vault_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,18 +81,19 @@
                 )
 
         elif self.config["VAULT_KUBERNETES_ROLE"] is not None:
             # POST /auth/{mount_point}/login
             auth_method = "kubernetes"
 
             with open(self.config["VAULT_KUBERNETES_JWT_PATH"], "r") as jwt:
+                # it is required to have params order mp, role, jwt
                 Kubernetes(client.adapter).login(
-                    role=self.config["VAULT_KUBERNETES_ROLE"],
-                    jwt=jwt,
                     mount_point=self.config["VAULT_KUBERNETES_MOUNT_POINT"],
+                    role=self.config["VAULT_KUBERNETES_ROLE"],
+                    jwt=jwt.read(),
                 )
 
         elif self.config["VAULT_LDAP_USERNAME"] is not None:
             auth_method = "ldap"
             client.auth.ldap.login(
                 username=self.config["VAULT_LDAP_USERNAME"],
                 password=self.config["VAULT_LDAP_PASSWORD"],
```

### Comparing `dexus_vault-0.2.1/dexus_vault/utils/client_parser.py` & `dexus_vault-0.2.2/dexus_vault/utils/client_parser.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/utils/config.py` & `dexus_vault-0.2.2/dexus_vault/utils/config.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/utils/logger.py` & `dexus_vault-0.2.2/dexus_vault/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault/utils/metrics.py` & `dexus_vault-0.2.2/dexus_vault/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/dexus_vault.egg-info/PKG-INFO` & `dexus_vault-0.2.2/dexus_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.1
+Version: 0.2.2
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dexus_vault-0.2.1/dexus_vault.egg-info/SOURCES.txt` & `dexus_vault-0.2.2/dexus_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.1/setup.py` & `dexus_vault-0.2.2/setup.py`

 * *Files identical despite different names*

