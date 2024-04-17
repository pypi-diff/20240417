# Comparing `tmp/amit_hvac_control-0.3.2.tar.gz` & `tmp/amit_hvac_control-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amit_hvac_control-0.3.2.tar", last modified: Wed Apr  3 18:49:04 2024, max compression
+gzip compressed data, was "amit_hvac_control-0.3.3.tar", last modified: Wed Apr 17 06:54:04 2024, max compression
```

## Comparing `amit_hvac_control-0.3.2.tar` & `amit_hvac_control-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.646937 amit_hvac_control-0.3.2/
--rw-r--r--   0 mitchdries   (501) staff       (20)     1068 2024-03-01 21:43:32.000000 amit_hvac_control-0.3.2/LICENSE
--rw-r--r--   0 mitchdries   (501) staff       (20)     1064 2024-04-03 18:49:04.646020 amit_hvac_control-0.3.2/PKG-INFO
--rw-r--r--   0 mitchdries   (501) staff       (20)      610 2024-03-31 07:11:33.000000 amit_hvac_control-0.3.2/README.md
--rw-r--r--   0 mitchdries   (501) staff       (20)      528 2024-04-03 18:41:33.000000 amit_hvac_control-0.3.2/pyproject.toml
--rw-r--r--   0 mitchdries   (501) staff       (20)       38 2024-04-03 18:49:04.647515 amit_hvac_control-0.3.2/setup.cfg
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.635863 amit_hvac_control-0.3.2/src/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:01.000000 amit_hvac_control-0.3.2/src/__init__.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.637381 amit_hvac_control-0.3.2/src/amit_hvac_control/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/__init__.py
--rw-r--r--   0 mitchdries   (501) staff       (20)      909 2024-04-03 18:42:39.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/__main__.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.643958 amit_hvac_control-0.3.2/src/amit_hvac_control/api/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:06.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/__init__.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2610 2024-04-03 18:48:32.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/status.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2806 2024-03-25 18:28:25.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/temperature.py
--rw-r--r--   0 mitchdries   (501) staff       (20)      377 2024-03-06 20:01:06.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/utils.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     5227 2024-03-29 07:25:54.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/ventilation.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2121 2024-03-22 13:23:38.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/client.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     1307 2024-03-05 11:41:14.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/models.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.644953 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/
--rw-r--r--   0 mitchdries   (501) staff       (20)     1064 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/PKG-INFO
--rw-r--r--   0 mitchdries   (501) staff       (20)      595 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/SOURCES.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)        1 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/dependency_links.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)       29 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/requires.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)       27 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/top_level.txt
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-17 06:54:04.183520 amit_hvac_control-0.3.3/
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1068 2024-03-01 21:43:32.000000 amit_hvac_control-0.3.3/LICENSE
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1071 2024-04-17 06:54:04.182723 amit_hvac_control-0.3.3/PKG-INFO
+-rw-r--r--   0 mitchdries   (501) staff       (20)      610 2024-04-03 18:54:08.000000 amit_hvac_control-0.3.3/README.md
+-rw-r--r--   0 mitchdries   (501) staff       (20)      535 2024-04-17 06:52:27.000000 amit_hvac_control-0.3.3/pyproject.toml
+-rw-r--r--   0 mitchdries   (501) staff       (20)       38 2024-04-17 06:54:04.183704 amit_hvac_control-0.3.3/setup.cfg
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-17 06:54:04.171482 amit_hvac_control-0.3.3/src/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:01.000000 amit_hvac_control-0.3.3/src/__init__.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-17 06:54:04.173099 amit_hvac_control-0.3.3/src/amit_hvac_control/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/__init__.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)      909 2024-04-17 06:52:12.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/__main__.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-17 06:54:04.180896 amit_hvac_control-0.3.3/src/amit_hvac_control/api/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:06.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/api/__init__.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2610 2024-04-03 18:48:32.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/api/status.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2806 2024-03-25 18:28:25.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/api/temperature.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)      329 2024-04-17 06:50:29.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/api/utils.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     5227 2024-03-29 07:25:54.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/api/ventilation.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2121 2024-03-22 13:23:38.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/client.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1307 2024-03-05 11:41:14.000000 amit_hvac_control-0.3.3/src/amit_hvac_control/models.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-17 06:54:04.181807 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1071 2024-04-17 06:54:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/PKG-INFO
+-rw-r--r--   0 mitchdries   (501) staff       (20)      595 2024-04-17 06:54:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/SOURCES.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)        1 2024-04-17 06:54:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/dependency_links.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)       36 2024-04-17 06:54:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/requires.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)       27 2024-04-17 06:54:04.000000 amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/top_level.txt
```

### Comparing `amit_hvac_control-0.3.2/LICENSE` & `amit_hvac_control-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/PKG-INFO` & `amit_hvac_control-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: amit_hvac_control
-Version: 0.3.2
+Version: 0.3.3
 Summary: Amit HVAC control
 Author-email: Mitch Dries <mitch.dries@gmail.com>
 Project-URL: Homepage, https://github.com/mitch3s/amit-hvac-control
 Project-URL: Issues, https://github.com/mitch3s/amit-hvac-control/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: asyncio
