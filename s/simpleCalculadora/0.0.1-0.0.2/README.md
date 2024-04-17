# Comparing `tmp/simpleCalculadora-0.0.1.tar.gz` & `tmp/simpleCalculadora-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleCalculadora-0.0.1.tar", last modified: Wed Apr 17 02:47:45 2024, max compression
+gzip compressed data, was "simpleCalculadora-0.0.2.tar", last modified: Wed Apr 17 02:56:09 2024, max compression
```

## Comparing `simpleCalculadora-0.0.1.tar` & `simpleCalculadora-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:47:45.624263 simpleCalculadora-0.0.1/
--rw-rw-rw-   0        0        0      201 2024-04-17 02:47:45.624263 simpleCalculadora-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 02:47:45.624263 simpleCalculadora-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      407 2024-04-17 02:42:56.000000 simpleCalculadora-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 02:47:45.620263 simpleCalculadora-0.0.1/simpleCalculadora/
--rw-rw-rw-   0        0        0       25 2024-04-17 02:35:10.000000 simpleCalculadora-0.0.1/simpleCalculadora/__init__.py
--rw-rw-rw-   0        0        0      163 2024-04-17 02:34:24.000000 simpleCalculadora-0.0.1/simpleCalculadora/calculadora.py
-drwxrwxrwx   0        0        0        0 2024-04-17 02:47:45.623264 simpleCalculadora-0.0.1/simpleCalculadora.egg-info/
--rw-rw-rw-   0        0        0      201 2024-04-17 02:47:45.000000 simpleCalculadora-0.0.1/simpleCalculadora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-17 02:47:45.000000 simpleCalculadora-0.0.1/simpleCalculadora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:47:45.000000 simpleCalculadora-0.0.1/simpleCalculadora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 02:47:45.000000 simpleCalculadora-0.0.1/simpleCalculadora.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 02:56:09.637524 simpleCalculadora-0.0.2/
+-rw-rw-rw-   0        0        0      201 2024-04-17 02:56:09.637524 simpleCalculadora-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:56:09.637524 simpleCalculadora-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      407 2024-04-17 02:56:05.000000 simpleCalculadora-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:56:09.633524 simpleCalculadora-0.0.2/simpleCalculadora/
+-rw-rw-rw-   0        0        0        0 2024-04-17 02:55:57.000000 simpleCalculadora-0.0.2/simpleCalculadora/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-04-17 02:34:24.000000 simpleCalculadora-0.0.2/simpleCalculadora/calculadora.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:56:09.636525 simpleCalculadora-0.0.2/simpleCalculadora.egg-info/
+-rw-rw-rw-   0        0        0      201 2024-04-17 02:56:09.000000 simpleCalculadora-0.0.2/simpleCalculadora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-17 02:56:09.000000 simpleCalculadora-0.0.2/simpleCalculadora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:56:09.000000 simpleCalculadora-0.0.2/simpleCalculadora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 02:56:09.000000 simpleCalculadora-0.0.2/simpleCalculadora.egg-info/top_level.txt
```

