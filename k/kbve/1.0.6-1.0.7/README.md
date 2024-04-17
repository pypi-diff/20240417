# Comparing `tmp/kbve-1.0.6.tar.gz` & `tmp/kbve-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbve-1.0.6.tar", max compression
+gzip compressed data, was "kbve-1.0.7.tar", max compression
```

## Comparing `kbve-1.0.6.tar` & `kbve-1.0.7.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0       35 2024-04-11 15:03:42.815267 kbve-1.0.6/README.md
--rw-r--r--   0        0        0      161 2024-04-11 15:03:42.815267 kbve-1.0.6/kbve_atlas/OAI_CONFIG_LIST.json
--rw-r--r--   0        0        0       12 2024-04-11 15:03:42.815267 kbve-1.0.6/kbve_atlas/__init__.py
--rw-r--r--   0        0        0        9 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/__init__.py
--rw-r--r--   0        0        0     4075 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/api_connector.py
--rw-r--r--   0        0        0      161 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/__init__.py
--rw-r--r--   0        0        0     1026 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/coindesk_client.py
--rw-r--r--   0        0        0     1166 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/poetry_db_client.py
--rw-r--r--   0        0        0     2967 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/websocket_echo_client.py
--rw-r--r--   0        0        0      196 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/broadcast_utils.py
--rw-r--r--   0        0        0     1088 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/cors_utils.py
--rw-r--r--   0        0        0      823 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/kr_decorator.py
--rw-r--r--   0        0        0     2974 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/rss_utils.py
--rw-r--r--   0        0        0     1517 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/theme_core.py
--rw-r--r--   0        0        0      940 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/atlas_autogen.py
--rw-r--r--   0        0        0      616 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/bigman.py
--rw-r--r--   0        0        0        0 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/__init__.py
--rw-r--r--   0        0        0     1480 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/doom.py
--rw-r--r--   0        0        0     1167 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/enter_the_matrix.py
--rw-r--r--   0        0        0     4640 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/memetris.py
--rw-r--r--   0        0        0     2012 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/pacman.py
--rw-r--r--   0        0        0     1379 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/snake.py
--rw-r--r--   0        0        0     2215 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/tetris.py
--rw-r--r--   0        0        0      473 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/hello.py
--rw-r--r--   0        0        0       11 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/__init__.py
--rw-r--r--   0        0        0      523 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/coindesk.py
--rw-r--r--   0        0        0      190 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/poem.py
--rw-r--r--   0        0        0      335 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/rss.py
--rw-r--r--   0        0        0    10499 2024-04-11 15:03:43.515257 kbve-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 kbve-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-04-17 13:56:58.189905 kbve-1.0.7/README.md
+-rw-r--r--   0        0        0      161 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/OAI_CONFIG_LIST.json
+-rw-r--r--   0        0        0       12 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/__init__.py
+-rw-r--r--   0        0        0        9 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/__init__.py
+-rw-r--r--   0        0        0     4075 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/api_connector.py
+-rw-r--r--   0        0        0      240 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/__init__.py
+-rw-r--r--   0        0        0     1998 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/coindesk_client.py
+-rw-r--r--   0        0        0     1985 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/novnc_client.py
+-rw-r--r--   0        0        0     1166 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/poetry_db_client.py
+-rw-r--r--   0        0        0     1336 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/screen_client.py
+-rw-r--r--   0        0        0     2967 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/clients/websocket_echo_client.py
+-rw-r--r--   0        0        0      234 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/broadcast_utils.py
+-rw-r--r--   0        0        0     1088 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/cors_utils.py
+-rw-r--r--   0        0        0     2350 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/image_utils.py
+-rw-r--r--   0        0        0      823 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/kr_decorator.py
+-rw-r--r--   0        0        0     3048 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/rss_utils.py
+-rw-r--r--   0        0        0     1517 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/theme_core.py
+-rw-r--r--   0        0        0      940 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/atlas_autogen.py
+-rw-r--r--   0        0        0      616 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/bigman.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/__init__.py
+-rw-r--r--   0        0        0     1480 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/doom.py
+-rw-r--r--   0        0        0     1167 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/enter_the_matrix.py
+-rw-r--r--   0        0        0     4640 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/memetris.py
+-rw-r--r--   0        0        0     2012 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/pacman.py
+-rw-r--r--   0        0        0     1379 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/snake.py
+-rw-r--r--   0        0        0     2215 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/tetris.py
+-rw-r--r--   0        0        0      473 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/hello.py
+-rw-r--r--   0        0        0       11 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/coindesk.py
+-rw-r--r--   0        0        0      190 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/poem.py
+-rw-r--r--   0        0        0     1434 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/rsps.py
+-rw-r--r--   0        0        0      335 2024-04-17 13:56:58.197904 kbve-1.0.7/kbve_atlas/models/rss.py
+-rw-r--r--   0        0        0    15477 2024-04-17 13:56:58.929907 kbve-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 kbve-1.0.7/PKG-INFO
```

### Comparing `kbve-1.0.6/kbve_atlas/api/api_connector.py` & `kbve-1.0.7/kbve_atlas/api/api_connector.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/clients/poetry_db_client.py` & `kbve-1.0.7/kbve_atlas/api/clients/poetry_db_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/clients/websocket_echo_client.py` & `kbve-1.0.7/kbve_atlas/api/clients/websocket_echo_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/utils/broadcast_utils.py` & `kbve-1.0.7/kbve_atlas/api/utils/broadcast_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/utils/cors_utils.py` & `kbve-1.0.7/kbve_atlas/api/utils/cors_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/utils/kr_decorator.py` & `kbve-1.0.7/kbve_atlas/api/utils/kr_decorator.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/api/utils/rss_utils.py` & `kbve-1.0.7/kbve_atlas/api/utils/rss_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,11 +72,15 @@
     @staticmethod
     def format_rss_feed(rss_feed: RssFeed) -> str:
         """
         Formats the RSS feed for display.
         """
         formatted_feed = f"RSS Feed: {rss_feed.title}\n"
         for item in rss_feed.items:
-            formatted_feed += f"\nTitle: {item.title}\nLink: {
-                item.link}\nDescription: {item.description}\nPubDate: {item.pubDate}\n"
+            formatted_feed += (
+                f"\nTitle: {item.title}\n"
+                f"Link: {item.link}\n"
+                f"Description: {item.description}\n"
+                f"PubDate: {item.pubDate}\n"
+            )
             formatted_feed += "-" * 50 + "\n"  # Separator between items
-        return formatted_feed
+        return formatted_feed
```

### Comparing `kbve-1.0.6/kbve_atlas/api/utils/theme_core.py` & `kbve-1.0.7/kbve_atlas/api/utils/theme_core.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/atlas_autogen.py` & `kbve-1.0.7/kbve_atlas/atlas_autogen.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/bigman.py` & `kbve-1.0.7/kbve_atlas/bigman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/doom.py` & `kbve-1.0.7/kbve_atlas/games/doom.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/enter_the_matrix.py` & `kbve-1.0.7/kbve_atlas/games/enter_the_matrix.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/memetris.py` & `kbve-1.0.7/kbve_atlas/games/memetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/pacman.py` & `kbve-1.0.7/kbve_atlas/games/pacman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/snake.py` & `kbve-1.0.7/kbve_atlas/games/snake.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/games/tetris.py` & `kbve-1.0.7/kbve_atlas/games/tetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/kbve_atlas/models/coindesk.py` & `kbve-1.0.7/kbve_atlas/models/coindesk.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.6/pyproject.toml` & `kbve-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,334 +5,489 @@
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html:'../../coverage/apps/atlas/html' --cov-report xml:'../../coverage/apps/atlas/coverage.xml' --html='../../reports/apps/atlas/unittests/html/index.html' --junitxml='../../reports/apps/atlas/unittests/junit.xml'"
 
+[tool.pyright]
+include = [ "kbve_atlas" ]
+exclude = [ "**/tests", "**/__pycache__", "**/*.venv" ]
+
+  [tool.pyright.behavior]
+  reportMissingImports = true
+  reportMissingTypeStubs = true
+  reportOptionalSubscript = true
+  reportOptionalMemberAccess = true
+  reportGeneralTypeIssues = true
+  reportFunctionMemberAccess = true
+  reportUnusedVariable = true
+  strict = true
+  typeCheckingMode = "strict"
+
+  [tool.pyright.environment]
+  pythonVersion = "3.12"
+  venvPath = ".venv"
+  venv = "myenv"
+  stubPath = "typings"
+  typingsPath = "typings"
+  analyzeTypeshed = false
+  autoSearchPaths = true
+
 [tool.poetry]
 name = "kbve"
-version = "1.0.6"
+version = "1.0.7"
 description = "ATLAS"
 authors = [ ]
 license = "Proprietary"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "kbve_atlas"
 
   [tool.poetry.dependencies]
-  python = ">=3.12,<3.13"
+  python = ">=3.10,<3.13"
 
     [tool.poetry.dependencies.aiohttp]
-    version = "3.9.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    version = "3.9.4 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.aiosignal]
     version = "1.3.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.annotated-types]
     version = "0.6.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.anyio]
     version = "4.3.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.async-timeout]
+    version = "4.0.3 "
+    markers = 'python_version >= "3.10" and python_full_version < "3.11.3"'
     optional = false
 
     [tool.poetry.dependencies.asyncio-redis]
     version = "0.16.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.attrs]
     version = "23.2.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.beautifulsoup4]
     version = "4.12.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.broadcaster]
     version = "0.2.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
     extras = [ "redis" ]
 
     [tool.poetry.dependencies.certifi]
     version = "2024.2.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.cffi]
