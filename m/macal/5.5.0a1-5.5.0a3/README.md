# Comparing `tmp/macal-5.5.0a1.tar.gz` & `tmp/macal-5.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.5.0a1.tar", last modified: Mon Apr 15 15:30:14 2024, max compression
+gzip compressed data, was "macal-5.5.0a3.tar", last modified: Tue Apr 16 21:59:08 2024, max compression
```

## Comparing `macal-5.5.0a1.tar` & `macal-5.5.0a3.tar`

### file list

```diff
@@ -1,49 +1,75 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/
--rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a1/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1878 2024-04-15 15:30:14.522592 macal-5.5.0a1/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     1228 2024-04-08 15:14:58.000000 macal-5.5.0a1/README.md
--rw-r--r--   0 marco     (1000) marco     (1000)      848 2024-04-04 14:03:06.000000 macal-5.5.0a1/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-15 15:30:14.522592 macal-5.5.0a1/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-07 01:56:29.000000 macal-5.5.0a1/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a1/src/macal/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/frontend/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a1/src/macal/frontend/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/frontend/ast/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a1/src/macal/frontend/ast/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a1/src/macal/frontend/ast/kind.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a1/src/macal/frontend/ast/metadata.py
--rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a1/src/macal/frontend/ast/node.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a1/src/macal/frontend/ast/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a1/src/macal/frontend/mlexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    49158 2024-04-15 14:43:00.000000 macal-5.5.0a1/src/macal/frontend/mparser.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4851 2024-04-09 09:41:36.000000 macal-5.5.0a1/src/macal/frontend/mparserstate.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a1/src/macal/frontend/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     5713 2024-04-10 21:36:36.000000 macal-5.5.0a1/src/macal/macal.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a1/src/macal/mexceptions.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3570 2024-04-10 14:47:02.000000 macal-5.5.0a1/src/macal/mrepl.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7519 2024-04-15 14:32:17.000000 macal-5.5.0a1/src/macal/mrun.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a1/src/macal/py.typed
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/runtime/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a1/src/macal/runtime/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/runtime/library/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a1/src/macal/runtime/library/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a1/src/macal/runtime/library/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a1/src/macal/runtime/library/system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a1/src/macal/runtime/library/time.py
--rw-r--r--   0 marco     (1000) marco     (1000)     8922 2024-04-09 13:03:11.000000 macal-5.5.0a1/src/macal/runtime/menvironment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a1/src/macal/runtime/mimporter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    77580 2024-04-15 14:47:24.000000 macal-5.5.0a1/src/macal/runtime/minterpreter.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a1/src/macal/runtime/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a1/src/macal/runtime/value_type.py
--rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a1/src/macal/runtime/values.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     1878 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     1071 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      117 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a1/tests/test.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/.vscode/
+-rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a3/.vscode/launch.json
+-rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a3/.vscode/settings.json
+-rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a3/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a3/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-16 21:59:08.076301 macal-5.5.0a3/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     4551 2024-04-16 13:27:36.000000 macal-5.5.0a3/README.md
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/documentation/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a3/documentation/history.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1016 2024-04-16 21:58:56.000000 macal-5.5.0a3/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-16 21:59:08.076301 macal-5.5.0a3/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-15 16:33:22.000000 macal-5.5.0a3/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a3/src/macal/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/frontend/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a3/src/macal/frontend/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/frontend/ast/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a3/src/macal/frontend/ast/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a3/src/macal/frontend/ast/kind.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a3/src/macal/frontend/ast/metadata.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a3/src/macal/frontend/ast/node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a3/src/macal/frontend/ast/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a3/src/macal/frontend/mlexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a3/src/macal/frontend/mparser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a3/src/macal/frontend/mparserstate.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a3/src/macal/frontend/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     5713 2024-04-10 21:36:36.000000 macal-5.5.0a3/src/macal/macal.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a3/src/macal/mexceptions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    11999 2024-04-16 21:53:55.000000 macal-5.5.0a3/src/macal/mrepl.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a3/src/macal/mrun.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a3/src/macal/py.typed
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/runtime/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a3/src/macal/runtime/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a3/src/macal/runtime/menvironment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a3/src/macal/runtime/mimporter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    77580 2024-04-15 14:47:24.000000 macal-5.5.0a3/src/macal/runtime/minterpreter.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/runtime/native/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a3/src/macal/runtime/native/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a3/src/macal/runtime/native/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a3/src/macal/runtime/native/system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a3/src/macal/runtime/native/time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a3/src/macal/runtime/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a3/src/macal/runtime/value_type.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a3/src/macal/runtime/values.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)      980 2024-04-12 12:31:29.000000 macal-5.5.0a3/tests/agent.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/tests/lib/
+-rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a3/tests/lib/csv.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_csv.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a3/tests/lib/ext_io.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_keyring.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_math.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a3/tests/lib/ext_strings.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_syslog.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a3/tests/lib/ext_system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a3/tests/lib/io.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a3/tests/lib/keyring.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a3/tests/lib/math.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a3/tests/lib/meraki_api_library_v1.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a3/tests/lib/meraki_v1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a3/tests/lib/strings.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a3/tests/lib/syslog.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2929 2024-04-10 19:31:44.000000 macal-5.5.0a3/tests/lib/system.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a3/tests/lib/time.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a3/tests/test.py
```

### Comparing `macal-5.5.0a1/LICENSE.txt` & `macal-5.5.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/pyproject.toml` & `macal-5.5.0a3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macal"
-version = "5.5.0.alpha.1"
+dynamic = ["version"]
 authors = [
   { name="Marco Caspers", email="SamaDevTeam@westcon.com" },
 ]
