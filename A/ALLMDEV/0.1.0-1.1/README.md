# Comparing `tmp/allmdev-0.1.0.tar.gz` & `tmp/allmdev-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allmdev-0.1.0.tar", last modified: Tue Apr 16 05:12:22 2024, max compression
+gzip compressed data, was "allmdev-1.1.tar", last modified: Wed Apr 17 15:21:39 2024, max compression
```

## Comparing `allmdev-0.1.0.tar` & `allmdev-1.1.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 05:12:22.686056 allmdev-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-16 05:12:22.684670 allmdev-0.1.0/ALLMDEV.egg-info/
--rw-rw-rw-   0        0        0      464 2024-04-16 05:12:22.000000 allmdev-0.1.0/ALLMDEV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-04-16 05:12:22.000000 allmdev-0.1.0/ALLMDEV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 05:12:22.000000 allmdev-0.1.0/ALLMDEV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-16 05:12:22.000000 allmdev-0.1.0/ALLMDEV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 05:12:22.000000 allmdev-0.1.0/ALLMDEV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      464 2024-04-16 05:12:22.686056 allmdev-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 05:12:22.686056 allmdev-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-04-16 05:11:23.000000 allmdev-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:21:39.313561 allmdev-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-17 15:21:39.300594 allmdev-1.1/ALLMDEV/
+-rw-rw-rw-   0        0        0       39 2024-04-17 06:01:48.000000 allmdev-1.1/ALLMDEV/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-04-17 06:35:05.000000 allmdev-1.1/ALLMDEV/cli.py
+-rw-rw-rw-   0        0        0    10332 2024-04-17 15:17:26.000000 allmdev-1.1/ALLMDEV/instruct.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:21:39.311082 allmdev-1.1/ALLMDEV.egg-info/
+-rw-rw-rw-   0        0        0     1995 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 15:21:39.000000 allmdev-1.1/ALLMDEV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1995 2024-04-17 15:21:39.312156 allmdev-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1358 2024-04-17 12:23:16.000000 allmdev-1.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 06:31:02.000000 allmdev-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:21:39.313561 allmdev-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-04-17 15:21:15.000000 allmdev-1.1/setup.py
```