+    version = "1.16.0 "
+    markers = 'os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.charset-normalizer]
     version = "3.3.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.click]
     version = "8.1.7 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.colorama]
     version = "0.4.6 "
-    markers = 'python_version >= "3.12" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")'
+    markers = 'python_version >= "3.10" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")'
     optional = false
 
     [tool.poetry.dependencies.diskcache]
     version = "5.6.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.distro]
     version = "1.9.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.docker]
     version = "7.0.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.exceptiongroup]
+    version = "1.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.fastapi]
     version = "0.110.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.filelock]
     version = "3.13.4 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.flaml]
     version = "2.1.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.frozenlist]
     version = "1.4.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.fsspec]
     version = "2024.3.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.h11]
     version = "0.14.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.httpcore]
     version = "1.0.5 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.httptools]
     version = "0.6.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.httpx]
     version = "0.27.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.huggingface-hub]
     version = "0.22.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.humancursor]
+    version = "1.1.5 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.idna]
     version = "3.7 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.importlib-metadata]
     version = "7.1.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.jinja2]
     version = "3.1.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.litellm]
-    version = "1.35.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    version = "1.35.4 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.lxml]
     version = "5.2.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.markupsafe]
     version = "2.1.5 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.mouseinfo]
+    version = "0.1.3 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.multidict]
     version = "6.0.5 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.numpy]
     version = "1.26.4 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.openai]
-    version = "1.17.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    version = "1.17.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.opencv-python]
+    version = "4.9.0.80 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.outcome]
+    version = "1.3.0.post0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.packaging]
     version = "24.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pillow]
     version = "10.3.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pyautogen]
     version = "0.2.23 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
     extras = [ "lmm", "redis" ]
 
+    [tool.poetry.dependencies.pyautogui]
+    version = "0.9.54 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pycparser]
+    version = "2.22 "
+    markers = 'os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pydantic-core]
-    version = "2.16.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    version = "2.18.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pydantic]
-    version = "2.6.4 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    version = "2.7.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pygetwindow]
+    version = "0.0.9 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pymsgbox]
+    version = "1.0.9 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pyobjc-core]
+    version = "10.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
+    optional = false
+
+    [tool.poetry.dependencies.pyobjc-framework-cocoa]
+    version = "10.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
+    optional = false
+
+    [tool.poetry.dependencies.pyobjc-framework-quartz]
+    version = "10.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
+    optional = false
+
+    [tool.poetry.dependencies.pyperclip]
+    version = "1.8.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pyrect]
+    version = "0.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pyscreeze]
+    version = "0.1.30 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pysocks]
+    version = "1.7.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.python-dotenv]
     version = "1.0.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.python3-xlib]
+    version = "0.15 "
+    markers = 'platform_system == "Linux" and python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytweening]
+    version = "1.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pywin32]
     version = "306 "
-    markers = 'python_version >= "3.12" and python_version < "3.13" and sys_platform == "win32"'
+    markers = 'python_version >= "3.10" and python_version < "3.13" and sys_platform == "win32"'
     optional = false
 
     [tool.poetry.dependencies.pyyaml]
     version = "6.0.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.redis]
     version = "5.0.3 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.regex]
     version = "2023.12.25 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.replicate]
     version = "0.25.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.requests]
     version = "2.31.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.rubicon-objc]
+    version = "0.4.8 "
+    markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
+    optional = false
+
+    [tool.poetry.dependencies.selenium]
+    version = "4.19.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.sniffio]
     version = "1.3.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.sortedcontainers]
+    version = "2.4.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.soupsieve]
     version = "2.5 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.starlette]
     version = "0.37.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.termcolor]
     version = "2.4.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tiktoken]
     version = "0.6.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tokenizers]
     version = "0.15.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tqdm]
     version = "4.66.2 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.trio-websocket]
+    version = "0.11.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.trio]
+    version = "0.25.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.typing-extensions]
     version = "4.11.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.urllib3]
     version = "2.2.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
+    extras = [ "socks" ]
 
     [tool.poetry.dependencies.uvicorn]
     version = "0.29.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
     extras = [ "standard" ]
 
     [tool.poetry.dependencies.uvloop]
     version = "0.19.0 "
-    markers = '(sys_platform != "win32" and sys_platform != "cygwin") and platform_python_implementation != "PyPy" and python_version >= "3.12" and python_version < "3.13"'
+    markers = '(sys_platform != "win32" and sys_platform != "cygwin") and platform_python_implementation != "PyPy" and python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.watchfiles]
     version = "0.21.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.websockets]
     version = "12.0 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.wsproto]
+    version = "1.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.yarl]
     version = "1.9.4 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.zipp]
     version = "3.18.1 "
-    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
 [tool.poetry.group.dev]
 dependencies = { }
 
 [build-system]
 requires = [ "poetry-core" ]
```