-description = "Macal is a DSL for collecting and transforming data from various sources."
+description = "Macal DSL is used for collecting and transforming data from various sources."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Development Status :: 3 - Alpha",
+    "Programming Language :: Python :: 3.9",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "unidecode",
     "keyring",
@@ -27,10 +30,11 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Sama-Developer/macal"
 
 [project.scripts]
 mrepl = "macal.mrepl:main"
-mdeco = "macal.mdeco:main"
-mcomp = "macal.mccomp:main"
 mrun = "macal.mrun:main"
+
+[tool.setuptools.dynamic]
+version = {attr = "macal.__about__.__version__"}
```

### Comparing `macal-5.5.0a1/src/macal/__about__.py` & `macal-5.5.0a3/src/macal/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 #
 
-__version__ = "5.5.0.alpha.1"
+__version__ = "5.5.0.alpha.3"
 __author__ = "Marco Caspers"
 __email__ = "samadevteam@westcon.com"
 __copyright__ = "Copyright 2024 Westcon Sama Development Team"
 __license__ = "MIT License"
```

### Comparing `macal-5.5.0a1/src/macal/__init__.py` & `macal-5.5.0a3/src/macal/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/__init__.py` & `macal-5.5.0a3/src/macal/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/ast/__init__.py` & `macal-5.5.0a3/src/macal/frontend/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/ast/kind.py` & `macal-5.5.0a3/src/macal/frontend/ast/kind.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/ast/metadata.py` & `macal-5.5.0a3/src/macal/frontend/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/ast/node.py` & `macal-5.5.0a3/src/macal/frontend/ast/node.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/mlexer.py` & `macal-5.5.0a3/src/macal/frontend/mlexer.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/frontend/mparser.py` & `macal-5.5.0a3/src/macal/frontend/mparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,26 +165,18 @@
     def _eat(self) -> Token:
         self._current += 1
         return self._tokens[self._current - 1]
 
     def _not_eof(self) -> bool:
         return self._at().kind != TokenKind.EOF
 
-    def _get_prev_pos(self) -> Tuple[int, int]:
-        tok = self._at(-1)
-        return tok.line, tok.column
-
     def _get_prev_meta(self) -> NodeMetadata:
         tok = self._at(-1)
         return NodeMetadata(tok.line, tok.column, self._filename)
 
-    def _get_curr_pos(self) -> Tuple[int, int]:
-        tok = self._at()
-        return tok.line, tok.column
-
     def _get_curr_meta(self) -> NodeMetadata:
         tok = self._at()
         return NodeMetadata(tok.line, tok.column, self._filename)
 
     def _get_meta(self, token: Token) -> NodeMetadata:
         return NodeMetadata(token.line, token.column, self._filename)
 
@@ -249,19 +241,19 @@
         if self._at().kind == TokenKind.RETURN:
             if state.is_in_function is False and state.is_function_definition is False:
                 raise SyntaxError("Unexpected 'return'.", self._get_curr_meta())
             return self._parse_return_statement(state)
         if self._at().kind == TokenKind.CONTINUE:
             if state.is_in_loop is False:
                 raise SyntaxError(f"Unexpected 'continue'.", self._get_curr_meta())
