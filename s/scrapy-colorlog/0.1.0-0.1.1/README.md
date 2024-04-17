# Comparing `tmp/scrapy_colorlog-0.1.0.tar.gz` & `tmp/scrapy_colorlog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_colorlog-0.1.0.tar", last modified: Thu Jan  4 18:24:27 2024, max compression
+gzip compressed data, was "scrapy_colorlog-0.1.1.tar", last modified: Wed Apr 17 19:16:24 2024, max compression
```

## Comparing `scrapy_colorlog-0.1.0.tar` & `scrapy_colorlog-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2236 2024-01-04 17:16:24.832677 scrapy_colorlog-0.1.0/README.md
--rw-r--r--   0        0        0      672 2024-01-04 18:24:27.111369 scrapy_colorlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       50 2024-01-04 10:31:26.508682 scrapy_colorlog-0.1.0/src/scrapy_colorlog/__init__.py
--rw-r--r--   0        0        0     1217 2024-01-04 09:43:05.633532 scrapy_colorlog-0.1.0/src/scrapy_colorlog/formatter.py
--rw-r--r--   0        0        0        0 2023-12-27 20:58:27.105093 scrapy_colorlog-0.1.0/src/scrapy_colorlog/py.typed
--rw-r--r--   0        0        0     1129 2024-01-04 08:48:28.551128 scrapy_colorlog-0.1.0/src/scrapy_colorlog/utils.py
--rw-r--r--   0        0        0        0 2023-12-28 14:55:09.656607 scrapy_colorlog-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 scrapy_colorlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2246 2024-01-04 18:30:49.557741 scrapy_colorlog-0.1.1/README.md
+-rw-r--r--   0        0        0      855 2024-04-17 19:16:24.353882 scrapy_colorlog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-01-04 10:31:26.508682 scrapy_colorlog-0.1.1/src/scrapy_colorlog/__init__.py
+-rw-r--r--   0        0        0     1268 2024-01-04 22:22:57.386958 scrapy_colorlog-0.1.1/src/scrapy_colorlog/formatter.py
+-rw-r--r--   0        0        0        0 2023-12-27 20:58:27.105093 scrapy_colorlog-0.1.1/src/scrapy_colorlog/py.typed
+-rw-r--r--   0        0        0     1296 2024-01-04 22:13:30.495435 scrapy_colorlog-0.1.1/src/scrapy_colorlog/utils.py
+-rw-r--r--   0        0        0        0 2023-12-28 14:55:09.656607 scrapy_colorlog-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-17 17:50:52.267737 scrapy_colorlog-0.1.1/tests/test_all.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 scrapy_colorlog-0.1.1/PKG-INFO
```

### Comparing `scrapy_colorlog-0.1.0/README.md` & `scrapy_colorlog-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 [COLORLOG_FORMAT](#colorlog_format).
 
 See also:
 [LOG_DATEFORMAT](https://docs.scrapy.org/en/latest/topics/settings.html#log-dateformat).
 
 ### COLORLOG_COLORS
 
+Default:
+
 ```python
 {
     "DEBUG": "blue",
     "INFO": "cyan",
     "WARNING": "yellow",
     "ERROR": "red",
     "CRITICAL": "purple",
```

### Comparing `scrapy_colorlog-0.1.0/pyproject.toml` & `scrapy_colorlog-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "scrapy-colorlog"
-version = "0.1.0"
+version = "0.1.1"
 description = "Color log output support for Scrapy"
 authors = [
     { name = "divtiply" },
 ]
 dependencies = [
     "scrapy>=1.0.0",
     "colorlog>=6.6.0",
+    "typing-extensions>=4.0.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Framework :: Scrapy",
     "Programming Language :: Python :: 3",
     "Typing :: Typed",
@@ -28,8 +29,15 @@
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
-package-type = "library"
+distribution = true
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "$version"
+version_scheme = "pep440"
+version_provider = "pep621"
+major_version_zero = true
```

### Comparing `scrapy_colorlog-0.1.0/src/scrapy_colorlog/formatter.py` & `scrapy_colorlog-0.1.1/src/scrapy_colorlog/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import colorlog
 from scrapy.crawler import Crawler
 from scrapy.settings import Settings
+from typing_extensions import Self
 
 DEFAULT_FORMAT = (
     "%(light_black)s%(asctime)s%(reset)s "
     "%(light_black)s[%(name)s]%(reset)s "
     "%(log_color)s%(levelname)s%(reset)s%(light_black)s:%(reset)s "
     "%(message)s"
 )
@@ -18,19 +19,19 @@
     "ERROR": "red",
     "CRITICAL": "purple",
 }
 
 
 class ColoredFormatter(colorlog.ColoredFormatter):
     @classmethod
-    def from_crawler(cls, crawler: Crawler):
+    def from_crawler(cls, crawler: Crawler) -> Self:
         return cls.from_settings(crawler.settings)
 
     @classmethod
-    def from_settings(cls, settings: Settings):
+    def from_settings(cls, settings: Settings) -> Self:
         return cls(
             fmt=settings.get("COLORLOG_FORMAT", DEFAULT_FORMAT),
             datefmt=settings.get("COLORLOG_DATEFORMAT", DEFAULT_DATEFORMAT),
             log_colors=settings.getdict("COLORLOG_COLORS", DEFAULT_COLORS),
             secondary_log_colors=settings.getdict("COLORLOG_SECONDARY_COLORS"),
             reset=settings.getbool("COLORLOG_RESET", True),
             no_color=settings.getbool("COLORLOG_NO_COLOR", False),
```

### Comparing `scrapy_colorlog-0.1.0/src/scrapy_colorlog/utils.py` & `scrapy_colorlog-0.1.1/src/scrapy_colorlog/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from __future__ import annotations
+
 import logging
 
+import scrapy.utils.log
 from scrapy.settings import Settings
 from scrapy.utils.log import get_scrapy_root_handler
 
 from .formatter import ColoredFormatter
 
 
+def install() -> None:
+    from scrapy import crawler
+
+    crawler.configure_logging = configure_logging
+    crawler.install_scrapy_root_handler = install_scrapy_root_handler
+
+
+def configure_logging(
+    settings: Settings | dict | None = None, install_root_handler: bool = True
+) -> None:
+    if isinstance(settings, dict) or settings is None:
+        settings = Settings(settings)
+    scrapy.utils.log.configure_logging(settings, install_root_handler)
+    replace_scrapy_root_handler_formatter(settings)
+
+
+def install_scrapy_root_handler(settings: Settings) -> None:
+    scrapy.utils.log.install_scrapy_root_handler(settings)
+    replace_scrapy_root_handler_formatter(settings)
+
+
 def replace_scrapy_root_handler_formatter(settings: Settings) -> None:
     handler = get_scrapy_root_handler()
     if (
         handler
         and isinstance(handler, logging.StreamHandler)
         and not isinstance(handler.formatter, ColoredFormatter)
     ):
         formatter = ColoredFormatter.from_settings(settings)
         formatter.stream = handler.stream
         handler.setFormatter(formatter)
-
-
-def install() -> None:
-    from scrapy import crawler
-    from scrapy.utils import log
-
-    def configure_logging(settings: Settings, install_root_handler: bool = True):
-        log.configure_logging(settings, install_root_handler)
-        replace_scrapy_root_handler_formatter(settings)
-
-    def install_scrapy_root_handler(settings: Settings):
-        log.install_scrapy_root_handler(settings)
-        replace_scrapy_root_handler_formatter(settings)
-
-    crawler.configure_logging = configure_logging
-    crawler.install_scrapy_root_handler = install_scrapy_root_handler
```

### Comparing `scrapy_colorlog-0.1.0/PKG-INFO` & `scrapy_colorlog-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapy-colorlog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Color log output support for Scrapy
 Author: divtiply
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Scrapy
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/divtiply/scrapy-colorlog
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Requires-Dist: scrapy>=1.0.0
 Requires-Dist: colorlog>=6.6.0
+Requires-Dist: typing-extensions>=4.0.0
 Description-Content-Type: text/markdown
 
 # scrapy-colorlog
 
 Color log output support for [Scrapy][1].
 
 ## Installation
@@ -64,14 +65,16 @@
 [COLORLOG_FORMAT](#colorlog_format).
 
 See also:
 [LOG_DATEFORMAT](https://docs.scrapy.org/en/latest/topics/settings.html#log-dateformat).
 
 ### COLORLOG_COLORS
 
+Default:
+
 ```python
 {
     "DEBUG": "blue",
     "INFO": "cyan",
     "WARNING": "yellow",
     "ERROR": "red",
     "CRITICAL": "purple",
```

