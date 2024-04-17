# Comparing `tmp/etos_client-6.2.0.tar.gz` & `tmp/etos_client-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_client-6.2.0.tar", last modified: Mon Dec  4 11:04:26 2023, max compression
+gzip compressed data, was "etos_client-6.3.0.tar", last modified: Wed Apr 17 07:46:52 2024, max compression
```

## Comparing `etos_client-6.2.0.tar` & `etos_client-6.3.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.136911 etos_client-6.2.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      594 2023-03-09 08:23:53.000000 etos_client-6.2.0/.coveragerc
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1579 2023-12-04 11:04:26.136911 etos_client-6.2.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      986 2023-03-09 08:23:53.000000 etos_client-6.2.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7616 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9178 2023-11-28 14:03:13.000000 etos_client-6.2.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      452 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:53.000000 etos_client-6.2.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      217 2023-11-28 14:03:13.000000 etos_client-6.2.0/pylintrc
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      670 2023-11-28 14:03:13.000000 etos_client-6.2.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1469 2023-12-04 11:04:26.136911 etos_client-6.2.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      555 2023-03-09 08:23:53.000000 etos_client-6.2.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1087 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1144 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/__main__.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/announcer/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      718 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/announcer/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3471 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/announcer/announcer.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/downloader/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      737 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/downloader/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7755 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/downloader/downloader.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/etos/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      710 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/etos/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4654 2023-12-01 11:39:11.000000 etos_client-6.2.0/src/etos_client/etos/etos.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3488 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/etos/schema.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/event_repository/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      726 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/event_repository/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7548 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/event_repository/graphql.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3542 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/event_repository/graphql_queries.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/events/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      694 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/events/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     8529 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/events/collector.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1784 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/events/events.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/sse/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      684 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/sse/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7168 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/sse/client.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3278 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/sse/protocol.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7385 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/start.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1337 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/test.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/test_results/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      731 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/test_results/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3594 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/test_results/test_results.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client/test_run/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      719 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/test_run/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     6078 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etos_client/test_run/test_run.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etos_client.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1579 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1690 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       88 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/entry_points.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-05 07:49:40.000000 etos_client-6.2.0/src/etos_client.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       57 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       20 2023-12-04 11:04:26.000000 etos_client-6.2.0/src/etos_client.egg-info/top_level.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etosctl/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      683 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3039 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/__main__.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etosctl/command/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      762 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/command/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4789 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/command/command.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.132911 etos_client-6.2.0/src/etosctl/engine/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      736 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/engine/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1621 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/engine/engine.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.136911 etos_client-6.2.0/src/etosctl/models/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      726 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/models/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1029 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/models/models.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.136911 etos_client-6.2.0/src/etosctl/options/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      733 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/options/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      795 2023-11-28 14:03:13.000000 etos_client-6.2.0/src/etosctl/options/options.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-12-04 11:04:26.136911 etos_client-6.2.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      686 2023-11-28 14:03:13.000000 etos_client-6.2.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      199 2023-03-09 08:23:53.000000 etos_client-6.2.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      293 2023-11-28 14:03:13.000000 etos_client-6.2.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      594 2023-03-09 08:23:53.000000 etos_client-6.3.0/.coveragerc
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1754 2024-04-17 07:46:52.619409 etos_client-6.3.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      986 2023-03-09 08:23:53.000000 etos_client-6.3.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.611409 etos_client-6.3.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7616 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.615409 etos_client-6.3.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9178 2023-11-28 14:03:13.000000 etos_client-6.3.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      452 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:53.000000 etos_client-6.3.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      217 2023-11-28 14:03:13.000000 etos_client-6.3.0/pylintrc
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      684 2024-03-04 07:06:26.000000 etos_client-6.3.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1484 2024-04-17 07:46:52.623409 etos_client-6.3.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      555 2023-03-09 08:23:53.000000 etos_client-6.3.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.607409 etos_client-6.3.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.615409 etos_client-6.3.0/src/etos_client/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1087 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1144 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/__main__.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.615409 etos_client-6.3.0/src/etos_client/announcer/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      718 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/announcer/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3471 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/announcer/announcer.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.615409 etos_client-6.3.0/src/etos_client/downloader/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      737 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/downloader/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7672 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/downloader/downloader.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.615409 etos_client-6.3.0/src/etos_client/etos/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      710 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/etos/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4373 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/etos/etos.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3488 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/etos/schema.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client/event_repository/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      726 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/event_repository/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7548 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/event_repository/graphql.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3542 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/event_repository/graphql_queries.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client/events/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      694 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/events/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     8529 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/events/collector.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1861 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/events/events.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client/sse/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      684 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/sse/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7168 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/sse/client.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3278 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/sse/protocol.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7386 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/start.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1337 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/test.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client/test_results/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      731 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/test_results/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3594 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/test_results/test_results.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client/test_run/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      719 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/test_run/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6078 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etos_client/test_run/test_run.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etos_client.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1754 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1690 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       88 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/entry_points.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2024-03-07 06:35:48.000000 etos_client-6.3.0/src/etos_client.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       71 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       20 2024-04-17 07:46:52.000000 etos_client-6.3.0/src/etos_client.egg-info/top_level.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etosctl/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      683 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3094 2024-03-07 06:35:07.000000 etos_client-6.3.0/src/etosctl/__main__.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etosctl/command/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      762 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/command/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4789 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/command/command.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etosctl/engine/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      736 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/engine/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1621 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/engine/engine.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etosctl/models/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      726 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/models/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1029 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/models/models.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/src/etosctl/options/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      733 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/options/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      795 2024-03-07 06:34:35.000000 etos_client-6.3.0/src/etosctl/options/options.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2024-04-17 07:46:52.619409 etos_client-6.3.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      686 2023-11-28 14:03:13.000000 etos_client-6.3.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      199 2023-03-09 08:23:53.000000 etos_client-6.3.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      293 2023-11-28 14:03:13.000000 etos_client-6.3.0/tox.ini
```

### Comparing `etos_client-6.2.0/.coveragerc` & `etos_client-6.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/PKG-INFO` & `etos_client-6.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: etos_client
-Version: 6.2.0
+Version: 6.3.0
 Summary: Test suite execution client for ETOS.
 Home-page: https://github.com/eiffel-community/etos-suite-starter
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.4
 Description-Content-Type: text/x-rst; charset=UTF-8