-Requires-Dist: aiohttp
+Requires-Dist: aiohttp>=3.9.5
 
 # Amit HVAC Control
 
 Library for controlling Amit HVAC solution using the web server as an interface. It works by scraping the HMI web pages and sending POST requests for save operations.
 
 Only works with the specifically developed machine logic runtime application for the following hardware:
 
 * AMiNi4W2 PLC
 * AMR-OP70RHC/04 Wall-mounted controller
 
 ## Run
 
 Run the main file with arguments to test the connection nd retrieve all data.
 ```bash
-python ./src/amit_hvac_control/__main__.py --host=<internal network address> --username=<username> --password=<password>
+python ./src/amit_hvac_control/__main__.py --host=<internal_network_address> --username=<username> --password=<password>
 ```
 
 ## Build
 
 ```bash
 python -m build
 ```
```

### Comparing `amit_hvac_control-0.3.2/README.md` & `amit_hvac_control-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 * AMiNi4W2 PLC
 * AMR-OP70RHC/04 Wall-mounted controller
 
 ## Run
 
 Run the main file with arguments to test the connection nd retrieve all data.
 ```bash
-python ./src/amit_hvac_control/__main__.py --host=<internal network address> --username=<username> --password=<password>
+python ./src/amit_hvac_control/__main__.py --host=<internal_network_address> --username=<username> --password=<password>
 ```
 
 ## Build
 
 ```bash
 python -m build
 ```
```

### Comparing `amit_hvac_control-0.3.2/pyproject.toml` & `amit_hvac_control-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amit_hvac_control"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Mitch Dries", email="mitch.dries@gmail.com" },
 ]
 description = "Amit HVAC control"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["requests", "bs4", "asyncio", "aiohttp"]
+dependencies = ["requests", "bs4", "asyncio", "aiohttp>=3.9.5"]
 
 [project.urls]
 Homepage = "https://github.com/mitch3s/amit-hvac-control"
 Issues = "https://github.com/mitch3s/amit-hvac-control/issues"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
```

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/__main__.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/__main__.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/api/status.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/api/status.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/api/temperature.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/api/temperature.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/api/ventilation.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/api/ventilation.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/client.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/client.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control/models.py` & `amit_hvac_control-0.3.3/src/amit_hvac_control/models.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/PKG-INFO` & `amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: amit_hvac_control
-Version: 0.3.2
+Version: 0.3.3
 Summary: Amit HVAC control
 Author-email: Mitch Dries <mitch.dries@gmail.com>
 Project-URL: Homepage, https://github.com/mitch3s/amit-hvac-control
 Project-URL: Issues, https://github.com/mitch3s/amit-hvac-control/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: asyncio
-Requires-Dist: aiohttp
+Requires-Dist: aiohttp>=3.9.5
 
 # Amit HVAC Control
 
 Library for controlling Amit HVAC solution using the web server as an interface. It works by scraping the HMI web pages and sending POST requests for save operations.
 
 Only works with the specifically developed machine logic runtime application for the following hardware:
 
 * AMiNi4W2 PLC
 * AMR-OP70RHC/04 Wall-mounted controller
 
 ## Run
 
 Run the main file with arguments to test the connection nd retrieve all data.
 ```bash
-python ./src/amit_hvac_control/__main__.py --host=<internal network address> --username=<username> --password=<password>
+python ./src/amit_hvac_control/__main__.py --host=<internal_network_address> --username=<username> --password=<password>
 ```
 
 ## Build
 
 ```bash
 python -m build
 ```
```

### Comparing `amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/SOURCES.txt` & `amit_hvac_control-0.3.3/src/amit_hvac_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

