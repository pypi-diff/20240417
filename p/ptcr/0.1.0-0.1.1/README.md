# Comparing `tmp/ptcr-0.1.0.tar.gz` & `tmp/ptcr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.0.tar", last modified: Wed Apr 17 02:26:44 2024, max compression
+gzip compressed data, was "ptcr-0.1.1.tar", last modified: Wed Apr 17 02:34:04 2024, max compression
```

## Comparing `ptcr-0.1.0.tar` & `ptcr-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:26:44.515308 ptcr-0.1.0/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      357 2024-04-17 02:26:44.514305 ptcr-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:26:44.513305 ptcr-0.1.0/ptcr.egg-info/
--rw-rw-rw-   0        0        0      357 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 02:26:44.515308 ptcr-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      400 2024-04-17 02:26:33.000000 ptcr-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:34:04.650390 ptcr-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5724 2024-04-17 02:34:04.650390 ptcr-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:34:04.649391 ptcr-0.1.1/ptcr.egg-info/
+-rw-rw-rw-   0        0        0     5724 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:34:04.650390 ptcr-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      512 2024-04-17 02:34:00.000000 ptcr-0.1.1/setup.py
```

### Comparing `ptcr-0.1.0/LICENSE` & `ptcr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.0/README.md` & `ptcr-0.1.1/README.md`

 * *Files identical despite different names*

