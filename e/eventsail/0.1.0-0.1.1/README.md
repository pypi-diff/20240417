# Comparing `tmp/eventsail-0.1.0.tar.gz` & `tmp/eventsail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventsail-0.1.0.tar", max compression
+gzip compressed data, was "eventsail-0.1.1.tar", max compression
```

## Comparing `eventsail-0.1.0.tar` & `eventsail-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3159 2024-04-08 14:37:31.048285 eventsail-0.1.0/README.md
--rw-r--r--   0        0        0     8439 2024-04-08 14:37:31.052285 eventsail-0.1.0/eventsail.py
--rw-r--r--   0        0        0     1474 2024-04-08 14:37:31.052285 eventsail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 eventsail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4025 2024-04-17 06:40:50.105695 eventsail-0.1.1/README.md
+-rw-r--r--   0        0        0    10460 2024-04-17 06:40:50.105695 eventsail-0.1.1/eventsail.py
+-rw-r--r--   0        0        0     1473 2024-04-17 06:40:50.105695 eventsail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5393 1970-01-01 00:00:00.000000 eventsail-0.1.1/PKG-INFO
```

### Comparing `eventsail-0.1.0/README.md` & `eventsail-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # EventSail
 
-[![codecov](https://codecov.io/gh/satyamsoni2211/eventsail/graph/badge.svg?token=1LW83DYL0R)](https://codecov.io/gh/satyamsoni2211/eventsail)
+[![codecov](https://codecov.io/gh/satyamsoni2211/eventsail/graph/badge.svg?token=AWAXXSH30S)](https://codecov.io/gh/satyamsoni2211/eventsail)
 
 EventSail is a minimal observer pattern package which is performant as well as supports both sync and async operations. Born out of utility and curiosity to replicate Javascript `EventEmitter`, here we are with library with similar functionalities.
 
+![codecov graph](https://codecov.io/gh/satyamsoni2211/eventsail/graphs/sunburst.svg?token=AWAXXSH30S)
+
 ## Usage
 
 ### Installation
 
 Package can be installed from `PyPi` using below command.
 
 ```bash
@@ -87,14 +89,29 @@
 
 ```python
 test_event.clear()
 ```
 
 `Event` class is also singleton class, so you will always get same instance for same set of arguments. This is intentionally kept in place so that we do not loose listeners subscribed.
 
+### Waiting for async tasks
+
+There can be instances where we would need to wait for async emitted tasks to complete before shutdown as this can be critical. `Event` class exposes certain properties containing `async` tasks.
+
+- `Event.all_async_tasks` : This will return all the async tasks scheduled over Event loop for the Emitter.
+- `Event.own_async_tasks` : This will only return async tasks corresponding to the immediate parent Emitter of the Event.
+
+To wait for async tasks to complete, `Event` class exposes awaitable API to wait for tasks to complete. This can be called as below.
+
+```python
+await test_event.wait_for_async_tasks()
+```
+
+This will wait for all the async tasks. This also has a default timeout for 10 seconds post which it will error out.
+
 ## Testing
 
 To run tests, simply run below command:
 
 ```bash
 pytest -s --cov=.
 ```
```

### Comparing `eventsail-0.1.0/eventsail.py` & `eventsail-0.1.1/eventsail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import uuid
 import atexit
 import asyncio
 import inspect
 import warnings
 import functools
+from itertools import chain
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from weakref import ref, WeakMethod
+from typing import Optional, Iterable
 from concurrent.futures import ThreadPoolExecutor
 
 _pool = ThreadPoolExecutor(max_workers=os.cpu_count())
 
 atexit.register(_pool.shutdown)
 
 
@@ -26,35 +28,36 @@
             cls._instances_[hash_] = instance = cls(*args, **kwargs)
         return instance
 
     return _singleton
 
 
 class EmitterCore(ABC):
-    _instances_ = defaultdict(None)
 
     @abstractmethod
     def subscribe(self, event: str, listener): ...
     @abstractmethod
     def unsubscribe(self, event: str, listener): ...
     @abstractmethod
     def emit(self, event, *args, **kwargs): ...
     @abstractmethod
     def clear(self, event: str): ...
     @abstractmethod
     def once(self, event: str, listener): ...
 
-    def _call_listener(self, listener, *args, **kwargs):
-        raise NotImplementedError("Method not implemented")  # noqa
-
 
 class EmitterBase(EmitterCore):
+
     def __init__(self):
         self._listeners = defaultdict(lambda: set())
 
+    @staticmethod
+    def get_hash(cls, args, kwargs):
+        return hash((cls, args, frozenset(kwargs.items())))
+
     def __prepare_listener(self, listener):
         # check if listener is an instance method
         # wrap it in WeakMethod to avoid memory leak
         # else wrap it in ref and return
         if hasattr(listener, "__self__"):
             return WeakMethod(listener)
         return ref(listener)
@@ -124,20 +127,24 @@
                 else:
                     warnings.warn(f"Listener {listener} is dead, removing it")
                     listeners.remove(listener)
 
 
 @singleton
 class SyncEmitter(EmitterBase):
+    _instances_ = defaultdict(None)
+
     def _call_listener(self, listener, *args, **kwargs):
         listener(*args, **kwargs)
 
 
 @singleton
 class AsyncEmitter(EmitterBase):
+    _instances_ = defaultdict(None)
+
     def __init__(self, aio: bool = False):
         """
         Emitter class supporting async listeners
 
         Args:
             aio (bool, optional): If supports passing coroutine functions to the emitted event.
                                   Defaults to False.
@@ -195,14 +202,16 @@
             return
         # if not aio, run listener in executor
         _pool.submit(listener, *args, **kwargs)
 
 
 @singleton
 class Event(EmitterBase):
+    _instances_ = defaultdict(None)
+
     def __init__(self, event: str, is_sync: bool = True, use_asyncio: bool = False):
         self.event = event
         self.is_sync = is_sync
         self.use_asyncio = use_asyncio
         self.emitter = self._populate_emitter()
 
     def _populate_emitter(self):
@@ -255,14 +264,46 @@
 
         Args:
             listener (_type_): listener to subscribe to the event
         """
         self.emitter.once(self.event, listener)
         return listener
 
+    @property
+    def all_async_tasks(self) -> Optional[Iterable[asyncio.Task]]:
+        """
+        All async tasks running in the event loop for all emitter instances
+
+        Returns:
+            list[asyncio.Task]: List of all async tasks running in the event loop
+        """
+        return chain.from_iterable(
+            [i.own_async_tasks for i in AsyncEmitter()._instances_.values() if i.aio]
+        )
+
+    @property
+    def own_async_tasks(self) -> Optional[list[asyncio.Task]]:
+        """
+        List of async tasks running in the event loop for current emitter instance
+
+        Returns:
+            list[asyncio.Task]: List of async tasks running in the event loop
+        """
+        if self.is_sync or (not self.is_sync and not self.use_asyncio):
+            warnings.warn("Event is not async, no async tasks to return")
+            return
+        hash_ = self.get_hash(self.emitter.__class__, (), {"aio": self.use_asyncio})
+        return self.emitter._instances_[hash_].own_async_tasks
+
+    async def wait_for_async_tasks(self):
+        """
+        Wait for all async tasks to complete
+        """
+        await asyncio.wait(self.all_async_tasks, timeout=10)
+
 
 def event(event: str, is_sync: bool = True, use_asyncio: bool = False) -> Event:
     """
     Factory function to create an event
 
     Args:
         event (str): Name of the event
@@ -272,8 +313,31 @@
 
     Returns:
         Event: Instance of Event class
     """
     return Event(event, is_sync, use_asyncio)
 
 
+def on(event: str, is_sync: bool = True, use_asyncio: bool = False):
+    """
+    Decorator to subscribe a function to an event. Returns listener instance with event bound to
+    the listener instance. Can be accessed using `listener.event`.
+
+    Args:
+        event (str): Name of the event
+        is_sync (bool, optional): If Event is synchronous. Defaults to True.
+        use_asyncio (bool, optional): If Event supports coroutine execution.
+                                    Defaults to False.
+    """
+
+    def _on(listener):
+        event_ = Event(event, is_sync, use_asyncio)
+        event_.subscribe(listener)
+        listener.event = event_
+        return listener
+
+    return _on
+
+
+event.on = on
+
 __all__ = ["SyncEmitter", "AsyncEmitter", "EmitterBase"]
```

### Comparing `eventsail-0.1.0/pyproject.toml` & `eventsail-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventsail"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library for emitting events and handling them in a decoupled way."
 authors = ["Satyam Soni <satyam.soni@hotmail.co.uk>"]
 readme = "README.md"
 homepage = "https://github.com/satyamsoni2211/eventsail"
 repository = "https://github.com/satyamsoni2211/eventsail"
 keywords = ["events", "emitter", "event-emitter", "event-handling", "event-listener", "event-subscriber", "event-publisher"]
 classifiers = [
@@ -23,15 +23,15 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
```

### Comparing `eventsail-0.1.0/PKG-INFO` & `eventsail-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: eventsail
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for emitting events and handling them in a decoupled way.
 Home-page: https://github.com/satyamsoni2211/eventsail
 Keywords: events,emitter,event-emitter,event-handling,event-listener,event-subscriber,event-publisher
 Author: Satyam Soni
 Author-email: satyam.soni@hotmail.co.uk
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/satyamsoni2211/eventsail
 Description-Content-Type: text/markdown
 
 # EventSail
 
-[![codecov](https://codecov.io/gh/satyamsoni2211/eventsail/graph/badge.svg?token=1LW83DYL0R)](https://codecov.io/gh/satyamsoni2211/eventsail)
+[![codecov](https://codecov.io/gh/satyamsoni2211/eventsail/graph/badge.svg?token=AWAXXSH30S)](https://codecov.io/gh/satyamsoni2211/eventsail)
 
 EventSail is a minimal observer pattern package which is performant as well as supports both sync and async operations. Born out of utility and curiosity to replicate Javascript `EventEmitter`, here we are with library with similar functionalities.
 
+![codecov graph](https://codecov.io/gh/satyamsoni2211/eventsail/graphs/sunburst.svg?token=AWAXXSH30S)
+
 ## Usage
 
 ### Installation
 
 Package can be installed from `PyPi` using below command.
 
 ```bash
@@ -116,14 +118,29 @@
 
 ```python
 test_event.clear()
 ```
 
 `Event` class is also singleton class, so you will always get same instance for same set of arguments. This is intentionally kept in place so that we do not loose listeners subscribed.
 
+### Waiting for async tasks
+
+There can be instances where we would need to wait for async emitted tasks to complete before shutdown as this can be critical. `Event` class exposes certain properties containing `async` tasks.
+
+- `Event.all_async_tasks` : This will return all the async tasks scheduled over Event loop for the Emitter.
+- `Event.own_async_tasks` : This will only return async tasks corresponding to the immediate parent Emitter of the Event.
+
+To wait for async tasks to complete, `Event` class exposes awaitable API to wait for tasks to complete. This can be called as below.
+
+```python
+await test_event.wait_for_async_tasks()
+```
+
+This will wait for all the async tasks. This also has a default timeout for 10 seconds post which it will error out.
+
 ## Testing
 
 To run tests, simply run below command:
 
 ```bash
 pytest -s --cov=.
 ```
```

