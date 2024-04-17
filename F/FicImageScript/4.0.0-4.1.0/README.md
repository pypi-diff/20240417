# Comparing `tmp/FicImageScript-4.0.0.tar.gz` & `tmp/ficimagescript-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImageScript-4.0.0.tar", last modified: Wed Feb 28 15:25:06 2024, max compression
+gzip compressed data, was "ficimagescript-4.1.0.tar", last modified: Wed Apr 17 12:43:45 2024, max compression
```

## Comparing `FicImageScript-4.0.0.tar` & `ficimagescript-4.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 15:25:06.219533 FicImageScript-4.0.0/
-drwxrwxrwx   0        0        0        0 2024-02-28 15:25:06.207532 FicImageScript-4.0.0/FicImage/
--rw-rw-rw-   0        0        0        0 2024-02-22 14:12:50.000000 FicImageScript-4.0.0/FicImage/__init__.py
--rw-rw-rw-   0        0        0     5682 2024-02-22 14:12:50.000000 FicImageScript-4.0.0/FicImage/image.py
--rw-rw-rw-   0        0        0    10887 2024-02-28 15:12:49.000000 FicImageScript-4.0.0/FicImage/main.py
--rw-rw-rw-   0        0        0     2704 2024-02-28 14:16:52.000000 FicImageScript-4.0.0/FicImage/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:25:06.216531 FicImageScript-4.0.0/FicImageScript.egg-info/
--rw-rw-rw-   0        0        0     8630 2024-02-28 15:25:06.000000 FicImageScript-4.0.0/FicImageScript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-02-28 15:25:06.000000 FicImageScript-4.0.0/FicImageScript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 15:25:06.000000 FicImageScript-4.0.0/FicImageScript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-28 15:25:06.000000 FicImageScript-4.0.0/FicImageScript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2024-02-22 14:12:50.000000 FicImageScript-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     8630 2024-02-28 15:25:06.217648 FicImageScript-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6543 2024-02-22 14:12:50.000000 FicImageScript-4.0.0/PYPI_README.rst
--rw-rw-rw-   0        0        0     6076 2024-02-22 14:12:50.000000 FicImageScript-4.0.0/README.md
--rw-rw-rw-   0        0        0      959 2024-02-28 15:22:48.000000 FicImageScript-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 15:25:06.219533 FicImageScript-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-02-28 15:22:48.000000 FicImageScript-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:43:45.788344 ficimagescript-4.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-17 12:43:45.769441 ficimagescript-4.1.0/FicImage/
+-rw-rw-rw-   0        0        0        0 2024-02-22 14:12:50.000000 ficimagescript-4.1.0/FicImage/__init__.py
+-rw-rw-rw-   0        0        0     5991 2024-04-17 12:40:35.000000 ficimagescript-4.1.0/FicImage/image.py
+-rw-rw-rw-   0        0        0    10887 2024-04-17 12:40:35.000000 ficimagescript-4.1.0/FicImage/main.py
+-rw-rw-rw-   0        0        0     2704 2024-02-28 14:16:52.000000 ficimagescript-4.1.0/FicImage/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:43:45.782406 ficimagescript-4.1.0/FicImageScript.egg-info/
+-rw-rw-rw-   0        0        0     8630 2024-04-17 12:43:45.000000 ficimagescript-4.1.0/FicImageScript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-17 12:43:45.000000 ficimagescript-4.1.0/FicImageScript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:43:45.000000 ficimagescript-4.1.0/FicImageScript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 12:43:45.000000 ficimagescript-4.1.0/FicImageScript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2024-02-22 14:12:50.000000 ficimagescript-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8630 2024-04-17 12:43:45.785315 ficimagescript-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6543 2024-02-22 14:12:50.000000 ficimagescript-4.1.0/PYPI_README.rst
+-rw-rw-rw-   0        0        0     6076 2024-04-17 12:31:23.000000 ficimagescript-4.1.0/README.md
+-rw-rw-rw-   0        0        0      959 2024-04-17 12:40:35.000000 ficimagescript-4.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:43:45.789407 ficimagescript-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-17 12:40:35.000000 ficimagescript-4.1.0/setup.py
```

### Comparing `FicImageScript-4.0.0/FicImage/image.py` & `ficimagescript-4.1.0/FicImage/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,23 @@
 				)
 			
 			if compress_images:
 				compressed_base64_image = compress_image(BytesIO(imgdata), max_image_size, file_ext, debug)
 				imgdata = PIL_Image_to_bytes(compressed_base64_image, file_ext)
 				
 			return imgdata, file_ext, f"image/{file_ext}"
-		
+		elif url.startswith("https://imgur.com/"):
+			url = "https://i.imgur.com/" + url.split("https://imgur.com/")[-1]
+
 		with requests.Session() as session:
-			img = session.get(url, stream=True)
+			headers = {
+				'user-agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
+				              "Chrome/122.0.0.0 Safari/537.36"
+			}
+			img = session.get(url, stream=True, headers=headers)
 		
 			if img.headers.get("content-type", "") == "image/svg+xml":
 				return img.content, "svg", "image/svg+xml"
 			
 			image = BytesIO(img.content)
 			image.seek(0)
```

### Comparing `FicImageScript-4.0.0/FicImage/main.py` & `ficimagescript-4.1.0/FicImage/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import ebooklib
 from ebooklib import epub
 from bs4 import BeautifulSoup
 from .image import get_image_from_url
 from .utils import config_check, load_config_json, default_ficimage_settings
 
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 
 def update_epub(path_to_epub, config_file_path, debug):
     try:
         book = epub.read_epub(path_to_epub)
         print(f'Opened {path_to_epub}')
```

### Comparing `FicImageScript-4.0.0/FicImage/utils.py` & `ficimagescript-4.1.0/FicImage/utils.py`

 * *Files identical despite different names*

### Comparing `FicImageScript-4.0.0/FicImageScript.egg-info/PKG-INFO` & `ficimagescript-4.1.0/FicImageScript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 4.0.0
+Version: 4.1.0
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImageScript-4.0.0/LICENSE` & `ficimagescript-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImageScript-4.0.0/PKG-INFO` & `ficimagescript-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 4.0.0
+Version: 4.1.0
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImageScript-4.0.0/PYPI_README.rst` & `ficimagescript-4.1.0/PYPI_README.rst`

 * *Files identical despite different names*

### Comparing `FicImageScript-4.0.0/README.md` & `ficimagescript-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FicImageScript-4.0.0/pyproject.toml` & `ficimagescript-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FicImageScript"
-version = "4.0.0"
+version = "4.1.0"
 authors = [
   { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
 ]
 description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
 readme = "PYPI_README.rst"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
```

### Comparing `FicImageScript-4.0.0/setup.py` & `ficimagescript-4.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("PYPI_README.rst", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImageScript",
-	version="4.0.0",
+	version="4.1.0",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
```

