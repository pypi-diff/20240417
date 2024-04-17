# Comparing `tmp/VisionCraftAPI-1.0.7.tar.gz` & `tmp/visioncraftapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraftAPI-1.0.7.tar", last modified: Mon Apr 15 18:51:53 2024, max compression
+gzip compressed data, was "visioncraftapi-1.0.8.tar", last modified: Wed Apr 17 12:49:09 2024, max compression
```

## Comparing `VisionCraftAPI-1.0.7.tar` & `visioncraftapi-1.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.556480 VisionCraftAPI-1.0.7/
--rw-rw-rw-   0        0        0     1091 2024-03-28 06:00:02.000000 VisionCraftAPI-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2542 2024-04-15 18:51:53.557480 VisionCraftAPI-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2024-04-15 18:35:25.000000 VisionCraftAPI-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.486144 VisionCraftAPI-1.0.7/VisionCraftAPI/
--rw-rw-rw-   0        0        0       34 2024-03-26 11:28:25.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/__init__.py
--rw-rw-rw-   0        0        0    21559 2024-04-15 18:50:42.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.534377 VisionCraftAPI-1.0.7/VisionCraftAPI/enums/
--rw-rw-rw-   0        0        0      125 2024-03-26 22:05:26.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/enums/__init__.py
--rw-rw-rw-   0        0        0      160 2024-03-26 22:04:43.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/enums/modes.py
--rw-rw-rw-   0        0        0      162 2024-03-26 22:04:35.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/enums/task_statuses.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.539436 VisionCraftAPI-1.0.7/VisionCraftAPI/exceptions/
--rw-rw-rw-   0        0        0      309 2024-03-27 16:35:37.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-03-27 16:42:14.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/exceptions/types.py
--rw-rw-rw-   0        0        0     2067 2024-04-15 18:35:25.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/http_client.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.549161 VisionCraftAPI-1.0.7/VisionCraftAPI/models/
--rw-rw-rw-   0        0        0      303 2024-03-27 20:35:50.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/models/__init__.py
--rw-rw-rw-   0        0        0      336 2024-03-27 20:24:16.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/models/limits.py
--rw-rw-rw-   0        0        0      147 2024-03-26 17:31:11.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/models/llm.py
--rw-rw-rw-   0        0        0      488 2024-03-27 20:28:11.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/models/midjourney.py
--rw-rw-rw-   0        0        0      823 2024-03-27 20:30:01.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/models/whisper.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.555479 VisionCraftAPI-1.0.7/VisionCraftAPI/utils/
--rw-rw-rw-   0        0        0       69 2024-03-26 22:05:35.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/utils/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-03-27 16:55:54.000000 VisionCraftAPI-1.0.7/VisionCraftAPI/utils/checker.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:51:53.528642 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/
--rw-rw-rw-   0        0        0     2542 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2024-04-15 18:51:53.000000 VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 18:51:53.560480 VisionCraftAPI-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-15 18:51:33.000000 VisionCraftAPI-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.227324 visioncraftapi-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2615 2024-04-17 12:49:09.227324 visioncraftapi-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 visioncraftapi-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.164364 visioncraftapi-1.0.8/VisionCraftAPI/
+-rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/__init__.py
+-rw-rw-rw-   0        0        0    21735 2024-04-17 12:46:03.000000 visioncraftapi-1.0.8/VisionCraftAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.190323 visioncraftapi-1.0.8/VisionCraftAPI/enums/
+-rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/enums/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/enums/modes.py
+-rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/enums/task_statuses.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.196325 visioncraftapi-1.0.8/VisionCraftAPI/exceptions/
+-rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/exceptions/types.py
+-rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 visioncraftapi-1.0.8/VisionCraftAPI/http_client.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.214327 visioncraftapi-1.0.8/VisionCraftAPI/models/
+-rw-rw-rw-   0        0        0      323 2024-04-17 12:20:48.000000 visioncraftapi-1.0.8/VisionCraftAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      442 2024-04-17 12:48:37.000000 visioncraftapi-1.0.8/VisionCraftAPI/models/limits.py
+-rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/models/llm.py
+-rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/models/midjourney.py
+-rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/models/whisper.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.221323 visioncraftapi-1.0.8/VisionCraftAPI/utils/
+-rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 visioncraftapi-1.0.8/VisionCraftAPI/utils/checker.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:49:09.224322 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/
+-rw-rw-rw-   0        0        0     2615 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2024-04-17 12:49:09.000000 visioncraftapi-1.0.8/VisionCraftAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:49:09.231324 visioncraftapi-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-17 12:44:27.000000 visioncraftapi-1.0.8/setup.py
```

### Comparing `VisionCraftAPI-1.0.7/LICENSE` & `visioncraftapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/PKG-INFO` & `visioncraftapi-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
+Requires-Dist: aiohttp
+Requires-Dist: pydantic
 
 ![photo (4)](https://github.com/Belyashik2K/VisionCraftAPI/assets/126521808/fa32e4fa-37bd-47a7-9574-bbc02191796b)
 # VisionCraft API
 > Fully async python wrapper for [VisionCraft API](https://api.visioncraft.top/docs)
 
 ## Installing
```

### Comparing `VisionCraftAPI-1.0.7/README.md` & `visioncraftapi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI/api.py` & `visioncraftapi-1.0.8/VisionCraftAPI/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import base64
 
 from json import loads
 from typing import Optional
 
 from .http_client import HTTPClient
-from .models import (RateLimits,
-                     MidjourneyTask,
+from .models import (MidjourneyTask,
                      MidjourneyResult,
                      LLMAnswer,
-                     WhisperResult)
+                     WhisperResult,
+                     Tiers)
 
 class VisionCraftClient(HTTPClient):
     """
     Client for interacting with the VisionCraft API.
     
     API Docs: https://docs.visioncraft.top/
     SDK Docs: https://vision.b2k.tech/
@@ -126,43 +126,47 @@
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-xl-models/available-loras
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-xl-models/get_xl_loras
         
         :return: A list of LORAs for StableDiffusion XL models
         """
         return await self.__get(f'{self.API_HOST}/loras-xl')
-
-    async def get_limits(self) -> RateLimits:
+    
+    async def get_limits(self) -> Tiers:
         """
         Get info about rate limits for free users.
         
         API Docs: https://api.visioncraft.top/limits
         SDK Docs: https://vision.b2k.tech/docs/api-methods/api-limits/get_limits
         
-        :return: A RateLimits object
+        :return: A Tiers object
         """
         
         limits: dict = loads(await self.__get(f'{self.API_HOST}/limits'))
         
         new_keys = {
+            "Free Tier": "FREE",
+            "Tier 1 ($10 per month)": "TIER_1",
+            "Tier 2 ($25 per month)": "TIER_2",
             "SD 1.X": "STABLEDIFFUSION",
             "SDXL models": "STABLEDIFFUSIONXL",
             "DALLE-3": "DALLE3",
             "Image Upscalilng": "IMAGEUPSCALING"
         }
         
-        for key, _ in limits.copy().items():
-            if key in ["SD 1.X", "SDXL models", "DALLE-3", "Image Upscalilng"]:
-                limits[new_keys[key]] = limits[key]
-            else:
-                limits[key.upper()] = limits[key]
-                
-            if key != key.upper():
-                del limits[key]
-        return RateLimits(**limits)
+        new_data = dict()
+        
+        for tier, models in limits.items():
+            new_data[new_keys[tier]] = {}
+            for model, limit in models.items():
+                if model in new_keys:
+                    new_data[new_keys[tier]][new_keys[model]] = limit
+                else:
+                    new_data[new_keys[tier]][model.upper()] = limit           
+        return Tiers(**new_data)
     
     async def get_i2i_schedulers(self) -> list:
         """
         Get list of all schedulers for Image2Image model.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/image2image/available-schedulers
         SDK Docs: https://vision.b2k.tech/docs/api-methods/image2image/get_i2i_schedulers
@@ -188,15 +192,15 @@
                              sampler: str,
                              width: Optional[int] = 1024,
                              height: Optional[int] = 1024,
                              image_count: Optional[int] = 1,
                              negative_prompt: Optional[str] = str(),
                              cfg_scale: Optional[int] = 10,
                              steps: Optional[int] = 30,
-                             loras: Optional[dict] = {},
+                             loras: Optional[dict] = dict(),
                              upscale: Optional[bool] = False) -> list[str]:
         """
         Generate an image using StableDiffusion 1.x models.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-1.x-models/image-generation
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-1.x-models/generate_image
         
@@ -238,15 +242,15 @@
                                 sampler: str,
                                 width: Optional[int] = 1024,
                                 height: Optional[int] = 1024,
                                 negative_prompt: Optional[str] = str(),
                                 cfg_scale: Optional[int] = 10,
                                 steps: Optional[int] = 30,
                                 image_count: Optional[int] = 1,
-                                loras: Optional[dict] = {}) -> list[str]:
+                                loras: Optional[dict] = dict()) -> list[str]:
         """
         Generate an image using StableDiffusion XL models.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-xl-models/image-generation
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-xl-models/generate_xl_image
         
         :param prompt: A text prompt for image generation
```

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI/exceptions/types.py` & `visioncraftapi-1.0.8/VisionCraftAPI/exceptions/types.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI/http_client.py` & `visioncraftapi-1.0.8/VisionCraftAPI/http_client.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI/models/whisper.py` & `visioncraftapi-1.0.8/VisionCraftAPI/models/whisper.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI/utils/checker.py` & `visioncraftapi-1.0.8/VisionCraftAPI/utils/checker.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/PKG-INFO` & `visioncraftapi-1.0.8/VisionCraftAPI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
+Requires-Dist: aiohttp
+Requires-Dist: pydantic
 
 ![photo (4)](https://github.com/Belyashik2K/VisionCraftAPI/assets/126521808/fa32e4fa-37bd-47a7-9574-bbc02191796b)
 # VisionCraft API
 > Fully async python wrapper for [VisionCraft API](https://api.visioncraft.top/docs)
 
 ## Installing
```

### Comparing `VisionCraftAPI-1.0.7/VisionCraftAPI.egg-info/SOURCES.txt` & `visioncraftapi-1.0.8/VisionCraftAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.7/setup.py` & `visioncraftapi-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.7'
+version = '1.0.8'
 
 with open('README.md', 'r') as f:
       long_description = f.read()
 
 setup(name='VisionCraftAPI',
       version=version,
```

