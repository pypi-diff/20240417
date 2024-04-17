# Comparing `tmp/raydar-0.2.0.tar.gz` & `tmp/raydar-0.2.1.tar.gz`

## Comparing `raydar-0.2.0.tar` & `raydar-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 raydar-0.2.0/js/build.js
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 raydar-0.2.0/js/package.json
--rw-r--r--   0        0        0   114300 2020-02-02 00:00:00.000000 raydar-0.2.0/js/yarn.lock
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 raydar-0.2.0/js/src/index.css
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 raydar-0.2.0/js/src/index.html
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 raydar-0.2.0/js/src/index.js
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 raydar-0.2.0/js/src/layouts/default.json
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/demo.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/server.py
--rw-r--r--   0        0        0   101519 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/static/index.css
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/static/index.html
--rw-r--r--   0        0        0  4275119 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/static/index.js
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/dashboard/static/layouts/default.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/task_tracker/__init__.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/task_tracker/schema.py
--rw-r--r--   0        0        0    16779 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/task_tracker/task_tracker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/tests/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/tests/conftest.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 raydar-0.2.0/raydar/tests/test_task_tracker.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 raydar-0.2.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 raydar-0.2.0/LICENSE
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 raydar-0.2.0/README.md
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 raydar-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 raydar-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 raydar-0.2.1/js/build.js
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 raydar-0.2.1/js/package.json
+-rw-r--r--   0        0        0   114298 2020-02-02 00:00:00.000000 raydar-0.2.1/js/yarn.lock
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 raydar-0.2.1/js/src/index.css
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 raydar-0.2.1/js/src/index.html
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 raydar-0.2.1/js/src/index.js
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 raydar-0.2.1/js/src/layouts/default.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/demo.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/server.py
+-rw-r--r--   0        0        0   101519 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/static/index.css
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/static/index.html
+-rw-r--r--   0        0        0  4275119 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/static/index.js
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/dashboard/static/layouts/default.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/task_tracker/__init__.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/task_tracker/schema.py
+-rw-r--r--   0        0        0    16779 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/task_tracker/task_tracker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/tests/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/tests/conftest.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 raydar-0.2.1/raydar/tests/test_task_tracker.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 raydar-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 raydar-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 raydar-0.2.1/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 raydar-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    24484 2020-02-02 00:00:00.000000 raydar-0.2.1/PKG-INFO
```

### Comparing `raydar-0.2.0/js/build.js` & `raydar-0.2.1/js/build.js`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/js/package.json` & `raydar-0.2.1/js/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'author'": "'OpenSource@Point72.com'", "'version'": "'0.2.1'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "author": "OSPO@Point72.com",
+    "author": "OpenSource@Point72.com",
     "dependencies": {
         "@finos/perspective": "^2.5.0",
         "@finos/perspective-viewer": "^2.5.0",
         "@finos/perspective-viewer-d3fc": "^2.5.0",
         "@finos/perspective-viewer-datagrid": "^2.5.0",
         "@finos/perspective-workspace": "^2.5.0"
     },
@@ -29,9 +29,9 @@
         "fix": "prettier --write  \"src/*.js\" \"src/*.html\" \"src/*.css\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/*.js\" \"src/*.html\" \"src/*.css\" \"*.js\" \"*.json\"",
         "test": ":",
         "watch": "npm-run-all -p watch:*",
         "watch:esbuild": "yarn build:esbuild --watch"
     },
     "type": "module",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `raydar-0.2.0/js/yarn.lock` & `raydar-0.2.1/js/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2326,17 +2326,17 @@
 
 supports-preserve-symlinks-flag@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz#6eda4bd344a3c94aea376d4cc31bc77311039e09"
   integrity sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==
 
 tar@^6.1.11:
-  version "6.1.15"
-  resolved "https://registry.yarnpkg.com/tar/-/tar-6.1.15.tgz#c9738b0b98845a3b344d334b8fa3041aaba53a69"
-  integrity sha512-/zKt9UyngnxIT/EAGYuxaMYgOIJiP81ab9ZfkILq4oNLPFX50qyYmu7jRj9qeXoxmJHjGlbH0+cm2uy1WCs10A==
+  version "6.2.1"
+  resolved "https://registry.yarnpkg.com/tar/-/tar-6.2.1.tgz#717549c541bc3c2af15751bea94b1dd068d4b03a"
+  integrity sha512-DZ4yORTwrbTj/7MZYq2w+/ZFdI6OZ/f9SFHR+71gIVUZhOQPHzVCLpvRnPgyaMpfWxxk/4ONva3GQSyNIKRv6A==
   dependencies:
     chownr "^2.0.0"
     fs-minipass "^2.0.0"
     minipass "^5.0.0"
     minizlib "^2.1.1"
     mkdirp "^1.0.3"
     yallist "^4.0.0"
