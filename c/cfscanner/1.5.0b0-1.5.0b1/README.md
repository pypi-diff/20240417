# Comparing `tmp/cfscanner-1.5.0b0.tar.gz` & `tmp/cfscanner-1.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfscanner-1.5.0b0.tar", last modified: Mon Jan 29 22:31:10 2024, max compression
+gzip compressed data, was "cfscanner-1.5.0b1.tar", last modified: Mon Jan 29 22:54:08 2024, max compression
```

## Comparing `cfscanner-1.5.0b0.tar` & `cfscanner-1.5.0b1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/
--rw-rw-r--   0 smz       (1000) smz       (1000)      100 2024-01-29 22:07:20.000000 cfscanner-1.5.0b0/.gitignore
--rw-rw-r--   0 smz       (1000) smz       (1000)    35149 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/LICENSE
--rw-r--r--   0 smz       (1000) smz       (1000)    10560 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/PKG-INFO
--rw-rw-r--   0 smz       (1000) smz       (1000)     9748 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/README.md
--rw-rw-r--   0 smz       (1000) smz       (1000)     1062 2024-01-29 22:27:23.000000 cfscanner-1.5.0b0/pyproject.toml
--rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/setup.cfg
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.423513 cfscanner-1.5.0b0/src/
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.423513 cfscanner-1.5.0b0/src/cfscanner/
--rw-rw-r--   0 smz       (1000) smz       (1000)       61 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)       58 2024-01-29 19:41:21.000000 cfscanner-1.5.0b0/src/cfscanner/__main__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      413 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner/_version.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.423513 cfscanner-1.5.0b0/src/cfscanner/args/
--rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/args/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     9339 2024-01-29 21:54:42.000000 cfscanner-1.5.0b0/src/cfscanner/args/parser.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     4254 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/args/testconfig.py
--rw-rw-r--   0 smz       (1000) smz       (1000)    12842 2024-01-29 22:00:08.000000 cfscanner-1.5.0b0/src/cfscanner/main.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.423513 cfscanner-1.5.0b0/src/cfscanner/report/
--rw-rw-r--   0 smz       (1000) smz       (1000)       27 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/report/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      164 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/report/colors.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      612 2024-01-29 22:02:25.000000 cfscanner-1.5.0b0/src/cfscanner/report/logging_setup.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     5356 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/report/print.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      763 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/report/result.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/src/cfscanner/speedtest/
--rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     7578 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/conduct.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1101 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/download.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     3694 2024-01-29 21:56:40.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/fronting.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1366 2024-01-29 22:03:32.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/tools.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1011 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/speedtest/upload.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/src/cfscanner/subnets/
--rw-rw-r--   0 smz       (1000) smz       (1000)      108 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/subnets/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     5490 2024-01-29 21:01:07.000000 cfscanner-1.5.0b0/src/cfscanner/subnets/cidr.py
--rw-rw-r--   0 smz       (1000) smz       (1000)       50 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/subnets/regex.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/src/cfscanner/utils/
--rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1078 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/decorators.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      617 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/exceptions.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     2876 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/os.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1763 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/random.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      992 2024-01-29 21:55:05.000000 cfscanner-1.5.0b0/src/cfscanner/utils/requests.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1159 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/utils/socket.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/src/cfscanner/xray/
--rw-rw-r--   0 smz       (1000) smz       (1000)      564 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/xray/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     3466 2024-01-29 22:15:32.000000 cfscanner-1.5.0b0/src/cfscanner/xray/binary.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1604 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/xray/config.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1346 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/xray/service.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     1051 2024-01-28 17:46:06.000000 cfscanner-1.5.0b0/src/cfscanner/xray/templates.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:31:10.427513 cfscanner-1.5.0b0/src/cfscanner.egg-info/
--rw-r--r--   0 smz       (1000) smz       (1000)    10560 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/PKG-INFO
--rw-rw-r--   0 smz       (1000) smz       (1000)     1297 2024-01-29 22:31:10.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/SOURCES.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/dependency_links.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       45 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/entry_points.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       76 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/requires.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-01-29 22:31:09.000000 cfscanner-1.5.0b0/src/cfscanner.egg-info/top_level.txt
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.857708 cfscanner-1.5.0b1/
+-rw-rw-r--   0 smz       (1000) smz       (1000)      100 2024-01-29 22:07:20.000000 cfscanner-1.5.0b1/.gitignore
+-rw-rw-r--   0 smz       (1000) smz       (1000)    35149 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/LICENSE
+-rw-r--r--   0 smz       (1000) smz       (1000)    10560 2024-01-29 22:54:08.857708 cfscanner-1.5.0b1/PKG-INFO
+-rw-rw-r--   0 smz       (1000) smz       (1000)     9748 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/README.md
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1062 2024-01-29 22:27:23.000000 cfscanner-1.5.0b1/pyproject.toml
+-rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-01-29 22:54:08.857708 cfscanner-1.5.0b1/setup.cfg
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       61 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)       58 2024-01-29 19:41:21.000000 cfscanner-1.5.0b1/src/cfscanner/__main__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      413 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner/_version.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/args/
+-rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/args/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     9339 2024-01-29 21:54:42.000000 cfscanner-1.5.0b1/src/cfscanner/args/parser.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     4254 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/args/testconfig.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)    13498 2024-01-29 22:50:31.000000 cfscanner-1.5.0b1/src/cfscanner/main.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/report/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       27 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/report/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      164 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/report/colors.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      611 2024-01-29 22:51:32.000000 cfscanner-1.5.0b1/src/cfscanner/report/logging_setup.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     5356 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/report/print.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      763 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/report/result.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/speedtest/
+-rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     7578 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/conduct.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1101 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/download.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     3864 2024-01-29 22:44:06.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/fronting.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1315 2024-01-29 22:51:14.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/tools.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1007 2024-01-29 22:45:20.000000 cfscanner-1.5.0b1/src/cfscanner/speedtest/upload.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/subnets/
+-rw-rw-r--   0 smz       (1000) smz       (1000)      108 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/subnets/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     5490 2024-01-29 21:01:07.000000 cfscanner-1.5.0b1/src/cfscanner/subnets/cidr.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)       50 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/subnets/regex.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.853708 cfscanner-1.5.0b1/src/cfscanner/utils/
+-rw-rw-r--   0 smz       (1000) smz       (1000)        0 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1078 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/decorators.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      617 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/exceptions.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     2876 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/os.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1763 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/random.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      992 2024-01-29 21:55:05.000000 cfscanner-1.5.0b1/src/cfscanner/utils/requests.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1159 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/utils/socket.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.857708 cfscanner-1.5.0b1/src/cfscanner/xray/
+-rw-rw-r--   0 smz       (1000) smz       (1000)      564 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/xray/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     3466 2024-01-29 22:15:32.000000 cfscanner-1.5.0b1/src/cfscanner/xray/binary.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1604 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/xray/config.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1346 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/xray/service.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1051 2024-01-28 17:46:06.000000 cfscanner-1.5.0b1/src/cfscanner/xray/templates.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-01-29 22:54:08.857708 cfscanner-1.5.0b1/src/cfscanner.egg-info/
+-rw-r--r--   0 smz       (1000) smz       (1000)    10560 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/PKG-INFO
+-rw-rw-r--   0 smz       (1000) smz       (1000)     1297 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       45 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/entry_points.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       76 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/requires.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-01-29 22:54:08.000000 cfscanner-1.5.0b1/src/cfscanner.egg-info/top_level.txt
```

### Comparing `cfscanner-1.5.0b0/LICENSE` & `cfscanner-1.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/PKG-INFO` & `cfscanner-1.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.5.0b0
+Version: 1.5.0b1
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cfscanner-1.5.0b0/README.md` & `cfscanner-1.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/pyproject.toml` & `cfscanner-1.5.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/args/parser.py` & `cfscanner-1.5.0b1/src/cfscanner/args/parser.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/args/testconfig.py` & `cfscanner-1.5.0b1/src/cfscanner/args/testconfig.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/main.py` & `cfscanner-1.5.0b1/src/cfscanner/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,31 +76,46 @@
                 logger.exception("Could not create config directory")
                 exit(1)
         console.log(
             f'[bright_blue]Config directory created "{CONFIGDIR}"[/bright_blue]'
         )
 
     # check if blocked