+Requires-Dist: etos_lib==4.0.0
+Requires-Dist: docopt~=0.6
+Requires-Dist: pydantic~=2.6
 Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 ===========
 ETOS Client
 ===========
 
 .. image:: https://img.shields.io/badge/Stage-Sandbox-yellow.svg
   :target: https://github.com/eiffel-community/community/blob/master/PROJECT_LIFECYCLE.md#stage-sandbox
```

### Comparing `etos_client-6.2.0/README.rst` & `etos_client-6.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/docs/Makefile` & `etos_client-6.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/docs/conf.py` & `etos_client-6.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/requirements.txt` & `etos_client-6.3.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 # Add your pinned requirements so that they can be easily installed with:
 # pip install -r requirements.txt
 # Remember to also add them in setup.cfg but unpinned.
 # Example:
 # numpy==1.13.3
 # scipy==1.0
 #
-etos_lib==2.1.0
+etos_lib==4.0.0
 docopt~=0.6
+pydantic~=2.6
```

### Comparing `etos_client-6.2.0/setup.cfg` & `etos_client-6.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	etos_lib==2.1.0
+	etos_lib==4.0.0
 	docopt~=0.6
+	pydantic~=2.6
 python_requires = >=3.4
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `etos_client-6.2.0/setup.py` & `etos_client-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/__init__.py` & `etos_client-6.3.0/src/etos_client/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/__main__.py` & `etos_client-6.3.0/src/etos_client/__main__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/announcer/__init__.py` & `etos_client-6.3.0/src/etos_client/announcer/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/announcer/announcer.py` & `etos_client-6.3.0/src/etos_client/announcer/announcer.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/downloader/__init__.py` & `etos_client-6.3.0/src/etos_client/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/downloader/downloader.py` & `etos_client-6.3.0/src/etos_client/downloader/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,34 @@
 from threading import Thread, Lock
 from multiprocessing.pool import ThreadPool
 from queue import Queue, Empty
 from json import JSONDecodeError
 
 from pydantic import BaseModel
 from urllib3.exceptions import MaxRetryError, NewConnectionError
+from urllib3.util import Retry
 import requests
 from requests.exceptions import HTTPError
 
+from etos_lib.lib.http import Http
 from etos_client.events.events import Artifact, TestSuite, SubSuite
 
 
+HTTP_RETRY_PARAMETERS = Retry(
+    total=None,
+    read=0,
+    connect=10,  # With 1 as backoff_factor, will retry for 1023s
+    status=10,  # With 1 as backoff_factor, will retry for 1023s
+    backoff_factor=1,
+    other=0,
+    # 413, 429, 503 + 404 (for cases when the file is not uploaded immediately)
+    status_forcelist=list(Retry.RETRY_AFTER_STATUS_CODES) + [404],
+)
+
+
 class Downloadable(BaseModel):
     """Represent a downloadable file."""
 
     uri: str
     name: Optional[Path]
 
 
@@ -49,37 +63,29 @@
         """Init."""
         super().__init__()
         self.__download_queue = Queue()
         self.__queued = []
         self.__exit = False
         self.__clear_queue = True
         self.__lock = Lock()
+        self.__http = Http(retry=HTTP_RETRY_PARAMETERS)
         self.failed: bool = False
         self.downloads: {str} = set()
 
         self.__report_dir = report_dir
         self.__artifact_dir = artifact_dir
 
-    def __retry_download(self, item: Downloadable) -> None:
+    def __download(self, item: Downloadable) -> None:
         """Download files."""
         self.logger.debug("Downloading %r", item)
-        end_time = time.time() + 60
-        while time.time() < end_time:
-            response = requests.get(item.uri, stream=True, timeout=10)
-            self.logger.debug("Download response: %r", response)
-            if self.__should_retry(response):
-                self.logger.debug("Download of %r failed. Retrying..", item)
-                time.sleep(10)
-                continue
-            if not response.ok:
-                with self.__lock:
-                    self.failed = True
-                self.logger.critical("Failed to download %r", item)
-                return
+        # retry rules are set in the Http client
+        response = self.__http.get(item.uri, stream=True)
+        if self.__download_ok(response):
             self.__save_file(item, response)
+            self.logger.debug("Item downloaded %r", item)
             return
         with self.__lock:
             self.failed = True
         self.logger.critical("Failed to download %r", item)
         return
 
     def __save_file(self, item: Downloadable, response: requests.Response) -> None:
@@ -92,50 +98,47 @@
         self.logger.debug("Saving file %s", download_name)
         with self.__lock:
             self.downloads.add(download_name)
         with open(download_name, "wb+") as report:
             for chunk in response:
                 report.write(chunk)
 
-    def __should_retry(self, response: requests.Response) -> bool:
-        """Check response to see whether it is worth retrying or not."""
+    def __download_ok(self, response: requests.Response) -> bool:
+        """Check download response and log response details."""
         try:
             response.raise_for_status()
+            return True
         except HTTPError as http_error:
             if http_error.response.status_code == 404:
-                self.logger.warning("File not found")
-                # Retry as it may just be that the file is being uploaded.
-                return True
-            if 400 <= http_error.response.status_code < 500:
-                try:
-                    response_json = response.json()
-                except JSONDecodeError:
-                    self.logger.debug("Raw response from download: %r", response.text)
-                    response_json = {
-                        "detail": "Unknown client error when downloading files from log area"
-                    }
-                self.logger.critical("Download response: %r", response_json)
+                self.logger.critical("File not found")
                 return False
-            return True
+            try:
+                response_json = response.json()
+            except JSONDecodeError:
+                self.logger.debug("Raw HTTP response from download: %r", response.text)
+                response_json = {
+                    "detail": "Unknown HTTP client error when downloading files from log area"
+                }
+            self.logger.critical("Download response: %r", response_json)
+            return False
         except (
             ConnectionError,
             NewConnectionError,
             MaxRetryError,
             TimeoutError,
         ):
             self.logger.exception("Network connectivity error when downloading logs and artifacts.")
-            return True
-        return False
+            return False
 
     def __trigger_download(self, pool: ThreadPool) -> bool:
         """Get downloadable from queue and add it to threadpool."""
         try:
             item = self.__download_queue.get_nowait()
             pool.apply_async(
-                self.__retry_download,
+                self.__download,
                 error_callback=self.__print_traceback,
                 args=(item,),
             )
             return True
         except Empty:
             return False
```

