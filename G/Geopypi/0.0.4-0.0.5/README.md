# Comparing `tmp/Geopypi-0.0.4.tar.gz` & `tmp/geopypi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Geopypi-0.0.4.tar", last modified: Tue Apr  9 21:22:01 2024, max compression
+gzip compressed data, was "geopypi-0.0.5.tar", last modified: Wed Apr 17 04:07:22 2024, max compression
```

## Comparing `Geopypi-0.0.4.tar` & `geopypi-0.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.152986 Geopypi-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.140986 Geopypi-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.144986 Geopypi-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.144986 Geopypi-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 21:21:47.000000 Geopypi-0.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.152986 Geopypi-0.0.4/Geopypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 21:22:01.000000 Geopypi-0.0.4/Geopypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:21:47.000000 Geopypi-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 21:21:47.000000 Geopypi-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 21:22:01.152986 Geopypi-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 21:21:47.000000 Geopypi-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.148986 Geopypi-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.148986 Geopypi-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    30850 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    47264 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab6.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/europe_110.geo.json
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/raster.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/examples/vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/geopypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.148986 Geopypi-0.0.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 21:21:47.000000 Geopypi-0.0.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.148986 Geopypi-0.0.4/geopypi/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 21:21:47.000000 Geopypi-0.0.4/geopypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 21:21:47.000000 Geopypi-0.0.4/geopypi/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-09 21:21:47.000000 Geopypi-0.0.4/geopypi/geopypi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 21:21:47.000000 Geopypi-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 21:21:47.000000 Geopypi-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 21:21:47.000000 Geopypi-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 21:21:47.000000 Geopypi-0.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:22:01.152986 Geopypi-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:22:01.152986 Geopypi-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 21:21:47.000000 Geopypi-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 21:21:47.000000 Geopypi-0.0.4/tests/test_geopypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.273095 geopypi-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-17 04:07:11.000000 geopypi-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.265095 geopypi-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.265095 geopypi-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.265095 geopypi-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 04:07:11.000000 geopypi-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 04:07:11.000000 geopypi-0.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.273095 geopypi-0.0.5/Geopypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 04:07:22.000000 geopypi-0.0.5/Geopypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:07:11.000000 geopypi-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 04:07:11.000000 geopypi-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 04:07:22.273095 geopypi-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 04:07:11.000000 geopypi-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.269095 geopypi-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.269095 geopypi-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    30850 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47264 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab6.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/ipywegets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/geopypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.269095 geopypi-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 04:07:11.000000 geopypi-0.0.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.273095 geopypi-0.0.5/geopypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 04:07:11.000000 geopypi-0.0.5/geopypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 04:07:11.000000 geopypi-0.0.5/geopypi/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-04-17 04:07:11.000000 geopypi-0.0.5/geopypi/geopypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-17 04:07:11.000000 geopypi-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-17 04:07:11.000000 geopypi-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 04:07:11.000000 geopypi-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-17 04:07:11.000000 geopypi-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:07:22.273095 geopypi-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:07:22.273095 geopypi-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 04:07:11.000000 geopypi-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 04:07:11.000000 geopypi-0.0.5/tests/test_geopypi.py
```

### Comparing `Geopypi-0.0.4/.github/workflows/docs-build.yml` & `geopypi-0.0.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/docs.yml` & `geopypi-0.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/installation.yml` & `geopypi-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/macos.yml` & `geopypi-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/pypi.yml` & `geopypi-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/ubuntu.yml` & `geopypi-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.github/workflows/windows.yml` & `geopypi-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/.gitignore` & `geopypi-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/Geopypi.egg-info/PKG-INFO` & `geopypi-0.0.5/Geopypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Geopypi-0.0.4/Geopypi.egg-info/SOURCES.txt` & `geopypi-0.0.5/Geopypi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/KH_Shakibul_Islam_lab4.ipynb
 docs/examples/KH_Shakibul_Islam_lab5.ipynb
 docs/examples/KH_Shakibul_Islam_lab6.ipynb
 docs/examples/europe_110.geo.json
-docs/examples/examples.ipynb
 docs/examples/intro.ipynb
+docs/examples/ipywegets.ipynb
 docs/examples/raster.ipynb
 docs/examples/vector.ipynb
 docs/overrides/main.html
 geopypi/__init__.py
 geopypi/common.py
 geopypi/geopypi.py
 tests/__init__.py
