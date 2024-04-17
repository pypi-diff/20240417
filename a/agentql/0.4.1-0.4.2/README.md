# Comparing `tmp/agentql-0.4.1.tar.gz` & `tmp/agentql-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.4.1.tar", max compression
+gzip compressed data, was "agentql-0.4.2.tar", max compression
```

## Comparing `agentql-0.4.1.tar` & `agentql-0.4.2.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1066 2024-04-05 17:21:47.290799 agentql-0.4.1/LICENSE
--rw-r--r--   0        0        0      111 2024-04-05 17:21:47.290799 agentql-0.4.1/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-04-05 17:21:47.378800 agentql-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/__init__.py
--rw-r--r--   0        0        0       78 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_api_constants.py
--rw-r--r--   0        0        0     4741 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_errors.py
--rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     5986 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/character_utils.py
--rw-r--r--   0        0        0     4997 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/node.py
--rw-r--r--   0        0        0     4686 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/source.py
--rw-r--r--   0        0        0     1602 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/token.py
--rw-r--r--   0        0        0      213 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/token_kind.py
--rw-r--r--   0        0        0      535 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_typing.py
--rw-r--r--   0        0        0      204 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_utils.py
--rw-r--r--   0        0        0      363 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     2574 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_api.py
--rw-r--r--   0        0        0     1605 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_popup.py
--rw-r--r--   0        0        0     5460 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_response_proxy.py
--rw-r--r--   0        0        0    10787 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_session.py
--rw-r--r--   0        0        0     5331 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_web_driver.py
--rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/__init__.py
--rw-r--r--   0        0        0      168 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/__init__.py
--rw-r--r--   0        0        0      193 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_driver_constants.py
--rw-r--r--   0        0        0      290 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_driver_settings.py
--rw-r--r--   0        0        0     1980 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_html_constants.py
--rw-r--r--   0        0        0     3813 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_network_monitor.py
--rw-r--r--   0        0        0    26759 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_async.py
--rw-r--r--   0        0        0    26608 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_sync.py
--rw-r--r--   0        0        0      363 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_api.py
--rw-r--r--   0        0        0     1525 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_popup.py
--rw-r--r--   0        0        0     4917 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_response_proxy.py
--rw-r--r--   0        0        0    10540 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_session.py
--rw-r--r--   0        0        0     4770 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_web_driver.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 20:21:24.344649 agentql-0.4.2/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-17 20:21:24.344649 agentql-0.4.2/PACKAGE_README.md
+-rw-r--r--   0        0        0      771 2024-04-17 20:21:24.432649 agentql-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     4741 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     5986 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      145 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     4997 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     2431 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     4686 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      213 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      535 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0      377 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     2893 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     1840 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     5979 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0    11329 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     5601 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-17 20:21:24.432649 agentql-0.4.2/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      280 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     3813 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    27588 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    27290 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1525 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     5291 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0    11068 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     5017 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      291 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/trail_logger/__init__.py
+-rw-r--r--   0        0        0     5151 2024-04-17 20:21:24.436649 agentql-0.4.2/src/agentql/trail_logger/trail_logger.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.2/PKG-INFO
```

### Comparing `agentql-0.4.1/LICENSE` & `agentql-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/pyproject.toml` & `agentql-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.4.1"
+version = "0.4.2"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.4.1/src/agentql/__init__.py` & `agentql-0.4.2/src/agentql/__init__.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_errors.py` & `agentql-0.4.2/src/agentql/_core/_errors.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_js_snippets/generate_accessibility_tree.js` & `agentql-0.4.2/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_js_snippets/set_iframe_path.js` & `agentql-0.4.2/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/character_utils.py` & `agentql-0.4.2/src/agentql/_core/_syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/lexer.py` & `agentql-0.4.2/src/agentql/_core/_syntax/lexer.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/node.py` & `agentql-0.4.2/src/agentql/_core/_syntax/node.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/parser.py` & `agentql-0.4.2/src/agentql/_core/_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/source.py` & `agentql-0.4.2/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_syntax/token.py` & `agentql-0.4.2/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/_core/_typing.py` & `agentql-0.4.2/src/agentql/_core/_typing.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/async_api/_api.py` & `agentql-0.4.2/src/agentql/async_api/_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import logging
 from typing import Any
 
 from playwright.async_api import Locator, Page
 
+from agentql import trail_logger
 from agentql.ext.playwright import PlaywrightWebDriverAsync as PlaywrightWebDriver
 
 from ._session import Session
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
@@ -20,39 +21,44 @@
 
 
 async def start_async_session(
     url: str = "",
     *,
     web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightDriverTypeStub(),
     user_auth_session: Any = None,
+    enable_history_log: bool = False,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
     """Start a new asynchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
     web_driver (webDriver) (optional): Web driver is responsible for interacting with the browser and page. Defaults to Playwright web driver, which is built on top of the [Playwright framework](https://playwright.dev/python/).
     user_auth_session (dict) (optional): The user authentication session that contains previous login session. Users could retrieve authentication session by starting a session, logging into desired website, and calling `session.get_user_auth_session()`, which will return a `auth_session` object defined in web driver.
+    enable_history_log (bool) (optional): Enable history log to record all the events during the session, retrieved via `session.get_last_trail()`.
 
     Returns:
     -------
     Session: An instance of AgentQL Session class for asynchronous environment.
     """
+    if enable_history_log:
+        trail_logger.init()
     log.debug(f"Starting asynchronous session with {url}")
 
     # this is a dirty hack to avoid instantiating PlaywrightWebDriver as a default value
     # which will be cached and reused across all sessions. This may cause problems when
     # start_session is called multiple times with default params. In this case driver will
     # be reused which is a problem since its stateful.
     if isinstance(web_driver, PlaywrightDriverTypeStub):
         web_driver = PlaywrightWebDriver()  # type: ignore
 
     try:
-        await web_driver.start_browser(user_auth_session=user_auth_session)
+        # pylint: disable=protected-access
+        await web_driver._start_browser(user_auth_session=user_auth_session)
         if url:
             await web_driver.open_url(url)
         session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
     except Exception as e:
         log.error(f"Failed to start session: {e}")
-        await web_driver.stop_browser()
+        await web_driver._stop_browser()
         raise e
     return session
```

### Comparing `agentql-0.4.1/src/agentql/async_api/_popup.py` & `agentql-0.4.2/src/agentql/sync_api/_popup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import Callable
 
 
 class Popup:
     """Popup objects are dispatched by session via session.on("popup") event. For each popup window detected on the page, there will be corresponding event and popup objects emitted."""
 
     def __init__(self, popup_tree: dict, popup_name: str, on_popup_close: Callable[[dict], None]):
@@ -31,21 +30,21 @@
 
         Returns:
         --------
         str: The name of the popup.
         """
         return self._name
 
-    async def close(self):
+    def close(self):
         """Close the popup by invoking the callback function passed into the Popup object when it is initialized."""
-        await self._close_popup_callback(self._tree)
+        self._close_popup_callback(self._tree)
 
 
-async def close_all_popups_handler(popups: list):
-    """This is a asynchronous handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
+def close_all_popups_handler(popups: list):
+    """This is a handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
 
     Parameters:
     ----------
     popups(list): The list containing popup objects.
     """
-    tasks = [popup.close() for popup in popups]
-    await asyncio.gather(*tasks)
+    for popup in popups:
+        popup.close()
```

### Comparing `agentql-0.4.1/src/agentql/async_api/_response_proxy.py` & `agentql-0.4.2/src/agentql/async_api/_response_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,76 @@
+# pylint: disable=protected-access
+
 import asyncio
 import json
 import logging
 from typing import Generic, Union
 
-from agentql import AttributeNotFoundError, ContainerListNode, ContainerNode, IdListNode, IdNode
+from agentql import (
+    AttributeNotFoundError,
+    ContainerListNode,
+    ContainerNode,
+    IdListNode,
+    IdNode,
+    trail_logger,
+)
 
-from ._web_driver import InteractiveItemTypeT, WebDriver
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 
 class AQLResponseProxy(Generic[InteractiveItemTypeT]):
     """
     AQLResponseProxy class acts as a dynamic proxy to the response received from AgentQL server. It allows users to interact with resulting web elements and to retrieve their text contents. This class is designed to work with the web driver to fetch and process query results.
     """
 
     def __init__(
         self,
-        data: dict,
-        web_driver: "WebDriver[InteractiveItemTypeT]",
+        data: Union[dict, list],
+        web_driver: "WebDriver[InteractiveItemTypeT, PageTypeT]",
         query_tree: ContainerNode,
     ):
         self._response_data = data
         self._web_driver = web_driver
         self._query_tree_node = query_tree
 
     def __getattr__(
         self, name
-    ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT]:
+    ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT, None]:
         if self._response_data is None:
             raise AttributeError("Response data is None")
         if name not in self._response_data:
             raise AttributeNotFoundError(name, self._response_data)
