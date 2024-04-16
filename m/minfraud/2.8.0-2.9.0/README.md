# Comparing `tmp/minfraud-2.8.0.tar.gz` & `tmp/minfraud-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minfraud-2.8.0.tar", last modified: Tue May  9 20:58:10 2023, max compression
+gzip compressed data, was "minfraud-2.9.0.tar", last modified: Tue Dec  5 22:42:16 2023, max compression
```

## Comparing `minfraud-2.8.0.tar` & `minfraud-2.9.0.tar`

### file list

```diff
@@ -1,73 +1,41 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.805362 minfraud-2.8.0/
--rw-r--r--   0 greg      (1000) greg      (1000)    13144 2023-05-09 20:30:14.000000 minfraud-2.8.0/HISTORY.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    11358 2020-07-13 16:21:25.000000 minfraud-2.8.0/LICENSE
--rw-r--r--   0 greg      (1000) greg      (1000)      263 2021-09-20 17:37:04.000000 minfraud-2.8.0/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)    11982 2023-05-09 20:58:10.805362 minfraud-2.8.0/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)    10831 2023-01-17 17:45:49.000000 minfraud-2.8.0/README.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.793362 minfraud-2.8.0/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)     8201 2023-01-17 17:45:49.000000 minfraud-2.8.0/docs/conf.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.797362 minfraud-2.8.0/docs/doctrees/
--rw-r--r--   0 greg      (1000) greg      (1000)  2453968 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/doctrees/environment.pickle
--rw-r--r--   0 greg      (1000) greg      (1000)   488049 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/doctrees/index.doctree
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.797362 minfraud-2.8.0/docs/html/
--rw-r--r--   0 greg      (1000) greg      (1000)      230 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/.buildinfo
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.797362 minfraud-2.8.0/docs/html/_sources/
--rw-r--r--   0 greg      (1000) greg      (1000)      552 2023-01-17 17:45:49.000000 minfraud-2.8.0/docs/html/_sources/index.rst.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.801362 minfraud-2.8.0/docs/html/_static/
--rw-r--r--   0 greg      (1000) greg      (1000)    14813 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/_static/basic.css
--rw-r--r--   0 greg      (1000) greg      (1000)      107 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/contents.png
--rw-r--r--   0 greg      (1000) greg      (1000)     4472 2023-05-09 20:58:01.000000 minfraud-2.8.0/docs/html/_static/doctools.js
--rw-r--r--   0 greg      (1000) greg      (1000)      420 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/_static/documentation_options.js
--rw-r--r--   0 greg      (1000) greg      (1000)      286 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/file.png
--rw-r--r--   0 greg      (1000) greg      (1000)   280364 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/jquery-3.4.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)   287630 2020-07-14 14:23:54.000000 minfraud-2.8.0/docs/html/_static/jquery-3.5.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    89476 2020-07-14 14:23:54.000000 minfraud-2.8.0/docs/html/_static/jquery.js
--rw-r--r--   0 greg      (1000) greg      (1000)     4758 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/_static/language_data.js
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/minus.png
--rw-r--r--   0 greg      (1000) greg      (1000)      120 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/navigation.png
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/plus.png
--rw-r--r--   0 greg      (1000) greg      (1000)     4846 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/_static/pygments.css
--rw-r--r--   0 greg      (1000) greg      (1000)    18215 2023-05-09 20:58:01.000000 minfraud-2.8.0/docs/html/_static/searchtools.js
--rw-r--r--   0 greg      (1000) greg      (1000)     4712 2023-05-09 20:58:01.000000 minfraud-2.8.0/docs/html/_static/sphinx_highlight.js
--rw-r--r--   0 greg      (1000) greg      (1000)     6263 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/_static/sphinxdoc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    68420 2021-09-20 17:44:35.000000 minfraud-2.8.0/docs/html/_static/underscore-1.13.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    35168 2019-12-20 18:41:55.000000 minfraud-2.8.0/docs/html/_static/underscore-1.3.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    19530 2021-09-20 17:44:35.000000 minfraud-2.8.0/docs/html/_static/underscore.js
--rw-r--r--   0 greg      (1000) greg      (1000)    28775 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/genindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)   243686 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/index.html
--rw-r--r--   0 greg      (1000) greg      (1000)     1411 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/objects.inv
--rw-r--r--   0 greg      (1000) greg      (1000)     4147 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/py-modindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)     3257 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/search.html
--rw-r--r--   0 greg      (1000) greg      (1000)    32946 2023-05-09 20:58:10.000000 minfraud-2.8.0/docs/html/searchindex.js
--rw-r--r--   0 greg      (1000) greg      (1000)      552 2023-01-17 17:45:49.000000 minfraud-2.8.0/docs/index.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.805362 minfraud-2.8.0/minfraud/
--rw-r--r--   0 greg      (1000) greg      (1000)      364 2023-01-17 21:45:15.000000 minfraud-2.8.0/minfraud/__init__.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     1662 2020-10-06 15:13:04.000000 minfraud-2.8.0/minfraud/errors.py
--rw-r--r--   0 greg      (1000) greg      (1000)    37838 2023-05-09 20:27:16.000000 minfraud-2.8.0/minfraud/models.py
--rw-r--r--   0 greg      (1000) greg      (1000)        0 2020-07-28 17:39:21.000000 minfraud-2.8.0/minfraud/py.typed
--rw-r--r--   0 greg      (1000) greg      (1000)     3447 2023-02-07 18:27:20.000000 minfraud-2.8.0/minfraud/request.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9369 2023-01-17 17:45:49.000000 minfraud-2.8.0/minfraud/validation.py
--rw-r--r--   0 greg      (1000) greg      (1000)       84 2023-05-09 20:38:34.000000 minfraud-2.8.0/minfraud/version.py
--rw-r--r--   0 greg      (1000) greg      (1000)    24306 2023-05-09 20:27:16.000000 minfraud-2.8.0/minfraud/webservice.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.805362 minfraud-2.8.0/minfraud.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)    11982 2023-05-09 20:58:10.000000 minfraud-2.8.0/minfraud.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     1621 2023-05-09 20:58:10.000000 minfraud-2.8.0/minfraud.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-09 20:58:10.000000 minfraud-2.8.0/minfraud.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      108 2023-05-09 20:58:10.000000 minfraud-2.8.0/minfraud.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        9 2023-05-09 20:58:10.000000 minfraud-2.8.0/minfraud.egg-info/top_level.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      169 2023-05-09 20:27:16.000000 minfraud-2.8.0/pyproject.toml
--rw-r--r--   0 greg      (1000) greg      (1000)      760 2023-05-09 20:58:10.805362 minfraud-2.8.0/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)     1980 2023-05-09 20:28:44.000000 minfraud-2.8.0/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.805362 minfraud-2.8.0/tests/
--rw-r--r--   0 greg      (1000) greg      (1000)        0 2019-02-08 20:47:45.000000 minfraud-2.8.0/tests/__init__.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:58:10.805362 minfraud-2.8.0/tests/data/
--rw-r--r--   0 greg      (1000) greg      (1000)     5073 2022-01-04 18:06:36.000000 minfraud-2.8.0/tests/data/factors-response.json
--rw-rw-r--   0 greg      (1000) greg      (1000)      306 2020-09-23 20:24:00.000000 minfraud-2.8.0/tests/data/full-report-request.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2234 2022-03-28 19:25:11.000000 minfraud-2.8.0/tests/data/full-transaction-request.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4485 2022-01-04 18:06:36.000000 minfraud-2.8.0/tests/data/insights-response.json
--rw-r--r--   0 greg      (1000) greg      (1000)        4 2020-07-14 14:22:19.000000 minfraud-2.8.0/tests/data/report-response.json
--rw-r--r--   0 greg      (1000) greg      (1000)      646 2019-02-08 20:47:45.000000 minfraud-2.8.0/tests/data/score-response.json
--rw-r--r--   0 greg      (1000) greg      (1000)    14671 2023-05-09 20:27:16.000000 minfraud-2.8.0/tests/test_models.py
--rw-r--r--   0 greg      (1000) greg      (1000)     6726 2022-01-25 16:57:06.000000 minfraud-2.8.0/tests/test_request.py
--rw-r--r--   0 greg      (1000) greg      (1000)    15656 2022-03-28 19:25:11.000000 minfraud-2.8.0/tests/test_validation.py
--rw-r--r--   0 greg      (1000) greg      (1000)    12344 2023-05-09 20:27:16.000000 minfraud-2.8.0/tests/test_webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.648708 minfraud-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2023-12-05 22:42:08.000000 minfraud-2.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-05 22:42:08.000000 minfraud-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-05 22:42:08.000000 minfraud-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2023-12-05 22:42:16.648708 minfraud-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-05 22:42:08.000000 minfraud-2.9.0/README.dev.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2023-12-05 22:42:08.000000 minfraud-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.644708 minfraud-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2023-12-05 22:42:08.000000 minfraud-2.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-05 22:42:08.000000 minfraud-2.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.644708 minfraud-2.9.0/minfraud/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37838 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24763 2023-12-05 22:42:08.000000 minfraud-2.9.0/minfraud/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.648708 minfraud-2.9.0/minfraud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2023-12-05 22:42:16.000000 minfraud-2.9.0/minfraud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-05 22:42:16.000000 minfraud-2.9.0/minfraud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 22:42:16.000000 minfraud-2.9.0/minfraud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-05 22:42:16.000000 minfraud-2.9.0/minfraud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-05 22:42:16.000000 minfraud-2.9.0/minfraud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-05 22:42:08.000000 minfraud-2.9.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-12-05 22:42:08.000000 minfraud-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-05 22:42:16.648708 minfraud-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.648708 minfraud-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:16.648708 minfraud-2.9.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/factors-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/full-report-request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/full-transaction-request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/insights-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/report-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/data/score-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2023-12-05 22:42:08.000000 minfraud-2.9.0/tests/test_webservice.py
```

### Comparing `minfraud-2.8.0/HISTORY.rst` & `minfraud-2.9.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. :changelog:
 
 History
 -------
 
