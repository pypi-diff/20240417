# Comparing `tmp/tarentula-4.3.4.tar.gz` & `tmp/tarentula-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarentula-4.3.4.tar", max compression
+gzip compressed data, was "tarentula-4.4.0.tar", max compression
```

## Comparing `tarentula-4.3.4.tar` & `tarentula-4.4.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    34551 2022-08-01 15:50:17.808633 tarentula-4.3.4/LICENSE
--rw-r--r--   0        0        0    19487 2023-06-05 12:24:17.517076 tarentula-4.3.4/README.md
--rw-r--r--   0        0        0      580 2023-06-05 12:33:13.411113 tarentula-4.3.4/pyproject.toml
--rw-r--r--   0        0        0       76 2022-12-14 10:46:14.379027 tarentula-4.3.4/tarentula/__init__.py
--rw-r--r--   0        0        0     3717 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/aggregate.py
--rw-r--r--   0        0        0    16649 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/cli.py
--rw-r--r--   0        0        0     1040 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/command.py
--rw-r--r--   0        0        0     1773 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/config_file_reader.py
--rw-r--r--   0        0        0     1822 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/count.py
--rw-r--r--   0        0        0    10601 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/datashare_client.py
--rw-r--r--   0        0        0     7274 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/download.py
--rw-r--r--   0        0        0     7266 2023-06-05 12:29:27.894104 tarentula-4.3.4/tarentula/export_by_query.py
--rw-r--r--   0        0        0     2474 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/graph_realtime.py
--rw-r--r--   0        0        0      964 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/logger.py
--rw-r--r--   0        0        0     3666 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/metadata_fields.py
--rw-r--r--   0        0        0     2574 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tag_cleaning_by_query.py
--rw-r--r--   0        0        0     5234 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tagging.py
--rw-r--r--   0        0        0     4979 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tagging_by_query.py
--rw-r--r--   0        0        0    20739 1970-01-01 00:00:00.000000 tarentula-4.3.4/setup.py
--rw-r--r--   0        0        0    20007 1970-01-01 00:00:00.000000 tarentula-4.3.4/PKG-INFO
+-rw-r--r--   0        0        0    34551 2024-02-19 17:44:20.651453 tarentula-4.4.0/LICENSE
+-rw-r--r--   0        0        0    19487 2024-02-19 17:44:20.651772 tarentula-4.4.0/README.md
+-rw-r--r--   0        0        0      573 2024-04-17 10:21:24.071115 tarentula-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-02-19 17:44:20.652620 tarentula-4.4.0/tarentula/__init__.py
+-rw-r--r--   0        0        0     3717 2024-02-19 17:44:20.652759 tarentula-4.4.0/tarentula/aggregate.py
+-rw-r--r--   0        0        0    16662 2024-02-19 17:44:20.652883 tarentula-4.4.0/tarentula/cli.py
+-rw-r--r--   0        0        0     1040 2024-02-19 17:44:20.652963 tarentula-4.4.0/tarentula/command.py
+-rw-r--r--   0        0        0     1773 2024-02-19 17:44:20.653042 tarentula-4.4.0/tarentula/config_file_reader.py
+-rw-r--r--   0        0        0     1822 2024-02-19 17:44:20.653151 tarentula-4.4.0/tarentula/count.py
+-rw-r--r--   0        0        0    10643 2024-04-17 10:16:47.784826 tarentula-4.4.0/tarentula/datashare_client.py
+-rw-r--r--   0        0        0     7274 2024-02-21 13:09:18.742676 tarentula-4.4.0/tarentula/download.py
+-rw-r--r--   0        0        0     7266 2024-02-19 17:44:20.653452 tarentula-4.4.0/tarentula/export_by_query.py
+-rw-r--r--   0        0        0     2474 2024-02-19 17:44:20.653538 tarentula-4.4.0/tarentula/graph_realtime.py
+-rw-r--r--   0        0        0      964 2024-02-19 17:44:20.653613 tarentula-4.4.0/tarentula/logger.py
+-rw-r--r--   0        0        0     3666 2024-02-19 17:44:20.653699 tarentula-4.4.0/tarentula/metadata_fields.py
+-rw-r--r--   0        0        0     2574 2024-02-19 17:44:20.653810 tarentula-4.4.0/tarentula/tag_cleaning_by_query.py
+-rw-r--r--   0        0        0     5234 2024-02-19 17:44:20.653903 tarentula-4.4.0/tarentula/tagging.py
+-rw-r--r--   0        0        0     4979 2024-02-19 17:44:20.654000 tarentula-4.4.0/tarentula/tagging_by_query.py
+-rw-r--r--   0        0        0    20096 1970-01-01 00:00:00.000000 tarentula-4.4.0/PKG-INFO
```

### Comparing `tarentula-4.3.4/LICENSE` & `tarentula-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/README.md` & `tarentula-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/pyproject.toml` & `tarentula-4.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "tarentula"
-version = "4.3.4"
+version = "4.4.0"
 description = ""
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "tarentula"}]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.8"
 click = "^8.1"
 requests = "^2.28"
 coloredlogs = "==14.0"
 rich = "^12"
+pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 responses = "^0.22"
-pyyaml = "==5.4.0"
 argh = "==0.26.2"
 pytest = "^7.2.0"
 matplotlib = "^3.6"
 pylint = "^2.17.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `tarentula-4.3.4/tarentula/aggregate.py` & `tarentula-4.4.0/tarentula/aggregate.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/cli.py` & `tarentula-4.4.0/tarentula/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 @click.option('--sort-by', help='Field to use to sort results', default='_id')
 @click.option('--order-by', help='Order to use to sort results', default='asc',
               type=click.Choice(['asc', 'desc']))
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
               callback=validate_progressbar)
 @click.option('--type', help='Type of indexed documents to download', default='Document',
-              type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
+              type=click.Choice(['Document', 'NamedEntity', 'Duplicate'], case_sensitive=True))
 @click.option('--size', help='Size of the scroll request that powers the operation.', default=1000)
 @click.option('--from', '-f', 'from_', type=int, help='Passed to the search it will bypass the first n documents',
               default=0)
 @click.option('--limit', '-l', type=int, help='Limit the total results to return', default=0)
 @click.option('--query-field/--no-query-field', help='Add the query to the export CSV', default=True)
 def export_by_query(**options):
     # Instantiate an ExportByQuery class with all the options
```

### Comparing `tarentula-4.3.4/tarentula/command.py` & `tarentula-4.4.0/tarentula/command.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/config_file_reader.py` & `tarentula-4.4.0/tarentula/config_file_reader.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/count.py` & `tarentula-4.4.0/tarentula/count.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/datashare_client.py` & `tarentula-4.4.0/tarentula/datashare_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         url = urljoin(self.elasticsearch_host, index, '_mappings')
         return requests.get(url,
                             cookies=self.cookies,
                             headers=self.headers, timeout=HTTP_REQUEST_TIMEOUT_SEC).json()
 
     def count(self, index=DATASHARE_DEFAULT_PROJECT, query=None):
         if query is None: query = {}
+        query = {'query': query['query']}
         url = urljoin(self.elasticsearch_host, index, '_count')
         return requests.post(url, json=query,
                              cookies=self.cookies,
                              headers=self.headers, timeout=HTTP_REQUEST_TIMEOUT_SEC).json()
 
     def document(self, index=DATASHARE_DEFAULT_PROJECT, id=None, routing=None, source=None):
         url = urljoin(self.elasticsearch_host, index, '/_doc/', id)