+        trail_logger.add_event(f"Resolving element {name} on {self._web_driver.current_url}")
         return self._resolve_item(
             self._response_data[name], self._query_tree_node.get_child_by_name(name)
         )
 
     def __getitem__(
         self, index: int
-    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]"]:
+    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if not isinstance(self._response_data, list):
             raise ValueError("This node is not a list")
         return self._resolve_item(self._response_data[index], self._query_tree_node)
 
     def _resolve_item(
         self, item, query_tree_node
-    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]"]:
+    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if item is None:
             return None
 
         if isinstance(item, list):
             return AQLResponseProxy[InteractiveItemTypeT](item, self._web_driver, query_tree_node)
 
         if isinstance(query_tree_node, IdNode) or isinstance(query_tree_node, IdListNode):
-            return self._web_driver.locate_interactive_element(item)
+            interactive_element = self._web_driver._locate_interactive_element(item)
+            trail_logger.add_event(f"Resolved to {interactive_element}")
+
+            return interactive_element
 
         return AQLResponseProxy[InteractiveItemTypeT](item, self._web_driver, query_tree_node)
 
     def __len__(self):
         if self._response_data is None:
             return 0
         return len(self._response_data)
@@ -113,24 +126,27 @@
     async def _to_data_container_list_node(
         self, response_data: dict, query_tree_node: ContainerListNode
     ) -> list:
         tasks = [self._to_data_container_node(item, query_tree_node) for item in response_data]
         result_list = await asyncio.gather(*tasks)
         return result_list
 
-    async def _to_data_id_node(self, response_data: dict) -> dict:
+    async def _to_data_id_node(self, response_data: dict) -> Union[dict, str, None]:
         if response_data is None:
             return None
         name = response_data.get("name")
         if not name or not name.strip():
-            web_element = self._web_driver.locate_interactive_element(response_data)
+            web_element = self._web_driver._locate_interactive_element(response_data)
             if not web_element:
                 log.warning(f"Could not locate web element for item {response_data}")
                 return None
             element_text = await self._web_driver.get_text_content(web_element)
+            if not element_text:
+                log.warning(f"Could not get text content for item {response_data}")
+                return None
             name = element_text.strip()
         return name
 
     async def _to_data_id_list_node(self, response_data: list) -> list:
         tasks = [self._to_data_id_node(item) for item in response_data]
         res = await asyncio.gather(*tasks)
         return [node for node in res if node is not None]
```

### Comparing `agentql-0.4.1/src/agentql/async_api/_session.py` & `agentql-0.4.2/src/agentql/async_api/_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+# pylint: disable=protected-access
+
 import copy
 import logging
 import os
-from typing import Callable, Generic, List, Literal, Optional
+from typing import Callable, Generic, List, Literal, Optional, Union
 
 import httpx
 
 from agentql import (
     AgentQLServerError,
     AgentQLServerTimeoutError,
     APIKeyError,
     AttributeNotFoundError,
     QueryParser,
     UnableToClosePopupError,
+    trail_logger,
 )
 from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
+from agentql._core._utils import minify_query
 
 from ._popup import Popup
 from ._response_proxy import AQLResponseProxy
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
@@ -44,22 +48,22 @@
         self._web_driver = web_driver
         self._event_listeners = {}
         self._check_popup = False
         self._last_query = None
         self._last_response = None
 
     @property
-    async def current_page(self) -> PageTypeT:
+    def current_page(self) -> PageTypeT:
         """Get the current page being processed by AgentQL.
 
         Returns:
         -------
         PageTypeT: A type variable representing the type of a page in a web driver session. If you did not pass a customized web driver when starting the session, then it will return [Playwright Page](https://playwright.dev/python/docs/api/class-page) object.
         """
-        return await self._web_driver.get_current_page()
+        return self._web_driver.current_page
 
     @property
     def driver(self) -> WebDriver[InteractiveItemTypeT, PageTypeT]:
         """Get the web driver.
 
         Returns:
         -------
@@ -73,14 +77,21 @@
         return self._last_query
 
     @property
     def last_response(self) -> Optional[dict]:
         """Get the last response."""
         return self._last_response
 
+    def get_last_trail(self) -> Union[trail_logger.TrailLogger, None]:
+        """
+        Get the last trail recorded, if enable_history_log is True when starting the session.
+        """
+        logger_store = trail_logger.TrailLoggerStore.get_loggers()
+        return logger_store[-1] if logger_store else None
+
     async def query(
         self,
         query: str,
         timeout: int = 500,
         lazy_load_pages_count: int = 0,
         wait_for_network_idle: bool = True,
         include_aria_hidden: bool = False,
@@ -94,61 +105,64 @@
         lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
         wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
 
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
+        trail_logger.add_event(f"Querying {minify_query(query)} on {self._web_driver.current_page}")
         log.debug(f"querying {query}")
 
         self._last_query = query
         parser = QueryParser(query)
         query_tree = parser.parse()
 
         await self._web_driver.wait_for_page_ready_state(
             wait_for_network_idle=wait_for_network_idle
         )
 
-        accessibility_tree = await self._web_driver.prepare_accessibility_tree(
+        accessibility_tree = await self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
         # Check if there is a popup in the page before sending the agentql query
+        popup_list = []
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 await self._handle_popup(popup_list)
 
         response = await self._query(query, accessibility_tree, timeout)
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
-            accessibility_tree = await self._web_driver.get_accessibility_tree()
+            accessibility_tree = await self._web_driver.accessibility_tree
 
             popup_list = self._detect_popup(accessibility_tree, popup_list)
             if popup_list:
                 await self._handle_popup(popup_list)
 
         return AQLResponseProxy[InteractiveItemTypeT](response, self._web_driver, query_tree)
 
     async def get_user_auth_session(self) -> dict:
         """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         User auth session in Python dictionary format.
         """
-        return await self._web_driver.get_user_auth_session()
+        return await self._web_driver._get_user_auth_session()
 
     async def stop(self):
         """Close the session."""
         log.debug("closing session")
-        await self._web_driver.stop_browser()
+        await self._web_driver._stop_browser()
+        trail_logger.finalize()
 
     def on(self, event: Literal["popup"], callback: Callable[[dict], None]):
         """Emitted when there is a popup (such as promotion window) on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections.
 
         Event Data:
         -----------
         popups (list): The list of popups captured on the page by AgentQL Popup Detection algorithm.
@@ -169,15 +183,15 @@
         timeout (int): The timeout value for the connection with backend api service
 
         Returns:
         -------
         dict: AgentQL response in json format.
         """
         try:
-            page_url = await self._web_driver.get_current_url()
+            page_url = self._web_driver.current_url
             request_data = {
                 "query": f"{query}",
                 "accessibility_tree": accessibility_tree,
                 "metadata": {"url": page_url},
             }
             url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + GET_AGENTQL_ENDPOINT
             log.debug(f"Making request to {url}")
@@ -225,15 +239,15 @@
         popup_list = []
         if tree_role == "dialog":
             popup = Popup(copy.deepcopy(tree), tree_name, self._close_popup)
 
             # Avoid adding existing popup to the dict and double handle the popup
             if known_popups:
                 for popup_object in known_popups:
-                    if popup_object.name() != popup.name():
+                    if popup_object.name != popup.name:
                         popup_list.append(popup)
             else:
                 popup_list.append(popup)
 
             return popup_list
 
         if "children" in tree:
```

### Comparing `agentql-0.4.1/src/agentql/async_api/_web_driver.py` & `agentql-0.4.2/src/agentql/async_api/_web_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any
+from typing import Any, Optional
 
 from typing_extensions import Protocol
 
 from agentql import InteractiveItemTypeT, PageTypeT
 
 
 class ScrollDirection(Enum):
@@ -12,127 +12,134 @@
 
 
 class WebDriver(Protocol[InteractiveItemTypeT, PageTypeT]):
     """
     The WebDriver protocol is a part of the AgentQL SDK, designed to facilitate custom web driver implementations. This protocol outlines the necessary interface for a web driver compatible with AgentQL, enabling interaction with web elements, page navigation, and accessibility tree manipulation.
     """
 
-    def locate_interactive_element(self, response_data: dict) -> InteractiveItemTypeT:
-        """
-        Locates an interactive element in the web page.
-
-        Parameters:
-        -----------
-        response_data (dict): The data of the interactive element from the AgentQL response.
-
-        Returns:
-        --------
-        InteractiveItemTypeT: The interactive element.
-        """
-
-    async def get_text_content(self, web_element: InteractiveItemTypeT) -> str:
+    async def get_text_content(self, web_element: InteractiveItemTypeT) -> Optional[str]:
         """
         Gets the text content of the web element.
 
         Parameters:
         -----------
         web_element (InteractiveItemTypeT): The web element to get text from.
 
         Returns:
         --------
         str: The text content of the web element."""
 
-    async def start_browser(self, user_auth_session: Any = None):
-        """Starts a new browser session and set user session state (if there is any).
-
-        Parameters:
-        -----------
-        user_auth_session (optional): The user authentication session that contains previous login session.
-        """
-
-    async def stop_browser(self):
-        """Closes the current browser session."""
-
     async def open_url(self, url: str, new_page: bool = False):
         """Open URL in the browser.
 
         Parameters:
         ----------
         url (str): The URL to open.
         new_page (bool): Whether to open the URL in a new page.
         """
 
-    async def get_current_url(self) -> str:
-        """Get the URL of the current page being processed by AgentQL.
+    async def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
+        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
 
