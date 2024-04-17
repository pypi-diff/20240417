# Comparing `tmp/gamdl-2.1.7.tar.gz` & `tmp/gamdl-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.7.tar` & `gamdl-2.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-04-12 21:07:37.058617 gamdl-2.1.7/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-12 21:07:37.058617 gamdl-2.1.7/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-12 21:07:37.058617 gamdl-2.1.7/.gitignore
--rw-r--r--   0        0        0    11960 2024-04-12 21:07:37.058617 gamdl-2.1.7/README.md
--rw-r--r--   0        0        0       22 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26706 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/cli.py
--rw-r--r--   0        0        0     5580 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/constants.py
--rw-r--r--   0        0        0    12691 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader.py
--rw-r--r--   0        0        0    10566 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2254 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14069 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3865 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      817 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/models.py
--rw-r--r--   0        0        0      592 2024-04-12 21:07:37.058617 gamdl-2.1.7/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-12 21:07:37.058617 gamdl-2.1.7/requirements.txt
--rw-r--r--   0        0        0    12467 1970-01-01 00:00:00.000000 gamdl-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-17 00:24:01.918930 gamdl-2.1.8/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-04-17 00:24:01.918930 gamdl-2.1.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-17 00:24:01.918930 gamdl-2.1.8/.gitignore
+-rw-r--r--   0        0        0    12010 2024-04-17 00:24:01.918930 gamdl-2.1.8/README.md
+-rw-r--r--   0        0        0       22 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26698 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/cli.py
+-rw-r--r--   0        0        0     5580 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/constants.py
+-rw-r--r--   0        0        0    12691 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader.py
+-rw-r--r--   0        0        0    10587 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2290 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14184 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3922 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      817 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/models.py
+-rw-r--r--   0        0        0      587 2024-04-17 00:24:01.918930 gamdl-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-17 00:24:01.918930 gamdl-2.1.8/requirements.txt
+-rw-r--r--   0        0        0    12512 1970-01-01 00:00:00.000000 gamdl-2.1.8/PKG-INFO
```

### Comparing `gamdl-2.1.7/.github/workflows/main.yml` & `gamdl-2.1.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/README.md` & `gamdl-2.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Glomatico's Apple Music Downloader
-A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
+A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
+
+**Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
@@ -155,22 +157,22 @@
 * `ask`
     * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
-* `h264-best` (with AAC 256kbps, up to 1080p)
-* `h265-best` (With AAC 256kpbs, up to 2160p)
+* `h264-best` (up to 1080p, with AAC 256kbps)
+* `h265-best` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
-* `best` (with AAC 256kbps, up to 1080p)
+* `best` (up to 1080p, with AAC 256kbps)
 * `ask`
     * When using this option, gamdl will ask you which video quality to use that is available for the video.
 
 Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
```

### Comparing `gamdl-2.1.7/gamdl/apple_music_api.py` & `gamdl-2.1.8/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/gamdl/cli.py` & `gamdl-2.1.8/gamdl/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         return param.default.value
     elif isinstance(param.default, Path):
         return str(param.default)
     else:
         return param.default
 
 
-def write_default_config_file(ctx: click.Context) -> None:
+def write_default_config_file(ctx: click.Context):
     ctx.params["config_path"].parent.mkdir(parents=True, exist_ok=True)
     config_file = {
         param.name: get_param_string(param)
         for param in ctx.command.params
         if param.name not in EXCLUDED_CONFIG_FILE_PARAMS
     }
     ctx.params["config_path"].write_text(json.dumps(config_file, indent=4))
```

### Comparing `gamdl-2.1.7/gamdl/constants.py` & `gamdl-2.1.8/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/gamdl/downloader.py` & `gamdl-2.1.8/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/gamdl/downloader_music_video.py` & `gamdl-2.1.8/gamdl/downloader_music_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,25 +233,26 @@
         )
 
     def remux_mp4box(
         self,
         decrypted_path_audio: Path,
         decrypted_path_video: Path,
         fixed_path: Path,
-    ) -> None:
+    ):
         subprocess.run(
             [
                 self.downloader.mp4box_path_full,
                 "-quiet",
                 "-add",
                 decrypted_path_audio,
                 "-add",
                 decrypted_path_video,
                 "-itags",
                 "artist=placeholder",
+                "-keep-utc",
                 "-new",
                 fixed_path,
             ],
             check=True,
             **self.downloader.subprocess_additional_args,
         )
```

### Comparing `gamdl-2.1.7/gamdl/downloader_post.py` & `gamdl-2.1.8/gamdl/downloader_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import click
 from tabulate import tabulate
 
 from .downloader import Downloader
 from .enums import PostQuality