```

### Comparing `tarentula-4.3.4/tarentula/download.py` & `tarentula-4.4.0/tarentula/download.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/export_by_query.py` & `tarentula-4.4.0/tarentula/export_by_query.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/graph_realtime.py` & `tarentula-4.4.0/tarentula/graph_realtime.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/logger.py` & `tarentula-4.4.0/tarentula/logger.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/metadata_fields.py` & `tarentula-4.4.0/tarentula/metadata_fields.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/tag_cleaning_by_query.py` & `tarentula-4.4.0/tarentula/tag_cleaning_by_query.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/tagging.py` & `tarentula-4.4.0/tarentula/tagging.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/tarentula/tagging_by_query.py` & `tarentula-4.4.0/tarentula/tagging_by_query.py`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.4/setup.py` & `tarentula-4.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,504 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tarentula
+Version: 4.4.0
+Summary: 
+Author: ICIJ
+Author-email: engineering@icij.org
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: coloredlogs (==14.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: rich (>=12,<13)
+Description-Content-Type: text/markdown
 
-packages = \
-['tarentula']
+# Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula)
 
-package_data = \
-{'': ['*']}
+Cli toolbelt for [Datashare](https://datashare.icij.org).
 
-install_requires = \
-['click>=8.1,<9.0', 'coloredlogs==14.0', 'requests>=2.28,<3.0', 'rich>=12,<13']
-
-entry_points = \
-{'console_scripts': ['tarentula = tarentula.cli:cli']}
-
-setup_kwargs = {
-    'name': 'tarentula',
-    'version': '4.3.4',
-    'description': '',
-    'long_description': '# Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula)\n\nCli toolbelt for [Datashare](https://datashare.icij.org).\n\n```\n     /      \\\n  \\  \\  ,,  /  /\n   \'-.`\\()/`.-\'\n  .--_\'(  )\'_--.\n / /` /`""`\\ `\\ \\\n  |  |  ><  |  |\n  \\  \\      /  /\n      \'.__.\'\n\nUsage: tarentula [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --syslog-address      TEXT    localhost   Syslog address\n  --syslog-port         INTEGER 514         Syslog port\n  --syslog-facility     TEXT    local7      Syslog facility\n  --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler\n  --help                                    Show this message and exit\n  --version                                 Show the installed version of Tarentula\n\nCommands:\n  aggregate\n  count\n  clean-tags-by-query\n  download\n  export-by-query\n  list-metadata\n  tagging\n  tagging-by-query\n```\n\n---\n<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->\n\n- [Installation](#installation)\n- [Usage](#usage)\n  - [Cookbook 👩\u200d🍳](#cookbook-)\n  - [Count](#count)\n  - [Clean Tags by Query](#clean-tags-by-query)\n  - [Download](#download)\n  - [Export by Query](#export-by-query)\n  - [Tagging](#tagging)\n    - [CSV formats](#csv-formats)\n  - [Tagging by Query](#tagging-by-query)\n  - [Aggregate](#aggregate)\n  - [Following your changes](#following-your-changes)\n- [Configuration File](#configuration-file)\n- [Testing](#testing)\n- [Releasing](#releasing)\n  - [1. Create a new release](#1-create-a-new-release)\n  - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)\n  - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)\n  - [4. Push your changes on Github](#4-push-your-changes-on-github)\n\n<!-- /TOC -->\n---\n\n## Installation\n\nYou can insatll Datashare Tarentula with your favorite package manager:\n\n```\npip3 install --user tarentula\n```\n\nOr alternativly with Docker:\n\n```\ndocker run icij/datashare-tarentula\n```\n\n## Usage\n\nDatashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.\n\n### Cookbook 👩\u200d🍳\n\nTo learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.\n\n### Count\n\nA command to just count the number of files matching a query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n  --datashare-url           TEXT        Datashare URL\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        You can additionally pass the Elasticsearch\n                                          URL in order to use scrollingcapabilities of\n                                          Elasticsearch (useful when dealing with a\n                                          lot of results)\n  --query                   TEXT        The query string to filter documents\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n                                          in the downloaded document from the index\n  --traceback / --no-traceback          Display a traceback in case of error\n  --type [Document|NamedEntity]         Type of indexed documents to download\n  --help                                Show this message and exit\n```\n\n### Clean Tags by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch untag documents directly in the index.\n\n```\nUsage: tarentula clean-tags-by-query [OPTIONS]\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --query                   TEXT        Give a JSON query to filter documents that\n                                          will have their tags cleaned. It can be\n                                          afile with @path/to/file. Default to all.\n  --help                                Show this message and exit\n```\n\n### Download\n\nA command to download all files matching a query.\n\n```\nUsage: tarentula download [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --destination-directory TEXT    Directory documents will be downloaded\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --path-format TEXT              Downloaded document path template\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the downloaded document from the index\n\n  -f, --from INTEGER              Passed to the search it will bypass the\n                                  first n documents\n  -l, --limit INTEGER             Limit the total results to return\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --once / --not-once             Download file only once\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --raw-file / --no-raw-file      Download raw file from Datashare\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --help                          Show this message and exit.\n```\n\n\n### Export by Query\n\nA command to export all files matching a query.\n\n```\nUsage: tarentula export-by-query [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --output-file TEXT              Path to the CSV file\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the export\n\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  -f, --from INTEGER              Passed to the search it will bypass the\n                                  first n documents\n  -l, --limit INTEGER             Limit the total results to return\n  --size INTEGER                  Size of the scroll request that powers the\n                                  operation.\n\n  --query-field / --no-query-field\n                                  Add the query to the export CSV\n  --help                          Show this message and exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents with a CSV file.\n\n```\nUsage: tarentula tagging [OPTIONS] CSV_PATH\n\nOptions:\n  --datashare-url       TEXT        http://localhost:8080   Datashare URL\n  --datashare-project   TEXT        local-datashare         Datashare project\n  --throttle            INTEGER     0                       Request throttling (in ms)\n  --cookies             TEXT        _Empty string_          Key/value pair to add a cookie to each request to the API. You can separate semicolons: key1=val1;key2=val2;...\n  --apikey              TEXT        None                    Datashare authentication apikey\n  --traceback / --no-traceback                              Display a traceback in case of error\n  --progressbar / --no-progressbar                          Display a progressbar\n  --help                                                    Show this message and exit\n```\n\n#### CSV formats\n\nTagging with a `documentId` and `routing`:\n\n```csv\ntag,documentId,routing\nActinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG\nAntrodiaetidae,DWLOskax28jPQ2CjFrCo\nAtracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN\nAtypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\nBarychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\n```\n\nTagging with a `documentUrl`:\n\n```csv\ntag,documentUrl\nMecicobothriidae,http://localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi\nMicrostigmatidae,http://localhost:8080/#/d/local-datashare/iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0\nMigidae,http://localhost:8080/#/d/local-datashare/BmovvXBisWtyyx6o9cuG/BmovvXBisWtyyx6o9cuG\nNemesiidae,http://localhost:8080/#/d/local-datashare/vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN\nParatropididae,http://localhost:8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/vYl1C4bsWphUKvXEBDhM\nPorrhothelidae,http://localhost:8080/#/d/local-datashare/fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp\nTheraphosidae,http://localhost:8080/#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu\n```\n\n### Tagging by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch tag documents directly in the index.\n\nTo see an example of input file, refer to [this JSON](tests/fixtures/tags-by-content-type.json).\n\n```\nUsage: tarentula tagging-by-query [OPTIONS] JSON_PATH\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --throttle                INTEGER     Request throttling (in ms)\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --progressbar / --no-progressbar      Display a progressbar\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --help                                Show this message and exit\n```\n\n\n### List Metadata\n\nYou can list the metadata from the mapping, optionally counting the number of occurrences of each field in the index, with the `--count` parameter. Counting the fields is disabled by default.\n\nIt includes a `--filter_by` parameter to narrow retrieving metadata properties of specific sets of documents. For instance it can be used to get just emails related properties with: `--filter_by "contentType=message/rfc822"`\n\n```\n$ tarentula list-metadata --help\nUsage: tarentula list-metadata [OPTIONS]\n\nOptions:\n  --datashare-project TEXT       Datashare project\n  --elasticsearch-url TEXT       You can additionally pass the Elasticsearch\n                                 URL in order to use scrollingcapabilities of\n                                 Elasticsearch (useful when dealing with a lot\n                                 of results)\n  --type [Document|NamedEntity]  Type of indexed documents to get metadata\n  --filter_by TEXT               Filter documents by pairs concatenated by\n                                 coma of field names and values separated by\n                                 =.Example "contentType=message/rfc822,content\n                                 Type=message/rfc822"\n  --count / --no-count           Count or not the number of docs for each\n                                 property found\n\n  --help                         Show this message and exit.\n\n```\n\n### Aggregate\n\nYou can run aggregations on the data, the ElasticSearch aggregations API is partially enabled with this command.\nThe possibilities are:\n\n- count: grouping by a given field different values, and count the num of docs.\n- nunique: returns the number of unique values of a given field.\n- date_histogram: returns counting of monthly or yearly grouped values for a given date field.\n- sum: returns the sum of values of number type fields.\n- min: returns the min of values of number type fields.\n- max: returns the max of values of number type fields.\n- avg: returns the average of values of number type fields.\n- stats: returns a bunch of statistics for a given number type fields.\n- string_stats: returns a bunch of string statistics for a given string type fields.\n\n\n\n```\n$ tarentula aggregate --help\nUsage: tarentula aggregate [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n  --query TEXT                    The query string to filter documents\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n  --traceback / --no-traceback    Display a traceback in case of error\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --group_by TEXT                 Field to use to aggregate results\n  --operation_field TEXT          Field to run the operation on\n  --run [count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]\n                                  Operation to run\n  --calendar_interval [year|month]\n                                  Calendar interval for date histogram\n                                  aggregation\n  --help                          Show this message and exit.\n```\n\n### Following your changes\n\nWhen running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.\n\nIt uses [mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf you see the following message :\n\n```\n$ graph_es\ngraph_realtime.py:32: UserWarning: Matplotlib is currently using agg, which is a non-GUI backend, so cannot show the figure\n```\n\nThen you have to install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.\n\nThe command has the options below:\n\n```\n$ graph_es --help\nUsage: graph_es [OPTIONS]\n\nOptions:\n  --query               TEXT        Give a JSON query to filter documents. It can be\n                                      a file with @path/to/file. Default to all.\n  --index               TEXT        Elasticsearch index (default local-datashare)\n  --refresh-interval    INTEGER     Graph refresh interval in seconds (default 5s)\n  --field               TEXT        Field value to display over time (default "hits.total")\n  --elasticsearch-url   TEXT        Elasticsearch URL which is used to perform\n                                      update by query (default http://elasticsearch:9200)\n```\n\n## Configuration File\n\nTarentula supports several sources for configuring its behavior, including an ini files and command-line options.\n\nConfiguration file will be searched for in the following order (use the first file found, all others are ignored):\n\n  * `TARENTULA_CONFIG` (environment variable if set)\n  * `tarentula.ini` (in the current directory)\n  * `~/.tarentula.ini` (in the home directory)\n  * `/etc/tarentula/tarentula.ini`\n\nIt should follow the following format (all values bellow are optional):\n\n```\n[DEFAULT]\napikey = SECRETHALONOPROCTIDAE\ndatashare_url = http://here:8080\ndatashare_project = local-datashare\n\n[logger]\nsyslog_address = 127.0.0.0\nsyslog_port = 514\nsyslog_facility = local7\nstdout_loglevel = INFO\n```\n\n## Testing\n\nTo test this tool, you must have Datashare and Elasticsearch running on your development machine.\n\nAfter you [installed Datashare](https://datashare.icij.org/), just run it with a test project/user:\n\n```\ndatashare -p test-datashare -u test\n```\n\nIn a separate terminal, install the development dependencies:\n\n```\nmake install\n```\n\nFinally, run the test\n\n```\nmake test\n```\n\n\n## Releasing\n\nThe releasing process uses [bumpversion](https://pypi.org/project/bumpversion/) to manage versions of this package, [pypi](https://pypi.org/project/tarentula/) to publish the Python package and [Docker Hub](https://hub.docker.com/) for the Docker image.\n\n### 1. Create a new release\n\n```\nmake [patch|minor|major]\n```\n\n### 2. Upload distributions on pypi\n\n_To be able to do this, you will need to be a maintainer of the [pypi](https://pypi.org/project/tarentula/) project._\n\n```\nmake distribute\n```\n\n### 3. Build and publish the Docker image\n\nTo build and upload a new image on the [docker repository](https://hub.docker.com/repository/docker/icij/datashare-tarentula) :\n\n_To be able to do this, you will need to be part of the ICIJ organization on docker_\n\n```\nmake docker-publish\n```\n\n**Note**: Datashare Tarentula is a multi-platform build. You might need to setup your environment for \nmulti-platform using the `make docker-setup-multiarch` command. Read more \n[on Docker documentation](https://docs.docker.com/build/building/multi-platform/). \n\n### 4. Push your changes on Github\n\nGit push release and tag :\n\n```\ngit push origin master --tags\n```\n',
-    'author': 'ICIJ',
-    'author_email': 'engineering@icij.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+```
+     /      \
+  \  \  ,,  /  /
+   '-.`\()/`.-'
+  .--_'(  )'_--.
+ / /` /`""`\ `\ \
+  |  |  ><  |  |
+  \  \      /  /
+      '.__.'
 
