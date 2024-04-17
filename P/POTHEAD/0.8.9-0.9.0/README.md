# Comparing `tmp/POTHEAD-0.8.9.tar.gz` & `tmp/POTHEAD-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "POTHEAD-0.8.9.tar", last modified: Wed Jun  7 09:28:04 2023, max compression
+gzip compressed data, was "POTHEAD-0.9.0.tar", last modified: Wed Apr 17 11:34:34 2024, max compression
```

## Comparing `POTHEAD-0.8.9.tar` & `POTHEAD-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:04.001194 POTHEAD-0.8.9/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.9/LICENSE
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-07 09:28:03.997194 POTHEAD-0.8.9/PKG-INFO
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:03.993193 POTHEAD-0.8.9/POTHEAD.egg-info/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/PKG-INFO
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/SOURCES.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      114 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/requires.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/top_level.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.9/README.md
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:03.997194 POTHEAD-0.8.9/pothead/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/__init__.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.9/pothead/cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.9/pothead/gating.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8134 2023-06-01 23:10:54.000000 POTHEAD-0.8.9/pothead/oob_response.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/resource_balancer.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/server.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    12045 2023-06-02 15:32:39.000000 POTHEAD-0.8.9/pothead/subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.9/pothead/test_cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/test_resource_balancer.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    16421 2023-06-02 16:27:07.000000 POTHEAD-0.8.9/pothead/test_subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    13439 2023-06-07 08:39:25.000000 POTHEAD-0.8.9/pothead/test_worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3784 2023-06-01 23:07:19.000000 POTHEAD-0.8.9/pothead/util.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14816 2023-06-02 16:27:07.000000 POTHEAD-0.8.9/pothead/worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.9/pothead/wsgi_typing.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-06-07 09:28:04.001194 POTHEAD-0.8.9/setup.cfg
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      914 2023-06-07 09:25:29.000000 POTHEAD-0.8.9/setup.py
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2024-04-17 11:34:34.257679 POTHEAD-0.9.0/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.9.0/LICENSE
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2024-04-17 11:34:34.257679 POTHEAD-0.9.0/PKG-INFO
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2024-04-17 11:34:34.257679 POTHEAD-0.9.0/POTHEAD.egg-info/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2024-04-17 11:34:34.000000 POTHEAD-0.9.0/POTHEAD.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      517 2024-04-17 11:34:34.000000 POTHEAD-0.9.0/POTHEAD.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        1 2024-04-17 11:34:34.000000 POTHEAD-0.9.0/POTHEAD.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      114 2024-04-17 11:34:34.000000 POTHEAD-0.9.0/POTHEAD.egg-info/requires.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        8 2024-04-17 11:34:34.000000 POTHEAD-0.9.0/POTHEAD.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.9.0/README.md
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2024-04-17 11:34:34.257679 POTHEAD-0.9.0/pothead/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.9.0/pothead/__init__.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.9.0/pothead/cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7733 2024-04-17 11:14:20.000000 POTHEAD-0.9.0/pothead/gating.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     9147 2023-08-23 18:45:53.000000 POTHEAD-0.9.0/pothead/oob_response.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2888 2024-04-17 11:14:20.000000 POTHEAD-0.9.0/pothead/resource_balancer.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2510 2023-06-08 10:16:14.000000 POTHEAD-0.9.0/pothead/server.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    12252 2023-06-08 10:16:14.000000 POTHEAD-0.9.0/pothead/subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.9.0/pothead/test_cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2527 2024-04-17 11:14:20.000000 POTHEAD-0.9.0/pothead/test_resource_balancer.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    16375 2023-06-08 10:16:14.000000 POTHEAD-0.9.0/pothead/test_subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    13801 2024-04-17 10:26:09.000000 POTHEAD-0.9.0/pothead/test_worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4791 2024-01-17 19:23:32.000000 POTHEAD-0.9.0/pothead/util.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    17077 2024-04-17 11:14:20.000000 POTHEAD-0.9.0/pothead/worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.9.0/pothead/wsgi_typing.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2024-04-17 11:34:34.257679 POTHEAD-0.9.0/setup.cfg
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      914 2024-04-17 11:32:10.000000 POTHEAD-0.9.0/setup.py
```

### Comparing `POTHEAD-0.8.9/LICENSE` & `POTHEAD-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/PKG-INFO` & `POTHEAD-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.9
+Version: 0.9.0
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.9/POTHEAD.egg-info/PKG-INFO` & `POTHEAD-0.9.0/POTHEAD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.9
+Version: 0.9.0
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.9/POTHEAD.egg-info/SOURCES.txt` & `POTHEAD-0.9.0/POTHEAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/README.md` & `POTHEAD-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/pothead/cgroups.py` & `POTHEAD-0.9.0/pothead/cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/pothead/gating.py` & `POTHEAD-0.9.0/pothead/gating.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         with self.lock:
             self.workers.remove(worker)
 
     def __len__(self):
         with self.lock:
             return len(self.workers)
 
