# Comparing `tmp/audio_toolkit-0.3.0.tar.gz` & `tmp/audio_toolkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_toolkit-0.3.0.tar", last modified: Wed Apr 17 08:47:16 2024, max compression
+gzip compressed data, was "audio_toolkit-0.4.0.tar", last modified: Wed Apr 17 08:48:46 2024, max compression
```

## Comparing `audio_toolkit-0.3.0.tar` & `audio_toolkit-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:47:16.659222 audio_toolkit-0.3.0/
--rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.3.0/LICENSE
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:47:16.659222 audio_toolkit-0.3.0/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.3.0/README.md
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:47:16.659222 audio_toolkit-0.3.0/audio_toolkit/
--rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.3.0/audio_toolkit/__init__.py
--rw-r--r--   0 khanh     (1004) asr      (10001)     7742 2024-04-17 08:47:06.000000 audio_toolkit-0.3.0/audio_toolkit/audio_stats.py
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:47:16.659222 audio_toolkit-0.3.0/audio_toolkit.egg-info/
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:47:16.000000 audio_toolkit-0.3.0/audio_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:47:16.000000 audio_toolkit-0.3.0/audio_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:47:16.000000 audio_toolkit-0.3.0/audio_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:47:16.000000 audio_toolkit-0.3.0/audio_toolkit.egg-info/requires.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:47:16.000000 audio_toolkit-0.3.0/audio_toolkit.egg-info/top_level.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:47:16.659222 audio_toolkit-0.3.0/setup.cfg
--rw-r--r--   0 khanh     (1004) asr      (10001)      610 2024-04-17 08:47:15.000000 audio_toolkit-0.3.0/setup.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:48:46.837609 audio_toolkit-0.4.0/
+-rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.4.0/LICENSE
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:48:46.837609 audio_toolkit-0.4.0/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.4.0/README.md
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:48:46.837609 audio_toolkit-0.4.0/audio_toolkit/
+-rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.4.0/audio_toolkit/__init__.py
+-rw-r--r--   0 khanh     (1004) asr      (10001)     7742 2024-04-17 08:48:35.000000 audio_toolkit-0.4.0/audio_toolkit/audio_stats.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:48:46.837609 audio_toolkit-0.4.0/audio_toolkit.egg-info/
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:48:46.000000 audio_toolkit-0.4.0/audio_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:48:46.000000 audio_toolkit-0.4.0/audio_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:48:46.000000 audio_toolkit-0.4.0/audio_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:48:46.000000 audio_toolkit-0.4.0/audio_toolkit.egg-info/requires.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:48:46.000000 audio_toolkit-0.4.0/audio_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:48:46.837609 audio_toolkit-0.4.0/setup.cfg
+-rw-r--r--   0 khanh     (1004) asr      (10001)      610 2024-04-17 08:48:45.000000 audio_toolkit-0.4.0/setup.py
```

### Comparing `audio_toolkit-0.3.0/LICENSE` & `audio_toolkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.3.0/audio_toolkit/audio_stats.py` & `audio_toolkit-0.4.0/audio_toolkit/audio_stats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -95,23 +95,23 @@
 class AudioStatsV2:
     def __init__(self, filename: str = "/tmp/audio_stats.sqlite", tablename: str = "audio_stats"):
         self.db = SqliteDict(filename=filename, tablename=tablename, autocommit=False)
         self.autocommit = True
     
     
     def __enter__(self) -> AudioStatsV2:
-        if self.autocommit == True:
+        if self.autocommit == False:
             raise RuntimeError("context cannot be entered multiple times")
         
         self.autocommit = False
 
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
-        if self.autocommit == False:
+        if self.autocommit == True:
             raise RuntimeError("context cannot be exited without entering")
         
         self.autocommit = True
 
     def ingest(self, cache_path: str="/tmp/audio_stats.json"):
         # load V1
         cache = {}
```

### Comparing `audio_toolkit-0.3.0/setup.py` & `audio_toolkit-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="audio-toolkit",
-        version="0.3.0",
+        version="0.4.0",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/audio-tools",
         packages=setuptools.find_packages(),
         license="MIT",
```