-            return self._parse_continue_statement()
+            return self._parse_continue_statement(state)
         if self._at().kind == TokenKind.BREAK:
             if state.is_in_loop is False and state.is_in_switch is False:
                 raise SyntaxError("Unexpected 'break'.", self._get_curr_meta())
-            return self._parse_break_statement()
+            return self._parse_break_statement(state)
         if self._at().kind == TokenKind.HALT:
             return self._parse_halt_statement(state)
         if self._at().kind == TokenKind.IF:
             return self._parse_if_statement(state)
         if self._at().kind == TokenKind.ELSE:
             raise SyntaxError("Parser Error: Unexpected 'else'.", self._get_curr_meta())
         if self._at().kind == TokenKind.ELIF:
@@ -287,15 +279,15 @@
         if self._at().kind == TokenKind.SELECT:
             return self._parse_select_statement(state)
         stmt: IStmt = self._parse_expr(state)
         self._expect(TokenKind.SEMICOLON, "Expected ';' after expression.")
         return stmt
 
     def _parse_function_declaration(self, state: ParserState) -> FunctionDeclaration:
-        identifier: Identifier = self._parse_identifier()
+        identifier: Identifier = self._parse_identifier(state)
         symbol = state.add_symbol(self._at(-1))
         decl_state = state.create_child(
             name=identifier.name, is_function_definition=True
         )
         self._expect(TokenKind.FN, "Function Declaration: Expected '=>' keyword.")
         args: list[IExpr] = self._parse_args(decl_state)
         params: list[str] = []
@@ -350,15 +342,15 @@
                 function_name=fun.lexeme,
             )
         decl.metadata.line = identifier.metadata.line
         decl.metadata.column = identifier.metadata.column
         decl.metadata.filename = self._filename
         return decl
 
-    def _parse_identifier(self) -> Identifier:
+    def _parse_identifier(self, state: ParserState) -> Identifier:
         token = self._expect(TokenKind.IDENTIFIER, "Expected identifier.")
         ident: Identifier = Identifier(token.lexeme, self._get_meta(token))
         return ident
 
     def _parse_return_statement(self, state: ParserState) -> ReturnStatement:
         ret = self._eat()
         if self._at().kind == TokenKind.SEMICOLON:
@@ -367,22 +359,22 @@
             return stmt
         expr: IExpr = self._parse_expr(state)
         self._expect(TokenKind.SEMICOLON, "Expected ';' after return expression.")
         rstmt: ReturnStatement = ReturnStatement(expr)
         self._set_stmt_metadata(rstmt, ret)
         return rstmt
 
-    def _parse_continue_statement(self) -> ContinueStatement:
+    def _parse_continue_statement(self, state: ParserState) -> ContinueStatement:
         cont = self._eat()
         self._expect(TokenKind.SEMICOLON, "Expected ';' after 'continue'.")
         stmt: ContinueStatement = ContinueStatement()
         self._set_stmt_metadata(stmt, cont)
         return stmt
 
-    def _parse_break_statement(self) -> BreakStatement:
+    def _parse_break_statement(self, state: ParserState) -> BreakStatement:
         brk = self._eat()
         self._expect(TokenKind.SEMICOLON, "Expected ';' after 'break'.")
         stmt: BreakStatement = BreakStatement()
         self._set_stmt_metadata(stmt, brk)
         return stmt
 
     def _parse_halt_statement(self, state: ParserState) -> HaltStatement:
@@ -402,15 +394,15 @@
         self, is_const: bool, state: ParserState
     ) -> VarDeclaration:
         if is_const:
             token = self._eat()  # eat 'const'
             meta = token
         else:
             meta = self._at()
-        identifier: Identifier = self._parse_identifier()
+        identifier: Identifier = self._parse_identifier(state)
         symbol_state = state.find_symbol(identifier.name)
         if symbol_state is not None:
             symbol = symbol_state.get_symbol(identifier.name)
             if is_const:
                 if symbol is not None:
                     ameta = self._get_prev_meta()
                     if symbol.is_const:
@@ -442,28 +434,28 @@
             # No value assigned to variable, it'll look weird but it's valid in Macal.
             decl: VarDeclaration = VarDeclaration(
                 identifier, None, False, self._get_meta(meta)
             )
             return decl
         if self._at().kind != TokenKind.ASSIGN:
             raise SyntaxError(
-                f"Variable '{identifier.name}' not found", self._get_curr_meta()
+                f"Variable '{identifier.name}' not found", self._get_prev_meta()
             )
-        eq = self._expect(TokenKind.ASSIGN, "Expected '=' after variable declaration.")
+        eq = self._eat()  # eat '='
         if eq.lexeme != "=":
             raise SyntaxError(
                 f"Expected '=' after variable declaration, got '{eq.lexeme}'.",
-                self._get_prev_meta(),
+                self._get_meta(eq),
             )
         value: IExpr = self._parse_expr(state)
         ch = self._at().lexeme
         if ch != ";":
             if value.kind == NodeKind.EXPR_BINARY:
                 raise SyntaxError(
-                    f"Expected ';' after variable declaration, got '{ch}'. \nPossible premature string termination, or the same termination was used in interpolation.\n",
+                    f"Expected ';' after variable declaration, got '{ch}'. \nPossible premature string termination",
                     self._get_curr_meta(),
                 )
         self._expect(TokenKind.SEMICOLON, "Expected ';' after variable declaration.")
         rdecl: VarDeclaration = VarDeclaration(
             identifier, value, is_const, self._get_meta(meta)
         )
         return rdecl
@@ -613,14 +605,17 @@
             raise SyntaxError(
                 "Expected library identifier after include.", self._get_prev_meta()
             )
         libs: list[LibraryLiteral] = []
         while self._not_eof() and self._at().kind != TokenKind.SEMICOLON:
             ltok = self._expect(TokenKind.IDENTIFIER, "Expected library identifier.")
             lib = LibraryLiteral(ltok.lexeme)
+            glob_state = state.get_global()
+            if not glob_state.find_symbol(ltok.lexeme):
+                glob_state.add_symbol(ltok, is_const=True)
             self._set_expr_metadata(lib, ltok)
             libs.append(lib)
             state.add_symbol(ltok)
             if self._at().kind != TokenKind.SEMICOLON:
                 self._expect(TokenKind.COMMA, "Expected ',' after library identifier.")
         self._expect(TokenKind.SEMICOLON, "Expected ';' after include statement.")
         stmt = IncludeStatement(libs, self._get_meta(tok))
@@ -677,25 +672,18 @@
         stmt = IsTypeStatement(expr, self._get_meta(tok), ttc)
         return stmt
 
     def _parse_assignment_statement(self, state: ParserState) -> IStmt:
         if self._at(1).kind == TokenKind.FN:
             return self._parse_function_declaration(state)
         varname = self._at().lexeme
-        # print()
-        # print(varname)
-        # for symbol in state.symbols:
-        #    print(symbol.name)
-        # print(state.find_symbol(varname) is not None)
         if (
             state.find_symbol(varname) is not None or varname == "it"
         ):  # 'it' is a reserved keyword in Macal, it's used in the foreach statement.
-            # print("b4 expr at: ", self._at().lexeme)
             expr = self._parse_assignment_expr(state)
-            # print("a8 expr at: ", self._at().lexeme)
             self._expect(TokenKind.SEMICOLON, "Expected ';' after assignment.")
             return expr
         vardecl = self._parse_var_declaration(is_const=False, state=state)
         return vardecl
 
     def _parse_select_statement(self, state: ParserState) -> IStmt:
         token = self._expect(TokenKind.SELECT, "Expected 'select' keyword.")
@@ -752,19 +740,22 @@
             into_var_name.lexeme,
             self._get_meta(token),
         )
 
     # ----------------------------------------- Expression Parsing -----------------------------------------
 
     def _parse_expr(self, state: ParserState) -> IExpr:
-        return self._parse_string_concatenation(state)
+        return self._parse_assignment_expr(state)
 
     def _parse_assignment_expr(self, state: ParserState) -> IExpr:
         token = self._at()
         left: IExpr = self._parse_string_concatenation(state)
+        if isinstance(left, Identifier):
+            if state.find_symbol(left.name) is None:
+                state.add_symbol(token)
         if self._at().lexeme in {"=", "+=", "-=", "*=", "/=", "%=", "^=", ".="}:
             op_token = self._eat()
             if left.kind != NodeKind.LIT_IDENT and left.kind != NodeKind.EXPR_MEMBER:
                 raise SyntaxError(
                     "Invalid assignment target (left)",
                     NodeMetadata(token.line, token.column, self._filename),
                 )
