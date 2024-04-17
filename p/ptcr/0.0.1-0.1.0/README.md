# Comparing `tmp/ptcr-0.0.1.tar.gz` & `tmp/ptcr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.0.1.tar", last modified: Wed Apr 17 02:20:28 2024, max compression
+gzip compressed data, was "ptcr-0.1.0.tar", last modified: Wed Apr 17 02:26:44 2024, max compression
```

## Comparing `ptcr-0.0.1.tar` & `ptcr-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:20:28.459104 ptcr-0.0.1/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5833 2024-04-17 02:20:28.458104 ptcr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.0.1/README.md
--rw-rw-rw-   0        0        0      494 2024-04-17 02:20:15.000000 ptcr-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 02:20:28.459104 ptcr-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 02:20:28.307137 ptcr-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 02:20:28.456107 ptcr-0.0.1/src/ptcr.egg-info/
--rw-rw-rw-   0        0        0     5833 2024-04-17 02:20:28.000000 ptcr-0.0.1/src/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-17 02:20:28.000000 ptcr-0.0.1/src/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:20:28.000000 ptcr-0.0.1/src/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 02:20:28.000000 ptcr-0.0.1/src/ptcr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 02:20:28.454110 ptcr-0.0.1/src/ptcr2/
--rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.0.1/src/ptcr2/__init__.py
--rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.0.1/src/ptcr2/automata_utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.0.1/src/ptcr2/base_model.py
--rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.0.1/src/ptcr2/belief_tree.py
--rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.0.1/src/ptcr2/event_predictor.py
--rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.0.1/src/ptcr2/fom.py
--rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.0.1/src/ptcr2/markov_chain.py
--rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.0.1/src/ptcr2/markov_decision_process.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:26:44.515308 ptcr-0.1.0/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      357 2024-04-17 02:26:44.514305 ptcr-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:26:44.513305 ptcr-0.1.0/ptcr.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:26:44.000000 ptcr-0.1.0/ptcr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:26:44.515308 ptcr-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      400 2024-04-17 02:26:33.000000 ptcr-0.1.0/setup.py
```

### Comparing `ptcr-0.0.1/LICENSE` & `ptcr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.0.1/PKG-INFO` & `ptcr-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ptcr
-Version: 0.0.1
-Summary: Construct and process PTCR simulations.
-Author-email: Tiernan Lindauer <tiernanlind@tamu.edu>
-Project-URL: Homepage, https://github.com/T-Lind/ptcr
-Project-URL: Issues, https://github.com/T-Lind/ptcr/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: ==3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 ## Overview
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
```