+    def num_reservations(self):
+        return sum((1 if w.cpu_reservation_amount > 0 else 0) for w in self.workers)
+
     def reserved_cpu_amount(self):
         with self.lock:
             return sum([w.cpu_reservation_amount for w in self.workers])
 
 
 class InertialTimeDerivate:
     """Timed measurement on an incrementing counter
@@ -108,15 +111,20 @@
         delta = new_value - self.last_value
         self.last_check = this_check
         self.last_value = new_value
         return self.inertial_value.update(delta / elapsed)
 
 
 def wait_for_idle_cpus(
-    required, *, max_concurrent=None, inertia=0.7, keep_cpu_reservation=False
+    required,
+    *,
+    max_concurrent=None,
+    inertia=0.7,
+    reservation_uncertainty=1.3,
+    keep_cpu_reservation=False
 ):
     """CPU-gated wait_for_slot implementation
 
     Creates a wait_for_slot-callable that will let through at least one concurrent job, and additional jobs
     as long as `required` cpu:s are idle. It is cgroup-aware, and will not fetch new jobs that would break
     configured cgroup-limit. It will also measure the total CPU _of the current cgroup_, as reported by
     /sys/fs/cgroup/cpu.stat. Typically, when running under Linux, in a container, or in the host operating
@@ -158,19 +166,23 @@
             max_concurrent = ceil(
                 cpu_count() * DEFAULT_MAX_CONCURRENT_MULTIPLIER / required
             )
 
     def cpu_is_available(idle, cpu_used):
         reserved = worker_list.reserved_cpu_amount()
         cpu_used += reserved
+        # If there are already reservations made, we increase the CPU required to start a new job
+        required_with_reservation_uncertainty = required * (
+            reservation_uncertainty ** worker_list.num_reservations()
+        )
 
         if cpu_used < CPU_PROMISED:
             return True
 
-        if idle - reserved < required:
+        if idle - reserved < required_with_reservation_uncertainty:
             return False
 
         return cpu_used <= cpu_quota
 
     def wait_for_slot(halt):
         start_time = monotonic()
```

### Comparing `POTHEAD-0.8.9/pothead/oob_response.py` & `POTHEAD-0.9.0/pothead/oob_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from logging import getLogger
 from os import environ, urandom
 from threading import Lock, Thread, Timer
 from time import monotonic, sleep
 from typing import (
-    Any,
     Dict,
     Generator,
+    Iterable,
     Iterator,
+    List,
     Optional,
     Sequence,
     Tuple,
     Generic,
     TypeVar,
     Callable,
 )
@@ -21,27 +22,28 @@
 from .wsgi_typing import (
     Environ,
     ExcInfo,
     ResponseStream,
     StartResponse,
     WsgiApplication,
 )
-from .util import SocketCheckingWSGIHandler, ThreadsTracker
+from .util import SocketCheckingWSGIHandler, JobTracker
 
 # Interval of how often to attempt cleanup of unclaimed jobs
 CLEANUP_INTERVAL_SECONDS = float(environ.get("OOB_CLEANUP_INTERVAL_SECONDS", "5"))
 
 # Maximum time a process is allowed to remain unclaimed before attempting to clean it up
 ITEM_EXPIRY_SECONDS = float(environ.get("OOB_ITEM_EXPIRY_SECONDS", "20"))
 
 LOGGER = getLogger("pothead.oob_response")
 
 
 class Response:
-    def __init__(self, headers, body, on_done):
+    def __init__(self, request_id, headers, body, on_done):
+        self.request_id = request_id
         self.headers = headers
         self.body = body
         self.on_done = on_done
 
     def close(self):
         if self.on_done:
             self.body.close()
