# Comparing `tmp/dj_tenants-0.1.0.tar.gz` & `tmp/dj_tenants-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_tenants-0.1.0.tar", max compression
+gzip compressed data, was "dj_tenants-0.1.1.tar", max compression
```

## Comparing `dj_tenants-0.1.0.tar` & `dj_tenants-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      213 2024-04-16 04:46:19.604445 dj_tenants-0.1.0/dj_tenants/__init__.py
--rw-r--r--   0        0        0      173 2024-04-16 03:25:30.163212 dj_tenants-0.1.0/dj_tenants/apps.py
--rw-r--r--   0        0        0        0 2024-04-16 04:44:50.371217 dj_tenants-0.1.0/dj_tenants/cache.py
--rw-r--r--   0        0        0      977 2024-04-16 04:25:36.290417 dj_tenants-0.1.0/dj_tenants/context.py
--rw-r--r--   0        0        0       41 2024-04-16 04:24:47.367391 dj_tenants-0.1.0/dj_tenants/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-16 04:44:41.967033 dj_tenants-0.1.0/dj_tenants/log.py
--rw-r--r--   0        0        0     1330 2024-04-16 04:28:12.561056 dj_tenants-0.1.0/dj_tenants/models.py
--rw-r--r--   0        0        0        0 2024-04-16 04:42:05.475683 dj_tenants-0.1.0/dj_tenants/storage.py
--rw-r--r--   0        0        0      606 2024-04-16 04:13:41.697387 dj_tenants-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.0/README.md
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1148 2024-04-16 21:50:11.453241 dj_tenants-0.1.1/dj_tenants/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-16 10:59:47.143776 dj_tenants-0.1.1/dj_tenants/apps.py
+-rw-r--r--   0        0        0      288 2024-04-16 22:10:43.102058 dj_tenants-0.1.1/dj_tenants/conf.py
+-rw-r--r--   0        0        0      996 2024-04-16 10:44:41.535837 dj_tenants-0.1.1/dj_tenants/context.py
+-rw-r--r--   0        0        0       46 2024-04-16 10:06:02.548359 dj_tenants-0.1.1/dj_tenants/exceptions.py
+-rw-r--r--   0        0        0     1496 2024-04-16 22:10:43.102058 dj_tenants-0.1.1/dj_tenants/middleware.py
+-rw-r--r--   0        0        0     1295 2024-04-16 21:18:08.416811 dj_tenants-0.1.1/dj_tenants/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:29:02.214763 dj_tenants-0.1.1/dj_tenants/postgres_backend/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-16 11:55:58.663429 dj_tenants-0.1.1/dj_tenants/postgres_backend/base.py
+-rw-r--r--   0        0        0     3666 2024-04-16 21:17:16.930323 dj_tenants-0.1.1/dj_tenants/postgres_backend/compiler.py
+-rw-r--r--   0        0        0      224 2024-04-16 11:55:44.287371 dj_tenants-0.1.1/dj_tenants/postgres_backend/operations.py
+-rw-r--r--   0        0        0      819 2024-04-16 14:33:07.299762 dj_tenants-0.1.1/dj_tenants/utils.py
+-rw-r--r--   0        0        0      606 2024-04-16 22:11:06.092489 dj_tenants-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.1/README.md
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.1/PKG-INFO
```

### Comparing `dj_tenants-0.1.0/dj_tenants/context.py` & `dj_tenants-0.1.1/dj_tenants/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from contextlib import contextmanager
 from contextvars import ContextVar
 
-from dj_tenants.exceptions import TenantError
+from dj_tenants.exceptions import TenantNotDefined
 
 state_local = ContextVar(
     "tenant-state",
     default={
         "enabled": True,
         "tenant": None,
     },
 )
 
 
-def get_state():
+def get_dj_state():
     state = state_local.get()
     return state
 
 
 def get_current_tenant():
-    state = get_state()
+    state = get_dj_state()
 
     if state["enabled"] and state["tenant"] is None:
-        raise TenantError("Tenant is required in context.")
+        raise TenantNotDefined("Tenant is required in context.")
 
     return state["tenant"]
 
 
 @contextmanager
 def tenant_context(tenant=None, enabled=True):
-    previous_state = get_state()
+    previous_state = get_dj_state()
 
     new_state = previous_state.copy()
     new_state["enabled"] = enabled
     new_state["tenant"] = tenant
 
     state_local.set(new_state)
```

### Comparing `dj_tenants-0.1.0/pyproject.toml` & `dj_tenants-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-tenants"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Hugo Mesquita <hugohomesquita@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "dj_tenants" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

