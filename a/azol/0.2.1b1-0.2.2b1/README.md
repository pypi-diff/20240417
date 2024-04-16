# Comparing `tmp/azol-0.2.1b1.tar.gz` & `tmp/azol-0.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azol-0.2.1b1.tar", last modified: Sun Apr  7 16:39:05 2024, max compression
+gzip compressed data, was "azol-0.2.2b1.tar", last modified: Tue Apr 16 22:16:19 2024, max compression
```

## Comparing `azol-0.2.1b1.tar` & `azol-0.2.2b1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-07 16:38:56.000000 azol-0.2.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-07 16:39:05.706318 azol-0.2.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 16:38:56.000000 azol-0.2.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.698318 azol-0.2.1b1/azol/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.698318 azol-0.2.1b1/azol/caches/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/azol_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/in_memory_token_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/local_token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43193 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/arm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/graph_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/key_vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/oauth_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/application_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/entraid_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/models/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/generic_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/sp_login_init_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/file_secret_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/key_vault_secret_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/graph_delegated_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/graph_permissions_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/rbac_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/services/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35337 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/services/token_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-07 16:38:56.000000 azol-0.2.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:39:05.706318 azol-0.2.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 16:38:56.000000 azol-0.2.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.431204 azol-0.2.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-16 22:16:08.000000 azol-0.2.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 22:16:19.427204 azol-0.2.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 22:16:08.000000 azol-0.2.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/azol_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/in_memory_token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/local_token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/arm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/graph_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/key_vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/oauth_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/application_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/entraid_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/generic_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/sp_login_init_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/file_secret_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/key_vault_secret_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/graph_delegated_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/graph_permissions_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/rbac_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44361 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/token_service_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 22:16:08.000000 azol-0.2.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:16:19.431204 azol-0.2.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 22:16:08.000000 azol-0.2.2b1/setup.py
```

### Comparing `azol-0.2.1b1/LICENSE` & `azol-0.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/PKG-INFO` & `azol-0.2.2b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.1b1
+Version: 0.2.2b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.1b1/README.md` & `azol-0.2.2b1/README.md`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/__init__.py` & `azol-0.2.2b1/azol/__init__.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/caches/azol_cache.py` & `azol-0.2.2b1/azol/caches/azol_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,28 +57,30 @@
             for s in scopes:
                 if s not in token_data["scopes"]:
                     token_found=False
             if token_found:
                 return token_data
 
     def cache_or_update(self, access_token, tenant_id, client_id, default_scope, scopes,
-                        oauth_resource, refresh_token=None, username=None):
+                        oauth_resource, refresh_token=None, username=None, 
+                        ests_cookie=None, ests_persistent_cookie=None):
         """
             Saves an access and refresh token to the cache, or updates an existing entry
 
              Args:
                 - access_token: string - an OAuth2 access token to cache
                 - tenant_id: string - the tenant Id that issued the token
                 - client_id: string - the Azure service principal client Id to fetch a token for
                 - default_scope: bool - if true, use the default scope for the resource
                 - scopes: list - a list of scopes to be issued in the token
                 - oauth_resource: string - the OAuth resource issued in the token.
                 - refresh_token: string - refresh token to cache
                 - username: string - optional. The username that should be issued in the token
-
+                - ests_cookie: string - optional. ests cookie to cache
+                
             Returns:
                 Null
         """
         if default_scope:
             scopes=[DEFAULTSCOPE]
         if tenant_id not in self.tokens.keys():
             self.tokens[ tenant_id ] = {}
@@ -132,11 +134,13 @@
             }
         else:
             new_token = {
                 "type": "delegated",
                 "scopes":scopes,
                 "username":username,
                 "access_token": access_token,
-                "refresh_token": refresh_token
+                "refresh_token": refresh_token,
+                "ests_cookie": ests_cookie,
+                "ests_persistent_cookie": ests_persistent_cookie
             }
         self.tokens[ tenant_id ][ oauth_resource ][ client_id ].append(new_token)
```

