# Comparing `tmp/gemini_ng-0.1.1.tar.gz` & `tmp/gemini_ng-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ng-0.1.1.tar", last modified: Mon Apr 15 17:24:26 2024, max compression
+gzip compressed data, was "gemini_ng-0.1.2.tar", last modified: Wed Apr 17 12:13:45 2024, max compression
```

## Comparing `gemini_ng-0.1.1.tar` & `gemini_ng-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.650340 gemini_ng-0.1.1/
--rw-r--r--   0 viv        (501) staff       (20)     1053 2024-04-15 16:41:45.000000 gemini_ng-0.1.1/LICENSE
--rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-15 17:24:26.649918 gemini_ng-0.1.1/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)     1019 2024-04-15 16:43:10.000000 gemini_ng-0.1.1/README.md
--rw-r--r--   0 viv        (501) staff       (20)     1012 2024-04-15 16:16:28.000000 gemini_ng-0.1.1/pyproject.toml
--rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-15 17:24:26.650529 gemini_ng-0.1.1/setup.cfg
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.644348 gemini_ng-0.1.1/src/
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.645616 gemini_ng-0.1.1/src/gemini_ng/
--rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-15 17:23:01.000000 gemini_ng-0.1.1/src/gemini_ng/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     1684 2024-04-15 16:14:47.000000 gemini_ng-0.1.1/src/gemini_ng/chat.py
--rw-r--r--   0 viv        (501) staff       (20)     8045 2024-04-15 17:22:34.000000 gemini_ng-0.1.1/src/gemini_ng/client.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.648295 gemini_ng-0.1.1/src/gemini_ng/schemas/
--rw-r--r--   0 viv        (501) staff       (20)      386 2024-04-14 18:22:25.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/base.py
--rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/harm.py
--rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/part.py
--rw-r--r--   0 viv        (501) staff       (20)     2838 2024-04-14 16:23:27.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/request.py
--rw-r--r--   0 viv        (501) staff       (20)     1441 2024-04-15 16:14:16.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/response.py
--rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.1.1/src/gemini_ng/schemas/upload.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.649137 gemini_ng-0.1.1/src/gemini_ng/utils/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.1.1/src/gemini_ng/utils/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      509 2024-04-15 16:23:14.000000 gemini_ng-0.1.1/src/gemini_ng/utils/cache.py
--rw-r--r--   0 viv        (501) staff       (20)     1435 2024-04-15 15:33:21.000000 gemini_ng-0.1.1/src/gemini_ng/utils/error.py
--rw-r--r--   0 viv        (501) staff       (20)     2417 2024-04-15 10:18:45.000000 gemini_ng-0.1.1/src/gemini_ng/utils/video.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 17:24:26.649559 gemini_ng-0.1.1/src/gemini_ng.egg-info/
--rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-15 17:24:26.000000 gemini_ng-0.1.1/src/gemini_ng.egg-info/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      640 2024-04-15 17:24:26.000000 gemini_ng-0.1.1/src/gemini_ng.egg-info/SOURCES.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-15 17:24:26.000000 gemini_ng-0.1.1/src/gemini_ng.egg-info/dependency_links.txt
--rw-r--r--   0 viv        (501) staff       (20)      137 2024-04-15 17:24:26.000000 gemini_ng-0.1.1/src/gemini_ng.egg-info/requires.txt
--rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-15 17:24:26.000000 gemini_ng-0.1.1/src/gemini_ng.egg-info/top_level.txt
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.127534 gemini_ng-0.1.2/
+-rw-r--r--   0 viv        (501) staff       (20)     1053 2024-04-15 16:41:45.000000 gemini_ng-0.1.2/LICENSE
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-17 12:13:45.127284 gemini_ng-0.1.2/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)     1019 2024-04-15 16:43:10.000000 gemini_ng-0.1.2/README.md
+-rw-r--r--   0 viv        (501) staff       (20)     1012 2024-04-15 16:16:28.000000 gemini_ng-0.1.2/pyproject.toml
+-rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-17 12:13:45.127596 gemini_ng-0.1.2/setup.cfg
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.120973 gemini_ng-0.1.2/src/
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.122544 gemini_ng-0.1.2/src/gemini_ng/
+-rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-17 12:13:13.000000 gemini_ng-0.1.2/src/gemini_ng/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     1693 2024-04-17 12:11:24.000000 gemini_ng-0.1.2/src/gemini_ng/chat.py
+-rw-r--r--   0 viv        (501) staff       (20)     8172 2024-04-17 12:11:51.000000 gemini_ng-0.1.2/src/gemini_ng/client.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.124755 gemini_ng-0.1.2/src/gemini_ng/schemas/
+-rw-r--r--   0 viv        (501) staff       (20)      385 2024-04-17 12:08:05.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/base.py
+-rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/harm.py
+-rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/part.py
+-rw-r--r--   0 viv        (501) staff       (20)     2842 2024-04-17 12:11:02.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/request.py
+-rw-r--r--   0 viv        (501) staff       (20)     1441 2024-04-15 16:14:16.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/response.py
+-rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.1.2/src/gemini_ng/schemas/upload.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.126453 gemini_ng-0.1.2/src/gemini_ng/utils/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.1.2/src/gemini_ng/utils/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      509 2024-04-15 16:23:14.000000 gemini_ng-0.1.2/src/gemini_ng/utils/cache.py
+-rw-r--r--   0 viv        (501) staff       (20)     1435 2024-04-15 15:33:21.000000 gemini_ng-0.1.2/src/gemini_ng/utils/error.py
+-rw-r--r--   0 viv        (501) staff       (20)     2417 2024-04-15 10:18:45.000000 gemini_ng-0.1.2/src/gemini_ng/utils/video.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 12:13:45.126824 gemini_ng-0.1.2/src/gemini_ng.egg-info/
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-17 12:13:45.000000 gemini_ng-0.1.2/src/gemini_ng.egg-info/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      640 2024-04-17 12:13:45.000000 gemini_ng-0.1.2/src/gemini_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-17 12:13:45.000000 gemini_ng-0.1.2/src/gemini_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 viv        (501) staff       (20)      137 2024-04-17 12:13:45.000000 gemini_ng-0.1.2/src/gemini_ng.egg-info/requires.txt
+-rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-17 12:13:45.000000 gemini_ng-0.1.2/src/gemini_ng.egg-info/top_level.txt
```

### Comparing `gemini_ng-0.1.1/LICENSE` & `gemini_ng-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/PKG-INFO` & `gemini_ng-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.1.1
+Version: 0.1.2
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 License: Copyright (c) 2024 Ming Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gemini_ng-0.1.1/README.md` & `gemini_ng-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/pyproject.toml` & `gemini_ng-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/chat.py` & `gemini_ng-0.1.2/src/gemini_ng/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import TYPE_CHECKING
 
 from .schemas import (
-    ChatMessage, ChatHistory, GenerationConfig, GenerationResponse, SafetySettings
+    ChatMessage, ChatHistory, GenerationConfig, GenerationResponse, SafetySetting
 )
 
 
 if TYPE_CHECKING:
     from .client import GeminiClient
 
 
 class ChatSession:
     def __init__(
         self,
         client: "GeminiClient",
         model: str,
         history: list[ChatMessage] | None = None,
         generation_config: GenerationConfig | dict | None = None,
-        safety_settings: SafetySettings | dict | None = None,
+        safety_settings: list[SafetySetting | dict] | None = None,
     ):
         self.client = client
         self.model = model
         self.history = history or []
         self.generation_config = generation_config
         self.safety_settings = safety_settings
 
     def send_message(
         self,
         message: list | str,
         generation_config: GenerationConfig | dict | None = None,
-        safety_settings: SafetySettings | dict | None = None,
+        safety_settings: list[SafetySetting | dict] | None = None,
     ) -> GenerationResponse:
         parts = self.client.normalize_prompt(message)
         self.history.append(ChatMessage(role="user", parts=parts))
 
         rsp = self.client.generate(
             self.model,
             ChatHistory(messages=self.history),
```

### Comparing `gemini_ng-0.1.1/src/gemini_ng/client.py` & `gemini_ng-0.1.2/src/gemini_ng/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .schemas import (
     ChatMessage,
     ChatHistory,
     GenerationConfig,
     GenerationRequest,
     GenerationRequestParts,
     GenerationResponse,
-    SafetySettings,
+    SafetySetting,
     TextPart,
     ImagePart,
     FilePart,
     VideoPart,
     UploadFile,
     UploadedFile,
 )
@@ -91,15 +91,15 @@
 
     @handle_http_exception
     def generate(
         self,
         model: str,
         prompt: GenerationRequest | ChatHistory | list | str,
         generation_config: GenerationConfig | dict | None = None,
-        safety_settings: SafetySettings | dict | None = None,
+        safety_settings: list[SafetySetting | dict] | None = None,
     ) -> GenerationResponse:
         generation_request = self._prepare_generation_request(
             prompt,
             generation_config=generation_config,
             safety_settings=safety_settings,
         )
 
@@ -116,15 +116,15 @@
         return GenerationResponse.model_validate(rsp)
 
     def start_chat(
         self,
         model: str,
         history: list[ChatMessage] | ChatHistory | None = None,
         generation_config: GenerationConfig | dict | None = None,
-        safety_settings: SafetySettings | dict | None = None,
+        safety_settings: list[SafetySetting | dict] | None = None,
     ) -> ChatSession:
         if isinstance(history, ChatHistory):
             history = history.messages
 
         return ChatSession(
             self,
             model,
@@ -133,15 +133,15 @@
             safety_settings=safety_settings,
         )
 
     def _prepare_generation_request(
         self,
         prompt: GenerationRequest | ChatHistory | list | str,
         generation_config: GenerationConfig | dict | None = None,
-        safety_settings: SafetySettings | dict | None = None,
+        safety_settings: list[SafetySetting | dict] | None = None,
     ) -> GenerationRequest:
         if isinstance(prompt, GenerationRequest):
             request = prompt
         elif isinstance(prompt, ChatHistory):
             request = GenerationRequest(contents=prompt.messages)
         else:
             parts = self.normalize_prompt(prompt)
@@ -151,16 +151,20 @@
 
         if generation_config is not None:
             if not isinstance(generation_config, GenerationConfig):
                 generation_config = GenerationConfig.model_validate(generation_config)
             request.generation_config = generation_config
 
         if safety_settings is not None:
-            if not isinstance(safety_settings, SafetySettings):
-                safety_settings = SafetySettings.model_validate(safety_settings)
+            safety_settings = [
+                safety_setting
+                if isinstance(safety_setting, SafetySetting)
+                else SafetySetting.model_validate(safety_setting)
+                for safety_setting in safety_settings
+            ]
             request.safety_settings = safety_settings
 
         return request
 
     def upload_image(self, image_path: str) -> ImagePart:
         if not os.path.exists(image_path):
             raise FileNotFoundError(f"Image file not found: {image_path}")
```

### Comparing `gemini_ng-0.1.1/src/gemini_ng/schemas/harm.py` & `gemini_ng-0.1.2/src/gemini_ng/schemas/harm.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/schemas/part.py` & `gemini_ng-0.1.2/src/gemini_ng/schemas/part.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/schemas/request.py` & `gemini_ng-0.1.2/src/gemini_ng/schemas/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     top_k: int | None = Field(
         None,
         alias="topK",
         description="The maximum number of tokens to consider when sampling.",
     )
 
 
-class SafetySettings(BaseModel):
+class SafetySetting(BaseModel):
     category: HarmCategory | None = Field(
         None, description="The category of harmful content to block."
     )
 
     threshold: HarmBlockThreshold | None = Field(
         None, description="The threshold of harmful content to block."
     )
@@ -89,10 +89,10 @@
         ..., description="Contents of the request."
     )
 
     generation_config: GenerationConfig | dict | None = Field(
         None, alias="generationConfig", description="Generation configuration."
     )
 
-    safety_settings: SafetySettings | dict | None = Field(
+    safety_settings: list[SafetySetting | dict] | None = Field(
         None, alias="safetySettings", description="Safety settings."
     )
```

### Comparing `gemini_ng-0.1.1/src/gemini_ng/schemas/response.py` & `gemini_ng-0.1.2/src/gemini_ng/schemas/response.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/schemas/upload.py` & `gemini_ng-0.1.2/src/gemini_ng/schemas/upload.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/utils/error.py` & `gemini_ng-0.1.2/src/gemini_ng/utils/error.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng/utils/video.py` & `gemini_ng-0.1.2/src/gemini_ng/utils/video.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.1/src/gemini_ng.egg-info/PKG-INFO` & `gemini_ng-0.1.2/src/gemini_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.1.1
+Version: 0.1.2
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 License: Copyright (c) 2024 Ming Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gemini_ng-0.1.1/src/gemini_ng.egg-info/SOURCES.txt` & `gemini_ng-0.1.2/src/gemini_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

