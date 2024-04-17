# Comparing `tmp/trame-components-2.3.0.tar.gz` & `tmp/trame-components-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-components-2.3.0.tar", last modified: Tue Apr 16 00:01:04 2024, max compression
+gzip compressed data, was "trame-components-2.3.1.tar", last modified: Wed Apr 17 20:45:11 2024, max compression
```

## Comparing `trame-components-2.3.0.tar` & `trame-components-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-16 00:00:48.000000 trame-components-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 00:00:48.000000 trame-components-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-16 00:01:04.958520 trame-components-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-16 00:00:48.000000 trame-components-2.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-16 00:01:04.958520 trame-components-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 00:00:48.000000 trame-components-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.954520 trame-components-2.3.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.954520 trame-components-2.3.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/modules/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/module/
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/module/serve/
--rw-r--r--   0 root         (0) root         (0)   227244 2024-04-16 00:01:01.000000 trame-components-2.3.0/trame_components/module/serve/trame-components.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15929 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.239639 trame-components-2.3.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-17 20:44:54.000000 trame-components-2.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-17 20:44:54.000000 trame-components-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-17 20:45:11.239639 trame-components-2.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-17 20:44:54.000000 trame-components-2.3.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-17 20:45:11.239639 trame-components-2.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:44:54.000000 trame-components-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/modules/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/module/
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/module/serve/
+-rw-r--r--   0 root         (0) root         (0)   227297 2024-04-17 20:45:07.000000 trame-components-2.3.1/trame_components/module/serve/trame-components.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.239639 trame-components-2.3.1/trame_components/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15929 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/top_level.txt
```

### Comparing `trame-components-2.3.0/LICENSE` & `trame-components-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.0/PKG-INFO` & `trame-components-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.3.0
+Version: 2.3.1
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.3.0/README.rst` & `trame-components-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.0/setup.cfg` & `trame-components-2.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-components
-version = 2.3.0
+version = 2.3.1
 description = Core components for trame widgets
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-components-2.3.0/trame_components/LICENSE` & `trame-components-2.3.1/trame_components/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.0/trame_components/module/serve/trame-components.umd.js` & `trame-components-2.3.1/trame_components/module/serve/trame-components.umd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1272,23 +1272,30 @@
             setup(e, {
                 emit: t
             }) {
                 const r = V9("trame"),
                     n = z9(null);
 
                 function a() {
-                    const c = n.value.getBoundingClientRect(),
-                        s = window.devicePixelRatio,
-                        u = 96 * s,
-                        i = {
-                            size: c,
-                            pixelRatio: s,
-                            dpi: u
-                        };
-                    e.name && (i.name = e.name), r && r.state.set(e.name, i), t("change", i)
+                    const {
+                        x: c,
+                        y: s,
+                        width: u,
+                        height: i
+                    } = n.value.getBoundingClientRect(), f = {
+                        x: c,
+                        y: s,
+                        width: u,
+                        height: i
+                    }, g = window.devicePixelRatio, l = 96 * g, p = {
+                        size: f,
+                        pixelRatio: g,
+                        dpi: l
+                    };
+                    e.name && (p.name = e.name), r && r.state.set(e.name, p), t("change", p)
                 }
                 const o = new ResizeObserver(a);
                 return H9(() => {
                     o.observe(n.value)
                 }), I9(() => {
                     o.unobserve(n.value)
                 }), {
```

### Comparing `trame-components-2.3.0/trame_components/widgets/trame.py` & `trame-components-2.3.1/trame_components/widgets/trame.py`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.0/trame_components.egg-info/PKG-INFO` & `trame-components-2.3.1/trame_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.3.0
+Version: 2.3.1
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.3.0/trame_components.egg-info/SOURCES.txt` & `trame-components-2.3.1/trame_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