+2.9.0 (2023-12-05)
+++++++++++++++++++
+
+* IMPORTANT: Python 3.8 or greater is required. If you are using an older
+  version, please use an earlier release.
+* Updated ``geoip2`` to version that includes the ``is_anycast`` attribute on
+  ``geoip2.record.Traits``. This property is ``True`` if the IP address
+  belongs to an `anycast network <https://en.wikipedia.org/wiki/Anycast>`_.
+  This is available in minFraud Insights and Factors.
+
 2.8.0 (2023-05-09)
 ++++++++++++++++++
 
 * IMPORTANT: Python 3.7 or greater is required. If you are using an older
   version, please use an earlier release.
 * Added the following new values to the ``/payment/processor`` validation:
   * ``google_pay``
```

### Comparing `minfraud-2.8.0/LICENSE` & `minfraud-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/PKG-INFO` & `minfraud-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: minfraud
-Version: 2.8.0
+Version: 2.9.0
 Summary: MaxMind minFraud Score, Insights, Factors and Report Transactions API
-Home-page: https://www.maxmind.com/
-Author: Gregory Oschwald
-Author-email: goschwald@maxmind.com
-License: Apache License 2.0 
+Author-email: Gregory Oschwald <goschwald@maxmind.com>
+License: Apache License 2.0
+Project-URL: Homepage, https://www.maxmind.com/
 Project-URL: Documentation, https://minfraud.readthedocs.org/
 Project-URL: Source Code, https://github.com/maxmind/minfraud-api-python
 Project-URL: Issue Tracker, https://github.com/maxmind/minfraud-api-python/issues
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: setuptools>=60.0.0
+Requires-Dist: aiohttp<4.0.0,>=3.6.2
+Requires-Dist: email_validator<3.0.0,>=2.0.0
+Requires-Dist: geoip2<5.0.0,>=4.8.0
+Requires-Dist: requests<3.0.0,>=2.24.0
+Requires-Dist: voluptuous
+Provides-Extra: test
+Requires-Dist: mocket>=3.11.1; extra == "test"
 
 ===================================================================
 minFraud Score, Insights, Factors and Report Transaction Python API
 ===================================================================
 
 Description
 -----------
