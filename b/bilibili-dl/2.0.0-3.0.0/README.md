# Comparing `tmp/bilibili-dl-2.0.0.tar.gz` & `tmp/bilibili_dl-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-dl-2.0.0.tar", last modified: Wed Mar 15 22:33:50 2023, max compression
+gzip compressed data, was "bilibili_dl-3.0.0.tar", last modified: Wed Apr 17 13:23:36 2024, max compression
```

## Comparing `bilibili-dl-2.0.0.tar` & `bilibili_dl-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2023-03-15 22:33:50.359208 bilibili-dl-2.0.0/
--rw-r--r--   0 youguang   (501) staff       (20)    19363 2023-03-15 18:24:02.000000 bilibili-dl-2.0.0/LICENSE
--rw-r--r--   0 youguang   (501) staff       (20)     1356 2023-03-15 22:33:50.359086 bilibili-dl-2.0.0/PKG-INFO
--rw-r--r--   0 youguang   (501) staff       (20)     1080 2023-03-15 22:14:04.000000 bilibili-dl-2.0.0/README.md
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2023-03-15 22:33:50.358428 bilibili-dl-2.0.0/bilibili_dl.egg-info/
--rw-r--r--   0 youguang   (501) staff       (20)     1356 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/PKG-INFO
--rw-r--r--   0 youguang   (501) staff       (20)      308 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/SOURCES.txt
--rw-r--r--   0 youguang   (501) staff       (20)        1 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/dependency_links.txt
--rw-r--r--   0 youguang   (501) staff       (20)       48 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/entry_points.txt
--rw-r--r--   0 youguang   (501) staff       (20)       26 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/requires.txt
--rw-r--r--   0 youguang   (501) staff       (20)        4 2023-03-15 22:33:50.000000 bilibili-dl-2.0.0/bilibili_dl.egg-info/top_level.txt
--rw-r--r--   0 youguang   (501) staff       (20)       38 2023-03-15 22:33:50.359245 bilibili-dl-2.0.0/setup.cfg
--rw-r--r--   0 youguang   (501) staff       (20)      641 2023-03-15 22:19:46.000000 bilibili-dl-2.0.0/setup.py
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2023-03-15 22:33:50.358934 bilibili-dl-2.0.0/src/
--rw-r--r--   0 youguang   (501) staff       (20)        0 2023-03-15 21:16:56.000000 bilibili-dl-2.0.0/src/__init__.py
--rw-r--r--   0 youguang   (501) staff       (20)       61 2023-03-15 22:22:47.000000 bilibili-dl-2.0.0/src/cli.py
--rw-r--r--   0 youguang   (501) staff       (20)     3341 2023-03-15 22:24:08.000000 bilibili-dl-2.0.0/src/downloader.py
--rw-r--r--   0 youguang   (501) staff       (20)     1438 2023-03-15 22:23:21.000000 bilibili-dl-2.0.0/src/main.py
--rw-r--r--   0 youguang   (501) staff       (20)     2117 2023-03-15 22:06:49.000000 bilibili-dl-2.0.0/src/utils.py
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.878344 bilibili_dl-3.0.0/
+-rw-r--r--   0 youguang   (501) staff       (20)    19363 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/LICENSE
+-rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-17 13:23:36.878153 bilibili_dl-3.0.0/PKG-INFO
+-rw-r--r--   0 youguang   (501) staff       (20)     1080 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/README.md
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.877136 bilibili_dl-3.0.0/bilibili_dl/
+-rw-r--r--   0 youguang   (501) staff       (20)        0 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/bilibili_dl/__init__.py
+-rw-r--r--   0 youguang   (501) staff       (20)       58 2024-04-17 13:13:19.000000 bilibili_dl-3.0.0/bilibili_dl/cli.py
+-rw-r--r--   0 youguang   (501) staff       (20)     3476 2024-04-17 13:13:23.000000 bilibili_dl-3.0.0/bilibili_dl/downloader.py
+-rw-r--r--   0 youguang   (501) staff       (20)     1408 2024-04-17 13:13:26.000000 bilibili_dl-3.0.0/bilibili_dl/main.py
+-rw-r--r--   0 youguang   (501) staff       (20)     2012 2024-04-17 13:14:08.000000 bilibili_dl-3.0.0/bilibili_dl/utils.py
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.877958 bilibili_dl-3.0.0/bilibili_dl.egg-info/
+-rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/PKG-INFO
+-rw-r--r--   0 youguang   (501) staff       (20)      348 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 youguang   (501) staff       (20)        1 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       56 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/entry_points.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       26 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/requires.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       12 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/top_level.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       38 2024-04-17 13:23:36.878380 bilibili_dl-3.0.0/setup.cfg
+-rw-r--r--   0 youguang   (501) staff       (20)      605 2024-04-17 12:58:39.000000 bilibili_dl-3.0.0/setup.py
```

### Comparing `bilibili-dl-2.0.0/LICENSE` & `bilibili_dl-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bilibili-dl-2.0.0/PKG-INFO` & `bilibili_dl-3.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: bilibili-dl
-Version: 2.0.0
+Version: 3.0.0
 Summary: Bilibili-dl 是一个下载B站音视频的工具（目前视频下载最高只支持720P）
 Home-page: https://github.com/Youguang-Zhou/bilibili-dl
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
+Requires-Dist: progressbar
 
 # Bilibili-dl
 
 ## 1. 简介
 
 Bilibili-dl 是一个下载 B 站音视频的工具（目前视频下载最高只支持720P）。
