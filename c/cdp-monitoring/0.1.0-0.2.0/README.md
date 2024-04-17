# Comparing `tmp/cdp_monitoring-0.1.0.tar.gz` & `tmp/cdp_monitoring-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp_monitoring-0.1.0.tar", max compression
+gzip compressed data, was "cdp_monitoring-0.2.0.tar", max compression
```

## Comparing `cdp_monitoring-0.1.0.tar` & `cdp_monitoring-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      683 2023-12-27 13:15:49.412107 cdp_monitoring-0.1.0/README.md
--rw-r--r--   0        0        0      536 2023-12-27 12:36:30.365489 cdp_monitoring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       76 2023-12-27 12:56:44.065970 cdp_monitoring-0.1.0/src/cdp_monitoring/__init__.py
--rw-r--r--   0        0        0     1654 2023-12-20 10:22:53.072798 cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_metrics.py
--rw-r--r--   0        0        0     5386 2023-12-27 12:55:17.159776 cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_middleware.py
--rw-r--r--   0        0        0     2481 2023-12-27 13:05:36.765177 cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_utils.py
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 cdp_monitoring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-12-27 13:15:49.412107 cdp_monitoring-0.2.0/README.md
+-rw-r--r--   0        0        0      536 2024-04-17 04:20:40.469167 cdp_monitoring-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-12-27 12:56:44.065970 cdp_monitoring-0.2.0/src/cdp_monitoring/__init__.py
+-rw-r--r--   0        0        0     1654 2023-12-20 10:22:53.072798 cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_metrics.py
+-rw-r--r--   0        0        0     5386 2023-12-27 12:55:17.159776 cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_middleware.py
+-rw-r--r--   0        0        0     2481 2023-12-27 13:05:36.765177 cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_utils.py
+-rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 cdp_monitoring-0.2.0/PKG-INFO
```

### Comparing `cdp_monitoring-0.1.0/README.md` & `cdp_monitoring-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cdp_monitoring-0.1.0/pyproject.toml` & `cdp_monitoring-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "cdp-monitoring"
-version = "0.1.0"
+version = "0.2.0"
 description = "cdp monitoring python sdk"
 authors = ["abeti.an <abeti.an@kakaocorp.com>"]
 readme = "README.md"
 packages = [
     { include = "cdp_monitoring", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 opentelemetry-api = "^1.22.0"
 opentelemetry-sdk = "^1.22.0"
 opentelemetry-exporter-otlp = "^1.22.0"
 prometheus-client = "^0.19.0"
 setuptools = "^69.0.3"
-fastapi = "^0.108.0"
+fastapi = "<0.108.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_metrics.py` & `cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_metrics.py`

 * *Files identical despite different names*

### Comparing `cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_middleware.py` & `cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_middleware.py`

 * *Files identical despite different names*

### Comparing `cdp_monitoring-0.1.0/src/cdp_monitoring/monitoring_utils.py` & `cdp_monitoring-0.2.0/src/cdp_monitoring/monitoring_utils.py`

 * *Files identical despite different names*

### Comparing `cdp_monitoring-0.1.0/PKG-INFO` & `cdp_monitoring-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cdp-monitoring
-Version: 0.1.0
+Version: 0.2.0
 Summary: cdp monitoring python sdk
 Author: abeti.an
 Author-email: abeti.an@kakaocorp.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fastapi (>=0.108.0,<0.109.0)
+Requires-Dist: fastapi (<0.108.0)
 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.22.0,<2.0.0)
 Requires-Dist: prometheus-client (>=0.19.0,<0.20.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Description-Content-Type: text/markdown
```