@@ -68,14 +76,22 @@
 constructors take your MaxMind account ID and license key:
 
 .. code-block:: pycon
 
     >>> client = Client(42, 'licensekey')
     >>> async_client = AsyncClient(42, 'licensekey')
 
+To use the Sandbox web service instead of the production web service,
+you can provide the host argument:
+
+.. code-block:: pycon
+
+    >>> client = Client(42, 'licensekey', 'sandbox.maxmind.com')
+    >>> async_client = AsyncClient(42, 'licensekey', 'sandbox.maxmind.com')
+
 Score, Insights and Factors Usage
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The Factors service is called with the ``factors()`` method:
 
 .. code-block:: pycon
 
@@ -322,15 +338,15 @@
     >>>          await async_client.report(transaction_report)
     >>>
     >>> asyncio.run(report())
 
 Requirements
 ------------
 
-Python 3.7 or greater is required. Older versions are not supported.
+Python 3.8 or greater is required. Older versions are not supported.
 
 Versioning
 ----------
 
 The minFraud Python API uses `Semantic Versioning <https://semver.org/>`_.
 
 Support
```

### Comparing `minfraud-2.8.0/README.rst` & `minfraud-2.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 constructors take your MaxMind account ID and license key:
 
 .. code-block:: pycon
 
     >>> client = Client(42, 'licensekey')
     >>> async_client = AsyncClient(42, 'licensekey')
 
