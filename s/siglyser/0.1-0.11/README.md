# Comparing `tmp/siglyser-0.1.tar.gz` & `tmp/siglyser-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglyser-0.1.tar", last modified: Wed Apr 17 16:15:46 2024, max compression
+gzip compressed data, was "siglyser-0.11.tar", last modified: Wed Apr 17 16:52:08 2024, max compression
```

## Comparing `siglyser-0.1.tar` & `siglyser-0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 16:15:46.598335 siglyser-0.1/
--rw-rw-rw-   0        0        0       53 2024-04-17 16:15:46.596809 siglyser-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      143 2024-04-17 15:48:54.000000 siglyser-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 16:15:46.598335 siglyser-0.1/setup.cfg
--rw-rw-rw-   0        0        0      208 2024-04-17 16:06:15.000000 siglyser-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:15:46.578317 siglyser-0.1/siglyser/
--rw-rw-rw-   0        0        0       53 2024-04-17 15:58:24.000000 siglyser-0.1/siglyser/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-17 15:58:21.000000 siglyser-0.1/siglyser/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:15:46.595807 siglyser-0.1/siglyser.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-17 16:15:46.000000 siglyser-0.1/siglyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-17 16:15:46.000000 siglyser-0.1/siglyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 16:15:46.000000 siglyser-0.1/siglyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 16:15:46.000000 siglyser-0.1/siglyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 16:52:08.283248 siglyser-0.11/
+-rw-rw-rw-   0        0        0      242 2024-04-17 16:52:08.283248 siglyser-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2024-04-17 15:48:54.000000 siglyser-0.11/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 16:52:08.283248 siglyser-0.11/setup.cfg
+-rw-rw-rw-   0        0        0      358 2024-04-17 16:51:06.000000 siglyser-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:52:08.283248 siglyser-0.11/siglyser/
+-rw-rw-rw-   0        0        0       53 2024-04-17 16:48:28.000000 siglyser-0.11/siglyser/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-17 16:48:27.000000 siglyser-0.11/siglyser/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:52:08.283248 siglyser-0.11/siglyser.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-04-17 16:52:08.000000 siglyser-0.11/siglyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-04-17 16:52:08.000000 siglyser-0.11/siglyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 16:52:08.000000 siglyser-0.11/siglyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 16:52:08.000000 siglyser-0.11/siglyser.egg-info/top_level.txt
```

### Comparing `siglyser-0.1/siglyser/main.py` & `siglyser-0.11/siglyser/main.py`

 * *Files identical despite different names*