@@ -1017,15 +1008,16 @@
                     )
             else:  # this allows obj[computedValue]
                 computed = True
                 if self._at().kind == TokenKind.CLOSE_BRACKET:
                     return self._parse_new_array_element(obj, state)
                 prop = self._parse_expr(state)
                 self._expect(
-                    TokenKind.CLOSE_BRACKET, "Expected ']' after computed property."
+                    TokenKind.CLOSE_BRACKET,
+                    "Expected ']' after computed property.",
                 )
 
             obj = MemberExpr(
                 obj=obj, prop=prop, computed=computed, new_array_element=False
             )
             self._set_expr_metadata(obj, op)
         return obj
@@ -1053,58 +1045,58 @@
             assignee=member, op="=", value=value, metadata=self._get_meta(tobj)
         )
         return asgn
 
     def _parse_primary_expr(self, state: ParserState) -> IExpr:
         token = self._at()
         if token.kind == TokenKind.IDENTIFIER:
-            return self._parse_identifier()
+            return self._parse_identifier(state)
         if token.kind == TokenKind.INTEGER:
-            return self._parse_int_literal()
+            return self._parse_int_literal(state)
         if token.kind == TokenKind.FLOAT:
-            return self._parse_float_literal()
+            return self._parse_float_literal(state)
         if token.kind == TokenKind.STRING:
-            return self._parse_string_literal()
+            return self._parse_string_literal(state)
         if token.kind == TokenKind.OPEN_PAREN:  # (expr)
             self._eat()
             expr: IExpr = self._parse_expr(state)
             self._expect(TokenKind.CLOSE_PAREN, "Expected ')' after expression.")
             return expr
         if token.kind == TokenKind.ARRAY:
             if self._at(1).kind == TokenKind.IDENTIFIER:
                 self._eat()  # eat 'array' because it is used as a type and we don't handle that yet.
-                return self._parse_identifier()
+                return self._parse_identifier(state)
             return self._parse_array_literal(state)
         if token.kind == TokenKind.RECORD:
             if self._at(1).kind == TokenKind.IDENTIFIER:
                 self._eat()  # eat 'record' because it is used as a type and we don't handle that yet.
-                return self._parse_identifier()
+                return self._parse_identifier(state)
             return self._parse_record_literal(state)
         if token.kind == TokenKind.TYPES:
             return self._parse_type_statement(state, as_expr=True)  # type: ignore
         if token.kind == TokenKind.ISTYPE:
             return self._parse_istype_statement(state, as_expr=True)  # type: ignore
         raise SyntaxError(
             f"Unexpected token ({token.lexeme}) in expression.",
             NodeMetadata(token.line, token.column, self._filename),
         )
 
-    def _parse_int_literal(self) -> IntLiteral:
+    def _parse_int_literal(self, state: ParserState) -> IntLiteral:
         token = self._expect(TokenKind.INTEGER, "Expected integer literal.")
         lit: IntLiteral = IntLiteral(int(token.lexeme))
         self._set_expr_metadata(lit, token)
         return lit
 
-    def _parse_float_literal(self) -> FloatLiteral:
+    def _parse_float_literal(self, state: ParserState) -> FloatLiteral:
         token = self._expect(TokenKind.FLOAT, "Expected float literal.")
         lit: FloatLiteral = FloatLiteral(float(token.lexeme))
         self._set_expr_metadata(lit, token)
         return lit
 