-        Returns:
-        --------
-        str: The URL of the current page.
+        Parameters:
+        -----------
+        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
         """
 
-    async def prepare_accessibility_tree(self, lazy_load_pages_count: int) -> dict:
-        """Prepare the accessibility tree by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
+    async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
+        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
-        lazy_load_pages_count (int): The number of times to scroll down and up the page when preparing the page. This will trigger lazy loading contents on the page.
-        include_aria_hidden: Whether to include elements with aria-hidden attribute in the AT.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
+        pixels (int) (optional): The number of pixels to scroll. 720 by default.
+        """
+
+    async def scroll_to_bottom(self):
+        """Scrolls to the bottom of the current page."""
+
+    async def scroll_to_top(self):
+        """Scrolls to the top of the current page."""
+
+    @property
+    async def accessibility_tree(self) -> dict:
+        """Returns the up-to-date accessibility tree of the page.
 
         Returns:
         --------
         dict: The accessibility tree of the page in Python Dict format.
         """
 
-    async def get_accessibility_tree(self) -> dict:
-        """Returns the up-to-date accessibility tree of the page.
+    @property
+    def current_url(self) -> str:
+        """Get the URL of the current page being processed by AgentQL.
 
         Returns:
         --------
-        dict: The accessibility tree of the page in Python Dict format.
+        str: The URL of the current page.
         """
 
-    async def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
-        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
+    @property
+    def html(self) -> Optional[str]:
+        """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page.".
 
-        Parameters:
-        -----------
-        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
+        Returns:
+        --------
+        dict: The HTML content of the web page.
         """
 
-    async def get_user_auth_session(self) -> Any:
-        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+    @property
+    def current_page(self) -> PageTypeT:
+        """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
         --------
-        The user session state.
+        PageTypeT: The current page object.
         """
 
-    async def get_html(self) -> dict:
-        """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page.".
+    async def _get_user_auth_session(self) -> Any:
+        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
-        dict: The HTML content of the web page.
+        The user session state.
         """
 
-    async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
-        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
+    def _locate_interactive_element(self, response_data: dict) -> InteractiveItemTypeT:
+        """
+        Locates an interactive element in the web page.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
-        pixels (int) (optional): The number of pixels to scroll. 720 by default.
-        """
+        response_data (dict): The data of the interactive element from the AgentQL response.
 
-    async def scroll_to_bottom(self):
-        """Scrolls to the bottom of the current page."""
+        Returns:
+        --------
+        InteractiveItemTypeT: The interactive element.
+        """
 
-    async def scroll_to_top(self):
-        """Scrolls to the top of the current page."""
+    async def _prepare_accessibility_tree(
+        self, lazy_load_pages_count: int, include_aria_hidden: bool
+    ) -> dict:
+        """Prepare the accessibility tree by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
 
-    async def get_current_page(self) -> PageTypeT:
-        """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
+        Parameters:
+        -----------
+        lazy_load_pages_count (int): The number of times to scroll down and up the page when preparing the page. This will trigger lazy loading contents on the page.
+        include_aria_hidden: Whether to include elements with aria-hidden attribute in the AT.
 
         Returns:
         --------
-        PageTypeT: The current page object.
+        dict: The accessibility tree of the page in Python Dict format.
+        """
+
+    async def _start_browser(self, user_auth_session: Any = None):
+        """Starts a new browser session and set user session state (if there is any).
+
+        Parameters:
+        -----------
+        user_auth_session (optional): The user authentication session that contains previous login session.
         """
+
+    async def _stop_browser(self):
+        """Closes the current browser session."""
```

### Comparing `agentql-0.4.1/src/agentql/ext/playwright/_html_constants.py` & `agentql-0.4.2/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/ext/playwright/_network_monitor.py` & `agentql-0.4.2/src/agentql/ext/playwright/_network_monitor.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_async.py` & `agentql-0.4.2/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import asyncio
 import time
 from typing import Optional, Union
 
-from playwright.async_api import Error, Frame, Locator, Page, StorageState, async_playwright
+from playwright.async_api import (
+    ElementHandle,
+    Error,
+    Frame,
+    FrameLocator,
+    Locator,
+    Page,
+    StorageState,
+    async_playwright,
+)
 from playwright_stealth import StealthConfig, stealth_async
 
+from agentql import trail_logger
 from agentql._core._errors import (
     AccessibilityTreeError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
 )
@@ -23,15 +33,15 @@
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
     """
     PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
     """
 