```

### Comparing `Geopypi-0.0.4/PKG-INFO` & `geopypi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Geopypi-0.0.4/docs/contributing.md` & `geopypi-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab4.ipynb` & `geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab4.ipynb`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab5.ipynb` & `geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab5.ipynb`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/docs/examples/KH_Shakibul_Islam_lab6.ipynb` & `geopypi-0.0.5/docs/examples/KH_Shakibul_Islam_lab6.ipynb`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/docs/examples/europe_110.geo.json` & `geopypi-0.0.5/docs/examples/europe_110.geo.json`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/docs/examples/examples.ipynb` & `geopypi-0.0.5/docs/examples/vector.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925415943287037%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, "*

 * *            "'[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/vector.ipynb)\\n'), "*

 * *            "(2, '## Add vector and geojson function to visualize vector datasets')], delete: [2, "*

 * *            "1, 0]}}, 2: {'execution_count': 8, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            '\'e70525f970a648e […]*

```diff
@@ -1,50 +1,21 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/examples.ipynb#scrollTo=vsp9e6EfuWz6)\n",
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/vector.ipynb)\n",
                 "\n",
-                "## A basic python package for CNN networking model\n",
-                "\n"
+                "## Add vector and geojson function to visualize vector datasets"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5e628a63273f40f3a39de3cb40a449c9",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Map(center=[40, -100], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_t\u2026"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "import geopypi\n",
-                "m = geopypi.Map()\n",
-                "m.add_basemap(\"OpenTopoMap\")\n",
-                "m"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Requirement already satisfied: geopypi in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (0.0.1)\n",
@@ -69,21 +40,112 @@
                         "Requirement already satisfied: colorama in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (0.4.6)\n",
                         "Requirement already satisfied: MarkupSafe>=2.0 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from jinja2>=3->branca>=0.5.0->ipyleaflet->geopypi) (2.1.5)\n",
                         "Requirement already satisfied: parso<0.9.0,>=0.8.3 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from jedi>=0.16->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (0.8.3)\n",
                         "Requirement already satisfied: wcwidth in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from prompt-toolkit<3.1.0,>=3.0.41->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (0.2.13)\n",
                         "Requirement already satisfied: executing>=1.2.0 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from stack-data->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (2.0.1)\n",
                         "Requirement already satisfied: asttokens>=2.1.0 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from stack-data->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (2.4.1)\n",
                         "Requirement already satisfied: pure-eval in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from stack-data->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (0.2.2)\n",
-                        "Requirement already satisfied: six>=1.12.0 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from asttokens>=2.1.0->stack-data->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (1.16.0)\n"
+                        "Requirement already satisfied: six>=1.12.0 in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (from asttokens>=2.1.0->stack-data->ipython>=6.1.0->ipywidgets<9,>=7.6.0->ipyleaflet->geopypi) (1.16.0)\n",
+                        "Note: you may need to restart the kernel to use updated packages.\n"
                     ]
                 }
             ],
             "source": [
-                "!pip install geopypi"
+                "pip install geopypi"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "e70525f970a648ebb4cdc729c00ca030",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "import geopypi\n",
+                "m = geopypi.Map()\n",
+                "m.add_basemap(\"OpenTopoMap\")\n",
+                "m.add_geojson(\"europe_110.geo.json\")\n",
+                "m.add_layers_control()\n",
+                "m"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "e70525f970a648ebb4cdc729c00ca030",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(bottom=654.0, center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', \u2026"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "m.add_vector('europe_110.geo.json')\n",
+                "m"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "e70525f970a648ebb4cdc729c00ca030",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(bottom=654.0, center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', \u2026"
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "m.add_shp(r\"D:\\spring 24\\software design\\AFG_adm\\AFG_adm2.shp\", name = \"afganistan\")\n",
+                "m.add_layers_control()\n",
+                "m"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "geo",
             "language": "python",
             "name": "python3"
```

### Comparing `Geopypi-0.0.4/docs/installation.md` & `geopypi-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.4/mkdocs.yml` & `geopypi-0.0.5/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -81,16 +81,18 @@
     - Report Issues: https://github.com/Metaliguns77/Geopypi/issues
     - Examples:
         - examples/intro.ipynb
         - examples/KH_Shakibul_Islam_lab4.ipynb
         - examples/KH_Shakibul_Islam_lab5.ipynb
         - examples/KH_Shakibul_Islam_lab6.ipynb
         - examples/vector.ipynb
-    - Labs:
-        -labs/KH_Shakibul_Islam_lab4.ipynb
-        -labs/KH_Shakibul_Islam_lab5.ipynb
+        - examples/raster.ipynb
+        
+    - Lab:
+        -lab/KH_Shakibul_Islam_lab4.ipynb
+        -lab/KH_Shakibul_Islam_lab5.ipynb
         
     - API Reference:
           - geopypi module: geopypi.md
           - common module: common.md
```

### Comparing `Geopypi-0.0.4/pyproject.toml` & `geopypi-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Geopypi"
-version = "0.0.4"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "This is a python package for batch geoprocessing."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

