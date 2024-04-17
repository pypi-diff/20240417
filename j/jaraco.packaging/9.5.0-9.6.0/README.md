# Comparing `tmp/jaraco.packaging-9.5.0.tar.gz` & `tmp/jaraco_packaging-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.packaging-9.5.0.tar", last modified: Sun Mar 31 23:08:12 2024, max compression
+gzip compressed data, was "jaraco_packaging-9.6.0.tar", last modified: Wed Apr 17 02:52:43 2024, max compression
```

## Comparing `jaraco.packaging-9.5.0.tar` & `jaraco_packaging-9.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.236592 jaraco.packaging-9.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.232592 jaraco.packaging-9.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.232592 jaraco.packaging-9.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-31 23:08:12.236592 jaraco.packaging-9.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.232592 jaraco.packaging-9.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.228592 jaraco.packaging-9.5.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.236592 jaraco.packaging-9.5.0/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/jaraco/packaging/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:08:12.236592 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-31 23:08:12.000000 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-31 23:08:12.000000 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:08:12.000000 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-31 23:08:12.000000 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 23:08:12.000000 jaraco.packaging-9.5.0/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-31 23:08:12.236592 jaraco.packaging-9.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 23:07:48.000000 jaraco.packaging-9.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.410340 jaraco_packaging-9.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.406340 jaraco_packaging-9.6.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 02:52:43.000000 jaraco_packaging-9.6.0/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 02:52:43.414340 jaraco_packaging-9.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 02:52:24.000000 jaraco_packaging-9.6.0/tox.ini
```

### Comparing `jaraco.packaging-9.5.0/.github/workflows/main.yml` & `jaraco_packaging-9.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/LICENSE` & `jaraco_packaging-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/NEWS.rst` & `jaraco_packaging-9.6.0/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v9.6.0
+======
+
+Features
+--------
+
+- Add support for other metadata fields since pyproject.toml shuffles things around. (#17)
+
+
 v9.5.0
 ======
 
 Features
 --------
 
 - Add ``metadata.load`` for loading metadata from a source dir with support for a BUILD_ENVIRONMENT setting. Set BUILD_ENVIRONMENT=current to bypass isolation when loading metadata. Ref pypa/build#556. (#556)
```

### Comparing `jaraco.packaging-9.5.0/PKG-INFO` & `jaraco_packaging-9.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.5.0
+Version: 9.6.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,15 @@
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Tools for packaging.
 
+
 sphinx
 ======
 
 This package provides a Sphinx extension that will inject into the config
 the following values from the project's package metadata (as presented by
 distutils):
 
@@ -70,20 +71,34 @@
 To enable, include 'jaraco.packaging' in the requirements and add
 'jaraco.packaging.sphinx' to the list of extensions in a Sphinx config
 file::
 
     extensions=['jaraco.packaging.sphinx']
 
 The extension by default builds the project in an isolated environment in
-order to extract the metadata. To build the documentation offline,
+order to extract the metadata. For offline builds, set
+``BUILD_ENVIRONMENT=current`` and ensure the build dependencies are
+met in the current environment.
+
+Deprecated: To build the documentation offline,
 provide an already built wheel by setting the environment variable
-``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of the existing wheel.
+``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of an existing wheel.
+
 
 make-tree
 =========
 
 A utility for taking output from ``pipdeptree --json`` and producing a tree
 rooted at a given package.
 
 Usage::
 
     pipdeptree --json | python -m jaraco.packaging.make-tree mypkg
+
+
+metadata
+=========
+
+A wrapper around ``build.util.project_wheel_metadata`` to enable dowstream
+packagers to indicate that they need an isolated build. Set the environment
+variable ``BUILD_ENVIRONMENT=current`` to bypass build isolation and use the
+current isolation for loading metadata from a project.
```

### Comparing `jaraco.packaging-9.5.0/README.rst` & `jaraco_packaging-9.6.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -15,14 +15,15 @@
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Tools for packaging.
 
+
 sphinx
 ======
 
 This package provides a Sphinx extension that will inject into the config
 the following values from the project's package metadata (as presented by
 distutils):
 
@@ -36,20 +37,34 @@
 To enable, include 'jaraco.packaging' in the requirements and add
 'jaraco.packaging.sphinx' to the list of extensions in a Sphinx config
 file::
 
     extensions=['jaraco.packaging.sphinx']
 
 The extension by default builds the project in an isolated environment in
-order to extract the metadata. To build the documentation offline,
+order to extract the metadata. For offline builds, set
+``BUILD_ENVIRONMENT=current`` and ensure the build dependencies are
+met in the current environment.
+
+Deprecated: To build the documentation offline,
 provide an already built wheel by setting the environment variable