@@ -61,31 +63,31 @@
 
     With regular intervals, unclaimed keys are purged. If the value has a method
     `close()`, it is called on purging."""
 
     def __init__(self, cleanup_interval_seconds: float, item_expiry_seconds: float):
         self._cleanup_interval_seconds = cleanup_interval_seconds
         self._item_expiry_seconds = item_expiry_seconds
-        self._dict: Dict[str, Tuple[float, Any]] = dict()
+        self._dict: Dict[str, Tuple[float, Response]] = dict()
         self._lock = Lock()
         self._shutdown = False
 
         self._cleanup()
 
-    def push(self, value: Any):
+    def push(self, value: Response):
         key = urandom(24).hex()
         now = monotonic()
         expires_at = now + self._item_expiry_seconds
         with self._lock:
             assert key not in self._dict
             self._dict[key] = (expires_at, value)
 
         return key
 
-    def pop(self, key) -> Optional[Any]:
+    def pop(self, key) -> Optional[Response]:
         with self._lock:
             return self._dict.pop(key, (None, None))[1]
 
     def close(self):
         self._shutdown = True
         with self._lock:
             for expires_at, job in self._dict.values():
@@ -96,14 +98,18 @@
     def wait_for_clear(self):
         while True:
             with self._lock:
                 if len(self._dict) == 0:
                     return
             sleep(self._cleanup_interval_seconds / 2)
 
+    def requests(self) -> List[str]:
+        with self._lock:
+            return [job.request_id for expires_at, job in self._dict.values()]
+
     def _cleanup(self):
         if not self._shutdown:
             t = Timer(self._cleanup_interval_seconds, self._cleanup)
             t.daemon = True
             t.start()
         now = monotonic()
         with self._lock:
@@ -133,19 +139,21 @@
 
     def get(self) -> AtomicReferenceT:
         with self._lock:
             return self.data
 
 
 def take_until(
-    iterator: Iterator[bytes], condition: Callable[[], bool]
+    iterable: Iterable[bytes], condition: Callable[[], bool]
 ) -> Generator[bytes, None, Iterator[bytes]]:
     """Yields chunks until the first one after which condition is true. That chunk, and all the remaining chunks, are
     returned via generator-return, as a new generator"""
 
+    iterator = iter(iterable)
+
     def trimmed_generator(first_value):
         yield first_value
         yield from iterator
 
     for chunk in iterator:
         if condition():
             return trimmed_generator(chunk)
@@ -180,49 +188,65 @@
             app=wsgi_app,
             threaded=True,
             request_handler=SocketCheckingWSGIHandler,
         )
         responder_service = Thread(target=self._server.serve_forever)
         responder_service.daemon = True
         responder_service.start()
-        self._worker_tracker = ThreadsTracker()
+        self._worker_tracker = JobTracker()
         self._service_port = self._server.port
 
+    def ongoing_requests(self) -> List[str]:
+        return self._worker_tracker.ongoing_requests()
+
     def _content_response_wsgi(self, environ, start_response):
-        with self._worker_tracker:
-            path = environ["PATH_INFO"]
-            if len(path) < 2 or path[0] != "/":
-                start_response("404 Not Found", {})
-                return []
+        path = environ["PATH_INFO"]
+        if len(path) < 2 or path[0] != "/":
+            start_response("404 Not Found", {})
+            return []
 
+        with self._worker_tracker.scope("<pending>") as work_scope:
             response_key = path[1:]
             response = self._job_transfer.pop(response_key)
             if response is None:
                 start_response(
                     f"410 {response_key} is claimed, expired, or never registered", {}
                 )
                 return []
 
+            work_scope.update(response.request_id)
             with response:
                 start_response(
                     "200 OK",
                     response.headers,
                 )
                 yield b""  # Flush response to client
                 for chunk in response.body:
                     yield chunk
 
     def shutdown(self):
-        LOGGER.info("Draining pending redirects")
+        request_ids = self._job_transfer.requests()
+        LOGGER.info(
+            f"Draining pending redirects: {','.join(request_ids)}",
+            extra={"requests": request_ids},
+        )
         self._job_transfer.wait_for_clear()
         self._server.shutdown()
         LOGGER.info("Waiting for jobs to complete")
-        self._worker_tracker.drain()
+        self._worker_tracker.drain(LOGGER)
         LOGGER.info("Shutdown complete")
 
+    def inspect(self):
+        yield "OOB responses waiting:\n".encode()
+        for request_id in self._job_transfer.requests():
+            yield f"  {request_id}\n".encode()
+        yield "OOB responses ongoing:\n".encode()
+        for request_id in self._worker_tracker.ongoing_requests():
+            yield f"  {request_id}\n".encode()
+
     def __call__(
         self,
         environ: Environ,
         start_response: StartResponse,
         assume_cleanup: Callable[[], Callable[[], None]],
     ) -> ResponseStream:
         start_response_called: AtomicReference[
@@ -246,15 +270,18 @@
             msg = "Application Terminated Without Response"
             LOGGER.error(msg)
             return
 
         (status, headers, exc_info) = start_response_called.get()
         if not exc_info and status.startswith("200 "):
             on_done = assume_cleanup()
-            key = self._job_transfer.push(Response(headers, response_chunks, on_done))
+            request_id = environ.get("REQUEST_ID", "<unknown>")
+            key = self._job_transfer.push(
+                Response(request_id, headers, response_chunks, on_done)
+            )
             start_response(
                 "303 See Other",
                 (
                     (
                         "Location",
                         f"http://{environ['SERVER_NAME']}:{self._service_port}/{key}",
                     ),
```

### Comparing `POTHEAD-0.8.9/pothead/resource_balancer.py` & `POTHEAD-0.9.0/pothead/resource_balancer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from itertools import chain
 from random import shuffle
 from threading import Condition, Lock
 from typing import Iterable
-from math import inf
 
 
 class Resource:
+    usage: int
+
     def __init__(self, resource):
         self.resource = resource
         self.usage = 0
 
-    def __cmp__(self, other):
-        return self.usage.__cmp__(other.usage)
-
     def __lt__(self, other):
         return self.usage.__lt__(other.usage)
 
 
 class ResourceLoan:
     def __init__(self, balancer, instance):
         self._lock = Lock()
@@ -32,24 +30,41 @@
                 self._balancer._release(self._instance)
                 self._balancer = None
 
     def __exit__(self, type, value, traceback):
         self.release()
 
 
-class BoundedResourceBalancer:
-    def __init__(self, bound=inf):
+class ResourceBalancer:
+    def __init__(self):
         self._active = list()
         self._ghosts = list()
         self._condition = Condition()
-        self.bound = bound
 
     def _available(self):
-        available = (r for r in self._active if r.usage < self.bound)
-        return next(available, None)
+        return next(iter(self._active), None)
+
+    def usage_min(self) -> int:
+        """Returns the usage-level for the least used resource"""
+        return min((r.usage for r in self._active), default=0)
+
+    def wait_for_change(self, value_fn, prev, timeout=None):
+        def predicate():
+            new_value = value_fn()
+            if new_value != prev:
+                return (new_value,)
+            else:
+                return None
+
+        with self._condition:
+            maybe_new = self._condition.wait_for(predicate=predicate, timeout=timeout)
+            if maybe_new:
+                return maybe_new[0]
+            else:
+                return prev
 
     def active_count(self):
         return len(self._active)
 
     def acquire(self) -> ResourceLoan:
         with self._condition:
             winner = self._condition.wait_for(self._available)
```

### Comparing `POTHEAD-0.8.9/pothead/server.py` & `POTHEAD-0.9.0/pothead/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from asyncio import Queue, sleep
 from asyncio import Future
 
 from aiohttp import web
 from aiohttp.client_reqrep import ClientRequest
 from aiohttp.client_proto import ResponseHandler
 
-jobs = Queue()
+jobs = Queue()  # type: ignore
 
 
 class MockConn:
     def __init__(self, protocol):
         self.protocol = protocol
 
     def release(self):
```

### Comparing `POTHEAD-0.8.9/pothead/subprocess_middleware.py` & `POTHEAD-0.9.0/pothead/subprocess_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 import io
 import multiprocessing
 import psutil
 from logging import Logger
 from multiprocessing.connection import Connection
+from multiprocessing.context import ForkServerProcess
 from re import compile
 from setproctitle import setproctitle
 from tblib import pickling_support
 from threading import Thread
 import werkzeug
 
 from typing import (
@@ -212,20 +213,34 @@
                 elif isinstance(msg, MsgDone):
                     break
                 else:
                     assert (
                         False
                     ), f"Got unknown message type from WSGI subprocess: {msg}"
         finally:
-            if subprocess.pid is None:
-                self.logger.info("Process failed startup, not killing")
-            else:
-                _kill_process_and_its_descendants(subprocess)
+            if self._kill_process_and_its_descendants(subprocess):
                 request_sender_thread.join()
 
+    def _kill_process_and_its_descendants(self, process: ForkServerProcess):
+        if process.pid is None:
+            self.logger.info("Process failed startup, not killing")
+            return False
+        descendants = _suspend_recursive(process.pid)
+
+        for descendant in descendants:
+            try:
+                descendant.kill()
+            except psutil.NoSuchProcess:
+                # Without a defined order, descendants might be already orphaned, adopted and killed
+                # by init when we get to them
+                continue
+
+        process.join()
+        return True
+
     @staticmethod
     def send_request_data(logger: Logger, environ: Environ, writer: Connection):
         try:
             with writer:
                 request_data = werkzeug.Request(
                     cast(Dict[str, Any], environ)
                 ).stream.read()
@@ -253,15 +268,17 @@
     environ: Environ,
     msg_writer: Connection,
     wsgi_input_reader: Connection,
     has_reset_cpu_reservation_callback,
 ):
     with msg_writer, wsgi_input_reader:
         try:
-            request_id = NAME_FILTER.sub("", environ.get("HTTP_X_REQUEST_ID", ""))
+            request_id_header = environ.get("HTTP_X_REQUEST_ID", "")
+            assert isinstance(request_id_header, str)
+            request_id = NAME_FILTER.sub("", request_id_header)
             if request_id:
                 setproctitle(f"ph-worker:{request_id}")
             else:
                 setproctitle("ph-worker (anon)")
 
             def wrapped_start_response(
                 http_status: str,
@@ -309,15 +326,15 @@
 
             msg_writer.send(MsgDone())
         except Exception as exc:
             msg_writer.send(MsgExceptionRaised(exc))
             raise
 
 
-def _suspend_recursive(pid: psutil.Process) -> Iterable[psutil.Process]:
+def _suspend_recursive(pid: int) -> Iterable[psutil.Process]:
     """Gets a list of process and descendants. The only way to do it ~"atomically", is to suspend
     them in the process, preventing them from forking or dying while we're looking the other way.
 
     Returns a list of now suspended processes, including the root specified by pid"""
     try:
         proc = psutil.Process(pid)
         proc.suspend()
@@ -337,21 +354,7 @@
                 continue
             else:
                 return []
         if len(descendants) == prior_count:
             break
 
     return descendants
-
-
-def _kill_process_and_its_descendants(process: multiprocessing.Process):
-    descendants = _suspend_recursive(process.pid)
-
-    for descendant in descendants:
-        try:
-            descendant.kill()
-        except psutil.NoSuchProcess:
-            # Without a defined order, descendants might be already orphaned, adopted and killed
-            # by init when we get to them
-            continue
-
-    process.join()
```

### Comparing `POTHEAD-0.8.9/pothead/test_cgroups.py` & `POTHEAD-0.9.0/pothead/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/pothead/test_resource_balancer.py` & `POTHEAD-0.9.0/pothead/test_resource_balancer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .resource_balancer import BoundedResourceBalancer
+from .resource_balancer import ResourceBalancer
 from threading import Thread
 from unittest import TestCase
 
 
 class AsyncRunner(Thread):
     def __init__(self, target):
         def main():
@@ -22,39 +22,39 @@
             raise self.exception
         else:
             return self.result
 
 
 class ResourceBalancerTest(TestCase):
     def test_basic_function(self):
-        b = BoundedResourceBalancer()
+        b = ResourceBalancer()
         b.provision([1, 2])
 
         with b.acquire() as resource1:
             with b.acquire() as resource2:
                 assert resource1 != resource2
             with b.acquire() as resource2:
                 assert resource1 != resource2
                 with b.acquire() as resource3:
                     assert resource3 in (resource1, resource2)
                     with b.acquire() as resource4:
                         assert resource3 != resource4
 
     def test_delayed_init(self):
-        b = BoundedResourceBalancer()
+        b = ResourceBalancer()
 
         t = AsyncRunner(b.acquire)
         with self.assertRaises(TimeoutError):
             t.join(0.001)
 
         b.provision([1])
         assert t.join().__enter__() == 1
 
     def test_ghosts(self):
-        b = BoundedResourceBalancer()
+        b = ResourceBalancer()
         b.provision([1])
 
         resource1 = b.acquire()
         with resource1:
             b.provision([])
 
             t = AsyncRunner(b.acquire)
@@ -65,28 +65,28 @@
             resource2 = t.join()
 
             assert resource1._instance is resource2._instance
             assert resource2._instance.usage == 2
             assert resource2._instance.resource == 1
 
     def test_vanishing_resource(self):
-        b = BoundedResourceBalancer()
+        b = ResourceBalancer()
         b.provision([1])
 
         with b.acquire():
             b.provision([])
             assert b._ghosts[0].usage == 1
             assert b._ghosts[0].resource == 1
 
         assert b._ghosts[0].usage == 0
         b.provision([])
         assert b._ghosts == []
 
     def test_even_load(self):
-        b = BoundedResourceBalancer()
+        b = ResourceBalancer()
         b.provision([1, 2])
 
         with b.acquire() as resource1:
             pass
 
         with b.acquire() as resource2:
             pass
```

### Comparing `POTHEAD-0.8.9/pothead/test_subprocess_middleware.py` & `POTHEAD-0.9.0/pothead/test_subprocess_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,15 +358,15 @@
                     p.terminate()
 
                 if leaked_subprocess:
                     assert False, f"Subprocess was leaked: {leaked_subprocess}"
 
     def test_middleware_provides_interruption_points(
         self,
-    ) -> Optional[Exception]:
+    ):
         from . import subprocess_middleware as mw
 
         orig_INTERRUPTIBLE_INTERVAL_S = mw.INTERRUPTIBLE_INTERVAL_S
         mw.INTERRUPTIBLE_INTERVAL_S = 0.05
 
         try:
             client = Client(SubprocessMiddleware(LOGGER, wrapped_app))
@@ -379,15 +379,15 @@
             )  # Even though the app is now hung, we expect the middleware to yield empty responses after a timeout
             assert next(response.response) == b""  # And keep yielding
         finally:
             mw.INTERRUPTIBLE_INTERVAL_S = orig_INTERRUPTIBLE_INTERVAL_S
 
     def test_closed_response_kills_subprocess(
         self,
-    ) -> Optional[Exception]:
+    ):
         request_id = str(uuid4())
         client = Client(SubprocessMiddleware(LOGGER, wrapped_app))
 
         response = client.post(
             "/hang_forever", data=b"", headers=[("x-request-id", request_id)]
         )
         wait_for(lambda: worker_running(request_id), timeout=100)
```

### Comparing `POTHEAD-0.8.9/pothead/test_worker.py` & `POTHEAD-0.9.0/pothead/test_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,19 @@
         wait_for(lambda: not worker_running(self.request_id), timeout=2)
 
 
 class TestShutdown(TestCase):
     DELAY_START_RESPONSE = 0.3
     DELAY_FINISH_RESPONSE = 0.8
 
+    @fixture(autouse=True)
+    def use_caplog(self, caplog):
+        caplog.set_level(INFO)
+        self.caplog = caplog
+
     def setUp(self):
         broker = DummyBroker()
         self.callbacks = MagicMock()
 
         def app(environ, start_response):
             sleep(self.DELAY_START_RESPONSE)
             start_response("200 OK", {})
@@ -405,30 +410,34 @@
 
     def test_ptth_finish_before_shutdown(self):
         self.connection.send_request()
         Thread(target=self.connection.read_response).start()
         self.assertGreaterEqual(
             self.shutdown_time(), OOB_ITEM_EXPIRY_SECONDS + self.DELAY_START_RESPONSE
         )
+        assert f"Draining ongoing requests: {REQUEST_ID}" in self.caplog.text
 
     def test_pending_oob_expire_before_shutdown(self):
         self.connection.send_request()
         self.connection.read_response()
         st = self.shutdown_time()
         self.assertGreaterEqual(st, OOB_ITEM_EXPIRY_SECONDS)
         self.assertLessEqual(st, self.DELAY_FINISH_RESPONSE)
+        assert f"Draining pending redirects: {REQUEST_ID}" in self.caplog.text
 
     def test_oob_finish_before_shutdown(self):
         self.connection.send_request()
         status, headers = self.connection.parse_response()
         assert status == 303
 
         with urlopen(headers.get("location")) as real_response:
             assert real_response.status == 200
 
             # Still running the request, we expect it to be finished before shutdown
             self.assertGreaterEqual(self.shutdown_time(), self.DELAY_FINISH_RESPONSE)
 
+            assert f"Draining ongoing requests: {REQUEST_ID}" in self.caplog.text
+
     def shutdown_time(self):
         start = monotonic()
         self.server.shutdown()
         return monotonic() - start
```

### Comparing `POTHEAD-0.8.9/pothead/worker.py` & `POTHEAD-0.9.0/pothead/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 from http import HTTPStatus
 from logging import getLogger
+from os import environ
 from signal import SIGTERM, signal
 from socket import (
     AF_INET,
     IPPROTO_TCP,
     SHUT_RDWR,
     SO_KEEPALIVE,
     SOCK_STREAM,
@@ -22,17 +23,17 @@
 from uuid import uuid4
 from wsgiref import simple_server
 
 from werkzeug.serving import BaseWSGIServer, make_server
 
 from .gating import wait_for_idle_cpus
 from .oob_response import OutOfBandResponder
-from .resource_balancer import BoundedResourceBalancer, ResourceLoan
+from .resource_balancer import ResourceBalancer, ResourceLoan
 from .subprocess_middleware import SubprocessMiddleware
-from .util import ObjectProxy, SocketCheckingWSGIHandler, ThreadsTracker
+from .util import JobTracker, ObjectProxy, SocketCheckingWSGIHandler
 from .wsgi_typing import (
     WsgiApplication,
 )
 
 LOGGER = getLogger("pothead.worker")
 BROKER_CONNECT_RETRY_INTERVAL = 2
 
@@ -70,26 +71,30 @@
     def wait(self, timeout: float):
         with self._cond:
             self._cond.wait_for(lambda: self._set, timeout)
 
 
 class Handler(SocketCheckingWSGIHandler):
     protocol_version = "HTTP/1.1"
+    ph_server: "Server"
+    request_received_at: Optional[float]
+    request_id: Optional[str]
 
     def __init__(
-        self, socket, address, server, cb_request_received, cb_processing_done
+        self, socket, address, server: "Server", cb_request_received, cb_processing_done
     ):
         self.cb_request_received = cb_request_received
         self.env = None
         self.request_id = None
         self.request_received_at = None
+        self.ph_server = server
 
         with DeferrableCleanup(cb_processing_done) as c:
             if isinstance(server.app, OutOfBandResponder):
-                server = ObjectProxy(server)
+                server = ObjectProxy(server)  # type: ignore
                 server.app = self._oob_wrapped_app(server.app, c.assume)
 
             super().__init__(socket, address, server)
 
     @staticmethod
     def _oob_wrapped_app(app, assume_cleanup) -> WsgiApplication:
         def application(environ, start_response):
@@ -102,68 +107,99 @@
             # Handler may be used for several requests, so we must reset
             # environment overrides each time
             self.env = None
             super().handle_one_request()
         finally:
             self.close_connection = True
 
+    def run_wsgi(self) -> None:
+        self.request_received_at = monotonic()
+        self.request_id = str(self.headers.get("X-Request-Id", None) or uuid4())
+
+        # This socket shall no longer be fast-closed on SIGTERM
+        socket = self.request
+        self.ph_server.sockets_waiting_for_request.remove(socket)
+
+        with self.ph_server.worker_tracker.scope(self.request_id):
+            super().run_wsgi()
+
     def make_environ(self):
         environ = super().make_environ()
+        environ["REQUEST_ID"] = self.request_id
 
         if self.cb_request_received:
             self.cb_request_received(environ)
 
         return environ
 
-    def parse_request(self):
-        success = super().parse_request()
-        if success:
-            self.request_received_at = monotonic()
-            self.request_id = self.headers.get("X-Request-Id", None) or str(uuid4())
-
-        # This socket shall no longer be fast-closed on SIGTERM
-        socket = self.request
-        self.server.sockets_waiting_for_request.remove(socket)
-
-        return success
-
     def log_message(self, format, *args):
         LOGGER.info("[%s] " + format, self.request_id, *args)
 
     def log_request(self, code="-", size="-"):
         if isinstance(code, HTTPStatus):
             code = code.value
         LOGGER.info(
-            'Starting request [%s] "%s" %s %s',
+            'Accepted request [%s] "%s" %s %s',
             self.request_id,
             self.requestline,
             str(code),
             str(size),
         )
 
+    def connection_dropped(self, e, env):
+        self.log_error("Cancelled by disconnected client")
+
     def log_error(self, format, *args):
         LOGGER.error("[%s] " + format, self.request_id, *args)
 
     def log_elapsed(self):
         LOGGER.info(
             "[%s] Elapsed: %.3f",
             self.request_id,
             monotonic() - self.request_received_at,
         )
 
 
 class LoadBalancer:
     REFRESH_INTERVAL = 5
+    DELAY_BASE = float(environ.get("LOAD_BALANCER_CONNECTION_DELAY_BASE", 1))
+    DELAY_EXP = float(environ.get("LOAD_BALANCER_CONNECTION_DELAY_EXP", 1.5))
 
     def __init__(self, host, port):
         self.host = host
         self.port = port
-        self._balancer = BoundedResourceBalancer(1)
+        self._balancer = ResourceBalancer()
         self.refresh()
 
+    def min_instance_connections(self):
+        return self._balancer.usage_min()
+
+    def wait_if_all_busy(self):
+        """If all resources are already busy, wait for a while, longer if resources are more busy.
+        If resources become more available while waiting, the wait-time will be reduced.
+        """
+        min_connections = self._balancer.usage_min()
+        if min_connections > 0:
+            # All endpoints already have
+            start = monotonic()
+            time_left = (
+                start
+                + (self.DELAY_BASE * (min_connections**self.DELAY_EXP))
+                - monotonic()
+            )
+            while time_left > 0:
+                min_connections = self._balancer.wait_for_change(
+                    self._balancer.usage_min, min_connections, timeout=time_left
+                )
+                time_left = (
+                    start
+                    + (self.DELAY_BASE * (min_connections**self.DELAY_EXP))
+                    - monotonic()
+                )
+
     def acquire_addr(self) -> ResourceLoan:
         return self._balancer.acquire()
 
     def refresh(self):
         try:
             results = getaddrinfo(self.host, self.port, type=SOCK_STREAM)
             hosts = (sockaddr for _f, _t, _p, _c, sockaddr in results)
@@ -173,18 +209,27 @@
                 "Failed to refresh endpoints for %s:%d", self.host, self.port
             )
         t = Timer(self.REFRESH_INTERVAL, self.refresh)
         t.daemon = True
         t.start()
 
 
+class RequestCounter:
+    def __init__(self, app):
+        self._app = app
+        self.started = 0
+        self.completed = 0
+
+    def __call__(self, environ, start_response):
+        self.started += 1
+        yield from self._app(environ, start_response)
+        self.completed += 1
+
+
 class Server:
-    shutdown_signal = (
-        False  # Must exist for werkzeug 1.x legacy. Can be dropped with werkzeug 2.x
-    )
     ssl_context = None
     multithread = False
     multiprocess = False
     passthrough_errors = False
     inspection_server: Optional[BaseWSGIServer] = None
 
     def __init__(
@@ -208,15 +253,15 @@
         env["REMOTE_HOST"] = ""
         env["CONTENT_LENGTH"] = ""
         env["SCRIPT_NAME"] = ""
         self.base_environ = env
 
         self.broker_balancer = load_balancer(host, port)
         self.sockets_waiting_for_request: Set[socket] = set()
-        self.worker_tracker = ThreadsTracker()
+        self.worker_tracker = JobTracker()
 
         self.stopping = Flag()
         self.stopped = Flag()
 
         if inspection_port is not None:
             self.inspection_server = make_server(
                 "", inspection_port, self.inspect, threaded=True
@@ -228,14 +273,15 @@
             del app.wait_for_slot
         self.app = app
         self.app = (
             SubprocessMiddleware(LOGGER, self.app)
             if use_request_subprocess
             else self.app
         )
+        self.app = self.request_counter = RequestCounter(self.app)
         self.app = (
             OutOfBandResponder(
                 self.app,
                 redirect_port,
                 oob_cleanup_interval_seconds,
                 oob_item_expiry_seconds,
             )
@@ -246,27 +292,32 @@
     def inspect(self, environ, start_response):
         if environ.get("REQUEST_METHOD", None) != "GET":
             start_response("405 Only GET supported", ())
             return
         path = environ.get("PATH_INFO", None)
         if path == "/inspect":
             start_response("200 OK", ())
-            yield f"{len(self.worker_tracker)} workers running\n".encode()
+            yield "requests pending:\n".encode()
+            for request_id in self.worker_tracker.ongoing_requests():
+                yield f"  {request_id}\n".encode()
+            if hasattr(self.app, "inspect"):
+                yield from self.app.inspect()
             yield f"{len(self.sockets_waiting_for_request)} blocked waiting for request\n".encode()
         elif path == "/apocalypse":
             start_response("200 OK", ())
             while not self.stopped.wait(5):
                 yield b"Not yet\n"
             yield b"It's time\n"
         else:
             start_response("404 Not found", ())
 
     def worker(self):
         while not self.stopping:
-            with self.worker_tracker, self.broker_balancer.acquire_addr() as addr:
+            with self.broker_balancer.acquire_addr() as addr:
+                self.broker_balancer.wait_if_all_busy()
                 self._fetch_and_run_one_job(addr)
 
     def _fetch_and_run_one_job(
         self, addr, cb_request_received=None, cb_processing_done=lambda: None
     ):
         with socket(AF_INET, SOCK_STREAM) as s:
             self.sockets_waiting_for_request.add(s)
@@ -309,22 +360,27 @@
         for s in list(self.sockets_waiting_for_request):
             try:
                 s.shutdown(SHUT_RDWR)
                 s.close()
             except OSError:
                 pass
 
-        self.worker_tracker.drain()
+        self.worker_tracker.drain(LOGGER)
 
         if isinstance(self.app, OutOfBandResponder):
             self.app.shutdown()
         LOGGER.info("Worker shutdown completed")
         self.stopped.set()
         if self.inspection_server is not None:
             self.inspection_server.shutdown()
+        LOGGER.info(
+            "%d jobs started. %d jobs successfully completed",
+            self.request_counter.started,
+            self.request_counter.completed,
+        )
         LOGGER.info("All services stopped")
 
     def poll_loop(self):
         """Uses app.wait_for_slot() spawn new workers dynamically. This is useful, for example to wait for
         enough CPU, memory, or disk space, to start next job.
 
         `wait_for_slot` is expected to block until it's time to poll for a new job. It is given a function
