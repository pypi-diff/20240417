# Comparing `tmp/netsome-0.3.2.tar.gz` & `tmp/netsome-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.2.tar", max compression
+gzip compressed data, was "netsome-0.3.3.tar", max compression
```

## Comparing `netsome-0.3.2.tar` & `netsome-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,17 @@
--rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.2/LICENSE
--rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.2/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.2/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      967 2024-04-15 07:10:54.993891 netsome-0.3.2/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      343 2024-04-15 07:10:54.994197 netsome-0.3.2/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0      662 2024-04-15 18:22:42.950755 netsome-0.3.2/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.821874 netsome-0.3.2/netsome/pools/__init__.py
--rw-r--r--   0        0        0      125 2024-04-11 18:59:46.822131 netsome-0.3.2/netsome/pools/bgp.py
--rw-r--r--   0        0        0     1027 2024-04-16 07:37:52.154983 netsome-0.3.2/netsome/pools/ipv4.py
--rw-r--r--   0        0        0     1409 2024-04-11 18:59:46.822516 netsome-0.3.2/netsome/pools/number.py
--rw-r--r--   0        0        0      130 2024-04-11 18:59:46.822953 netsome-0.3.2/netsome/pools/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.2/netsome/types/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-15 07:10:54.995099 netsome-0.3.2/netsome/types/bgp.py
--rw-r--r--   0        0        0     4510 2024-04-15 07:10:55.013884 netsome-0.3.2/netsome/types/ipv4.py
--rw-r--r--   0        0        0      906 2024-04-15 07:10:55.014565 netsome-0.3.2/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.2/netsome/validators/__init__.py
--rw-r--r--   0        0        0     2022 2024-04-15 18:35:57.465187 netsome-0.3.2/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2112 2024-04-15 19:18:19.904520 netsome-0.3.2/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      381 2024-04-15 07:10:55.016488 netsome-0.3.2/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1262 2024-04-16 07:37:58.242228 netsome-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 netsome-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.3/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.3/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.3/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-15 07:10:54.993891 netsome-0.3.3/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-15 07:10:54.994197 netsome-0.3.3/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0      662 2024-04-15 18:22:42.950755 netsome-0.3.3/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.3/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-15 07:10:54.995099 netsome-0.3.3/netsome/types/bgp.py
+-rw-r--r--   0        0        0     4510 2024-04-15 07:10:55.013884 netsome-0.3.3/netsome/types/ipv4.py
+-rw-r--r--   0        0        0      906 2024-04-15 07:10:55.014565 netsome-0.3.3/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.3/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2022 2024-04-15 18:35:57.465187 netsome-0.3.3/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-15 19:18:19.904520 netsome-0.3.3/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      381 2024-04-15 07:10:55.016488 netsome-0.3.3/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1234 2024-04-17 18:11:35.677357 netsome-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.3/PKG-INFO
```

### Comparing `netsome-0.3.2/LICENSE` & `netsome-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/_converters/bgp.py` & `netsome-0.3.3/netsome/_converters/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/constants.py` & `netsome-0.3.3/netsome/constants.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/types/bgp.py` & `netsome-0.3.3/netsome/types/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/types/ipv4.py` & `netsome-0.3.3/netsome/types/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/types/vlans.py` & `netsome-0.3.3/netsome/types/vlans.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/validators/bgp.py` & `netsome-0.3.3/netsome/validators/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/netsome/validators/ipv4.py` & `netsome-0.3.3/netsome/validators/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.2/pyproject.toml` & `netsome-0.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.2"
+version = "0.3.3"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sortedcontainers = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.3.5"
 toml-sort = "^0.23.1"
```

### Comparing `netsome-0.3.2/PKG-INFO` & `netsome-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.2
+Version: 0.3.3
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,14 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
-Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/kuderr/netsome/issues
 Project-URL: Repository, https://github.com/kuderr/netsome
 Description-Content-Type: text/markdown
 
 # netsome
 
 # About
```

