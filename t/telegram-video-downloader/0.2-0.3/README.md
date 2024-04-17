# Comparing `tmp/telegram-video-downloader-0.2.tar.gz` & `tmp/telegram-video-downloader-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-video-downloader-0.2.tar", last modified: Wed Apr 17 19:57:59 2024, max compression
+gzip compressed data, was "telegram-video-downloader-0.3.tar", last modified: Wed Apr 17 20:00:49 2024, max compression
```

## Comparing `telegram-video-downloader-0.2.tar` & `telegram-video-downloader-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 19:57:59.813046 telegram-video-downloader-0.2/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:47:10.000000 telegram-video-downloader-0.2/LICENSE
--rw-rw-rw-   0        0        0      413 2024-04-17 19:57:59.810052 telegram-video-downloader-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       80 2024-04-17 15:43:12.000000 telegram-video-downloader-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 19:57:59.814050 telegram-video-downloader-0.2/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-04-17 19:57:38.000000 telegram-video-downloader-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 19:57:59.761754 telegram-video-downloader-0.2/telegram_video_downloader/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-0.2/telegram_video_downloader/__init__.py
--rw-rw-rw-   0        0        0     2613 2024-04-17 19:52:34.000000 telegram-video-downloader-0.2/telegram_video_downloader/app.py
-drwxrwxrwx   0        0        0        0 2024-04-17 19:57:59.805049 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 19:57:59.000000 telegram-video-downloader-0.2/telegram_video_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 20:00:49.496860 telegram-video-downloader-0.3/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:47:10.000000 telegram-video-downloader-0.3/LICENSE
+-rw-rw-rw-   0        0        0      299 2024-04-17 20:00:49.494852 telegram-video-downloader-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2024-04-17 15:43:12.000000 telegram-video-downloader-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:00:49.496860 telegram-video-downloader-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      586 2024-04-17 20:00:34.000000 telegram-video-downloader-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:00:49.463312 telegram-video-downloader-0.3/telegram_video_downloader/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-0.3/telegram_video_downloader/__init__.py
+-rw-rw-rw-   0        0        0     2613 2024-04-17 19:52:34.000000 telegram-video-downloader-0.3/telegram_video_downloader/app.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:00:49.492339 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/
+-rw-rw-rw-   0        0        0      299 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 20:00:49.000000 telegram-video-downloader-0.3/telegram_video_downloader.egg-info/top_level.txt
```

### Comparing `telegram-video-downloader-0.2/setup.py` & `telegram-video-downloader-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='telegram-video-downloader',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'quart',
         'telethon',
     ],
     author='David Grau Martínez',
     author_email='fe80grau@gmail.com',
     description='Command to download a video published on Telegram',
     keywords='telegram video download',
-    classifiers=[
-        'Programming Language :: Python :: 3.7',
-        'Framework :: Flask',  # Como alternativa, dada la similitud conceptual de Quart con Flask
-        'Topic :: Internet',
-    ],
     entry_points={
         'console_scripts': [
             'telegram-video-downloader=telegram_video_downloader.main:main',
         ],
     },
 )
```

### Comparing `telegram-video-downloader-0.2/telegram_video_downloader/app.py` & `telegram-video-downloader-0.3/telegram_video_downloader/app.py`

 * *Files identical despite different names*