-``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of the existing wheel.
+``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of an existing wheel.
+
 
 make-tree
 =========
 
 A utility for taking output from ``pipdeptree --json`` and producing a tree
 rooted at a given package.
 
 Usage::
 
     pipdeptree --json | python -m jaraco.packaging.make-tree mypkg
+
+
+metadata
+=========
+
+A wrapper around ``build.util.project_wheel_metadata`` to enable dowstream
+packagers to indicate that they need an isolated build. Set the environment
+variable ``BUILD_ENVIRONMENT=current`` to bypass build isolation and use the
+current isolation for loading metadata from a project.
```

### Comparing `jaraco.packaging-9.5.0/docs/conf.py` & `jaraco_packaging-9.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/jaraco/packaging/make-tree.py` & `jaraco_packaging-9.6.0/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/jaraco/packaging/sphinx.py` & `jaraco_packaging-9.6.0/jaraco/packaging/sphinx.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 to conf.py, and the setup hook does the rest.
 
 >>> 'setup' in globals()
 True
 """
 
 import os
+import re
 import warnings
 from importlib import metadata
 from typing import ClassVar
 
 import docutils.statemachine
 import domdf_python_tools.stringlist
 import sphinx.util.docutils
@@ -111,16 +112,35 @@
     Replace values in app.config from package metadata
     """
     # for now, assume project root is one level up
     root = os.path.join(app.confdir, '..')
     meta = _load_metadata_from_wheel() or load(root)
     app.config.project = meta['Name']
     app.config.version = app.config.release = meta['Version']
-    app.config.package_url = meta['Home-page']
-    app.config.author = app.config.copyright = meta['Author']
+    app.config.package_url = hunt_down_url(meta)
+    app.config.author = app.config.copyright = extract_author(meta)
+
+
+def hunt_down_url(meta):
+    """
+    Given project metadata, figure out what the package URL is.
+    """
+    return meta['Home-page'] or get_best(meta.get_all('Project-URL'))
+
+
+def get_best(project_urls):
+    lookup = dict(url.split(', ') for url in project_urls)
+    return lookup.get('Source') or lookup.get('Homepage')
+
+
+def extract_author(meta):
+    """
+    Given project metadata, figure out who the author is.
+    """
+    return meta['Author'] or re.search(r'"(.+)"', meta['Author-email']).group(1)
 
 
 def configure_substitutions(app):
     epilogs = app.config.rst_epilog, f'.. |project| replace:: {app.config.project}'
     app.config.rst_epilog = '\n'.join(filter(None, epilogs))
```

### Comparing `jaraco.packaging-9.5.0/jaraco.packaging.egg-info/PKG-INFO` & `jaraco_packaging-9.6.0/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.5.0
+Version: 9.6.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,15 @@
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Tools for packaging.
 
+
 sphinx
 ======
 
 This package provides a Sphinx extension that will inject into the config
 the following values from the project's package metadata (as presented by
 distutils):
 
@@ -70,20 +71,34 @@
 To enable, include 'jaraco.packaging' in the requirements and add
 'jaraco.packaging.sphinx' to the list of extensions in a Sphinx config
 file::
 
     extensions=['jaraco.packaging.sphinx']
 
 The extension by default builds the project in an isolated environment in
-order to extract the metadata. To build the documentation offline,
+order to extract the metadata. For offline builds, set
+``BUILD_ENVIRONMENT=current`` and ensure the build dependencies are
+met in the current environment.
+
+Deprecated: To build the documentation offline,
 provide an already built wheel by setting the environment variable
-``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of the existing wheel.
+``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of an existing wheel.
+
 
 make-tree
 =========
 
 A utility for taking output from ``pipdeptree --json`` and producing a tree
 rooted at a given package.
 
 Usage::
 
     pipdeptree --json | python -m jaraco.packaging.make-tree mypkg
+
+
+metadata
+=========
+
+A wrapper around ``build.util.project_wheel_metadata`` to enable dowstream
+packagers to indicate that they need an isolated build. Set the environment
+variable ``BUILD_ENVIRONMENT=current`` to bypass build isolation and use the
+current isolation for loading metadata from a project.
```

### Comparing `jaraco.packaging-9.5.0/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco_packaging-9.6.0/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/pytest.ini` & `jaraco_packaging-9.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/setup.cfg` & `jaraco_packaging-9.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.5.0/tox.ini` & `jaraco_packaging-9.6.0/tox.ini`

 * *Files identical despite different names*

