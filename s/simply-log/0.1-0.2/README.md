# Comparing `tmp/simply-log-0.1.tar.gz` & `tmp/simply-log-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-log-0.1.tar", last modified: Wed Apr 17 09:54:58 2024, max compression
+gzip compressed data, was "simply-log-0.2.tar", last modified: Wed Apr 17 09:58:21 2024, max compression
```

## Comparing `simply-log-0.1.tar` & `simply-log-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:54:58.294327 simply-log-0.1/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       52 2024-04-17 09:54:58.294160 simply-log-0.1/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      499 2024-04-17 09:45:56.000000 simply-log-0.1/README.md
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:54:58.293368 simply-log-0.1/log/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.1/log/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.1/log/main.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 09:54:58.294384 simply-log-0.1/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      132 2024-04-17 09:54:07.000000 simply-log-0.1/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:54:58.293977 simply-log-0.1/simply_log.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       52 2024-04-17 09:54:58.000000 simply-log-0.1/simply_log.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 09:54:58.000000 simply-log-0.1/simply_log.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 09:54:58.000000 simply-log-0.1/simply_log.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 09:54:58.000000 simply-log-0.1/simply_log.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:58:21.517401 simply-log-0.2/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      592 2024-04-17 09:58:21.517245 simply-log-0.2/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      499 2024-04-17 09:45:56.000000 simply-log-0.2/README.md
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:58:21.516018 simply-log-0.2/log/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2/log/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2/log/main.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 09:58:21.517452 simply-log-0.2/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      308 2024-04-17 09:58:05.000000 simply-log-0.2/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 09:58:21.516889 simply-log-0.2/simply_log.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      592 2024-04-17 09:58:21.000000 simply-log-0.2/simply_log.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 09:58:21.000000 simply-log-0.2/simply_log.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 09:58:21.000000 simply-log-0.2/simply_log.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 09:58:21.000000 simply-log-0.2/simply_log.egg-info/top_level.txt
```

### Comparing `simply-log-0.1/log/main.py` & `simply-log-0.2/log/main.py`

 * *Files identical despite different names*

