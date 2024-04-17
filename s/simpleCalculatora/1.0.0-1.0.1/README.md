# Comparing `tmp/simpleCalculatora-1.0.0.tar.gz` & `tmp/simpleCalculatora-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleCalculatora-1.0.0.tar", last modified: Wed Apr 17 03:17:31 2024, max compression
+gzip compressed data, was "simpleCalculatora-1.0.1.tar", last modified: Wed Apr 17 03:20:07 2024, max compression
```

## Comparing `simpleCalculatora-1.0.0.tar` & `simpleCalculatora-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 03:17:31.844594 simpleCalculatora-1.0.0/
--rw-rw-rw-   0        0        0      201 2024-04-17 03:17:31.843558 simpleCalculatora-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 03:17:31.844594 simpleCalculatora-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      407 2024-04-17 03:17:15.000000 simpleCalculatora-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:17:31.839898 simpleCalculatora-1.0.0/simpleCalculatora/
--rw-rw-rw-   0        0        0       42 2024-04-17 03:15:16.000000 simpleCalculatora-1.0.0/simpleCalculatora/__init__.py
--rw-rw-rw-   0        0        0      163 2024-04-17 02:34:24.000000 simpleCalculatora-1.0.0/simpleCalculatora/calculadora.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:17:31.843558 simpleCalculatora-1.0.0/simpleCalculatora.egg-info/
--rw-rw-rw-   0        0        0      201 2024-04-17 03:17:31.000000 simpleCalculatora-1.0.0/simpleCalculatora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-17 03:17:31.000000 simpleCalculatora-1.0.0/simpleCalculatora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 03:17:31.000000 simpleCalculatora-1.0.0/simpleCalculatora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 03:17:31.000000 simpleCalculatora-1.0.0/simpleCalculatora.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 03:20:07.021839 simpleCalculatora-1.0.1/
+-rw-rw-rw-   0        0        0      201 2024-04-17 03:20:07.020839 simpleCalculatora-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-17 03:20:07.021839 simpleCalculatora-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      407 2024-04-17 03:19:40.000000 simpleCalculatora-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:20:07.017839 simpleCalculatora-1.0.1/simpleCalculatora/
+-rw-rw-rw-   0        0        0       74 2024-04-17 03:20:02.000000 simpleCalculatora-1.0.1/simpleCalculatora/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-04-17 02:34:24.000000 simpleCalculatora-1.0.1/simpleCalculatora/calculadora.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:20:07.020839 simpleCalculatora-1.0.1/simpleCalculatora.egg-info/
+-rw-rw-rw-   0        0        0      201 2024-04-17 03:20:06.000000 simpleCalculatora-1.0.1/simpleCalculatora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-17 03:20:06.000000 simpleCalculatora-1.0.1/simpleCalculatora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 03:20:06.000000 simpleCalculatora-1.0.1/simpleCalculatora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 03:20:06.000000 simpleCalculatora-1.0.1/simpleCalculatora.egg-info/top_level.txt
```

