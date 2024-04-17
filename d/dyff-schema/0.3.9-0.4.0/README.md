# Comparing `tmp/dyff_schema-0.3.9.tar.gz` & `tmp/dyff_schema-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.3.9.tar", last modified: Sat Apr 13 18:44:26 2024, max compression
+gzip compressed data, was "dyff_schema-0.4.0.tar", last modified: Wed Apr 17 20:40:21 2024, max compression
```

## Comparing `dyff_schema-0.3.9.tar` & `dyff_schema-0.4.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.570580 dyff_schema-0.3.9/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.577580 dyff_schema-0.3.9/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.578580 dyff_schema-0.3.9/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.578580 dyff_schema-0.3.9/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.579580 dyff_schema-0.3.9/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.580580 dyff_schema-0.3.9/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.582580 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.582580 dyff_schema-0.3.9/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    56247 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.583580 dyff_schema-0.3.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.501099 dyff_schema-0.4.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.508099 dyff_schema-0.4.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.512099 dyff_schema-0.4.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.514099 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.514099 dyff_schema-0.4.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    56634 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:40:21.517099 dyff_schema-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.515099 dyff_schema-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/tests/test_import.py
```

### Comparing `dyff_schema-0.3.9/.gitlab-ci.yml` & `dyff_schema-0.4.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 include:
   - project: buildgarden/pipelines/gitlab
     ref: 0.2.2
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
-    ref: 0.1.0
+    ref: 0.2.1
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
```

### Comparing `dyff_schema-0.3.9/.pre-commit-config.yaml` & `dyff_schema-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/.secrets.baseline` & `dyff_schema-0.4.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/CODE_OF_CONDUCT.md` & `dyff_schema-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/LICENSE` & `dyff_schema-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/PKG-INFO` & `dyff_schema-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.9
+Version: 0.4.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.3.9/README.md` & `dyff_schema-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/__init__.py` & `dyff_schema-0.4.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/copydoc.py` & `dyff_schema-0.4.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/ids.py` & `dyff_schema-0.4.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/quantity.py` & `dyff_schema-0.4.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/base.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,23 +135,14 @@
     Label values must have 63 characters or fewer (can be empty).
 
     See: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
     """
     return _k8s_label_maxlen()
 
 
-class StorageSignedURL(DyffSchemaBaseModel):
-    url: str = pydantic.Field(description="The signed URL")
-    method: str = pydantic.Field(description="The HTTP method applicable to the URL")
-    headers: dict[str, str] = pydantic.Field(
-        default_factory=dict,
-        description="Mandatory headers that must be passed with the request",
-    )
-
-
 class Entities(str, enum.Enum):
     """The kinds of entities in the dyff system."""
 
     Account = "Account"
     Analysis = "Analysis"
     Audit = "Audit"
     AuditProcedure = "AuditProcedure"
@@ -467,14 +458,51 @@
         description="For account keys: a secret value to check when verifying the APIKey",
     )
     grants: list[AccessGrant] = pydantic.Field(
         default_factory=list, description="AccessGrants associated with the APIKey"
     )
 
 
+# ----------------------------------------------------------------------------
+
+
+class Digest(DyffSchemaBaseModel):
+    md5: Optional[str] = pydantic.Field(
+        default=None, description="md5 digest of artifact data"
+    )
+
+
+class Artifact(DyffSchemaBaseModel):
+    # TODO: In v1, rename this to 'contentType' or something and commit to making it the MIME type
+    kind: Optional[str] = pydantic.Field(
+        default=None, description="The kind of artifact"
+    )
+    path: str = pydantic.Field(
+        description="The relative path of the artifact within the tree"
+    )
+    digest: Digest = pydantic.Field(
+        default_factory=Digest,
+        description="One or more message digests (hashes) of the artifact data",
+    )
+
+
+class StorageSignedURL(DyffSchemaBaseModel):
+    url: str = pydantic.Field(description="The signed URL")
+    method: str = pydantic.Field(description="The HTTP method applicable to the URL")
+    headers: dict[str, str] = pydantic.Field(
+        default_factory=dict,
+        description="Mandatory headers that must be passed with the request",
+    )
+
+
+class ArtifactURL(DyffSchemaBaseModel):
+    artifact: Artifact
+    signedURL: StorageSignedURL
+
+
 class AuditRequirement(DyffSchemaBaseModel):
     """An evaluation report that must exist in order to apply an AuditProcedure."""
 
     dataset: str
     rubric: str
 
 
@@ -539,29 +567,14 @@
     Dataset."""
 
     action: str
     name: Optional[str] = None
     type: Optional[str] = None
 
 
-class Digest(DyffSchemaBaseModel):
-    md5: Optional[str] = pydantic.Field(None)
-
-
-class Artifact(DyffSchemaBaseModel):
-    # TODO: Enumerate the available kinds
-    kind: str = pydantic.Field(description="The kind of artifact")
-    path: str = pydantic.Field(
-        description="The relative path of the artifact within the dataset"
-    )
-    digest: Digest = pydantic.Field(
-        description="One or more message digests (hashes) of the artifact data"
-    )
-
-
 class DyffDataSchema(DyffSchemaBaseModel):
     components: list[str] = pydantic.Field(
         min_items=1,
         description="A list of named dyff data schemas. The final schema is"
         " the composition of these component schemas.",
     )
     schemaVersion: SomeSchemaVersion = pydantic.Field(
@@ -1709,14 +1722,15 @@
     "AnalysisOutputQueryFields",
     "AnalysisScope",
     "Annotation",
     "APIFunctions",
     "APIKey",
     "ArchiveFormat",
     "Artifact",
+    "ArtifactURL",
     "Audit",
     "AuditProcedure",
     "AuditRequirement",
     "DataSchema",
     "Dataset",
     "DatasetBase",
     "DatasetFilter",
```

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/requests.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff/schema/v0/r1/test.py` & `dyff_schema-0.4.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.4.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.9
+Version: 0.4.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.3.9/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.4.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/pyproject.toml` & `dyff_schema-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.3.9/tests/test_import.py` & `dyff_schema-0.4.0/tests/test_import.py`

 * *Files identical despite different names*

