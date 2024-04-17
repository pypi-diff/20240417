# Comparing `tmp/cmind-2.1.0.tar.gz` & `tmp/cmind-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.1.0.tar", last modified: Tue Apr 16 14:54:06 2024, max compression
+gzip compressed data, was "cmind-2.1.1.tar", last modified: Tue Apr 16 17:56:09 2024, max compression
```

## Comparing `cmind-2.1.0.tar` & `cmind-2.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 14:53:52.000000 cmind-2.1.0/LICENSE.CK.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 14:53:52.000000 cmind-2.1.0/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 14:54:06.513303 cmind-2.1.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9978 2024-04-16 14:53:52.000000 cmind-2.1.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/ckx/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    37831 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    22835 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1293 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-16 14:54:06.513303 cmind-2.1.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2898 2024-04-16 14:53:52.000000 cmind-2.1.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 17:55:55.000000 cmind-2.1.1/LICENSE.CK.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 17:55:55.000000 cmind-2.1.1/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 17:56:09.195616 cmind-2.1.1/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9978 2024-04-16 17:55:55.000000 cmind-2.1.1/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.185615 cmind-2.1.1/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.185615 cmind-2.1.1/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/automation/ckx/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/ckx/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/ckx/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/ckx/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    38133 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    23378 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-16 17:55:55.000000 cmind-2.1.1/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 17:56:09.195616 cmind-2.1.1/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1293 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-16 17:56:09.000000 cmind-2.1.1/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-16 17:56:09.195616 cmind-2.1.1/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2927 2024-04-16 17:55:55.000000 cmind-2.1.1/setup.py
```

### Comparing `cmind-2.1.0/LICENSE.CK.md` & `cmind-2.1.1/LICENSE.CK.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/LICENSE.md` & `cmind-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/PKG-INFO` & `cmind-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.1.0
+Version: 2.1.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.1.0/README.md` & `cmind-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/artifact.py` & `cmind-2.1.1/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/automation.py` & `cmind-2.1.1/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/cli.py` & `cmind-2.1.1/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/config.py` & `cmind-2.1.1/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/core.py` & `cmind-2.1.1/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/index.py` & `cmind-2.1.1/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/net.py` & `cmind-2.1.1/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/automation/README.md` & `cmind-2.1.1/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/automation/module.py` & `cmind-2.1.1/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.1.1/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/automation/module_misc.py` & `cmind-2.1.1/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/ckx/README.md` & `cmind-2.1.1/cmind/repo/automation/ckx/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/ckx/module.py` & `cmind-2.1.1/cmind/repo/automation/ckx/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/core/README.md` & `cmind-2.1.1/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/core/module.py` & `cmind-2.1.1/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/repo/README.md` & `cmind-2.1.1/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repo/automation/repo/module.py` & `cmind-2.1.1/cmind/repo/automation/repo/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
           (pat) (str): Personal Access Token (if supported and url=='')
           (branch) (str): Git branch
           (checkout) (str): Git checkout
           (checkout_only) (bool): only checkout existing repo
           (depth) (int): Git depth
           (desc) (str): brief repository description (1 line)
           (prefix) (str): extra directory to keep CM artifacts
+          (skip_zip_parent_dir) (bool): skip parent dir in CM ZIP repo (useful when 
+                                        downloading CM repo archives from GitHub)
 
         Returns:
           (CM return dict):
 
           * return (int): return code == 0 if no error and >0 if error
           * (error) (str): error string if return>0
 
@@ -46,14 +48,15 @@
         alias = i.get('artifact','')
         url = i.get('url','')
         desc = i.get('desc','')
         prefix = i.get('prefix','')
         pat = i.get('pat','')
 
         checkout_only = i.get('checkout_only', False)
+        skip_zip_parent_dir = i.get('skip_zip_parent_dir', False)
 
         if url == '':
             if alias != '':
                 url = self.cmind.cfg['repo_url_prefix']
 
                 if '@' not in alias:
                     alias = self.cmind.cfg['repo_url_org'] + '@' + alias
