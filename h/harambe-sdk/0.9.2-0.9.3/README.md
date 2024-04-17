# Comparing `tmp/harambe_sdk-0.9.2.tar.gz` & `tmp/harambe_sdk-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harambe_sdk-0.9.2.tar", max compression
+gzip compressed data, was "harambe_sdk-0.9.3.tar", max compression
```

## Comparing `harambe_sdk-0.9.2.tar` & `harambe_sdk-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     5141 2024-04-04 00:50:22.029190 harambe_sdk-0.9.2/README.md
--rw-r--r--   0        0        0      278 2024-03-17 22:34:41.210967 harambe_sdk-0.9.2/harambe/__init__.py
--rw-r--r--   0        0        0    13631 2024-03-29 19:10:57.314846 harambe_sdk-0.9.2/harambe/core.py
--rw-r--r--   0        0        0     2397 2024-03-01 06:20:44.777193 harambe_sdk-0.9.2/harambe/handlers.py
--rw-r--r--   0        0        0     3038 2024-03-01 05:38:05.074579 harambe_sdk-0.9.2/harambe/meta.py
--rw-r--r--   0        0        0     2457 2024-03-17 23:05:42.149184 harambe_sdk-0.9.2/harambe/normalize_url.py
--rw-r--r--   0        0        0     5014 2024-03-28 23:00:00.635703 harambe_sdk-0.9.2/harambe/observer.py
--rw-r--r--   0        0        0     2269 2024-03-29 19:10:57.314547 harambe_sdk-0.9.2/harambe/parser/parser.py
--rw-r--r--   0        0        0        0 2023-11-16 20:05:34.307080 harambe_sdk-0.9.2/harambe/py.typed
--rw-r--r--   0        0        0     3907 2024-03-01 05:38:05.074901 harambe_sdk-0.9.2/harambe/tracker.py
--rw-r--r--   0        0        0      256 2024-03-01 05:38:05.075229 harambe_sdk-0.9.2/harambe/types.py
--rw-r--r--   0        0        0     3049 2024-03-01 05:43:34.226033 harambe_sdk-0.9.2/harambe/utils.py
--rw-r--r--   0        0        0      835 2024-04-04 00:50:34.319790 harambe_sdk-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 harambe_sdk-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     5141 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/README.md
+-rw-r--r--   0        0        0      278 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/__init__.py
+-rw-r--r--   0        0        0    12846 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/core.py
+-rw-r--r--   0        0        0     2397 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/handlers.py
+-rw-r--r--   0        0        0     1747 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/harness.py
+-rw-r--r--   0        0        0     3038 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/meta.py
+-rw-r--r--   0        0        0     2457 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/normalize_url.py
+-rw-r--r--   0        0        0     5014 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/observer.py
+-rw-r--r--   0        0        0     2269 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/py.typed
+-rw-r--r--   0        0        0     3907 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/tracker.py
+-rw-r--r--   0        0        0      256 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/types.py
+-rw-r--r--   0        0        0     3049 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/utils.py
+-rw-r--r--   0        0        0     1189 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 harambe_sdk-0.9.3/PKG-INFO
```

### Comparing `harambe_sdk-0.9.2/README.md` & `harambe_sdk-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/core.py` & `harambe_sdk-0.9.3/harambe/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 import uuid
 from functools import wraps
 from typing import Any, Callable, List, Optional, Protocol, Union, Awaitable
 
 import aiohttp
 from playwright.async_api import (
     Page,
-    async_playwright,
     ElementHandle,
     TimeoutError as PlaywrightTimeoutError,
 )
-from playwright_stealth import stealth_async
 
 from harambe.handlers import (
     ResourceRequestHandler,
     ResourceType,
-    UnnecessaryResourceHandler,
 )
