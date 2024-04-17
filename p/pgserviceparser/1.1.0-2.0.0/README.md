# Comparing `tmp/pgserviceparser-1.1.0.tar.gz` & `tmp/pgserviceparser-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgserviceparser-1.1.0.tar", last modified: Mon Jun 27 10:25:48 2022, max compression
+gzip compressed data, was "pgserviceparser-2.0.0.tar", last modified: Wed Apr 17 07:44:21 2024, max compression
```

## Comparing `pgserviceparser-1.1.0.tar` & `pgserviceparser-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-27 10:25:48.871175 pgserviceparser-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-06-27 10:25:36.000000 pgserviceparser-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2022-06-27 10:25:48.871175 pgserviceparser-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1313 2022-06-27 10:25:36.000000 pgserviceparser-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-27 10:25:48.871175 pgserviceparser-1.1.0/pgserviceparser/
--rw-r--r--   0 runner    (1001) docker     (116)     1801 2022-06-27 10:25:36.000000 pgserviceparser-1.1.0/pgserviceparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-27 10:25:48.871175 pgserviceparser-1.1.0/pgserviceparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2022-06-27 10:25:48.000000 pgserviceparser-1.1.0/pgserviceparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      210 2022-06-27 10:25:48.000000 pgserviceparser-1.1.0/pgserviceparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-27 10:25:48.000000 pgserviceparser-1.1.0/pgserviceparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-06-27 10:25:48.000000 pgserviceparser-1.1.0/pgserviceparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-27 10:25:48.871175 pgserviceparser-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      807 2022-06-27 10:25:36.000000 pgserviceparser-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/docs_builder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/pgserviceparser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/pgserviceparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/pgserviceparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 07:44:21.000000 pgserviceparser-2.0.0/pgserviceparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:44:21.544521 pgserviceparser-2.0.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/data/service_base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 07:44:09.000000 pgserviceparser-2.0.0/test/test_lib.py
```

### Comparing `pgserviceparser-1.1.0/PKG-INFO` & `pgserviceparser-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 Metadata-Version: 2.1
 Name: pgserviceparser
-Version: 1.1.0
-Summary: A package parsing the PostgreSQL connection service file. 
-Home-page: https://github.com/opengisch/pgserviceparser
-Author: Dave Signer
-Author-email: david@opengis.ch
+Version: 2.0.0
+Summary: A package parsing the PostgreSQL connection service file
+Author-email: David Signer <info@opengis.ch>, Julien Moura <julien.moura@oslandia.com>, Germán Carrillo <info@opengis.ch>, Denis Rouzaud <info@opengis.ch>
+License: MIT License
+Project-URL: homepage, https://opengisch.github.io/pgserviceparser/
+Project-URL: repository, https://github.com/opengisch/pgserviceparser
+Project-URL: tracker, https://github.com/opengisch/pgserviceparser/issues
+Keywords: postgres,service
 Classifier: Topic :: Database
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pgserviceparser
+
 A python package parsing the PostgreSQL connection service file.
 
-```
+```python
 >>> import pgserviceparser
 ```
 
 ## Finding the PostgreSQL connection service file with `conf_path`
 
 Returns the path found for the pg_service.conf on the system as string.
-```
+
+```python
 >>> pgserviceparser.conf_path()
 '/home/dave/.pg_service.conf'
 ```
+
 ## Listing all the services with `service_names`
 
 Returns all service names in a list.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_names()
 ['srvce_wandplaene', 'ktn_solothurn', 'daves_bakery']
