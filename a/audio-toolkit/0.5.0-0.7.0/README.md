# Comparing `tmp/audio_toolkit-0.5.0.tar.gz` & `tmp/audio_toolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_toolkit-0.5.0.tar", last modified: Wed Apr 17 08:52:36 2024, max compression
+gzip compressed data, was "audio_toolkit-0.7.0.tar", last modified: Wed Apr 17 08:55:00 2024, max compression
```

## Comparing `audio_toolkit-0.5.0.tar` & `audio_toolkit-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:52:36.159798 audio_toolkit-0.5.0/
--rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.5.0/LICENSE
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:52:36.159798 audio_toolkit-0.5.0/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.5.0/README.md
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:52:36.159798 audio_toolkit-0.5.0/audio_toolkit/
--rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.5.0/audio_toolkit/__init__.py
--rw-r--r--   0 khanh     (1004) asr      (10001)     7702 2024-04-17 08:52:24.000000 audio_toolkit-0.5.0/audio_toolkit/audio_stats.py
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:52:36.159798 audio_toolkit-0.5.0/audio_toolkit.egg-info/
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:52:36.000000 audio_toolkit-0.5.0/audio_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:52:36.000000 audio_toolkit-0.5.0/audio_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:52:36.000000 audio_toolkit-0.5.0/audio_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:52:36.000000 audio_toolkit-0.5.0/audio_toolkit.egg-info/requires.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:52:36.000000 audio_toolkit-0.5.0/audio_toolkit.egg-info/top_level.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:52:36.159798 audio_toolkit-0.5.0/setup.cfg
--rw-r--r--   0 khanh     (1004) asr      (10001)      610 2024-04-17 08:52:31.000000 audio_toolkit-0.5.0/setup.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:55:00.860075 audio_toolkit-0.7.0/
+-rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.7.0/LICENSE
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:55:00.860075 audio_toolkit-0.7.0/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.7.0/README.md
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:55:00.860075 audio_toolkit-0.7.0/audio_toolkit/
+-rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.7.0/audio_toolkit/__init__.py
+-rw-r--r--   0 khanh     (1004) asr      (10001)     7702 2024-04-17 08:52:24.000000 audio_toolkit-0.7.0/audio_toolkit/audio_stats.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:55:00.860075 audio_toolkit-0.7.0/audio_toolkit.egg-info/
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:55:00.000000 audio_toolkit-0.7.0/audio_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:55:00.000000 audio_toolkit-0.7.0/audio_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:55:00.000000 audio_toolkit-0.7.0/audio_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:55:00.000000 audio_toolkit-0.7.0/audio_toolkit.egg-info/requires.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:55:00.000000 audio_toolkit-0.7.0/audio_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:55:00.860075 audio_toolkit-0.7.0/setup.cfg
+-rw-r--r--   0 khanh     (1004) asr      (10001)      790 2024-04-17 08:54:53.000000 audio_toolkit-0.7.0/setup.py
```

### Comparing `audio_toolkit-0.5.0/LICENSE` & `audio_toolkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.5.0/audio_toolkit/audio_stats.py` & `audio_toolkit-0.7.0/audio_toolkit/audio_stats.py`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.5.0/setup.py` & `audio_toolkit-0.7.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
+    
+    with open("version") as f:
+        version = int(f.read())
+
+    new_version = version+1
+    with open("version", "w") as f:
+        f.write(str(new_version))
 
     setuptools.setup(
         name="audio-toolkit",
-        version="0.5.0",
+        version=f"0.{new_version}.0",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/audio-tools",
         packages=setuptools.find_packages(),
         license="MIT",
```

