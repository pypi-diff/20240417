# Comparing `tmp/prometheus-pve-exporter-3.2.4.tar.gz` & `tmp/prometheus_pve_exporter-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-pve-exporter-3.2.4.tar", last modified: Fri Apr 12 07:45:30 2024, max compression
+gzip compressed data, was "prometheus_pve_exporter-3.2.5.tar", last modified: Wed Apr 17 05:14:14 2024, max compression
```

## Comparing `prometheus-pve-exporter-3.2.4.tar` & `prometheus_pve_exporter-3.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/container-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/container-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pve.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pylintrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.142176 prometheus-pve-exporter-3.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/container-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pylintrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.189552 prometheus_pve_exporter-3.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/http.py
```

### Comparing `prometheus-pve-exporter-3.2.4/.github/workflows/ci.yml` & `prometheus_pve_exporter-3.2.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/.github/workflows/container-image.yml` & `prometheus_pve_exporter-3.2.5/.github/workflows/container-image.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/.github/workflows/container-test.yml` & `prometheus_pve_exporter-3.2.5/.github/workflows/container-test.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/.github/workflows/pypi.yml` & `prometheus_pve_exporter-3.2.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/CHANGELOG.rst` & `prometheus_pve_exporter-3.2.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
 
+`3.2.5`_ - 2024-04-17
+---------------------
+
+Changed
+~~~~~~~
+
+- Bump gunicorn from 21.2.0 to 22.0.0 (#241)
+
+
 `3.2.4`_ - 2024-04-12
 ---------------------
 
 Changed
 ~~~~~~~
 
 - Bump idna from 3.6 to 3.7 (#239)
@@ -376,15 +385,16 @@
 ~~~~~
 
 -  IPv6 support
 
 
 .. _Keep a Changelog: http://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: http://semver.org/spec/v2.0.0.html
-.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...HEAD
+.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...HEAD
+.. _3.2.5: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...v3.2.4
 .. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.3
 .. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.2
 .. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.1
 .. _3.2.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.0
 .. _3.2.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.0...v3.1.0
 .. _3.1.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.1.0...v3.0.2
 .. _3.0.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.2...v3.0.1
```

### Comparing `prometheus-pve-exporter-3.2.4/Dockerfile` & `prometheus_pve_exporter-3.2.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/LICENSE` & `prometheus_pve_exporter-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/PKG-INFO` & `prometheus_pve_exporter-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.4
+Version: 3.2.5
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus-pve-exporter-3.2.4/README.rst` & `prometheus_pve_exporter-3.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/pylintrc.toml` & `prometheus_pve_exporter-3.2.5/pylintrc.toml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/pyproject.toml` & `prometheus_pve_exporter-3.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus-pve-exporter"
-version = "3.2.4"
+version = "3.2.5"
 authors = [{ name = "Lorenz Schori", email = "lo@znerol.ch" }]
 description = "Proxmox VE exporter for the Prometheus monitoring system."
 requires-python = ">=3.9"
 keywords = ["prometheus", "exporter", "network", "monitoring", "proxmox"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `prometheus-pve-exporter-3.2.4/requirements.txt` & `prometheus_pve_exporter-3.2.5/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,17 @@
     --hash=sha256:e09469a2cec88fb7b078e16d4adec594414397e8879a4341c6ace96013463d5b \
     --hash=sha256:e53dc41cda40b248ebc40b83b31516487f7db95ab8ceac1f042626bc43a2f992 \
     --hash=sha256:f1e85a178384bf19e36779d91ff35c7617c885da487d689b05c1366f9933ad74 \
     --hash=sha256:f47be41843200f7faec0683ad751e5ef11b9a56a220d57f300376cd8aba81660 \
     --hash=sha256:fb0cef872d8193e487fc6bdb08559c3aa41b659a7d9be48b2e10747f47863925 \
     --hash=sha256:ffc73996c4fca3d2b6c1c8c12bfd3ad00def8621da24f547626bf06441400449
     # via paramiko
-gunicorn==21.2.0 \
-    --hash=sha256:3213aa5e8c24949e792bcacfc176fef362e7aac80b76c56f6b5122bf350722f0 \
-    --hash=sha256:88ec8bff1d634f98e61b9f65bc4bf3cd918a90806c6f5c48bc5603849ec81033
+gunicorn==22.0.0 \
+    --hash=sha256:350679f91b24062c86e386e198a15438d53a7a8207235a78ba1b53df4c4378d9 \
+    --hash=sha256:4a0b436239ff76fb33f11c07a16482c521a7e09c1ce3cc293c2330afe01bec63
     # via -r requirements.in
 idna==3.7 \
     --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
     --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 markupsafe==2.1.3 \
     --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
```

### Comparing `prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.4
+Version: 3.2.5
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/SOURCES.txt` & `prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/cli.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/__init__.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/cluster.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/cluster.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/node.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/node.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/config.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.4/src/pve_exporter/http.py` & `prometheus_pve_exporter-3.2.5/src/pve_exporter/http.py`

 * *Files identical despite different names*

