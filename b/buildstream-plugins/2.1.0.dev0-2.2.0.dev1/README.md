# Comparing `tmp/buildstream-plugins-2.1.0.dev0.tar.gz` & `tmp/buildstream-plugins-2.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildstream-plugins-2.1.0.dev0.tar", last modified: Mon Sep 18 05:00:51 2023, max compression
+gzip compressed data, was "buildstream-plugins-2.2.0.dev1.tar", last modified: Wed Apr 17 10:05:12 2024, max compression
```

## Comparing `buildstream-plugins-2.1.0.dev0.tar` & `buildstream-plugins-2.2.0.dev1.tar`

### file list

```diff
@@ -1,50 +1,81 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/
--rw-r--r--   0 tristan   (1000) tristan   (1000)      797 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/.asf.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1350 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/COMMITTERS.rst
--rw-r--r--   0 tristan   (1000) tristan   (1000)    11358 2022-04-08 08:04:24.000000 buildstream-plugins-2.1.0.dev0/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)      152 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/MANIFEST.in
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2183 2023-09-18 04:59:37.000000 buildstream-plugins-2.1.0.dev0/NEWS
--rw-r--r--   0 tristan   (1000) tristan   (1000)      167 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/NOTICE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1675 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      443 2023-02-17 05:15:44.000000 buildstream-plugins-2.1.0.dev0/README.rst
--rw-r--r--   0 tristan   (1000) tristan   (1000)      985 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/project.conf
--rw-r--r--   0 tristan   (1000) tristan   (1000)      989 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/pyproject.toml
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/requirements/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       79 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/requirements/mypy-requirements.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      177 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/requirements/plugin-requirements.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      163 2023-09-18 04:01:58.000000 buildstream-plugins-2.1.0.dev0/requirements/test-requirements.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      561 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/setup.cfg
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)     4076 2023-02-17 05:55:22.000000 buildstream-plugins-2.1.0.dev0/setup.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.768898 buildstream-plugins-2.1.0.dev0/src/
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/
--rw-r--r--   0 tristan   (1000) tristan   (1000)      654 2023-09-18 04:57:27.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/__init__.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/
--rw-r--r--   0 tristan   (1000) tristan   (1000)        0 2022-04-08 08:04:24.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2297 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/autotools.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3675 2022-12-05 03:18:33.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/autotools.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2259 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/cmake.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1927 2022-12-05 04:20:07.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/cmake.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1775 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/make.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1438 2022-12-05 03:18:20.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/make.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2114 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/meson.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2098 2022-12-05 04:20:07.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/meson.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1566 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/pip.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1255 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/pip.yaml
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1675 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/setuptools.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1363 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/setuptools.yaml
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/
--rw-r--r--   0 tristan   (1000) tristan   (1000)        0 2022-04-08 08:04:24.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     8486 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/bzr.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)    16083 2023-09-18 04:01:58.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/cargo.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)    22173 2023-02-17 07:27:25.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/docker.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)    39482 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/git.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3510 2022-11-27 05:16:55.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/patch.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     9290 2023-02-17 05:55:22.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/pip.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-09-18 05:00:51.772898 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1675 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1445 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      612 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/not-zip-safe
--rw-r--r--   0 tristan   (1000) tristan   (1000)       48 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       20 2023-09-18 05:00:51.000000 buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      797 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/.asf.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4135 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/projectconfig.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2966 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/userconfig.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1505 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/compose.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1517 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/filter.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      995 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/import.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      964 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/manual.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1485 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/script.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2446 2024-04-17 09:10:06.000000 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/markdown_it/port.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1350 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/COMMITTERS.rst
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    11358 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/LICENSE
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      152 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/MANIFEST.in
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2183 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/NEWS
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      167 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/NOTICE
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/PKG-INFO
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      443 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/README.rst
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      985 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/project.conf
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      989 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/pyproject.toml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/requirements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       79 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/mypy-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      177 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/plugin-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      163 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/test-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      561 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/setup.cfg
+-rwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4076 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/setup.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/src/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      654 2024-04-17 09:07:37.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/__init__.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/__init__.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2297 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2259 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1775 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2114 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1566 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/__init__.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4261 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/_utils.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     8486 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/bzr.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    15309 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/cargo.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    23204 2024-04-07 14:36:16.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/docker.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    39482 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/git.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3510 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/patch.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     9290 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/pip.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2579 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      612 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-04 13:11:50.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/not-zip-safe
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       48 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/requires.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       20 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/top_level.txt
```

### Comparing `buildstream-plugins-2.1.0.dev0/.asf.yaml` & `buildstream-plugins-2.2.0.dev1/.asf.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/COMMITTERS.rst` & `buildstream-plugins-2.2.0.dev1/COMMITTERS.rst`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/LICENSE` & `buildstream-plugins-2.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/NEWS` & `buildstream-plugins-2.2.0.dev1/NEWS`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/PKG-INFO` & `buildstream-plugins-2.2.0.dev1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildstream-plugins
-Version: 2.1.0.dev0
+Version: 2.2.0.dev1
 Summary: A collection of plugins for BuildStream.
 Home-page: https://buildstream.build
 Author: The Apache Software Foundation
 Author-email: dev@buildstream.apache.org
 License: Apache License Version 2.0
 Project-URL: Documentation, https://apache.github.io/buildstream-plugins/
 Project-URL: Source, https://github.com/apache/buildstream-plugins/
