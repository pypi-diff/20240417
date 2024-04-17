# Comparing `tmp/omniblack.setup-0.0.1.tar.gz` & `tmp/omniblack.setup-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniblack.setup-0.0.1.tar", last modified: Sun Oct  3 19:53:15 2021, max compression
+gzip compressed data, was "omniblack.setup-0.1.0.tar", last modified: Wed Apr 17 20:11:53 2024, max compression
```

## Comparing `omniblack.setup-0.0.1.tar` & `omniblack.setup-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2021-10-03 19:53:15.965623 omniblack.setup-0.0.1/
--rw-r--r--   0 terryp    (1000) terryp    (1000)      736 2021-10-03 19:53:15.965623 omniblack.setup-0.0.1/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      457 2021-10-03 19:52:58.000000 omniblack.setup-0.0.1/README.md
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2021-10-03 19:53:15.964623 omniblack.setup-0.0.1/omniblack/
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2021-10-03 19:53:15.965623 omniblack.setup-0.0.1/omniblack/setup/
--rw-r--r--   0 terryp    (1000) terryp    (1000)     3596 2021-10-03 19:45:15.000000 omniblack.setup-0.0.1/omniblack/setup/__init__.py
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2021-10-03 19:53:15.965623 omniblack.setup-0.0.1/omniblack.setup.egg-info/
--rw-r--r--   0 terryp    (1000) terryp    (1000)      736 2021-10-03 19:53:15.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      289 2021-10-03 19:53:15.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/SOURCES.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2021-10-03 19:53:15.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/dependency_links.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       46 2021-10-03 19:53:15.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/requires.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2021-10-03 19:53:15.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/top_level.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2021-09-28 16:07:19.000000 omniblack.setup-0.0.1/omniblack.setup.egg-info/zip-safe
--rw-r--r--   0 terryp    (1000) terryp    (1000)      648 2021-10-03 19:45:28.000000 omniblack.setup-0.0.1/pyproject.toml
--rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2021-10-03 19:53:15.965623 omniblack.setup-0.0.1/setup.cfg
--rw-r--r--   0 terryp    (1000) terryp    (1000)      202 2021-10-03 17:28:25.000000 omniblack.setup-0.0.1/setup.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-17 20:11:53.391312 omniblack.setup-0.1.0/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    11358 2023-02-07 20:02:33.000000 omniblack.setup-0.1.0/LICENSE.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       27 2024-04-17 18:19:25.000000 omniblack.setup-0.1.0/MANIFEST.in
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13609 2024-04-17 20:11:53.391312 omniblack.setup-0.1.0/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      104 2024-04-17 20:00:27.000000 omniblack.setup-0.1.0/README.md
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       43 2024-04-17 18:19:25.000000 omniblack.setup-0.1.0/package_config.yaml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      901 2024-04-17 20:11:35.000000 omniblack.setup-0.1.0/pyproject.toml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-04-17 20:11:53.391312 omniblack.setup-0.1.0/setup.cfg
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-17 20:11:53.388312 omniblack.setup-0.1.0/src/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-17 20:11:53.388312 omniblack.setup-0.1.0/src/omniblack/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-17 20:11:53.391312 omniblack.setup-0.1.0/src/omniblack/setup/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      395 2024-04-17 18:19:25.000000 omniblack.setup-0.1.0/src/omniblack/setup/__init__.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-17 20:11:53.390312 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13609 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      372 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/SOURCES.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/dependency_links.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       76 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/entry_points.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       29 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/requires.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-04-17 20:11:53.000000 omniblack.setup-0.1.0/src/omniblack.setup.egg-info/top_level.txt
```

