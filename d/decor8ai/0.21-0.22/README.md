# Comparing `tmp/decor8ai-0.21.tar.gz` & `tmp/decor8ai-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decor8ai-0.21.tar", max compression
+gzip compressed data, was "decor8ai-0.22.tar", max compression
```

## Comparing `decor8ai-0.21.tar` & `decor8ai-0.22.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11102 2024-04-15 18:41:58.478588 decor8ai-0.21/README.md
--rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.21/decor8ai/__init__.py
--rw-r--r--   0        0        0     6445 2024-04-15 17:37:52.313129 decor8ai-0.21/decor8ai/client.py
--rw-r--r--   0        0        0      534 2024-04-15 23:21:07.668205 decor8ai-0.21/pyproject.toml
--rw-r--r--   0        0        0    11782 1970-01-01 00:00:00.000000 decor8ai-0.21/PKG-INFO
+-rw-r--r--   0        0        0    11446 2024-04-17 17:24:20.585730 decor8ai-0.22/README.md
+-rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.22/decor8ai/__init__.py
+-rw-r--r--   0        0        0     7176 2024-04-17 17:15:42.773864 decor8ai-0.22/decor8ai/client.py
+-rw-r--r--   0        0        0      534 2024-04-17 17:27:02.341074 decor8ai-0.22/pyproject.toml
+-rw-r--r--   0        0        0    12126 1970-01-01 00:00:00.000000 decor8ai-0.22/PKG-INFO
```

### Comparing `decor8ai-0.21/README.md` & `decor8ai-0.22/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 The app specializes in virtual staging, transforming empty spaces into vivid, attractive interiors, enhancing their appeal for better marketability. 
 
 Equipped with a powerful Python SDK, Decor8 AI facilitates seamless integrations, enabling enhanced design generation capabilities directly within your Python environment. Its user-friendly interface is optimized for performance on smaller screens, ensuring that your design process is as effortless and efficient as possible.
 
 This documentation describes how you can use Decor8 AI Python SDK to integrate Decor8 AI's powerful features in your application. 
 
-Please reach out to [Decor8 AI Team](mailto:decor8@immex.tech) with questions or suggestions.
+See [complete documentation for Decor8 AI api for Virtual Staging and Interior Design](https://api-docs.decor8.ai/). Please reach out to [Decor8 AI Team](mailto:decor8@immex.tech) with questions or suggestions. 
 
 ## <a id="installation"></a>Installation
 
 You can install the Decor8 AI Python SDK using pip:
 
 ```bash
 pip install decor8ai
@@ -116,14 +116,18 @@
 design_style = 'frenchcountry' # See below for all supported design Styles
 num_images = 1 # Up to 4 images can be generated at a time
 
 # Optional Parameters
 num_captions = None # Choose 1 or 2 for number of image captions to generate
 
 response_json = generate_designs(room_type=room_type, design_style=design_style, num_images=num_images, num_captions=1)
+
+# If you like HTTP URLs for output, use new API
+from decor8ai.client import generate_inspirational_designs
+response_json = generate_inspirational_designs(room_type=room_type, design_style=design_style, num_images=num_images)
 ```
 
 ## <a id="prime-the-walls">Priming the walls
 
 If your room contains unfinished walls, unpainted walls or walls which need touch-up, use this API to get walls with basic white colored, smooth textured walls or as it's called 'primed walls'. 
 
 You can use the returned image as input to generate_designs API for filling it with furniture.
```

### Comparing `decor8ai-0.21/decor8ai/client.py` & `decor8ai-0.22/decor8ai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,14 +144,38 @@
         
     response = requests.post(url + '/generate_designs_for_room', headers=headers, data=data)
     
     response_json = json.loads(response.text)
     
     return response_json
 
+def generate_inspirational_designs(room_type, design_style, num_images=1,color_scheme=None, speciality_decor=None):
+    
+    if not token:
+        raise Exception("DECOR8AI_API_KEY environment variable is not set.")
+    
+    headers = {
+        'Authorization': f'Bearer {token}'
+    }
+    data = {
+        'room_type': room_type,
+        'design_style': design_style,
+        'num_images': num_images
+    }
+    if color_scheme:
+        data['color_scheme'] = color_scheme
+    if speciality_decor:
+        data['speciality_decor'] = speciality_decor
+
+    response = requests.post(url + '/generate_inspirational_designs', headers=headers, data=data)
+    
+    response_json = json.loads(response.text)
+    
+    return response_json
+
 def generate_image_captions(design_style, room_type, num_captions):
     
     if not token:
         raise Exception("DECOR8AI_API_KEY environment variable is not set.")
     
     headers = {
         'Authorization': f'Bearer {token}'
```

### Comparing `decor8ai-0.21/pyproject.toml` & `decor8ai-0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decor8ai"
-version = "0.21"
+version = "0.22"
 description = "Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos."
 authors = ["Akhilesh Joshi <akhilesh@immex.tech>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.decor8.ai"
 repository = "https://github.com/immex-tech/decor8ai-sdk"
```

### Comparing `decor8ai-0.21/PKG-INFO` & `decor8ai-0.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decor8ai
-Version: 0.21
+Version: 0.22
 Summary: Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos.
 Home-page: https://www.decor8.ai
 License: MIT
 Author: Akhilesh Joshi
 Author-email: akhilesh@immex.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 
 The app specializes in virtual staging, transforming empty spaces into vivid, attractive interiors, enhancing their appeal for better marketability. 
 
 Equipped with a powerful Python SDK, Decor8 AI facilitates seamless integrations, enabling enhanced design generation capabilities directly within your Python environment. Its user-friendly interface is optimized for performance on smaller screens, ensuring that your design process is as effortless and efficient as possible.
 
 This documentation describes how you can use Decor8 AI Python SDK to integrate Decor8 AI's powerful features in your application. 
 
-Please reach out to [Decor8 AI Team](mailto:decor8@immex.tech) with questions or suggestions.
+See [complete documentation for Decor8 AI api for Virtual Staging and Interior Design](https://api-docs.decor8.ai/). Please reach out to [Decor8 AI Team](mailto:decor8@immex.tech) with questions or suggestions. 
 
 ## <a id="installation"></a>Installation
 
 You can install the Decor8 AI Python SDK using pip:
 
 ```bash
 pip install decor8ai
@@ -133,14 +133,18 @@
 design_style = 'frenchcountry' # See below for all supported design Styles
 num_images = 1 # Up to 4 images can be generated at a time
 
 # Optional Parameters
 num_captions = None # Choose 1 or 2 for number of image captions to generate
 
 response_json = generate_designs(room_type=room_type, design_style=design_style, num_images=num_images, num_captions=1)
+
+# If you like HTTP URLs for output, use new API
+from decor8ai.client import generate_inspirational_designs
+response_json = generate_inspirational_designs(room_type=room_type, design_style=design_style, num_images=num_images)
 ```
 
 ## <a id="prime-the-walls">Priming the walls
 
 If your room contains unfinished walls, unpainted walls or walls which need touch-up, use this API to get walls with basic white colored, smooth textured walls or as it's called 'primed walls'. 
 
 You can use the returned image as input to generate_designs API for filling it with furniture.
```