@@ -136,15 +139,16 @@
                             branch = branch,
                             checkout = checkout,
                             console = console,
                             desc=desc,
                             prefix=prefix,
                             depth=depth,
                             path_to_repo=path_to_repo,
-                            checkout_only=checkout_only)
+                            checkout_only=checkout_only,
+                            skip_zip_parent_dir=skip_zip_parent_dir)
              if r['return']>0: return r
 
              repo_meta = r['meta']
 
              repo_metas[alias] = repo_meta
 
         if len(pull_repos)>0 and self.cmind.use_index:
```

### Comparing `cmind-2.1.0/cmind/repo.py` & `cmind-2.1.1/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind/repos.py` & `cmind-2.1.1/cmind/repos.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,29 +248,33 @@
 
             # Reload repos
             self.load(init=True)
 
         return {'return':0}
 
     ############################################################
-    def pull(self, alias, url = '', branch = '', checkout = '', console = False, desc = '', prefix = '', depth = None, path_to_repo = None, checkout_only = False):
+    def pull(self, alias, url = '', branch = '', checkout = '', console = False, desc = '', prefix = '', depth = None, 
+                    path_to_repo = None, checkout_only = False, skip_zip_parent_dir = False):
         """
         Clone or pull CM repository
 
         Args:
             alias (str): CM repository alias
             (url) (str): Git repository URL
             (branch) (str): Git repository branch
             (checkout) (str): Git repository checkout
            (checkout_only) (bool): only checkout existing repo
             (depth) (int): Git repository depth
             (console) (bool): if True, print some info to console
             (desc) (str): optional repository description
             (prefix) (str): sub-directory to be used inside this CM repository to store artifacts
             (path_to_repo) (str): force path to repo (useful to pull imported repos with non-standard path)
+            (checkout_only) (bool): only checkout Git repository but don't pull
+            (skip_zip_parent_dir) (bool): skip parent dir in CM ZIP repo (useful when 
+                                          downloading CM repo archives from GitHub)
 
         Returns: 
             (CM return dict):
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
 
@@ -366,18 +370,27 @@
             files=repo_pack_zip.namelist()
 
             repo_path = path_to_repo
 
             if console:
                 print ('Unpacking {} to {} ...'.format(pack_file, repo_path))
 
+            parent_dir = ''
+            
             # Unpacking zip
             for f in files:
                 if not f.startswith('..') and not f.startswith('/') and not f.startswith('\\'):
-                    file_path = os.path.join(repo_path, f)
+
+                    if skip_zip_parent_dir and parent_dir == '':
+                        parent_dir = f
+
+                    ff = f[len(parent_dir):] if parent_dir != '' else f
+                    
+                    file_path = os.path.join(repo_path, ff)
+
                     if f.endswith('/'):
                         # create directory
                         if not os.path.exists(file_path):
                             os.makedirs(file_path)
                     else:
                         dir_name = os.path.dirname(file_path)
                         if not os.path.exists(dir_name):
```

### Comparing `cmind-2.1.0/cmind/utils.py` & `cmind-2.1.1/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/cmind.egg-info/PKG-INFO` & `cmind-2.1.1/cmind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.1.0
+Version: 2.1.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.1.0/cmind.egg-info/SOURCES.txt` & `cmind-2.1.1/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-2.1.0/setup.py` & `cmind-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     package_data={'cmind': repo_dirs},
 
     cmdclass={
         'install': custom_install
     },
 
-    install_requires=['pyyaml', 'requests'],
+    install_requires=['pyyaml', 'requests', 'setuptools', 'giturlparse'],
 
     entry_points={"console_scripts": [
                       "cmind = cmind.cli:run",
                       "cm = cmind.cli:run",
                       "cmr = cmind.cli:run_script",
                       "cmrd = cmind.cli:docker_script",
                       "cmg = cmind.cli:gui_script",
```

