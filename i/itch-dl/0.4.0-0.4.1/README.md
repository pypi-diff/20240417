# Comparing `tmp/itch_dl-0.4.0.tar.gz` & `tmp/itch_dl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itch_dl-0.4.0.tar", max compression
+gzip compressed data, was "itch_dl-0.4.1.tar", max compression
```

## Comparing `itch_dl-0.4.0.tar` & `itch_dl-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2022-05-15 18:15:45.506900 itch_dl-0.4.0/LICENSE
--rw-r--r--   0        0        0     2533 2023-01-29 14:30:48.990460 itch_dl-0.4.0/README.md
--rw-r--r--   0        0        0       22 2024-03-16 23:37:09.398262 itch_dl-0.4.0/itch_dl/__init__.py
--rw-r--r--   0        0        0       57 2022-05-15 18:15:45.506900 itch_dl-0.4.0/itch_dl/__main__.py
--rw-r--r--   0        0        0     1914 2023-01-29 14:18:49.772600 itch_dl-0.4.0/itch_dl/api.py
--rw-r--r--   0        0        0     3149 2022-06-12 16:54:15.598930 itch_dl-0.4.0/itch_dl/cli.py
--rw-r--r--   0        0        0     1929 2022-06-12 16:57:16.783723 itch_dl-0.4.0/itch_dl/config.py
--rw-r--r--   0        0        0      428 2022-05-15 18:15:45.506900 itch_dl-0.4.0/itch_dl/consts.py
--rw-r--r--   0        0        0    14232 2023-01-29 14:15:09.970064 itch_dl-0.4.0/itch_dl/downloader.py
--rw-r--r--   0        0        0     8718 2024-03-16 22:38:57.811739 itch_dl-0.4.0/itch_dl/handlers.py
--rw-r--r--   0        0        0     4554 2024-03-16 22:38:57.811739 itch_dl-0.4.0/itch_dl/infobox.py
--rw-r--r--   0        0        0     1575 2024-03-16 22:38:57.811739 itch_dl-0.4.0/itch_dl/keys.py
--rw-r--r--   0        0        0     1027 2022-05-15 18:15:45.506900 itch_dl-0.4.0/itch_dl/utils.py
--rw-r--r--   0        0        0     1000 2024-03-16 23:43:02.907364 itch_dl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 itch_dl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-05-15 18:15:45.506900 itch_dl-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2533 2023-01-29 14:30:48.990460 itch_dl-0.4.1/README.md
+-rw-r--r--   0        0        0       22 2024-03-17 00:15:08.349607 itch_dl-0.4.1/itch_dl/__init__.py
+-rw-r--r--   0        0        0       58 2024-03-17 00:15:08.349607 itch_dl-0.4.1/itch_dl/__main__.py
+-rw-r--r--   0        0        0     1896 2024-03-17 00:18:54.245953 itch_dl-0.4.1/itch_dl/api.py
+-rw-r--r--   0        0        0     3220 2024-03-17 00:15:52.990031 itch_dl-0.4.1/itch_dl/cli.py
+-rw-r--r--   0        0        0     1930 2024-03-17 00:15:08.350607 itch_dl-0.4.1/itch_dl/config.py
+-rw-r--r--   0        0        0      428 2022-05-15 18:15:45.506900 itch_dl-0.4.1/itch_dl/consts.py
+-rw-r--r--   0        0        0    14678 2024-04-17 17:10:03.230143 itch_dl-0.4.1/itch_dl/downloader.py
+-rw-r--r--   0        0        0     8671 2024-03-17 00:15:08.350607 itch_dl-0.4.1/itch_dl/handlers.py
+-rw-r--r--   0        0        0     4554 2024-03-17 00:15:08.350607 itch_dl-0.4.1/itch_dl/infobox.py
+-rw-r--r--   0        0        0     1576 2024-03-17 00:15:08.350607 itch_dl-0.4.1/itch_dl/keys.py
+-rw-r--r--   0        0        0     1027 2022-05-15 18:15:45.506900 itch_dl-0.4.1/itch_dl/utils.py
+-rw-r--r--   0        0        0     1140 2024-04-17 17:11:40.172832 itch_dl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 itch_dl-0.4.1/PKG-INFO
```

### Comparing `itch_dl-0.4.0/LICENSE` & `itch_dl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itch_dl-0.4.0/README.md` & `itch_dl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `itch_dl-0.4.0/itch_dl/api.py` & `itch_dl-0.4.1/itch_dl/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 
 class ItchApiClient:
     def __init__(self, api_key: str, user_agent: str, base_url: Optional[str] = None):
         self.base_url = base_url or ITCH_API
         self.api_key = api_key
 
         self.requests = Session()
-        self.requests.headers['User-Agent'] = user_agent
+        self.requests.headers["User-Agent"] = user_agent
 
         retry_strategy = Retry(
             total=5,
             backoff_factor=10,
             allowed_methods=["HEAD", "GET"],
-            status_forcelist=[429, 500, 502, 503, 504]
+            status_forcelist=[429, 500, 502, 503, 504],
         )
 
         # No timeouts - set them explicitly on API calls below!
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self.requests.mount("https://", adapter)
         self.requests.mount("http://", adapter)
 
     def get(
-            self,
-            endpoint: str,
-            append_api_key: bool = True,
-            guess_encoding: bool = False,
-            **kwargs
+        self,
+        endpoint: str,
+        append_api_key: bool = True,
+        guess_encoding: bool = False,
+        **kwargs,
     ) -> requests.Response:
         """Wrapper around `requests.get`.
 
         :param endpoint: Path to fetch on the specified base URL.
         :param append_api_key: Send an authenticated API request.
         :param guess_encoding: Let requests guess the response encoding.
         """
         if append_api_key:
-            params = kwargs.get('data') or {}
+            params = kwargs.get("data") or {}
 
-            if 'api_key' not in params:
-                params['api_key'] = self.api_key
+            if "api_key" not in params:
+                params["api_key"] = self.api_key
 
-            kwargs['data'] = params
+            kwargs["data"] = params
 
         if endpoint.startswith("https://"):
             url = endpoint
         else:
             url = self.base_url + endpoint
 
         r = self.requests.get(url, **kwargs)
 
         # Itch always returns UTF-8 pages and API responses. Force
         # UTF-8 everywhere, except for binary file downloads.
         if not guess_encoding:
-            r.encoding = 'utf-8'
+            r.encoding = "utf-8"
 
         return r
```

