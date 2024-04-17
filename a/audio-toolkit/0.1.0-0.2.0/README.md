# Comparing `tmp/audio_toolkit-0.1.0.tar.gz` & `tmp/audio_toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_toolkit-0.1.0.tar", last modified: Wed Apr 17 08:15:37 2024, max compression
+gzip compressed data, was "audio_toolkit-0.2.0.tar", last modified: Wed Apr 17 08:21:40 2024, max compression
```

## Comparing `audio_toolkit-0.1.0.tar` & `audio_toolkit-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/
--rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.1.0/LICENSE
--rw-r--r--   0 khanh     (1004) asr      (10001)      393 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.1.0/README.md
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/audio_toolkit/
--rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.1.0/audio_toolkit/__init__.py
--rw-r--r--   0 khanh     (1004) asr      (10001)     7276 2024-04-04 09:17:39.000000 audio_toolkit-0.1.0/audio_toolkit/audio_stats.py
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/audio_toolkit.egg-info/
--rw-r--r--   0 khanh     (1004) asr      (10001)      393 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       13 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/requires.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:15:37.000000 audio_toolkit-0.1.0/audio_toolkit.egg-info/top_level.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:15:37.244678 audio_toolkit-0.1.0/setup.cfg
--rw-r--r--   0 khanh     (1004) asr      (10001)      576 2024-04-17 08:15:24.000000 audio_toolkit-0.1.0/setup.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:21:40.430383 audio_toolkit-0.2.0/
+-rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.2.0/LICENSE
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:21:40.430383 audio_toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.2.0/README.md
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:21:40.430383 audio_toolkit-0.2.0/audio_toolkit/
+-rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.2.0/audio_toolkit/__init__.py
+-rw-r--r--   0 khanh     (1004) asr      (10001)     7276 2024-04-04 09:17:39.000000 audio_toolkit-0.2.0/audio_toolkit/audio_stats.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:21:40.430383 audio_toolkit-0.2.0/audio_toolkit.egg-info/
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/audio_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/audio_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/audio_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/audio_toolkit.egg-info/requires.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/audio_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:21:40.430383 audio_toolkit-0.2.0/setup.cfg
+-rw-r--r--   0 khanh     (1004) asr      (10001)      610 2024-04-17 08:21:40.000000 audio_toolkit-0.2.0/setup.py
```

### Comparing `audio_toolkit-0.1.0/LICENSE` & `audio_toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.1.0/audio_toolkit/audio_stats.py` & `audio_toolkit-0.2.0/audio_toolkit/audio_stats.py`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.1.0/setup.py` & `audio_toolkit-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="audio-toolkit",
-        version="0.1.0",
+        version="0.2.0",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/audio-tools",
         packages=setuptools.find_packages(),
         license="MIT",
         install_requires=[
-            "tqdm==4.65.0"
+            "tqdm==4.65.0",
+            "sqlitedict==2.1.0",
         ],
     )
```

