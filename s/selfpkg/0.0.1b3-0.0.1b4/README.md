# Comparing `tmp/selfpkg-0.0.1b3.tar.gz` & `tmp/selfpkg-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfpkg-0.0.1b3.tar", last modified: Tue Apr 16 08:44:56 2024, max compression
+gzip compressed data, was "selfpkg-0.0.1b4.tar", last modified: Tue Apr 16 09:07:00 2024, max compression
```

## Comparing `selfpkg-0.0.1b3.tar` & `selfpkg-0.0.1b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 08:44:49.000000 selfpkg-0.0.1b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 08:44:49.000000 selfpkg-0.0.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:44:56.798692 selfpkg-0.0.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/src/selfpkg/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 08:44:49.000000 selfpkg-0.0.1b3/src/selfpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 08:44:49.000000 selfpkg-0.0.1b3/src/selfpkg/greeting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/src/selfpkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 08:44:56.000000 selfpkg-0.0.1b3/src/selfpkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 08:44:56.000000 selfpkg-0.0.1b3/src/selfpkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:44:56.000000 selfpkg-0.0.1b3/src/selfpkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 08:44:56.000000 selfpkg-0.0.1b3/src/selfpkg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:44:56.802692 selfpkg-0.0.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 08:44:49.000000 selfpkg-0.0.1b3/tests/test_greeting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:07:00.770056 selfpkg-0.0.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 09:07:00.770056 selfpkg-0.0.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 09:06:57.000000 selfpkg-0.0.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 09:06:57.000000 selfpkg-0.0.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:07:00.770056 selfpkg-0.0.1b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:07:00.766056 selfpkg-0.0.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:07:00.766056 selfpkg-0.0.1b4/src/selfpkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 09:06:57.000000 selfpkg-0.0.1b4/src/selfpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 09:06:57.000000 selfpkg-0.0.1b4/src/selfpkg/greeting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:07:00.766056 selfpkg-0.0.1b4/src/selfpkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 09:07:00.000000 selfpkg-0.0.1b4/src/selfpkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 09:07:00.000000 selfpkg-0.0.1b4/src/selfpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:07:00.000000 selfpkg-0.0.1b4/src/selfpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 09:07:00.000000 selfpkg-0.0.1b4/src/selfpkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:07:00.766056 selfpkg-0.0.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 09:06:57.000000 selfpkg-0.0.1b4/tests/test_greeting.py
```