```

### Comparing `bilibili-dl-2.0.0/README.md` & `bilibili_dl-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bilibili-dl-2.0.0/bilibili_dl.egg-info/PKG-INFO` & `bilibili_dl-3.0.0/bilibili_dl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: bilibili-dl
-Version: 2.0.0
+Version: 3.0.0
 Summary: Bilibili-dl 是一个下载B站音视频的工具（目前视频下载最高只支持720P）
 Home-page: https://github.com/Youguang-Zhou/bilibili-dl
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
+Requires-Dist: progressbar
 
 # Bilibili-dl
 
 ## 1. 简介
 
 Bilibili-dl 是一个下载 B 站音视频的工具（目前视频下载最高只支持720P）。
```

### Comparing `bilibili-dl-2.0.0/src/downloader.py` & `bilibili_dl-3.0.0/bilibili_dl/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import re
 import subprocess
 import urllib.request
 
-from src.utils import *
+from .utils import *
 
 
 def download(videos, is_audio_only):
     for bvid, cid, title, up_name, cover_url in videos:
         params = {'bvid': bvid, 'cid': cid}
         if is_audio_only:
             params['fnval'] = '16'  # dash格式
         else:
-            params['fnval'] = '1'   # mp4格式
-            params['qn'] = '64'     # 720P画质
+            params['fnval'] = '1'  # mp4格式
+            params['qn'] = '64'  # 720P画质
 
         # 发送请求
         res = send_request(URL_PLAY, params)
 
         if is_audio_only:
             download_url = res['dash']['audio'][0]['base_url']
             # 如果标题里有书名号，则提取书名号里的内容作为新标题，否则保持原标题不变
@@ -50,24 +50,30 @@
             urllib.request.install_opener(opener)
             # 下载音频和封面
             urllib.request.urlretrieve(download_url, raw_fname, show_progress)
             urllib.request.urlretrieve(cover_url, cover_fname)
             # 添加封面到音频上
             print(f'[ffmpeg] 正在合并封面中...')
             if is_audio_only:
-                subprocess.call(f'ffmpeg -i "{raw_fname}" -i "{cover_fname}"     \
+                subprocess.call(
+                    f'ffmpeg -i "{raw_fname}" -i "{cover_fname}"                 \
                                          -loglevel error                         \
                                          -map 0:0 -map 1:0                       \
                                          -metadata album="{title}"               \
                                          -metadata artist="{up_name}"            \
                                          -metadata:s:v title="Album cover"       \
                                          -metadata:s:v comment="Cover (Front)"   \
-                                         -id3v2_version 3 -write_id3v1 1 "{final_fname}"', shell=True)
+                                         -id3v2_version 3 -write_id3v1 1 "{final_fname}"',
+                    shell=True,
+                )
             else:
-                subprocess.call(f'ffmpeg -i "{raw_fname}" -i "{cover_fname}"     \
+                subprocess.call(
+                    f'ffmpeg -i "{raw_fname}" -i "{cover_fname}"                 \
                                          -loglevel error                         \
                                          -map 1 -map 0                           \
                                          -c copy                                 \
-                                         -disposition:0 attached_pic "{final_fname}"', shell=True)
+                                         -disposition:0 attached_pic "{final_fname}"',
+                    shell=True,
+                )
             os.remove(raw_fname)
             os.remove(cover_fname)
             print(f'[bilibili-dl] ✅ 下载完成: {os.path.abspath(final_fname)}')
```

### Comparing `bilibili-dl-2.0.0/src/main.py` & `bilibili_dl-3.0.0/bilibili_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from argparse import ArgumentParser, BooleanOptionalAction
 import sys
+from argparse import ArgumentParser, BooleanOptionalAction
 
-from src.downloader import download
-from src.utils import *
+from .downloader import download
+from .utils import *
 
 
 def get_args():
     parser = ArgumentParser('Bilibili Downloader')
 
     parser.add_argument('bvid', nargs='?', help='BV号')
     parser.add_argument('--mid', help='up主id')
-    parser.add_argument('--audio-only', '-a',
-                        action=BooleanOptionalAction, default=False, help='仅下载音频')
+    parser.add_argument('--audio-only', '-a', action=BooleanOptionalAction, default=False, help='仅下载音频')
 
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit()
     else:
         return parser.parse_args()
```

### Comparing `bilibili-dl-2.0.0/src/utils.py` & `bilibili_dl-3.0.0/bilibili_dl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
 
 import progressbar
 import requests
 from tqdm import tqdm
 
-
 URL_SPACE = 'https://api.bilibili.com/x/space/wbi/arc/search'
 URL_VIDEO_INFO = 'https://api.bilibili.com/x/web-interface/view'
 URL_PLAY = 'https://api.bilibili.com/x/player/playurl'
 
 
 pbar = None
 
@@ -42,15 +41,15 @@
     获取该up主的所有投稿视频的BV号
     '''
     params = {'mid': mid, 'pn': '1', 'ps': '50'}
     try:
         res = send_request(URL_SPACE, params)
         total_pages = res['page']['count']
         bvids = [v['bvid'] for v in res['list']['vlist']]
-        for page_num in range(2, math.ceil(total_pages/int(params['ps']))+1):
+        for page_num in range(2, math.ceil(total_pages / int(params['ps'])) + 1):
             params['pn'] = page_num
             res = send_request(URL_SPACE, params)
             bvids.extend(v['bvid'] for v in res['list']['vlist'])
         return bvids
     except Exception:
         raise Exception('获取BV号失败！')
 
@@ -62,15 +61,11 @@
     try:
         print('[bilibili-dl] 获取视频详细信息中...')
         if type(bvids) == str:
             bvids = [bvids]
         videos = []
         for bvid in tqdm(bvids):
             res = send_request(URL_VIDEO_INFO, params={'bvid': bvid})
-            videos.append((res['bvid'],
-                           res['cid'],
-                           res['title'],
-                           res['owner']['name'],
-                           res['pic']))
+            videos.append((res['bvid'], res['cid'], res['title'], res['owner']['name'], res['pic']))
         return videos
     except Exception:
         raise Exception('获取视频详细信息失败！')
```