### Comparing `azol-0.2.1b1/azol/caches/local_token_cache.py` & `azol-0.2.2b1/azol/caches/local_token_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/clients/arm_client.py` & `azol-0.2.2b1/azol/clients/arm_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -868,14 +868,24 @@
                           "Raw error: %s", response.status_code, scope,
                           response.content )
             raise ArmRequestFailedException()
 
         deployments = response.json()
         return deployments
 
+    def get_current_user_pim_eligibility(self, scope):
+        response = self._send_request( f"{scope}/providers/Microsoft.Authorization/roleEligibilityScheduleInstances",
+                                       query_parameters={ "api-version": "2020-10-01",
+                                                         "$filter": "asTarget()"},
+                                       method="GET" )
+
+
+        roles = response.json()
+        return roles
+
     def get_descendants( self, management_group ):
         """Get direct descendants of a management group.
 
         This function will return subscriptions or management groups that are nested under
         the management group.
         
         Args:
@@ -963,15 +973,15 @@
 
         """
         arm_raw_response = self._send_request( path, method="PATCH",
                                               query_parameters={ "api-version": api_version},
                                               json=data )
         return arm_raw_response.json()
 
-    def get( self, path, api_version ):
+    def get( self, path, api_version=None ):
         """Send a GET request to ARM, and return the raw results
 
         Calls ARM at the path specified, and returns the raw deserialized results.
         
         Args:
             path - (str) The API path to call on ARM
             api_version - (str) The api-version to call for the ARM API
@@ -979,19 +989,39 @@
         Returns:
             A dictionary containing the raw results from the ARM request.
 
         Raises:
             ArmRequestFailedException: An error occurred accessing the ARM API
 
         """
+        if "/providers" not in path:
+            namespace="microsoft.resources"
+            provider=path.split("/")[1]
+        else:    
+            namespace_and_provider=path.split('/providers/')[-1]
+            namespace_and_provider_list=namespace_and_provider.split("/")
+            namespace = namespace_and_provider_list[0].lower()
+            provider_and_resource = "/".join(namespace_and_provider_list[1:])
+            matching_providers=[]
+            for provider in self.providers[namespace].keys():
+                if provider in provider_and_resource:
+                    matching_providers.append(provider)
+            
+            provider=max(p for p in matching_providers)
+            logging.info("Resolved namespace to ", namespace)
+            logging.info("Resolved provider to ", provider)
+
+        provider_versions=self.providers[namespace][provider]
+        latest=provider_versions[0]
+        logging.info("Resolved latest provider version to ", latest)
+        api_version = latest
         arm_raw_response = self._send_request( path,
-                                              query_parameters={ "api-version": api_version} )
+            query_parameters={ "api-version": api_version} )
         return arm_raw_response.json()
 
-    
     def delete( self, path ):
         """Make a DELETE request to a specific API path within the ARM API.
 
         Args:
             - path - (string) The ARM API path.
 
         Returns:
```

### Comparing `azol-0.2.1b1/azol/clients/graph_client.py` & `azol-0.2.2b1/azol/clients/graph_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/clients/key_vault_client.py` & `azol-0.2.2b1/azol/clients/key_vault_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/clients/oauth_http_client.py` & `azol-0.2.2b1/azol/clients/oauth_http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from azol.credentials import User
 
 class OAuthHTTPClient:
     """
         Base class for OAuth HTTP client objects.
     """
 
-    def __init__( self, tenant, oauth_resource, base_url,
-                  cred, azol_id=None, oauth_flow=None, secrets_provider=None,
+    def __init__( self, cred, oauth_resource, base_url,
+                  tenant=None, azol_id=None, oauth_flow=None, secrets_provider=None,
                   use_persistent_cache=True, auto_refresh=True):
+        if tenant is None:
+            if cred.credentialType != "user":
+                raise Exception("tenant must be specified if credential is not of type 'user'")
+            if not cred.default_oauth_flow=="refresh_token":
+                username=cred.get_username()
+                tenant=username.split("@")[1]
         self.scopes=[]
         self.default_scope=True
         self.profile_scope=True
         self.openid_scope=True
         self.offline_access_scope=True
         self._baseurl = base_url
-        # get the tenant Id if its a domain name. If it cant be parsed as a guid, its a domain name.
-        try:
-            uuid.UUID(tenant, version=4)
-        except ValueError:
-            tenant=get_tenant_id(tenant)
 
         self._tenant = tenant
         self._resource = oauth_resource
         self._current_token = None
 
         # if no specific oauth flow is provided, get the default from the credential
         if oauth_flow is None:
@@ -167,14 +168,17 @@
                 raw ascii representation of the current token or None if no token is saved
         """
         if self._current_token is None:
             return None
 
         return self._current_token
 
