# Comparing `tmp/xpk-0.3.0.tar.gz` & `tmp/xpk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpk-0.3.0.tar", last modified: Mon Feb 26 21:24:02 2024, max compression
+gzip compressed data, was "xpk-0.4.0.tar", last modified: Wed Apr 17 21:29:30 2024, max compression
```

## Comparing `xpk-0.3.0.tar` & `xpk-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-x---   0 vbarr    (992102) primarygroup (89939)        0 2024-02-26 21:24:02.572637 xpk-0.3.0/
--rw-r-----   0 vbarr    (992102) primarygroup (89939)    11358 2023-10-11 21:05:42.000000 xpk-0.3.0/LICENSE
--rw-r--r--   0 vbarr    (992102) primarygroup (89939)    21884 2024-02-26 21:24:02.572637 xpk-0.3.0/PKG-INFO
--rw-r-----   0 vbarr    (992102) primarygroup (89939)    21367 2024-02-22 20:42:52.000000 xpk-0.3.0/README.md
--rw-r-----   0 vbarr    (992102) primarygroup (89939)     1307 2024-02-26 21:06:00.000000 xpk-0.3.0/pyproject.toml
--rw-r-----   0 vbarr    (992102) primarygroup (89939)       38 2024-02-26 21:24:02.572637 xpk-0.3.0/setup.cfg
-drwxr-x---   0 vbarr    (992102) primarygroup (89939)        0 2024-02-26 21:24:02.572637 xpk-0.3.0/xpk.egg-info/
--rw-r--r--   0 vbarr    (992102) primarygroup (89939)    21884 2024-02-26 21:24:02.000000 xpk-0.3.0/xpk.egg-info/PKG-INFO
--rw-r-----   0 vbarr    (992102) primarygroup (89939)      177 2024-02-26 21:24:02.000000 xpk-0.3.0/xpk.egg-info/SOURCES.txt
--rw-r-----   0 vbarr    (992102) primarygroup (89939)        1 2024-02-26 21:24:02.000000 xpk-0.3.0/xpk.egg-info/dependency_links.txt
--rw-r-----   0 vbarr    (992102) primarygroup (89939)       33 2024-02-26 21:24:02.000000 xpk-0.3.0/xpk.egg-info/entry_points.txt
--rw-r-----   0 vbarr    (992102) primarygroup (89939)       11 2024-02-26 21:24:02.000000 xpk-0.3.0/xpk.egg-info/top_level.txt
--rw-r-----   0 vbarr    (992102) primarygroup (89939)   111620 2024-02-26 19:37:33.000000 xpk-0.3.0/xpk.py
+drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-17 21:29:30.540634 xpk-0.4.0/
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    11358 2024-04-17 21:29:16.000000 xpk-0.4.0/LICENSE
+-rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44328 2024-04-17 21:29:30.540634 xpk-0.4.0/PKG-INFO
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    43614 2024-04-17 21:29:16.000000 xpk-0.4.0/README.md
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)     1767 2024-04-17 21:29:16.000000 xpk-0.4.0/pyproject.toml
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       38 2024-04-17 21:29:30.540634 xpk-0.4.0/setup.cfg
+drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-17 21:29:30.540634 xpk-0.4.0/xpk.egg-info/
+-rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44328 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/PKG-INFO
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)      203 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/SOURCES.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        1 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/dependency_links.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       33 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/entry_points.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       76 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/requires.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        4 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/top_level.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)   215487 2024-04-17 21:29:16.000000 xpk-0.4.0/xpk.py
```

### Comparing `xpk-0.3.0/LICENSE` & `xpk-0.4.0/LICENSE`

 * *Files identical despite different names*