```

### Comparing `raydar-0.2.0/js/src/index.html` & `raydar-0.2.1/js/src/index.html`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/js/src/index.js` & `raydar-0.2.1/js/src/index.js`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/dashboard/demo.py` & `raydar-0.2.1/raydar/dashboard/demo.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/dashboard/server.py` & `raydar-0.2.1/raydar/dashboard/server.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/dashboard/static/index.css` & `raydar-0.2.1/raydar/dashboard/static/index.css`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/dashboard/static/index.html` & `raydar-0.2.1/raydar/dashboard/static/index.html`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/dashboard/static/index.js` & `raydar-0.2.1/raydar/dashboard/static/index.js`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/task_tracker/schema.py` & `raydar-0.2.1/raydar/task_tracker/schema.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/task_tracker/task_tracker.py` & `raydar-0.2.1/raydar/task_tracker/task_tracker.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/tests/conftest.py` & `raydar-0.2.1/raydar/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/raydar/tests/test_task_tracker.py` & `raydar-0.2.1/raydar/tests/test_task_tracker.py`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/.gitignore` & `raydar-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/LICENSE` & `raydar-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raydar-0.2.0/README.md` & `raydar-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 ```python
 task_tracker = RayTaskTracker(enable_perspective_dashboard=True)
 ```
 
 ![Example](docs/img/example_perspective_dashboard.gif)
 
-# Recreating custom perspective views is supported.
+## Create/Store Custom Views
 From the developer console, save your workspace layout locally.
 
 ```javascript
 let workspace = document.getElementById('perspective-workspace');
 
 // Save the current layout
 workspace.save().then(config => {
@@ -110,19 +110,21 @@
 
     // Append the link to the document body and click it to start the download
     document.body.appendChild(link);
     link.click();
     document.body.removeChild(link);
 });
 ```
+
 Then, move this json file to `js/src/layouts/default.json`.
 
 ![Example](docs/img/example_perspective_dashboard_layouts.gif)
 
-# The data available to you includes much of what Ray's GCS tracks, and also allows for user defined metadata per task.
+## Expose Ray GCS Information
+The data available to you includes much of what Ray's GCS tracks, and also allows for user defined metadata per task.
 
 Specifically, tracked fields include:
  * `task_id`
  * `user_defined_metadata`
  * `attempt_number`
  * `name`
  * `state`
@@ -144,15 +146,15 @@
  * `start_time_ms`
  * `end_time_ms`
  * `task_log_info`
  * `error_message`
 
 ![Example](docs/img/example_task_metadata.gif)
 
-# Custom data sources and update logic are also suported
+## Custom Sources / Update Logic
 
 The proxy server helpd by the `RayTaskTracker` is exposed via the `.proxy_server()` property, meaning we can create new tables as follows:
 
 
 ```python
 task_tracker = RayTaskTracker(enable_perspective_dashboard=True)
 proxy_server = task_tracker.proxy_server()
@@ -164,22 +166,23 @@
         "metric_name": "str",
         "value": "float",
         "timestamp": "datetime",
     },
 )
 ```
 
+### Example: Live Per-Node Training Loss Metrics
+
 If a user were to then update this table with data coming from, for example, a pytorch model training loop with metrics:
 
 ```python
 def my_model_training_loop()
 
 	for epoch in range(num_epochs):
-
-    # ... my training code here ...
+        # ... my training code here ...
 
 		data = dict(
 			node_id=ray.get_runtime_context().get_node_id(),
 			metric_name="loss",
 			value=loss.item(),
 			timestamp=time.time(),
 		)
@@ -192,19 +195,19 @@
 
 ## Installation
 `raydar` can be installed via [pip](https://pip.pypa.io) or [conda](https://docs.conda.io/en/latest/), the two primary package managers for the Python ecosystem.
 
 To install `raydar` via **pip**, run this command in your terminal:
 
 ```bash
-    pip install raydar
+pip install raydar
 ```
 
 To install `raydar` via **conda**, run this command in your terminal:
 
 ```bash
-    conda install raydar -c conda-forge
+conda install raydar -c conda-forge
 ```
 
 ## License
 This software is licensed under the Apache 2.0 license. See the [LICENSE](LICENSE) file for details.
```

### Comparing `raydar-0.2.0/pyproject.toml` & `raydar-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     "hatch-jupyter-builder",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "raydar"
 description = "A perspective powered, user editable ray dashboard via ray serve"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
