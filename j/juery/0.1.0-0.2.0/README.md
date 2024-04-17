# Comparing `tmp/juery-0.1.0.tar.gz` & `tmp/juery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juery-0.1.0.tar", max compression
+gzip compressed data, was "juery-0.2.0.tar", max compression
```

## Comparing `juery-0.1.0.tar` & `juery-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 07:21:43.398054 juery-0.1.0/README.md
--rw-r--r--   0        0        0       92 2024-04-15 07:24:52.880634 juery-0.1.0/juery/__init__.py
--rw-r--r--   0        0        0     2229 2024-04-15 07:22:39.160438 juery-0.1.0/juery/juery.py
--rw-r--r--   0        0        0      118 2024-04-15 07:22:20.151676 juery-0.1.0/juery/payload.py
--rw-r--r--   0        0        0      272 2024-04-15 07:25:15.721189 juery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 juery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 07:21:43.398054 juery-0.2.0/README.md
+-rw-r--r--   0        0        0       92 2024-04-15 07:24:52.880634 juery-0.2.0/juery/__init__.py
+-rw-r--r--   0        0        0     2494 2024-04-17 02:16:23.316784 juery-0.2.0/juery/juery.py
+-rw-r--r--   0        0        0      118 2024-04-15 07:22:20.151676 juery-0.2.0/juery/payload.py
+-rw-r--r--   0        0        0      677 2024-04-17 02:08:40.419107 juery-0.2.0/juery/special.py
+-rw-r--r--   0        0        0      272 2024-04-17 02:18:56.331842 juery-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 juery-0.2.0/PKG-INFO
```

