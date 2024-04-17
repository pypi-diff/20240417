# Comparing `tmp/photo_gps_client-0.1.5.tar.gz` & `tmp/photo_gps_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo_gps_client-0.1.5.tar", max compression
+gzip compressed data, was "photo_gps_client-0.1.6.tar", max compression
```

## Comparing `photo_gps_client-0.1.5.tar` & `photo_gps_client-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       49 2024-04-13 19:53:28.707149 photo_gps_client-0.1.5/README.md
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.5/photo_gps/DSCF0311.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.5/photo_gps/DSCF0312.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.5/photo_gps/DSCF0313.xmp
--rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.5/photo_gps/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-14 20:14:50.652061 photo_gps_client-0.1.5/photo_gps/commands.py
--rw-r--r--   0        0        0      307 2024-04-15 20:24:07.074275 photo_gps_client-0.1.5/photo_gps/photogps.example.yaml
--rw-r--r--   0        0        0     1880 2024-04-15 21:36:29.595295 photo_gps_client-0.1.5/photo_gps/photogps.py
--rw-r--r--   0        0        0     1952 2024-04-14 13:43:40.253343 photo_gps_client-0.1.5/photo_gps/tools.py
--rw-r--r--   0        0        0      668 2024-04-15 21:37:01.937423 photo_gps_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 photo_gps_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-04-17 18:35:03.061611 photo_gps_client-0.1.6/README.md
+-rw-r--r--   0        0        0      532 2024-04-17 16:36:49.817402 photo_gps_client-0.1.6/photo_gps/DSCF0311.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.6/photo_gps/DSCF0312.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.6/photo_gps/DSCF0313.xmp
+-rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.6/photo_gps/__init__.py
+-rw-r--r--   0        0        0     2711 2024-04-17 17:05:22.779144 photo_gps_client-0.1.6/photo_gps/commands.py
+-rw-r--r--   0        0        0     1272 2024-04-17 17:00:45.203444 photo_gps_client-0.1.6/photo_gps/config.py
+-rw-r--r--   0        0        0      551 2024-04-17 18:26:05.323417 photo_gps_client-0.1.6/photo_gps/jinja/xmp.jinja
+-rw-r--r--   0        0        0      327 2024-04-17 16:51:39.780517 photo_gps_client-0.1.6/photo_gps/photogps.example.yaml
+-rw-r--r--   0        0        0     1112 2024-04-17 17:01:24.642844 photo_gps_client-0.1.6/photo_gps/photogps.py
+-rw-r--r--   0        0        0     2881 2024-04-17 18:26:05.326871 photo_gps_client-0.1.6/photo_gps/tools.py
+-rw-r--r--   0        0        0      686 2024-04-17 18:31:44.388155 photo_gps_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 photo_gps_client-0.1.6/PKG-INFO
```

### Comparing `photo_gps_client-0.1.5/photo_gps/DSCF0311.xmp` & `photo_gps_client-0.1.6/photo_gps/DSCF0312.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.5/photo_gps/DSCF0312.xmp` & `photo_gps_client-0.1.6/photo_gps/DSCF0313.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.5/photo_gps/DSCF0313.xmp` & `photo_gps_client-0.1.6/photo_gps/DSCF0311.xmp`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <?xpacket begin='﻿' id='W5M0MpCehiHzreSzNTczkc9d'?>
 <x:xmpmeta xmlns:x='adobe:ns:meta/' x:xmptk='Image::ExifTool 12.70'>
 <rdf:RDF xmlns:rdf='http://www.w3.org/1999/02/22-rdf-syntax-ns#'>
 
- <rdf:Description rdf:about=''
-  xmlns:exif='http://ns.adobe.com/exif/1.0/'>
+ <rdf:Description rdf:about='' xmlns:exif='http://ns.adobe.com/exif/1.0/'>
   <exif:GPSAltitude>179073/1307</exif:GPSAltitude>
   <exif:GPSAltitudeRef>0</exif:GPSAltitudeRef>
   <exif:GPSLatitude>44,48.09288N</exif:GPSLatitude>
   <exif:GPSLongitude>20,29.46774E</exif:GPSLongitude>
  </rdf:Description>
 </rdf:RDF>
 </x:xmpmeta>
```

### Comparing `photo_gps_client-0.1.5/photo_gps/commands.py` & `photo_gps_client-0.1.6/photo_gps/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from pathlib import Path
 from colorama import Fore
 from tqdm import tqdm
 import requests
 
-from .tools import get_meta, get_all_meta, str_to_time, set_meta, set_author
+from .tools import get_meta, get_all_meta, str_to_time, set_meta, create_xmp
 
 
-def set_gps(path: str, user: str, token: str):
-    path = Path(path)
-
+def set_gps(path: Path, user: str, token: str, config: dict):
     images = []
-    # extensions = ['RAF', 'JPG', 'MP4']  RAF файлы ломаются при записи метаданных
-    extensions = ['JPG', 'jpg', 'MP4']
-    for ext in extensions:
-        for img in path.glob(f'**/*.{ext}'):
-            images.append(img)
+    for file in path.glob(f'**/*'):
+        if file.is_file():
+            suffix = file.suffix.lower()[1:]
+            if suffix in config['exif'] or suffix in config['xmp']:
+                images.append(file)
 
     ts_to_files = {}
 
     cnt_ok = cnt_todo = cnt_no_time = 0
     for img in tqdm(images, desc="Reading images"):
         tm, lat, lon, alt = get_meta(img)
         if not tm:
@@ -61,25 +59,18 @@
         return
     ts_to_loc = r.json()['ts_to_loc']
 
     for ts, files in tqdm(ts_to_files.items(), desc="Writing GPS data"):
         loc = ts_to_loc.get(str(ts))
         if loc:
             for img in files:
-                set_meta(img, loc[0], loc[1], loc[2])
-                # set_author(img, 'Anton Silin')
-                tqdm.write(f"{Fore.GREEN}{img.name} {loc}{Fore.RESET}")
+                if img.suffix.lower() in config['exif']:
+                    set_meta(img, loc[0], loc[1], loc[2])
+                    _mode = f'{Fore.BLUE}written to EXIF{Fore.RESET}'
+                else:
+                    create_xmp(img, loc[0], loc[1], loc[2])
+                    _mode = f'{Fore.CYAN}created .XMP file{Fore.RESET}'
+                tqdm.write(f"{img.name} {loc} {_mode}")
         else:
             for img in files:
                 tqdm.write(f"{Fore.RED}{img.name} no location{Fore.RESET}")
 
-    # metas = []
-    # for img in sorted(images):
-    #     metas.append(get_all_meta(img))
-    #
-    # for key in metas[0]:
-    #     # if 'GPS' not in key.upper():
-    #     #     continue
-    #     values = [meta.get(key) for meta in metas]
-    #     if len(set(values)) == 1:
-    #         print(f"{key.center(30)}: {values}")
-
```

### Comparing `photo_gps_client-0.1.5/photo_gps/tools.py` & `photo_gps_client-0.1.6/photo_gps/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 from pathlib import Path
 from exiftool import ExifToolHelper
 import arrow
+import os
+from pathlib import Path
+import yaml
+from colorama import Fore
+from jinja2 import Environment, PackageLoader, select_autoescape
 
 
 def str_to_time(time_str: str) -> int:
     # Конвертация строки в объект Arrow в локальной таймзоне
     arrow_obj = arrow.get(time_str, "YYYY:MM:DD HH:mm:ss", tzinfo="local")
 
     # Конвертация объекта Arrow в Unix timestamp
     unix_timestamp = arrow_obj.int_timestamp
 
     return unix_timestamp
 
 
+def deg_to_dms(deg, lat_or_lon):
+    letter = ''
+    if lat_or_lon == 'lat':
+        letter = 'N' if deg > 0 else 'S'
+    elif lat_or_lon == 'lon':
+        letter = 'E' if deg > 0 else 'W'
+    deg = abs(deg)
+    d = int(deg)
+    md = abs(deg - d) * 60
+    m = int(md)
+    sd = round((md - m) * 60, 2)
+    # return [d, m, sd]
+    return f"{d},{m},{sd}{letter}"
+
 def get_all_meta(img: Path) -> dict:
     with ExifToolHelper() as et:
         meta = et.get_tags(str(img), [])
         return meta[0]
 
+
 def get_meta(img: Path) -> [str, float, float, int]:
     with ExifToolHelper() as et:
         meta = et.get_tags(
             str(img),
             ['EXIF:DateTimeOriginal', 'EXIF:GPSLatitude', 'EXIF:GPSLongitude', 'EXIF:GPSAltitude']
         )
         meta = meta[0]
@@ -46,14 +66,26 @@
                 'EXIF:GPSAltitude': abs(alt),
                 'EXIF:GPSAltitudeRef': 0 if alt > 0 else 1
             },
             params=['-overwrite_original']
         )
 
 
+def create_xmp(img: Path, lat: float, lon: float, alt: int):
+    env = Environment(
+        loader=PackageLoader('photo_gps', 'jinja'),
+        autoescape=select_autoescape(['xml'])
+    )
+    tpl = env.get_template('xmp.jinja')
+    file_content = tpl.render(lat=deg_to_dms(lat, 'lat'), lon=deg_to_dms(lon, 'lon'), alt=alt)
+    xmp_file = img.with_suffix('.xmp')
+    with open(xmp_file, 'w') as f:
+        f.write(file_content)
+
+
 def set_author(img: Path, name: str):
     with ExifToolHelper() as et:
         res = et.set_tags(
             str(img),
             {
                 'Artist': name,
             },
```

### Comparing `photo_gps_client-0.1.5/pyproject.toml` & `photo_gps_client-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "photo-gps-client"
-version = "0.1.5"  # set by antonio-py-dynamic-version
+version = "0.1.6"  # set by antonio-py-dynamic-version
 description = ""
 authors = ["antonio <mr.antonsilin@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "photo_gps"},
 ]
 
@@ -15,14 +15,15 @@
 python = "^3.11"
 pyexiftool = "^0.5.6"
 colorama = "^0.4.6"
 arrow = "^1.3.0"
 tqdm = "^4.66.2"
 pyyaml = "^6.0.1"
 requests = "^2.31.0"
+jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 antonio-py-dynamic-version = {git = "https://bitbucket.org/asilin/antonio-py-dynamic-version.git"}
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `photo_gps_client-0.1.5/PKG-INFO` & `photo_gps_client-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: photo-gps-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pyexiftool (>=0.5.6,<0.6.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Dependencies
 
 https://exiftool.org/index.html
 
+# Publish:
+
+`poetry publish --build`
```