### Comparing `etos_client-6.2.0/src/etos_client/etos/__init__.py` & `etos_client-6.3.0/src/etos_client/etos/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/etos/etos.py` & `etos_client-6.3.0/src/etos_client/etos/etos.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,35 +11,52 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS API handler."""
 import logging
-import time
 from json import JSONDecodeError
 from typing import Union
 
 import requests
 from requests.exceptions import HTTPError, Timeout
 from urllib3.exceptions import MaxRetryError, NewConnectionError
+from urllib3.util import Retry
 
+from etos_lib.lib.http import Http
 from .schema import RequestSchema, ResponseSchema
 
 
+# Max total time for a ping request including delays with backoff factor 0.5 will be:
+# 0.5 + 1.5 + 3.5 + 7.5 + 15.5 = 28.5 (seconds)
+HTTP_RETRY_PARAMETERS = Retry(
+    total=5,  # limit the total number of retries only (regardless of error type)
+    connect=None,
+    read=None,
+    status_forcelist=[500, 502, 503, 504],  # Common temporary error status codes
+    backoff_factor=0.5,
+    raise_on_redirect=True,  # Raise an exception if too many redirects
+)
+
+
 class ETOS:  # pylint:disable=too-few-public-methods
     """Handle communication with ETOS."""
 
     logger = logging.getLogger(__name__)
     reason = ""
     response: ResponseSchema = None
 
     def __init__(self, cluster: str) -> None:
         """Initialize ETOS."""
         self.cluster = cluster