+To use the Sandbox web service instead of the production web service,
+you can provide the host argument:
+
+.. code-block:: pycon
+
+    >>> client = Client(42, 'licensekey', 'sandbox.maxmind.com')
+    >>> async_client = AsyncClient(42, 'licensekey', 'sandbox.maxmind.com')
+
 Score, Insights and Factors Usage
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The Factors service is called with the ``factors()`` method:
 
 .. code-block:: pycon
 
@@ -294,15 +302,15 @@
     >>>          await async_client.report(transaction_report)
     >>>
     >>> asyncio.run(report())
 
 Requirements
 ------------
 
-Python 3.7 or greater is required. Older versions are not supported.
+Python 3.8 or greater is required. Older versions are not supported.
 
 Versioning
 ----------
 
 The minFraud Python API uses `Semantic Versioning <https://semver.org/>`_.
 
 Support
```

### Comparing `minfraud-2.8.0/docs/conf.py` & `minfraud-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/docs/html/_sources/index.rst.txt` & `minfraud-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/minfraud/errors.py` & `minfraud-2.9.0/minfraud/errors.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/minfraud/models.py` & `minfraud-2.9.0/minfraud/models.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/minfraud/request.py` & `minfraud-2.9.0/minfraud/request.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/minfraud/validation.py` & `minfraud-2.9.0/minfraud/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return str(ipaddress.ip_address(s))
     raise ValueError
 
 
 def _email_or_md5(s: str) -> str:
     if re.match(r"^[0-9A-Fa-f]{32}$", s):
         return s
-    return validate_email(s, check_deliverability=False).email
+    return validate_email(s, check_deliverability=False).normalized
 
 
 # based off of:
 # https://stackoverflow.com/questions/2532053/validate-a-hostname-string
 def _hostname(hostname: str) -> str:
     if len(hostname) > 255:
         raise ValueError
```

### Comparing `minfraud-2.8.0/minfraud/webservice.py` & `minfraud-2.9.0/minfraud/webservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 from .request import prepare_report, prepare_transaction
 
 
 _AIOHTTP_UA = f"minFraud-API/{__version__} {aiohttp.http.SERVER_SOFTWARE}"
 
 _REQUEST_UA = f"minFraud-API/{__version__} {requests.utils.default_user_agent()}"
 
+# We have this so that we can avoid a mocket issue:
+# https://github.com/mindflayer/python-mocket/issues/209
+_SCHEME = "https"
+
 
 # pylint: disable=too-many-instance-attributes, missing-class-docstring
 class BaseClient:
     _account_id: str
     _license_key: str
     _locales: Tuple[str, ...]
     _timeout: float