+from harambe.harness import playwright_harness
 from harambe.normalize_url import normalize_url
 from harambe.observer import (
     LocalStorageObserver,
     LoggingObserver,
     OutputObserver,
     DownloadMeta,
     DuplicateHandler,
@@ -230,82 +228,69 @@
             return await asyncio.gather(
                 *[getattr(o, method)(*args, **kwargs) for o in self._observers]
             )
 
     @staticmethod
     async def run(
         scraper: AsyncScraperType,
-        url: Optional[str] = None,
+        url: str,
         context: Optional[Context] = None,
         headless: bool = False,
+        cdp_endpoint: Optional[str] = None,
     ) -> None:
         """
         Convenience method for running a scraper. This will launch a browser and
         invoke the scraper function.
         :param scraper: scraper to run
         :param url: starting url to run the scraper on
         :param context: additional context to pass to the scraper
         :param headless: whether to run the browser headless
+        :param cdp_endpoint: endpoint to connect to the browser (if using a remote browser)
         :return none: everything should be saved to the database or file
         """
         domain = getattr(scraper, "domain", None)
         stage = getattr(scraper, "stage", None)
         observer = getattr(scraper, "observer", None)
+        context = context or {}
 
-        async with async_playwright() as p:
-            browser = await p.chromium.launch(headless=headless)
-            ctx = await browser.new_context(
-                viewport={"width": 1280, "height": 1024},
-                ignore_https_errors=True,
-                user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36"
-                " (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36",
+        async with playwright_harness(
+            headless=headless, cdp_endpoint=cdp_endpoint
+        ) as page:
+            await page.goto(url)
+            await scraper(
+                SDK(
+                    page,
+                    domain=domain,
+                    stage=stage,
+                    observer=observer,
+                    scraper=scraper,
+                    context=context,
+                ),
+                url,
+                context,
             )
-            ctx.set_default_timeout(60000)
-
-            await ctx.route("**/*", UnnecessaryResourceHandler().handle)
-
-            await ctx.tracing.start(screenshots=True, snapshots=True, sources=True)
-            page = await ctx.new_page()
-            await stealth_async(page)
-
-            try:
-                await page.goto(url)
-                await scraper(
-                    SDK(
-                        page,
-                        domain=domain,
-                        stage=stage,
-                        observer=observer,
-                        scraper=scraper,
-                        context=context,
-                    ),
-                    url,
-                    context,
-                )
-            except Exception as e:
-                await ctx.tracing.stop(path="trace.zip")
-                await browser.close()
-                raise e
-            else:
-                await ctx.tracing.stop(path="trace.zip")
-                await browser.close()
 
     async def get_content_type(self, url: str) -> str:
         async with aiohttp.ClientSession() as session:
             async with session.head(normalize_url(url, self.page.url)) as response:
                 return response.headers.get("Content-Type", "")
 
     @staticmethod
-    async def run_from_file(scraper: AsyncScraperType, headless: bool = False) -> None:
+    async def run_from_file(
+        scraper: AsyncScraperType,
+        headless: bool = False,
+        cdp_endpoint: Optional[str] = None,
+    ) -> None:
         """
         Convenience method for running a detail scraper from file. This will load
         the listing data from file and pass it to the scraper.
 
         :param scraper: the scraper to run (function)
         :param headless: whether to run the browser headless
+        :param cdp_endpoint: endpoint to connect to the browser (if using a remote browser)
         :return: None: the scraper should save data to the database or file
         """
         domain = getattr(scraper, "domain", None)
         stage = getattr(scraper, "stage", None)
         observer: Optional[OutputObserver] = getattr(scraper, "observer", None)
 
         if stage != "detail" and stage != "listing":
@@ -319,35 +304,31 @@
         if not file_path.exists():
             raise ValueError(
                 f"Could not find {file_path}."
                 f" No listing data found for this domain. Run the listing scraper first."
             )
 
         listing_data = tracker.load_data(domain, prev)
-        async with async_playwright() as p:
-            browser = await p.chromium.launch(headless=headless)
-            ctx = await browser.new_context()
-            page = await ctx.new_page()
-            await stealth_async(page)
-
+        async with playwright_harness(
+            headless=headless, cdp_endpoint=cdp_endpoint
+        ) as page:
             for listing in listing_data:
+                await page.goto(listing["url"])
                 await scraper(
                     SDK(
                         page,
                         domain=domain,
                         stage=stage,
                         observer=observer,
                         scraper=scraper,
                     ),
                     listing["url"],
                     listing["context"],
                 )
 
-            await browser.close()
-
     @staticmethod
     def scraper(
         domain: str, stage: Stage
     ) -> Callable[[AsyncScraperType], AsyncScraperType]:
         """
         Decorator for scrapers. This will add the domain and stage to the function.
         All scrapers should be decorated with this decorator.
```

### Comparing `harambe_sdk-0.9.2/harambe/handlers.py` & `harambe_sdk-0.9.3/harambe/handlers.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/meta.py` & `harambe_sdk-0.9.3/harambe/meta.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/normalize_url.py` & `harambe_sdk-0.9.3/harambe/normalize_url.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/observer.py` & `harambe_sdk-0.9.3/harambe/observer.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/parser/parser.py` & `harambe_sdk-0.9.3/harambe/parser/parser.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/tracker.py` & `harambe_sdk-0.9.3/harambe/tracker.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/harambe/utils.py` & `harambe_sdk-0.9.3/harambe/utils.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.2/pyproject.toml` & `harambe_sdk-0.9.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harambe-sdk"
-version = "0.9.2"
+version = "0.9.3"
 description = "Data extraction SDK for Playwright 🐒🍌"
 authors = ["awtkns <hello@awtkns.com>"]
 readme = "README.md"
 packages = [
     { include = "harambe", from = "." },
 ]
 
@@ -17,22 +17,38 @@
 beautifulsoup4 = "^4.12.2"
 requests = "^2.31.0"
 playwright-stealth = "^1.0.6" # TODO: self host this package
 aiohttp = "^3.9.3"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.2.1"
+mypy = "^1.9.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.1"
 pytest-mock = "^3.12.0"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 
+[tool.mypy]
+strict = true
+ignore_missing_imports = true
+allow_subclassing_any = true
+allow_untyped_calls = true
+pretty = true
+show_error_codes = true
+implicit_reexport = true
+allow_untyped_decorators = true
+warn_unused_ignores = false
+warn_return_any = false
+namespace_packages = true
+files = "harambe"
+exclude = ["tests", "extractors"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `harambe_sdk-0.9.2/PKG-INFO` & `harambe_sdk-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harambe-sdk
-Version: 0.9.2
+Version: 0.9.3
 Summary: Data extraction SDK for Playwright 🐒🍌
 Author: awtkns
 Author-email: hello@awtkns.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