+        # ping HTTP client with 5 sec timeout for each attempt:
+        self.__http_ping = Http(retry=HTTP_RETRY_PARAMETERS, timeout=5)
+        # greater HTTP timeout for other requests:
+        self.__http = Http(retry=HTTP_RETRY_PARAMETERS, timeout=10)
 
     def start(self, request_data: RequestSchema) -> Union[ResponseSchema, None]:
         """Start ETOS."""
         self.logger.info("Check connection to ETOS.")
         if not self.__check_connection():
             self.reason = "Unable to connect to ETOS. Please check your connection."
             return None
@@ -49,79 +66,43 @@
         if not self.response:
             self.reason = "Failed to start ETOS"
             return None
         return self.response
 
     def __check_connection(self) -> bool:
         """Check connection to ETOS."""
-        end_time = time.time() + 30
-        while time.time() < end_time:
-            try:
-                response = requests.get(f"{self.cluster}/api/selftest/ping", timeout=5)
-            except (
-                ConnectionError,
-                NewConnectionError,
-                MaxRetryError,
-                TimeoutError,
-                Timeout,
-            ):
-                self.logger.exception(
-                    "Network connectivity errors when checking connection to ETOS."
-                )
-                time.sleep(2)
-                continue
-            if self.__should_retry(response):
-                time.sleep(2)
-                continue
-            return True
-        return False
+        # retry rules are set in the Http client
+        response = self.__http_ping.get(f"{self.cluster}/api/selftest/ping")
+        return self.__response_ok(response)
 
     def __start(self, request_data: RequestSchema) -> Union[ResponseSchema, None]:
         """Start an ETOS testrun."""
         response = self.__retry_trigger_etos(request_data)
         if not response:
             return None
-
         return response
 
     def __retry_trigger_etos(self, request_data: RequestSchema) -> Union[ResponseSchema, None]:
         """Trigger ETOS, retrying on non-client errors until successful."""
