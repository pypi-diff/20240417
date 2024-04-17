# Comparing `tmp/openai-to-sqlite-0.4.tar.gz` & `tmp/openai_to_sqlite-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-to-sqlite-0.4.tar", last modified: Tue Aug 15 05:01:26 2023, max compression
+gzip compressed data, was "openai_to_sqlite-0.4.1.tar", last modified: Wed Apr 17 02:53:31 2024, max compression
```

## Comparing `openai-to-sqlite-0.4.tar` & `openai_to_sqlite-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/openai_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/openai_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/openai_to_sqlite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/openai_to_sqlite/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-15 05:01:26.000000 openai-to-sqlite-0.4/openai_to_sqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:01:26.465382 openai-to-sqlite-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-08-15 05:01:05.000000 openai-to-sqlite-0.4/tests/test_openai_to_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/openai_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/openai_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/openai_to_sqlite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/openai_to_sqlite/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:53:31.000000 openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:53:31.940353 openai_to_sqlite-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-17 02:53:24.000000 openai_to_sqlite-0.4.1/tests/test_openai_to_sqlite.py
```

### Comparing `openai-to-sqlite-0.4/LICENSE` & `openai_to_sqlite-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-to-sqlite-0.4/PKG-INFO` & `openai_to_sqlite-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-Metadata-Version: 2.1
-Name: openai-to-sqlite
-Version: 0.4
-Summary: Save OpenAI API results to a SQLite database
-Home-page: https://github.com/simonw/openai-to-sqlite
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
-Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
-Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # openai-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/main/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
 See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
 
+For a tutorial on using this for related content, see [Storing and serving related documents with openai-to-sqlite and embeddings](https://til.simonwillison.net/llms/openai-embeddings-related-content).
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install openai-to-sqlite
 ```
 ## Configuration
@@ -248,14 +235,17 @@
 openai-to-sqlite similar embeddings-bjcp-2021.db \
   '23G Gose' '01A American Light Lager'
 ```
 Or pass `--all` to run similarity for every item in the database. This runs similarity calculations for the number of items squared so it can be quite a long running operation:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all
 ```
+
+### Saving similarity calculations to the database
+
 To save these calculations to a `similarities` table in the database, use the `--save` option:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save
 ```
 The `--save` option disables output. You can re-enable output with `--print`:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save --print
```

### Comparing `openai-to-sqlite-0.4/README.md` & `openai_to_sqlite-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,43 @@
+Metadata-Version: 2.1
+Name: openai-to-sqlite
+Version: 0.4.1
+Summary: Save OpenAI API results to a SQLite database
+Home-page: https://github.com/simonw/openai-to-sqlite
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
+Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
+Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: httpx
+Requires-Dist: sqlite-utils>=3.28
+Requires-Dist: openai
+Requires-Dist: tiktoken
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-httpx; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+
 # openai-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/main/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
 See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
 
+For a tutorial on using this for related content, see [Storing and serving related documents with openai-to-sqlite and embeddings](https://til.simonwillison.net/llms/openai-embeddings-related-content).
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install openai-to-sqlite
 ```
 ## Configuration
@@ -233,14 +258,17 @@
 openai-to-sqlite similar embeddings-bjcp-2021.db \
   '23G Gose' '01A American Light Lager'
 ```
 Or pass `--all` to run similarity for every item in the database. This runs similarity calculations for the number of items squared so it can be quite a long running operation:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all
 ```
+
+### Saving similarity calculations to the database
+
 To save these calculations to a `similarities` table in the database, use the `--save` option:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save
 ```
 The `--save` option disables output. You can re-enable output with `--print`:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save --print
@@ -280,8 +308,8 @@
 Now install the dependencies and test dependencies:
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
-```
+```
```

### Comparing `openai-to-sqlite-0.4/openai_to_sqlite/cli.py` & `openai_to_sqlite-0.4.1/openai_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `openai-to-sqlite-0.4/openai_to_sqlite.egg-info/PKG-INFO` & `openai_to_sqlite-0.4.1/openai_to_sqlite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: openai-to-sqlite
-Version: 0.4
+Version: 0.4.1
 Summary: Save OpenAI API results to a SQLite database
 Home-page: https://github.com/simonw/openai-to-sqlite
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
 Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
 Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: httpx
+Requires-Dist: sqlite-utils>=3.28
+Requires-Dist: openai
+Requires-Dist: tiktoken
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-httpx; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 # openai-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/main/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
 See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
 
+For a tutorial on using this for related content, see [Storing and serving related documents with openai-to-sqlite and embeddings](https://til.simonwillison.net/llms/openai-embeddings-related-content).
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install openai-to-sqlite
 ```
 ## Configuration
@@ -248,14 +258,17 @@
 openai-to-sqlite similar embeddings-bjcp-2021.db \
   '23G Gose' '01A American Light Lager'
 ```
 Or pass `--all` to run similarity for every item in the database. This runs similarity calculations for the number of items squared so it can be quite a long running operation:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all
 ```
+
+### Saving similarity calculations to the database
+
 To save these calculations to a `similarities` table in the database, use the `--save` option:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save
 ```
 The `--save` option disables output. You can re-enable output with `--print`:
 ```bash
 openai-to-sqlite similar embeddings-bjcp-2021.db --all --save --print
```

### Comparing `openai-to-sqlite-0.4/setup.py` & `openai_to_sqlite-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4"
+VERSION = "0.4.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `openai-to-sqlite-0.4/tests/test_openai_to_sqlite.py` & `openai_to_sqlite-0.4.1/tests/test_openai_to_sqlite.py`

 * *Files identical despite different names*

