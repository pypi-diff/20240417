# Comparing `tmp/pyaction-0.5.4.tar.gz` & `tmp/pyaction-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.5.4.tar", last modified: Mon Apr 15 06:32:23 2024, max compression
+gzip compressed data, was "pyaction-0.5.5.tar", last modified: Wed Apr 17 19:08:36 2024, max compression
```

## Comparing `pyaction-0.5.4.tar` & `pyaction-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 06:32:18.000000 pyaction-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 06:32:18.000000 pyaction-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-15 06:32:23.023181 pyaction-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 06:32:18.000000 pyaction-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.019181 pyaction-0.5.4/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.019181 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:32:23.023181 pyaction-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 19:08:27.000000 pyaction-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 19:08:27.000000 pyaction-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-17 19:08:36.002700 pyaction-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-17 19:08:27.000000 pyaction-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:35.998700 pyaction-0.5.5/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/issues/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:35.998700 pyaction-0.5.5/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:08:36.002700 pyaction-0.5.5/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 19:08:35.000000 pyaction-0.5.5/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-17 19:08:27.000000 pyaction-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:08:36.002700 pyaction-0.5.5/setup.cfg
```

### Comparing `pyaction-0.5.4/LICENSE` & `pyaction-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.4/PKG-INFO` & `pyaction-0.5.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.4
+Version: 0.5.5
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,23 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://pyaction.imsadra.me
 Project-URL: Repository, https://github.com/lnxpy/pyaction
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: copier>=9.2
 Requires-Dist: click>=8.1
 Requires-Dist: pygithub>=2.3.0
 Requires-Dist: markdown-to-json==2.1.0
@@ -38,15 +47,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=white&label=Python) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.4/README.md` & `pyaction-0.5.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=white&label=Python) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.4/pyaction/cli.py` & `pyaction-0.5.5/pyaction/cli.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.4/pyaction/io.py` & `pyaction-0.5.5/pyaction/io.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.4/pyaction/issues/connector.py` & `pyaction-0.5.5/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.4/pyaction/template/copier.yml` & `pyaction-0.5.5/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.4/pyaction.egg-info/PKG-INFO` & `pyaction-0.5.5/pyaction.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.4
+Version: 0.5.5
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,23 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://pyaction.imsadra.me
 Project-URL: Repository, https://github.com/lnxpy/pyaction
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: copier>=9.2
 Requires-Dist: click>=8.1
 Requires-Dist: pygithub>=2.3.0
 Requires-Dist: markdown-to-json==2.1.0
@@ -38,15 +47,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=white&label=Python) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.4/pyaction.egg-info/SOURCES.txt` & `pyaction-0.5.5/pyaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

