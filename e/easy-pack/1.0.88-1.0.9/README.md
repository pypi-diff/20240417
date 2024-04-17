# Comparing `tmp/easy-pack-1.0.88.tar.gz` & `tmp/easy-pack-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-pack-1.0.88.tar", last modified: Wed Apr 17 15:08:18 2024, max compression
+gzip compressed data, was "easy-pack-1.0.9.tar", last modified: Tue Sep 20 01:31:36 2022, max compression
```

## Comparing `easy-pack-1.0.88.tar` & `easy-pack-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:08:18.185151 easy-pack-1.0.88/
--rw-rw-rw-   0        0        0       31 2024-04-17 15:08:17.000000 easy-pack-1.0.88/MANIFEST.in
--rw-rw-rw-   0        0        0     4735 2024-04-17 15:08:18.183141 easy-pack-1.0.88/PKG-INFO
--rw-rw-rw-   0        0        0     3982 2024-04-17 15:08:17.000000 easy-pack-1.0.88/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:08:18.160150 easy-pack-1.0.88/easy_pack/
--rw-rw-rw-   0        0        0     3982 2024-04-17 15:08:17.000000 easy-pack-1.0.88/easy_pack/README.md
--rw-rw-rw-   0        0        0       45 2023-06-20 17:47:37.000000 easy-pack-1.0.88/easy_pack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:08:18.179140 easy-pack-1.0.88/easy_pack/__pycache__/
--rw-rw-rw-   0        0        0      189 2023-06-20 17:58:28.000000 easy-pack-1.0.88/easy_pack/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      192 2024-04-17 13:48:47.000000 easy-pack-1.0.88/easy_pack/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     7527 2023-12-22 23:04:49.000000 easy-pack-1.0.88/easy_pack/__pycache__/easy_pack_module.cpython-310.pyc
--rw-rw-rw-   0        0        0    14309 2024-04-17 13:58:14.000000 easy-pack-1.0.88/easy_pack/__pycache__/easy_pack_module.cpython-312.pyc
--rw-rw-rw-   0        0        0    11090 2024-04-17 13:57:52.000000 easy-pack-1.0.88/easy_pack/easy_pack_module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:08:18.181142 easy-pack-1.0.88/easy_pack/files/
--rw-rw-rw-   0        0        0     1466 2023-12-22 23:02:28.000000 easy-pack-1.0.88/easy_pack/files/build.py
--rw-rw-rw-   0        0        0     1636 2024-04-17 15:08:17.000000 easy-pack-1.0.88/easy_pack/license.txt
--rw-rw-rw-   0        0        0      133 2024-04-17 15:08:17.000000 easy-pack-1.0.88/easy_pack/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 15:08:18.182141 easy-pack-1.0.88/easy_pack.egg-info/
--rw-rw-rw-   0        0        0     4735 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 15:08:18.000000 easy-pack-1.0.88/easy_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 15:08:18.185151 easy-pack-1.0.88/setup.cfg
--rw-rw-rw-   0        0        0      518 2024-04-17 15:08:17.000000 easy-pack-1.0.88/setup.py
+drwxr-xr-x   0 german    (1000) german    (1000)        0 2022-09-20 01:31:36.735269 easy-pack-1.0.9/
+-rw-r--r--   0 german    (1000) german    (1000)      152 2022-09-20 01:31:36.733164 easy-pack-1.0.9/PKG-INFO
+drwxr-xr-x   0 german    (1000) german    (1000)        0 2022-09-20 01:31:36.653335 easy-pack-1.0.9/easy_pack/
+-rw-r--r--   0 german    (1000) german    (1000)    12256 2022-09-20 01:31:35.000000 easy-pack-1.0.9/easy_pack/easy_pack_module.py
+drwxr-xr-x   0 german    (1000) german    (1000)        0 2022-09-20 01:31:36.722329 easy-pack-1.0.9/easy_pack.egg-info/
+-rw-r--r--   0 german    (1000) german    (1000)      152 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/PKG-INFO
+-rw-r--r--   0 german    (1000) german    (1000)      234 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/SOURCES.txt
+-rw-r--r--   0 german    (1000) german    (1000)        1 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/dependency_links.txt
+-rw-r--r--   0 german    (1000) german    (1000)        1 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/not-zip-safe
+-rw-r--r--   0 german    (1000) german    (1000)        6 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/requires.txt
+-rw-r--r--   0 german    (1000) german    (1000)       10 2022-09-20 01:31:36.000000 easy-pack-1.0.9/easy_pack.egg-info/top_level.txt
+-rw-r--r--   0 german    (1000) german    (1000)       38 2022-09-20 01:31:36.736180 easy-pack-1.0.9/setup.cfg
+-rw-r--r--   0 german    (1000) german    (1000)      242 2022-09-20 01:31:35.000000 easy-pack-1.0.9/setup.py
```