@@ -333,33 +389,35 @@
         It may return an object, if so `obj.request_received(environ)` will be called when a request is
         received and `obj.done()` when either the request is received, or if polling failed in which case
         `request_received()` was never called.
 
         See pothead.gating for some ready-made `wait_for_slot` implementations"""
 
         while not self.stopping:
+            # If all brokers are already waiting for a request, we want to hold off for a little bit
+            self.broker_balancer.wait_if_all_busy()
+
             callbacks = self.wait_for_slot(lambda: bool(self.stopping))
             if self.stopping:
                 break
 
-            # This will block as long as we are waiting for requests from all broker-instances
             broker_instance_lease = self.broker_balancer.acquire_addr()
             if self.stopping:
                 break
 
             Thread(
                 target=self._run_one_poll, args=(broker_instance_lease, callbacks)
             ).start()
 
     def _run_one_poll(self, broker_instance_lease: ResourceLoan, callbacks):
         def request_received(environ):
             broker_instance_lease.release()
             getattr(callbacks, "request_received", lambda _: None)(environ)
 
-        with self.worker_tracker, broker_instance_lease as addr:
+        with broker_instance_lease as addr:
             self._fetch_and_run_one_job(
                 addr, request_received, getattr(callbacks, "done", lambda: None)
             )
 
     def log(self, type, msg, *args, **kwargs):
         getattr(LOGGER, type)(msg.rstrip(), *args, **kwargs)
 
@@ -374,36 +432,36 @@
 
     p = signal(SIGTERM, on_term)
     if p:
         previous.append(p)
 
 
 demo_app = simple_server.demo_app
-demo_app.wait_for_slot = wait_for_idle_cpus(3)
+demo_app.wait_for_slot = wait_for_idle_cpus(3)  # type: ignore
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
     from importlib import import_module
     from logging import INFO, basicConfig
-    from os import environ
     from sys import path
 
     path.insert(0, ".")
 
     def address(str):
         (host, port) = str.rsplit(":", 1)
         return (host, int(port))
 
     def func(str):
         (module, symbol) = str.rsplit(":", 1)
         module = import_module(module)
         return getattr(module, symbol)
 
     DEFAULT_WORKERS = int(environ.get("POTHEAD_WORKERS", 1))
+    DEFAULT_MAX_PENDING = int(environ.get("POTHEAD_MAX_PENDING", 1))
 
     parser = ArgumentParser(description="Run WSGI app in sequential `worker` mode")
     parser.add_argument(
         "--connect",
         default="localhost:4040",
         type=address,
         help="Load Balancer Hub to connect to [host:port]",
@@ -429,15 +487,15 @@
     )
 
     job_control_group = parser.add_mutually_exclusive_group()
     job_control_group.add_argument(
         "--workers",
         default=DEFAULT_WORKERS,
         type=int,
-        help="Number of worker Processes",
+        help=f"Number of worker Processes (default: {DEFAULT_WORKERS})",
     )
     job_control_group.add_argument(
         "--poll-jobs",
         action="store_true",
         help="Use `app.wait_for_slot` to determine when to pull new jobs",
     )
```

### Comparing `POTHEAD-0.8.9/pothead/wsgi_typing.py` & `POTHEAD-0.9.0/pothead/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.9/setup.py` & `POTHEAD-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 common_deps = ["psutil", "werkzeug>=2.1", "tblib", "setproctitle"]
 test_deps = [*common_deps, "aiohttp", "timeout-decorator"]
 
 setuptools.setup(
     name="POTHEAD",
-    version="0.8.9",
+    version="0.9.0",
     author="Ulrik Mikaelsson",
     author_email="ulrik.mikaelsson@gmail.com",
     description="A reverse-http proxy implementation for non-concurrent requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/rawler/pothead",
     packages=setuptools.find_packages(),
```