### Comparing `itch_dl-0.4.0/itch_dl/cli.py` & `itch_dl-0.4.1/itch_dl/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .api import ItchApiClient
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
 
 def parse_args() -> argparse.Namespace:
+    # fmt: off
     parser = argparse.ArgumentParser(description="Bulk download stuff from Itch.io.")
     parser.add_argument("url_or_path",
                         help="itch.io URL or path to a game jam entries.json file")
     parser.add_argument("--api-key", metavar="key", default=None,
                         help="itch.io API key - https://itch.io/user/settings/api-keys")
     parser.add_argument("--profile", metavar="profile", default=None,
                         help="configuration profile to load")
@@ -27,14 +28,15 @@
     parser.add_argument("--parallel", metavar="parallel", type=int, default=1,
                         help="how many threads to use for downloading games (default: 1)")
     parser.add_argument("--mirror-web", action="store_true",
                         help="try to fetch assets on game sites")
     parser.add_argument("--verbose", action="store_true",
                         help="print verbose logs")
     return parser.parse_args()
+    # fmt: on
 
 
 def apply_args_on_settings(args: argparse.Namespace, settings: Settings):
     if args.api_key:
         settings.api_key = args.api_key
 
 
@@ -43,23 +45,27 @@
     if args.verbose:
         logging.getLogger().setLevel(logging.DEBUG)
 
     settings = load_config(profile=args.profile)
     apply_args_on_settings(args, settings)
 
     if not settings.api_key:
-        exit("You did not provide an API key which itch-dl requires.\n"
-             "See https://github.com/DragoonAethis/itch-dl/wiki/API-Keys for more info.")
+        exit(
+            "You did not provide an API key which itch-dl requires.\n"
+            "See https://github.com/DragoonAethis/itch-dl/wiki/API-Keys for more info."
+        )
 
     # Check API key validity:
     client = ItchApiClient(settings.api_key, settings.user_agent)
     profile_req = client.get("/profile")
     if not profile_req.ok:
-        exit(f"Provided API key appears to be invalid: {profile_req.text}\n"
-             "See https://github.com/DragoonAethis/itch-dl/wiki/API-Keys for more info.")
+        exit(
+            f"Provided API key appears to be invalid: {profile_req.text}\n"
+            "See https://github.com/DragoonAethis/itch-dl/wiki/API-Keys for more info."
+        )
 
     jobs = get_jobs_for_url_or_path(args.url_or_path, settings)
     jobs = list(set(jobs))  # Deduplicate, just in case...
     logging.info(f"Found {len(jobs)} URL(s).")
 
     if len(jobs) == 0:
         exit("No URLs to download.")
