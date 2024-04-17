# Comparing `tmp/selfpkg-0.0.2.tar.gz` & `tmp/selfpkg-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfpkg-0.0.2.tar", last modified: Wed Apr 17 09:26:50 2024, max compression
+gzip compressed data, was "selfpkg-0.0.3a1.tar", last modified: Wed Apr 17 09:39:06 2024, max compression
```

## Comparing `selfpkg-0.0.2.tar` & `selfpkg-0.0.3a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:26:50.786759 selfpkg-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 09:26:50.786759 selfpkg-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 09:26:43.000000 selfpkg-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-17 09:26:43.000000 selfpkg-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:26:50.786759 selfpkg-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:26:50.782760 selfpkg-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:26:50.782760 selfpkg-0.0.2/src/selfpkg/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 09:26:43.000000 selfpkg-0.0.2/src/selfpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 09:26:43.000000 selfpkg-0.0.2/src/selfpkg/farewell.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 09:26:43.000000 selfpkg-0.0.2/src/selfpkg/greeting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:26:50.782760 selfpkg-0.0.2/src/selfpkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 09:26:50.000000 selfpkg-0.0.2/src/selfpkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:26:50.000000 selfpkg-0.0.2/src/selfpkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:26:50.000000 selfpkg-0.0.2/src/selfpkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:26:50.000000 selfpkg-0.0.2/src/selfpkg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:26:50.782760 selfpkg-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 09:26:43.000000 selfpkg-0.0.2/tests/test_greeting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/src/selfpkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/src/selfpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/src/selfpkg/farewell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/src/selfpkg/greeting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/src/selfpkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 09:39:06.000000 selfpkg-0.0.3a1/src/selfpkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:39:06.000000 selfpkg-0.0.3a1/src/selfpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:39:06.000000 selfpkg-0.0.3a1/src/selfpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:39:06.000000 selfpkg-0.0.3a1/src/selfpkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:39:06.147239 selfpkg-0.0.3a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 09:39:02.000000 selfpkg-0.0.3a1/tests/test_greeting.py
```