-    def __init__(self, headless=False, proxy: ProxySettings = None) -> None:
+    def __init__(self, headless=False, proxy: Optional[ProxySettings] = None) -> None:
         """
         Construct the PlaywrightWebDriver instance.
 
         Parameters:
         -----------
         headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
         proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
@@ -61,35 +71,15 @@
 
         self._page_monitor = None
 
         self._current_tf_id = None
 
         self._stealth_mode_config = None
 
-    def locate_interactive_element(self, response_data: dict) -> Locator:
-        """
-        Locates an interactive element in the web page.
-
-        Parameters:
-        -----------
-
-        response_data (dict): The data of the interactive element from the AgentQL response.
-
-        Returns:
-        --------
-
-        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
-        """
-        tf623_id = response_data.get("tf623_id")
-        if not tf623_id:
-            raise ElementNotFoundError("tf623_id")
-        iframe_path = response_data.get("attributes", {}).get("iframe_path")
-        return self.find_element_by_id(tf623_id, iframe_path)
-
-    async def get_text_content(self, web_element: Locator) -> str:
+    async def get_text_content(self, web_element: Locator) -> Optional[str]:
         """
         Gets the text content of the web element.
 
         Parameters:
         -----------
 
         web_element ([Playwright Locator](https://playwright.dev/python/docs/api/class-locator)): The web element represented by Playwright's Locator object.
@@ -97,52 +87,28 @@
         Returns:
         --------
 
         str: The text content of the web element.
         """
         return await web_element.text_content()
 
-    async def start_browser(self, user_auth_session: StorageState = None):
-        """
-        Starts a new browser session and set user session state (if there is any).
-
-        Parameters:
-        -----------
-        user_auth_session (optional): The user authentication session information.
-        """
-        await self._start_browser(
-            headless=self._headless, user_session_extras=user_auth_session, proxy=self._proxy
-        )
-
     @property
     def is_headless(self) -> bool:
         """Returns whether the browser is running in headless mode or not.
 
         Returns:
         --------
         bool: True if the browser is running in headless mode, False otherwise."""
         return self._headless
 
-    async def stop_browser(self):
-        """Closes the current browser session."""
-        if self._context:
-            await self._context.close()
-            self._context = None
-        if self._browser:
-            await self._browser.close()
-            self._browser = None
-        if self._playwright:
-            await self._playwright.stop()
-            self._playwright = None
-
     def enable_stealth_mode(
         self,
         webgl_vendor: str = VENDOR,
         webgl_renderer: str = RENDERER,
-        nav_user_agent: Optional[str] = USER_AGENT,
+        nav_user_agent: str = USER_AGENT,
     ):
         """Enable the stealth mode and set the stealth mode configuration.
         Ideally parameters values should match some real values to avoid detection.
         To get a realistic examples, you can use browser fingerprinting websites such as https://bot.sannysoft.com/ and https://pixelscan.net/
 
         Parameters:
         -----------
@@ -168,37 +134,40 @@
         if not self._browser:
             raise NoOpenBrowserError()
         if new_page or self._current_page is None:
             await self._open_url(url)
         else:
             await self._current_page.goto(url, wait_until="load")
 
-    async def get_current_url(self) -> str:
+    @property
+    def current_url(self) -> str:
         """Get the URL of the current page being processed by AgentQL.
 
         Returns:
         --------
         str: The URL of the current page.
         """
         if not self._current_page:
             raise NoOpenPageError()
         return self._current_page.url
 
-    async def get_html(self) -> dict:
+    @property
+    def html(self) -> Optional[str]:
         """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page".
 
         Returns:
         --------
         dict: The HTML content of the web page in Dict format.
         """
         if not self._current_page:
             raise NoOpenPageError()
         return self._original_html
 
-    async def get_current_page(self) -> Page:
+    @property
+    def current_page(self) -> Page:
         """Returns the [Playwright page object](https://playwright.dev/python/docs/api/class-page) that represents the current page. Users could do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
         --------
         [Playwright Page](https://playwright.dev/python/docs/api/class-page): The current page.
         """
         if not self._current_page:
@@ -209,70 +178,38 @@
         """
         Opens a new page and loads the given HTML content.
 
         Parameters:
         -----------
         html (str): The HTML content to load in the page.
         """
-        if not self._browser:
+        if not self._browser or not self._context:
             raise NoOpenBrowserError()
         self._current_page = await self._context.new_page()
         self._current_tf_id = 0
         await self._current_page.set_content(html)
 
-    async def prepare_accessibility_tree(
-        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
-    ) -> dict:
-        """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
-
-        Parameters:
-        -----------
-        lazy_load_pages_count: The number of times to scroll down and up the page.
-
-        Returns:
-        --------
-        dict: AT of the page
-        """
-        if not self._current_page:
-            raise NoOpenPageError()
-
-        self._original_html = await self._current_page.content()
-        await self._page_scroll(pages=lazy_load_pages_count)
-
-        accessibility_tree = None
-        try:
-            accessibility_tree = await self._get_page_accessibility_tree(
-                self._current_page, include_aria_hidden=include_aria_hidden
-            )
-            await self._process_iframes(accessibility_tree)
-            await self._post_process_accessibility_tree(accessibility_tree)
-
-        except Exception as e:
-            raise AccessibilityTreeError() from e
-
-        return accessibility_tree
-
-    async def get_accessibility_tree(self) -> dict:
+    @property
+    async def accessibility_tree(self) -> dict:
         """Returns the up-to-date accessibility tree of the page.
 
         Returns:
         --------
         dict: The accessibility tree of the page in Dict format.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         try:
             accessibility_tree = await self._get_page_accessibility_tree(self._current_page)
             await self._process_iframes(accessibility_tree)
+            return accessibility_tree
         except Exception as e:
             raise AccessibilityTreeError() from e
 
-        return accessibility_tree
-
     async def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
         """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
 
         Usage:
         -----
         ```py
         session = agentql.start_async_session(YOUTUBE_URL)
@@ -331,56 +268,89 @@
     async def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         await self._current_page.evaluate(load_js("scroll_to_top"))
 
-    async def get_user_auth_session(self) -> StorageState:
+    async def _get_user_auth_session(self) -> StorageState:
         """
-        **NOT RECOMMENDED** (Use session.get_user_auth_session() instead)
-
         Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         dict: User auth session in Python dictionary format.
         """
-        if not self._browser:
+        if not self._context:
             raise NoOpenBrowserError()
         return await self._context.storage_state()
 
+    async def _prepare_accessibility_tree(
+        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
+    ) -> dict:
+        """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
+
+        Parameters:
+        -----------
+        lazy_load_pages_count: The number of times to scroll down and up the page.
+
+        Returns:
+        --------
+        dict: AT of the page
+        """
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        self._original_html = await self._current_page.content()
+        await self._page_scroll(pages=lazy_load_pages_count)
+
+        try:
+            accessibility_tree = await self._get_page_accessibility_tree(
+                self._current_page, include_aria_hidden=include_aria_hidden
+            )
+            await self._process_iframes(accessibility_tree)
+            await self._post_process_accessibility_tree(accessibility_tree)
+            return accessibility_tree
+
+        except Exception as e:
+            raise AccessibilityTreeError() from e
+
     async def _post_process_accessibility_tree(self, accessibility_tree: dict):
         """Post-process the accessibility tree by removing node's attributes that are Null."""
         if "children" in accessibility_tree and accessibility_tree.get("children") is None:
             del accessibility_tree["children"]
 
         for child in accessibility_tree.get("children", []):
             await self._post_process_accessibility_tree(child)
 
     async def _process_iframes(
         self,
-        page_accessibility_tree: dict = None,
+        page_accessibility_tree: dict,
         *,
         iframe_path: str = "",
-        frame: Frame = None,
+        frame: Union[Frame, ElementHandle, None] = None,
     ):
         """
         Recursively retrieves the accessibility trees for all iframes in a page or frame.
 
         Parameters:
         ----------
         iframe_path (str): The path of the iframe in the frame hierarchy.
         frame (Frame): The frame object representing the current frame.
         page_accessibility_tree (dict): The accessibility tree of the page.
         """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if frame is None:
             iframes = await self._current_page.query_selector_all("iframe")
         else:
             content_frame = await frame.content_frame()
+            if not content_frame:
+                return
             iframes = await content_frame.query_selector_all("iframe")
 
         for iframe in iframes:
             iframe_id = await iframe.get_attribute("tf623_id")
             iframe_path_to_send = ""
             if iframe_path:
                 iframe_path_to_send = f"{iframe_path}."
@@ -423,15 +393,17 @@
             },
         )
 
         self._current_tf_id = result.get("lastUsedId")
 
         return result.get("tree")
 
-    async def _get_frame_accessibility_tree(self, frame: Frame, iframe_path) -> dict:
+    async def _get_frame_accessibility_tree(
+        self, frame: Union[Frame, ElementHandle], iframe_path
+    ) -> dict:
         """
         Retrieves the accessibility tree for a given frame.
 
         Parameters:
         ----------
         frame (Frame): The frame for which to retrieve the accessibility tree.
         iframe_path: The path of the iframe within the frame.
@@ -472,47 +444,73 @@
             if "tf623_id" in attributes and attributes["tf623_id"] == iframe_id:
                 if not child.get("children"):
                     child["children"] = []
                 child["children"].append(iframe_accessibility_tree)
                 break
             self._merge_iframe_tree_into_page(iframe_id, child, iframe_accessibility_tree)
 
+    def _locate_interactive_element(self, response_data: dict) -> Locator:
+        """
+        Locates an interactive element in the web page.
+
+        Parameters:
+        -----------
+
+        response_data (dict): The data of the interactive element from the AgentQL response.
+
+        Returns:
+        --------
+
+        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
+        """
+        tf623_id = response_data.get("tf623_id")
+        if not tf623_id:
+            raise ElementNotFoundError("tf623_id")
+        iframe_path = response_data.get("attributes", {}).get("iframe_path")
+        interactive_element = self._find_element_by_id(tf623_id, iframe_path)
+        trail_logger.spy_on_object(interactive_element)
+        return interactive_element
+
     async def _apply_stealth_mode_to_page(self, page: Page):
         """Applies stealth mode to the given page.
 
         Parameters:
         ----------
         page (Page): The page to which stealth mode will be applied.
         """
         # Only mask User Agent in headless mode to avoid detection for headless browsers
         mask_user_agent = self._headless
 
-        await stealth_async(
-            page,
-            config=StealthConfig(
-                vendor=self._stealth_mode_config["vendor"],
-                renderer=self._stealth_mode_config["renderer"],
-                # nav_user_agent will only take effect when navigator_user_agent parameter is True
-                nav_user_agent=self._stealth_mode_config["nav_user_agent"],
-                navigator_user_agent=mask_user_agent,
-            ),
-        )
+        if self._stealth_mode_config is not None:
+            await stealth_async(
+                page,
+                config=StealthConfig(
+                    vendor=self._stealth_mode_config["vendor"],
+                    renderer=self._stealth_mode_config["renderer"],
+                    # nav_user_agent will only take effect when navigator_user_agent parameter is True
+                    nav_user_agent=self._stealth_mode_config["nav_user_agent"],
+                    navigator_user_agent=mask_user_agent,
+                ),
+            )
 
     async def _open_url(self, url: str):
         """Opens a new page and navigates to the given URL. Initialize the storgage state if provided.
 
         Parameters:
         ----------
         url (str): The URL to navigate to.
         storgate_state_content (optional): The storage state with which user would like to initialize the browser.
         """
 
         self._current_page = None
         url = ensure_url_scheme(url)
 
+        if not self._context:
+            raise NoOpenBrowserError()
+
         try:
             page = await self._context.new_page()
             if self._stealth_mode_config is not None:
                 await self._apply_stealth_mode_to_page(page)
             self._current_tf_id = 0
             await page.goto(url, wait_until="domcontentloaded")
         except Exception as e:
@@ -540,14 +538,17 @@
         Parameters:
         ----------
         pages (int): The number of pages to scroll down.
         """
         if pages < 1:
             return
 
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if self._stealth_mode_config is None:
             delta_y = 10000
             for _ in range(pages):
                 await self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
                 await asyncio.sleep(0.1)
 
             delta_y = -10000
@@ -564,17 +565,15 @@
 
             for _ in range(pages):
                 await self.scroll_to_top()
                 await asyncio.sleep(0.1)
 
     async def _start_browser(
         self,
-        user_session_extras: dict = None,
-        headless=True,
-        proxy: ProxySettings = None,
+        user_auth_session: Optional[StorageState] = None,
     ):
         """Starts a new browser session and set storage state (if there is any).
 
         Parameters:
         ----------
         user_session_extras (optional): the JSON object that holds user session information
         headless (bool): Whether to start the browser in headless mode.
@@ -587,42 +586,61 @@
         args = [
             "--no-sandbox",
             "--disable-setuid-sandbox",
             "--disable-blink-features=AutomationControlled",
         ]
         self._playwright = await async_playwright().start()
         self._browser = await self._playwright.chromium.launch(
-            headless=headless, proxy=proxy, args=args, ignore_default_args=ignored_args
+            headless=self._headless, proxy=self._proxy, args=args, ignore_default_args=ignored_args
         )
         self._current_tf_id = 0
         self._context = await self._browser.new_context(
-            user_agent=USER_AGENT, storage_state=user_session_extras
+            user_agent=USER_AGENT, storage_state=user_auth_session
         )
 
-    def _get_frame_context(self, iframe_path: str = None) -> Union[Frame, Page]:
+    async def _stop_browser(self):
+        """Closes the current browser session."""
+        if self._current_page:
+            await self._current_page.close()
+            self._current_page = None
+        if self._context:
+            await self._context.close()
+            self._context = None
+        if self._browser:
+            await self._browser.close()
+            self._browser = None
+        if self._playwright:
+            await self._playwright.stop()
+            self._playwright = None
+
+    def _get_frame_context(self, iframe_path: Optional[str] = None) -> Union[FrameLocator, Page]:
         """
         Returns the frame context for the given iframe path.
 
         Parameters:
         ----------
         iframe_path (str): The path of the iframe within the frame.
 
         Returns:
         --------
         Frame | Page: The frame context for the given iframe path.
         """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if not iframe_path:
             return self._current_page
+
         iframe_path_list = iframe_path.split(".")
         frame_context = self._current_page
         for iframe_id in iframe_path_list:
             frame_context = frame_context.frame_locator(f"[tf623_id='{iframe_id}']")
         return frame_context
 
-    def find_element_by_id(self, tf623_id: str, iframe_path: str = None) -> Locator:
+    def _find_element_by_id(self, tf623_id: str, iframe_path: str = "") -> Locator:
         """
         Finds an element by its TF ID within a specified iframe.
 
         Parameters:
         ----------
         tf623_id (str): The generated tf id of the element to find.
         iframe_path (str): The path to the iframe containing the element.
@@ -640,14 +658,20 @@
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
             raise ElementNotFoundError(tf623_id) from e
 
     async def _determine_load_state(
         self, monitor: PageActivityMonitor, timeout_seconds=14, wait_for_network_idle=True
     ):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         start_time = time.time()
 
         while True:
             if wait_for_network_idle:
                 try:
                     last_updated_timestamp = await self._current_page.evaluate(
                         load_js("get_last_dom_change")
@@ -667,14 +691,20 @@
                     break
 
             if time.time() - start_time > timeout_seconds:
                 break
             await asyncio.sleep(0.1)
 
     async def _add_page_event_listeners(self):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         self._current_page.on("request", self._page_monitor.track_network_request)
         self._current_page.on("requestfinished", self._page_monitor.track_network_response)
         self._current_page.on("requestfailed", self._page_monitor.track_network_response)
         self._current_page.on("load", self._page_monitor.track_load)
 
         try:
             await self._current_page.evaluate(load_js("add_dom_change_listener"))
@@ -683,14 +713,20 @@
             start_time = time.time()
             while True:
                 if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                     break
                 await asyncio.sleep(0.2)
 
     async def _remove_page_event_listeners(self):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         self._current_page.remove_listener("request", self._page_monitor.track_network_request)
         self._current_page.remove_listener(
             "requestfinished", self._page_monitor.track_network_response
         )
         self._current_page.remove_listener(
             "requestfailed", self._page_monitor.track_network_response
         )
```

### Comparing `agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_sync.py` & `agentql-0.4.2/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import time
 from typing import Optional, Union
 
-from playwright.sync_api import Error, Frame, Locator, Page, StorageState, sync_playwright
+from playwright.sync_api import (
+    ElementHandle,
+    Error,
+    Frame,
+    FrameLocator,
+    Locator,
+    Page,
+    StorageState,
+    sync_playwright,
+)
 from playwright_stealth import StealthConfig, stealth_sync
 
+from agentql import trail_logger
 from agentql._core._errors import (
     AccessibilityTreeError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
 )
@@ -22,15 +32,15 @@
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
     """
     PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
     """
 
-    def __init__(self, headless=False, proxy: ProxySettings = None) -> None:
+    def __init__(self, headless=False, proxy: Optional[ProxySettings] = None) -> None:
         """
         Construct the PlaywrightWebDriver instance.
 
         Parameters:
         -----------
         headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
         proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
@@ -60,44 +70,24 @@
 
         self._page_monitor = None
 
         self._current_tf_id = None
 
         self._stealth_mode_config = None
 
-    def locate_interactive_element(self, response_data: dict) -> Locator:
-        """
-        Locates an interactive element in the web page.
-
-        Parameters:
-        -----------
-
-        response_data (dict): The data of the interactive element from the AgentQL response.
-
-        Returns:
-        --------
-
-        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
-        """
-        tf623_id = response_data.get("tf623_id")
-        if not tf623_id:
-            raise ElementNotFoundError("tf623_id")
-        iframe_path = response_data.get("attributes", {}).get("iframe_path")
-        return self.find_element_by_id(tf623_id, iframe_path)
-
     @property
     def is_headless(self) -> bool:
         """Returns whether the browser is running in headless mode or not.
 
         Returns:
         --------
         bool: True if the browser is running in headless mode, False otherwise."""
         return self._headless
 
-    def get_text_content(self, web_element: Locator) -> str:
+    def get_text_content(self, web_element: Locator) -> Optional[str]:
         """
         Gets the text content of the web element.
 
         Parameters:
         -----------
 
         web_element ([Playwright Locator](https://playwright.dev/python/docs/api/class-locator)): The web element represented by Playwright's Locator object.
@@ -105,43 +95,34 @@
         Returns:
         --------
 
         str: The text content of the web element.
         """
         return web_element.text_content()
 
-    def start_browser(self, user_auth_session: StorageState = None):
-        """
-        Starts a new browser session and set user session state (if there is any).
-
-        Parameters:
-        -----------
-        user_auth_session (optional): The user authentication session information.
-        """
-        self._start_browser(
-            headless=self._headless, user_auth_session=user_auth_session, proxy=self._proxy
-        )
-
-    def stop_browser(self):
+    def _stop_browser(self):
         """Closes the current browser session."""
+        if self._current_page:
+            self._current_page.close()
+            self._current_page = None
         if self._context:
             self._context.close()
             self._context = None
         if self._browser:
             self._browser.close()
             self._browser = None
         if self._playwright:
             self._playwright.stop()
             self._playwright = None
 
     def enable_stealth_mode(
         self,
         webgl_vendor: str = VENDOR,
         webgl_renderer: str = RENDERER,
-        nav_user_agent: Optional[str] = USER_AGENT,
+        nav_user_agent: str = USER_AGENT,
     ):
         """Enable the stealth mode and set the stealth mode configuration.
         Ideally parameters values should match some real values to avoid detection.
         To get a realistic examples, you can use browser fingerprinting websites such as https://bot.sannysoft.com/ and https://pixelscan.net/
 
         Parameters:
         -----------
@@ -168,138 +149,82 @@
             raise NoOpenBrowserError()
 
         if new_page or self._current_page is None:
             self._open_url(url)
         else:
             self._current_page.goto(url, wait_until="domcontentloaded")
 
-    def get_current_url(self) -> str:
+    @property
+    def current_url(self) -> str:
         """Get the URL of the current page being processed by AgentQL.
 
         Returns:
         --------
         str: The URL of the current page.
         """
         if not self._current_page:
             raise NoOpenPageError()
         return self._current_page.url
 
-    def get_html(self) -> dict:
+    @property
+    def html(self) -> Optional[str]:
         """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page".
 
         Returns:
         --------
         dict: The HTML content of the web page in Dict format.
         """
         if not self._current_page:
             raise NoOpenPageError()
         return self._original_html
 
-    def get_current_page(self) -> Page:
+    @property
+    def current_page(self) -> Page:
         """Returns the [Playwright page object](https://playwright.dev/python/docs/api/class-page) that represents the current page. Users could do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
         --------
         [Playwright Page](https://playwright.dev/python/docs/api/class-page): The current page.
         """
         if not self._current_page:
             raise NoOpenPageError()
         return self._current_page
 
-    def navigate_to(self, url: str):
-        """Navigates the current page to the given URL.
-
-        Parameters:
-        ----------
-        url (str): The URL to navigate to.
-        """
-        if not self._current_page:
-            self._open_url(url)
-        else:
-            self._current_page.goto(url, wait_until="load")
-
     def open_html(self, html: str):
         """
         Opens a new page and loads the given HTML content.
 
         Parameters:
         -----------
         html (str): The HTML content to load in the page.
         """
-        if not self._browser:
+        if not self._browser or not self._context:
             raise NoOpenBrowserError()
         self._current_page = self._context.new_page()
         self._current_tf_id = 0
         self._current_page.set_content(html)
 
-    def prepare_accessibility_tree(
-        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
-    ) -> dict:
-        """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
-
-        Parameters:
-        -----------
-        lazy_load_pages_count (int): The number of times to scroll down and up the page.
-        include_aria_hidden (bool): Whether to include elements with aria-hidden attribute in the accessibility tree.
-
-        Returns:
-        --------
-        dict: AT of the page
-        """
-        if not self._current_page:
-            raise NoOpenPageError()
-
-        self._original_html = self._current_page.content()
-        self._page_scroll(pages=lazy_load_pages_count)
-
-        accessibility_tree = None
-        try:
-            accessibility_tree = self._get_page_accessibility_tree(
-                self._current_page, include_aria_hidden=include_aria_hidden
-            )
-            self._process_iframes(accessibility_tree)
-            self._post_process_accessibility_tree(accessibility_tree)
-
-        except Exception as e:
-            raise AccessibilityTreeError() from e
-
-        return accessibility_tree
-
-    def get_accessibility_tree(self) -> dict:
+    @property
+    def accessibility_tree(self) -> dict:
         """Returns the up-to-date accessibility tree of the page.
 
         Returns:
         --------
         dict: The accessibility tree of the page in Dict format.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         try:
             accessibility_tree = self._get_page_accessibility_tree(self._current_page)
             self._process_iframes(accessibility_tree)
+            return accessibility_tree
         except Exception as e:
             raise AccessibilityTreeError() from e
 
-        return accessibility_tree
-
-    def get_user_auth_session(self) -> StorageState:
-        """
-        **NOT RECOMMENDED** (Use session.get_user_auth_session() instead)
-
-        Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
-
-        Returns:
-        --------
-        dict: User auth session in Python dictionary format.
-        """
-        if not self._browser:
-            raise NoOpenBrowserError()
-        return self._context.storage_state()
-
     def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
         """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
 
         Usage:
         -----
         ```py
         session = agentql.start_async_session(YOUTUBE_URL)
@@ -315,14 +240,15 @@
         Parameters:
         -----------
         wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
+        trail_logger.add_event(f"Waiting for {self._current_page} to reach 'Page Ready' state")
         if not self._page_monitor:
             self._page_monitor = PageActivityMonitor()
         else:
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
@@ -330,14 +256,18 @@
 
         # Wait for the page to reach the "Page Ready" state
         self._determine_load_state(self._page_monitor, wait_for_network_idle)
 
         # Remove the event listeners to prevent overwhelming the async event loop
         self._remove_page_event_listeners()
 
+        trail_logger.add_event(
+            f"Finished waiting for {self._current_page} to reach 'Page Ready' state"
+        )
+
     def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
         scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
@@ -358,42 +288,110 @@
     def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         self._current_page.evaluate(load_js("scroll_to_top"))
 
+    def _get_user_auth_session(self) -> StorageState:
+        """
+        Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+
+        Returns:
+        --------
+        dict: User auth session in Python dictionary format.
+        """
+        if not self._browser or not self._context:
+            raise NoOpenBrowserError()
+        return self._context.storage_state()
+
+    def _locate_interactive_element(self, response_data: dict) -> Locator:
+        """
+        Locates an interactive element in the web page.
+
+        Parameters:
+        -----------
+
+        response_data (dict): The data of the interactive element from the AgentQL response.
+
+        Returns:
+        --------
+
+        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
+        """
+        tf623_id = response_data.get("tf623_id")
+        if not tf623_id:
+            raise ElementNotFoundError("tf623_id")
+        iframe_path = response_data.get("attributes", {}).get("iframe_path")
+        interactive_element = self._find_element_by_id(tf623_id, iframe_path)
+        trail_logger.spy_on_object(interactive_element)
+        return interactive_element
+
+    def _prepare_accessibility_tree(
+        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
+    ) -> dict:
+        """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
+
+        Parameters:
+        -----------
+        lazy_load_pages_count (int): The number of times to scroll down and up the page.
+        include_aria_hidden (bool): Whether to include elements with aria-hidden attribute in the accessibility tree.
+
+        Returns:
+        --------
+        dict: AT of the page
+        """
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        self._original_html = self._current_page.content()
+        self._page_scroll(pages=lazy_load_pages_count)
+
+        try:
+            accessibility_tree = self._get_page_accessibility_tree(
+                self._current_page, include_aria_hidden=include_aria_hidden
+            )
+            self._process_iframes(accessibility_tree)
+            self._post_process_accessibility_tree(accessibility_tree)
+            return accessibility_tree
+
+        except Exception as e:
+            raise AccessibilityTreeError() from e
+
     def _post_process_accessibility_tree(self, accessibility_tree: dict):
         """Post-process the accessibility tree by removing node's attributes that are Null."""
         if "children" in accessibility_tree and accessibility_tree.get("children") is None:
             del accessibility_tree["children"]
 
         for child in accessibility_tree.get("children", []):
             self._post_process_accessibility_tree(child)
 
     def _process_iframes(
         self,
-        page_accessibility_tree: dict = None,
+        page_accessibility_tree: dict,
         *,
         iframe_path: str = "",
-        frame: Frame = None,
+        frame: Union[Frame, ElementHandle, None] = None,
     ):
         """
         Recursively retrieves the accessibility trees for all iframes in a page or frame.
 
         Parameters:
         ----------
         iframe_path (str): The path of the iframe in the frame hierarchy.
         frame (Frame): The frame object representing the current frame.
         page_accessibility_tree (dict): The accessibility tree of the page.
 
         Returns:
         --------
         None
         """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if frame is None:
             iframes = self._current_page.query_selector_all("iframe")
         else:
             frame = frame.content_frame()
             if not frame:
                 return
             iframes = frame.query_selector_all("iframe")
@@ -442,15 +440,17 @@
             },
         )
 
         self._current_tf_id = result.get("lastUsedId")
 
         return result.get("tree")
 
-    def _get_frame_accessibility_tree(self, frame: Frame, iframe_path) -> dict:
+    def _get_frame_accessibility_tree(
+        self, frame: Union[Frame, ElementHandle], iframe_path
+    ) -> dict:
         """
         Retrieves the accessibility tree for a given frame.
 
         Parameters:
         ----------
         frame (Frame): The frame for which to retrieve the accessibility tree.
         iframe_path: The path of the iframe within the frame.
@@ -503,14 +503,17 @@
         Parameters:
         ----------
         page (Page): The page to which stealth mode will be applied.
         """
         # Only mask User Agent in headless mode to avoid detection for headless browsers
         mask_user_agent = self._headless
 
+        if self._stealth_mode_config is None:
+            return
+
         stealth_sync(
             page,
             config=StealthConfig(
                 vendor=self._stealth_mode_config["vendor"],
                 renderer=self._stealth_mode_config["renderer"],
                 # nav_user_agent will only take effect when navigator_user_agent parameter is True
                 nav_user_agent=self._stealth_mode_config["nav_user_agent"],
@@ -526,14 +529,17 @@
         url (str): The URL to navigate to.
         storgate_state_content (optional): The storage state with which user would like to initialize the browser.
         """
 
         self._current_page = None
         url = ensure_url_scheme(url)
 
+        if not self._browser or not self._context:
+            raise NoOpenBrowserError()
+
         try:
             page = self._context.new_page()
             if self._stealth_mode_config is not None:
                 self._apply_stealth_mode_to_page(page)
             self._current_tf_id = 0
             page.goto(url, wait_until="domcontentloaded")
         except Exception as e:
@@ -561,14 +567,17 @@
         Parameters:
         ----------
         pages (int): The number of pages to scroll down.
         """
         if pages < 1:
             return
 
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if self._stealth_mode_config is None:
             delta_y = 10000
             for _ in range(pages):
                 self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
                 time.sleep(0.1)
 
             time.sleep(1)
@@ -585,16 +594,14 @@
             for _ in range(pages):
                 self.scroll_to_top()
                 time.sleep(0.1)
 
     def _start_browser(
         self,
         user_auth_session=None,
-        headless=True,
-        proxy: ProxySettings = None,
     ):
         """Starts a new browser session and set storage state (if there is any).
 
         Parameters:
         ----------
         user_session_extras (optional): the JSON object that holds user session information
         headless (bool): Whether to start the browser in headless mode.
@@ -604,43 +611,45 @@
         args = [
             "--no-sandbox",
             "--disable-setuid-sandbox",
             "--disable-blink-features=AutomationControlled",
         ]
         self._playwright = sync_playwright().start()
         self._browser = self._playwright.chromium.launch(
-            headless=headless, proxy=proxy, args=args, ignore_default_args=ignored_args
+            headless=self._headless, proxy=self._proxy, args=args, ignore_default_args=ignored_args
         )
         self._current_tf_id = 0
         self._context = self._browser.new_context(
             user_agent=USER_AGENT,
             storage_state=user_auth_session,
         )
 
-    def _get_frame_context(self, iframe_path: str = None) -> Union[Frame, Page]:
+    def _get_frame_context(self, iframe_path: str = "") -> Union[FrameLocator, Page]:
         """
         Returns the frame context for the given iframe path.
 
         Parameters:
         ----------
         iframe_path (str): The path of the iframe within the frame.
 
         Returns:
         --------
         Frame | Page: The frame context for the given iframe path.
         """
+        if not self._current_page:
+            raise NoOpenPageError()
         if not iframe_path:
             return self._current_page
         iframe_path_list = iframe_path.split(".")
         frame_context = self._current_page
         for iframe_id in iframe_path_list:
             frame_context = frame_context.frame_locator(f"[tf623_id='{iframe_id}']")
         return frame_context
 
-    def find_element_by_id(self, tf623_id: str, iframe_path: str = None) -> Locator:
+    def _find_element_by_id(self, tf623_id: str, iframe_path: str = "") -> Locator:
         """
         Finds an element by its TF ID within a specified iframe.
 
         Parameters:
         ----------
         tf623_id (str): The generated tf id of the element to find.
         iframe_path (str): The path to the iframe containing the element.
@@ -661,14 +670,20 @@
 
     def _determine_load_state(
         self,
         monitor: PageActivityMonitor,
         timeout_seconds=14,
         wait_for_network_idle=True,
     ):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         start_time = time.time()
 
         while True:
             if wait_for_network_idle:
                 try:
                     last_updated_timestamp = self._current_page.evaluate(
                         load_js("get_last_dom_change")
@@ -687,14 +702,20 @@
                 if self._page_monitor.get_load_status():
                     break
             if time.time() - start_time > timeout_seconds:
                 break
             time.sleep(0.1)
 
     def _add_page_event_listeners(self):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         self._current_page.on("request", self._page_monitor.track_network_request)
         self._current_page.on("requestfinished", self._page_monitor.track_network_response)
         self._current_page.on("requestfailed", self._page_monitor.track_network_response)
         self._current_page.on("load", self._page_monitor.track_load)
 
         try:
             self._current_page.evaluate(load_js("add_dom_change_listener"))
@@ -703,14 +724,20 @@
             start_time = time.time()
             while True:
                 if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                     break
                 time.sleep(0.2)
 
     def _remove_page_event_listeners(self):
+        if not self._current_page:
+            raise NoOpenPageError()
+
+        if not self._page_monitor:
+            raise ValueError("Page monitor is not initialized.")
+
         self._current_page.remove_listener("request", self._page_monitor.track_network_request)
         self._current_page.remove_listener(
             "requestfinished", self._page_monitor.track_network_response
         )
         self._current_page.remove_listener(
             "requestfailed", self._page_monitor.track_network_response
         )
```

### Comparing `agentql-0.4.1/src/agentql/sync_api/_api.py` & `agentql-0.4.2/src/agentql/sync_api/_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import logging
 from typing import Any
 
 from playwright.sync_api import Locator, Page
 
+from agentql import trail_logger
 from agentql.ext.playwright import PlaywrightWebDriverSync as PlaywrightWebDriver
 
 from ._session import Session
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
@@ -20,39 +21,44 @@
 
 
 def start_session(
     url: str = "",
     *,
     web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightDriverTypeStub(),
     user_auth_session: Any = None,
+    enable_history_log: bool = False,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
     """Start a new synchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
     web_driver (webDriver) (optional): Web driver is responsible for interacting with the browser and page. Defaults to Playwright web driver, which is built on top of the [Playwright framework](https://playwright.dev/python/).
     user_auth_session (dict) (optional): The user authentication session that contains previous login session. Users could retrieve authentication session by starting a session, logging into desired website, and calling `session.get_user_auth_session()`, which will return a `auth_session` object defined in web driver.
+    enable_history_log (bool) (optional): Enable history log to record all the events during the session, retrieved via `session.get_last_trail()`.
 
     Returns:
     -------
     Session: An instance of AgentQL Session class for synchronous environment.
     """
+    if enable_history_log:
+        trail_logger.init()
     log.debug(f"Starting session with {url}")
 
     # this is a dirty hack to avoid instantiating PlaywrightWebDriver as a default value
     # which will be cached and reused across all sessions. This may cause problems when
     # start_session is called multiple times with default params. In this case driver will
     # be reused which is a problem since its stateful.
     if isinstance(web_driver, PlaywrightDriverTypeStub):
         web_driver = PlaywrightWebDriver()  # type: ignore
 
     try:
-        web_driver.start_browser(user_auth_session=user_auth_session)
+        # pylint: disable=protected-access
+        web_driver._start_browser(user_auth_session=user_auth_session)
         if url:
             web_driver.open_url(url)
         session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
     except Exception as e:
         log.error(f"Failed to start session: {e}")
-        web_driver.stop_browser()
+        web_driver._stop_browser()
         raise e
     return session
```

### Comparing `agentql-0.4.1/src/agentql/sync_api/_response_proxy.py` & `agentql-0.4.2/src/agentql/sync_api/_response_proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,75 @@
+# pylint: disable=protected-access
+
 import json
 import logging
 from typing import Generic, Union
 
-from agentql import AttributeNotFoundError, ContainerListNode, ContainerNode, IdListNode, IdNode
+from agentql import (
+    AttributeNotFoundError,
+    ContainerListNode,
+    ContainerNode,
+    IdListNode,
+    IdNode,
+    trail_logger,
+)
 
-from ._web_driver import InteractiveItemTypeT, WebDriver
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
 
 class AQLResponseProxy(Generic[InteractiveItemTypeT]):
     """
     AQLResponseProxy class acts as a dynamic proxy to the response received from AgentQL server. It allows users to interact with resulting web elements and to retrieve their text contents. This class is designed to work with the web driver to fetch and process query results.
     """
 
     def __init__(
         self,
-        data: dict,
-        web_driver: "WebDriver[InteractiveItemTypeT]",
+        data: Union[dict, list],
+        web_driver: "WebDriver[InteractiveItemTypeT, PageTypeT]",
         query_tree: ContainerNode,
     ):
         self._response_data = data
         self._web_driver = web_driver
         self._query_tree_node = query_tree
 
     def __getattr__(
         self, name
-    ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT]:
+    ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT, None]:
         if self._response_data is None:
             raise AttributeError("Response data is None")
         if name not in self._response_data:
             raise AttributeNotFoundError(name, self._response_data)
+        trail_logger.add_event(f"Resolving element {name} on {self._web_driver.current_url}")
         return self._resolve_item(
             self._response_data[name], self._query_tree_node.get_child_by_name(name)
         )
 
     def __getitem__(
         self, index: int
-    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]"]:
+    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if not isinstance(self._response_data, list):
             raise ValueError("This node is not a list")
         return self._resolve_item(self._response_data[index], self._query_tree_node)
 
     def _resolve_item(
         self, item, query_tree_node
-    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]"]:
+    ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if item is None:
             return None
 
         if isinstance(item, list):
             return AQLResponseProxy[InteractiveItemTypeT](item, self._web_driver, query_tree_node)
 
         if isinstance(query_tree_node, IdNode) or isinstance(query_tree_node, IdListNode):
-            return self._web_driver.locate_interactive_element(item)
+            interactive_element = self._web_driver._locate_interactive_element(item)
+            trail_logger.add_event(f"Resolved to {interactive_element}")
+
+            return interactive_element
 
         return AQLResponseProxy[InteractiveItemTypeT](item, self._web_driver, query_tree_node)
 
     def __len__(self):
         if self._response_data is None:
             return 0
         return len(self._response_data)
@@ -99,20 +112,20 @@
         return data_dict
 
     def _to_data_container_list_node(
         self, response_data: dict, query_tree_node: ContainerListNode
     ) -> list:
         return [self._to_data_container_node(item, query_tree_node) for item in response_data]
 
-    def _to_data_id_node(self, response_data: dict) -> dict:
+    def _to_data_id_node(self, response_data: dict) -> Union[dict, str, None]:
         if response_data is None:
             return None
         name = response_data.get("name")
         if not name or not name.strip():
-            web_element = self._web_driver.locate_interactive_element(response_data)
+            web_element = self._web_driver._locate_interactive_element(response_data)
             if not web_element:
                 log.warning(f"Could not locate web element for item {response_data}")
                 return None
             name = self._web_driver.get_text_content(web_element)
         return name
 
     def _to_data_id_list_node(self, response_data: list) -> list:
```

### Comparing `agentql-0.4.1/src/agentql/sync_api/_session.py` & `agentql-0.4.2/src/agentql/sync_api/_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+# pylint: disable=protected-access
+
 import copy
 import json
 import logging
 import os
-from typing import Callable, Generic, List, Literal, Optional
+from typing import Callable, Generic, List, Literal, Optional, Union
 
 import requests
 
 from agentql import (
     AgentQLServerError,
     AgentQLServerTimeoutError,
     APIKeyError,
     AttributeNotFoundError,
     QueryParser,
     UnableToClosePopupError,
+    trail_logger,
 )
 from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
+from agentql._core._utils import minify_query
 
 from ._popup import Popup
 from ._response_proxy import AQLResponseProxy
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
@@ -51,15 +55,15 @@
     def current_page(self) -> PageTypeT:
         """Get the current page being processed by AgentQL.
 
         Returns:
         -------
         PageTypeT: A type variable representing the type of a page in a web driver session. If you did not pass a customized web driver when starting the session, then it will return [Playwright Page](https://playwright.dev/python/docs/api/class-page) object.
         """
-        return self._web_driver.get_current_page()
+        return self._web_driver.current_page
 
     @property
     def driver(self) -> WebDriver[InteractiveItemTypeT, PageTypeT]:
         """Get the web driver.
 
         Returns:
         -------
@@ -73,22 +77,29 @@
         return self._last_query
 
     @property
     def last_response(self) -> Optional[dict]:
         """Get the last response."""
         return self._last_response
 
+    def get_last_trail(self) -> Union[trail_logger.TrailLogger, None]:
+        """
+        Get the last trail recorded, if enable_history_log is True when starting the session.
+        """
+        logger_store = trail_logger.TrailLoggerStore.get_loggers()
+        return logger_store[-1] if logger_store else None
+
     def get_user_auth_session(self):
         """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         User auth session in Python dictionary format.
         """
-        return self._web_driver.get_user_auth_session()
+        return self._web_driver._get_user_auth_session()
 
     def query(
         self,
         query: str,
         timeout: int = 500,
         lazy_load_pages_count: int = 0,
         wait_for_network_idle: bool = True,
@@ -103,23 +114,24 @@
         lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
         wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
 
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
+        trail_logger.add_event(f"Querying {minify_query(query)} on {self.current_page}")
         log.debug(f"querying {query}")
 
         self._last_query = query
         parser = QueryParser(query)
         query_tree = parser.parse()
 
         self._web_driver.wait_for_page_ready_state(wait_for_network_idle)
 
-        accessibility_tree = self._web_driver.prepare_accessibility_tree(
+        accessibility_tree = self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
         # Check if there is a popup in the page before sending the agentql query
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
@@ -127,26 +139,27 @@
 
         response = self._query(query, accessibility_tree, timeout)
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
-            accessibility_tree = self._web_driver.get_accessibility_tree()
+            accessibility_tree = self._web_driver.accessibility_tree
 
             popup_list = self._detect_popup(accessibility_tree, popup_list)
             if popup_list:
                 self._handle_popup(popup_list)
 
         return AQLResponseProxy[InteractiveItemTypeT](response, self._web_driver, query_tree)
 
     def stop(self):
         """Close the session."""
         log.debug("closing session")
-        self._web_driver.stop_browser()
+        self._web_driver._stop_browser()
+        trail_logger.finalize()
 
     def on(self, event: Literal["popup"], callback: Callable[[dict], None]):
         """Emitted when there is a popup (such as promotion window) on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections.
 
         Event Data:
         -----------
         popups (list): The list of popups captured on the page by AgentQL Popup Detection algorithm.
@@ -167,15 +180,15 @@
         timeout (int): The timeout value for the connection with backend api service
 
         Returns:
         -------
         dict: AgentQL response in json format.
         """
         try:
-            page_url = self._web_driver.get_current_url()
+            page_url = self._web_driver.current_url
             request_data = {
                 "query": f"{query}",
                 "accessibility_tree": accessibility_tree,
                 "metadata": {"url": page_url},
             }
             url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + GET_AGENTQL_ENDPOINT
             log.debug(f"Making request to {url}")
```

### Comparing `agentql-0.4.1/src/agentql/sync_api/_web_driver.py` & `agentql-0.4.2/src/agentql/sync_api/_web_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,134 @@
-from typing import Any
+from typing import Any, Optional
 
 from typing_extensions import Protocol
 
 from agentql.async_api import InteractiveItemTypeT, PageTypeT, ScrollDirection
 
 
 class WebDriver(Protocol[InteractiveItemTypeT, PageTypeT]):
-    def locate_interactive_element(self, response_data: dict) -> InteractiveItemTypeT:
-        """
-        Locates an interactive element in the web page.
-
-        Parameters:
-        -----------
-        response_data (dict): The data of the interactive element from the AgentQL response.
-
-        Returns:
-        --------
-        InteractiveItemTypeT: The interactive element.
-        """
-
-    def get_text_content(self, web_element: InteractiveItemTypeT) -> str:
+    def get_text_content(self, web_element: InteractiveItemTypeT) -> Optional[str]:
         """
         Gets the text content of the web element.
 
         Parameters:
         -----------
         web_element (InteractiveItemTypeT): The web element to get text from.
 
         Returns:
         --------
         str: The text content of the web element."""
 
-    def start_browser(self, user_auth_session: Any = None):
-        """Starts a new browser session and set user session state (if there is any).
-
-        Parameters:
-        -----------
-        user_auth_session (optional): The user authentication session that contains previous login session.
-        """
-
-    def stop_browser(self):
-        """Closes the current browser session."""
-
     def open_url(self, url: str, new_page: bool = False):
         """Open URL in the browser.
 
         Parameters:
         ----------
         url (str): The URL to open.
         new_page (bool): Whether to open the URL in a new page.
         """
 
-    def get_current_url(self) -> str:
-        """Get the URL of the current page being processed by AgentQL.
+    def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
+        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
 
-        Returns:
-        --------
-        str: The URL of the current page.
+        Parameters:
+        -----------
+        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
         """
 
-    def prepare_accessibility_tree(
-        self, lazy_load_pages_count: int, include_aria_hidden: bool
-    ) -> dict:
-        """Prepare the AT by modifing the dom. It will return the accessibility tree after preparation.
+    def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
+        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
-        lazy_load_pages_count: The number of times to scroll down and up the page.
-        include_aria_hidden: Whether to include elements with aria-hidden attribute in the AT.
+        -----------
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
+        pixels (int) (optional): The number of pixels to scroll. 720 by default.
+        """
+
+    def scroll_to_bottom(self):
+        """Scrolls to the bottom of the current page."""
+
+    def scroll_to_top(self):
+        """Scrolls to the top of the current page."""
+
+    @property
+    def current_url(self) -> str:
+        """Get the URL of the current page being processed by AgentQL.
 
         Returns:
         --------
-        dict: The accessibility tree of the page in Python Dict format.
+        str: The URL of the current page.
         """
 
-    def get_accessibility_tree(self) -> dict:
+    @property
+    def accessibility_tree(self) -> dict:
         """Returns the up-to-date accessibility tree of the page.
 
         Returns:
         --------
         dict: The accessibility tree of the page in Python Dict format.
         """
 
-    def get_user_auth_session(self) -> Any:
-        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+    @property
+    def html(self) -> Optional[str]:
+        """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page.".
 
         Returns:
         --------
-        The user session state.
+        dict: The HTML content of the web page.
         """
 
-    def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
-        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
+    @property
+    def current_page(self) -> PageTypeT:
+        """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
-        Parameters:
-        -----------
-        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
+        Returns:
+        --------
+        PageTypeT: The current page object.
         """
 
-    def get_html(self) -> dict:
-        """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page.".
+    def _get_user_auth_session(self) -> Any:
+        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
-        dict: The HTML content of the web page.
+        The user session state.
         """
 
-    def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
-        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
+    def _locate_interactive_element(self, response_data: dict) -> InteractiveItemTypeT:
+        """
+        Locates an interactive element in the web page.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
-        pixels (int) (optional): The number of pixels to scroll. 720 by default.
-        """
+        response_data (dict): The data of the interactive element from the AgentQL response.
 
-    def scroll_to_bottom(self):
-        """Scrolls to the bottom of the current page."""
+        Returns:
+        --------
+        InteractiveItemTypeT: The interactive element.
+        """
 
-    def scroll_to_top(self):
-        """Scrolls to the top of the current page."""
+    def _prepare_accessibility_tree(
+        self, lazy_load_pages_count: int, include_aria_hidden: bool
+    ) -> dict:
+        """Prepare the AT by modifing the dom. It will return the accessibility tree after preparation.
 
-    def get_current_page(self) -> PageTypeT:
-        """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
+        Parameters:
+        lazy_load_pages_count: The number of times to scroll down and up the page.
+        include_aria_hidden: Whether to include elements with aria-hidden attribute in the AT.
 
         Returns:
         --------
-        PageTypeT: The current page object.
+        dict: The accessibility tree of the page in Python Dict format.
+        """
+
+    def _start_browser(self, user_auth_session: Any = None):
+        """Starts a new browser session and set user session state (if there is any).
+
+        Parameters:
+        -----------
+        user_auth_session (optional): The user authentication session that contains previous login session.
         """
+
+    def _stop_browser(self):
+        """Closes the current browser session."""
```

### Comparing `agentql-0.4.1/PKG-INFO` & `agentql-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

