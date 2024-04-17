# Comparing `tmp/boilerplates-1.0.2.dev1.tar.gz` & `tmp/boilerplates-1.0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boilerplates-1.0.2.dev1.tar", last modified: Thu Feb 15 11:21:09 2024, max compression
+gzip compressed data, was "boilerplates-1.0.2.dev2.tar", last modified: Wed Mar  6 03:20:08 2024, max compression
```

## Comparing `boilerplates-1.0.2.dev1.tar` & `boilerplates-1.0.2.dev2.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwx------   0 mateusz   (1000) mateusz   (1000)        0 2024-02-15 11:21:09.241816 boilerplates-1.0.2.dev1/
--rw-r-----   0 mateusz   (1000) mateusz   (1000)    11358 2023-08-12 12:15:05.000000 boilerplates-1.0.2.dev1/LICENSE
--rw-------   0 mateusz   (1000) mateusz   (1000)      384 2024-02-15 11:05:03.000000 boilerplates-1.0.2.dev1/MANIFEST.in
--rw-r-----   0 mateusz   (1000) mateusz   (1000)      592 2024-02-15 11:05:20.000000 boilerplates-1.0.2.dev1/NOTICE
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    14186 2024-02-15 11:21:09.241816 boilerplates-1.0.2.dev1/PKG-INFO
--rw-------   0 mateusz   (1000) mateusz   (1000)    11474 2024-02-15 10:14:11.000000 boilerplates-1.0.2.dev1/README.rst
-drwx------   0 mateusz   (1000) mateusz   (1000)        0 2024-02-15 11:21:09.233816 boilerplates-1.0.2.dev1/boilerplates/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       93 2023-08-12 12:33:14.000000 boilerplates-1.0.2.dev1/boilerplates/__init__.py
--rw-------   0 mateusz   (1000) mateusz   (1000)      119 2023-08-14 19:26:04.000000 boilerplates-1.0.2.dev1/boilerplates/_version.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4238 2023-08-15 17:25:06.000000 boilerplates-1.0.2.dev1/boilerplates/cli.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      985 2023-08-28 03:54:54.000000 boilerplates-1.0.2.dev1/boilerplates/config.py
--rw-------   0 mateusz   (1000) mateusz   (1000)     2913 2023-09-25 03:38:16.000000 boilerplates-1.0.2.dev1/boilerplates/git_repo_tests.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     8358 2023-09-25 03:38:23.000000 boilerplates-1.0.2.dev1/boilerplates/logging.py
--rw-------   0 mateusz   (1000) mateusz   (1000)     5138 2023-08-28 03:53:19.000000 boilerplates-1.0.2.dev1/boilerplates/packaging_tests.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-08-12 12:14:02.000000 boilerplates-1.0.2.dev1/boilerplates/py.typed
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1485 2024-02-15 09:56:25.000000 boilerplates-1.0.2.dev1/boilerplates/sentry.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     8839 2024-02-15 09:33:45.000000 boilerplates-1.0.2.dev1/boilerplates/sentry_future.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    14742 2023-08-14 10:59:29.000000 boilerplates-1.0.2.dev1/boilerplates/setup.py
-drwx------   0 mateusz   (1000) mateusz   (1000)        0 2024-02-15 11:21:09.237816 boilerplates-1.0.2.dev1/boilerplates.egg-info/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    14186 2024-02-15 11:21:09.000000 boilerplates-1.0.2.dev1/boilerplates.egg-info/PKG-INFO
--rw-------   0 mateusz   (1000) mateusz   (1000)     1133 2024-02-15 11:21:09.000000 boilerplates-1.0.2.dev1/boilerplates.egg-info/SOURCES.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)        1 2024-02-15 11:21:09.000000 boilerplates-1.0.2.dev1/boilerplates.egg-info/dependency_links.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)      321 2024-02-15 11:21:09.000000 boilerplates-1.0.2.dev1/boilerplates.egg-info/requires.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)       18 2024-02-15 11:21:09.000000 boilerplates-1.0.2.dev1/boilerplates.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      814 2023-08-14 20:06:34.000000 boilerplates-1.0.2.dev1/pyproject.toml
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       21 2023-08-14 19:21:07.000000 boilerplates-1.0.2.dev1/requirements.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)       19 2023-08-15 16:41:17.000000 boilerplates-1.0.2.dev1/requirements_cli.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)        0 2023-08-14 11:19:37.000000 boilerplates-1.0.2.dev1/requirements_config.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)       17 2023-08-15 17:57:01.000000 boilerplates-1.0.2.dev1/requirements_git_repo_tests.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)       43 2023-08-15 16:46:24.000000 boilerplates-1.0.2.dev1/requirements_logging.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       52 2023-08-14 03:27:57.000000 boilerplates-1.0.2.dev1/requirements_packaging_tests.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       36 2024-02-06 08:32:46.000000 boilerplates-1.0.2.dev1/requirements_sentry.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       67 2023-08-13 04:01:00.000000 boilerplates-1.0.2.dev1/requirements_setup.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)      196 2023-08-15 17:57:01.000000 boilerplates-1.0.2.dev1/requirements_test.txt
--rw-------   0 mateusz   (1000) mateusz   (1000)       38 2024-02-15 11:21:09.241816 boilerplates-1.0.2.dev1/setup.cfg
--rw-------   0 mateusz   (1000) mateusz   (1000)     1959 2024-02-15 09:57:00.000000 boilerplates-1.0.2.dev1/setup.py
-drwx------   0 mateusz   (1000) mateusz   (1000)        0 2024-02-15 11:21:09.237816 boilerplates-1.0.2.dev1/test/
--rw-r-----   0 mateusz   (1000) mateusz   (1000)      239 2023-08-25 04:38:49.000000 boilerplates-1.0.2.dev1/test/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     5168 2023-09-25 03:41:59.000000 boilerplates-1.0.2.dev1/test/test_cli.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2391 2023-08-27 04:30:44.000000 boilerplates-1.0.2.dev1/test/test_config.py
--rw-------   0 mateusz   (1000) mateusz   (1000)      892 2023-08-15 17:57:01.000000 boilerplates-1.0.2.dev1/test/test_git_repo.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4905 2023-08-15 16:48:00.000000 boilerplates-1.0.2.dev1/test/test_logging.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      133 2023-08-25 04:05:06.000000 boilerplates-1.0.2.dev1/test/test_packaging.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      439 2024-02-15 10:02:28.000000 boilerplates-1.0.2.dev1/test/test_sentry.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      965 2024-02-15 09:58:51.000000 boilerplates-1.0.2.dev1/test/test_sentry_future.py
--rw-r-----   0 mateusz   (1000) mateusz   (1000)     9822 2023-09-25 03:38:38.000000 boilerplates-1.0.2.dev1/test/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:08.181712 boilerplates-1.0.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-03-06 03:20:08.181712 boilerplates-1.0.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:08.177713 boilerplates-1.0.2.dev2/boilerplates/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/git_repo_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/packaging_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14742 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/boilerplates/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:08.181712 boilerplates-1.0.2.dev2/boilerplates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-03-06 03:20:08.000000 boilerplates-1.0.2.dev2/boilerplates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-06 03:20:08.000000 boilerplates-1.0.2.dev2/boilerplates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 03:20:08.000000 boilerplates-1.0.2.dev2/boilerplates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-06 03:20:08.000000 boilerplates-1.0.2.dev2/boilerplates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-06 03:20:08.000000 boilerplates-1.0.2.dev2/boilerplates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_cli.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_git_repo_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_logging.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_packaging_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_sentry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 03:20:08.181712 boilerplates-1.0.2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:20:08.181712 boilerplates-1.0.2.dev2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-03-06 03:20:02.000000 boilerplates-1.0.2.dev2/test/test_setup.py
```

### Comparing `boilerplates-1.0.2.dev1/LICENSE` & `boilerplates-1.0.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/NOTICE` & `boilerplates-1.0.2.dev2/NOTICE`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/PKG-INFO` & `boilerplates-1.0.2.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boilerplates
-Version: 1.0.2.dev1
+Version: 1.0.2.dev2
 Summary: Various boilerplates used in almost all of my Python packages.
 Home-page: https://github.com/mbdevpl/python-boilerplates
 Download-URL: 
 Author: Mateusz Bysiek
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -45,16 +45,15 @@
 Requires-Dist: setuptools>=67.4; extra == "packaging-tests"
 Requires-Dist: pip>=23.0; extra == "packaging-tests"
 Requires-Dist: wheel>=0.40; extra == "packaging-tests"
 Provides-Extra: config
 Provides-Extra: logging
 Requires-Dist: colorlog~=6.7; extra == "logging"
 Provides-Extra: sentry
-Requires-Dist: ratelimit~=2.2; extra == "sentry"
-Requires-Dist: sentry-sdk~=1.40; extra == "sentry"
+Requires-Dist: sentry-sdk[pure_eval]~=1.40; extra == "sentry"
 Provides-Extra: cli
 Requires-Dist: argcomplete~=3.1; extra == "cli"
 Provides-Extra: git-repo-tests
 Requires-Dist: GitPython~=3.1; extra == "git-repo-tests"
 
 .. role:: python(code)
     :language: python
@@ -81,32 +80,32 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/f22939bf833e40b89833d96c859bd7a4
     :target: https://app.codacy.com/gh/mbdevpl/python-boilerplates
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/python-boilerplates.svg
-    :target: https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/NOTICE
+    :target: https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/NOTICE
     :alt: license
 
 This package includes boilerplates for various common tasks in Python packages, such as building
 the package, testing the packaging process, storing the package config, logging for the package
 or creating a CLI.
 
 .. contents::
     :backlinks: none
 
 Requirements
 ============
 
 Python version 3.8 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/requirements_test.txt>`_.
 
 Tested on Linux, macOS and Windows.
 
 Available boilerplates
 ======================
 
 Setup boilerplate
