# Comparing `tmp/lunar-interceptor-0.3.2.tar.gz` & `tmp/lunar_interceptor-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunar-interceptor-0.3.2.tar", last modified: Wed Feb 21 08:02:55 2024, max compression
+gzip compressed data, was "lunar_interceptor-0.3.3.tar", last modified: Wed Apr 17 11:43:27 2024, max compression
```

## Comparing `lunar-interceptor-0.3.2.tar` & `lunar_interceptor-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    48047 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.736778 lunar-interceptor-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.736778 lunar-interceptor-0.3.2/src/lunar_interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/fail_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/src/lunar_interceptor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-21 08:02:55.000000 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-21 08:02:55.000000 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:02:55.000000 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-21 08:02:55.000000 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-21 08:02:55.000000 lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:02:55.740778 lunar-interceptor-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/test/fail_safe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/test/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/test/interceptor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-02-21 08:02:37.000000 lunar-interceptor-0.3.2/test/traffic_filter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    48047 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.399835 lunar_interceptor-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.403835 lunar_interceptor-0.3.3/src/lunar_interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.403835 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/fail_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/fail_safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/interceptor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/traffic_filter_test.py
```

### Comparing `lunar-interceptor-0.3.2/Pipfile.lock` & `lunar_interceptor-0.3.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/__init__.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import logging
 import platform
 
 from lunar_interceptor.interceptor import (
     Interceptor,
     InterceptorConfig,
+    get_interceptor_config,
     ENV_LUNAR_PROXY_HOST_KEY,
 )
+from lunar_interceptor.interceptor.helpers import load_env_value
 from lunar_interceptor.interceptor.traffic_filter import TrafficFilter
 from lunar_interceptor.interceptor.fail_safe import (
     FailSafe,
     ProxyErrorException,
 )
 
 _INTERCEPTOR_NAME = "lunar-interceptor"
-interceptor_config = InterceptorConfig()
+_ENV_LUNAR_INTERCEPTOR_LOG_LEVEL = "LUNAR_INTERCEPTOR_LOG_LEVEL"
 
 
 def _initialize_lunar_logger() -> logging.Logger:
     log_format = logging.Formatter(
         f"%(asctime)s - {_INTERCEPTOR_NAME} - %(levelname)s: %(message)s"
     )
-    log_level = interceptor_config.log_level
+    log_level = load_env_value(_ENV_LUNAR_INTERCEPTOR_LOG_LEVEL, str, "INFO")
 
     logger = logging.getLogger(name=_INTERCEPTOR_NAME)
     logger.setLevel(log_level)
 
     stream_handler = logging.StreamHandler()
     stream_handler.setLevel(log_level)
     stream_handler.setFormatter(log_format)
     logger.addHandler(stream_handler)
 
     return logger
 
 
 _LOGGER = _initialize_lunar_logger()
+interceptor_config: InterceptorConfig = get_interceptor_config(_LOGGER)
 
 
 def _load_fail_safe() -> FailSafe:
     fail_safe = FailSafe(
         cooldown_time=interceptor_config.fail_safe_config.cooldown_time,
         max_errors_allowed=interceptor_config.fail_safe_config.max_errors,
         logger=_LOGGER,
@@ -53,24 +56,20 @@
         interceptor_config.traffic_filter.allow_list,
         _LOGGER,
     )
 
 
 def _initialize_hooks():
     lunar_interceptor = Interceptor(
-        lunar_proxy_host=interceptor_config.connection_config.proxy_host,
-        lunar_tenant_id=interceptor_config.connection_config.tenant_id,
-        lunar_handshake_port=interceptor_config.connection_config.handshake_port,
-        proxy_support_tls=interceptor_config.connection_config.tls_supported == 1,
+        lunar_proxy_configuration=interceptor_config.connection_config,
         fail_safe=_load_fail_safe(),
         traffic_filter=_build_traffic_filter_from_env_vars(),
         logger=_LOGGER,
     )
     lunar_interceptor.set_hooks()