-    def _parse_string_literal(self) -> StringLiteral:
+    def _parse_string_literal(self, state: ParserState) -> StringLiteral:
         token = self._expect(TokenKind.STRING, "Expected string literal.")
         lit: StringLiteral = StringLiteral(token.lexeme)
         self._set_expr_metadata(lit, token)
         return lit
 
     def _parse_array_literal(
         self, state: ParserState
```

### Comparing `macal-5.5.0a1/src/macal/frontend/mparserstate.py` & `macal-5.5.0a3/src/macal/frontend/mparserstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 from macal.frontend.ast.metadata import NodeMetadata
 
 
 class ParserSymbol:
     def __init__(
         self, name: str, metadata: NodeMetadata, is_global: bool, is_const: bool = False
     ) -> None:
-        self.name = name
-        self.metadata = metadata
-        self.is_global = is_global
-        self.is_const = is_const
+        self.name: str = name
+        self.metadata: NodeMetadata = metadata
+        self.is_global: bool = is_global
+        self.is_const: bool = is_const
 
     def json(self) -> dict:
         return {
             "name": self.name,
             "metadata": self.metadata.json(),
             "is_global": self.is_global,
             "is_const": self.is_const,
@@ -72,14 +72,19 @@
         self.filename: str = filename
         self.symbols: list[ParserSymbol] = []
         self.is_in_loop: bool = is_in_loop
         self.is_in_function: bool = is_in_function
         self.is_in_switch: bool = is_in_switch
         self.is_function_definition: bool = is_function_definition
 
+    def reset(self):  # reset is used by the repl to reset the symbol table
+        self.symbols = []
+        if self.parent is not None:
+            self.parent.reset()
+
     def is_global(self) -> bool:
         return self.parent is None
 
     def get_global(self) -> ParserState:
         if self.parent is not None:
             return self.parent.get_global()
         return self
```

### Comparing `macal-5.5.0a1/src/macal/macal.py` & `macal-5.5.0a3/src/macal/macal.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/mexceptions.py` & `macal-5.5.0a3/src/macal/mexceptions.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/mrun.py` & `macal-5.5.0a3/src/macal/mrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,14 @@
             sys.exit(1)
         except RuntimeErrorLC as e:
             print(f"{e}")
             sys.exit(1)
         except SyntaxError as e:
             print(f"{e}")
             sys.exit(1)
-        except SyntaxError as e:
-            print(f"{e}")
-            sys.exit(1)
 
 
 def main():
     args = parse_args()
     if args.version:
         print(f"Macal DSL {__version__}")
         sys.exit(0)
```

### Comparing `macal-5.5.0a1/src/macal/runtime/__init__.py` & `macal-5.5.0a3/src/macal/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/library/__init__.py` & `macal-5.5.0a3/src/macal/runtime/native/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/library/system.py` & `macal-5.5.0a3/src/macal/runtime/native/system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/library/time.py` & `macal-5.5.0a3/src/macal/runtime/native/time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/menvironment.py` & `macal-5.5.0a3/src/macal/runtime/menvironment.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     IRuntimeValue,
     BooleanValue,
     NilValue,
     NativeFunctionValue,
     ValueType,
 )
 
-from macal.runtime.library.time import ms_timer, ns_timer
-from macal.runtime.library.system import Print, ShowVersion
+from macal.runtime.native.time import ms_timer, ns_timer
+from macal.runtime.native.system import Print, ShowVersion
 from macal.runtime.mimporter import ModuleInfo, ModuleImport
 from macal.mexceptions import RuntimeError, RuntimeErrorLC
 from macal.frontend.ast.metadata import NodeMetadata
 import json
 
 
 class Env:
@@ -57,14 +57,25 @@
         self.constants: list[str] = []
         self.is_in_loop = False
         self.is_in_function = False
         self.is_in_switch = False
         self.external_modules: Dict[str, ModuleInfo] = {}
         self.libraries: Dict[str, Env] = {}
 
+    def reset(self) -> None:  # reset is used by repl to reset the environment
+        self.variables = {}
+        self.constants = []
+        self.is_in_loop = False
+        self.is_in_function = False
+        self.is_in_switch = False
+        self.external_modules = {}
+        self.libraries = {}
+        if self.parent is not None:
+            self.parent.reset()
+
     def create_child_env(self, name: Optional[str] = "Local") -> Env:
         child = Env(self, name)
         child.is_in_function = self.is_in_function
         child.is_in_loop = self.is_in_loop
         self.is_in_switch = self.is_in_switch
         return child
```

### Comparing `macal-5.5.0a1/src/macal/runtime/mimporter.py` & `macal-5.5.0a3/src/macal/runtime/mimporter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/minterpreter.py` & `macal-5.5.0a3/src/macal/runtime/minterpreter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/value_type.py` & `macal-5.5.0a3/src/macal/runtime/value_type.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/src/macal/runtime/values.py` & `macal-5.5.0a3/src/macal/runtime/values.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a1/tests/test.py` & `macal-5.5.0a3/tests/test.py`

 * *Files identical despite different names*

