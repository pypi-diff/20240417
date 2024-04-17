# Comparing `tmp/jaraco_packaging-9.6.0.tar.gz` & `tmp/jaraco_packaging-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_packaging-9.6.0.tar", last modified: Wed Apr 17 02:52:43 2024, max compression
+gzip compressed data, was "jaraco_packaging-9.7.0.tar", last modified: Wed Apr 17 02:58:44 2024, max compression
```

## Comparing `jaraco_packaging-9.6.0.tar` & `jaraco_packaging-9.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.406340 jaraco_packaging-9.6.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 02:58:44.819431 jaraco_packaging-9.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/tox.ini
```

### Comparing `jaraco_packaging-9.6.0/.github/workflows/main.yml` & `jaraco_packaging-9.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/LICENSE` & `jaraco_packaging-9.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/NEWS.rst` & `jaraco_packaging-9.7.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v9.7.0
+======
+
+Features
+--------
+
+- Configure Sphinx earlier in 'config-inited', allowing other etxensions to rely on the produced values. (#16)
+
+
 v9.6.0
 ======
 
 Features
 --------
 
 - Add support for other metadata fields since pyproject.toml shuffles things around. (#17)
```

### Comparing `jaraco_packaging-9.6.0/PKG-INFO` & `jaraco_packaging-9.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.6.0
+Version: 9.7.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco_packaging-9.6.0/README.rst` & `jaraco_packaging-9.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/docs/conf.py` & `jaraco_packaging-9.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/jaraco/packaging/make-tree.py` & `jaraco_packaging-9.7.0/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/jaraco/packaging/sphinx.py` & `jaraco_packaging-9.7.0/jaraco/packaging/sphinx.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from jaraco.context import suppress
 
 from .metadata import load
 
 
 def setup(app):
     app.add_config_value('package_url', '', '')
-    app.connect('builder-inited', load_config_from_setup)
-    app.connect('builder-inited', configure_substitutions)
+    app.connect('config-inited', load_config_from_setup)
+    app.connect('config-inited', configure_substitutions)
     app.connect('html-page-context', add_package_url)
     app.add_directive("sidebar-links", SidebarLinksDirective)
     return dict(version=metadata.version('jaraco.packaging'), parallel_read_safe=True)
 
 
 class SidebarLinksDirective(sphinx.util.docutils.SphinxDirective):
     """
@@ -103,25 +103,25 @@
         "use BUILD_ENVIRONMENT=current instead",
         DeprecationWarning,
     )
     (dist,) = metadata.distributions(path=[wheel])
     return dist.metadata
 
 
-def load_config_from_setup(app):
+def load_config_from_setup(app, config):
     """
     Replace values in app.config from package metadata
     """
     # for now, assume project root is one level up
     root = os.path.join(app.confdir, '..')
     meta = _load_metadata_from_wheel() or load(root)
-    app.config.project = meta['Name']
-    app.config.version = app.config.release = meta['Version']
-    app.config.package_url = hunt_down_url(meta)
-    app.config.author = app.config.copyright = extract_author(meta)
+    config.project = meta['Name']
+    config.version = config.release = meta['Version']
+    config.package_url = hunt_down_url(meta)
+    config.author = config.copyright = extract_author(meta)
 
 
 def hunt_down_url(meta):
     """
     Given project metadata, figure out what the package URL is.
     """
     return meta['Home-page'] or get_best(meta.get_all('Project-URL'))
@@ -135,14 +135,14 @@
 def extract_author(meta):
     """
     Given project metadata, figure out who the author is.
     """
     return meta['Author'] or re.search(r'"(.+)"', meta['Author-email']).group(1)
 
 
-def configure_substitutions(app):
-    epilogs = app.config.rst_epilog, f'.. |project| replace:: {app.config.project}'
-    app.config.rst_epilog = '\n'.join(filter(None, epilogs))
+def configure_substitutions(app, config):
+    epilogs = config.rst_epilog, f'.. |project| replace:: {config.project}'
+    config.rst_epilog = '\n'.join(filter(None, epilogs))
 
 
 def add_package_url(app, pagename, templatename, context, doctree):
     context['package_url'] = app.config.package_url
```

### Comparing `jaraco_packaging-9.6.0/jaraco.packaging.egg-info/PKG-INFO` & `jaraco_packaging-9.7.0/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.6.0
+Version: 9.7.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco_packaging-9.6.0/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco_packaging-9.7.0/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/pytest.ini` & `jaraco_packaging-9.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/setup.cfg` & `jaraco_packaging-9.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.6.0/tox.ini` & `jaraco_packaging-9.7.0/tox.ini`

 * *Files identical despite different names*