-    if not args.no_vpn and args.fronting_domain:
-        with console.status(
-            f"[green]Checking if fronting domain is blocked[/green]"
-        ):
-            if is_blocked(args.fronting_domain):
-                console.log("Trying direct fronting test")
+    if not args.no_vpn:
+        if args.fronting_domain:
+            with console.status(
+                "[green]Checking if fronting domain is blocked[/green]"
+            ):
+                if is_blocked(args.fronting_domain):
+                    console.log("Trying direct fronting test")
+                    if is_blocked("speed.cloudflare.com"):
+                        console.log(
+                            "[red1]Fronting domain and direct fronting test "
+                            "are blocked[/red1]"
+                        )
+                        console.log(
+                            "Consider using another cname or pass "
+                            "--no-fronting to skip fronting test"
+                        )
+                        console.log("Exiting...")
+                        exit(1)
+                    else:
+                        args.fronting_domain = None
+        else:
+            with console.status(
+                "[green]Checking if speed.cloudflare.com is blocked[/green]"
+            ):
                 if is_blocked("speed.cloudflare.com"):
+                    console.log("[red1]speed.cloudflare.com is blocked[/red1]")
                     console.log(
-                        "[red1]Fronting domain and direct fronting test are blocked[/red1]"
-                    )
-                    console.log(
-                        "Consider using another cname or pass --no-fronting to skip fronting test"
+                        "Consider using a cname or pass --no-fronting to skip "
+                        "fronting test"
                     )
                     console.log("Exiting...")
                     exit(1)
