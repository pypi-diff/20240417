# Comparing `tmp/simple_performance_timer-0.1.2.tar.gz` & `tmp/simple_performance_timer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_performance_timer-0.1.2.tar", max compression
+gzip compressed data, was "simple_performance_timer-0.1.3.tar", max compression
```

## Comparing `simple_performance_timer-0.1.2.tar` & `simple_performance_timer-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       29 2023-12-23 08:04:12.521429 simple_performance_timer-0.1.2/README.md
--rw-r--r--   0        0        0      257 2023-12-23 09:31:49.030249 simple_performance_timer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1886 2023-12-23 09:31:38.800252 simple_performance_timer-0.1.2/simple_performance_timer/Timer.py
--rw-r--r--   0        0        0        0 2023-12-23 08:01:38.261463 simple_performance_timer-0.1.2/simple_performance_timer/__init__.py
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 simple_performance_timer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2024-04-17 04:40:10.856678 simple_performance_timer-0.1.3/README.md
+-rw-r--r--   0        0        0      257 2024-04-17 04:40:50.866676 simple_performance_timer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-04-17 04:40:14.986678 simple_performance_timer-0.1.3/simple_performance_timer/Timer.py
+-rw-r--r--   0        0        0        0 2024-04-17 04:40:14.986678 simple_performance_timer-0.1.3/simple_performance_timer/__init__.py
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 simple_performance_timer-0.1.3/PKG-INFO
```

### Comparing `simple_performance_timer-0.1.2/simple_performance_timer/Timer.py` & `simple_performance_timer-0.1.3/simple_performance_timer/Timer.py`

 * *Files identical despite different names*