@@ -54,15 +58,15 @@
         timeout: float = 60,
     ) -> None:
         self._locales = locales
         self._account_id = str(account_id)
         self._license_key = license_key
         self._timeout = timeout
 
-        base_uri = f"https://{host}/minfraud/v2.0"
+        base_uri = f"{_SCHEME}://{host}/minfraud/v2.0"
         self._score_uri = "/".join([base_uri, "score"])
         self._insights_uri = "/".join([base_uri, "insights"])
         self._factors_uri = "/".join([base_uri, "factors"])
         self._report_uri = "/".join([base_uri, "transactions", "report"])
 
     def _handle_success(
         self,
@@ -451,14 +455,19 @@
         """Constructor for Client.
 
         :param account_id: Your MaxMind account ID
         :type account_id: int
         :param license_key: Your MaxMind license key
         :type license_key: str
         :param host: The host to use when connecting to the web service.
+          By default, the client connects to the production host. However,
+          during testing and development, you can set this option to
+          'sandbox.maxmind.com' to use the Sandbox environment's host. The
+          sandbox allows you to experiment with the API without affecting your
+          production data.
         :type host: str
         :param locales: A tuple of locale codes to use in name property
         :type locales: tuple[str]
         :param timeout: The timeout in seconds to use when waiting on the request.
           This sets both the connect timeout and the read timeout. The default is
           60.
         :param proxy: The URL of an HTTP proxy to use. It may optionally include
```

### Comparing `minfraud-2.8.0/minfraud.egg-info/PKG-INFO` & `minfraud-2.9.0/minfraud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: minfraud
-Version: 2.8.0
+Version: 2.9.0
 Summary: MaxMind minFraud Score, Insights, Factors and Report Transactions API
-Home-page: https://www.maxmind.com/
-Author: Gregory Oschwald
-Author-email: goschwald@maxmind.com
-License: Apache License 2.0 
+Author-email: Gregory Oschwald <goschwald@maxmind.com>
+License: Apache License 2.0
+Project-URL: Homepage, https://www.maxmind.com/
 Project-URL: Documentation, https://minfraud.readthedocs.org/
 Project-URL: Source Code, https://github.com/maxmind/minfraud-api-python
 Project-URL: Issue Tracker, https://github.com/maxmind/minfraud-api-python/issues
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: setuptools>=60.0.0
+Requires-Dist: aiohttp<4.0.0,>=3.6.2
+Requires-Dist: email_validator<3.0.0,>=2.0.0
+Requires-Dist: geoip2<5.0.0,>=4.8.0
+Requires-Dist: requests<3.0.0,>=2.24.0
+Requires-Dist: voluptuous
+Provides-Extra: test
+Requires-Dist: mocket>=3.11.1; extra == "test"
 
 ===================================================================
 minFraud Score, Insights, Factors and Report Transaction Python API
 ===================================================================
 
 Description
 -----------
@@ -68,14 +76,22 @@
 constructors take your MaxMind account ID and license key:
 
 .. code-block:: pycon
 
     >>> client = Client(42, 'licensekey')
     >>> async_client = AsyncClient(42, 'licensekey')
 
+To use the Sandbox web service instead of the production web service,
+you can provide the host argument:
+
+.. code-block:: pycon
+
+    >>> client = Client(42, 'licensekey', 'sandbox.maxmind.com')
+    >>> async_client = AsyncClient(42, 'licensekey', 'sandbox.maxmind.com')
+
 Score, Insights and Factors Usage
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The Factors service is called with the ``factors()`` method:
 
 .. code-block:: pycon
 
@@ -322,15 +338,15 @@
     >>>          await async_client.report(transaction_report)
     >>>
     >>> asyncio.run(report())
 
 Requirements
 ------------
 
-Python 3.7 or greater is required. Older versions are not supported.
+Python 3.8 or greater is required. Older versions are not supported.
 
 Versioning
 ----------
 
 The minFraud Python API uses `Semantic Versioning <https://semver.org/>`_.
 
 Support
```

### Comparing `minfraud-2.8.0/setup.cfg` & `minfraud-2.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-[aliases]
-build_html = build_sphinx -b html --build-dir docs
-
 [flake8]
 max-line-length = 88
 
-[wheel]
-universal = 1
-
 [tox:tox]
-envlist = {py37,py38,py39,py310}-test,py310-{black,lint,flake8,mypy}
+envlist = {py38,py39,py310,py311,py312}-test,py312-{black,lint,flake8,mypy}
 
 [gh-actions]
 python = 
-	3.7: py37
 	3.8: py38
 	3.9: py39
-	3.10: py310,black,lint,flake8,mypy
+	3.10: py310
+	3.11: py311
+	3.12: py312,black,lint,flake8,mypy
 
-[testenv:{py37,py38,py39,py310}-test]
+[testenv:{py38,py39,py310,py311,py312}-test]
 deps = 
 	mocket
 	pytest
 	
 	charset-normalizer==2.1.1
-	urllib3==1.26.15
 commands = pytest tests
 
-[testenv:py310-black]
+[testenv:py312-black]
 deps = black
 commands = black --check --diff .
 
-[testenv:py310-lint]
+[testenv:py312-lint]
 deps = pylint
 commands = pylint minfraud
 
-[testenv:py310-flake8]
+[testenv:py312-flake8]
 deps = flake8
 commands = flake8 minfraud
 
-[testenv:py310-mypy]
+[testenv:py312-mypy]
 deps = 
 	mypy
 	types-requests
 	voluptuous-stubs
 commands = mypy minfraud tests
 
 [egg_info]
```

### Comparing `minfraud-2.8.0/setup.py` & `minfraud-2.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,57 @@
-#!/usr/bin/env python
-
-import ast
-import io
-import os
-import re
-import sys
-
-from setuptools import setup
-
-_version_re = re.compile(r"__version__\s+=\s+(.*)")
-
-with io.open("minfraud/version.py", "r", encoding="utf-8") as f:
-    _version = str(ast.literal_eval(_version_re.search(f.read()).group(1)))
-
-with io.open("README.rst", "r", encoding="utf-8") as f:
-    _readme = f.read()
-
-requirements = [
+[project]
+name = "minfraud"
+version = "2.9.0"
+description = "MaxMind minFraud Score, Insights, Factors and Report Transactions API"
+authors = [
+    {name = "Gregory Oschwald", email = "goschwald@maxmind.com"},
+]
+dependencies = [
+    "setuptools>=60.0.0",
     "aiohttp>=3.6.2,<4.0.0",
-    "email_validator>=1.1.1,<3.0.0",
-    "geoip2>=4.7.0,<5.0.0",
+    "email_validator>=2.0.0,<3.0.0",
+    "geoip2>=4.8.0,<5.0.0",
     "requests>=2.24.0,<3.0.0",
     "voluptuous",
 ]
+requires-python = ">=3.8"
+readme = "README.rst"
+license = {text = "Apache License 2.0"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Internet",
+    "Topic :: Internet :: Proxy Servers",
+    "Topic :: Internet :: WWW/HTTP",
+]
+
+[project.optional-dependencies]
+test = [
+    "mocket>=3.11.1",
+]
+
+[tool.setuptools.package-data]
+minfraud = ["py.typed"]
 
-setup(
-    name="minfraud",
-    version=_version,
-    description="MaxMind minFraud Score, Insights, Factors and Report Transactions API",
-    long_description=_readme,
-    author="Gregory Oschwald",
-    author_email="goschwald@maxmind.com",
-    url="https://www.maxmind.com/",
-    packages=["minfraud"],
-    package_data={"minfraud": ["py.typed"]},
-    include_package_data=True,
-    platforms="any",
-    python_requires=">=3.7",
-    install_requires=requirements,
-    tests_require=["mocket>=3.8.6"],
-    test_suite="tests",
-    license="Apache License 2.0 ",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Web Environment",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python",
-        "Topic :: Internet :: Proxy Servers",
-        "Topic :: Internet :: WWW/HTTP",
-        "Topic :: Internet",
-    ],
-    project_urls={
-        "Documentation": "https://minfraud.readthedocs.org/",
-        "Source Code": "https://github.com/maxmind/minfraud-api-python",
-        "Issue Tracker": "https://github.com/maxmind/minfraud-api-python/issues",
-    },
-)
+[project.urls]
+Homepage = "https://www.maxmind.com/"
+Documentation = "https://minfraud.readthedocs.org/"
+"Source Code" = "https://github.com/maxmind/minfraud-api-python"
+"Issue Tracker" = "https://github.com/maxmind/minfraud-api-python/issues"
+
+[build-system]
+requires = ["setuptools", "setuptools-scm", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.black]
+# src is showing up in our GitHub linting builds. It seems to
+# contain deps.
+extend-exclude = '^/src/'
```

### Comparing `minfraud-2.8.0/tests/data/factors-response.json` & `minfraud-2.9.0/tests/data/factors-response.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998575498575499%*

 * *Differences: {"'ip_address'": "{'traits': {'connection_type': 'Cable/DSL'}}"}*

```diff
@@ -127,14 +127,15 @@
                     "es": "Inglaterra",
                     "fr": "Angleterre",
                     "pt-BR": "Inglaterra"
                 }
             }
         ],
         "traits": {
+            "connection_type": "Cable/DSL",
             "domain": "in-addr.arpa",
             "ip_address": "152.216.7.110",
             "is_anonymous": true,
             "is_anonymous_vpn": true,
             "is_hosting_provider": true,
             "is_public_proxy": true,
             "is_residential_proxy": true,
```

### Comparing `minfraud-2.8.0/tests/data/full-transaction-request.json` & `minfraud-2.9.0/tests/data/full-transaction-request.json`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/tests/data/insights-response.json` & `minfraud-2.9.0/tests/data/insights-response.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998456790123457%*

 * *Differences: {"'ip_address'": "{'traits': {'connection_type': 'Cable/DSL'}}"}*

```diff
@@ -127,14 +127,15 @@
                     "es": "Inglaterra",
                     "fr": "Angleterre",
                     "pt-BR": "Inglaterra"
                 }
             }
         ],
         "traits": {
+            "connection_type": "Cable/DSL",
             "domain": "in-addr.arpa",
             "ip_address": "152.216.7.110",
             "is_anonymous": true,
             "is_anonymous_vpn": true,
             "is_hosting_provider": true,
             "is_public_proxy": true,
             "is_residential_proxy": true,
```

### Comparing `minfraud-2.8.0/tests/data/score-response.json` & `minfraud-2.9.0/tests/data/score-response.json`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/tests/test_models.py` & `minfraud-2.9.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/tests/test_request.py` & `minfraud-2.9.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/tests/test_validation.py` & `minfraud-2.9.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `minfraud-2.8.0/tests/test_webservice.py` & `minfraud-2.9.0/tests/test_webservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,21 @@
     InsufficientFundsError,
     MinFraudError,
     PermissionRequiredError,
 )
 from minfraud.models import Factors, Insights, Score
 from minfraud.webservice import AsyncClient, Client
 
+import minfraud.webservice
 import unittest
 
+# We have this so that we can avoid a mocket issue:
+# https://github.com/mindflayer/python-mocket/issues/209
+minfraud.webservice._SCHEME = "http"
+
 
 class BaseTest(unittest.TestCase):
     client_class: Union[Type[AsyncClient], Type[Client]] = Client
 
     def setUp(self):
         self.client = self.client_class(42, "abcdef123456")
 
@@ -32,15 +37,15 @@
         with open(os.path.join(test_dir, self.request_file), encoding="utf-8") as file:
             content = file.read()
         self.full_request = json.loads(content)
 
         with open(os.path.join(test_dir, self.response_file), encoding="utf-8") as file:
             self.response = file.read()
 
-    base_uri = "https://minfraud.maxmind.com/minfraud/v2.0"
+    base_uri = "http://minfraud.maxmind.com/minfraud/v2.0"
 
     @httprettified
     def test_invalid_auth(self):
         for error in (
             "ACCOUNT_ID_REQUIRED",
             "AUTHORIZATION_INVALID",
             "LICENSE_KEY_REQUIRED",
```

