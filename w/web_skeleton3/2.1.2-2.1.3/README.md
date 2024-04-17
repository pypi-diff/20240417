# Comparing `tmp/web_skeleton3-2.1.2.tar.gz` & `tmp/web_skeleton3-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_skeleton3-2.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "web_skeleton3-2.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `web_skeleton3-2.1.2.tar` & `web_skeleton3-2.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      123 2024-03-21 08:08:05.245022 web_skeleton3-2.1.2/.gitignore
--rw-r--r--   0        0        0      411 2024-03-21 07:31:21.216446 web_skeleton3-2.1.2/CHANGES.txt
--rw-r--r--   0        0        0     1078 2024-03-21 07:31:21.216446 web_skeleton3-2.1.2/LICENSE.txt
--rw-r--r--   0        0        0       92 2024-03-21 07:31:21.216446 web_skeleton3-2.1.2/MANIFEST.in
--rw-r--r--   0        0        0      772 2024-04-11 17:28:17.586665 web_skeleton3-2.1.2/README.rst
--rw-r--r--   0        0        0     1112 2024-03-21 07:31:21.216446 web_skeleton3-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      197 2024-03-21 07:31:21.216446 web_skeleton3-2.1.2/setup.cfg
--rw-r--r--   0        0        0     1594 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/setup.py
--rw-r--r--   0        0        0     1565 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/PKG-INFO
--rw-r--r--   0        0        0     1699 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       58 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/entry_points.txt
--rw-r--r--   0        0        0        1 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/not-zip-safe
--rw-r--r--   0        0        0       44 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/requires.txt
--rw-r--r--   0        0        0       14 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3.egg-info/top_level.txt
--rw-r--r--   0        0        0       48 2024-04-11 17:36:08.084431 web_skeleton3-2.1.2/web_skeleton3/__init__.py
--rw-r--r--   0        0        0      281 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/README.txt
--rw-r--r--   0        0        0     1054 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/404.html
--rw-r--r--   0        0        0      381 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/browserconfig.xml
--rw-r--r--   0        0        0      766 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/favicon.ico
--rw-r--r--   0        0        0      229 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/humans.txt
--rw-r--r--   0        0        0     4029 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/icon.png
--rw-r--r--   0        0        0       78 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/robots.txt
--rw-r--r--   0        0        0      231 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/site.webmanifest
--rw-r--r--   0        0        0     5569 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/css/main.css
--rw-r--r--   0        0        0     6138 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/css/normalize.css
--rw-r--r--   0        0        0     8606 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/js/modernizr.js
--rw-r--r--   0        0        0      706 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/js/plugins.js
--rw-r--r--   0        0        0     1854 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/tile-wide.png
--rw-r--r--   0        0        0     3482 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/tile.png
--rw-r--r--   0        0        0     1428 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/favicon.ico
--rwxr-xr-x   0        0        0      222 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/genera_apple_icons.sh
--rw-r--r--   0        0        0     8657 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/icon.png
--rw-r--r--   0        0        0     2568 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/sample.svg
--rw-r--r--   0        0        0    17615 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/tile-wide.png
--rw-r--r--   0        0        0    25792 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/assets/logo/tile.png
--rw-r--r--   0        0        0       57 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/code/app/sample.js
--rw-r--r--   0        0        0      369 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/code/config.json
--rw-r--r--   0        0        0     1704 2024-03-21 09:45:25.822271 web_skeleton3-2.1.2/web_skeleton3/code/index.mako
--rw-r--r--   0        0        0       32 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/code/scss-mixins/README.txt
--rw-r--r--   0        0        0    19087 2024-04-11 17:26:35.266597 web_skeleton3-2.1.2/web_skeleton3/main.py
--rw-r--r--   0        0        0       72 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/setup/.gitignore
--rw-r--r--   0        0        0       84 2024-03-06 09:01:18.441953 web_skeleton3-2.1.2/web_skeleton3/setup/Makefile
--rw-r--r--   0        0        0      987 2024-04-11 17:28:52.058688 web_skeleton3-2.1.2/web_skeleton3/setup/README.rst
--rw-r--r--   0        0        0      493 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/setup/watch.json
--rwxr-xr-x   0        0        0       37 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/setup/watch.sh
--rw-r--r--   0        0        0      101 2024-03-21 07:31:21.220446 web_skeleton3-2.1.2/web_skeleton3/setup/web-skeleton3.ini
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 web_skeleton3-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-03-21 08:08:05.245022 web_skeleton3-2.1.3/.gitignore
+-rw-r--r--   0        0        0      411 2024-03-21 07:31:21.216446 web_skeleton3-2.1.3/CHANGES.txt
+-rw-r--r--   0        0        0     1078 2024-03-21 07:31:21.216446 web_skeleton3-2.1.3/LICENSE.txt
+-rw-r--r--   0        0        0       92 2024-03-21 07:31:21.216446 web_skeleton3-2.1.3/MANIFEST.in
+-rw-r--r--   0        0        0      772 2024-04-11 17:28:17.586665 web_skeleton3-2.1.3/README.rst
+-rw-r--r--   0        0        0     1112 2024-03-21 07:31:21.216446 web_skeleton3-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      197 2024-03-21 07:31:21.216446 web_skeleton3-2.1.3/setup.cfg
+-rw-r--r--   0        0        0     1594 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/setup.py
+-rw-r--r--   0        0        0     1565 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     1699 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       58 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        1 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/not-zip-safe
+-rw-r--r--   0        0        0       44 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/requires.txt
+-rw-r--r--   0        0        0       14 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3.egg-info/top_level.txt
+-rw-r--r--   0        0        0       48 2024-04-17 12:12:41.012165 web_skeleton3-2.1.3/web_skeleton3/__init__.py
+-rw-r--r--   0        0        0      281 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/README.txt
+-rw-r--r--   0        0        0     1054 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/404.html
+-rw-r--r--   0        0        0      381 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/browserconfig.xml
+-rw-r--r--   0        0        0      766 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/favicon.ico
+-rw-r--r--   0        0        0      229 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/humans.txt
+-rw-r--r--   0        0        0     4029 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/icon.png
+-rw-r--r--   0        0        0       78 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/robots.txt
+-rw-r--r--   0        0        0      231 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/site.webmanifest
+-rw-r--r--   0        0        0     5569 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/css/main.css
+-rw-r--r--   0        0        0     6138 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/css/normalize.css
+-rw-r--r--   0        0        0     8606 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/js/modernizr.js
+-rw-r--r--   0        0        0      706 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/js/plugins.js
+-rw-r--r--   0        0        0     1854 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/tile-wide.png
+-rw-r--r--   0        0        0     3482 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/tile.png
+-rw-r--r--   0        0        0     1428 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/favicon.ico
+-rwxr-xr-x   0        0        0      222 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/genera_apple_icons.sh
+-rw-r--r--   0        0        0     8657 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/icon.png
+-rw-r--r--   0        0        0     2568 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/sample.svg
+-rw-r--r--   0        0        0    17615 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/tile-wide.png
+-rw-r--r--   0        0        0    25792 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/assets/logo/tile.png
+-rw-r--r--   0        0        0       57 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/code/app/sample.js
+-rw-r--r--   0        0        0      369 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/code/config.json
+-rw-r--r--   0        0        0     1704 2024-03-21 09:45:25.822271 web_skeleton3-2.1.3/web_skeleton3/code/index.mako
+-rw-r--r--   0        0        0       32 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/code/scss-mixins/README.txt
+-rw-r--r--   0        0        0    19089 2024-04-17 12:00:33.016894 web_skeleton3-2.1.3/web_skeleton3/main.py
+-rw-r--r--   0        0        0       72 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/setup/.gitignore
+-rw-r--r--   0        0        0       84 2024-03-06 09:01:18.441953 web_skeleton3-2.1.3/web_skeleton3/setup/Makefile
+-rw-r--r--   0        0        0      987 2024-04-11 17:28:52.058688 web_skeleton3-2.1.3/web_skeleton3/setup/README.rst
+-rw-r--r--   0        0        0      493 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/setup/watch.json
+-rwxr-xr-x   0        0        0       37 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/setup/watch.sh
+-rw-r--r--   0        0        0      101 2024-03-21 07:31:21.220446 web_skeleton3-2.1.3/web_skeleton3/setup/web-skeleton3.ini
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 web_skeleton3-2.1.3/PKG-INFO
```

### Comparing `web_skeleton3-2.1.2/LICENSE.txt` & `web_skeleton3-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/README.rst` & `web_skeleton3-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/pyproject.toml` & `web_skeleton3-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/setup.py` & `web_skeleton3-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3.egg-info/PKG-INFO` & `web_skeleton3-2.1.3/web_skeleton3.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3.egg-info/SOURCES.txt` & `web_skeleton3-2.1.3/web_skeleton3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/404.html` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/404.html`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/favicon.ico` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/favicon.ico`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/icon.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/icon.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/css/main.css` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/css/main.css`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/css/normalize.css` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/css/normalize.css`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/js/modernizr.js` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/js/modernizr.js`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/static/h5bp/js/plugins.js` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/static/h5bp/js/plugins.js`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/tile-wide.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/tile-wide.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/h5bp/tile.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/h5bp/tile.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/logo/favicon.ico` & `web_skeleton3-2.1.3/web_skeleton3/assets/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/logo/icon.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/logo/icon.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/logo/sample.svg` & `web_skeleton3-2.1.3/web_skeleton3/assets/logo/sample.svg`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/logo/tile-wide.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/logo/tile-wide.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/assets/logo/tile.png` & `web_skeleton3-2.1.3/web_skeleton3/assets/logo/tile.png`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/code/index.mako` & `web_skeleton3-2.1.3/web_skeleton3/code/index.mako`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/web_skeleton3/main.py` & `web_skeleton3-2.1.3/web_skeleton3/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
                 except Exception as error:
                     print("ERROR processing filename '%s': %s" % (scss_file, error))
 
             css = Bundle(
                 css_bundle,
                 *scss_bundle,
                 #filters='cssutils,cssrewrite',
-                filters='cleancss',
+                # filters='cleancss',
                 output='packed.css'
             )
             assets_env.register('css', css)
 
         return assets_env
 
     def get_assets_top_js_env(self, code_path, output_path):
```

### Comparing `web_skeleton3-2.1.2/web_skeleton3/setup/README.rst` & `web_skeleton3-2.1.3/web_skeleton3/setup/README.rst`

 * *Files identical despite different names*

### Comparing `web_skeleton3-2.1.2/PKG-INFO` & `web_skeleton3-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web_skeleton3
-Version: 2.1.2
+Version: 2.1.3
 Summary: Static html code generator.
 Author-email: rmm <rosa.martinez@artgins.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