+    def get_client_id( self ):
+        return self.token_service.get_client_id()
+
     def switch_client(self, client_id):
         """
             Switch the oauth client used by the HTTP Client. Used to abuse FOCI functionality.
 
             nullifies current cached access token, but leaves refresh token in client.
 
             Vars:
@@ -182,14 +186,37 @@
 
             Returns:
                 OAuthHTTPClient subclass
         """
         self._current_token = None
         self.token_service.switch_client(client_id)
 
+    @classmethod
+    def from_client(cls, client, *args, **kwargs):
+        """
+            Generate a new HTTP Client with a different OAuth Resource, using the current client class.
+
+            Use this class to switch from, for example, a GraphClient to an ArmClient.
+            Nullifies current cached access token, but leaves refresh token in client.
+
+            Note: alternative to "refresh_to_new_resource" of an active client, but results in the same.
+
+            Vars:
+                - client - OAuthHTTP child class that will be used to instantiate the 
+                              new class. Note that this must be a valid
+                              OAuth HTTP child class. For example, ArmClient, GraphClient,
+                              or KeyVaultClient
+
+            Returns:
+                OAuthHTTPClient subclass instance
+        """
+        rt = client.get_current_refresh_token()
+        user = User(refresh_token=rt, client_id=client.get_client_id())
+        newClass = cls(*args, tenant=client._tenant, cred=user, **kwargs)
+        return newClass
 
     def refresh_to_new_resource(self, oauth_http_client_class):
         """
             Generate a new HTTP Client with a different OAuth Resource, using the current token.
 
             Use this class to switch from, for example, a GraphClient to an ArmClient.
             Nullifies current cached access token, but leaves refresh token in client.
```

### Comparing `azol-0.2.1b1/azol/constants.py` & `azol-0.2.2b1/azol/constants.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/credentials/access_token.py` & `azol-0.2.2b1/azol/credentials/access_token.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/credentials/application_object.py` & `azol-0.2.2b1/azol/credentials/application_object.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/credentials/credential.py` & `azol-0.2.2b1/azol/credentials/credential.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,22 +37,14 @@
         """
             Get the current client id set in the credential.
     
             Returns: A string containing the client id
         """
         return self._client_id
 
-    def set_client_id( self, client_id ):
-        """
-            Set the current client id set in the credential.
-    
-            Returns: None
-        """
-        self._client_id=client_id
-
     def get_username( self ):
         """
             Get the username of the user object
 
             Returns: A string containing the username of the credential
         """
         if self._username is not None:
```

### Comparing `azol-0.2.1b1/azol/credentials/service_principal.py` & `azol-0.2.2b1/azol/credentials/service_principal.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/credentials/user.py` & `azol-0.2.2b1/azol/credentials/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     """
         A credential object that may be used when a refresh token is stolen, 
         or a username/password combo is stolen
     """
 
     supportedOAuthFlows = [ "refresh_token", "device_code", "authorization_code" ]
     credentialType="user"
-    default_oauth_flow="authorization_code"
+    default_oauth_flow="device_code"
 
     def __init__( self, username=None, refresh_token=None,
-                  client_id=FOCIClients.AzurePortal,
-                  redirect_uri=known_client_redirect_uris[FOCIClients.AzurePortal], 
+                  client_id=FOCIClients.MicrosoftAzurePowershell,
+                  redirect_uri=None, 
                   *args, **kwargs ):
         """
             User objects always have a username, pasword and refresh token. 
             However, sometimes some or all of these are unknown
             during a test. Accept any combo except for password only, 
             and if none are provided, ask the user.
         """
```

### Comparing `azol-0.2.1b1/azol/models/generic_resource.py` & `azol-0.2.2b1/azol/models/generic_resource.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/providers/file_secret_provider.py` & `azol-0.2.2b1/azol/providers/file_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/providers/key_vault_secret_provider.py` & `azol-0.2.2b1/azol/providers/key_vault_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/resources/graph_delegated_permissions.py` & `azol-0.2.2b1/azol/resources/graph_delegated_permissions.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/resources/graph_permissions_map.py` & `azol-0.2.2b1/azol/resources/graph_permissions_map.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/resources/rbac_roles.py` & `azol-0.2.2b1/azol/resources/rbac_roles.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol/utils/auth_utils.py` & `azol-0.2.2b1/azol/utils/auth_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Module that contains functions that are useful when working with Entra ID and Azure"""
 import logging
 import json
 import requests
 from azol.utils import string_between
 from azol.models.sp_login_init_model import SPLoginModel
 
