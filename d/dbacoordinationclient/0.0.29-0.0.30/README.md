# Comparing `tmp/dbacoordinationclient-0.0.29.tar.gz` & `tmp/dbacoordinationclient-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbacoordinationclient-0.0.29.tar", last modified: Tue Apr 16 08:19:51 2024, max compression
+gzip compressed data, from Unix
```

## Comparing `dbacoordinationclient-0.0.29.tar` & `dbacoordinationclient-0.0.30.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:19:51.347522 dbacoordinationclient-0.0.29/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      237 2024-04-16 08:19:51.343522 dbacoordinationclient-0.0.29/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:19:51.343522 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      237 2024-04-16 08:19:51.000000 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2024-04-16 08:19:51.000000 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:19:51.000000 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 08:19:51.000000 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:19:51.000000 dbacoordinationclient-0.0.29/dbacoordinationclient.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 08:19:51.347522 dbacoordinationclient-0.0.29/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1219 2024-04-16 08:19:34.000000 dbacoordinationclient-0.0.29/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 06:55:19.000000 dbacoordinationclient-0.0.30/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-17 06:53:56.000000 dbacoordinationclient-0.0.30/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2024-04-17 06:55:19.000000 dbacoordinationclient-0.0.30/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/dbacoordinationclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-17 06:54:18.000000 dbacoordinationclient-0.0.30/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       33 2024-04-17 06:55:02.000000 dbacoordinationclient-0.0.30/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

