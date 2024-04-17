# Comparing `tmp/audio-toolkit-0.0.2.tar.gz` & `tmp/audio_toolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-toolkit-0.0.2.tar", last modified: Thu Jul 27 08:40:28 2023, max compression
+gzip compressed data, was "audio_toolkit-0.1.0.tar", last modified: Wed Apr 17 08:15:37 2024, max compression
```

## Comparing `audio-toolkit-0.0.2.tar` & `audio_toolkit-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-27 08:40:28.235147 audio-toolkit-0.0.2/
--rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-07-27 06:29:50.000000 audio-toolkit-0.0.2/LICENSE
--rw-r--r--   0 khanh      (501) staff       (20)      365 2023-07-27 08:40:28.234994 audio-toolkit-0.0.2/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      110 2023-07-27 06:29:50.000000 audio-toolkit-0.0.2/README.md
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-27 08:40:28.233876 audio-toolkit-0.0.2/audio_toolkit/
--rw-r--r--   0 khanh      (501) staff       (20)       89 2023-07-27 06:59:49.000000 audio-toolkit-0.0.2/audio_toolkit/__init__.py
--rw-r--r--   0 khanh      (501) staff       (20)      300 2023-07-27 08:40:04.000000 audio-toolkit-0.0.2/audio_toolkit/audio_converter.py
--rw-r--r--   0 khanh      (501) staff       (20)     5908 2023-07-27 06:45:46.000000 audio-toolkit-0.0.2/audio_toolkit/audio_stats.py
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-27 08:40:28.234784 audio-toolkit-0.0.2/audio_toolkit.egg-info/
--rw-r--r--   0 khanh      (501) staff       (20)      365 2023-07-27 08:40:28.000000 audio-toolkit-0.0.2/audio_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      298 2023-07-27 08:40:28.000000 audio-toolkit-0.0.2/audio_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 khanh      (501) staff       (20)        1 2023-07-27 08:40:28.000000 audio-toolkit-0.0.2/audio_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 khanh      (501) staff       (20)       13 2023-07-27 08:40:28.000000 audio-toolkit-0.0.2/audio_toolkit.egg-info/requires.txt
--rw-r--r--   0 khanh      (501) staff       (20)       14 2023-07-27 08:40:28.000000 audio-toolkit-0.0.2/audio_toolkit.egg-info/top_level.txt
--rw-r--r--   0 khanh      (501) staff       (20)       38 2023-07-27 08:40:28.235200 audio-toolkit-0.0.2/setup.cfg
--rw-r--r--   0 khanh      (501) staff       (20)      576 2023-07-27 08:40:22.000000 audio-toolkit-0.0.2/setup.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/
+-rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.1.0/LICENSE
+-rw-r--r--   0 khanh     (1004) asr      (10001)      393 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.1.0/README.md
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/audio_toolkit/
+-rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.1.0/audio_toolkit/__init__.py
+-rw-r--r--   0 khanh     (1004) asr      (10001)     7276 2024-04-04 09:17:39.000000 audio_toolkit-0.1.0/audio_toolkit/audio_stats.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/audio_toolkit.egg-info/
+-rw-r--r--   0 khanh     (1004) asr      (10001)      393 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       13 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/requires.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/setup.cfg
+-rw-r--r--   0 khanh     (1004) asr      (10001)      576 2024-04-17 08:15:24.000000 audio_toolkit-0.1.0/setup.py
```

### Comparing `audio-toolkit-0.0.2/LICENSE` & `audio_toolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-toolkit-0.0.2/audio_toolkit/audio_stats.py` & `audio_toolkit-0.1.0/audio_toolkit/audio_stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import contextlib
 import json
 import os
 import struct
 import wave
 from typing import *
-
+from sqlitedict import SqliteDict
 from tqdm import tqdm
 
 
 def bytes_to_int(bytes: list) -> int:
     result = 0
     for byte in bytes:
         result = (result << 8) + byte
@@ -88,14 +88,49 @@
 
 
 get_duration = {
     ".wav": get_wav_duration,
     ".flac": get_flac_duration,
 }
 
+class AudioStatsV2:
+    def __init__(self, filename: str = "/tmp/audio_stats.sqlite", tablename: str = "audio_stats", cache_path: str | None = None):
+        self.db = SqliteDict(filename=filename, tablename=tablename, autocommit=False)
+        # load V1
+        if cache_path is not None and os.path.exists(cache_path):
+            cache = {}
+            # read cache
+            with open(cache_path) as f:
+                for line in tqdm(list(f), desc=f"loading cache {cache_path}"):
+                    o = json.loads(line)
+                    path, frame_count, sample_rate = o["path"], o["frame_count"], o["sample_rate"]
+                    cache[path] = o
+            # write
+            for path, o in tqdm(cache.items(), desc=f"ingesting cache {filename}"):
+                self.db[path] = o
+            self.db.commit()
+
+    def get(self, path: str) -> Dict[str, Union[int, float]]:
+        path = os.path.realpath(path)
+
+        o = self.db.get(path, None)
+        if o is None:
+            ext = os.path.splitext(path)[1]
+            frame_count, sample_rate = get_duration[ext.lower()](path)
+
+            o = {
+                "path": path,
+                "frame_count": frame_count,
+                "sample_rate": sample_rate,
+            }
+            self.db[path] = o
+            self.db.commit()
+
+        return o
+
 
 class AudioStats:
     def __init__(self, cache_path: str = "/tmp/audio_stats.tmp"):
         self.cache_path = cache_path
         self.cache = {}
 
         self.opened = False
```

### Comparing `audio-toolkit-0.0.2/setup.py` & `audio_toolkit-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="audio-toolkit",
-        version="0.0.2",
+        version="0.1.0",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/audio-tools",
         packages=setuptools.find_packages(),
         license="MIT",
```