+
 ```
+
 ## Receiving the configuration for a service with `service_config`
 
 Returns the config from the given service name as a dict.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_config('daves_bakery')
 {'host': 'localhost', 'port': '5432', 'dbname': 'bakery', 'user': 'dave', 'password': 'fischersfritz'}
 ```
 
 ## Getting the full configuration with `full_config`
 
 Returns full pgservice config as [configparser.ConfigParser()](https://docs.python.org/3/library/configparser.html).
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.full_config()
 <configparser.ConfigParser object at 0x7f4c6d66b580>
 ```
+
+----
+
+## Contribute
+
+### Git hooks
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pgserviceparser-1.1.0/README.md` & `pgserviceparser-2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 # pgserviceparser
+
 A python package parsing the PostgreSQL connection service file.
 
-```
+```python
 >>> import pgserviceparser
 ```
 
 ## Finding the PostgreSQL connection service file with `conf_path`
 
 Returns the path found for the pg_service.conf on the system as string.
-```
+
+```python
 >>> pgserviceparser.conf_path()
 '/home/dave/.pg_service.conf'
 ```
+
 ## Listing all the services with `service_names`
 
 Returns all service names in a list.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_names()
 ['srvce_wandplaene', 'ktn_solothurn', 'daves_bakery']
+
 ```
+
 ## Receiving the configuration for a service with `service_config`
 
 Returns the config from the given service name as a dict.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_config('daves_bakery')
 {'host': 'localhost', 'port': '5432', 'dbname': 'bakery', 'user': 'dave', 'password': 'fischersfritz'}
 ```
 
 ## Getting the full configuration with `full_config`
 
 Returns full pgservice config as [configparser.ConfigParser()](https://docs.python.org/3/library/configparser.html).
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.full_config()
 <configparser.ConfigParser object at 0x7f4c6d66b580>
 ```
+
+----
+
+## Contribute
+
+### Git hooks
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `pgserviceparser-1.1.0/pgserviceparser.egg-info/PKG-INFO` & `pgserviceparser-2.0.0/pgserviceparser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 Metadata-Version: 2.1
 Name: pgserviceparser
-Version: 1.1.0
-Summary: A package parsing the PostgreSQL connection service file. 
-Home-page: https://github.com/opengisch/pgserviceparser
-Author: Dave Signer
-Author-email: david@opengis.ch
+Version: 2.0.0
+Summary: A package parsing the PostgreSQL connection service file
+Author-email: David Signer <info@opengis.ch>, Julien Moura <julien.moura@oslandia.com>, Germán Carrillo <info@opengis.ch>, Denis Rouzaud <info@opengis.ch>
+License: MIT License
+Project-URL: homepage, https://opengisch.github.io/pgserviceparser/
+Project-URL: repository, https://github.com/opengisch/pgserviceparser
+Project-URL: tracker, https://github.com/opengisch/pgserviceparser/issues
+Keywords: postgres,service
 Classifier: Topic :: Database
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pgserviceparser
+
 A python package parsing the PostgreSQL connection service file.
 
-```
+```python
 >>> import pgserviceparser
 ```
 
 ## Finding the PostgreSQL connection service file with `conf_path`
 
 Returns the path found for the pg_service.conf on the system as string.
-```
+
+```python
 >>> pgserviceparser.conf_path()
 '/home/dave/.pg_service.conf'
 ```
+
 ## Listing all the services with `service_names`
 
 Returns all service names in a list.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_names()
 ['srvce_wandplaene', 'ktn_solothurn', 'daves_bakery']
+
 ```
+
 ## Receiving the configuration for a service with `service_config`
 
 Returns the config from the given service name as a dict.
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.service_config('daves_bakery')
 {'host': 'localhost', 'port': '5432', 'dbname': 'bakery', 'user': 'dave', 'password': 'fischersfritz'}
 ```
 
 ## Getting the full configuration with `full_config`
 
 Returns full pgservice config as [configparser.ConfigParser()](https://docs.python.org/3/library/configparser.html).
 Optionally you can pass a config file path. Otherwise it gets it by `conf_path`.
-```
+
+```python
 >>> pgserviceparser.full_config()
 <configparser.ConfigParser object at 0x7f4c6d66b580>
 ```
+
+----
+
+## Contribute
+
+### Git hooks
+
+```sh
+pip install pre-commit
+pre-commit install
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