@@ -341,14 +340,17 @@
     ...
 
 
     if __name__ == '__main__':
         Sentry.init()
         ...
 
+You can and should adjust the class fields to your needs, please take a look
+at the ``boilerplates.sentry.Sentry`` class implementation for details.
+
 And, you will need to add the following to your ``requirements.txt`` file (or equivalent):
 
 .. code:: text
 
     boilerplates[sentry] ~= <version>
 
 CLI boilerplate
@@ -379,15 +381,15 @@
         boilerplates.cli.add_verbosity_group(parser)
 
         parsed_args = parser.parse_args(args)
 
         verbosity = boilerplates.cli.get_verbosity_level(parsed_args)
         ...
 
-You can see the above example in action in the `examples.ipynb <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/examples.ipynb>`_ notebook.
+You can see the above example in action in the `examples.ipynb <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/examples.ipynb>`_ notebook.
 Please see the ``boilerplates.cli`` module for details of the available features.
 
 And then, an example ``__main__.py`` file may look like:
 
 .. code:: python
 
     """Entry point of the command-line interface."""
```

### Comparing `boilerplates-1.0.2.dev1/README.rst` & `boilerplates-1.0.2.dev2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,17 @@
     ...
 
 
     if __name__ == '__main__':
         Sentry.init()
         ...
 
