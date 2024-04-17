# Comparing `tmp/habluetooth-2.5.3.tar.gz` & `tmp/habluetooth-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habluetooth-2.5.3.tar", max compression
+gzip compressed data, was "habluetooth-2.6.0.tar", max compression
```

## Comparing `habluetooth-2.5.3.tar` & `habluetooth-2.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11345 2024-04-17 00:31:22.829009 habluetooth-2.5.3/LICENSE
--rw-r--r--   0        0        0     3805 2024-04-17 00:31:22.829009 habluetooth-2.5.3/README.md
--rw-r--r--   0        0        0     1496 2024-04-17 00:31:22.829009 habluetooth-2.5.3/build_ext.py
--rw-r--r--   0        0        0     3791 2024-04-17 00:31:24.129010 habluetooth-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     1457 2024-04-17 00:31:24.129010 habluetooth-2.5.3/src/habluetooth/__init__.py
--rw-r--r--   0        0        0      395 2024-04-17 00:31:22.829009 habluetooth-2.5.3/src/habluetooth/advertisement_tracker.pxd
--rw-r--r--   0        0        0     2809 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/advertisement_tracker.py
--rw-r--r--   0        0        0     1917 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/base_scanner.pxd
--rw-r--r--   0        0        0    16704 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/base_scanner.py
--rw-r--r--   0        0        0      650 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/central_manager.py
--rw-r--r--   0        0        0     1709 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/const.py
--rw-r--r--   0        0        0     2214 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/manager.pxd
--rw-r--r--   0        0        0    28056 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/manager.py
--rw-r--r--   0        0        0      726 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/models.pxd
--rw-r--r--   0        0        0     7310 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/models.py
--rw-r--r--   0        0        0        0 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/py.typed
--rw-r--r--   0        0        0      542 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/scanner.pxd
--rw-r--r--   0        0        0    18297 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/scanner.py
--rw-r--r--   0        0        0      530 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/scanner_device.py
--rw-r--r--   0        0        0     1733 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/usage.py
--rw-r--r--   0        0        0      544 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/util.py
--rw-r--r--   0        0        0    14651 2024-04-17 00:31:22.833009 habluetooth-2.5.3/src/habluetooth/wrappers.py
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 habluetooth-2.5.3/setup.py
--rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 habluetooth-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-17 00:59:35.387433 habluetooth-2.6.0/LICENSE
+-rw-r--r--   0        0        0     3805 2024-04-17 00:59:35.387433 habluetooth-2.6.0/README.md
+-rw-r--r--   0        0        0     1496 2024-04-17 00:59:35.387433 habluetooth-2.6.0/build_ext.py
+-rw-r--r--   0        0        0     3819 2024-04-17 00:59:36.147436 habluetooth-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1457 2024-04-17 00:59:36.147436 habluetooth-2.6.0/src/habluetooth/__init__.py
+-rw-r--r--   0        0        0      395 2024-04-17 00:59:35.387433 habluetooth-2.6.0/src/habluetooth/advertisement_tracker.pxd
+-rw-r--r--   0        0        0     2809 2024-04-17 00:59:35.387433 habluetooth-2.6.0/src/habluetooth/advertisement_tracker.py
+-rw-r--r--   0        0        0     1917 2024-04-17 00:59:35.387433 habluetooth-2.6.0/src/habluetooth/base_scanner.pxd
+-rw-r--r--   0        0        0    16704 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/base_scanner.py
+-rw-r--r--   0        0        0      650 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/central_manager.py
+-rw-r--r--   0        0        0     1709 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/const.py
+-rw-r--r--   0        0        0     2214 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/manager.pxd
+-rw-r--r--   0        0        0    28056 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/manager.py
+-rw-r--r--   0        0        0      726 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/models.pxd
+-rw-r--r--   0        0        0     7310 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/models.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/py.typed
+-rw-r--r--   0        0        0      579 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/scanner.pxd
+-rw-r--r--   0        0        0    19420 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/scanner.py
+-rw-r--r--   0        0        0      530 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/scanner_device.py
+-rw-r--r--   0        0        0     1733 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/usage.py
+-rw-r--r--   0        0        0      544 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/util.py
+-rw-r--r--   0        0        0    14651 2024-04-17 00:59:35.391433 habluetooth-2.6.0/src/habluetooth/wrappers.py
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 habluetooth-2.6.0/setup.py
+-rw-r--r--   0        0        0     5133 1970-01-01 00:00:00.000000 habluetooth-2.6.0/PKG-INFO
```

### Comparing `habluetooth-2.5.3/LICENSE` & `habluetooth-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/README.md` & `habluetooth-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/build_ext.py` & `habluetooth-2.6.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/pyproject.toml` & `habluetooth-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habluetooth"
-version = "2.5.3"
+version = "2.6.0"
 description = "High availability Bluetooth"
 authors = ["J. Nick Koston <bluetooth@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/habluetooth"
 documentation = "https://habluetooth.readthedocs.io"
 classifiers = [
@@ -29,14 +29,15 @@
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 bleak = ">=0.21.1"
 bleak-retry-connector = ">=3.3.0"
 bluetooth-data-tools = ">=1.16.0"
 bluetooth-adapters = ">=0.16.1"
 bluetooth-auto-recovery = ">=1.2.3"
+async-interrupt = ">=1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 pytest-asyncio = "^0.23.6"
 
 [tool.poetry.group.docs]
```

### Comparing `habluetooth-2.5.3/src/habluetooth/__init__.py` & `habluetooth-2.6.0/src/habluetooth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.5.3"
+__version__ = "2.6.0"
 
 from .advertisement_tracker import (
     TRACKER_BUFFERING_WOBBLE_SECONDS,
     AdvertisementTracker,
 )
 from .base_scanner import BaseHaRemoteScanner, BaseHaScanner
 from .central_manager import get_manager, set_manager
```

### Comparing `habluetooth-2.5.3/src/habluetooth/advertisement_tracker.py` & `habluetooth-2.6.0/src/habluetooth/advertisement_tracker.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/base_scanner.pxd` & `habluetooth-2.6.0/src/habluetooth/base_scanner.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/base_scanner.py` & `habluetooth-2.6.0/src/habluetooth/base_scanner.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/central_manager.py` & `habluetooth-2.6.0/src/habluetooth/central_manager.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/const.py` & `habluetooth-2.6.0/src/habluetooth/const.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/manager.pxd` & `habluetooth-2.6.0/src/habluetooth/manager.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/manager.py` & `habluetooth-2.6.0/src/habluetooth/manager.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/models.pxd` & `habluetooth-2.6.0/src/habluetooth/models.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/models.py` & `habluetooth-2.6.0/src/habluetooth/models.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/scanner.pxd` & `habluetooth-2.6.0/src/habluetooth/scanner.pxd`

 * *Files 9% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 cdef class HaScanner(BaseHaScanner):
 
     cdef public object mac_address
     cdef public object mode
     cdef public object _start_stop_lock
     cdef public object _background_tasks
     cdef public object scanner
+    cdef public object _start_future
 
     cpdef void _async_detection_callback(
         self,
         object device,
         object advertisement_data
     )
```

### Comparing `habluetooth-2.5.3/src/habluetooth/scanner.py` & `habluetooth-2.6.0/src/habluetooth/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import platform
 from typing import Any, Coroutine, Iterable
 
+import async_interrupt
 import bleak
 from bleak import BleakError
 from bleak.assigned_numbers import AdvertisementDataType
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData, AdvertisementDataCallback
 from bleak_retry_connector import restore_discoveries
 from bluetooth_adapters import DEFAULT_ADDRESS
@@ -79,14 +80,18 @@
 # without success when the first time the watch
 # dog hit the failure path.
 SCANNER_WATCHDOG_MULTIPLE = (
     SCANNER_WATCHDOG_TIMEOUT + SCANNER_WATCHDOG_INTERVAL.total_seconds()
 )
 
 
+class _AbortStartError(Exception):
+    """Error to indicate that the start should be aborted."""
+
+
 class ScannerStartError(Exception):
     """Error to indicate that the scanner failed to start."""
 
 
 def create_bleak_scanner(
     detection_callback: AdvertisementDataCallback,
     scanning_mode: BluetoothScanningMode,
@@ -152,14 +157,15 @@
         super().__init__(source, adapter)
         self.connectable = True
         self.mode = mode
         self._start_stop_lock = asyncio.Lock()
         self.scanning = False
         self._background_tasks: set[asyncio.Task[Any]] = set()
         self.scanner: bleak.BleakScanner | None = None
+        self._start_future: asyncio.Future[None] | None = None
 
     def _create_background_task(self, coro: Coroutine[Any, Any, None]) -> None:
         """Create a background task and add it to the background tasks set."""
         task = asyncio.create_task(coro)
         self._background_tasks.add(task)
         task.add_done_callback(self._background_tasks.discard)
 
@@ -260,14 +266,18 @@
         """Run when the scanner has successfully started."""
         self.scanning = True
         self._async_setup_scanner_watchdog()
         await restore_discoveries(self.scanner, self.adapter)
 
     async def _async_start_attempt(self, attempt: int) -> bool:
         """Start the scanner and handle errors."""
+        assert (  # noqa: S101
+            self._loop is not None
+        ), "Loop is not set, call async_setup first"
+
         mode = self.mode
         # 1st attempt - no auto reset
         # 2nd attempt - try to reset the adapter and wait a bit
         # 3th attempt - no auto reset
         # 4th attempt - fallback to passive if available
 
         if (
@@ -284,17 +294,23 @@
                 START_ATTEMPTS,
             )
 
         self.scanner = create_bleak_scanner(
             self._async_detection_callback, mode, self.adapter
         )
         self._log_start_attempt(attempt)
+        self._start_future = self._loop.create_future()
         try:
-            async with asyncio.timeout(START_TIMEOUT):
+            async with asyncio.timeout(START_TIMEOUT), async_interrupt.interrupt(
+                self._start_future, _AbortStartError, None
+            ):
                 await self.scanner.start()
+        except _AbortStartError as ex:
+            await self._async_stop_scanner()
+            self._raise_for_abort_start(ex)
         except InvalidMessageError as ex:
             await self._async_stop_scanner()
             self._raise_for_invalid_dbus_message(ex)
         except BrokenPipeError as ex:
             await self._async_stop_scanner()
             self._raise_for_broken_pipe_error(ex)
         except FileNotFoundError as ex:
@@ -331,14 +347,16 @@
             raise ScannerStartError(
                 f"{self.name}: Failed to start Bluetooth: {ex}; "
                 "Try power cycling the Bluetooth hardware."
             ) from ex
         except BaseException:
             await self._async_stop_scanner()
             raise
+        finally:
+            self._start_future = None
 
         self._log_start_success(attempt)
         return True
 
     def _log_adapter_init_wait(self, attempt: int) -> None:
         _LOGGER.debug(
             "%s: Waiting for adapter to initialize; attempt (%s/%s)",
@@ -377,14 +395,24 @@
         _LOGGER.debug(
             "%s: Starting bluetooth discovery attempt: (%s/%s)",
             self.name,
             attempt,
             START_ATTEMPTS,
         )
 
+    def _raise_for_abort_start(self, ex: _AbortStartError) -> None:
+        _LOGGER.debug(
+            "%s: Starting bluetooth scanner aborted: %s",
+            self.name,
+            ex,
+            exc_info=True,
+        )
+        msg = f"{self.name}: Starting bluetooth scanner aborted"
+        raise ScannerStartError(msg) from ex
+
     def _raise_for_file_not_found_error(self, ex: FileNotFoundError) -> None:
         _LOGGER.debug(
             "%s: FileNotFoundError while starting bluetooth: %s",
             self.name,
             ex,
             exc_info=True,
         )
@@ -478,14 +506,16 @@
         # strategy, we will change this to raise a repair issue as well.
         _LOGGER.debug("%s: adapter stopped responding; executing reset", self.name)
         result = await async_reset_adapter(self.adapter, self.mac_address)
         _LOGGER.debug("%s: adapter reset result: %s", self.name, result)
 
     async def async_stop(self) -> None:
         """Stop bluetooth scanner."""
+        if self._start_future is not None and not self._start_future.done():
+            self._start_future.set_exception(_AbortStartError())
         async with self._start_stop_lock:
             self._async_stop_scanner_watchdog()
             await self._async_stop_scanner()
 
     async def _async_stop_scanner(self) -> None:
         """Stop bluetooth discovery under the lock."""
         self.scanning = False
```

### Comparing `habluetooth-2.5.3/src/habluetooth/scanner_device.py` & `habluetooth-2.6.0/src/habluetooth/scanner_device.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/usage.py` & `habluetooth-2.6.0/src/habluetooth/usage.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/util.py` & `habluetooth-2.6.0/src/habluetooth/util.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/src/habluetooth/wrappers.py` & `habluetooth-2.6.0/src/habluetooth/wrappers.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.5.3/setup.py` & `habluetooth-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 packages = \
 ['habluetooth']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bleak-retry-connector>=3.3.0',
+['async-interrupt>=1.1.1',
+ 'bleak-retry-connector>=3.3.0',
  'bleak>=0.21.1',
  'bluetooth-adapters>=0.16.1',
  'bluetooth-auto-recovery>=1.2.3',
  'bluetooth-data-tools>=1.16.0']
 
 setup_kwargs = {
     'name': 'habluetooth',
-    'version': '2.5.3',
+    'version': '2.6.0',
     'description': 'High availability Bluetooth',
     'long_description': '# habluetooth\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/habluetooth/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bluetooth-devices/habluetooth/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://habluetooth.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/habluetooth.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/habluetooth">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/habluetooth.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/habluetooth/">\n    <img src="https://img.shields.io/pypi/v/habluetooth.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/habluetooth.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/habluetooth.svg?style=flat-square" alt="License">\n</p>\n\n---\n\n**Documentation**: <a href="https://habluetooth.readthedocs.io" target="_blank">https://habluetooth.readthedocs.io </a>\n\n**Source Code**: <a href="https://github.com/bluetooth-devices/habluetooth" target="_blank">https://github.com/bluetooth-devices/habluetooth </a>\n\n---\n\nHigh availability Bluetooth\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install habluetooth`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/habluetooth',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['habluetooth'] package_data = \ {'': ['*']}
-install_requires = \ ['bleak-retry-connector>=3.3.0', 'bleak>=0.21.1',
-'bluetooth-adapters>=0.16.1', 'bluetooth-auto-recovery>=1.2.3', 'bluetooth-
-data-tools>=1.16.0'] setup_kwargs = { 'name': 'habluetooth', 'version':
-'2.5.3', 'description': 'High availability Bluetooth', 'long_description': '#
-habluetooth\n\n
+install_requires = \ ['async-interrupt>=1.1.1', 'bleak-retry-connector>=3.3.0',
+'bleak>=0.21.1', 'bluetooth-adapters>=0.16.1', 'bluetooth-auto-
+recovery>=1.2.3', 'bluetooth-data-tools>=1.16.0'] setup_kwargs = { 'name':
+'habluetooth', 'version': '2.6.0', 'description': 'High availability
+Bluetooth', 'long_description': '# habluetooth\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
 \n\n---\n\n**Documentation**: _h_t_t_p_s_:_/_/_h_a_b_l_u_e_t_o_o_t_h_._r_e_a_d_t_h_e_d_o_c_s_._i_o_ \n\n**Source
```

### Comparing `habluetooth-2.5.3/PKG-INFO` & `habluetooth-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habluetooth
-Version: 2.5.3
+Version: 2.6.0
 Summary: High availability Bluetooth
 Home-page: https://github.com/bluetooth-devices/habluetooth
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: bluetooth@koston.org
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: async-interrupt (>=1.1.1)
 Requires-Dist: bleak (>=0.21.1)
 Requires-Dist: bleak-retry-connector (>=3.3.0)
 Requires-Dist: bluetooth-adapters (>=0.16.1)
 Requires-Dist: bluetooth-auto-recovery (>=1.2.3)
 Requires-Dist: bluetooth-data-tools (>=1.16.0)
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/habluetooth/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/habluetooth/blob/main/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: habluetooth Version: 2.5.3 Summary: High
+Metadata-Version: 2.1 Name: habluetooth Version: 2.6.0 Summary: High
 availability Bluetooth Home-page: https://github.com/bluetooth-devices/
 habluetooth License: Apache Software License 2.0 Author: J. Nick Koston Author-
 email: bluetooth@koston.org Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
-Software Development :: Libraries Requires-Dist: bleak (>=0.21.1) Requires-
-Dist: bleak-retry-connector (>=3.3.0) Requires-Dist: bluetooth-adapters
-(>=0.16.1) Requires-Dist: bluetooth-auto-recovery (>=1.2.3) Requires-Dist:
-bluetooth-data-tools (>=1.16.0) Project-URL: Bug Tracker, https://github.com/
-bluetooth-devices/habluetooth/issues Project-URL: Changelog, https://
-github.com/bluetooth-devices/habluetooth/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://habluetooth.readthedocs.io Project-URL: Repository,
-https://github.com/bluetooth-devices/habluetooth Description-Content-Type:
-text/markdown # habluetooth
+Software Development :: Libraries Requires-Dist: async-interrupt (>=1.1.1)
+Requires-Dist: bleak (>=0.21.1) Requires-Dist: bleak-retry-connector (>=3.3.0)
+Requires-Dist: bluetooth-adapters (>=0.16.1) Requires-Dist: bluetooth-auto-
+recovery (>=1.2.3) Requires-Dist: bluetooth-data-tools (>=1.16.0) Project-URL:
+Bug Tracker, https://github.com/bluetooth-devices/habluetooth/issues Project-
+URL: Changelog, https://github.com/bluetooth-devices/habluetooth/blob/main/
+CHANGELOG.md Project-URL: Documentation, https://habluetooth.readthedocs.io
+Project-URL: Repository, https://github.com/bluetooth-devices/habluetooth
+Description-Content-Type: text/markdown # habluetooth
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Documentation**: _h_t_t_p_s_:_/_/_h_a_b_l_u_e_t_o_o_t_h_._r_e_a_d_t_h_e_d_o_c_s_._i_o_ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_l_u_e_t_o_o_t_h_-_d_e_v_i_c_e_s_/_h_a_b_l_u_e_t_o_o_t_h_ --- High availability
 Bluetooth ## Installation Install this via pip (or your favourite package
 manager): `pip install habluetooth` ## Contributors â¨ Thanks goes to these
```