```

### Comparing `gamdl-2.1.7/gamdl/downloader_song.py` & `gamdl-2.1.8/gamdl/downloader_song.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,30 +174,32 @@
         text: str,
     ) -> str:
         timestamp_srt_start = self.get_lyrics_synced_timestamp_srt(timestamp_ttml_start)
         timestamp_srt_end = self.get_lyrics_synced_timestamp_srt(timestamp_ttml_end)
         return f"{index}\n{timestamp_srt_start} --> {timestamp_srt_end}\n{text}\n"
 
     def get_lyrics(self, track_metadata: dict) -> Lyrics:
+        lyrics = Lyrics()
         if not track_metadata["attributes"]["hasLyrics"]:
-            return Lyrics()
+            return lyrics
         elif track_metadata.get("relationships") is None:
             track_metadata = self.downloader.apple_music_api.get_song(
                 track_metadata["id"]
             )
-        if track_metadata["relationships"]["lyrics"]["data"] and track_metadata[
-            "relationships"
-        ]["lyrics"]["data"][0].get("attributes"):
-            return self._get_lyrics(
+        if (
+            track_metadata["relationships"].get("lyrics")
+            and track_metadata["relationships"]["lyrics"].get("data")
+            and track_metadata["relationships"]["lyrics"]["data"][0].get("attributes")
+        ):
+            lyrics = self._get_lyrics(
                 track_metadata["relationships"]["lyrics"]["data"][0]["attributes"][
                     "ttml"
                 ]
             )
-        else:
-            return Lyrics()
+        return lyrics
 
     def _get_lyrics(self, lyrics_ttml: str) -> Lyrics:
         lyrics = Lyrics("", "")
         lyrics_ttml_et = ElementTree.fromstring(lyrics_ttml)
         index = 1
         for div in lyrics_ttml_et.iter("{http://www.w3.org/ns/ttml}div"):
             for p in div.iter("{http://www.w3.org/ns/ttml}p"):
@@ -316,14 +318,15 @@
             [
                 self.downloader.mp4box_path_full,
                 "-quiet",
                 "-add",
                 decrypted_path,
                 "-itags",
                 "artist=placeholder",
+                "-keep-utc",
                 "-new",
                 remuxed_path,
             ],
             check=True,
             **self.downloader.subprocess_additional_args,
         )
```

### Comparing `gamdl-2.1.7/gamdl/downloader_song_legacy.py` & `gamdl-2.1.8/gamdl/downloader_song_legacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import base64
 import subprocess
 from pathlib import Path
 
 import m3u8
 from pywidevine import PSSH
 from pywidevine.license_protocol_pb2 import WidevinePsshData
@@ -61,23 +63,24 @@
                 f"1:{decryption_key}",
                 decrypted_path,
             ],
             check=True,
             **self.downloader.subprocess_additional_args,
         )
 
-    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path) -> None:
+    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path):
         subprocess.run(
             [
                 self.downloader.mp4box_path_full,
                 "-quiet",
                 "-add",
                 decrypted_path,
                 "-itags",
                 "artist=placeholder",
+                "-keep-utc",
                 "-new",
                 remuxed_path,
             ],
             check=True,
             **self.downloader.subprocess_additional_args,
         )
```

### Comparing `gamdl-2.1.7/gamdl/enums.py` & `gamdl-2.1.8/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/gamdl/hardcoded_wvd.py` & `gamdl-2.1.8/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/gamdl/itunes_api.py` & `gamdl-2.1.8/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.7/pyproject.toml` & `gamdl-2.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gamdl"
-description = "A Python script to download Apple Music songs/music videos/albums/playlists/post videos."
+description = "A Python CLI app to download Apple Music songs/music videos/albums/playlists/posts."
 requires-python = ">=3.8"
 authors = [{ name = "glomatico" }]
 dependencies = [
     "ciso8601",
     "click",
     "m3u8",
     "tabulate",
```

### Comparing `gamdl-2.1.7/PKG-INFO` & `gamdl-2.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.7
-Summary: A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
+Version: 2.1.8
+Summary: A Python CLI app to download Apple Music songs/music videos/albums/playlists/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
 Requires-Dist: tabulate
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: yt-dlp
 Project-URL: homepage, https://github.com/glomatico/gamdl
 Project-URL: repository, https://github.com/glomatico/gamdl
 
 # Glomatico's Apple Music Downloader
-A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
+A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
+
+**Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
@@ -172,22 +174,22 @@
 * `ask`
     * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
-* `h264-best` (with AAC 256kbps, up to 1080p)
-* `h265-best` (With AAC 256kpbs, up to 2160p)
+* `h264-best` (up to 1080p, with AAC 256kbps)
+* `h265-best` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
-* `best` (with AAC 256kbps, up to 1080p)
+* `best` (up to 1080p, with AAC 256kbps)
 * `ask`
     * When using this option, gamdl will ask you which video quality to use that is available for the video.
 
 Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
```