-    { name = "Point72", email = "OSPO@Point72.com" },
+    { name = "Point72", email = "OpenSource@Point72.com" },
 ]
 keywords = [
     "perspective",
     "ray",
     "dashboard",
     "dataviz",
     "data visualization",
@@ -40,29 +40,29 @@
 ]
 
 dependencies = [
     "coolname",
     "fastapi",
     "packaging",
     "perspective-python",
-    "pydantic<2",
+    "polars",
+    "pyarrow",
+    "pydantic",
     "ray[serve]>=2.8",
 ]
 
 [project.optional-dependencies]
 develop = [
     "bump2version>=1.0.0",
     "check-manifest",
     "hatchling",
     "hatch-jupyter-builder",
     "isort",
     "ruff>=0.3,<0.4",
     # Test deps
-    "polars",
-    "pyarrow",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-sugar",
 ]
 
 test = [
@@ -140,15 +140,15 @@
 path = "js"
 build_cmd = "build"
 npm = "yarn"
 
 [tool.isort]
 combine_as_imports = true
 include_trailing_comma = true
-line_length = 120
+line_length = 150
 profile = "black"
 default_section = "THIRDPARTY"
 sections = "FUTURE,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 known_first_party = "raydar"
 
 [tool.ruff]
 line-length = 150
```

### Comparing `raydar-0.2.0/PKG-INFO` & `raydar-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: raydar
-Version: 0.2.0
+Version: 0.2.1
 Summary: A perspective powered, user editable ray dashboard via ray serve
 Project-URL: Repository, https://github.com/point72/raydar
 Project-URL: Homepage, https://github.com/point72/raydar
-Author-email: Point72 <OSPO@Point72.com>
+Author-email: Point72 <OpenSource@Point72.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -220,24 +220,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: coolname
 Requires-Dist: fastapi
 Requires-Dist: packaging
 Requires-Dist: perspective-python
-Requires-Dist: pydantic<2
+Requires-Dist: polars
+Requires-Dist: pyarrow
+Requires-Dist: pydantic
 Requires-Dist: ray[serve]>=2.8
 Provides-Extra: develop
 Requires-Dist: bump2version>=1.0.0; extra == 'develop'
 Requires-Dist: check-manifest; extra == 'develop'
 Requires-Dist: hatch-jupyter-builder; extra == 'develop'
 Requires-Dist: hatchling; extra == 'develop'
 Requires-Dist: isort; extra == 'develop'
-Requires-Dist: polars; extra == 'develop'
-Requires-Dist: pyarrow; extra == 'develop'
 Requires-Dist: pytest; extra == 'develop'
 Requires-Dist: pytest-asyncio; extra == 'develop'
 Requires-Dist: pytest-cov; extra == 'develop'
 Requires-Dist: pytest-sugar; extra == 'develop'
 Requires-Dist: ruff<0.4,>=0.3; extra == 'develop'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
@@ -333,15 +333,15 @@
 
 ```python
 task_tracker = RayTaskTracker(enable_perspective_dashboard=True)
 ```
 
 ![Example](docs/img/example_perspective_dashboard.gif)
 
-# Recreating custom perspective views is supported.
+## Create/Store Custom Views
 From the developer console, save your workspace layout locally.
 
 ```javascript
 let workspace = document.getElementById('perspective-workspace');
 
 // Save the current layout
 workspace.save().then(config => {
@@ -358,19 +358,21 @@
 
     // Append the link to the document body and click it to start the download
     document.body.appendChild(link);
     link.click();
     document.body.removeChild(link);
 });
 ```
+
 Then, move this json file to `js/src/layouts/default.json`.
 
 ![Example](docs/img/example_perspective_dashboard_layouts.gif)
 
-# The data available to you includes much of what Ray's GCS tracks, and also allows for user defined metadata per task.
+## Expose Ray GCS Information
+The data available to you includes much of what Ray's GCS tracks, and also allows for user defined metadata per task.
 
 Specifically, tracked fields include:
  * `task_id`
  * `user_defined_metadata`
  * `attempt_number`
  * `name`
  * `state`
@@ -392,15 +394,15 @@
  * `start_time_ms`
  * `end_time_ms`
  * `task_log_info`
  * `error_message`
 
 ![Example](docs/img/example_task_metadata.gif)
 
-# Custom data sources and update logic are also suported
+## Custom Sources / Update Logic
 
 The proxy server helpd by the `RayTaskTracker` is exposed via the `.proxy_server()` property, meaning we can create new tables as follows:
 
 
 ```python
 task_tracker = RayTaskTracker(enable_perspective_dashboard=True)
 proxy_server = task_tracker.proxy_server()
@@ -412,22 +414,23 @@
         "metric_name": "str",
         "value": "float",
         "timestamp": "datetime",
     },
 )
 ```
 
+### Example: Live Per-Node Training Loss Metrics
+
 If a user were to then update this table with data coming from, for example, a pytorch model training loop with metrics:
 
 ```python
 def my_model_training_loop()
 
 	for epoch in range(num_epochs):
-
-    # ... my training code here ...
+        # ... my training code here ...
 
 		data = dict(
 			node_id=ray.get_runtime_context().get_node_id(),
 			metric_name="loss",
 			value=loss.item(),
 			timestamp=time.time(),
 		)
@@ -440,19 +443,19 @@
 
 ## Installation
 `raydar` can be installed via [pip](https://pip.pypa.io) or [conda](https://docs.conda.io/en/latest/), the two primary package managers for the Python ecosystem.
 
 To install `raydar` via **pip**, run this command in your terminal:
 
 ```bash
-    pip install raydar
+pip install raydar
 ```
 
 To install `raydar` via **conda**, run this command in your terminal:
 
 ```bash
-    conda install raydar -c conda-forge
+conda install raydar -c conda-forge
 ```
 
 ## License
 This software is licensed under the Apache 2.0 license. See the [LICENSE](LICENSE) file for details.
```