-    _LOGGER.debug(f"Lunar Interceptor is ENABLED!")
 
 
 if _LOGGER.isEnabledFor(logging.DEBUG):
     _LOGGER.debug(
         "Lunar Interceptor has loaded in debug mode."
         "The current configuration are"
         f"  * Interceptor Version: {interceptor_config.version}"
```

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/fail_safe.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/fail_safe.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/helpers.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/helpers.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/aiohttp.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/aiohttp.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, List, Dict, Optional
 
 from lunar_interceptor.interceptor.hooks.const import *
 from lunar_interceptor.interceptor.hooks.helpers import *
 from lunar_interceptor.interceptor.fail_safe import FailSafe
 from lunar_interceptor.interceptor.hooks.hook import LunarHook
 from lunar_interceptor.interceptor.traffic_filter import TrafficFilter
+from lunar_interceptor.interceptor.configuration import ConnectionConfig
 
 _hook = True
 
 try:
     import aiohttp
     from aiohttp.typedefs import StrOrURL
     from aiohttp.client_exceptions import (
@@ -23,45 +24,45 @@
 except ImportError:
     _hook = False
 
 
 class AioHttpHook(LunarHook):
     def __init__(
         self,
-        scheme: str,
-        lunar_proxy: str,
-        lunar_tenant_id: str,
         logger: logging.Logger,
         fail_safe: FailSafe,
         traffic_filter: TrafficFilter,
+        lunar_proxy_configuration: ConnectionConfig,
     ) -> None:
-        self._scheme = scheme
-        self._lunar_tenant_id: str = lunar_tenant_id
-        self._lunar_proxy = lunar_proxy
+        self._connection_config = lunar_proxy_configuration
         self._logger = logger
         self._traffic_filter = traffic_filter
         self._fail_safe = fail_safe
         self._original_function = aiohttp.client.ClientSession._request  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
 
-        # fmt: off
-        aiohttp.client.ClientSession._request = self._hook_module()  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
-        # fmt: on
-
         self._fail_safe.handle_on(
             (
                 ClientConnectionError,  # type: ignore [reportOptionalCall, reportUnboundVariable]
                 ClientConnectorError,  # type: ignore [reportOptionalCall, reportUnboundVariable]
                 ClientSSLError,  # type: ignore [reportOptionalCall, reportUnboundVariable]
             )
         )
 
     @staticmethod
     def is_hook_supported() -> bool:
         return _hook
 
+    def init_hooks(self) -> None:
+        self._logger.debug("Initializing AioHttp Hook")
+        aiohttp.client.ClientSession._request = self._hook_module()  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
+
+    def remove_hooks(self) -> None:
+        self._logger.debug("Removing AioHttp Hook")
+        aiohttp.client.ClientSession._request = self._original_function  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
+
     async def make_connection(
         self, url: str, headers: Optional[Dict[str, str]]
     ) -> bool:
         try:
             async with aiohttp.ClientSession() as validate_session:  # type: ignore [reportUnboundVariable]
                 async with validate_session.get(
                     url,
@@ -127,23 +128,25 @@
         *args: List[Any],
         **kwargs: Dict[str, Any],
     ) -> "aiohttp.client.ClientResponse":
         manipulated_headers = generate_modified_headers(
             original_url=url_object,
             original_headers=original_headers,
             sequence_id=sequence_id,
-            lunar_tenant_id=self._lunar_tenant_id,
+            lunar_tenant_id=self._connection_config.tenant_id,
             traffic_filter=self._traffic_filter,
         )
 
         response = await self._original_function(  # type: ignore [reportOptionalCall]
             self=client_session,
             method=method,
             str_or_url=generate_modified_url(
-                self._scheme, self._lunar_proxy, url_object
+                self._connection_config.proxy_scheme,
+                self._connection_config.proxy_host_with_port,
+                url_object,
             ),
             headers=manipulated_headers,
             *args,
             **kwargs,
         )
 
         self._fail_safe.validate_headers(response.headers)
```

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/const.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/const.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/helpers.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/helpers.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/hooks/requests.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,54 +4,55 @@
 from typing import Any, List, Dict, Optional
 
 from lunar_interceptor.interceptor.hooks.const import *
 from lunar_interceptor.interceptor.hooks.helpers import *
 from lunar_interceptor.interceptor.fail_safe import FailSafe
 from lunar_interceptor.interceptor.hooks.hook import LunarHook
 from lunar_interceptor.interceptor.traffic_filter import TrafficFilter
+from lunar_interceptor.interceptor.configuration import ConnectionConfig
 
 _hook = True
 
 try:
     import requests  # type: ignore [reportMissingModuleSource]
 
 except ImportError:
     _hook = False
 
 
 class RequestsHook(LunarHook):
     def __init__(
         self,
-        scheme: str,
-        lunar_proxy: str,
-        lunar_tenant_id: str,
         logger: logging.Logger,
         fail_safe: FailSafe,
         traffic_filter: TrafficFilter,
+        lunar_proxy_configuration: ConnectionConfig,
     ) -> None:
-        self._scheme = scheme
-        self._lunar_tenant_id: str = lunar_tenant_id
-        self._lunar_proxy = lunar_proxy
+        self._connection_config = lunar_proxy_configuration
         self._logger = logger
         self._traffic_filter = traffic_filter
         self._fail_safe = fail_safe
         self._original_function = requests.Session.request  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
 
-        # fmt: off
-        requests.Session.request = self._hook_module()  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
-        # fmt: on
-
         self._fail_safe.handle_on(
             (requests.ConnectionError,)  # type: ignore [reportOptionalCall]
         )
 
     @staticmethod
     def is_hook_supported() -> bool:
         return _hook
 
+    def init_hooks(self) -> None:
+        self._logger.debug("Initializing Requests Hook")
+        requests.Session.request = self._hook_module()  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
+
+    def remove_hooks(self) -> None:
+        self._logger.debug("Removing Requests Hook")
+        requests.Session.request = self._original_function  # type: ignore [reportPrivateUsage, reportUnknownMemberType]
+
     async def make_connection(
         self, url: str, headers: Optional[Dict[str, str]]
     ) -> bool:
         try:
             response = requests.get(url, headers=headers)  # type: ignore [reportUnboundVariable]
 
             if response.status_code == 200:
@@ -107,19 +108,23 @@
         *args: List[Any],
         **kwargs: Dict[str, Any],
     ) -> "requests.Response":
         manipulated_headers = generate_modified_headers(
             original_url=url_object,
             original_headers=original_headers,
             sequence_id=sequence_id,
-            lunar_tenant_id=self._lunar_tenant_id,
+            lunar_tenant_id=self._connection_config.tenant_id,
             traffic_filter=self._traffic_filter,
         )
         modified_url = str(
-            generate_modified_url(self._scheme, self._lunar_proxy, url_object)
+            generate_modified_url(
+                self._connection_config.proxy_scheme,
+                self._connection_config.proxy_host_with_port,
+                url_object,
+            ),
         )
         self._logger.debug(
             f"Forwarding the request to {modified_url} using Lunar Proxy"
         )
         response = self._original_function(
             self=client_session,
             method=method,
```

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/interceptor.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/interceptor.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from lunar_interceptor.interceptor.hooks.const import *
 from lunar_interceptor.interceptor.hooks import LUNAR_HOOKS
 from lunar_interceptor.interceptor.fail_safe import FailSafe
 from lunar_interceptor.interceptor.singleton import Singleton
 from lunar_interceptor.interceptor.hooks.hook import LunarHook
 from lunar_interceptor.interceptor.traffic_filter import TrafficFilter
+from lunar_interceptor.interceptor.configuration import ConnectionConfig
 
 
 class Interceptor(metaclass=Singleton):
     """
     This is the logic that allow the framework to forward the HTTP/S requests through Lunar Proxy.
 
     Args:
@@ -22,42 +23,34 @@
         fail_safe (FailSafe): The FailSafe module.
         traffic_filter (TrafficFilter): The TrafficFilter module.
         logger (logging.Logger): Logger.
     """
 
     def __init__(
         self,
-        lunar_proxy_host: str,
-        lunar_tenant_id: str,
-        lunar_handshake_port: str,
-        proxy_support_tls: bool,
+        lunar_proxy_configuration: ConnectionConfig,
         fail_safe: FailSafe,
         traffic_filter: TrafficFilter,
         logger: logging.Logger,
     ):
-        self._proxy_scheme = HTTPS_SCHEME if proxy_support_tls else HTTP_SCHEME
-        self._lunar_proxy: str = lunar_proxy_host
-        self._lunar_tenant_id: str = lunar_tenant_id
-        self._lunar_proxy_handshake_port: str = lunar_handshake_port
+        self._connection_config = lunar_proxy_configuration
         self._traffic_filter = traffic_filter
         self._fail_safe = fail_safe
         self._logger = logger
         self._lunar_hooks: List[LunarHook] = []
 
     def set_hooks(self) -> None:
         """
         Initialize the required hooks to the AioHttp framework in order to allow traffic to be forwarded through Lunar Proxy.
         """
         for module in LUNAR_HOOKS:
             if module.is_hook_supported():
                 self._lunar_hooks.append(
                     module(
-                        scheme=self._proxy_scheme,
-                        lunar_proxy=self._lunar_proxy,
-                        lunar_tenant_id=self._lunar_tenant_id,
+                        lunar_proxy_configuration=self._connection_config,
                         logger=self._logger,
                         fail_safe=self._fail_safe,
                         traffic_filter=self._traffic_filter,
                     )
                 )
 
         self._logger.debug("Python Interceptor is loaded...")
@@ -67,35 +60,38 @@
         )
 
     async def _validate_lunar_proxy_connection(self) -> None:
         """
         Checks the communication to Lunar Proxy.
         """
 
-        proxy_handshake_host = (
-            f"{self._lunar_proxy.split(':')[0]}:{self._lunar_proxy_handshake_port}"
-        )
-        headers = {X_LUNAR_TENANT_ID_HEADER_KEY: self._lunar_tenant_id}
-        proxy_handshake_host = (
-            f"{self._proxy_scheme}://{proxy_handshake_host}/handshake"
-        )
+        headers = {X_LUNAR_TENANT_ID_HEADER_KEY: self._connection_config.tenant_id}
+        proxy_handshake_host = f"{self._connection_config.proxy_scheme}://{self._connection_config.proxy_host}:{self._connection_config.handshake_port}/handshake"
 
         if not self._lunar_hooks:
             return
 
         self._logger.debug("Establishing handshake with Lunar Proxy...")
 
         res = await self._lunar_hooks[0].make_connection(
             url=proxy_handshake_host, headers=headers
         )
 
-        if res:
-            self._logger.debug(f"[ⓥ] Successfully communicate with Lunar Proxy")
-
-        else:
+        if not res:
             self._logger.warning(
-                f"[ⓧ] Failed to communicate with Lunar Proxy,"
-                f" please make sure that Lunar Proxy is running and port '{self._lunar_proxy_handshake_port}'"
-                f" is set as the health-check port.\n"
+                f"[ⓧ] Failed to communicate with Lunar Proxy.\n"
+                f" Lunar Interceptor is disabled.\n"
+                f" please make sure that Lunar Proxy is running and port '{self._connection_config.handshake_port}'"
+                f" is set as the handshake port.\n"
                 f" For more information please refer to:"
                 f" http://docs.lunar.dev/installation-configuration/configuration#lunar-interceptor-configuration"
             )
+            return
+
+        print(res)
+        for hook in self._lunar_hooks:
+            hook.init_hooks()
+
+        self._logger.info(
+            "[ⓥ] Successfully communicate with Lunar Proxy"
+            "Lunar Interceptor is ENABLED!"
+        )
```

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor/interceptor/traffic_filter.py` & `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/traffic_filter.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/src/lunar_interceptor.egg-info/SOURCES.txt` & `lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/test/fail_safe_test.py` & `lunar_interceptor-0.3.3/test/fail_safe_test.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/test/interceptor_test.py` & `lunar_interceptor-0.3.3/test/interceptor_test.py`

 * *Files identical despite different names*

### Comparing `lunar-interceptor-0.3.2/test/traffic_filter_test.py` & `lunar_interceptor-0.3.3/test/traffic_filter_test.py`

 * *Files identical despite different names*

