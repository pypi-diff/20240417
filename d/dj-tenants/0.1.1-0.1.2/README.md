# Comparing `tmp/dj_tenants-0.1.1.tar.gz` & `tmp/dj_tenants-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_tenants-0.1.1.tar", max compression
+gzip compressed data, was "dj_tenants-0.1.2.tar", max compression
```

## Comparing `dj_tenants-0.1.1.tar` & `dj_tenants-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1148 2024-04-16 21:50:11.453241 dj_tenants-0.1.1/dj_tenants/__init__.py
--rw-r--r--   0        0        0      411 2024-04-16 10:59:47.143776 dj_tenants-0.1.1/dj_tenants/apps.py
--rw-r--r--   0        0        0      288 2024-04-16 22:10:43.102058 dj_tenants-0.1.1/dj_tenants/conf.py
--rw-r--r--   0        0        0      996 2024-04-16 10:44:41.535837 dj_tenants-0.1.1/dj_tenants/context.py
--rw-r--r--   0        0        0       46 2024-04-16 10:06:02.548359 dj_tenants-0.1.1/dj_tenants/exceptions.py
--rw-r--r--   0        0        0     1496 2024-04-16 22:10:43.102058 dj_tenants-0.1.1/dj_tenants/middleware.py
--rw-r--r--   0        0        0     1295 2024-04-16 21:18:08.416811 dj_tenants-0.1.1/dj_tenants/models.py
--rw-r--r--   0        0        0        0 2024-04-16 11:29:02.214763 dj_tenants-0.1.1/dj_tenants/postgres_backend/__init__.py
--rw-r--r--   0        0        0      434 2024-04-16 11:55:58.663429 dj_tenants-0.1.1/dj_tenants/postgres_backend/base.py
--rw-r--r--   0        0        0     3666 2024-04-16 21:17:16.930323 dj_tenants-0.1.1/dj_tenants/postgres_backend/compiler.py
--rw-r--r--   0        0        0      224 2024-04-16 11:55:44.287371 dj_tenants-0.1.1/dj_tenants/postgres_backend/operations.py
--rw-r--r--   0        0        0      819 2024-04-16 14:33:07.299762 dj_tenants-0.1.1/dj_tenants/utils.py
--rw-r--r--   0        0        0      606 2024-04-16 22:11:06.092489 dj_tenants-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.1/README.md
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1148 2024-04-16 21:50:11.453241 dj_tenants-0.1.2/dj_tenants/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-16 10:59:47.143776 dj_tenants-0.1.2/dj_tenants/apps.py
+-rw-r--r--   0        0        0      324 2024-04-16 23:38:59.972309 dj_tenants-0.1.2/dj_tenants/conf.py
+-rw-r--r--   0        0        0      996 2024-04-16 10:44:41.535837 dj_tenants-0.1.2/dj_tenants/context.py
+-rw-r--r--   0        0        0       46 2024-04-16 10:06:02.548359 dj_tenants-0.1.2/dj_tenants/exceptions.py
+-rw-r--r--   0        0        0     1451 2024-04-16 23:41:38.999642 dj_tenants-0.1.2/dj_tenants/middleware.py
+-rw-r--r--   0        0        0     1295 2024-04-16 21:18:08.416811 dj_tenants-0.1.2/dj_tenants/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:29:02.214763 dj_tenants-0.1.2/dj_tenants/postgres_backend/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-16 11:55:58.663429 dj_tenants-0.1.2/dj_tenants/postgres_backend/base.py
+-rw-r--r--   0        0        0     3666 2024-04-16 21:17:16.930323 dj_tenants-0.1.2/dj_tenants/postgres_backend/compiler.py
+-rw-r--r--   0        0        0      224 2024-04-16 11:55:44.287371 dj_tenants-0.1.2/dj_tenants/postgres_backend/operations.py
+-rw-r--r--   0        0        0      819 2024-04-16 14:33:07.299762 dj_tenants-0.1.2/dj_tenants/utils.py
+-rw-r--r--   0        0        0      606 2024-04-16 23:48:16.830070 dj_tenants-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.2/README.md
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.2/PKG-INFO
```

### Comparing `dj_tenants-0.1.1/dj_tenants/__init__.py` & `dj_tenants-0.1.2/dj_tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.1/dj_tenants/context.py` & `dj_tenants-0.1.2/dj_tenants/context.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.1/dj_tenants/middleware.py` & `dj_tenants-0.1.2/dj_tenants/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from django.shortcuts import redirect
-from django.urls import reverse
+from django.urls import reverse, resolve
 
 from dj_tenants.conf import settings
 
 from dj_tenants import get_tenant_model, tenant_context, tenant_context_disabled
 
+allowed_paths = settings.DJ_TENANTS_URLS_ALLOW_WITHOUT_TENANT
+
+login_url = settings.DJ_TENANTS_LOGIN_VIEW_NAME
+
 
 class DjTenantsMiddleware:
     TenantModel = None
-    LoginUrl = 'login'
 
     def __init__(self, get_response):
         self.get_response = get_response
         self.TenantModel = get_tenant_model()
-        self.LoginUrl = settings.DJ_TENANTS_LOGIN_VIEW_NAME
 
     def __call__(self, request):
         if not request.user.is_authenticated:
             return self.get_response(request)
 
         if request.path.startswith("/admin/"):
             with tenant_context_disabled():
                 return self.get_response(request)
 
-        view_func = None
-        if hasattr(request, 'resolver_match') and request.resolver_match:
-            view_func = request.resolver_match.func
-
-        if view_func and getattr(view_func, 'tenant_not_required', False):
+        ignored_path = any(
+            resolve(request.path).view_name == ignored for ignored in allowed_paths
+        )
+        if ignored_path:
             return self.get_response(request)
 
         tenant = self._get_tenant(request)
 
         if tenant is None:
-            return redirect(reverse(self.LoginUrl))
+            return redirect(reverse(login_url))
 
         with tenant_context(tenant):
             request.tenant = tenant
             return self.get_response(request)
 
     def _get_tenant(self, request):
         tenant_id = request.session.get("tenant_id", None)
```

### Comparing `dj_tenants-0.1.1/dj_tenants/models.py` & `dj_tenants-0.1.2/dj_tenants/models.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.1/dj_tenants/postgres_backend/compiler.py` & `dj_tenants-0.1.2/dj_tenants/postgres_backend/compiler.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.1/dj_tenants/utils.py` & `dj_tenants-0.1.2/dj_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.1/pyproject.toml` & `dj_tenants-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-tenants"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Hugo Mesquita <hugohomesquita@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "dj_tenants" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