```

### Comparing `itch_dl-0.4.0/itch_dl/config.py` & `itch_dl-0.4.1/itch_dl/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 
 from . import __version__
 
 
 class Settings(BaseModel):
     """Available settings for itch-dl. Make sure all of them
     have default values, as the config file may not exist."""
+
     api_key: Optional[str] = None
     user_agent: str = f"python-requests/{requests.__version__} itch-dl/{__version__}"
 
 
 def create_and_get_config_path() -> str:
     """Returns the configuration directory in the appropriate
     location for the current OS. The directory may not exist."""
     system = platform.system()
     if system == "Linux":
-        base_path = os.environ.get('XDG_CONFIG_HOME') or os.path.expanduser('~/.config/')
+        base_path = os.environ.get("XDG_CONFIG_HOME") or os.path.expanduser("~/.config/")
     elif system == "Darwin":
-        base_path = os.path.expanduser('~/Library/Application Support/')
+        base_path = os.path.expanduser("~/Library/Application Support/")
     elif system == "Windows":
-        base_path = os.environ.get('APPDATA') or os.path.expanduser('~/AppData/Roaming/')
+        base_path = os.environ.get("APPDATA") or os.path.expanduser("~/AppData/Roaming/")
     else:
         raise NotImplementedError(f"Unknown platform: {system}")
 
     return os.path.join(base_path, "itch-dl")
 
 
 def load_config(profile: Optional[str] = None) -> Settings:
```

### Comparing `itch_dl-0.4.0/itch_dl/downloader.py` & `itch_dl-0.4.1/itch_dl/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 import json
 import re
 import logging
 import urllib.parse
 from typing import List, Dict, TypedDict, Optional, Union
 
 from bs4 import BeautifulSoup
-from requests.exceptions import HTTPError
+from requests.exceptions import HTTPError, JSONDecodeError
 
 from tqdm import tqdm
 from tqdm.contrib.concurrent import thread_map
 
 from .api import ItchApiClient
 from .utils import ItchDownloadError, get_int_after_marker_in_json
 from .consts import ITCH_GAME_URL_REGEX
 from .config import Settings
 from .infobox import parse_infobox, InfoboxMetadata
 
 TARGET_PATHS = {
-    'site': 'site.html',
-    'cover': 'cover',
-    'metadata': 'metadata.json',
-    'files': 'files',
-    'screenshots': 'screenshots'
+    "site": "site.html",
+    "cover": "cover",
+    "metadata": "metadata.json",
+    "files": "files",
+    "screenshots": "screenshots",
 }
 
 
 class DownloadResult:
     def __init__(self, url: str, success: bool, errors, external_urls: List[str]):
         self.url = url
         self.success = success
@@ -106,20 +106,29 @@
                 marker = "I.ViewGame"
                 if marker in script_src:
                     game_id = get_int_after_marker_in_json(script_src, marker, "id")
                     break
 
         if game_id is None:
             # We have to hit the server again :(
-            data_url = url.rstrip('/') + "/data.json"
+            data_url = url.rstrip("/") + "/data.json"
             data_request = self.client.get(data_url, append_api_key=False)
             if data_request.ok:
                 try:
-                    game_id = int(data_request.json().get("id"))
-                except ValueError:
+                    game_data = data_request.json()
+
+                    if "errors" in game_data:
+                        raise ItchDownloadError(
+                            f"Game data fetching failed for {url} "
+                            f"(likely access restricted, see issue #16): {game_data['errors']}"
+                        )
+
+                    if "id" in game_data:
+                        game_id = int(game_data["id"])
+                except (ValueError, TypeError, JSONDecodeError):
                     pass
 
         if game_id is None:
             raise ItchDownloadError(f"Could not get the Game ID for URL: {url}")
 
         return game_id
 
@@ -130,152 +139,156 @@
         description: Optional[str] = self.get_meta(site, property="og:description")
         if not description:
             description = self.get_meta(site, name="description")
 
         screenshot_urls: List[str] = []
         screenshots_node = site.find("div", class_="screenshot_list")
         if screenshots_node:
-            screenshot_urls = [a['href'] for a in screenshots_node.find_all('a')]
+            screenshot_urls = [a["href"] for a in screenshots_node.find_all("a")]
 
         metadata = GameMetadata(
             game_id=game_id,
             title=title or site.find("h1", class_="game_title").text.strip(),
             url=url,
             cover_url=self.get_meta(site, property="og:image"),
             screenshots=screenshot_urls,
             description=description,
         )
 
         infobox_div = site.find("div", class_="game_info_panel_widget")
         if infobox_div:
             infobox = parse_infobox(infobox_div)