-        end_time = time.time() + 30
-        while time.time() < end_time:
-            try:
-                response = requests.post(
-                    f"{self.cluster}/api/etos", json=request_data.dict(), timeout=10
-                )
-            except (
-                ConnectionError,
-                NewConnectionError,
-                MaxRetryError,
-                TimeoutError,
-                Timeout,
-            ):
-                self.logger.exception("Network connectivity errors when triggering ETOS.")
-                time.sleep(2)
-                continue
-            if self.__should_retry(response):
-                time.sleep(2)
-                continue
-            if not response.ok:
-                return None
+        # retry rules are set in the Http client
+        response = self.__http.post(f"{self.cluster}/api/etos", json=request_data.dict())
+        if self.__response_ok(response):
             return ResponseSchema.from_response(response.json())
         self.logger.critical("Failed to trigger ETOS.")
         return None
 
-    def __should_retry(self, response: requests.Response) -> bool:
-        """Check response to see whether it is worth retrying or not."""
+    def __response_ok(self, response: requests.Response) -> bool:
+        """Check response and log the relevant information."""
         try:
             response.raise_for_status()
+            return True
         except HTTPError as http_error:
             if 400 <= http_error.response.status_code < 500:
                 try:
                     response_json = response.json()
                 except JSONDecodeError:
                     self.logger.info("Raw response from ETOS: %r", response.text)
                     response_json = {"detail": "Unknown client error from ETOS"}
                 self.logger.critical(response_json.get("detail"))
-                return False
-            return True
+            else:
+                self.logger.critical("Network connectivity error")
         return False
```

### Comparing `etos_client-6.2.0/src/etos_client/etos/schema.py` & `etos_client-6.3.0/src/etos_client/etos/schema.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/event_repository/__init__.py` & `etos_client-6.3.0/src/etos_client/event_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/event_repository/graphql.py` & `etos_client-6.3.0/src/etos_client/event_repository/graphql.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/event_repository/graphql_queries.py` & `etos_client-6.3.0/src/etos_client/event_repository/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/events/__init__.py` & `etos_client-6.3.0/src/etos_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/events/collector.py` & `etos_client-6.3.0/src/etos_client/events/collector.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/events/events.py` & `etos_client-6.3.0/src/etos_client/events/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,58 +17,58 @@
 from typing import Optional
 from pydantic import BaseModel
 
 
 class Activity(BaseModel):
     """ETOS activity events."""
 
-    triggered: Optional[dict]
-    canceled: Optional[dict]
-    finished: Optional[dict]
+    triggered: Optional[dict] = None
+    canceled: Optional[dict] = None
+    finished: Optional[dict] = None
 
 
 class Environment(BaseModel):
     """ETOS environment events."""
 
     name: str
-    uri: Optional[str]
+    uri: Optional[str] = None
 
 
 class Artifact(BaseModel):
     """ETOS artifact."""
 
     files: list[str]
     suite_name: str
     location: str
 
 
 class SubSuite(BaseModel):
     """ETOS sub suite events."""
 
-    started: Optional[dict]
-    finished: Optional[dict]
+    started: Optional[dict] = None
+    finished: Optional[dict] = None
 
 
 class TestSuite(BaseModel):
     """ETOS main suite events."""
 
-    started: Optional[dict]
-    finished: Optional[dict]
+    started: Optional[dict] = None
+    finished: Optional[dict] = None
     sub_suites: list[SubSuite] = []
 
 
 class TestCase(BaseModel):
     """ETOS test case events."""
 
-    finished: Optional[dict]
-    canceled: Optional[dict]
+    finished: Optional[dict] = None
+    canceled: Optional[dict] = None
 
 
 class Events(BaseModel):
     """ETOS events."""
 
     activity: Activity = Activity()
-    tercc: Optional[dict]
+    tercc: Optional[dict] = None
     main_suites: list[TestSuite] = []
     environments: list[Environment] = []
     artifacts: list[Artifact] = []
     test_cases: list[TestCase] = []
