# Comparing `tmp/spear_ai_ruff_config-3.0.0.tar.gz` & `tmp/spear_ai_ruff_config-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear_ai_ruff_config-3.0.0.tar", max compression
+gzip compressed data, was "spear_ai_ruff_config-4.0.0.tar", max compression
```

## Comparing `spear_ai_ruff_config-3.0.0.tar` & `spear_ai_ruff_config-4.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      407 2024-04-17 09:56:23.916062 spear_ai_ruff_config-3.0.0/README.md
--rw-r--r--   0        0        0      474 2024-04-17 09:56:23.916062 spear_ai_ruff_config-3.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2024-04-17 09:56:23.916062 spear_ai_ruff_config-3.0.0/spear_ai_ruff_config/__init__.py
--rw-r--r--   0        0        0      820 2024-04-17 09:56:23.916062 spear_ai_ruff_config-3.0.0/spear_ai_ruff_config/config.toml
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 spear_ai_ruff_config-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      407 2024-04-17 14:29:16.295641 spear_ai_ruff_config-4.0.0/README.md
+-rw-r--r--   0        0        0      474 2024-04-17 14:29:16.295641 spear_ai_ruff_config-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-04-17 14:29:16.295641 spear_ai_ruff_config-4.0.0/spear_ai_ruff_config/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-17 14:29:16.295641 spear_ai_ruff_config-4.0.0/spear_ai_ruff_config/config.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 spear_ai_ruff_config-4.0.0/PKG-INFO
```

### Comparing `spear_ai_ruff_config-3.0.0/spear_ai_ruff_config/config.toml` & `spear_ai_ruff_config-4.0.0/spear_ai_ruff_config/config.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 line-length = 120
 target-version = "py311"
 
 [lint]
 allowed-confusables = [
+  "–",
   "‘",
   "’"
 ]
 ignore = [
   "COM812",
   "ISC001",
   "S101",
```

### Comparing `spear_ai_ruff_config-3.0.0/PKG-INFO` & `spear_ai_ruff_config-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: spear-ai-ruff-config
-Version: 3.0.0
+Version: 4.0.0
 Summary: Spear AI Ruff config
 Home-page: https://github.com/spear-ai/citizen
 Keywords: ai,config,ruff,spear
 Author: Spear AI
 Author-email: org@spear.ai
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ruff (>=0.2.0,<0.3.0)
+Requires-Dist: ruff (>=0.3.7,<0.4.0)
 Project-URL: Repository, https://github.com/spear-ai/citizen
 Description-Content-Type: text/markdown
 
 # @spear-ai/ruff-config
 
 A [Ruff](https://docs.astral.sh/ruff) config.
```