-            for dt in ('created_at', 'updated_at', 'released_at', 'published_at'):
+            for dt in ("created_at", "updated_at", "released_at", "published_at"):
                 if dt in infobox:
                     metadata[dt] = infobox[dt].isoformat()  # noqa (non-literal TypedDict keys)
                     del infobox[dt]  # noqa (non-literal TypedDict keys)
 
-            if 'author' in infobox:
-                metadata['author'] = infobox['author']['author']
-                metadata['author_url'] = infobox['author']['author_url']
-                del infobox['author']
+            if "author" in infobox:
+                metadata["author"] = infobox["author"]["author"]
+                metadata["author_url"] = infobox["author"]["author_url"]
+                del infobox["author"]
 
-            if 'authors' in infobox and 'author' not in metadata:
+            if "authors" in infobox and "author" not in metadata:
                 # Some games may have multiple authors (ex. compilations).
-                metadata['author'] = "Multiple authors"
-                metadata['author_url'] = f"https://{urllib.parse.urlparse(url).netloc}"
+                metadata["author"] = "Multiple authors"
+                metadata["author_url"] = f"https://{urllib.parse.urlparse(url).netloc}"
 
-            metadata['extra'] = infobox
+            metadata["extra"] = infobox
 
-        agg_rating = rating_json.get('aggregateRating') if rating_json else None
+        agg_rating = rating_json.get("aggregateRating") if rating_json else None
         if agg_rating:
             try:
-                metadata['rating'] = {
-                    'average': float(agg_rating['ratingValue']),
-                    'votes': agg_rating['ratingCount']
-                }
+                metadata["rating"] = {"average": float(agg_rating["ratingValue"]), "votes": agg_rating["ratingCount"]}
             except:  # noqa
                 logging.exception("Could not extract the rating metadata...")
                 pass  # Nope, just, don't
 
         return metadata
 
     def get_credentials(self, title: str, game_id: int) -> dict:
         credentials = {}
         if game_id in self.download_keys:
-            credentials['download_key_id'] = self.download_keys[game_id]
+            credentials["download_key_id"] = self.download_keys[game_id]
             logging.debug("Got credentials for %s: %s", title, str(credentials))
 
         return credentials
 
     def download_file(self, url: str, download_path: Optional[str], credentials: dict) -> str:
         """Performs a request to download a given file, optionally saves the
         file to the provided path and returns the final URL that was downloaded."""
         try:
             # No timeouts, chunked uploads, default retry strategy, should be all good?
             with self.client.get(url, data=credentials, stream=True, guess_encoding=True) as r:
                 r.raise_for_status()
 
                 if download_path is not None:  # ...and it will be for external downloads.
-                    with tqdm.wrapattr(open(download_path, "wb"), "write",
-                                       miniters=1, desc=url,
-                                       total=int(r.headers.get('content-length', 0))) as f:
+                    with tqdm.wrapattr(
+                        open(download_path, "wb"),
+                        "write",
+                        miniters=1,
+                        desc=url,
+                        total=int(r.headers.get("content-length", 0)),
+                    ) as f:
                         for chunk in r.iter_content(chunk_size=1048576):  # 1MB chunks
                             f.write(chunk)
 
                 return r.url
         except HTTPError as e:
-            raise ItchDownloadError(f"Unrecoverable download error: {e}")
+            raise ItchDownloadError(f"Unrecoverable download error: {e}") from e
 
     def download_file_by_upload_id(self, upload_id: int, download_path: Optional[str], credentials: dict) -> str:
         """Performs a request to download a given upload by its ID."""
         return self.download_file(f"/uploads/{upload_id}/download", download_path, credentials)
 
     def download(self, url: str, skip_downloaded: bool = True):
         match = re.match(ITCH_GAME_URL_REGEX, url)
         if not match:
             return DownloadResult(url, False, [f"Game URL is invalid: {url} - please file a new issue."], [])
 
-        author, game = match['author'], match['game']
+        author, game = match["author"], match["game"]
 
         download_path = os.path.join(self.download_to, author, game)
         os.makedirs(download_path, exist_ok=True)
 
         paths: Dict[str, str] = {k: os.path.join(download_path, v) for k, v in TARGET_PATHS.items()}
 