```

### Comparing `etos_client-6.2.0/src/etos_client/sse/__init__.py` & `etos_client-6.3.0/src/etos_client/sse/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/sse/client.py` & `etos_client-6.3.0/src/etos_client/sse/client.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/sse/protocol.py` & `etos_client-6.3.0/src/etos_client/sse/protocol.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/start.py` & `etos_client-6.3.0/src/etos_client/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         log_downloader.stop(clear_queue)
         log_downloader.join()
 
     LOGGER.info("Downloaded a total of %d logs from test runners", len(log_downloader.downloads))
     LOGGER.info("Archiving reports.")
     shutil.make_archive(artifact_dir.joinpath("reports").relative_to(Path.cwd()), "zip", report_dir)
     LOGGER.info("Reports: %s", report_dir)
-    LOGGER.info("Artifacs: %s", artifact_dir)
+    LOGGER.info("Artifacts: %s", artifact_dir)
 
     if log_downloader.failed:
         sys.exit("ETOS logs did not download successfully.")
     return TestResults().get_results(events)
 
 
 class Start(SubCommand):
```

### Comparing `etos_client-6.2.0/src/etos_client/test.py` & `etos_client-6.3.0/src/etos_client/test.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/test_results/__init__.py` & `etos_client-6.3.0/src/etos_client/test_results/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/test_results/test_results.py` & `etos_client-6.3.0/src/etos_client/test_results/test_results.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/test_run/__init__.py` & `etos_client-6.3.0/src/etos_client/test_run/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client/test_run/test_run.py` & `etos_client-6.3.0/src/etos_client/test_run/test_run.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etos_client.egg-info/PKG-INFO` & `etos_client-6.3.0/src/etos_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: etos-client
-Version: 6.2.0
+Name: etos_client
+Version: 6.3.0
 Summary: Test suite execution client for ETOS.
 Home-page: https://github.com/eiffel-community/etos-suite-starter
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.4
 Description-Content-Type: text/x-rst; charset=UTF-8
+Requires-Dist: etos_lib==4.0.0
+Requires-Dist: docopt~=0.6
+Requires-Dist: pydantic~=2.6
 Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 ===========
 ETOS Client
 ===========
 
 .. image:: https://img.shields.io/badge/Stage-Sandbox-yellow.svg
   :target: https://github.com/eiffel-community/community/blob/master/PROJECT_LIFECYCLE.md#stage-sandbox
```

### Comparing `etos_client-6.2.0/src/etos_client.egg-info/SOURCES.txt` & `etos_client-6.3.0/src/etos_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/__init__.py` & `etos_client-6.3.0/src/etosctl/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/__main__.py` & `etos_client-6.3.0/src/etosctl/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     elif verbosity == 2:
         loglevel = logging.DEBUG
 
     logformat = "[%(asctime)s] %(levelname)s:%(message)s"
     logging.basicConfig(
         level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
     )
+    logging.getLogger("gql").setLevel(logging.WARNING)
 
 
 class Main(Command):
     """
     etosctl.
 
     Usage: etosctl [-v|-vv] [options] <command> [<args>...]
```

### Comparing `etos_client-6.2.0/src/etosctl/command/__init__.py` & `etos_client-6.3.0/src/etosctl/command/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/command/command.py` & `etos_client-6.3.0/src/etosctl/command/command.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/engine/__init__.py` & `etos_client-6.3.0/src/etosctl/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/engine/engine.py` & `etos_client-6.3.0/src/etosctl/engine/engine.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/models/__init__.py` & `etos_client-6.3.0/src/etosctl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/models/models.py` & `etos_client-6.3.0/src/etosctl/models/models.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/options/__init__.py` & `etos_client-6.3.0/src/etosctl/options/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/src/etosctl/options/options.py` & `etos_client-6.3.0/src/etosctl/options/options.py`

 * *Files identical despite different names*

### Comparing `etos_client-6.2.0/tests/__init__.py` & `etos_client-6.3.0/tests/__init__.py`

 * *Files identical despite different names*

