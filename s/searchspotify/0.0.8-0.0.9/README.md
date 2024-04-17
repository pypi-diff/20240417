# Comparing `tmp/searchspotify-0.0.8.tar.gz` & `tmp/searchspotify-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchspotify-0.0.8.tar", last modified: Sat Apr 13 01:28:25 2024, max compression
+gzip compressed data, was "searchspotify-0.0.9.tar", last modified: Wed Apr 17 02:47:08 2024, max compression
```

## Comparing `searchspotify-0.0.8.tar` & `searchspotify-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.071377 searchspotify-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-13 01:28:19.000000 searchspotify-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-13 01:28:25.071377 searchspotify-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-13 01:28:19.000000 searchspotify-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 01:28:19.000000 searchspotify-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-13 01:28:25.071377 searchspotify-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.067377 searchspotify-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.067377 searchspotify-0.0.8/src/searchspotify/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/urlbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.071377 searchspotify-0.0.8/src/searchspotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:08.212403 searchspotify-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-17 02:47:04.000000 searchspotify-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-17 02:47:08.212403 searchspotify-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-17 02:47:04.000000 searchspotify-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 02:47:04.000000 searchspotify-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 02:47:08.212403 searchspotify-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:08.208403 searchspotify-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:08.212403 searchspotify-0.0.9/src/searchspotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-17 02:47:04.000000 searchspotify-0.0.9/src/searchspotify/urlbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:08.212403 searchspotify-0.0.9/src/searchspotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-17 02:47:08.000000 searchspotify-0.0.9/src/searchspotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 02:47:08.000000 searchspotify-0.0.9/src/searchspotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:47:08.000000 searchspotify-0.0.9/src/searchspotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 02:47:08.000000 searchspotify-0.0.9/src/searchspotify.egg-info/top_level.txt
```

### Comparing `searchspotify-0.0.8/LICENSE` & `searchspotify-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/PKG-INFO` & `searchspotify-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchspotify
-Version: 0.0.8
+Version: 0.0.9
 Summary: A complete wrapper for the Search API provided by Spotify written in Python.
 Home-page: https://github.com/ufoptg/SearchSpotify
 Author: True Saiyan
 Project-URL: Bug Tracker, https://github.com/ufoptg/SearchSpotify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: searchspotify Version: 0.0.8 Summary: A complete
+Metadata-Version: 2.1 Name: searchspotify Version: 0.0.9 Summary: A complete
 wrapper for the Search API provided by Spotify written in Python. Home-page:
 https://github.com/ufoptg/SearchSpotify Author: True Saiyan Project-URL: Bug
 Tracker, https://github.com/ufoptg/SearchSpotify/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Spotify Search
 _[_L_I_C_E_N_S_E_]_[_P_I_P_]
```

### Comparing `searchspotify-0.0.8/README.md` & `searchspotify-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/setup.cfg` & `searchspotify-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = searchspotify
-version = 0.0.8
+version = 0.0.9
 author = True Saiyan
 description = A complete wrapper for the Search API provided by Spotify written in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ufoptg/SearchSpotify
 project_urls = 
 	Bug Tracker = https://github.com/ufoptg/SearchSpotify/issues
```

### Comparing `searchspotify-0.0.8/src/searchspotify/__init__.py` & `searchspotify-0.0.9/src/searchspotify/__init__.py`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/src/searchspotify/calls.py` & `searchspotify-0.0.9/src/searchspotify/calls.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,8 +44,26 @@
 
     :param access_token: Access token for authentication.
     :param args: Tuple of arguments for the search endpoint.
     :return: Response object containing the search results.
     """
     endpoint = urlbuilder.search_endpoint(*args)
     headers = {"Authorization": f"Bearer {acess_token}"}
-    return get(url=endpoint, headers=headers)
+    return get(url=endpoint, headers=headers)
+
+
+def call_track_preview(track_id, access_token):
+    """
+    Calls Spotify API to retrieve the preview URL for a given track.
+
+    :param track_id: Spotify track ID.
+    :param access_token: Access token for authentication.
+    :return: Preview URL if available, None otherwise.
+    """
+    endpoint = f"https://api.spotify.com/v1/tracks/{track_id}"
+    headers = {"Authorization": f"Bearer {access_token}"}
+    response = get(url=endpoint, headers=headers)
+    if response.status_code == 200:
+        track_data = response.json()
+        if "preview_url" in track_data:
+            return track_data["preview_url"]
+    return None
```

### Comparing `searchspotify-0.0.8/src/searchspotify/classes.py` & `searchspotify-0.0.9/src/searchspotify/classes.py`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/src/searchspotify/client.py` & `searchspotify-0.0.9/src/searchspotify/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,7 +138,21 @@
                         title = title_parts[0].strip()
                 if title and "| Spotify" in title:
                     title = title.split("| Spotify")[0].strip()
                 return title
         except Exception as e:
             print(f"Error extracting title: {e}")
         return None
+
+    def get_track_preview(self, track_link: str) -> str:
+        """
+        Retrieves the preview link for a given track.
+
+        :param track_link: Link to the track.
+        :return: Preview link if available, empty string otherwise.
+        """
+        if "spotify.com/track/" in track_link:
+            track_id = track_link.split("/")[-1]
+            access_token = self.auth.get_acess_token()
+            preview_url = calls.call_track_preview(track_id, access_token)
+            return preview_url if preview_url else ""
+        return ""
```

### Comparing `searchspotify-0.0.8/src/searchspotify/constructor.py` & `searchspotify-0.0.9/src/searchspotify/constructor.py`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/src/searchspotify/urlbuilder.py` & `searchspotify-0.0.9/src/searchspotify/urlbuilder.py`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.8/src/searchspotify.egg-info/PKG-INFO` & `searchspotify-0.0.9/src/searchspotify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchspotify
-Version: 0.0.8
+Version: 0.0.9
 Summary: A complete wrapper for the Search API provided by Spotify written in Python.
 Home-page: https://github.com/ufoptg/SearchSpotify
 Author: True Saiyan
 Project-URL: Bug Tracker, https://github.com/ufoptg/SearchSpotify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: searchspotify Version: 0.0.8 Summary: A complete
+Metadata-Version: 2.1 Name: searchspotify Version: 0.0.9 Summary: A complete
 wrapper for the Search API provided by Spotify written in Python. Home-page:
 https://github.com/ufoptg/SearchSpotify Author: True Saiyan Project-URL: Bug
 Tracker, https://github.com/ufoptg/SearchSpotify/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Spotify Search
 _[_L_I_C_E_N_S_E_]_[_P_I_P_]
```