-        if os.path.exists(paths['metadata']) and skip_downloaded:
+        if os.path.exists(paths["metadata"]) and skip_downloaded:
             # As metadata is the final file we write, all the files
             # should already be downloaded at this point.
             logging.info("Skipping already-downloaded game for URL: %s", url)
-            return DownloadResult(url, True, [f"Game already downloaded."], [])
+            return DownloadResult(url, True, ["Game already downloaded."], [])
 
         try:
             logging.info("Downloading %s", url)
             r = self.client.get(url, append_api_key=False)
             r.raise_for_status()
         except Exception as e:
             return DownloadResult(url, False, [f"Could not download the game site for {url}: {e}"], [])
 
         site = BeautifulSoup(r.text, features="lxml")
         try:
             game_id = self.get_game_id(url, site)
             metadata = self.extract_metadata(game_id, url, site)
-            title = metadata['title'] or game
+            title = metadata["title"] or game
         except ItchDownloadError as e:
             return DownloadResult(url, False, [str(e)], [])
 
         credentials = self.get_credentials(title, game_id)
         try:
             game_uploads_req = self.client.get(f"/games/{game_id}/uploads", data=credentials, timeout=15)
             game_uploads_req.raise_for_status()
         except Exception as e:
             return DownloadResult(url, False, [f"Could not fetch game uploads for {title}: {e}"], [])
 
-        game_uploads = game_uploads_req.json()['uploads']
+        game_uploads = game_uploads_req.json()["uploads"]
         logging.debug("Found %d upload(s): %s", len(game_uploads), str(game_uploads))
 
         external_urls = []
         errors = []
 
         try:
-            os.makedirs(paths['files'], exist_ok=True)
+            os.makedirs(paths["files"], exist_ok=True)
             for upload in game_uploads:
-                if any([key not in upload for key in ('id', 'filename', 'storage')]):
+                if any(key not in upload for key in ("id", "filename", "storage")):
                     errors.append(f"Upload metadata incomplete: {upload}")
                     continue
 
-                upload_id = upload['id']
-                file_name = upload['filename']
-                file_size = upload.get('size')
-                upload_is_external = upload['storage'] == 'external'
-
-                logging.debug("Downloading '%s' (%d), %s",
-                              file_name, upload_id,
-                              f"{file_size} bytes" if file_size is not None else "unknown size")
+                upload_id = upload["id"]
+                file_name = upload["filename"]
+                file_size = upload.get("size")
+                upload_is_external = upload["storage"] == "external"
+
+                logging.debug(
+                    "Downloading '%s' (%d), %s",
+                    file_name,
+                    upload_id,
+                    f"{file_size} bytes" if file_size is not None else "unknown size",
+                )
 
-                target_path = None if upload_is_external else os.path.join(paths['files'], file_name)
+                target_path = None if upload_is_external else os.path.join(paths["files"], file_name)
 
                 try:
                     target_url = self.download_file_by_upload_id(upload_id, target_path, credentials)
                 except ItchDownloadError as e:
                     errors.append(f"Download failed for upload {upload}: {e}")
                     continue
 
@@ -290,60 +303,60 @@
                 except FileNotFoundError:
                     errors.append(f"Downloaded file not found for upload {upload}")
 
             logging.debug("Done downloading files for %s", title)
         except Exception as e:
             errors.append(f"Download failed for {title}: {e}")
 
-        metadata['errors'] = errors
-        metadata['external_downloads'] = external_urls
+        metadata["errors"] = errors
+        metadata["external_downloads"] = external_urls
 
         if len(external_urls) > 0:
             logging.warning(f"Game {title} has external download URLs: {external_urls}")
 
         # TODO: Mirror JS/CSS assets
         if self.mirror_web:
-            os.makedirs(paths['screenshots'], exist_ok=True)
-            for screenshot in metadata['screenshots']:
+            os.makedirs(paths["screenshots"], exist_ok=True)
+            for screenshot in metadata["screenshots"]:
                 if not screenshot:
                     continue
 
                 file_name = os.path.basename(screenshot)
                 try:
-                    self.download_file(screenshot, os.path.join(paths['screenshots'], file_name), credentials={})
+                    self.download_file(screenshot, os.path.join(paths["screenshots"], file_name), credentials={})
                 except Exception as e:
                     errors.append(f"Screenshot download failed (this is not fatal): {e}")
 
-        cover_url = metadata.get('cover_url')
+        cover_url = metadata.get("cover_url")
         if cover_url:
             try:
-                self.download_file(cover_url, paths['cover'] + os.path.splitext(cover_url)[-1], credentials={})
+                self.download_file(cover_url, paths["cover"] + os.path.splitext(cover_url)[-1], credentials={})
             except Exception as e:
                 errors.append(f"Cover art download failed (this is not fatal): {e}")
 
-        with open(paths['site'], 'wb') as f:
-            f.write(site.prettify(encoding='utf-8'))
+        with open(paths["site"], "wb") as f:
+            f.write(site.prettify(encoding="utf-8"))
 
-        with open(paths['metadata'], 'w') as f:
+        with open(paths["metadata"], "w") as f:
             json.dump(metadata, f, indent=4)
 
         if len(errors) > 0:
             logging.error(f"Game {title} has download errors: {errors}")
 
         logging.info("Finished job %s (%s)", url, title)
         return DownloadResult(url, len(errors) == 0, errors, external_urls)
 
 
 def drive_downloads(
-        jobs: List[str],
-        download_to: str,
-        mirror_web: bool,
-        settings: Settings,
-        keys: Dict[int, str],
-        parallel: int = 1
+    jobs: List[str],
+    download_to: str,
+    mirror_web: bool,
+    settings: Settings,
+    keys: Dict[int, str],
+    parallel: int = 1,
 ):
     downloader = GameDownloader(download_to, mirror_web, settings, keys)
     tqdm_args = {
         "desc": "Games",
         "unit": "game",
     }
```

### Comparing `itch_dl-0.4.0/itch_dl/handlers.py` & `itch_dl-0.4.1/itch_dl/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 from .utils import ItchDownloadError, get_int_after_marker_in_json
 from .consts import ITCH_API, ITCH_BASE, ITCH_URL, ITCH_BROWSER_TYPES
 from .config import Settings
 from .keys import get_owned_games
 
 
 def get_jobs_for_game_jam_json(game_jam_json: dict) -> List[str]:
-    if 'jam_games' not in game_jam_json:
+    if "jam_games" not in game_jam_json:
         raise Exception("Provided JSON is not a valid itch.io jam JSON.")
 
-    return [g['game']['url'] for g in game_jam_json['jam_games']]
+    return [g["game"]["url"] for g in game_jam_json["jam_games"]]
 
 
 def get_game_jam_json(jam_url: str, client: ItchApiClient) -> dict:
     r = client.get(jam_url)
     if not r.ok:
         raise ItchDownloadError(f"Could not download the game jam site: {r.status_code} {r.reason}")
 
     jam_id: Optional[int] = get_int_after_marker_in_json(r.text, "I.ViewJam", "id")
     if jam_id is None:
-        raise ItchDownloadError("Provided site did not contain the Game Jam ID. Provide "
-                                "the path to the game jam entries JSON file instead, or "
-                                "create an itch-dl issue with the Game Jam URL.")
+        raise ItchDownloadError(
+            "Provided site did not contain the Game Jam ID. Provide "
+            "the path to the game jam entries JSON file instead, or "
+            "create an itch-dl issue with the Game Jam URL."
+        )
 
     logging.info(f"Extracted Game Jam ID: {jam_id}")
     r = client.get(f"{ITCH_URL}/jam/{jam_id}/entries.json")
     if not r.ok:
         raise ItchDownloadError(f"Could not download the game jam entries list: {r.status_code} {r.reason}")
 
     return r.json()