+You can and should adjust the class fields to your needs, please take a look
+at the ``boilerplates.sentry.Sentry`` class implementation for details.
+
 And, you will need to add the following to your ``requirements.txt`` file (or equivalent):
 
 .. code:: text
 
     boilerplates[sentry] ~= <version>
 
 CLI boilerplate
```

### Comparing `boilerplates-1.0.2.dev1/boilerplates/cli.py` & `boilerplates-1.0.2.dev2/boilerplates/cli.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates/config.py` & `boilerplates-1.0.2.dev2/boilerplates/config.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates/git_repo_tests.py` & `boilerplates-1.0.2.dev2/boilerplates/git_repo_tests.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates/logging.py` & `boilerplates-1.0.2.dev2/boilerplates/logging.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates/packaging_tests.py` & `boilerplates-1.0.2.dev2/boilerplates/packaging_tests.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates/setup.py` & `boilerplates-1.0.2.dev2/boilerplates/setup.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/boilerplates.egg-info/PKG-INFO` & `boilerplates-1.0.2.dev2/boilerplates.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boilerplates
-Version: 1.0.2.dev1
+Version: 1.0.2.dev2
 Summary: Various boilerplates used in almost all of my Python packages.
 Home-page: https://github.com/mbdevpl/python-boilerplates
 Download-URL: 
 Author: Mateusz Bysiek
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -45,16 +45,15 @@
 Requires-Dist: setuptools>=67.4; extra == "packaging-tests"
 Requires-Dist: pip>=23.0; extra == "packaging-tests"
 Requires-Dist: wheel>=0.40; extra == "packaging-tests"
 Provides-Extra: config
 Provides-Extra: logging
 Requires-Dist: colorlog~=6.7; extra == "logging"
 Provides-Extra: sentry
