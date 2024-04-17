# Comparing `tmp/shipyard_motherduck-0.1.0a1.tar.gz` & `tmp/shipyard_motherduck-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_motherduck-0.1.0a1.tar", max compression
+gzip compressed data, was "shipyard_motherduck-0.1.0a2.tar", max compression
```

## Comparing `shipyard_motherduck-0.1.0a1.tar` & `shipyard_motherduck-0.1.0a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-11 02:41:42.600015 shipyard_motherduck-0.1.0a1/README.md
--rw-r--r--   0        0        0      618 2024-04-17 01:40:06.034682 shipyard_motherduck-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-11 13:59:39.563880 shipyard_motherduck-0.1.0a1/shipyard_motherduck/__init__.py
--rw-r--r--   0        0        0      547 2024-04-17 00:40:23.894354 shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/authtest.py
--rw-r--r--   0        0        0     1003 2024-04-17 01:39:58.119732 shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/execute.py
--rw-r--r--   0        0        0     1880 2024-04-17 01:39:58.136436 shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/fetch.py
--rw-r--r--   0        0        0     2817 2024-04-17 00:40:23.938301 shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/upload.py
--rw-r--r--   0        0        0      865 2024-04-17 00:40:23.907409 shipyard_motherduck-0.1.0a1/shipyard_motherduck/errors.py
--rw-r--r--   0        0        0     6433 2024-04-17 00:40:23.959410 shipyard_motherduck-0.1.0a1/shipyard_motherduck/motherduck.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 02:41:42.600015 shipyard_motherduck-0.1.0a2/README.md
+-rw-r--r--   0        0        0      618 2024-04-17 01:51:07.343057 shipyard_motherduck-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-11 13:59:39.563880 shipyard_motherduck-0.1.0a2/shipyard_motherduck/__init__.py
+-rw-r--r--   0        0        0      547 2024-04-17 00:40:23.894354 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/authtest.py
+-rw-r--r--   0        0        0     1090 2024-04-17 01:50:41.897777 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/execute.py
+-rw-r--r--   0        0        0     1880 2024-04-17 01:39:58.136436 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/fetch.py
+-rw-r--r--   0        0        0     2817 2024-04-17 00:40:23.938301 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/upload.py
+-rw-r--r--   0        0        0      865 2024-04-17 00:40:23.907409 shipyard_motherduck-0.1.0a2/shipyard_motherduck/errors.py
+-rw-r--r--   0        0        0     6433 2024-04-17 00:40:23.959410 shipyard_motherduck-0.1.0a2/shipyard_motherduck/motherduck.py
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.0a2/PKG-INFO
```

### Comparing `shipyard_motherduck-0.1.0a1/pyproject.toml` & `shipyard_motherduck-0.1.0a2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-motherduck"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "A local client for working with Python and MotherDuck"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.2"
```

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/authtest.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/execute.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/execute.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,17 @@
     parser.add_argument("--database", required=False, dest="database", default="")
     return parser.parse_args()
 
 
 def main():
     try:
         args = get_args()
-        client = MotherDuckClient(args.token)
         query = args.query
+        database = args.database if args.database != "" else None
+        client = MotherDuckClient(args.token, database = database)
         client.execute_query(query)
 
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(
```

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/fetch.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/cli/upload.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/errors.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/errors.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a1/shipyard_motherduck/motherduck.py` & `shipyard_motherduck-0.1.0a2/shipyard_motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a1/PKG-INFO` & `shipyard_motherduck-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-motherduck
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A local client for working with Python and MotherDuck
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

