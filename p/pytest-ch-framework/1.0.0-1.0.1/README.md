# Comparing `tmp/pytest_ch_framework-1.0.0.tar.gz` & `tmp/pytest_ch_framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ch_framework-1.0.0.tar", last modified: Wed Mar 13 08:22:14 2024, max compression
+gzip compressed data, was "pytest_ch_framework-1.0.1.tar", last modified: Wed Apr 17 05:44:09 2024, max compression
```

## Comparing `pytest_ch_framework-1.0.0.tar` & `pytest_ch_framework-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.152849 pytest_ch_framework-1.0.0/
--rw-rw-rw-   0        0        0      428 2024-03-13 08:22:14.151727 pytest_ch_framework-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      625 2024-03-13 08:20:52.000000 pytest_ch_framework-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 08:22:14.152849 pytest_ch_framework-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.142756 pytest_ch_framework-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.143911 pytest_ch_framework-1.0.0/src/framework/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.0/src/framework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.144922 pytest_ch_framework-1.0.0/src/framework/allure/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.0/src/framework/allure/__init__.py
--rw-rw-rw-   0        0        0     6304 2024-03-13 06:55:04.000000 pytest_ch_framework-1.0.0/src/framework/allure/report.py
--rw-rw-rw-   0        0        0      252 2024-03-11 05:10:25.000000 pytest_ch_framework-1.0.0/src/framework/allure/step.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.145251 pytest_ch_framework-1.0.0/src/framework/config/
--rw-rw-rw-   0        0        0        0 2024-03-12 09:06:30.000000 pytest_ch_framework-1.0.0/src/framework/config/__init__.py
--rw-rw-rw-   0        0        0     1562 2024-03-12 09:15:21.000000 pytest_ch_framework-1.0.0/src/framework/config/csv.py
--rw-rw-rw-   0        0        0     2042 2024-03-13 02:33:59.000000 pytest_ch_framework-1.0.0/src/framework/config/yaml.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.146261 pytest_ch_framework-1.0.0/src/framework/io/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.0/src/framework/io/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-12 07:01:18.000000 pytest_ch_framework-1.0.0/src/framework/io/config.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.147454 pytest_ch_framework-1.0.0/src/framework/mod/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:53:28.000000 pytest_ch_framework-1.0.0/src/framework/mod/__init__.py
--rw-rw-rw-   0        0        0      188 2024-03-08 10:17:15.000000 pytest_ch_framework-1.0.0/src/framework/mod/mod.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.148648 pytest_ch_framework-1.0.0/src/framework/plugin/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.0/src/framework/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.148648 pytest_ch_framework-1.0.0/src/framework/plugin/extra/
--rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.0/src/framework/plugin/extra/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-03-13 04:04:13.000000 pytest_ch_framework-1.0.0/src/framework/plugin/extra/metadata_property.py
--rw-rw-rw-   0        0        0        0 2024-03-12 08:24:38.000000 pytest_ch_framework-1.0.0/src/framework/plugin/functions.py
--rw-rw-rw-   0        0        0      355 2024-03-12 08:30:16.000000 pytest_ch_framework-1.0.0/src/framework/plugin/mark.py
-drwxrwxrwx   0        0        0        0 2024-03-13 08:22:14.151727 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/
--rw-rw-rw-   0        0        0      428 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-13 08:22:14.000000 pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.410703 pytest_ch_framework-1.0.1/
+-rw-rw-rw-   0        0        0      428 2024-04-17 05:44:09.410703 pytest_ch_framework-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-17 04:05:35.000000 pytest_ch_framework-1.0.1/README.md
+-rw-rw-rw-   0        0        0      625 2024-04-17 05:24:17.000000 pytest_ch_framework-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 05:44:09.410703 pytest_ch_framework-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.401534 pytest_ch_framework-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.403588 pytest_ch_framework-1.0.1/src/framework/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.1/src/framework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.403588 pytest_ch_framework-1.0.1/src/framework/allure/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.1/src/framework/allure/__init__.py
+-rw-rw-rw-   0        0        0      252 2024-03-11 05:10:25.000000 pytest_ch_framework-1.0.1/src/framework/allure/step.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.404540 pytest_ch_framework-1.0.1/src/framework/config/
+-rw-rw-rw-   0        0        0        0 2024-03-12 09:06:30.000000 pytest_ch_framework-1.0.1/src/framework/config/__init__.py
+-rw-rw-rw-   0        0        0     1562 2024-03-12 09:15:21.000000 pytest_ch_framework-1.0.1/src/framework/config/csv.py
+-rw-rw-rw-   0        0        0     2042 2024-03-13 02:33:59.000000 pytest_ch_framework-1.0.1/src/framework/config/yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.405558 pytest_ch_framework-1.0.1/src/framework/io/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.1/src/framework/io/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-12 07:01:18.000000 pytest_ch_framework-1.0.1/src/framework/io/config.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.406585 pytest_ch_framework-1.0.1/src/framework/mod/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:53:28.000000 pytest_ch_framework-1.0.1/src/framework/mod/__init__.py
+-rw-rw-rw-   0        0        0      188 2024-03-08 10:17:15.000000 pytest_ch_framework-1.0.1/src/framework/mod/mod.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.406585 pytest_ch_framework-1.0.1/src/framework/plugin/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.1/src/framework/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.407611 pytest_ch_framework-1.0.1/src/framework/plugin/extra/
+-rw-rw-rw-   0        0        0        0 2024-03-08 14:41:00.000000 pytest_ch_framework-1.0.1/src/framework/plugin/extra/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-03-13 04:04:13.000000 pytest_ch_framework-1.0.1/src/framework/plugin/extra/metadata_property.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 08:24:38.000000 pytest_ch_framework-1.0.1/src/framework/plugin/functions.py
+-rw-rw-rw-   0        0        0      355 2024-03-12 08:30:16.000000 pytest_ch_framework-1.0.1/src/framework/plugin/mark.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:44:09.410703 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 05:44:09.000000 pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/top_level.txt
```

### Comparing `pytest_ch_framework-1.0.0/pyproject.toml` & `pytest_ch_framework-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
-version = "1.0.0"
+version = "1.0.1"
 name = "pytest_ch_framework"
 authors = [ #作者列表
   {name = "caihua zhan", email = "caihuadaye@outlook.com"}
 ]
 description = "My pytest framework"
 classifiers = [
     "Framework :: Pytest",
```

### Comparing `pytest_ch_framework-1.0.0/src/framework/config/csv.py` & `pytest_ch_framework-1.0.1/src/framework/config/csv.py`

 * *Files identical despite different names*

### Comparing `pytest_ch_framework-1.0.0/src/framework/config/yaml.py` & `pytest_ch_framework-1.0.1/src/framework/config/yaml.py`

 * *Files identical despite different names*

### Comparing `pytest_ch_framework-1.0.0/src/framework/io/config.py` & `pytest_ch_framework-1.0.1/src/framework/io/config.py`

 * *Files identical despite different names*

### Comparing `pytest_ch_framework-1.0.0/src/framework/plugin/extra/metadata_property.py` & `pytest_ch_framework-1.0.1/src/framework/plugin/extra/metadata_property.py`

 * *Files identical despite different names*

### Comparing `pytest_ch_framework-1.0.0/src/pytest_ch_framework.egg-info/SOURCES.txt` & `pytest_ch_framework-1.0.1/src/pytest_ch_framework.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+README.md
 pyproject.toml
 src/framework/__init__.py
 src/framework/allure/__init__.py
-src/framework/allure/report.py
 src/framework/allure/step.py
 src/framework/config/__init__.py
 src/framework/config/csv.py
 src/framework/config/yaml.py
 src/framework/io/__init__.py
 src/framework/io/config.py
 src/framework/mod/__init__.py
```