-Requires-Dist: ratelimit~=2.2; extra == "sentry"
-Requires-Dist: sentry-sdk~=1.40; extra == "sentry"
+Requires-Dist: sentry-sdk[pure_eval]~=1.40; extra == "sentry"
 Provides-Extra: cli
 Requires-Dist: argcomplete~=3.1; extra == "cli"
 Provides-Extra: git-repo-tests
 Requires-Dist: GitPython~=3.1; extra == "git-repo-tests"
 
 .. role:: python(code)
     :language: python
@@ -81,32 +80,32 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/f22939bf833e40b89833d96c859bd7a4
     :target: https://app.codacy.com/gh/mbdevpl/python-boilerplates
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/python-boilerplates.svg
-    :target: https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/NOTICE
+    :target: https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/NOTICE
     :alt: license
 
 This package includes boilerplates for various common tasks in Python packages, such as building
 the package, testing the packaging process, storing the package config, logging for the package
 or creating a CLI.
 
 .. contents::
     :backlinks: none
 
 Requirements
 ============
 
 Python version 3.8 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/requirements_test.txt>`_.
 
 Tested on Linux, macOS and Windows.
 
 Available boilerplates
 ======================
 
 Setup boilerplate
@@ -341,14 +340,17 @@
     ...
 
 
     if __name__ == '__main__':
         Sentry.init()
         ...
 
+You can and should adjust the class fields to your needs, please take a look
+at the ``boilerplates.sentry.Sentry`` class implementation for details.
+
 And, you will need to add the following to your ``requirements.txt`` file (or equivalent):
 
 .. code:: text
 
     boilerplates[sentry] ~= <version>
 
 CLI boilerplate
@@ -379,15 +381,15 @@
         boilerplates.cli.add_verbosity_group(parser)
 
         parsed_args = parser.parse_args(args)
 
         verbosity = boilerplates.cli.get_verbosity_level(parsed_args)
         ...
 
-You can see the above example in action in the `examples.ipynb <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev1/examples.ipynb>`_ notebook.
+You can see the above example in action in the `examples.ipynb <https://github.com/mbdevpl/python-boilerplates/blob/v1.0.2.dev2/examples.ipynb>`_ notebook.
 Please see the ``boilerplates.cli`` module for details of the available features.
 
 And then, an example ``__main__.py`` file may look like:
 
 .. code:: python
 
     """Entry point of the command-line interface."""
```

### Comparing `boilerplates-1.0.2.dev1/boilerplates.egg-info/SOURCES.txt` & `boilerplates-1.0.2.dev2/boilerplates.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,31 +18,28 @@
 ./boilerplates/cli.py
 ./boilerplates/config.py
 ./boilerplates/git_repo_tests.py
 ./boilerplates/logging.py
 ./boilerplates/packaging_tests.py
 ./boilerplates/py.typed
 ./boilerplates/sentry.py
-./boilerplates/sentry_future.py
 ./boilerplates/setup.py
 ./test/__init__.py
 ./test/test_cli.py
 ./test/test_config.py
 ./test/test_git_repo.py
 ./test/test_logging.py
 ./test/test_packaging.py
 ./test/test_sentry.py
-./test/test_sentry_future.py
 ./test/test_setup.py
 boilerplates.egg-info/PKG-INFO
 boilerplates.egg-info/SOURCES.txt
 boilerplates.egg-info/dependency_links.txt
 boilerplates.egg-info/requires.txt
 boilerplates.egg-info/top_level.txt
 test/test_cli.py
 test/test_config.py
 test/test_git_repo.py
 test/test_logging.py
 test/test_packaging.py
 test/test_sentry.py
-test/test_sentry_future.py
 test/test_setup.py
```

### Comparing `boilerplates-1.0.2.dev1/pyproject.toml` & `boilerplates-1.0.2.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/setup.py` & `boilerplates-1.0.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/test/test_cli.py` & `boilerplates-1.0.2.dev2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/test/test_config.py` & `boilerplates-1.0.2.dev2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/test/test_git_repo.py` & `boilerplates-1.0.2.dev2/test/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/test/test_logging.py` & `boilerplates-1.0.2.dev2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `boilerplates-1.0.2.dev1/test/test_setup.py` & `boilerplates-1.0.2.dev2/test/test_setup.py`

 * *Files identical despite different names*

