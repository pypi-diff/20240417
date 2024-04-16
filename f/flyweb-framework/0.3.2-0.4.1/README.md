# Comparing `tmp/flyweb_framework-0.3.2.tar.gz` & `tmp/flyweb_framework-0.4.1.tar.gz`

## Comparing `flyweb_framework-0.3.2.tar` & `flyweb_framework-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/.gitattributes
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/.python-version
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/bootstrap
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/requirements-dev.lock
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/requirements.lock
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/.github/workflows/python.yml
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/misc/run_precommit
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/__init__.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/_app.py
--rw-r--r--   0        0        0    28179 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/_flyweb.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/_server.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/_server_stub.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/components/__init__.py
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/components/_components.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/examples/counter/__main__.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/examples/misc/__main__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/examples/stopwatch/__main__.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/examples/todo/__main__.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/static/index.html
--rw-r--r--   0        0        0    41680 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/static/maquette.umd.js
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/static/script.js
--rw-r--r--   0        0        0    45806 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/src/flyweb/static/socket.io.min.js
--rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/tests/browser_test.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/tests/components_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/tests/conftest.py
--rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/tests/flyweb_test.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/.gitignore
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/LICENSE
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/README.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 flyweb_framework-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.gitattributes
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.python-version
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/bootstrap
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/requirements-dev.lock
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/requirements.lock
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.github/release-drafter.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/misc/run_precommit
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/__init__.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/_app.py
+-rw-r--r--   0        0        0    28179 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/_flyweb.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/_server.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/_server_stub.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/components/__init__.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/components/_components.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/examples/counter/__main__.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/examples/misc/__main__.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/examples/stopwatch/__main__.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/examples/todo/__main__.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/static/index.html
+-rw-r--r--   0        0        0    41680 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/static/maquette.umd.js
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/static/script.js
+-rw-r--r--   0        0        0    45806 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/src/flyweb/static/socket.io.min.js
+-rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/tests/browser_test.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/tests/components_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/tests/conftest.py
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/tests/flyweb_test.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/.gitignore
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/README.md
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 flyweb_framework-0.4.1/PKG-INFO
```

### Comparing `flyweb_framework-0.3.2/.pre-commit-config.yaml` & `flyweb_framework-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/bootstrap` & `flyweb_framework-0.4.1/bootstrap`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/requirements-dev.lock` & `flyweb_framework-0.4.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/requirements.lock` & `flyweb_framework-0.4.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/.github/workflows/python.yml` & `flyweb_framework-0.4.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/__init__.py` & `flyweb_framework-0.4.1/src/flyweb/__init__.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/_app.py` & `flyweb_framework-0.4.1/src/flyweb/_app.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/_flyweb.py` & `flyweb_framework-0.4.1/src/flyweb/_flyweb.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/_server.py` & `flyweb_framework-0.4.1/src/flyweb/_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
     async def run(self, *, task_status=anyio.TASK_STATUS_IGNORED) -> None:
         cfg = hypercorn.config.Config()
         cfg.bind = f"0.0.0.0:{self._port}"
         cfg.accesslog = logging.getLogger("hypercorn.accesslog")
         cfg.access_log_format = '%(h)s "%(R)s" %(s)s %(b)s "%(f)s" "%(a)s"'
         cfg.errorlog = logging.getLogger("hypercorn.errorlog")
+        # Don't wait too long for connections to close, as it seems to keep waiting for
+        # websocket connections forever.
+        cfg.graceful_timeout = 0.5  # seconds
 
         event = anyio.Event()
         async with anyio.create_task_group() as tg:
             await tg.start(self._serve, cfg, event)
             task_status.started()
             try:
                 await anyio.sleep_forever()
```

### Comparing `flyweb_framework-0.3.2/src/flyweb/components/_components.py` & `flyweb_framework-0.4.1/src/flyweb/components/_components.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/examples/counter/__main__.py` & `flyweb_framework-0.4.1/src/flyweb/examples/counter/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 
+import logging
+import sys
+
 import anyio
 import flyweb
 
 try:
     import hypercorn  # noqa: F401
 except ImportError:
     raise RuntimeError("install extras with flyweb[examples] to run this!") from None
@@ -28,8 +31,9 @@
 
 async def main():
     counter = Counter()
     await flyweb.Server(counter.render, port=8000).run()
 
 
 if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     anyio.run(main)
```

### Comparing `flyweb_framework-0.3.2/src/flyweb/examples/misc/__main__.py` & `flyweb_framework-0.4.1/src/flyweb/examples/misc/__main__.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/examples/stopwatch/__main__.py` & `flyweb_framework-0.4.1/src/flyweb/examples/stopwatch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3
 
 import datetime
+import logging
+import sys
 
 import anyio
 import flyweb
 
 try:
     import hypercorn  # noqa: F401
 except ImportError:
@@ -68,8 +70,9 @@
 
     async with anyio.create_task_group() as tg:
         tg.start_soon(_update_task, server)
         await server.run()
 
 
 if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     anyio.run(main)
```

### Comparing `flyweb_framework-0.3.2/src/flyweb/examples/todo/__main__.py` & `flyweb_framework-0.4.1/src/flyweb/examples/todo/__main__.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/static/index.html` & `flyweb_framework-0.4.1/src/flyweb/static/index.html`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/static/maquette.umd.js` & `flyweb_framework-0.4.1/src/flyweb/static/maquette.umd.js`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/static/script.js` & `flyweb_framework-0.4.1/src/flyweb/static/script.js`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/src/flyweb/static/socket.io.min.js` & `flyweb_framework-0.4.1/src/flyweb/static/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/tests/browser_test.py` & `flyweb_framework-0.4.1/tests/browser_test.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/tests/components_test.py` & `flyweb_framework-0.4.1/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/tests/flyweb_test.py` & `flyweb_framework-0.4.1/tests/flyweb_test.py`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/LICENSE` & `flyweb_framework-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flyweb_framework-0.3.2/README.md` & `flyweb_framework-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -36,20 +36,20 @@
     await flyweb.Server(counter.render, port=8000).run()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 There are a couple more examples under
-[flyweb/examples](https://github.com/girtsf/flyweb/tree/main/flyweb/examples).
+[src/flyweb/examples](https://github.com/girtsf/flyweb/tree/main/src/flyweb/examples).
 
 ## Try it out
 
 ```
-$ pip install 'flyweb[examples] @ git+https://github.com/girtsf/flyweb'
+$ pip install 'flyweb-framework[examples]'
 $ python -m flyweb.examples.todo
 ```
 
 Then go to http://localhost:8000/.
 
 ## Design
 
@@ -79,9 +79,14 @@
 users. Implementing per-user state would not be too difficult.
 
 Security: currently there is none, and it's probably pretty easy to crash the
 backend if you try.
 
 ## Status
 
-It works, at least for simple pages. The API is definitely not stable and will
-likely change as it evolves.
+* It works, and I've been successfully using it for a handful of different
+  internal tools.
+* Using stateful elements (e.g., checkboxes or textboxes) isn't yet as
+  streamlined as I would like. You have to instantiate (and reuse) objects that
+  keep track of the state
+  ([example](https://github.com/girtsf/flyweb/blob/f020e68acc766b1967ee4819a37de1d8d06b3775/src/flyweb/examples/todo/__main__.py#L78)).
+* The API is likely going to change as things evolve.
```

### Comparing `flyweb_framework-0.3.2/pyproject.toml` & `flyweb_framework-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [project]
 name = "flyweb-framework"
-version = "0.3.2"
+# Updated by CI when publishing.
+version = "0.4.1"
 description = "Immediate-mode web framework"
 authors = [
     { name = "Girts Folkmanis", email = "opensource@girts.me" }
 ]
 license = "MIT"
 dependencies = [
     "python-socketio>=5.7.2",
```

### Comparing `flyweb_framework-0.3.2/PKG-INFO` & `flyweb_framework-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flyweb-framework
-Version: 0.3.2
+Version: 0.4.1
 Summary: Immediate-mode web framework
 Project-URL: Homepage, https://github.com/girtsf/flyweb
 Author-email: Girts Folkmanis <opensource@girts.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.10
 Requires-Dist: anyio>=3.6
@@ -54,20 +54,20 @@
     await flyweb.Server(counter.render, port=8000).run()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 There are a couple more examples under
-[flyweb/examples](https://github.com/girtsf/flyweb/tree/main/flyweb/examples).
+[src/flyweb/examples](https://github.com/girtsf/flyweb/tree/main/src/flyweb/examples).
 
 ## Try it out
 
 ```
-$ pip install 'flyweb[examples] @ git+https://github.com/girtsf/flyweb'
+$ pip install 'flyweb-framework[examples]'
 $ python -m flyweb.examples.todo
 ```
 
 Then go to http://localhost:8000/.
 
 ## Design
 
@@ -97,9 +97,14 @@
 users. Implementing per-user state would not be too difficult.
 
 Security: currently there is none, and it's probably pretty easy to crash the
 backend if you try.
 
 ## Status
 
-It works, at least for simple pages. The API is definitely not stable and will
-likely change as it evolves.
+* It works, and I've been successfully using it for a handful of different
+  internal tools.
+* Using stateful elements (e.g., checkboxes or textboxes) isn't yet as
+  streamlined as I would like. You have to instantiate (and reuse) objects that
+  keep track of the state
+  ([example](https://github.com/girtsf/flyweb/blob/f020e68acc766b1967ee4819a37de1d8d06b3775/src/flyweb/examples/todo/__main__.py#L78)).
+* The API is likely going to change as things evolve.
```

