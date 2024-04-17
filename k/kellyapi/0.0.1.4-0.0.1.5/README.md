# Comparing `tmp/kellyapi-0.0.1.4.tar.gz` & `tmp/kellyapi-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.1.4.tar", last modified: Sat Apr 13 14:54:21 2024, max compression
+gzip compressed data, was "kellyapi-0.0.1.5.tar", last modified: Wed Apr 17 16:00:32 2024, max compression
```

## Comparing `kellyapi-0.0.1.4.tar` & `kellyapi-0.0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:54:21.761991 kellyapi-0.0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 14:54:21.761991 kellyapi-0.0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:54:21.761991 kellyapi-0.0.1.4/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:54:21.761991 kellyapi-0.0.1.4/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 14:54:21.000000 kellyapi-0.0.1.4/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 14:54:21.000000 kellyapi-0.0.1.4/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:54:21.000000 kellyapi-0.0.1.4/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 14:54:21.000000 kellyapi-0.0.1.4/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 14:54:21.000000 kellyapi-0.0.1.4/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:54:21.761991 kellyapi-0.0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 14:54:17.000000 kellyapi-0.0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:00:32.109675 kellyapi-0.0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-17 16:00:32.109675 kellyapi-0.0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:00:32.109675 kellyapi-0.0.1.5/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:00:32.109675 kellyapi-0.0.1.5/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-17 16:00:32.000000 kellyapi-0.0.1.5/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 16:00:32.000000 kellyapi-0.0.1.5/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:00:32.000000 kellyapi-0.0.1.5/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 16:00:32.000000 kellyapi-0.0.1.5/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 16:00:32.000000 kellyapi-0.0.1.5/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:00:32.109675 kellyapi-0.0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-17 16:00:27.000000 kellyapi-0.0.1.5/setup.py
```

### Comparing `kellyapi-0.0.1.4/LICENSE` & `kellyapi-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.4/PKG-INFO` & `kellyapi-0.0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.4/README.md` & `kellyapi-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.4/kellyapi/api.py` & `kellyapi-0.0.1.5/kellyapi/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,14 @@
         session: aiohttp.ClientSession = None,
     ):
         self.api = api or "https://api.kellyai.pro/"
         self.api_key = api_key
         self.session = session or aiohttp.ClientSession
 
     def _parse_result(self, response: dict) -> Union[DotMap, List[BytesIO]]:
-        response.get("type")
-        error = response.get("error")
         response = DotMap(response)
         if not error:
             response.success = True
         return response
 
     async def _fetch(self, route, timeout=60, **params):
         try:
@@ -142,14 +140,19 @@
         return content.message
 
     async def upscale(self, image: str):
         kwargs = dict(image=image)
         content = await self._post_data("upscale", data=kwargs)
         return content
 
+    async def rmbg(self, image: str):
+        kwargs = dict(image=image)
+        content = await self._post_data("rmbg", data=kwargs)
+        return content
+
     async def voice_models(self):
         content = await self._fetch("voice-models")
         return content
 
     async def text2voice(self, text: str, model: str = "en-US_LisaExpressive"):
         kwargs = dict(text=text, model=model)
         content = await self._post_data("text2voice", data=kwargs)
```

### Comparing `kellyapi-0.0.1.4/kellyapi/errors.py` & `kellyapi-0.0.1.5/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.4/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.1.5/kellyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.4/setup.py` & `kellyapi-0.0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.1.4",
+    version="0.0.1.5",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