@@ -47,15 +49,15 @@
     the last returned <channel> has no <item> children.
 
     The input URL is cleaned in the main URL handler, so append the
     .xml?page=N suffix and iterate until we've caught 'em all.
     """
     page = 1
     found_urls: Set[str] = set()
-    logging.info(f"Scraping game URLs from RSS feeds for %s", url)
+    logging.info("Scraping game URLs from RSS feeds for %s", url)
 
     while True:
         logging.info(f"Downloading page {page} (found {len(found_urls)} URLs total)")
         r = client.get(f"{url}.xml?page={page}", append_api_key=False)
         if not r.ok:
             logging.info("RSS feed returned %s, finished.", r.reason)
             break
@@ -88,16 +90,15 @@
     page = 1
     found_urls: Set[str] = set()
 
     while True:
         logging.info(f"Downloading page {page} (found {len(found_urls)} URLs total)")
         r = client.get(url, data={"page": page}, timeout=15)
         if not r.ok:
-            logging.info("Collection page %d returned %d %s, finished.",
-                         page, r.status_code, r.reason)
+            logging.info("Collection page %d returned %d %s, finished.", page, r.status_code, r.reason)
             break
 
         data = r.json()
 
         if len(data["collection_games"]) < 1:
             logging.info("No more items, finished.")
             break
@@ -119,18 +120,18 @@
 def get_jobs_for_itch_url(url: str, client: ItchApiClient) -> List[str]:
     if url.startswith("http://"):
         logging.info("HTTP link provided, upgrading to HTTPS")
         url = "https://" + url[7:]
 
     if url.startswith(f"https://www.{ITCH_BASE}/"):
         logging.info(f"Correcting www.{ITCH_BASE} to {ITCH_BASE}")
-        url = ITCH_URL + '/' + url[20:]
+        url = ITCH_URL + "/" + url[20:]
 
     url_parts = urllib.parse.urlparse(url)
-    url_path_parts: List[str] = [x for x in str(url_parts.path).split('/') if len(x) > 0]
+    url_path_parts: List[str] = [x for x in str(url_parts.path).split("/") if len(x) > 0]
 
     if url_parts.netloc == ITCH_BASE:
         if len(url_path_parts) == 0:
             raise NotImplementedError("itch-dl cannot download the entirety of itch.io.")
         # (yet) (also leafo would not be happy with the bandwidth bill)
 
         site = url_path_parts[0]
@@ -141,15 +142,15 @@
 
             logging.info("Fetching Game Jam JSON...")
             clean_game_jam_url = f"{ITCH_URL}/jam/{url_path_parts[1]}"
             game_jam_json = get_game_jam_json(clean_game_jam_url, client)
             return get_jobs_for_game_jam_json(game_jam_json)
 
         elif site in ITCH_BROWSER_TYPES:  # Browser
-            clean_browse_url = '/'.join([ITCH_URL, *url_path_parts])
+            clean_browse_url = "/".join([ITCH_URL, *url_path_parts])
             return get_jobs_for_browse_url(clean_browse_url, client)
 
         elif site in ("b", "bundle"):  # Bundles
             raise NotImplementedError("itch-dl cannot download bundles yet.")
 
         elif site in ("j", "jobs"):  # Jobs...
             raise ValueError("itch-dl cannot download a job.")
@@ -170,15 +171,15 @@
 
         elif site == "c":  # Collections
             collection_id = url_path_parts[1]
             clean_collection_url = f"{ITCH_API}/collections/{collection_id}/collection-games"
             return get_jobs_for_collection_json(clean_collection_url, client)
 
         # Something else?
-        raise NotImplementedError(f"itch-dl does not understand \"{site}\" URLs. Please file a new issue.")
+        raise NotImplementedError(f'itch-dl does not understand "{site}" URLs. Please file a new issue.')
 
     elif url_parts.netloc.endswith(f".{ITCH_BASE}"):
         if len(url_path_parts) == 0:  # Author
             # TODO: Find I.UserPage, regex for "user_id": [0-9]+, find the responsible API?
             raise NotImplementedError("itch-dl cannot download author pages yet.")
 
         else:  # Single game
@@ -193,15 +194,15 @@
     try:  # Game Jam Entries JSON?
         with open(path, "rb") as f:
             json_data = json.load(f)
 
         if not isinstance(json_data, dict):
             raise ValueError(f"File does not contain a JSON dict: {path}")
 
-        if 'jam_games' in json_data:
+        if "jam_games" in json_data:
             logging.info("Parsing provided file as a Game Jam Entries JSON...")
             return get_jobs_for_game_jam_json(json_data)
     except json.JSONDecodeError:
         pass  # Not a valid JSON, okay...
 
     url_list = []
     with open(path) as f:  # Plain job list?
@@ -210,15 +211,15 @@
             if line.startswith("https://") or line.startswith("http://"):
                 url_list.append(line)
 
     if len(url_list) > 0:
         logging.info("Parsing provided file as a list of URLs to fetch...")
         return url_list
 
-    raise ValueError(f"File format is unknown - cannot read URLs to download.")
+    raise ValueError("File format is unknown - cannot read URLs to download.")
 
 
 def get_jobs_for_url_or_path(path_or_url: str, settings: Settings) -> List[str]:
     """Returns a list of Game URLs for a given itch.io URL or file."""
     path_or_url = path_or_url.strip()
 
     if path_or_url.startswith("http://"):
```

### Comparing `itch_dl-0.4.0/itch_dl/infobox.py` & `itch_dl-0.4.1/itch_dl/infobox.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     links: Dict[str, str]  # Links
     mentions: Dict[str, str]  # Links
     category: Dict[str, str]  # Links
 
 
 def parse_date_block(td: BeautifulSoup) -> Optional[datetime]:
     abbr = td.find("abbr")
-    if not abbr or 'title' not in abbr.attrs:
+    if not abbr or "title" not in abbr.attrs:
         return None
 
-    date_str, time_str = abbr['title'].split('@')
+    date_str, time_str = abbr["title"].split("@")
     date = datetime.strptime(date_str.strip(), "%d %B %Y")
     time = datetime.strptime(time_str.strip(), "%H:%M UTC")
     return datetime(date.year, date.month, date.day, time.hour, time.minute)
 
 
 def parse_links(td: BeautifulSoup) -> Dict[str, str]:
     """Parses blocks of comma-separated <a> blocks, returns a dict
     of link text -> URL it points at."""
-    return {link.text.strip(): link['href'] for link in td.find_all("a")}
+    return {link.text.strip(): link["href"] for link in td.find_all("a")}
 
 
 def parse_text_from_links(td: BeautifulSoup) -> List[str]:
     return list(parse_links(td).keys())
 
 
 def parse_tr(name: str, content: BeautifulSoup) -> Optional[Tuple[str, Any]]:
```

### Comparing `itch_dl-0.4.0/itch_dl/keys.py` & `itch_dl-0.4.1/itch_dl/keys.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     while True:
         logging.info(f"Downloading page {page} (found {len(download_keys)} keys total)")
         r = client.get("/profile/owned-keys", data={"page": page}, timeout=15)
         if not r.ok:
             break
 
         data = r.json()
-        if 'owned_keys' not in data:
+        if "owned_keys" not in data:
             break  # Assuming we're out of keys already...
 
-        for key in data['owned_keys']:
-            download_keys[key['game_id']] = key['id']
-            game_urls.append(key['game']['url'])
+        for key in data["owned_keys"]:
+            download_keys[key["game_id"]] = key["id"]
+            game_urls.append(key["game"]["url"])
 
-        if len(data['owned_keys']) == data['per_page']:
+        if len(data["owned_keys"]) == data["per_page"]:
             page += 1
         else:
             break
 
     logging.info(f"Fetched {len(download_keys)} download keys.")
 
     cached_owned_keys = (download_keys, game_urls)
@@ -46,8 +46,8 @@
 def get_download_keys(client: ItchApiClient) -> Dict[int, str]:
     (download_keys, _) = get_owned_keys(client)
     return download_keys
 
 
 def get_owned_games(client: ItchApiClient) -> List[str]:
     (_, game_urls) = get_owned_keys(client)
-    return game_urls
+    return game_urls
```

### Comparing `itch_dl-0.4.0/itch_dl/utils.py` & `itch_dl-0.4.1/itch_dl/utils.py`

 * *Files identical despite different names*

### Comparing `itch_dl-0.4.0/pyproject.toml` & `itch_dl-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "itch-dl"
 packages = [{ include = "itch_dl" }]
-version = "0.4.0"
+version = "0.4.1"
 description = "itch.io bulk game downloader"
 homepage = "https://github.com/DragoonAethis/itch-dl"
 repository = "https://github.com/DragoonAethis/itch-dl"
 authors = ["Dragoon Aethis <dragoon@dragonic.eu>"]
 readme = "README.md"
 license = "MIT"
 
@@ -24,16 +24,23 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tqdm = "^4.66.2"
 urllib3 = "^1.26.18"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
-lxml = "^5.1.0"
-pydantic = "^1.10.14"
+lxml = "^5.2.1"
+pydantic = "^1.10.15"
 
 [tool.poetry.scripts]
 itch-dl = "itch_dl.cli:run"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 120
+target-version = "py38"
+
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "B", "C4", "T10", "N", "UP", "S"]
```

### Comparing `itch_dl-0.4.0/PKG-INFO` & `itch_dl-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itch-dl
-Version: 0.4.0
+Version: 0.4.1
 Summary: itch.io bulk game downloader
 Home-page: https://github.com/DragoonAethis/itch-dl
 License: MIT
 Author: Dragoon Aethis
 Author-email: dragoon@dragonic.eu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
-Requires-Dist: pydantic (>=1.10.14,<2.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: pydantic (>=1.10.15,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/DragoonAethis/itch-dl/issues
 Project-URL: Repository, https://github.com/DragoonAethis/itch-dl
 Project-URL: Wiki, https://github.com/DragoonAethis/itch-dl/wiki
 Description-Content-Type: text/markdown
```

