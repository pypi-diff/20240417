# Comparing `tmp/rewire_fastapi-0.0.5.tar.gz` & `tmp/rewire_fastapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire_fastapi-0.0.5.tar", last modified: Mon Feb 12 12:52:03 2024, max compression
+gzip compressed data, was "rewire_fastapi-0.0.6.tar", last modified: Wed Apr 17 06:41:50 2024, max compression
```

## Comparing `rewire_fastapi-0.0.5.tar` & `rewire_fastapi-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 12:52:03.219995 rewire_fastapi-0.0.5/
--rw-rw-rw-   0        0        0     1086 2024-02-01 21:35:51.000000 rewire_fastapi-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3403 2024-02-12 12:52:03.218996 rewire_fastapi-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1498 2024-02-01 22:53:53.000000 rewire_fastapi-0.0.5/README.md
--rw-rw-rw-   0        0        0      734 2024-02-12 12:51:33.000000 rewire_fastapi-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-12 12:52:03.202790 rewire_fastapi-0.0.5/rewire_fastapi/
--rw-rw-rw-   0        0        0     6299 2024-02-12 12:51:43.000000 rewire_fastapi-0.0.5/rewire_fastapi/__init__.py
--rw-rw-rw-   0        0        0     1646 2024-01-24 06:53:30.000000 rewire_fastapi-0.0.5/rewire_fastapi/dependable.py
-drwxrwxrwx   0        0        0        0 2024-02-12 12:52:03.217996 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/
--rw-rw-rw-   0        0        0     3403 2024-02-12 12:52:03.000000 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-02-12 12:52:03.000000 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 12:52:03.000000 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-02-12 12:52:03.000000 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-12 12:52:03.000000 rewire_fastapi-0.0.5/rewire_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-12 12:52:03.219995 rewire_fastapi-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.320377 rewire_fastapi-0.0.6/
+-rw-rw-rw-   0        0        0     1086 2024-02-01 21:35:51.000000 rewire_fastapi-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3403 2024-04-17 06:41:50.319377 rewire_fastapi-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2024-02-01 22:53:53.000000 rewire_fastapi-0.0.6/README.md
+-rw-rw-rw-   0        0        0      734 2024-04-17 06:41:39.000000 rewire_fastapi-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.303847 rewire_fastapi-0.0.6/rewire_fastapi/
+-rw-rw-rw-   0        0        0     6299 2024-04-17 06:41:30.000000 rewire_fastapi-0.0.6/rewire_fastapi/__init__.py
+-rw-rw-rw-   0        0        0     1646 2024-01-24 06:53:30.000000 rewire_fastapi-0.0.6/rewire_fastapi/dependable.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.319377 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     3403 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:41:50.321377 rewire_fastapi-0.0.6/setup.cfg
```

### Comparing `rewire_fastapi-0.0.5/LICENSE` & `rewire_fastapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.5/PKG-INFO` & `rewire_fastapi-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire_fastapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fastapi integration for rewire
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire_fastapi-0.0.5/README.md` & `rewire_fastapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.5/pyproject.toml` & `rewire_fastapi-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire_fastapi"
-version = "0.0.5"
+version = "0.0.6"
 description = "Fastapi integration for rewire"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire_fastapi-0.0.5/rewire_fastapi/__init__.py` & `rewire_fastapi-0.0.6/rewire_fastapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,20 @@
     server: Literal["uvicorn", "hypercorn", None] = "hypercorn"
     app: AppConfig = AppConfig()
     routes: RouteConfig = RouteConfig()
     uvicorn: UvicornConfig = UvicornConfig()
     hypercorn: HypercornConfig = HypercornConfig()
     patch: PatchConfig = PatchConfig()
     middleware: MiddlewareConfig = MiddlewareConfig()
-    _endpoint: Annotated[Optional[str], Field(alias="endpoint")] = None
+    endpoint_: Annotated[Optional[str], Field(alias="endpoint")] = None
 
     @property
     def endpoint(self):
-        if self._endpoint is not None:
-            return self._endpoint
+        if self.endpoint_ is not None:
+            return self.endpoint_
         host = self.uvicorn.host
         if host == "0.0.0.0":
             host = "localhost"
 
         return f"http://{host}:{self.uvicorn.port}"
```

### Comparing `rewire_fastapi-0.0.5/rewire_fastapi/dependable.py` & `rewire_fastapi-0.0.6/rewire_fastapi/dependable.py`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.5/rewire_fastapi.egg-info/PKG-INFO` & `rewire_fastapi-0.0.6/rewire_fastapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire_fastapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fastapi integration for rewire
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