-def start_azure_portal_login():
+def start_azure_portal_login(*args):
     # get a nonce cookie from portal, and have the portal initiate a login flow
-    resp=requests.get("https://portal.azure.com/signin/idpRedirect.js/?sessionId=cb357678cb1c4365a9a8fa8a0de9718a&feature.argsubscriptions=true&feature.showservicehealthalerts=true&feature.prefetchtokens=true&feature.internalgraphapiversion=true&feature.selftoken=true&feature.globalresourcefilter=true&feature.msaljs=true&feature.fetchpolicyforrestypes=true&feature.testcrosscloudpuid=true&feature.useredirecthint=true&feature.usetenanthint=true&idpc=0&savedDefaultDirectory=f01eea3a-026a-4680-be79-da5fe4842a3d")
+    resp=requests.get("https://portal.azure.com/signin/idpRedirect.js/?feature.argsubscriptions=true&feature.showservicehealthalerts=true&feature.prefetchtokens=true&feature.internalgraphapiversion=true&feature.selftoken=true&feature.globalresourcefilter=true&feature.msaljs=true&feature.fetchpolicyforrestypes=true&feature.testcrosscloudpuid=true&feature.useredirecthint=true&feature.usetenanthint=true&idpc=0")
 
     # Save Portal cookies for later - required when finishing login flow
     portalCookies=resp.cookies
 
     # Extract portal redirect URL
     portalRedirectUrl=string_between(resp.text, "https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize", "\")", include_start=True)
```

### Comparing `azol-0.2.1b1/azol/utils/utils.py` & `azol-0.2.2b1/azol/utils/utils.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.1b1/azol.egg-info/PKG-INFO` & `azol-0.2.2b1/azol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.1b1
+Version: 0.2.2b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.1b1/azol.egg-info/SOURCES.txt` & `azol-0.2.2b1/azol.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,10 +33,11 @@
 azol/providers/key_vault_secret_provider.py
 azol/resources/__init__.py
 azol/resources/graph_delegated_permissions.py
 azol/resources/graph_permissions_map.py
 azol/resources/rbac_roles.py
 azol/services/__init__.py
 azol/services/token_service.py
+azol/services/token_service_helpers.py
 azol/utils/__init__.py
 azol/utils/auth_utils.py
 azol/utils/utils.py
```

### Comparing `azol-0.2.1b1/setup.py` & `azol-0.2.2b1/setup.py`

 * *Files identical despite different names*

