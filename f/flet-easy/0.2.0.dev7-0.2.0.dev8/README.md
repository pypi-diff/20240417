# Comparing `tmp/flet_easy-0.2.0.dev7.tar.gz` & `tmp/flet_easy-0.2.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.0.dev7.tar", last modified: Sun Apr  7 23:54:34 2024, max compression
+gzip compressed data, was "flet_easy-0.2.0.dev8.tar", last modified: Wed Apr 17 00:35:29 2024, max compression
```

## Comparing `flet_easy-0.2.0.dev7.tar` & `flet_easy-0.2.0.dev8.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0    11541 2024-03-27 23:22:54.481270 flet_easy-0.2.0.dev7/LICENSE
--rw-r--r--   0        0        0    11541 2024-03-27 23:22:54.481270 flet_easy-0.2.0.dev7/LICENSE
--rw-r--r--   0        0        0     4215 2024-03-27 23:22:54.482257 flet_easy-0.2.0.dev7/README.md
--rw-r--r--   0        0        0     4215 2024-03-27 23:22:54.482257 flet_easy-0.2.0.dev7/README.md
--rw-r--r--   0        0        0     1564 2024-04-07 23:54:34.630972 flet_easy-0.2.0.dev7/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-07 22:47:44.055967 flet_easy-0.2.0.dev7/src/flet_easy/__init__.py
--rw-r--r--   0        0        0    13856 2024-03-30 00:26:40.645132 flet_easy-0.2.0.dev7/src/flet_easy/__pycache__/route.cpython-311.pyc.2038480740688
--rw-r--r--   0        0        0     2356 2024-04-02 03:23:24.628507 flet_easy-0.2.0.dev7/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2099 2024-03-27 23:30:22.585369 flet_easy-0.2.0.dev7/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-03-27 23:25:17.554726 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-03-27 23:25:17.554726 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-03-27 23:25:17.555756 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-03-27 23:25:17.556749 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-03-27 23:25:17.557757 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-03-27 23:25:17.558274 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-03-27 23:25:17.559303 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-03-27 23:25:17.560320 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-03-27 23:25:17.562336 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-03-27 23:25:17.562336 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-03-27 23:25:17.563331 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       84 2024-03-27 23:30:22.582338 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2422 2024-03-27 23:30:22.583375 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-03-27 23:25:17.564875 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       44 2024-03-27 23:30:22.583375 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1258 2024-03-27 23:30:22.580809 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-03-27 23:25:17.567392 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      304 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0       66 2024-03-27 23:30:22.586373 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/__init__.py
--rw-r--r--   0        0        0      588 2024-03-27 23:30:22.580809 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-03-27 23:25:17.571969 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    12191 2024-04-07 23:18:44.195005 flet_easy-0.2.0.dev7/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      187 2024-04-07 23:06:12.478685 flet_easy-0.2.0.dev7/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2483 2024-04-07 23:06:20.563626 flet_easy-0.2.0.dev7/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    18283 2024-04-07 23:06:36.428370 flet_easy-0.2.0.dev7/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0     9732 2024-04-07 23:06:51.294251 flet_easy-0.2.0.dev7/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1191 2024-04-07 23:07:10.214456 flet_easy-0.2.0.dev7/src/flet_easy/job.py
--rw-r--r--   0        0        0     3987 2024-04-07 23:09:10.638387 flet_easy-0.2.0.dev7/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     7534 2024-04-07 23:10:13.620117 flet_easy-0.2.0.dev7/src/flet_easy/pagesy.py
--rw-r--r--   0        0        0    11102 2024-04-07 23:13:15.908162 flet_easy-0.2.0.dev7/src/flet_easy/route.py
--rw-r--r--   0        0        0     1540 2024-04-07 23:13:26.115988 flet_easy-0.2.0.dev7/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     5251 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev8/LICENSE
+-rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev8/LICENSE
+-rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev8/README.md
+-rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev8/README.md
+-rw-r--r--   0        0        0     1732 2024-04-17 00:35:29.556105 flet_easy-0.2.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-04-12 03:14:22.077045 flet_easy-0.2.0.dev8/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0     1322 2024-04-14 22:48:16.071270 flet_easy-0.2.0.dev8/src/flet_easy/auto_route.py
+-rw-r--r--   0        0        0     2356 2024-04-12 03:14:22.079042 flet_easy-0.2.0.dev8/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2099 2024-04-12 03:14:22.079042 flet_easy-0.2.0.dev8/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-04-12 03:14:22.080559 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-04-12 03:14:22.082609 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.083607 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.084612 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.085610 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.086618 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-04-12 03:14:22.087607 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       45 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-04-12 03:14:22.092763 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-12 03:14:22.093720 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      246 2024-04-17 00:24:27.890970 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-04-12 03:14:22.094724 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-12 03:14:22.096720 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-04-16 23:25:58.330304 flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12208 2024-04-16 21:36:20.961519 flet_easy-0.2.0.dev8/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev8/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev8/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18351 2024-04-16 17:27:54.462979 flet_easy-0.2.0.dev8/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9856 2024-04-16 17:27:34.348744 flet_easy-0.2.0.dev8/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-04-16 21:14:26.280232 flet_easy-0.2.0.dev8/src/flet_easy/job.py
+-rw-r--r--   0        0        0     4024 2024-04-16 21:27:52.940346 flet_easy-0.2.0.dev8/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7512 2024-04-16 17:27:54.461988 flet_easy-0.2.0.dev8/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11402 2024-04-16 18:07:25.972524 flet_easy-0.2.0.dev8/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-04-12 03:14:22.105829 flet_easy-0.2.0.dev8/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     5251 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev8/PKG-INFO
```

### Comparing `flet_easy-0.2.0.dev7/LICENSE` & `flet_easy-0.2.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/README.md` & `flet_easy-0.2.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/pyproject.toml` & `flet_easy-0.2.0.dev8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flet-easy"
-version = "0.2.0.dev7"
+version = "0.2.0.dev8"
 description = "Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
 authors = [
     { name = "Daxexs", email = "Daxexsdev@gmail.com" },
 ]
 dependencies = [
     "parse>=1.20.1",
     "pyJWT>=2.8.0",
@@ -51,21 +51,31 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 test = [
     "flet>=0.21.1",
     "ruff>=0.3.4",
+    "peewee>=3.17.2",
+]
+docs = [
+    "mkdocs-material>=9.5.17",
+    "mike>=2.0.0",
 ]
 
 [tool.pdm.build]
 excludes = [
     "./**/.git",
 ]
 package-dir = "src"
 includes = [
     "src/flet_easy",
 ]
 source-includes = [
     "LICENSE",
     "README.md",
 ]
+
+[tool.pdm.scripts]
+doc = "mkdocs serve"
+format = "ruff format"
+check = "ruff check"
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/copy.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/copy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/main.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/main.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/components/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/views/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.0.dev8/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/datasy.py` & `flet_easy-0.2.0.dev8/src/flet_easy/datasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         self.__share = SessionStorageEdit(self.__page)
         self.__on_keyboard_event = page_on_keyboard
         self.__on_resize = page_on_resize
         self.__route: str = None
         self.__go = go
 
         self.__secret_key: SecretKey = secret_key
-        self.__key_login: str = None
         self.__auto_logout: bool = auto_logout
         self.__sleep: int = 1
+        self._key_login: str = None
         self._login_done: bool = False
         self._login_async: bool = login_async
         self._check_event_router: bool = False
 
     @property
     def page(self):
         return self.__page
@@ -143,15 +143,15 @@
 
     @on_resize.setter
     def on_resize(self, on_resize: object):
         self.__on_resize = on_resize
 
     @property
     def key_login(self):
-        return self.__key_login
+        return self._key_login
 
     @property
     def auto_logout(self):
         return self.__auto_logout
 
     @property
     def secret_key(self):
@@ -198,23 +198,23 @@
             return ft.View(
                 controls=[
                     ft.FilledButton('Logout', onclick=data.logout('key-login')),
             )
         ```
         """
 
-        def execute():
+        def execute(key: str):
             assert self.route_login is not None, "Adds a login path in the FletEasy Class"
             if self.page.web:
                 self.page.pubsub.send_all_on_topic(self.page.client_ip, Msg("logout", key))
             else:
                 self.page.run_task(self.page.client_storage.remove_async, key)
                 self.page.go(self.route_login)
 
-        return lambda _=None: execute()
+        return lambda _=None: execute(key)
 
     async def __logaut_init(self, topic, msg: Msg):
         if msg.method == "login":
             self._check_event_router = False
             await self.page.client_storage.set_async(msg.key, msg.value.get("value"))
             if self.page.route == self.route_login:
                 self.page.go(msg.value.get("next_route"))
@@ -285,28 +285,28 @@
             ), "Use a dict in login method values or don't use time_expiry."
             assert (
                 self.__secret_key is not None
             ), "Set the secret_key in the FletEasy class parameter or don't use time_expiry."
 
         if self.__secret_key:
             evaluate_secret_key(self)
-            self.__key_login = key
+            self._key_login = key
             self.__sleep = sleep
             value = encode_verified(self.secret_key, value, time_expiry)
             self._login_done = True
 
             if self.__auto_logout:
                 self._create_tasks(time_expiry, key, sleep)
 
         if self.page.web:
             self.page.pubsub.send_all_on_topic(
                 self.page.client_ip, Msg("login", key, {"value": value, "next_route": next_route})
             )
         else:
-            self.page.run_task(self.page.client_storage.set_async, key, value)
+            self.page.run_task(self.page.client_storage.set_async, key, value).result()
             self.__go(next_route)
 
     """ Page go  """
 
     def go(self, route: str):
         """To change the application path, it is important for better validation to avoid using `page.go()`."""
         return lambda _=None: self.__go(route)
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.0.dev8/src/flet_easy/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/fletEasy.py` & `flet_easy-0.2.0.dev8/src/flet_easy/fletEasy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,120 +1,101 @@
 try:
     from flet import AppView, Page, WebRenderer, app
 except ImportError:
     raise Exception('Install "flet" the latest version available -> pip install flet --upgrade.')
 
 from functools import wraps
+from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional
 
 from flet import View
 
+from flet_easy.auto_route import automatic_routing
 from flet_easy.datasy import Datasy
 from flet_easy.extrasJwt import SecretKey
 from flet_easy.inheritance import Viewsy
 from flet_easy.pagesy import AddPagesy, Middleware, Pagesy
 from flet_easy.route import FletEasyX
 
 
 class FletEasy:
-    """we create the app object, in it you can configure:
-    * The path that is different from '/'.
-    * The initial path when initializing the app
-    * The path that will be redirected when the app has path protection configured.
+    """
+    we create the app object, in it you can configure:
+
+    * `route_prefix` : The route that is different from ` /`.
+    * `route_init` : The initial route to initialize the app, by default is `/`.
+    * `route_login` : The route that will be redirected when the app has route protectionconfigured.
+    * `on_Keyboard` : Enables the on_Keyboard event, by default it is disabled (False).
+    * `on_resize` : Triggers the on_resize event, by default it is disabled (False).
+    * `secret_key` : Used with `SecretKey` class of Flet easy, to configure JWT or client storage.
+    * `auto_logout` : If you use JWT, you can configure it.
+    * `path_views` : Configuration of the folder where are the .py files of the pages, you use the `Path` class to configure it.
 
     Example:
     ```python
     import flet as ft
     import flet_easy as fs
 
     app = fs.FletEasy(
-        route_prefix="/index",
-        route_init="/index/hi",
+        route_prefix="/FletEasy",
+        route_init="/FletEasy/home",
     )
 
 
-    @app.view()
-    async def view(page: ft.Page):
-        def modify_theme():
-            if page.theme_mode == ft.ThemeMode.DARK:
-                page.theme_mode = ft.ThemeMode.LIGHT
-            else:
-                page.theme_mode = ft.ThemeMode.DARK
-
-        async def theme(e):
-            if page.theme_mode == ft.ThemeMode.SYSTEM:
-                modify_theme()
-            modify_theme()
-            await page.update_async()
-
-        async def go_home(e):
-            await page.go_async("/index/hi")
-
+    @app.view
+    async def view(data: fs.Datasy):
         return fs.Viewsy(
             appbar=ft.AppBar(
                 title=ft.Text("AppBar Example"),
                 center_title=False,
                 bgcolor=ft.colors.SURFACE_VARIANT,
                 actions=[
-                    ft.IconButton(ft.icons.WB_SUNNY_OUTLINED, on_click=theme),
                     ft.PopupMenuButton(
                         items=[
-                            ft.PopupMenuItem(text="🔥 Home", on_click=go_home),
+                            ft.PopupMenuItem(
+                                text="🔥 Home", on_click=data.go(data.route_init)
+                            ),
                         ]
-                    ),
+                    )
                 ],
             ),
             vertical_alignment=ft.MainAxisAlignment.CENTER,
             horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
 
-    @app.page("/hi", page_clear=True)
+    @app.page("/home", title="Index - Home", page_clear=True)
     async def index_page(data: fs.Datasy):
-        page = data.page
         view = data.view
-        page.title = "Index - Home"
-
         view.appbar.title = ft.Text("Index - Home")
-
-        async def go_test(e):
-            await page.go_async(f"/index/test/10/user/junior")
-
         return ft.View(
-            "/index/hi",
+            data.route_init,
             controls=[
                 ft.Text("Menú", size=40),
                 ft.ElevatedButton(
                     "Go to Test",
-                    on_click=go_test,
+                    on_click=data.go(f"{data.route_prefix}/test/10/user/dxs"),
                 ),
             ],
             appbar=view.appbar,
             vertical_alignment=ft.MainAxisAlignment.CENTER,
             horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
 
-    @app.page("/test/{id:d}/user/{name:l}")
-    async def test_page(data: fs.Datasy, id: int, name: str):
-        page = data.page
+    @app.page("/test/{id:d}/user/{name:l}", title="Test")
+    def test_page(data: fs.Datasy, id: int, name: str):
         view = data.view
-
-        page.title = "Test"
         view.appbar.title = ft.Text("test")
-
-        async def go_index(e):
-            await page.go_async(f"/index/hi")
-
         return ft.View(
             "/index/test",
             controls=[
-                ft.Text(f"Test {data.url_params}"),
+                ft.Text(f"Test {id} | {name}"),
                 ft.Text(f"Test Id is: {id}"),
-                ft.ElevatedButton("Go to Home", on_click=go_index),
+                ft.ElevatedButton("Go to Home", on_click=data.go(data.route_init)),
             ],
             appbar=view.appbar,
             vertical_alignment=ft.MainAxisAlignment.CENTER,
             horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
 
@@ -128,14 +109,15 @@
         route_prefix: str = None,
         route_init: str = "/",
         route_login: str = None,
         on_resize: bool = False,
         on_Keyboard: bool = False,
         secret_key: SecretKey = None,
         auto_logout: bool = False,
+        path_views: Path = None,
     ):
         self.__route_prefix = route_prefix
         self.__route_init = route_init
         self.__route_login = route_login
         self.__on_resize = on_resize
         self.__on_Keyboard = on_Keyboard
         self.__secret_key = secret_key
@@ -145,14 +127,17 @@
         self.__pages = set()
         self.__page_404: Pagesy = None
         self.__view_data: Viewsy = None
         self.__view_config: Callable[[Datasy], None] = None
         self.__config_event: Callable[[Datasy], None] = None
         self.__middlewares: Middleware = None
 
+        if path_views is not None:
+            self.add_pages(automatic_routing(path_views))
+
     # -------------------------------------------------------------------
     # -- initialize / Supports async
 
     def run(
         self,
         name="",
         host=None,
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/inheritance.py` & `flet_easy-0.2.0.dev8/src/flet_easy/inheritance.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,16 @@
     ---
     * `e` : Returns `ControlEvent` event, each time the height and width changes.
     * `page` : Returns `ControlEvent` event, each time the height and width changes.
     * `height` : Returns its updated value.
     * `width` : Returns its updated value.
     * `heightX()` :This method allows to obtain the values of the height of the page, which requires as parameter to enter an integer value from 1 to 100 (100 = 100%).
     * `widthx()` : This method is similar to the previous one in terms of page width.
+    * `margin_y` : Requires an integer value on the y-axis.
+    * `margin_x` : Requires an integer value on the x-axis.
 
     ```
     """
 
     def __init__(self, page: Page = None) -> None:
         self.__page = page
         self.__height: float = page.height
@@ -190,14 +192,15 @@
             return (self.width - self.margin_x) * float("0." + str(width))
         else:
             return self.width - self.margin_x
 
 
 # Add new attributes if flet adds in its updates.
 
+
 @dataclass
 class Viewsy:
     route: str | None = None
     controls: List[Control] | None = None
     appbar: AppBar | None = None
     bottom_appbar: BottomAppBar | None = None
     floating_action_button: FloatingActionButton | None = None
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/job.py` & `flet_easy-0.2.0.dev8/src/flet_easy/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/jwt.py` & `flet_easy-0.2.0.dev8/src/flet_easy/jwt.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def secret_key(self) -> str:
         return token_bytes(64).hex().encode("utf-8")
 
 
 async def _handle_decode_errors(data: Datasy, key_login: str) -> Union[Dict[str, Any], bool]:
     """decodes the jwt and updates the browser sessions."""
     try:
+        data._key_login = key_login
         evaluate_secret_key(data)
 
         if not await data.page.client_storage.contains_key_async(key_login):
             return False
 
         if data.auto_logout and not data._login_done:
             data.page.pubsub.send_others_on_topic(
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/pagesy.py` & `flet_easy-0.2.0.dev8/src/flet_easy/pagesy.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,33 +159,31 @@
         -> The decorated function must receive a parameter, for example `data:fs.Datasy`.
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
-        counter = fs.AddPagesy(
-            route_prefix='/counter'
-        )
+        counter = fs.AddPagesy(route_prefix="/counter")
 
-        @counter.page('/', title='Counter)
-        async def counter_page(data: fs.Datasy):
 
+        @counter.page("/", title="Counter")
+        async def counter_page(data: fs.Datasy):
             view = data.view
 
-            view.appbar.title = ft.Text('Counter')
+            view.appbar.title = ft.Text("Counter")
 
             return ft.View(
-                route='/counter',
+                route="/counter",
                 controls=[
-                    ft.Text('Counter'),
+                    ft.Text("Counter"),
                 ],
                 appbar=view.appbar,
                 vertical_alignment=view.vertical_alignment,
-                horizontal_alignment=view.horizontal_alignment
+                horizontal_alignment=view.horizontal_alignment,
             )
         ```
         """
         data = {
             "route": route,
             "title": title,
             "page_clear": page_clear,
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/route.py` & `flet_easy-0.2.0.dev8/src/flet_easy/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,22 +57,31 @@
             secret_key=secret_key,
             auto_logout=auto_logout,
             page_on_keyboard=self.__page_on_keyboard,
             page_on_resize=self.__page_on_resize,
             login_async=iscoroutinefunction(self.__config_login),
             go=self._go,
         )
-        self.__data.view = self.__page.run_task(self.__view_data_config).result()
+        self.__data.view = (
+            self.__page.run_task(self.__view_data_config).result()
+            if self.__view_data is not None
+            else None
+        )
         if self.__route_login is not None:
             self.__data._create_login()
 
     # ----------- Supports async
     def __route_change(self, e: RouteChangeEvent):
         if not self.__data._check_event_router:
-            self._go(e.route)
+            route = (
+                self.__data.route_init
+                if self.__data.route_init != "/" and e.route == "/"
+                else e.route
+            )
+            self._go(route)
         self.__data._check_event_router = False
 
     def __view_pop(self, e):
         self.__page.views.pop()
         top_view = self.__page.views[-1]
         self.__page.go(top_view.route)
 
@@ -89,18 +98,18 @@
         if self.__view_config:
             if iscoroutinefunction(self.__view_config):
                 await self.__view_config(self.__page)
             else:
                 self.__view_config(self.__page)
 
         if self.__config_event:
-            if iscoroutinefunction(self.__view_config):
-                await self.__config_event(self.__page)
+            if iscoroutinefunction(self.__config_event):
+                await self.__config_event(self.__data)
             else:
-                self.__config_event(self.__page)
+                self.__config_event(self.__data)
 
     def __disconnect(self, e):
         if self.__data._login_done:
             self.__page.pubsub.send_others_on_topic(
                 self.__page.client_ip,
                 Msg("updateLoginSessions", value=self.__data._login_done),
             )
@@ -202,20 +211,20 @@
                 return False
             else:
                 _middlewares = self.__pagesy.middleware
                 _middlewares_two = True
 
     def __process_route(self, custom_params: Dict[str, Callable[[], bool]], path: str, route: str):
         if custom_params is None:
-            route_math = parse(route, path)
+            route_math = parse(route, path, case_sensitive=True)
             return [route_math, route_math]
 
         else:
             try:
-                route_math = parse(route, path, custom_params)
+                route_math = parse(route, path, custom_params, case_sensitive=True)
                 route_check = (
                     all(
                         valor is not False and valor is not None
                         for valor in dict(route_math.named).values()
                     )
                     if route_math
                     else route_math
@@ -231,15 +240,15 @@
         pg_404 = True
         self.__data._check_event_router = True
         self.__data.on_keyboard_event.clear()
         path = self.__route_init if route == "/" else route
 
         for page in self.__pages:
             route_math, route_check = self.__process_route(page.custom_params, path, page.route)
-            if route_check is not None:
+            if route_check:
                 pg_404 = False
                 self.__pagesy = page
                 try:
                     if page.protected_route:
                         if iscoroutinefunction(self.__config_login):
                             try:
                                 auth = self.__page.run_task(
```

### Comparing `flet_easy-0.2.0.dev7/src/flet_easy/view_404.py` & `flet_easy-0.2.0.dev8/src/flet_easy/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev7/PKG-INFO` & `flet_easy-0.2.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.0.dev7
+Version: 0.2.0.dev8
 Summary: Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
-Keywords: flet easy flet python flet router
+Keywords: flet easy,flet,python,flet router
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