@@ -18,17 +18,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: cargo
 License-File: LICENSE
 License-File: NOTICE
+Provides-Extra: cargo
+Requires-Dist: tomli; python_version < "3.11" and extra == "cargo"
 
 BuildStream Plugins
 ===================
 A collection of plugins for the `BuildStream <https://buildstream.build>`_ project.
 
 
 How to use plugins
```

### Comparing `buildstream-plugins-2.1.0.dev0/project.conf` & `buildstream-plugins-2.2.0.dev1/project.conf`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/pyproject.toml` & `buildstream-plugins-2.2.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/setup.cfg` & `buildstream-plugins-2.2.0.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/setup.py` & `buildstream-plugins-2.2.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/__init__.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 #
 # Remember to adjust this version number before tagging releases
 #
-__version__ = "2.1.0.dev0"
+__version__ = "2.2.0.dev1"
```

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/autotools.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/autotools.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/cmake.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/cmake.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/make.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/make.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/meson.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/meson.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/pip.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/pip.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/setuptools.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/elements/setuptools.yaml` & `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/bzr.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/bzr.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/cargo.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/cargo.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,33 +56,30 @@
 
 
 See `built-in functionality doumentation
 <https://docs.buildstream.build/master/buildstream.source.html#core-source-builtins>`_ for
 details on common configuration options for sources.
 """
 
-import contextlib
 import json
 import os.path
-import shutil
 import tarfile
-import urllib.error
-import urllib.request
-from urllib.parse import urljoin
 
 # We prefer tomli that was put into standard library as tomllib
 # starting from 3.11
 try:
     import tomllib  # type: ignore
 except ImportError:
     import tomli as tomllib  # type: ignore
 
 from buildstream import Source, SourceFetcher, SourceError
 from buildstream import utils
 
+from ._utils import download_file
+
 
 # This automatically goes into .cargo/config
 #
 _default_vendor_config_template = (
     "[source.crates-io]\n"
     + 'registry = "{vendorurl}"\n'
     + 'replace-with = "vendored-sources"\n'
@@ -105,15 +102,15 @@
     def __init__(self, cargo, name, version, sha=None):
         super().__init__()
 
         self.cargo = cargo
         self.name = name
         self.version = str(version)
         self.sha = sha
-        self.mark_download_url(self._get_url())
+        self.mark_download_url(cargo.url)
 
     ########################################################
     #     SourceFetcher API method implementations         #
     ########################################################
 
     def fetch(self, alias_override=None, **kwargs):
 
@@ -121,17 +118,17 @@
         # file to be already cached because Source.fetch() will
         # not be called if the source is already cached.
         #
         if os.path.isfile(self._get_mirror_file()):
             return  # pragma: nocover
 
         # Download the crate
-        crate_url = self._get_url(alias_override)
+        crate_url, auth_scheme = self._get_url(alias_override)
         with self.cargo.timed_activity("Downloading: {}".format(crate_url), silent_nested=True):
-            sha256 = self._download(crate_url)
+            sha256 = self._download(crate_url, auth_scheme)
             if self.sha is not None and sha256 != self.sha:
                 raise SourceError(
                     "File downloaded from {} has sha256sum '{}', not '{}'!".format(crate_url, sha256, self.sha)
                 )
 
     ########################################################
     #        Helper APIs for the Cargo Source to use       #
@@ -193,90 +190,63 @@
     #
     # Args:
     #    url (str): The url to download from
     #
     # Returns:
     #    (str): The sha256 checksum of the downloaded crate
     #
-    def _download(self, url):
-
-        try:
-            with self.cargo.tempdir() as td:
-                default_name = os.path.basename(url)
-                request = urllib.request.Request(url)
-                request.add_header("Accept", "*/*")
-                request.add_header("User-Agent", "BuildStream/2")
-
-                # We do not use etag in case what we have in cache is
-                # not matching ref in order to be able to recover from
-                # corrupted download.
-                if self.sha:
-                    etag = self._get_etag(self.sha)
-                    if etag and self.is_cached():
-                        request.add_header("If-None-Match", etag)
-
-                with contextlib.closing(urllib.request.urlopen(request)) as response:
-                    info = response.info()
-
-                    etag = info["ETag"] if "ETag" in info else None
-
-                    filename = info.get_filename(default_name)
-                    filename = os.path.basename(filename)
-                    local_file = os.path.join(td, filename)
-                    with open(local_file, "wb") as dest:
-                        shutil.copyfileobj(response, dest)
-
-                # Make sure url-specific mirror dir exists.
-                os.makedirs(self._get_mirror_dir(), exist_ok=True)
-
-                # Store by sha256sum
-                sha256 = utils.sha256sum(local_file)
-                # Even if the file already exists, move the new file over.
-                # In case the old file was corrupted somehow.
-                os.rename(local_file, self._get_mirror_file(sha256))
-
-                if etag:
-                    self._store_etag(sha256, etag)
-                return sha256
-
-        except urllib.error.HTTPError as e:
-            if e.code == 304:
-                # 304 Not Modified.
-                # Because we use etag only for matching sha, currently specified sha is what
-                # we would have downloaded.
-                return self.sha
-            raise SourceError(
-                "{}: Error mirroring {}: {}".format(self, url, e),
-                temporary=True,
-            ) from e
-
-        except (
-            urllib.error.URLError,
-            urllib.error.ContentTooShortError,
-            OSError,
-        ) as e:
-            raise SourceError(
-                "{}: Error mirroring {}: {}".format(self, url, e),
-                temporary=True,
-            ) from e
+    def _download(self, url, auth_scheme):
+        # We do not use etag in case what we have in cache is
+        # not matching ref in order to be able to recover from
+        # corrupted download.
+        if self.sha:
+            etag = self._get_etag(self.sha)
+        else:
+            etag = None
+
+        with self.cargo.tempdir() as td:
+            local_file, etag, error = download_file(url, etag, td, auth_scheme)
+
+            if error:
+                raise SourceError("{}: Error mirroring {}: {}".format(self, url, error), temporary=True)
+
+            # Make sure url-specific mirror dir exists.
+            os.makedirs(self._get_mirror_dir(), exist_ok=True)
+
+            # Store by sha256sum
+            sha256 = utils.sha256sum(local_file)
+            # Even if the file already exists, move the new file over.
+            # In case the old file was corrupted somehow.
+            os.rename(local_file, self._get_mirror_file(sha256))
+
+            if etag:
+                self._store_etag(sha256, etag)
+            return sha256
 
     # _get_url()
     #
     # Fetches the URL to download this crate from
     #
     # Args:
     #    alias (str|None): The URL alias to apply, if any
     #
     # Returns:
     #    (str): The URL for this crate
     #
     def _get_url(self, alias=None):
-        url = self.cargo.translate_url(self.cargo.url, alias_override=alias)
         path = "{name}/{name}-{version}.crate".format(name=self.name, version=self.version)
-        return urljoin(f"{url}/", path)
+        extra_data = {}
+        if utils.get_bst_version() >= (2, 2):
+            translated_url = self.cargo.translate_url(
+                self.cargo.url, suffix=path, alias_override=alias, extra_data=extra_data
+            )
+        else:
+            translated_url = self.cargo.translate_url(self.cargo.url, alias_override=alias) + path
+
+        return translated_url, extra_data.get("http-auth")
 
     # _get_etag()
     #
     # Fetches the locally stored ETag information for this
     # crate's download.
     #
     # Args:
@@ -339,30 +309,37 @@
     ########################################################
     #       Plugin/Source API method implementations       #
     ########################################################
     def configure(self, node):
 
         # The url before any aliasing
         #
-        self.url = node.get_str("url", "https://static.crates.io/crates")
+        self.original_url = node.get_str("url", "https://static.crates.io/crates")
         self.cargo_lock = node.get_str("cargo-lock", "Cargo.lock")
         self.vendor_dir = node.get_str("vendor-dir", "crates")
 
+        # If the specified URL is just an alias, require the alias to resolve
+        # to a URL with a trailing slash. Otherwise, append a trailing slash if
+        # it's missing, for backward compatibility.
+        self.url = self.original_url
+        if not self.url.endswith(":") and not self.url.endswith("/"):
+            self.url += "/"
+
         node.validate_keys(Source.COMMON_CONFIG_KEYS + ["url", "ref", "cargo-lock", "vendor-dir"])
 
         # Needs to be marked here so that `track` can translate it later.
         self.mark_download_url(self.url)
 
         self.load_ref(node)
 
     def preflight(self):
         return
 
     def get_unique_key(self):
-        return [self.url, self.cargo_lock, self.vendor_dir, self.ref]
+        return [self.original_url, self.cargo_lock, self.vendor_dir, self.ref]
 
     def is_resolved(self):
         return (self.ref is not None) and all(crate.is_resolved() for crate in self.crates)
 
     def is_cached(self):
         return all(crate.is_cached() for crate in self.crates)
 
@@ -411,17 +388,17 @@
         # Download the crates and get their shas
         for crate_obj in new_ref:
             if crate_obj["sha"] is not None:
                 continue
 
             crate = Crate(self, crate_obj["name"], crate_obj["version"])
 
-            crate_url = crate._get_url()
+            crate_url, auth_scheme = crate._get_url()
             with self.timed_activity("Downloading: {}".format(crate_url), silent_nested=True):
-                crate_obj["sha"] = crate._download(crate_url)
+                crate_obj["sha"] = crate._download(crate_url, auth_scheme)
 
         return new_ref
 
     def stage(self, directory):
 
         # Stage the crates into the vendor directory
         vendor_dir = os.path.join(directory, self.vendor_dir)
```

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/docker.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,21 @@
 
    # Specify the docker source kind
    kind: docker
 
    # Specify the registry endpoint, defaults to Docker Hub (optional)
    registry-url: https://registry.hub.docker.com
 
-   # Image path (required)
+   # Image path
    image: library/alpine
 
+   # Alternatively, you can specify a full url, the registry endpoint
+   # is assumed to be at the root of the domain
+   # url: https://registry.hub.docker.com/library/alpine
+
    # Image tag to follow (optional)
    track: latest
 
    # Specify the digest of the exact image to use (required)
    ref: 6c9f6f68a131ec6381da82f2bff978083ed7f4f7991d931bfa767b7965ebc94b
 
    # Some images are built for multiple platforms. When tracking a tag, we
@@ -117,14 +121,35 @@
     for arg in args:
         if not url.endswith("/"):
             url += "/"
         url = urllib.parse.urljoin(url, arg.lstrip("/"))
     return url
 
 
+# Handles authentication with a bearer token
+class BearerAuth(requests.auth.AuthBase):
+    def __init__(self, api_timeout=3):
+        self.token = None
+        self.api_timeout = api_timeout
+
+    def __call__(self, r):
+        if self.token:
+            r.headers["Authorization"] = "Bearer {}".format(self.token)
+        return r
+
+    def refresh_token(self, auth_challenge):
+        auth_vars = parse_bearer_authorization_challenge(auth_challenge)
+        # Respond to an Www-Authenticate challenge by requesting the necessary
+        # token from the 'realm' (endpoint) that we were given in the challenge.
+        request_url = "{realm}?service={service}&scope={scope}".format(**auth_vars)
+        response = requests.get(request_url, timeout=self.api_timeout)
+        response.raise_for_status()
+        self.token = response.json()["token"]
+
+
 # DockerManifestError
 #
 # Raised if something goes wrong while querying an image manifest from a remote
 # registry.
 #
 class DockerManifestError(SourceError):
     def __init__(self, message, manifest=None):
@@ -133,49 +158,37 @@
 
 
 class DockerRegistryV2Client:
     def __init__(self, endpoint, api_timeout=3):
         self.endpoint = endpoint
         self.api_timeout = api_timeout
 
-        self.token = None
+        self.auth = BearerAuth(api_timeout)
 
     def _request(self, subpath, extra_headers=None, stream=False, _reauthorized=False):
         if not extra_headers:
             extra_headers = {}
 
         headers = {"content-type": "application/json"}
         headers.update(extra_headers)
 
-        if self.token:
-            headers["Authorization"] = "Bearer {}".format(self.token)
-
         url = urljoin(self.endpoint, "v2", subpath)
-        response = requests.get(url, headers=headers, stream=stream, timeout=self.api_timeout)
+        response = requests.get(url, headers=headers, stream=stream, timeout=self.api_timeout, auth=self.auth)
 
         if response.status_code == requests.codes["unauthorized"] and not _reauthorized:
             # This request requires (re)authorization. See:
             # https://docs.docker.com/registry/spec/auth/token/
             auth_challenge = response.headers["Www-Authenticate"]
-            auth_vars = parse_bearer_authorization_challenge(auth_challenge)
-            self._auth(auth_vars["realm"], auth_vars["service"], auth_vars["scope"])
+            self.auth.refresh_token(auth_challenge)
             return self._request(subpath, extra_headers=extra_headers, _reauthorized=True)
         else:
             response.raise_for_status()
 
             return response
 
-    def _auth(self, realm, service, scope):
-        # Respond to an Www-Authenticate challenge by requesting the necessary
-        # token from the 'realm' (endpoint) that we were given in the challenge.
-        request_url = "{}?service={}&scope={}".format(realm, service, scope)
-        response = requests.get(request_url, timeout=self.api_timeout)
-        response.raise_for_status()
-        self.token = response.json()["token"]
-
     # digest():
     #
     # Calculate a Docker-compatible digest of an arbitrary string of bytes.
     #
     # Args:
     #    content (bytes): Content to hash
     #
@@ -351,22 +364,32 @@
     def configure(self, node):
         # url is deprecated, but accept it as a valid key so that we can raise
         # a nicer warning.
         node.validate_keys(
             Source.COMMON_CONFIG_KEYS + ["architecture", "registry-url", "image", "os", "ref", "track", "url"]
         )
 
-        if "url" in node:
-            raise SourceError(
-                "{}: 'url' parameter is now deprecated, " "use 'registry-url' and 'image' instead.".format(self)
-            )
+        if "url" in node and ("image" in node or "registry-url" in node):
+            raise SourceError("{}: May specify either 'url', or 'image' and 'registry-url'".format(self))
 
-        self.image = node.get_str("image")
-        self.original_registry_url = node.get_str("registry-url", _DOCKER_HUB_URL)
-        self.registry_url = self.translate_url(self.original_registry_url)
+        if "url" not in node and "image" not in node:
+            raise SourceError("{}: Must define either 'url' or 'image'".format(self))
+
+        if "url" in node:
+            self.url = node.get_str("url")
+            translated_url = self.translate_url(self.url)
+            scheme, netloc, path, _, _ = urllib.parse.urlsplit(translated_url)
+            self.registry_url = urllib.parse.urlunsplit((scheme, netloc, "", "", ""))
+            self.image = path
+
+        if "image" in node:
+            self.url = None
+            self.image = node.get_str("image")
+            self.original_registry_url = node.get_str("registry-url", _DOCKER_HUB_URL)
+            self.registry_url = self.translate_url(self.original_registry_url)
 
         if "ref" in node:
             self.digest = self._ref_to_digest(node.get_str("ref"))
         else:
             self.digest = None
         self.tag = node.get_str("track", "") or None
 
@@ -380,15 +403,18 @@
 
         self.manifest = None
 
     def preflight(self):
         return
 
     def get_unique_key(self):
-        return [self.original_registry_url, self.image, self.digest]
+        if self.url is not None:
+            return [self.url, self.digest]
+        else:
+            return [self.original_registry_url, self.image, self.digest]
 
     def get_ref(self):
         return None if self.digest is None else self._digest_to_ref(self.digest)
 
     def set_ref(self, ref, node):
         node["ref"] = ref
         self.digest = self._ref_to_digest(ref)
```

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/git.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/git.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/patch.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/patch.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins/sources/pip.py` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/pip.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/PKG-INFO` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildstream-plugins
-Version: 2.1.0.dev0
+Version: 2.2.0.dev1
 Summary: A collection of plugins for BuildStream.
 Home-page: https://buildstream.build
 Author: The Apache Software Foundation
 Author-email: dev@buildstream.apache.org
 License: Apache License Version 2.0
 Project-URL: Documentation, https://apache.github.io/buildstream-plugins/
 Project-URL: Source, https://github.com/apache/buildstream-plugins/
@@ -18,17 +18,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: cargo
 License-File: LICENSE
 License-File: NOTICE
+Provides-Extra: cargo
+Requires-Dist: tomli; python_version < "3.11" and extra == "cargo"
 
 BuildStream Plugins
 ===================
 A collection of plugins for the `BuildStream <https://buildstream.build>`_ project.
 
 
 How to use plugins
```

### Comparing `buildstream-plugins-2.1.0.dev0/src/buildstream_plugins.egg-info/entry_points.txt` & `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/entry_points.txt`

 * *Files identical despite different names*