+Usage: tarentula [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --syslog-address      TEXT    localhost   Syslog address
+  --syslog-port         INTEGER 514         Syslog port
+  --syslog-facility     TEXT    local7      Syslog facility
+  --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler
+  --help                                    Show this message and exit
+  --version                                 Show the installed version of Tarentula
+
+Commands:
+  aggregate
+  count
+  clean-tags-by-query
+  download
+  export-by-query
+  list-metadata
+  tagging
+  tagging-by-query
+```
+
+---
+<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Cookbook 👩‍🍳](#cookbook-)
+  - [Count](#count)
+  - [Clean Tags by Query](#clean-tags-by-query)
+  - [Download](#download)
+  - [Export by Query](#export-by-query)
+  - [Tagging](#tagging)
+    - [CSV formats](#csv-formats)
+  - [Tagging by Query](#tagging-by-query)
+  - [Aggregate](#aggregate)
+  - [Following your changes](#following-your-changes)
+- [Configuration File](#configuration-file)
+- [Testing](#testing)
+- [Releasing](#releasing)
+  - [1. Create a new release](#1-create-a-new-release)
+  - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)
+  - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)
+  - [4. Push your changes on Github](#4-push-your-changes-on-github)
+
+<!-- /TOC -->
+---
+
+## Installation
+
+You can insatll Datashare Tarentula with your favorite package manager:
+
+```
+pip3 install --user tarentula
+```
+
+Or alternativly with Docker:
+
+```
+docker run icij/datashare-tarentula
+```
+
+## Usage
+
+Datashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.
+
+### Cookbook 👩‍🍳
+
+To learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.
+
+### Count
+
+A command to just count the number of files matching a query.
+
+```
+Usage: tarentula count [OPTIONS]
+
+Options:
+  --datashare-url           TEXT        Datashare URL
+  --datashare-project       TEXT        Datashare project
+  --elasticsearch-url       TEXT        You can additionally pass the Elasticsearch
+                                          URL in order to use scrollingcapabilities of
+                                          Elasticsearch (useful when dealing with a
+                                          lot of results)
+  --query                   TEXT        The query string to filter documents
+  --cookies                 TEXT        Key/value pair to add a cookie to each
+                                          request to the API. You can
+                                          separatesemicolons: key1=val1;key2=val2;...
+  --apikey                  TEXT        Datashare authentication apikey
+                                          in the downloaded document from the index
+  --traceback / --no-traceback          Display a traceback in case of error
+  --type [Document|NamedEntity]         Type of indexed documents to download
+  --help                                Show this message and exit
+```
+
+### Clean Tags by Query
+
+A command that uses Elasticsearch `update-by-query` feature to batch untag documents directly in the index.
+
+```
+Usage: tarentula clean-tags-by-query [OPTIONS]
+
+Options:
+  --datashare-project       TEXT        Datashare project
+  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform
+                                          update by query
+  --cookies                 TEXT        Key/value pair to add a cookie to each
+                                          request to the API. You can
+                                          separatesemicolons: key1=val1;key2=val2;...
+  --apikey                  TEXT        Datashare authentication apikey
+  --traceback / --no-traceback          Display a traceback in case of error
+  --wait-for-completion / --no-wait-for-completion
+                                        Create a Elasticsearch task to perform the
+                                          updateasynchronously
+  --query                   TEXT        Give a JSON query to filter documents that
+                                          will have their tags cleaned. It can be
+                                          afile with @path/to/file. Default to all.
+  --help                                Show this message and exit
+```
+
+### Download
+
+A command to download all files matching a query.
+
+```
+Usage: tarentula download [OPTIONS]
+
+Options:
+  --apikey TEXT                   Datashare authentication apikey
+  --datashare-url TEXT            Datashare URL
+  --datashare-project TEXT        Datashare project
+  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch
+                                  URL in order to use scrollingcapabilities of
+                                  Elasticsearch (useful when dealing with a
+                                  lot of results)
+
+  --query TEXT                    The query string to filter documents
+  --destination-directory TEXT    Directory documents will be downloaded
+  --throttle INTEGER              Request throttling (in ms)
+  --cookies TEXT                  Key/value pair to add a cookie to each
+                                  request to the API. You can
+                                  separatesemicolons: key1=val1;key2=val2;...
+
+  --path-format TEXT              Downloaded document path template
+  --scroll TEXT                   Scroll duration
+  --source TEXT                   A comma-separated list of field to include
+                                  in the downloaded document from the index
+
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
+  --sort-by TEXT                  Field to use to sort results
+  --order-by [asc|desc]           Order to use to sort results
+  --once / --not-once             Download file only once
+  --traceback / --no-traceback    Display a traceback in case of error
+  --progressbar / --no-progressbar
+                                  Display a progressbar
+  --raw-file / --no-raw-file      Download raw file from Datashare
+  --type [Document|NamedEntity]   Type of indexed documents to download
+  --help                          Show this message and exit.
+```
+
+
+### Export by Query
+
+A command to export all files matching a query.
+
+```
+Usage: tarentula export-by-query [OPTIONS]
+
+Options:
+  --apikey TEXT                   Datashare authentication apikey
+  --datashare-url TEXT            Datashare URL
+  --datashare-project TEXT        Datashare project
+  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch
+                                  URL in order to use scrollingcapabilities of
+                                  Elasticsearch (useful when dealing with a
+                                  lot of results)
+
+  --query TEXT                    The query string to filter documents
+  --output-file TEXT              Path to the CSV file
+  --throttle INTEGER              Request throttling (in ms)
+  --cookies TEXT                  Key/value pair to add a cookie to each
+                                  request to the API. You can
+                                  separatesemicolons: key1=val1;key2=val2;...
+
+  --scroll TEXT                   Scroll duration
+  --source TEXT                   A comma-separated list of field to include
+                                  in the export
+
+  --sort-by TEXT                  Field to use to sort results
+  --order-by [asc|desc]           Order to use to sort results
+  --traceback / --no-traceback    Display a traceback in case of error
+  --progressbar / --no-progressbar
+                                  Display a progressbar
+  --type [Document|NamedEntity]   Type of indexed documents to download
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
+  --size INTEGER                  Size of the scroll request that powers the
+                                  operation.
+
+  --query-field / --no-query-field
+                                  Add the query to the export CSV
+  --help                          Show this message and exit.
+```
+
+
+### Tagging
+
+A command to batch tag documents with a CSV file.
+
+```
+Usage: tarentula tagging [OPTIONS] CSV_PATH
+
+Options:
+  --datashare-url       TEXT        http://localhost:8080   Datashare URL
+  --datashare-project   TEXT        local-datashare         Datashare project
+  --throttle            INTEGER     0                       Request throttling (in ms)
+  --cookies             TEXT        _Empty string_          Key/value pair to add a cookie to each request to the API. You can separate semicolons: key1=val1;key2=val2;...
+  --apikey              TEXT        None                    Datashare authentication apikey
+  --traceback / --no-traceback                              Display a traceback in case of error
+  --progressbar / --no-progressbar                          Display a progressbar
+  --help                                                    Show this message and exit
+```
+
+#### CSV formats
+
+Tagging with a `documentId` and `routing`:
+
+```csv
+tag,documentId,routing
+Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
+Antrodiaetidae,DWLOskax28jPQ2CjFrCo
+Atracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN
+Atypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi
+Barychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi
+```
+
+Tagging with a `documentUrl`:
+
+```csv
+tag,documentUrl
+Mecicobothriidae,http://localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi
+Microstigmatidae,http://localhost:8080/#/d/local-datashare/iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0
+Migidae,http://localhost:8080/#/d/local-datashare/BmovvXBisWtyyx6o9cuG/BmovvXBisWtyyx6o9cuG
+Nemesiidae,http://localhost:8080/#/d/local-datashare/vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN
+Paratropididae,http://localhost:8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/vYl1C4bsWphUKvXEBDhM
+Porrhothelidae,http://localhost:8080/#/d/local-datashare/fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp
+Theraphosidae,http://localhost:8080/#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu
+```
+
+### Tagging by Query
+
+A command that uses Elasticsearch `update-by-query` feature to batch tag documents directly in the index.
+
+To see an example of input file, refer to [this JSON](tests/fixtures/tags-by-content-type.json).
+
+```
+Usage: tarentula tagging-by-query [OPTIONS] JSON_PATH
+
+Options:
+  --datashare-project       TEXT        Datashare project
+  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform
+                                          update by query
+  --throttle                INTEGER     Request throttling (in ms)
+  --cookies                 TEXT        Key/value pair to add a cookie to each
+                                          request to the API. You can
+                                          separatesemicolons: key1=val1;key2=val2;...
+  --apikey                  TEXT        Datashare authentication apikey
+  --traceback / --no-traceback          Display a traceback in case of error
+  --progressbar / --no-progressbar      Display a progressbar
+  --wait-for-completion / --no-wait-for-completion
+                                        Create a Elasticsearch task to perform the
+                                          updateasynchronously
+  --help                                Show this message and exit
+```
+
+
+### List Metadata
+
+You can list the metadata from the mapping, optionally counting the number of occurrences of each field in the index, with the `--count` parameter. Counting the fields is disabled by default.
+
+It includes a `--filter_by` parameter to narrow retrieving metadata properties of specific sets of documents. For instance it can be used to get just emails related properties with: `--filter_by "contentType=message/rfc822"`
+
+```
+$ tarentula list-metadata --help
+Usage: tarentula list-metadata [OPTIONS]
+
+Options:
+  --datashare-project TEXT       Datashare project
+  --elasticsearch-url TEXT       You can additionally pass the Elasticsearch
+                                 URL in order to use scrollingcapabilities of
+                                 Elasticsearch (useful when dealing with a lot
+                                 of results)
+  --type [Document|NamedEntity]  Type of indexed documents to get metadata
+  --filter_by TEXT               Filter documents by pairs concatenated by
+                                 coma of field names and values separated by
+                                 =.Example "contentType=message/rfc822,content
+                                 Type=message/rfc822"
+  --count / --no-count           Count or not the number of docs for each
+                                 property found
+
+  --help                         Show this message and exit.
+
+```
+
+### Aggregate
+
+You can run aggregations on the data, the ElasticSearch aggregations API is partially enabled with this command.
+The possibilities are:
+
+- count: grouping by a given field different values, and count the num of docs.
+- nunique: returns the number of unique values of a given field.
+- date_histogram: returns counting of monthly or yearly grouped values for a given date field.
+- sum: returns the sum of values of number type fields.
+- min: returns the min of values of number type fields.
+- max: returns the max of values of number type fields.
+- avg: returns the average of values of number type fields.
+- stats: returns a bunch of statistics for a given number type fields.
+- string_stats: returns a bunch of string statistics for a given string type fields.
+
+
+
+```
+$ tarentula aggregate --help
+Usage: tarentula aggregate [OPTIONS]
+
+Options:
+  --apikey TEXT                   Datashare authentication apikey
+  --datashare-url TEXT            Datashare URL
+  --datashare-project TEXT        Datashare project
+  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch
+                                  URL in order to use scrollingcapabilities of
+                                  Elasticsearch (useful when dealing with a
+                                  lot of results)
+  --query TEXT                    The query string to filter documents
+  --cookies TEXT                  Key/value pair to add a cookie to each
+                                  request to the API. You can
+                                  separatesemicolons: key1=val1;key2=val2;...
+  --traceback / --no-traceback    Display a traceback in case of error
+  --type [Document|NamedEntity]   Type of indexed documents to download
+  --group_by TEXT                 Field to use to aggregate results
+  --operation_field TEXT          Field to run the operation on
+  --run [count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]
+                                  Operation to run
+  --calendar_interval [year|month]
+                                  Calendar interval for date histogram
+                                  aggregation
+  --help                          Show this message and exit.
+```
+
+### Following your changes
+
+When running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.
+
+It uses [mathplotlib](https://matplotlib.org/) and python3-tk.
+
+If you see the following message :
+
+```
+$ graph_es
+graph_realtime.py:32: UserWarning: Matplotlib is currently using agg, which is a non-GUI backend, so cannot show the figure
+```
+
+Then you have to install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.
+
+The command has the options below:
+
+```
+$ graph_es --help
+Usage: graph_es [OPTIONS]
+
+Options:
+  --query               TEXT        Give a JSON query to filter documents. It can be
+                                      a file with @path/to/file. Default to all.
+  --index               TEXT        Elasticsearch index (default local-datashare)
+  --refresh-interval    INTEGER     Graph refresh interval in seconds (default 5s)
+  --field               TEXT        Field value to display over time (default "hits.total")
+  --elasticsearch-url   TEXT        Elasticsearch URL which is used to perform
+                                      update by query (default http://elasticsearch:9200)
+```
+
+## Configuration File
+
+Tarentula supports several sources for configuring its behavior, including an ini files and command-line options.
+
+Configuration file will be searched for in the following order (use the first file found, all others are ignored):
+
+  * `TARENTULA_CONFIG` (environment variable if set)
+  * `tarentula.ini` (in the current directory)
+  * `~/.tarentula.ini` (in the home directory)
+  * `/etc/tarentula/tarentula.ini`
+
+It should follow the following format (all values bellow are optional):
+
+```
+[DEFAULT]
+apikey = SECRETHALONOPROCTIDAE
+datashare_url = http://here:8080
+datashare_project = local-datashare
+
+[logger]
+syslog_address = 127.0.0.0
+syslog_port = 514
+syslog_facility = local7
+stdout_loglevel = INFO
+```
+
+## Testing
+
+To test this tool, you must have Datashare and Elasticsearch running on your development machine.
+
+After you [installed Datashare](https://datashare.icij.org/), just run it with a test project/user:
+
+```
+datashare -p test-datashare -u test
+```
+
+In a separate terminal, install the development dependencies:
+
+```
+make install
+```
+
+Finally, run the test
+
+```
+make test
+```
+
+
+## Releasing
+
+The releasing process uses [bumpversion](https://pypi.org/project/bumpversion/) to manage versions of this package, [pypi](https://pypi.org/project/tarentula/) to publish the Python package and [Docker Hub](https://hub.docker.com/) for the Docker image.
+
+### 1. Create a new release
+
+```
+make [patch|minor|major]
+```
+
+### 2. Upload distributions on pypi
+
+_To be able to do this, you will need to be a maintainer of the [pypi](https://pypi.org/project/tarentula/) project._
+
+```
+make distribute
+```
+
+### 3. Build and publish the Docker image
+
+To build and upload a new image on the [docker repository](https://hub.docker.com/repository/docker/icij/datashare-tarentula) :
+
+_To be able to do this, you will need to be part of the ICIJ organization on docker_
+
+```
+make docker-publish
+```
+
+**Note**: Datashare Tarentula is a multi-platform build. You might need to setup your environment for 
+multi-platform using the `make docker-setup-multiarch` command. Read more 
+[on Docker documentation](https://docs.docker.com/build/building/multi-platform/). 
+
+### 4. Push your changes on Github
+
+Git push release and tag :
+
+```
+git push origin master --tags
+```
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,225 +1,214 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['tarentula']
-package_data = \ {'': ['*']} install_requires = \ ['click>=8.1,<9.0',
-'coloredlogs==14.0', 'requests>=2.28,<3.0', 'rich>=12,<13'] entry_points = \
-{'console_scripts': ['tarentula = tarentula.cli:cli']} setup_kwargs = { 'name':
-'tarentula', 'version': '4.3.4', 'description': '', 'long_description': '#
-Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-
-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-
-tarentula)\n\nCli toolbelt for [Datashare](https://
-datashare.icij.org).\n\n```\n / \\\n \\ \\ ,, / /\n \'-.`\\()/`.-\'\n .--_\'
-( )\'_--.\n / /` /`""`\\ `\\ \\\n | | >< | |\n \\ \\ / /\n \'.__.\'\n\nUsage:
-tarentula [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n --syslog-address TEXT
-localhost Syslog address\n --syslog-port INTEGER 514 Syslog port\n --syslog-
-facility TEXT local7 Syslog facility\n --stdout-loglevel TEXT ERROR Change the
-default log level for stdout error handler\n --help Show this message and
-exit\n --version Show the installed version of Tarentula\n\nCommands:\n
-aggregate\n count\n clean-tags-by-query\n download\n export-by-query\n list-
-metadata\n tagging\n tagging-by-query\n```\n\n---\n\n\n- [Installation]
-(#installation)\n- [Usage](#usage)\n - [Cookbook ð©\u200dð³](#cookbook-)\n
-- [Count](#count)\n - [Clean Tags by Query](#clean-tags-by-query)\n -
-[Download](#download)\n - [Export by Query](#export-by-query)\n - [Tagging]
-(#tagging)\n - [CSV formats](#csv-formats)\n - [Tagging by Query](#tagging-by-
-query)\n - [Aggregate](#aggregate)\n - [Following your changes](#following-
-your-changes)\n- [Configuration File](#configuration-file)\n- [Testing]
-(#testing)\n- [Releasing](#releasing)\n - [1. Create a new release](#1-create-
-a-new-release)\n - [2. Upload distributions on pypi](#2-upload-distributions-
-on-pypi)\n - [3. Build and publish the Docker image](#3-build-and-publish-the-
-docker-image)\n - [4. Push your changes on Github](#4-push-your-changes-on-
-github)\n\n\n---\n\n## Installation\n\nYou can insatll Datashare Tarentula with
-your favorite package manager:\n\n```\npip3 install --user tarentula\n```\n\nOr
-alternativly with Docker:\n\n```\ndocker run icij/datashare-
-tarentula\n```\n\n## Usage\n\nDatashare Tarentula comes with basic commands to
-interact with a Datashare instance (running locally or on a remote server).
-Primarily focus on bulk actions, it provides you with both a cli interface and
-a python API.\n\n### Cookbook ð©\u200dð³\n\nTo learn more about how to use
-Datashare Tarentula with a list of examples, please refer to _t_h_e
-_C_o_o_k_b_o_o_k.\n\n### Count\n\nA command to just count the number of files matching
-a query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n --datashare-url
-TEXT Datashare URL\n --datashare-project TEXT Datashare project\n --
-elasticsearch-url TEXT You can additionally pass the Elasticsearch\n URL in
-order to use scrollingcapabilities of\n Elasticsearch (useful when dealing with
-a\n lot of results)\n --query TEXT The query string to filter documents\n --
-cookies TEXT Key/value pair to add a cookie to each\n request to the API. You
-can\n separatesemicolons: key1=val1;key2=val2;...\n --apikey TEXT Datashare
-authentication apikey\n in the downloaded document from the index\n --traceback
-/ --no-traceback Display a traceback in case of error\n --type
-[Document|NamedEntity] Type of indexed documents to download\n --help Show this
-message and exit\n```\n\n### Clean Tags by Query\n\nA command that uses
-Elasticsearch `update-by-query` feature to batch untag documents directly in
-the index.\n\n```\nUsage: tarentula clean-tags-by-query [OPTIONS]\n\nOptions:\n
---datashare-project TEXT Datashare project\n --elasticsearch-url TEXT
-Elasticsearch URL which is used to perform\n update by query\n --cookies TEXT
-Key/value pair to add a cookie to each\n request to the API. You can\n
-separatesemicolons: key1=val1;key2=val2;...\n --apikey TEXT Datashare
-authentication apikey\n --traceback / --no-traceback Display a traceback in
-case of error\n --wait-for-completion / --no-wait-for-completion\n Create a
-Elasticsearch task to perform the\n updateasynchronously\n --query TEXT Give a
-JSON query to filter documents that\n will have their tags cleaned. It can be\n
-afile with @path/to/file. Default to all.\n --help Show this message and
-exit\n```\n\n### Download\n\nA command to download all files matching a
-query.\n\n```\nUsage: tarentula download [OPTIONS]\n\nOptions:\n --apikey TEXT
-Datashare authentication apikey\n --datashare-url TEXT Datashare URL\n --
-datashare-project TEXT Datashare project\n --elasticsearch-url TEXT You can
-additionally pass the Elasticsearch\n URL in order to use scrollingcapabilities
-of\n Elasticsearch (useful when dealing with a\n lot of results)\n\n --query
-TEXT The query string to filter documents\n --destination-directory TEXT
-Directory documents will be downloaded\n --throttle INTEGER Request throttling
-(in ms)\n --cookies TEXT Key/value pair to add a cookie to each\n request to
-the API. You can\n separatesemicolons: key1=val1;key2=val2;...\n\n --path-
-format TEXT Downloaded document path template\n --scroll TEXT Scroll duration\n
---source TEXT A comma-separated list of field to include\n in the downloaded
-document from the index\n\n -f, --from INTEGER Passed to the search it will
-bypass the\n first n documents\n -l, --limit INTEGER Limit the total results to
-return\n --sort-by TEXT Field to use to sort results\n --order-by [asc|desc]
-Order to use to sort results\n --once / --not-once Download file only once\n --
-traceback / --no-traceback Display a traceback in case of error\n --progressbar
-/ --no-progressbar\n Display a progressbar\n --raw-file / --no-raw-file
-Download raw file from Datashare\n --type [Document|NamedEntity] Type of
-indexed documents to download\n --help Show this message and
-exit.\n```\n\n\n### Export by Query\n\nA command to export all files matching a
-query.\n\n```\nUsage: tarentula export-by-query [OPTIONS]\n\nOptions:\n --
-apikey TEXT Datashare authentication apikey\n --datashare-url TEXT Datashare
-URL\n --datashare-project TEXT Datashare project\n --elasticsearch-url TEXT You
-can additionally pass the Elasticsearch\n URL in order to use
-scrollingcapabilities of\n Elasticsearch (useful when dealing with a\n lot of
-results)\n\n --query TEXT The query string to filter documents\n --output-file
-TEXT Path to the CSV file\n --throttle INTEGER Request throttling (in ms)\n --
-cookies TEXT Key/value pair to add a cookie to each\n request to the API. You
-can\n separatesemicolons: key1=val1;key2=val2;...\n\n --scroll TEXT Scroll
-duration\n --source TEXT A comma-separated list of field to include\n in the
-export\n\n --sort-by TEXT Field to use to sort results\n --order-by [asc|desc]
-Order to use to sort results\n --traceback / --no-traceback Display a traceback
-in case of error\n --progressbar / --no-progressbar\n Display a progressbar\n -
--type [Document|NamedEntity] Type of indexed documents to download\n -f, --from
-INTEGER Passed to the search it will bypass the\n first n documents\n -l, --
-limit INTEGER Limit the total results to return\n --size INTEGER Size of the
-scroll request that powers the\n operation.\n\n --query-field / --no-query-
-field\n Add the query to the export CSV\n --help Show this message and
-exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents with a CSV
-file.\n\n```\nUsage: tarentula tagging [OPTIONS] CSV_PATH\n\nOptions:\n --
-datashare-url TEXT http://localhost:8080 Datashare URL\n --datashare-project
-TEXT local-datashare Datashare project\n --throttle INTEGER 0 Request
-throttling (in ms)\n --cookies TEXT _Empty string_ Key/value pair to add a
-cookie to each request to the API. You can separate semicolons:
-key1=val1;key2=val2;...\n --apikey TEXT None Datashare authentication apikey\n
---traceback / --no-traceback Display a traceback in case of error\n --
-progressbar / --no-progressbar Display a progressbar\n --help Show this message
-and exit\n```\n\n#### CSV formats\n\nTagging with a `documentId` and `routing`:
-\n\n```csv\ntag,documentId,routing\nActinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG\nAntrodiaetidae,DWLOskax28jPQ2CjFrCo\nAtracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN\nAtypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\nBarychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\n```\n\nTagging
-with a `documentUrl`:\n\n```csv\ntag,documentUrl\nMecicobothriidae,http://
-localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/
-DbhveTJEwQfJL5Gn3Zgi\nMicrostigmatidae,http://localhost:8080/#/d/local-
-datashare/iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0\nMigidae,http://localhost:
-8080/#/d/local-datashare/BmovvXBisWtyyx6o9cuG/
-BmovvXBisWtyyx6o9cuG\nNemesiidae,http://localhost:8080/#/d/local-datashare/
-vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN\nParatropididae,http://localhost:
-8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/
-vYl1C4bsWphUKvXEBDhM\nPorrhothelidae,http://localhost:8080/#/d/local-datashare/
-fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp\nTheraphosidae,http://localhost:8080/
-#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu\n```\n\n###
-Tagging by Query\n\nA command that uses Elasticsearch `update-by-query` feature
-to batch tag documents directly in the index.\n\nTo see an example of input
-file, refer to [this JSON](tests/fixtures/tags-by-content-
-type.json).\n\n```\nUsage: tarentula tagging-by-query [OPTIONS]
-JSON_PATH\n\nOptions:\n --datashare-project TEXT Datashare project\n --
-elasticsearch-url TEXT Elasticsearch URL which is used to perform\n update by
-query\n --throttle INTEGER Request throttling (in ms)\n --cookies TEXT Key/
-value pair to add a cookie to each\n request to the API. You can\n
-separatesemicolons: key1=val1;key2=val2;...\n --apikey TEXT Datashare
-authentication apikey\n --traceback / --no-traceback Display a traceback in
-case of error\n --progressbar / --no-progressbar Display a progressbar\n --
-wait-for-completion / --no-wait-for-completion\n Create a Elasticsearch task to
-perform the\n updateasynchronously\n --help Show this message and
-exit\n```\n\n\n### List Metadata\n\nYou can list the metadata from the mapping,
-optionally counting the number of occurrences of each field in the index, with
-the `--count` parameter. Counting the fields is disabled by default.\n\nIt
-includes a `--filter_by` parameter to narrow retrieving metadata properties of
-specific sets of documents. For instance it can be used to get just emails
-related properties with: `--filter_by "contentType=message/rfc822"`\n\n```\n$
-tarentula list-metadata --help\nUsage: tarentula list-metadata
-[OPTIONS]\n\nOptions:\n --datashare-project TEXT Datashare project\n --
-elasticsearch-url TEXT You can additionally pass the Elasticsearch\n URL in
-order to use scrollingcapabilities of\n Elasticsearch (useful when dealing with
-a lot\n of results)\n --type [Document|NamedEntity] Type of indexed documents
-to get metadata\n --filter_by TEXT Filter documents by pairs concatenated by\n
-coma of field names and values separated by\n =.Example "contentType=message/
-rfc822,content\n Type=message/rfc822"\n --count / --no-count Count or not the
-number of docs for each\n property found\n\n --help Show this message and
-exit.\n\n```\n\n### Aggregate\n\nYou can run aggregations on the data, the
-ElasticSearch aggregations API is partially enabled with this command.\nThe
-possibilities are:\n\n- count: grouping by a given field different values, and
-count the num of docs.\n- nunique: returns the number of unique values of a
-given field.\n- date_histogram: returns counting of monthly or yearly grouped
-values for a given date field.\n- sum: returns the sum of values of number type
-fields.\n- min: returns the min of values of number type fields.\n- max:
-returns the max of values of number type fields.\n- avg: returns the average of
-values of number type fields.\n- stats: returns a bunch of statistics for a
-given number type fields.\n- string_stats: returns a bunch of string statistics
-for a given string type fields.\n\n\n\n```\n$ tarentula aggregate --
-help\nUsage: tarentula aggregate [OPTIONS]\n\nOptions:\n --apikey TEXT
-Datashare authentication apikey\n --datashare-url TEXT Datashare URL\n --
-datashare-project TEXT Datashare project\n --elasticsearch-url TEXT You can
-additionally pass the Elasticsearch\n URL in order to use scrollingcapabilities
-of\n Elasticsearch (useful when dealing with a\n lot of results)\n --query TEXT
-The query string to filter documents\n --cookies TEXT Key/value pair to add a
-cookie to each\n request to the API. You can\n separatesemicolons:
-key1=val1;key2=val2;...\n --traceback / --no-traceback Display a traceback in
-case of error\n --type [Document|NamedEntity] Type of indexed documents to
-download\n --group_by TEXT Field to use to aggregate results\n --
-operation_field TEXT Field to run the operation on\n --run
-[count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]\n Operation
-to run\n --calendar_interval [year|month]\n Calendar interval for date
-histogram\n aggregation\n --help Show this message and exit.\n```\n\n###
-Following your changes\n\nWhen running Elasticsearch changes on big datasets,
-it could take a very long time. As we were curling ES to see if the task was
-still running well, we added a small utility to follow the changes. It makes a
-live graph of a provided ES indicator with a specified filter.\n\nIt uses
-[mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf you see the
-following message :\n\n```\n$ graph_es\ngraph_realtime.py:32: UserWarning:
-Matplotlib is currently using agg, which is a non-GUI backend, so cannot show
-the figure\n```\n\nThen you have to install [tkinter](https://docs.python.org/
-3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.\n\nThe command has
-the options below:\n\n```\n$ graph_es --help\nUsage: graph_es
-[OPTIONS]\n\nOptions:\n --query TEXT Give a JSON query to filter documents. It
-can be\n a file with @path/to/file. Default to all.\n --index TEXT
-Elasticsearch index (default local-datashare)\n --refresh-interval INTEGER
-Graph refresh interval in seconds (default 5s)\n --field TEXT Field value to
-display over time (default "hits.total")\n --elasticsearch-url TEXT
-Elasticsearch URL which is used to perform\n update by query (default http://
-elasticsearch:9200)\n```\n\n## Configuration File\n\nTarentula supports several
-sources for configuring its behavior, including an ini files and command-line
-options.\n\nConfiguration file will be searched for in the following order (use
-the first file found, all others are ignored):\n\n * `TARENTULA_CONFIG`
-(environment variable if set)\n * `tarentula.ini` (in the current directory)\n
-* `~/.tarentula.ini` (in the home directory)\n * `/etc/tarentula/
-tarentula.ini`\n\nIt should follow the following format (all values bellow are
-optional):\n\n```\n[DEFAULT]\napikey = SECRETHALONOPROCTIDAE\ndatashare_url =
-http://here:8080\ndatashare_project = local-datashare\n\n
-[logger]\nsyslog_address = 127.0.0.0\nsyslog_port = 514\nsyslog_facility =
-local7\nstdout_loglevel = INFO\n```\n\n## Testing\n\nTo test this tool, you
-must have Datashare and Elasticsearch running on your development
-machine.\n\nAfter you [installed Datashare](https://datashare.icij.org/), just
-run it with a test project/user:\n\n```\ndatashare -p test-datashare -
-u test\n```\n\nIn a separate terminal, install the development dependencies:
-\n\n```\nmake install\n```\n\nFinally, run the test\n\n```\nmake
-test\n```\n\n\n## Releasing\n\nThe releasing process uses [bumpversion](https:/
-/pypi.org/project/bumpversion/) to manage versions of this package, [pypi]
-(https://pypi.org/project/tarentula/) to publish the Python package and [Docker
-Hub](https://hub.docker.com/) for the Docker image.\n\n### 1. Create a new
-release\n\n```\nmake [patch|minor|major]\n```\n\n### 2. Upload distributions on
-pypi\n\n_To be able to do this, you will need to be a maintainer of the [pypi]
-(https://pypi.org/project/tarentula/) project._\n\n```\nmake
-distribute\n```\n\n### 3. Build and publish the Docker image\n\nTo build and
-upload a new image on the [docker repository](https://hub.docker.com/
-repository/docker/icij/datashare-tarentula) :\n\n_To be able to do this, you
-will need to be part of the ICIJ organization on docker_\n\n```\nmake docker-
-publish\n```\n\n**Note**: Datashare Tarentula is a multi-platform build. You
-might need to setup your environment for \nmulti-platform using the `make
-docker-setup-multiarch` command. Read more \n[on Docker documentation](https://
-docs.docker.com/build/building/multi-platform/). \n\n### 4. Push your changes
-on Github\n\nGit push release and tag :\n\n```\ngit push origin master --
-tags\n```\n', 'author': 'ICIJ', 'author_email': 'engineering@icij.org',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.8,<3.11', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: tarentula Version: 4.4.0 Summary: Author: ICIJ
+Author-email: engineering@icij.org Requires-Python: >=3.8,<4.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: click (>=8.1,<9.0) Requires-Dist: coloredlogs
+(==14.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: requests
+(>=2.28,<3.0) Requires-Dist: rich (>=12,<13) Description-Content-Type: text/
+markdown # Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/
+datashare-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-
+tarentula) Cli toolbelt for [Datashare](https://datashare.icij.org). ``` / \ \
+\ ,, / / '-.`\()/`.-' .--_'( )'_--. / /` /`""`\ `\ \ | | >< | | \ \ / / '.__.'
+Usage: tarentula [OPTIONS] COMMAND [ARGS]... Options: --syslog-address TEXT
+localhost Syslog address --syslog-port INTEGER 514 Syslog port --syslog-
+facility TEXT local7 Syslog facility --stdout-loglevel TEXT ERROR Change the
+default log level for stdout error handler --help Show this message and exit --
+version Show the installed version of Tarentula Commands: aggregate count
+clean-tags-by-query download export-by-query list-metadata tagging tagging-by-
+query ``` --- - [Installation](#installation) - [Usage](#usage) - [Cookbook
+ð©âð³](#cookbook-) - [Count](#count) - [Clean Tags by Query](#clean-tags-
+by-query) - [Download](#download) - [Export by Query](#export-by-query) -
+[Tagging](#tagging) - [CSV formats](#csv-formats) - [Tagging by Query]
+(#tagging-by-query) - [Aggregate](#aggregate) - [Following your changes]
+(#following-your-changes) - [Configuration File](#configuration-file) -
+[Testing](#testing) - [Releasing](#releasing) - [1. Create a new release](#1-
+create-a-new-release) - [2. Upload distributions on pypi](#2-upload-
+distributions-on-pypi) - [3. Build and publish the Docker image](#3-build-and-
+publish-the-docker-image) - [4. Push your changes on Github](#4-push-your-
+changes-on-github) --- ## Installation You can insatll Datashare Tarentula with
+your favorite package manager: ``` pip3 install --user tarentula ``` Or
+alternativly with Docker: ``` docker run icij/datashare-tarentula ``` ## Usage
+Datashare Tarentula comes with basic commands to interact with a Datashare
+instance (running locally or on a remote server). Primarily focus on bulk
+actions, it provides you with both a cli interface and a python API. ###
+Cookbook ð©âð³ To learn more about how to use Datashare Tarentula with a
+list of examples, please refer to _t_h_e_ _C_o_o_k_b_o_o_k. ### Count A command to just
+count the number of files matching a query. ``` Usage: tarentula count
+[OPTIONS] Options: --datashare-url TEXT Datashare URL --datashare-project TEXT
+Datashare project --elasticsearch-url TEXT You can additionally pass the
+Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
+(useful when dealing with a lot of results) --query TEXT The query string to
+filter documents --cookies TEXT Key/value pair to add a cookie to each request
+to the API. You can separatesemicolons: key1=val1;key2=val2;... --apikey TEXT
+Datashare authentication apikey in the downloaded document from the index --
+traceback / --no-traceback Display a traceback in case of error --type
+[Document|NamedEntity] Type of indexed documents to download --help Show this
+message and exit ``` ### Clean Tags by Query A command that uses Elasticsearch
+`update-by-query` feature to batch untag documents directly in the index. ```
+Usage: tarentula clean-tags-by-query [OPTIONS] Options: --datashare-project
+TEXT Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used
+to perform update by query --cookies TEXT Key/value pair to add a cookie to
+each request to the API. You can separatesemicolons: key1=val1;key2=val2;... --
+apikey TEXT Datashare authentication apikey --traceback / --no-traceback
+Display a traceback in case of error --wait-for-completion / --no-wait-for-
+completion Create a Elasticsearch task to perform the updateasynchronously --
+query TEXT Give a JSON query to filter documents that will have their tags
+cleaned. It can be afile with @path/to/file. Default to all. --help Show this
+message and exit ``` ### Download A command to download all files matching a
+query. ``` Usage: tarentula download [OPTIONS] Options: --apikey TEXT Datashare
+authentication apikey --datashare-url TEXT Datashare URL --datashare-project
+TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
+Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
+(useful when dealing with a lot of results) --query TEXT The query string to
+filter documents --destination-directory TEXT Directory documents will be
+downloaded --throttle INTEGER Request throttling (in ms) --cookies TEXT Key/
+value pair to add a cookie to each request to the API. You can
+separatesemicolons: key1=val1;key2=val2;... --path-format TEXT Downloaded
+document path template --scroll TEXT Scroll duration --source TEXT A comma-
+separated list of field to include in the downloaded document from the index -
+f, --from INTEGER Passed to the search it will bypass the first n documents -l,
+--limit INTEGER Limit the total results to return --sort-by TEXT Field to use
+to sort results --order-by [asc|desc] Order to use to sort results --once / --
+not-once Download file only once --traceback / --no-traceback Display a
+traceback in case of error --progressbar / --no-progressbar Display a
+progressbar --raw-file / --no-raw-file Download raw file from Datashare --type
+[Document|NamedEntity] Type of indexed documents to download --help Show this
+message and exit. ``` ### Export by Query A command to export all files
+matching a query. ``` Usage: tarentula export-by-query [OPTIONS] Options: --
+apikey TEXT Datashare authentication apikey --datashare-url TEXT Datashare URL
+--datashare-project TEXT Datashare project --elasticsearch-url TEXT You can
+additionally pass the Elasticsearch URL in order to use scrollingcapabilities
+of Elasticsearch (useful when dealing with a lot of results) --query TEXT The
+query string to filter documents --output-file TEXT Path to the CSV file --
+throttle INTEGER Request throttling (in ms) --cookies TEXT Key/value pair to
+add a cookie to each request to the API. You can separatesemicolons:
+key1=val1;key2=val2;... --scroll TEXT Scroll duration --source TEXT A comma-
+separated list of field to include in the export --sort-by TEXT Field to use to
+sort results --order-by [asc|desc] Order to use to sort results --traceback / -
+-no-traceback Display a traceback in case of error --progressbar / --no-
+progressbar Display a progressbar --type [Document|NamedEntity] Type of indexed
+documents to download -f, --from INTEGER Passed to the search it will bypass
+the first n documents -l, --limit INTEGER Limit the total results to return --
+size INTEGER Size of the scroll request that powers the operation. --query-
+field / --no-query-field Add the query to the export CSV --help Show this
+message and exit. ``` ### Tagging A command to batch tag documents with a CSV
+file. ``` Usage: tarentula tagging [OPTIONS] CSV_PATH Options: --datashare-url
+TEXT http://localhost:8080 Datashare URL --datashare-project TEXT local-
+datashare Datashare project --throttle INTEGER 0 Request throttling (in ms) --
+cookies TEXT _Empty string_ Key/value pair to add a cookie to each request to
+the API. You can separate semicolons: key1=val1;key2=val2;... --apikey TEXT
+None Datashare authentication apikey --traceback / --no-traceback Display a
+traceback in case of error --progressbar / --no-progressbar Display a
+progressbar --help Show this message and exit ``` #### CSV formats Tagging with
+a `documentId` and `routing`: ```csv tag,documentId,routing
+Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
+Antrodiaetidae,DWLOskax28jPQ2CjFrCo
+Atracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN
+Atypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi
+Barychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi ``` Tagging with a
+`documentUrl`: ```csv tag,documentUrl Mecicobothriidae,http://localhost:8080/#/
+d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi
+Microstigmatidae,http://localhost:8080/#/d/local-datashare/
+iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0 Migidae,http://localhost:8080/#/d/
+local-datashare/BmovvXBisWtyyx6o9cuG/BmovvXBisWtyyx6o9cuG Nemesiidae,http://
+localhost:8080/#/d/local-datashare/vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN
+Paratropididae,http://localhost:8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/
+vYl1C4bsWphUKvXEBDhM Porrhothelidae,http://localhost:8080/#/d/local-datashare/
+fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp Theraphosidae,http://localhost:8080/
+#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu ``` ### Tagging
+by Query A command that uses Elasticsearch `update-by-query` feature to batch
+tag documents directly in the index. To see an example of input file, refer to
+[this JSON](tests/fixtures/tags-by-content-type.json). ``` Usage: tarentula
+tagging-by-query [OPTIONS] JSON_PATH Options: --datashare-project TEXT
+Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used to
+perform update by query --throttle INTEGER Request throttling (in ms) --cookies
+TEXT Key/value pair to add a cookie to each request to the API. You can
+separatesemicolons: key1=val1;key2=val2;... --apikey TEXT Datashare
+authentication apikey --traceback / --no-traceback Display a traceback in case
+of error --progressbar / --no-progressbar Display a progressbar --wait-for-
+completion / --no-wait-for-completion Create a Elasticsearch task to perform
+the updateasynchronously --help Show this message and exit ``` ### List
+Metadata You can list the metadata from the mapping, optionally counting the
+number of occurrences of each field in the index, with the `--count` parameter.
+Counting the fields is disabled by default. It includes a `--filter_by`
+parameter to narrow retrieving metadata properties of specific sets of
+documents. For instance it can be used to get just emails related properties
+with: `--filter_by "contentType=message/rfc822"` ``` $ tarentula list-metadata
+--help Usage: tarentula list-metadata [OPTIONS] Options: --datashare-project
+TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
+Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
+(useful when dealing with a lot of results) --type [Document|NamedEntity] Type
+of indexed documents to get metadata --filter_by TEXT Filter documents by pairs
+concatenated by coma of field names and values separated by =.Example
+"contentType=message/rfc822,content Type=message/rfc822" --count / --no-count
+Count or not the number of docs for each property found --help Show this
+message and exit. ``` ### Aggregate You can run aggregations on the data, the
+ElasticSearch aggregations API is partially enabled with this command. The
+possibilities are: - count: grouping by a given field different values, and
+count the num of docs. - nunique: returns the number of unique values of a
+given field. - date_histogram: returns counting of monthly or yearly grouped
+values for a given date field. - sum: returns the sum of values of number type
+fields. - min: returns the min of values of number type fields. - max: returns
+the max of values of number type fields. - avg: returns the average of values
+of number type fields. - stats: returns a bunch of statistics for a given
+number type fields. - string_stats: returns a bunch of string statistics for a
+given string type fields. ``` $ tarentula aggregate --help Usage: tarentula
+aggregate [OPTIONS] Options: --apikey TEXT Datashare authentication apikey --
+datashare-url TEXT Datashare URL --datashare-project TEXT Datashare project --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in order
+to use scrollingcapabilities of Elasticsearch (useful when dealing with a lot
+of results) --query TEXT The query string to filter documents --cookies TEXT
+Key/value pair to add a cookie to each request to the API. You can
+separatesemicolons: key1=val1;key2=val2;... --traceback / --no-traceback
+Display a traceback in case of error --type [Document|NamedEntity] Type of
+indexed documents to download --group_by TEXT Field to use to aggregate results
+--operation_field TEXT Field to run the operation on --run
+[count|nunique|date_histogram|sum|stats|string_stats|min|max|avg] Operation to
+run --calendar_interval [year|month] Calendar interval for date histogram
+aggregation --help Show this message and exit. ``` ### Following your changes
+When running Elasticsearch changes on big datasets, it could take a very long
+time. As we were curling ES to see if the task was still running well, we added
+a small utility to follow the changes. It makes a live graph of a provided ES
+indicator with a specified filter. It uses [mathplotlib](https://
+matplotlib.org/) and python3-tk. If you see the following message : ``` $
+graph_es graph_realtime.py:32: UserWarning: Matplotlib is currently using agg,
+which is a non-GUI backend, so cannot show the figure ``` Then you have to
+install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e.
+python3-tk for Debian/Ubuntu. The command has the options below: ``` $ graph_es
+--help Usage: graph_es [OPTIONS] Options: --query TEXT Give a JSON query to
+filter documents. It can be a file with @path/to/file. Default to all. --index
+TEXT Elasticsearch index (default local-datashare) --refresh-interval INTEGER
+Graph refresh interval in seconds (default 5s) --field TEXT Field value to
+display over time (default "hits.total") --elasticsearch-url TEXT Elasticsearch
+URL which is used to perform update by query (default http://elasticsearch:
+9200) ``` ## Configuration File Tarentula supports several sources for
+configuring its behavior, including an ini files and command-line options.
+Configuration file will be searched for in the following order (use the first
+file found, all others are ignored): * `TARENTULA_CONFIG` (environment variable
+if set) * `tarentula.ini` (in the current directory) * `~/.tarentula.ini` (in
+the home directory) * `/etc/tarentula/tarentula.ini` It should follow the
+following format (all values bellow are optional): ``` [DEFAULT] apikey =
+SECRETHALONOPROCTIDAE datashare_url = http://here:8080 datashare_project =
+local-datashare [logger] syslog_address = 127.0.0.0 syslog_port = 514
+syslog_facility = local7 stdout_loglevel = INFO ``` ## Testing To test this
+tool, you must have Datashare and Elasticsearch running on your development
+machine. After you [installed Datashare](https://datashare.icij.org/), just run
+it with a test project/user: ``` datashare -p test-datashare -u test ``` In a
+separate terminal, install the development dependencies: ``` make install ```
+Finally, run the test ``` make test ``` ## Releasing The releasing process uses
+[bumpversion](https://pypi.org/project/bumpversion/) to manage versions of this
+package, [pypi](https://pypi.org/project/tarentula/) to publish the Python
+package and [Docker Hub](https://hub.docker.com/) for the Docker image. ### 1.
+Create a new release ``` make [patch|minor|major] ``` ### 2. Upload
+distributions on pypi _To be able to do this, you will need to be a maintainer
+of the [pypi](https://pypi.org/project/tarentula/) project._ ``` make
+distribute ``` ### 3. Build and publish the Docker image To build and upload a
+new image on the [docker repository](https://hub.docker.com/repository/docker/
+icij/datashare-tarentula) : _To be able to do this, you will need to be part of
+the ICIJ organization on docker_ ``` make docker-publish ``` **Note**:
+Datashare Tarentula is a multi-platform build. You might need to setup your
+environment for multi-platform using the `make docker-setup-multiarch` command.
+Read more [on Docker documentation](https://docs.docker.com/build/building/
+multi-platform/). ### 4. Push your changes on Github Git push release and tag :
+``` git push origin master --tags ```
```

