# Comparing `tmp/tyjuliacall-0.7.3.tar.gz` & `tmp/tyjuliacall-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyjuliacall-0.7.3.tar", max compression
+gzip compressed data, was "tyjuliacall-0.7.4.tar", max compression
```

## Comparing `tyjuliacall-0.7.3.tar` & `tyjuliacall-0.7.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1123 2024-04-12 02:27:39.100720 tyjuliacall-0.7.3/LICENSE
--rw-r--r--   0        0        0      499 2024-04-12 03:31:40.491352 tyjuliacall-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4302 2024-04-12 02:27:39.101720 tyjuliacall-0.7.3/README.md
--rw-r--r--   0        0        0      172 2024-04-12 02:27:39.102720 tyjuliacall-0.7.3/tyjuliacall/__init__.py
--rw-r--r--   0        0        0    11608 2024-04-12 02:27:39.103720 tyjuliacall-0.7.3/tyjuliasetup/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-12 02:27:39.103720 tyjuliacall-0.7.3/tyjuliasetup/compat.py
--rw-r--r--   0        0        0    16175 2024-04-12 03:31:23.911075 tyjuliacall-0.7.3/tyjuliasetup/julia_src_binding.py
--rw-r--r--   0        0        0     5207 2024-04-12 02:27:39.104721 tyjuliacall-0.7.3/tyjuliasetup/jv.py
--rw-r--r--   0        0        0       84 2024-04-12 02:27:39.102720 tyjuliacall-0.7.3/tyjuliasetup/Project.toml
--rw-r--r--   0        0        0    16077 2024-04-12 03:31:23.911075 tyjuliacall-0.7.3/tyjuliasetup/src/TyJuliaSetup.jl
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 tyjuliacall-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-02-05 10:06:04.251992 tyjuliacall-0.7.4/LICENSE
+-rw-r--r--   0        0        0      499 2024-04-17 07:17:38.573313 tyjuliacall-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4302 2024-02-05 10:06:04.252990 tyjuliacall-0.7.4/README.md
+-rw-r--r--   0        0        0      919 2024-04-17 07:17:38.574304 tyjuliacall-0.7.4/tyjuliacall/__init__.py
+-rw-r--r--   0        0        0    11608 2024-04-17 06:14:39.223014 tyjuliacall-0.7.4/tyjuliasetup/__init__.py
+-rw-r--r--   0        0        0     1291 2024-02-05 10:06:04.254991 tyjuliacall-0.7.4/tyjuliasetup/compat.py
+-rw-r--r--   0        0        0    16175 2024-04-17 06:14:39.228015 tyjuliacall-0.7.4/tyjuliasetup/julia_src_binding.py
+-rw-r--r--   0        0        0     5207 2024-02-05 10:06:04.254991 tyjuliacall-0.7.4/tyjuliasetup/jv.py
+-rw-r--r--   0        0        0       84 2024-02-05 10:06:04.253991 tyjuliacall-0.7.4/tyjuliasetup/Project.toml
+-rw-r--r--   0        0        0    16077 2024-04-17 06:14:39.233014 tyjuliacall-0.7.4/tyjuliasetup/src/TyJuliaSetup.jl
+-rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 tyjuliacall-0.7.4/PKG-INFO
```

### Comparing `tyjuliacall-0.7.3/LICENSE` & `tyjuliacall-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/README.md` & `tyjuliacall-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/tyjuliasetup/__init__.py` & `tyjuliacall-0.7.4/tyjuliasetup/__init__.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/tyjuliasetup/compat.py` & `tyjuliacall-0.7.4/tyjuliasetup/compat.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/tyjuliasetup/julia_src_binding.py` & `tyjuliacall-0.7.4/tyjuliasetup/julia_src_binding.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/tyjuliasetup/jv.py` & `tyjuliacall-0.7.4/tyjuliasetup/jv.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/tyjuliasetup/src/TyJuliaSetup.jl` & `tyjuliacall-0.7.4/tyjuliasetup/src/TyJuliaSetup.jl`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.3/PKG-INFO` & `tyjuliacall-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyjuliacall
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python-Julia interops.
 Author: Suzhou-Tongyuan
 Author-email: support@tongyuan.cc
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