-                else:
-                    args.fronting_domain = None
 
     with console.status(
         f'[green]Creating results directory "{RESULTDIR}"[/green]'
     ):
         try:
             create_dir(RESULTDIR)
         except Exception as e:
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner/report/logging_setup.py` & `cfscanner-1.5.0b1/src/cfscanner/report/logging_setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 START_DT_STR = datetime.now().strftime(r"%Y%m%d_%H%M%S")
 INTERIM_RESULTS_PATH = os.path.join(RESULTDIR, f"{START_DT_STR}_result.csv")
 CWD = pathlib.Path(os.getcwd())
 
 console = Console()
 fancylogging.setup_fancy_logging(
     "cfscanner",
-    console_log_level=logging.DEBUG,
+    console_log_level=logging.INFO,
     file_log_level=logging.DEBUG,
     file_log_path=CWD / "log" / f"{START_DT_STR}.jsonl",
     console=console,
 )
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner/report/print.py` & `cfscanner-1.5.0b1/src/cfscanner/report/print.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/report/result.py` & `cfscanner-1.5.0b1/src/cfscanner/report/result.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/speedtest/conduct.py` & `cfscanner-1.5.0b1/src/cfscanner/speedtest/conduct.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/speedtest/download.py` & `cfscanner-1.5.0b1/src/cfscanner/speedtest/download.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/speedtest/fronting.py` & `cfscanner-1.5.0b1/src/cfscanner/speedtest/fronting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import re
 
 import requests
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 def fronting_test(ip: str, timeout: float, fronting_domain=None) -> bool:
     if not fronting_domain:
+        logger.debug(f"Testing {ip} with direct fronting")
         return fronting_test_direct(ip, timeout)
     else:
+        logger.debug(f"Testing {ip} with cname fronting")
         return fronting_test_cname(ip, timeout, fronting_domain)
 
 
 def fronting_test_cname(ip: str, timeout: float, fronting_domain=None) -> bool:
     """conducts a fronting test on an ip and return true if ok
 
     Args:
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner/speedtest/tools.py` & `cfscanner-1.5.0b1/src/cfscanner/speedtest/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import socket
 import statistics
-from ipaddress import IPv4Address, IPv6Address, ip_address
-from typing import Union
+from ipaddress import ip_address
 
 logger = logging.getLogger(__name__)
 
 
 def mean_jitter(latencies: list) -> float:
     """calculates the mean jitter of a list of latencies
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner/speedtest/upload.py` & `cfscanner-1.5.0b1/src/cfscanner/speedtest/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
     timeout: int,
 ) -> Tuple[float, float]:
     """tests the upload speed using cloudflare servers
 
     Args:
         n_bytes (int): size of file to upload in bytes
         proxies (dict): the proxies to use for ``requests.post``
-        timeout (int): the timeout for the download ``requests.post``   
+        timeout (int): the timeout for the download ``requests.post``
 
     Returns:
         upload_speed (float): the upload speed in mbps
-        latency (float): the rount trip time latency in seconds
+        latency (float): the round trip time latency in seconds
     """
 
     start_time = time.perf_counter()
     r = requests.post(
         url="https://speed.cloudflare.com/__up",
         data="0" * n_bytes,
         timeout=timeout,
-        proxies=proxies
+        proxies=proxies,
     )
     total_time = time.perf_counter() - start_time
     cf_time = float(r.headers.get("Server-Timing").split("=")[1]) / 1000
     latency = total_time - cf_time
 
-    mb = n_bytes * 8 / (10 ** 6)
+    mb = n_bytes * 8 / (10**6)
     upload_speed = mb / cf_time
 
     return upload_speed, latency
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner/subnets/cidr.py` & `cfscanner-1.5.0b1/src/cfscanner/subnets/cidr.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/decorators.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/exceptions.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/os.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/os.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/random.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/random.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/requests.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/requests.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/utils/socket.py` & `cfscanner-1.5.0b1/src/cfscanner/utils/socket.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/xray/__init__.py` & `cfscanner-1.5.0b1/src/cfscanner/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/xray/binary.py` & `cfscanner-1.5.0b1/src/cfscanner/xray/binary.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/xray/config.py` & `cfscanner-1.5.0b1/src/cfscanner/xray/config.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/xray/service.py` & `cfscanner-1.5.0b1/src/cfscanner/xray/service.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner/xray/templates.py` & `cfscanner-1.5.0b1/src/cfscanner/xray/templates.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.5.0b0/src/cfscanner.egg-info/PKG-INFO` & `cfscanner-1.5.0b1/src/cfscanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.5.0b0
+Version: 1.5.0b1
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cfscanner-1.5.0b0/src/cfscanner.egg-info/SOURCES.txt` & `cfscanner-1.5.0b1/src/cfscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

